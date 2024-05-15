# Comparing `tmp/acetone_nnet-0.2.3.tar.gz` & `tmp/acetone_nnet-0.2.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.2.3.tar", last modified: Tue May 14 08:11:16 2024, max compression
+gzip compressed data, was "acetone_nnet-0.2.3.dev1.tar", last modified: Wed May 15 08:22:38 2024, max compression
```

## Comparing `acetone_nnet-0.2.3.tar` & `acetone_nnet-0.2.3.dev1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.626575 acetone_nnet-0.2.3/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.3/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6679 2024-05-14 08:11:16.626575 acetone_nnet-0.2.3/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.2.3/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2065 2024-05-14 08:10:46.000000 acetone_nnet-0.2.3/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-14 08:11:16.626575 acetone_nnet-0.2.3/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.586562 acetone_nnet-0.2.3/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.696564 acetone_nnet-0.2.3/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1801 2024-05-13 12:52:48.000000 acetone_nnet-0.2.3/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.715564 acetone_nnet-0.2.3/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.3/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-19 14:05:22.000000 acetone_nnet-0.2.3/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.2.3/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.751564 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-05-13 12:08:36.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4742 2024-05-06 12:16:27.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.926566 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3217 2024-05-06 13:03:06.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.064568 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1678 2024-04-23 14:51:52.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-04-18 12:32:50.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1683 2024-04-23 14:51:35.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1694 2024-04-23 14:51:42.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1693 2024-04-23 14:51:25.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.089568 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-05-13 09:26:47.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8205 2024-05-13 07:02:54.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.144569 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.163570 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.209570 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10588 2024-05-06 08:24:39.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6667 2024-05-06 08:24:16.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6085 2024-05-13 06:58:55.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5128 2024-05-06 08:24:06.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25546 2024-05-14 07:43:39.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.210570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.210570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18466 2024-05-14 07:01:26.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.226570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7452 2024-04-18 15:31:47.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14538 2024-05-14 06:56:48.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.233570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3871 2024-05-13 14:43:41.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5370 2024-05-14 07:02:59.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.234570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    30296 2024-05-14 07:20:12.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4461 2024-05-13 14:13:26.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2907 2024-05-13 13:34:22.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.250571 acetone_nnet-0.2.3/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.372572 acetone_nnet-0.2.3/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.488573 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.525574 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.566574 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-05-13 08:47:21.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-05-13 08:47:14.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-05-13 13:12:23.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-05-13 08:47:28.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.568575 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.597575 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.610575 acetone_nnet-0.2.3/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.621575 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1244 2024-05-06 08:26:40.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.625575 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6679 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6926 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.515886 acetone_nnet-0.2.3.dev1/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.3.dev1/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3.dev1/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3.dev1/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-15 08:22:38.515886 acetone_nnet-0.2.3.dev1/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.2.3.dev1/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-15 08:22:19.000000 acetone_nnet-0.2.3.dev1/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-15 08:22:38.515886 acetone_nnet-0.2.3.dev1/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.154882 acetone_nnet-0.2.3.dev1/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.200882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1801 2024-05-13 12:52:48.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.201882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2822 2024-05-15 08:16:02.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.201882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-15 06:49:54.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4946 2024-05-15 06:49:14.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.203882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2874 2024-05-15 07:11:48.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3371 2024-05-15 07:10:42.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.205882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1708 2024-05-15 08:12:43.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5004 2024-05-15 08:12:08.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1713 2024-05-15 08:12:54.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1724 2024-05-15 08:13:23.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1723 2024-05-15 08:13:39.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4095 2024-05-15 07:08:03.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.206882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3891 2024-05-15 08:07:41.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-05-15 08:09:29.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3063 2024-05-15 07:07:25.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4691 2024-05-15 07:06:26.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2401 2024-05-15 07:05:22.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4046 2024-05-15 07:04:47.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8308 2024-05-15 07:02:42.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2313 2024-05-15 06:57:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3290 2024-05-15 06:56:35.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.208882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2705 2024-05-15 08:01:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.208882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5096 2024-05-15 07:56:21.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.209882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10875 2024-05-15 07:49:14.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6712 2024-05-15 07:39:10.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5193 2024-05-15 07:37:13.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2193 2024-05-15 06:51:30.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26988 2024-05-15 06:38:26.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.210883 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.210883 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18659 2024-05-15 06:28:43.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.210883 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14558 2024-05-14 15:18:40.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.211882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5379 2024-05-14 15:15:39.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.211882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    31813 2024-05-14 15:14:48.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-14 14:54:21.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.211882 acetone_nnet-0.2.3.dev1/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.277883 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.360884 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.412885 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.444885 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-05-13 08:47:21.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-05-13 08:47:14.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-05-13 13:12:23.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-05-13 08:47:28.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.452885 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.486886 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.499886 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.511886 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1244 2024-05-06 08:26:40.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 08:22:38.514886 acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-15 08:22:38.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6926 2024-05-15 08:22:38.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-15 08:22:38.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-15 08:22:38.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-15 08:22:38.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-15 08:22:38.000000 acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.2.3/AUTHORS.md` & `acetone_nnet-0.2.3.dev1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/COPYING` & `acetone_nnet-0.2.3.dev1/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/LICENSE` & `acetone_nnet-0.2.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/PKG-INFO` & `acetone_nnet-0.2.3.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2.3
+Version: 0.2.3.dev1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.2.3/README.md` & `acetone_nnet-0.2.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/pyproject.toml` & `acetone_nnet-0.2.3.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.2.3"
+version = "0.2.3.dev1"
 requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/cli_acetone.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 
 import argparse
 import pathlib
 
 from .code_generator.neural_network import CodeGenerator
 
-def cli_acetone(model_file, function_name, nb_tests, conv_algorithm, output_dir, test_dataset_file=None, normalize=False ):
+def cli_acetone(model_file:str, function_name:str, nb_tests:int, conv_algorithm:str, output_dir:str, test_dataset_file:str|None=None, normalize:bool=False ):
     normalize = bool(normalize)
     print(normalize)
     print("C CODE GENERATOR FOR NEURAL NETWORKS")
 
     pathlib.Path(output_dir).mkdir(parents=True, exist_ok=True)
 
     net = CodeGenerator(file = model_file, test_dataset_file = test_dataset_file, function_name = function_name, nb_tests = nb_tests, conv_algorithm = conv_algorithm, normalize = normalize)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/cli_compare.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,36 +22,36 @@
 import argparse
 import numpy as np
 
 # Source document for floating comparison
 # https://floating-point-gui.de/errors/comparison/
 
 
-def compare_floats(a, b, epsilon = (128*sys.float_info.epsilon), abs_th = sys.float_info.min):
+def compare_floats(a:float|int, b:float|int, epsilon:float=(128*sys.float_info.epsilon), abs_th:float=sys.float_info.min):
     diff = abs(a-b) 
     if a == b:
         return True, diff
 
     else:
         norm = min((abs(a)+abs(b)), (sys.float_info.max))
         if diff < max(abs_th, epsilon * norm):
             return True, diff
         else: 
             return False, diff
 
-def preprocess_line(line, precision):
+def preprocess_line(line:list, precision:str):
     line = line.split(' ')
     line[:] = [x for x in line if x.strip()]
     if precision == 'double':
         line = list(map(np.float64,line))
     elif precision == 'float':
         line = list(map(np.float32,line))  
     return line 
 
-def compare_lines(line_f1, line_f2, precision):
+def compare_lines(line_f1:list, line_f2:list, precision:str):
 
     line_f1 = preprocess_line(line_f1, precision)
     line_f2 = preprocess_line(line_f2, precision)
     max_diff = 0
     length = len(line_f1)
 
     for j in range(length): 
@@ -61,15 +61,15 @@
 
     if comparison:
         return True, max_diff
     else:
         return False, max_diff
 
 
-def compare_files(file1, file2, nb_tests, precision):
+def compare_files(file1:str, file2:str, nb_tests:int, precision:str):
     f1 = open(file1, 'r')
     f2 = open(file2, 'r')
 
     line_counter = 0
     max_diff_file = 0
 
 
@@ -89,15 +89,15 @@
 
     if comparison:
         return True, max_diff_file
         
     else: 
         return False, max_diff_file
 
-def cli_compare(reference_file, c_file, nb_tests, precision):
+def cli_compare(reference_file:str, c_file:str, nb_tests:int, precision:str):
     _, max_diff_file = compare_files(reference_file, c_file, nb_tests, precision)
     
     print("   Max absolute error for %s test(s): %s" % (nb_tests, max_diff_file))
 
 
 if __name__ == "__main__":
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/Layer.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,20 +43,20 @@
     def generate_inference_code_layer(self):
         pass
 
     @abstractmethod
     def forward_path_layer(self):
         pass
 
-    def count_elements_array(self, array):
+    def count_elements_array(self, array:np.ndarray):
         nb_elements = 1
         for dim in np.shape(array) : nb_elements *= dim
         return nb_elements
 
-    def compute_padding(self,padding, in_height, in_width, kernel_h, kernel_w, strides, dilation_rate=1):
+    def compute_padding(self,padding:str|list, in_height:int, in_width:int, kernel_h:int, kernel_w:int, strides:int, dilation_rate:int=1):
         if(type(padding) == str):
             # Compute 'same' padding tensorflow
 
             filter_height = (kernel_h - (kernel_h-1)*(dilation_rate-1))
             filter_width = (kernel_w - (kernel_w-1)*(dilation_rate-1))
 
             # The total padding applied along the height and width is computed as:
@@ -84,15 +84,15 @@
                     pad_left = pad_along_width - pad_right        
         else:
             pad_right, pad_left, pad_bottom, pad_top = padding[3], padding[1], padding[2], padding[0]
             
         return pad_right, pad_left, pad_bottom, pad_top
     
     #Give to the layer an string saying were the output will be saved (either in a 'cst' or in an 'output_road')
-    def find_output_str(self,dict_cst):
+    def find_output_str(self, dict_cst:dict):
         #dict_cst is the dict linking an layer to the cst in which the must be saved if needed
         
         #either it has to be saved
         if(self in dict_cst):
             output_str = 'cst_'+str(dict_cst[self])
         #Or it can directly go to the next layer
         else:
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,143 +23,145 @@
 
 class ActivationFunctions():
     def __init__(self):
         self.name = ''
         self.comment = ''
 
     @abstractmethod
-    def compute():
+    def compute(self, z:np.ndarray):
         pass
 
     @abstractmethod
-    def write_activation_str(local_var):
+    def write_activation_str(self, local_var:str):
         pass
 
 class Sigmoid(ActivationFunctions):
     
     def __init__(self):
         super().__init__()
         self.name = 'sigmoid'
         self.comment = ' and apply sigmoid function'
         #self.layer_type
 
-    def compute(self, z):
+    def compute(self, z:np.ndarray):
         return 1/(1+np.exp(-z))
 
-    def write_activation_str(self, local_var):
+    def write_activation_str(self, local_var:str):
 
         s = '1 / (1 + exp(-'+ local_var +'))'
         
         return s
 
 class ReLu(ActivationFunctions):
     
     def __init__(self):
         super().__init__()
         self.name = 'relu'
         self.comment = ' and apply rectifier'
     
-    def compute(self, z):
+    def compute(self, z:np.ndarray):
         return np.maximum(0,z)
 
-    def write_activation_str(self, local_var):
+    def write_activation_str(self, local_var:str):
 
         s = local_var +' > 0 ? '+ local_var +' : 0' # output = condition ? value_if_true : value_if_false
         
         return s
 
 class LeakyReLu(ActivationFunctions):
     
-    def __init__(self,alpha):
+    def __init__(self, alpha:float):
         super().__init__()
         self.name = 'leakyrelu'
         self.comment = ' and apply rectifier'
         self.alpha = alpha
+
+        assert self.alpha > 0
     
-    def compute(self, z):
+    def compute(self, z:np.ndarray):
         temp_tensor = z.flatten()
         for i in range(len(temp_tensor)):
             if(temp_tensor[i]<0):
                 temp_tensor[i] =  self.alpha*temp_tensor[i]
         return temp_tensor.reshape(z.shape)
 
-    def write_activation_str(self, local_var):
+    def write_activation_str(self, local_var:str):
 
         s = local_var +' > 0 ? '+ local_var +' : '+str(self.alpha)+'*'+local_var # output = condition ? value_if_true : value_if_false
         
         return s
 
 class TanH(ActivationFunctions):
     def __init__(self):
         super().__init__()
         self.name = 'hyperb_tan'
         self.comment = ' and apply hyperbolic tangent function'
         
     
-    def compute(self, z):
+    def compute(self, z:np.ndarray):
         return (np.exp(z)-np.exp(-z))/(np.exp(z)+np.exp(-z))
 
-    def write_activation_str(self, local_var):
+    def write_activation_str(self, local_var:str):
 
         s = '(exp('+ local_var +')-exp(-'+ local_var +'))/(exp('+ local_var +')+exp(-'+ local_var +'))'
         
         return s
 
 class Linear(ActivationFunctions):
     def __init__(self):
         super().__init__()
         self.name = 'linear'
         self.comment = ''
     
-    def compute(self, z):
+    def compute(self, z:np.ndarray):
         return z
 
-    def write_activation_str(self, local_var):
+    def write_activation_str(self, local_var:str):
 
         s = local_var
         
         return s
     
 class Exponential(ActivationFunctions):
     def __init__(self):
         super().__init__()
         self.name = 'Exponential'
         self.comment = ' and apply exponential function'
     
-    def compute(self, z):
+    def compute(self, z:np.ndarray):
         return np.exp(z)
     
-    def write_activation_str(self, local_var):
+    def write_activation_str(self, local_var:str):
 
         s = 'exp('+local_var+')'
 
         return s
     
 class Logarithm(ActivationFunctions):
     def __init__(self):
         super().__init__()
         self.name = 'Logarithm'
         self.comment = ' and apply logarithm function'
     
-    def compute(self, z):
+    def compute(self, z:np.ndarray):
         return np.log(z)
     
-    def write_activation_str(self, local_var):
+    def write_activation_str(self, local_var:str):
         
         s = 'log('+local_var+')'
         
         return s
 
 class Clip(ActivationFunctions):
-    def __init__(self,max,min):
+    def __init__(self, max:float|int, min:float|int):
         super().__init__()
         self.name = 'Clip'
         self.comment = ' and apply rectifier'
         self.max = max
         self.min = min
     
-    def compute(self, z):
+    def compute(self, z:np.ndarray):
         return np.clip(z,self.min,self.max)
     
     def write_activation_str(self,local_var):
         s = local_var +' > '+str(self.max)+' ? '+ str(self.max) +' : (' + local_var + ' < ' + str(self.min) + ' ? ' + str(self.min) + ' : ' + local_var + ')'
         return s
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,21 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
+from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 class Add_Bias(Layer):
 
-    def __init__(self, idx, size, biases,activation_function):
+    def __init__(self, idx:int, size:int, biases:int, activation_function:ActivationFunctions):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Add_Biass'
         self.biases = np.asarray(biases)
         self.nb_biases = self.count_elements_array(self.biases)
@@ -57,11 +58,11 @@
 
         with open(self.template_path+'layers/template_AddBiase.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.previous_layer[0].size)
 
         return self.activation_function.compute(input + self.biases)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,21 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
+from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 class BatchNormalization(Layer):
 
-    def __init__(self, idx, size, input_shape, epsilon, scale, biases, mean, var, activation_function):
+    def __init__(self, idx:int, size:int, input_shape:list, epsilon:float|int, scale:np.ndarray, biases:np.ndarray, mean:np.ndarray, var:np.ndarray, activation_function:ActivationFunctions):
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'BatchNormalization'
         self.output_channels = input_shape[1]
         self.output_height = input_shape[2]
         self.output_width = input_shape[3]
@@ -62,13 +63,13 @@
 
         with open(self.template_path+'layers/template_BatchNormalization.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
-    def forward_path_layer(self,input):
+    def forward_path_layer(self, input:np.ndarray):
         input = np.reshape(input, (self.output_channels, self.output_height, self.output_width))
         output = []
         for i in range(self.output_channels):
             output.append((input[i] - self.mean[i])/np.sqrt(self.var[i] + self.epsilon)*self.scale[i] + self.biases[i])
         return np.array(output)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,29 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
+import numpy as np
 
-#Addition of several tensor
-class Add(Broadcast):
+#Multiplication of several tensors
+class Multiply(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Add'
-        self.specific_operator = ' + '
+        self.name = 'Multiply'
+        self.specific_operator = '*'
     
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         if(self.constant is None):
-            constant = 0
+            constant = 1
         else: 
             constant = self.constant
         if(len(self.previous_layer) > 1):
             output = inputs[0]
             for input in inputs[1:]:
-                output += input
+                output *= input
         else:
             output = inputs
-        return self.activation_function.compute(output+constant)
+        return self.activation_function.compute(constant*output)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,21 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
+import numpy as np
 
 #Return a tensor with where each position (f,i,j) contains the average of all the values at position (f,i,j) in each tensor
 class Average(Broadcast):
     def __init__(self,**kwargs):
         super().__init__(**kwargs)
         self.name = 'Average'
         self.specific_operator = ' + '
 
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         output = inputs[0]
         for input in inputs[1:]:
             output +=input 
         return self.activation_function.compute(output/(len(inputs)))
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,25 +15,26 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ...Layer import Layer
+from ...activation_functions import ActivationFunctions
 
 from abc import abstractmethod
 import pystache
 import numpy as np
 
 #The class of the Layers which compute operation with broadcast numpy style
 #attribut: none
 #input: a list of tensor
 #output: the resultant tensor
 class Broadcast(Layer):
-    def __init__(self, idx, size, input_shapes, output_shape,activation_function, constant = None):
+    def __init__(self, idx:int, size:int, input_shapes:list, output_shape:list, activation_function:ActivationFunctions, constant:np.ndarray|float|int|None=None):
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = ''
         self.input_shapes = input_shapes
         
         self.output_height = output_shape[2]
@@ -106,9 +107,9 @@
         with open(self.template_path+'layers/template_Broadcast.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     @abstractmethod
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         pass
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,25 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
+import numpy as np
 
 #Division of several tensors
 class Divide(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = 'Divide'
         self.specific_operator = '/'
     
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         if(self.constant is None):
             constant = 1
         else: 
             constant = self.constant
         if(len(self.previous_layer) > 1):
             output = inputs[0]
             for input in inputs[1:]:
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,22 +15,21 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
-
 import numpy as np
 
 #Return a tensor with where each position (f,i,j) contains the max of all the values at position (f,i,j) in each tensor
 class Maximum(Broadcast):
     def __init__(self,**kwargs):
         super().__init__(**kwargs)
         self.name = 'Maximum'
         self.specific_operator = ', '
 
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         maxi = inputs[0]
         for input in inputs[1:]:
             maxi = np.maximum(maxi, input)
         return self.activation_function.compute(maxi)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,21 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
-
 import numpy as np
 
 #Return a tensor with where each position (f,i,j) contains the min of all the values at position (f,i,j) in each tensor
 class Minimum(Broadcast):
     def __init__(self,**kwargs):
         super().__init__(**kwargs)
         self.name = 'Minimum'
         self.specific_operator = ', '
 
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         mini = inputs[0]
         for input in inputs[1:]:
             mini = np.minimum(mini, input)
         return self.activation_function.compute(mini)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,29 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
+import numpy as np
 
-#Multiplication of several tensors
-class Multiply(Broadcast):
+#Subtraction of several tensors
+class Subtract(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Multiply'
-        self.specific_operator = '*'
+        self.name = 'Subtract'
+        self.specific_operator = ' - '
     
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         if(self.constant is None):
-            constant = 1
+            constant = 0
         else: 
             constant = self.constant
         if(len(self.previous_layer) > 1):
             output = inputs[0]
             for input in inputs[1:]:
-                output *= input
+                output -= input
         else:
             output = inputs
-        return self.activation_function.compute(constant*output)
+        return self.activation_function.compute(output-constant)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,28 +15,29 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
+import numpy as np
 
-#Subtraction of several tensors
-class Subtract(Broadcast):
+#Addition of several tensor
+class Add(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Subtract'
-        self.specific_operator = ' - '
+        self.name = 'Add'
+        self.specific_operator = ' + '
     
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         if(self.constant is None):
             constant = 0
         else: 
             constant = self.constant
         if(len(self.previous_layer) > 1):
             output = inputs[0]
             for input in inputs[1:]:
-                output -= input
+                output += input
         else:
             output = inputs
-        return self.activation_function.compute(output-constant)
+        return self.activation_function.compute(output+constant)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,23 +15,24 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
+from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 #Concatenate two tensor alongside a given axis
 #attribut: axis alongside of which the concatenation will be done
 #input: a list of tensor to concatenate
 #output: the concatenated tensor 
 class Concatenate(Layer):
-    def __init__(self, idx, size, axis, input_shapes,output_shape,activation_function):
+    def __init__(self, idx:int, size:int, axis:int, input_shapes:list, output_shape:list, activation_function:ActivationFunctions):
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shapes = input_shapes
         self.name = 'Concatenate'
         self.axis = axis
         self.output_height = output_shape[2]
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,21 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ...Layer import Layer
-
+from ...activation_functions import ActivationFunctions
 import numpy as np
 from abc import abstractmethod
 
 class Conv2D(Layer):
     
-    def __init__(self, idx, conv_algorithm, size, padding, strides, kernel_h, kernel_w, dilation_rate, nb_filters, input_shape, output_shape, weights, biases, activation_function):
+    def __init__(self, idx:int, conv_algorithm:str, size:int, padding:str|list, strides:int, kernel_h:int, kernel_w:int, dilation_rate:int, nb_filters:int, input_shape:list, output_shape:list, weights:np.ndarray, biases:np.ndarray, activation_function:ActivationFunctions):
         super().__init__()
         self.conv_algorithm = conv_algorithm
         self.idx = idx
         self.size = size
         self.name = 'Conv2D'
         self.padding = padding
         self.strides = strides
@@ -43,28 +43,28 @@
         self.input_width = input_shape[3]
         self.output_height = output_shape[2]
         self.output_width = output_shape[3]
 
         self.input_shape = [self.input_channels, self.input_height, self.input_width]
         self.output_channels = self.nb_filters
 
-        self.weights = np.asarray(weights)
-        self.biases = np.asarray(biases)
+        self.weights = weights
+        self.biases = biases
         self.activation_function = activation_function
         self.local_var = 'sum'
 
         self.nb_weights = self.count_elements_array(self.weights)
         self.nb_biases = self.count_elements_array(self.biases)
         self.pad_right, self.pad_left, self.pad_bottom, self.pad_top = self.compute_padding(self.padding,self.input_height, self.input_width, self.kernel_h, self.kernel_w, self.strides, self.dilation_rate)
     
     @abstractmethod
     def generate_inference_code_layer(self):
         pass
 
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         # Conv for chw
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
         
         output = np.zeros((self.nb_filters, self.output_height, self.output_width))
         print(self.weights.shape)
 
         if self.pad_right and self.pad_left and self.pad_top and self.pad_bottom:
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         self.conv_algorithm = self.conv_algorithm[-7:]
         self.algo_gemm_mapping = { 'gemm_nn' : self.write_gemm_nn,
                                    'gemm_nt' : self.write_gemm_nt,
                                    'gemm_tn' : self.write_gemm_tn,
                                    'gemm_tt' : self.write_gemm_tt}
 
-    def write_gemm_nn(self, m, n, k, A, B, C, direct):
+    def write_gemm_nn(self, m:int, n:int, k:int, A:str, B:str, C:str, direct:bool):
 
         mustach_hash = {}
 
         mustach_hash['direct'] = direct
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['m'] = m
@@ -61,15 +61,15 @@
 
         with open(self.template_path+'layers/Conv/template_Conv_gemm_nn.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
-    def write_gemm_nt(self, m, n, k, A, B, C, direct):
+    def write_gemm_nt(self, m:int, n:int, k:int, A:str, B:str, C:str, direct:bool):
 
         mustach_hash = {}
 
         mustach_hash['direct'] = direct
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['m'] = m
@@ -90,15 +90,15 @@
 
         with open(self.template_path+'layers/Conv/template_Conv_gemm_nt.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
-    def write_gemm_tn(self, m, n, k, A, B, C, direct):
+    def write_gemm_tn(self, m:int, n:int, k:int, A:str, B:str, C:str, direct:bool):
 
         mustach_hash = {}
 
         mustach_hash['direct'] = direct
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['m'] = m
@@ -119,15 +119,15 @@
 
         with open(self.template_path+'layers/Conv/template_Conv_gemm_tn.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
-    def write_gemm_tt(self, m, n, k, A, B, C, direct):
+    def write_gemm_tt(self, m:int, n:int, k:int, A:str, B:str, C:str, direct:bool):
 
         mustach_hash = {}
 
         mustach_hash['direct'] = direct
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['m'] = m
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,27 +15,28 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
+from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 class Dense(Layer):
 
-    def __init__(self, idx, size, weights, biases, activation_function):
+    def __init__(self, idx:int, size:int, weights:np.ndarray, biases:np.ndarray, activation_function:ActivationFunctions):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Dense'
-        self.weights = np.asarray(weights)
-        self.biases = np.asarray(biases)
+        self.weights = weights
+        self.biases = biases
         self.activation_function = activation_function
         self.local_var = 'dotproduct'
         
         self.nb_weights = self.count_elements_array(self.weights)
         self.nb_biases = self.count_elements_array(self.biases)
 
         
@@ -64,10 +65,10 @@
         
         with open(self.template_path+'layers/template_Dense.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.previous_layer[0].size)
         return self.activation_function.compute(np.dot(input, self.weights) + self.biases)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,25 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
+from..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 
 #Do the dotproduct of two tensors
 #atribut: the axis alongside of which the dot product will be done. if type(axis) == int, same axis for the two tensor. can be tuples of axis (element i of axis represent axis of tensor i)
 #input: two tensor
 #output: the resultant tensor 
 class Dot(Layer):
-    def __init__(self, idx, size, axis, input_shapes,output_shape,activation_function):
+    def __init__(self, idx:int, size:int, axis:int|list, input_shapes:list, output_shape:list, activation_function:ActivationFunctions):
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shapes = input_shapes
         self.name = 'Dot'
         #we seek a tuple of axis
         if (type(axis) == int):
@@ -81,12 +82,12 @@
         
         with open(self.template_path+'layers/template_Dot.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
-    def forward_path_layer(self, inputs):
+    def forward_path_layer(self, inputs:np.ndarray):
         inputs[0] = inputs[0].reshape(self.input_shapes[0][1],self.input_shapes[0][2],self.input_shapes[0][3])
         inputs[1] = inputs[1].reshape(self.input_shapes[1][1],self.input_shapes[1][2],self.input_shapes[1][3])
         output = np.tensordot(inputs[0],inputs[1],axes=[self.axis[0]-1,self.axis[1]-1])
         return self.activation_function.compute(output)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 
 from ..Layer import Layer
 import pystache
 import numpy as np
 
 class Flatten(Layer):
 
-    def __init__(self, idx, size, input_shape, data_format):
+    def __init__(self, idx:int, size:int, input_shape:int, data_format:str):
        
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shape = input_shape
         self.data_format = data_format
-        self.name = 'Input_layer'
+        self.name = 'Flatten'
 
     def generate_inference_code_layer(self):
 
         mustach_hash = {}
 
         if(self.data_format == 'channels_last'):
             mustach_hash['channels_last'] = True
@@ -49,12 +49,12 @@
 
         with open(self.template_path+'layers/template_Flatten.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         if(self.data_format == 'channels_last'):
             return np.transpose(np.reshape(input,self.input_shape[1:]),(1,2,0))
         else:
             return input
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,25 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
+from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 #extract a list of subtensor from a given tensor
 #attribut: axis alongside of which the submatrix will be extracted (if the desired submatrix must have the height, width or channels of the parent tensor)
 #input: a tensor
 #output: a list of tensor
 class Gather(Layer):
     
-    def __init__(self, idx, size, axis,  indices, input_shape, output_shape,activation_function):
+    def __init__(self, idx:int, size:int, axis:int,  indices:list, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Gather'
         self.indices = indices
         self.axis = axis
@@ -82,10 +83,10 @@
 
         with open(self.template_path+'layers/template_Gather.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
         
-    def forward_path_layer(self,input):
+    def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.input_channels,self.input_height,self.input_width)
         return np.take(input, indices=self.indices, axis=self.axis-1)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,24 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
+from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 #The layer which compute the general matrix multiplication
 #input: weight tesnsor W and bias tensor B, input tensor T. The tensor must be of 2D
 #data: alpha and beta constante used in the operation, transpo un tuple saying if the tensor T or W must be transposed before the operation
 #output: The result of the operation """alpha*T*W + beta*B"""
 class Gemm(Layer):
-    def __init__(self, idx, size, alpha, beta, transA, transB, weights, bias, input_shape, output_shape,activation_function):
+    def __init__(self, idx:int, size:int, alpha:float|int, beta:float|int, transA:bool, transB:bool, weights:np.ndarray, bias:np.ndarray, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
         super().__init__() 
         self.name = 'Gemm'
         self.idx = idx
         self.size = size
         
         self.alpha = [alpha]
         self.beta =  [beta]
@@ -40,27 +41,26 @@
                              (0,1):self.write_gemm_nt,
                              (1,1):self.write_gemm_tt,
                              (1,0):self.write_gemm_tn}
         
         self.output_height = output_shape[2]
         self.output_width = output_shape[3]
         if(input_shape):
-            print(input_shape)
             if(transA):
                 self.input_height = input_shape[3]
                 self.input_width = input_shape[2]
             else:
                 self.input_height = input_shape[2]
                 self.input_width = input_shape[3]
         else:
             self.input_height = 1
             self.input_width = 1
         
-        self.weights = np.asarray(weights)
-        self.biases = np.asarray(bias)
+        self.weights = weights
+        self.biases = bias
         self.activation_function = activation_function
         self.nb_weights = self.count_elements_array(self.weights)
         self.nb_biases = self.count_elements_array(self.biases)
         
     #The various ways to compute the operation: 
     
     #None of the tensor ar transposed
@@ -164,15 +164,15 @@
 
         with open(self.template_path+'layers/Gemm/template_gemm_tt.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
-    def forward_path_layer(self,input):
+    def forward_path_layer(self, input:np.ndarray):
         if(self.transpo[0]):
             input = input.reshape(self.input_width,self.input_height).transpose()
         else:
             input = input.reshape(self.input_height,self.input_width)
             
         if(self.transpo[1]):
             self.weights = self.weights.transpose()
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,21 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
+import numpy as np
 from ..Layer import Layer
 import pystache
 
 class InputLayer(Layer):
 
-    def __init__(self, idx, size, input_shape, data_format):
+    def __init__(self, idx:int, size:int, input_shape:list, data_format:str):
        
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shape = input_shape
         self.data_format = data_format
         self.name = 'Input_layer'
@@ -53,10 +54,10 @@
 
         with open(self.template_path+'layers/template_Input_Layer.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         
         return input
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,20 +15,21 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
+from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 class MatMul(Layer):
 
-    def __init__(self, idx, size, input_shape, weights, side, activation_function):
+    def __init__(self, idx:int, size:int, input_shape:list, weights:list, side:bool, activation_function:ActivationFunctions):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'MatMul'
         self.weights = np.asarray(weights)
         self.activation_function = activation_function
@@ -68,10 +69,10 @@
         
     def forward_path_layer(self, input):
         
         input = input.reshape(self.previous_layer[0].size)
         if (self.side):
             weights = np.moveaxis(self.weights, 3,0)
             weights = np.reshape(weights, (weights.shape[1],weights.shape[2],weights.shape[3],weights.shape[0]))
-            return self.activation_function.compute((np.matmul(weights,input)))
+            return self.activation_function.compute(np.matmul(weights,input))
         else:
-            return self.activation_function.compute((np.matmul(input,self.weights)))
+            return self.activation_function.compute(np.matmul(input,self.weights))
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,42 +15,42 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ...Layer import Layer
-
+from ...activation_functions import ActivationFunctions
 import numpy as np
 from abc import abstractmethod
 
 #The Pad Layers
 #Pad alongside each dimmensions
 #attribut: the mode of padding required
 #input: a tensor to be padded, the desired pads, the value of teh constant if mode == constant
 #output:the resized tensor
 ######################### cf https://onnx.ai/onnx/operators/onnx__Pad.html for the doc
 class Pad(Layer):
     
-    def __init__(self, idx, size, pads, constant_value, axes, input_shape,activation_function):
+    def __init__(self, idx:int, size:int, pads:list, constant_value:float, axes:np.ndarray, input_shape:list, activation_function:ActivationFunctions):
         super().__init__()
         self.idx = idx
         self.size = size
         self.pads = pads
         self.constant_value = constant_value
         self.axes = axes
         self.name = 'Pad'
         self.input_shape = input_shape
         self.output_channels = input_shape[1] + pads[1] + pads[5]
         self.output_height = input_shape[2] + pads[2] + pads[6]
         self.output_width = input_shape[3] + pads[3] + pads[7]
         self.mode = ''
         self.activation_function = activation_function
     
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.input_shape[1], self.input_shape[2], self.input_shape[3])
         nb_dim = len(self.pads)//2
         pad_width = [(self.pads[i],self.pads[i+nb_dim]) for i in range(1,nb_dim)] #Constructing the pads accordingly to the numpy nomenclature
         return self.activation_function.compute(np.pad(input,pad_width=pad_width,mode=self.mode,constant_values=self.constant_value,))
     
     @abstractmethod
     def generate_inference_code_layer(self):
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,26 +28,19 @@
         
         self.name = 'AveragePooling2D'
         self.pooling_function = np.mean
         self.local_var = 'sum'
         self.local_var_2 = 'count'
         self.output_var = self.local_var + '/' + self.local_var_2
 
-    def declare_local_vars(self, data_type):
-        
-        s = '    '+ data_type + ' '+ self.local_var +';\n'
-        s += '    int '+ self.local_var_2 + ';\n\n'
-
-        return s
-
     def update_local_vars(self):
 
         s = self.local_var + ' = 0; '+ self.local_var_2 + ' = 0;\n'
   
         return s
 
-    def specific_function(self, index, input_of_layer):
+    def specific_function(self, index:str, input_of_layer:str):
         # Computes the average in this subclass AveragePooling2D 
         s = self.local_var+' += '+input_of_layer+'['+index+'];\n'
         s += '                            '+self.local_var_2+' ++;\n'
         
         return s
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,24 +27,18 @@
         super().__init__(**kwds)
         
         self.name = 'MaxPooling2D'
         self.pooling_function = np.amax
         self.local_var = 'max'
         self.output_var = self.local_var
 
-    def declare_local_vars(self, data_type):
-        
-        s = '    '+ data_type + ' '+ self.local_var +';\n\n'
-
-        return s
-
     def update_local_vars(self):
         
         s = self.local_var +' = -INFINITY;\n'
 
         return s
 
-    def specific_function(self, index, input_of_layer):
+    def specific_function(self, index:str, input_of_layer:str):
         s = 'if ('+input_of_layer+'['+index+'] > '+self.local_var+')\n'
         s += '                                '+self.local_var+' = '+input_of_layer+'['+index+'];\n'
     
         return s
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,21 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ...Layer import Layer
-
+from ...activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 from abc import abstractmethod
 
 class Pooling2D(Layer):
-    def __init__(self, idx, size, padding, strides, pool_size, input_shape, output_shape, activation_function,**kwargs):
+    def __init__(self, idx:int, size:int, padding:str|list, strides:int, pool_size:int, input_shape:list, output_shape:list, activation_function:ActivationFunctions, **kwargs):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = ''
         self.padding = padding
         self.strides = strides
@@ -49,15 +49,19 @@
         self.output_var = ''
 
         self.activation_function = activation_function
 
         self.pad_right, self.pad_left, self.pad_bottom, self.pad_top = self.compute_padding(self.padding,self.input_height, self.input_width, self.pool_size,self.pool_size, self.strides)
 
     @abstractmethod    
-    def specific_function(self, index, input_of_layer):
+    def specific_function(self, index:str, input_of_layer:str):
+        pass
+
+    @abstractmethod    
+    def update_local_vars(self):
         pass
 
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
@@ -88,15 +92,15 @@
         
         with open(self.template_path+'layers/template_Pooling2D.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
         
         output = np.zeros((self.input_channels, self.output_height, self.output_width))
                 
         if self.pad_right and self.pad_left and self.pad_top and self.pad_bottom:
             input_padded = np.zeros((self.input_channels, self.input_height + self.pad_top + self.pad_bottom, self.input_width + self.pad_left + self.pad_right))
             input_padded[:, self.pad_top:-self.pad_bottom, self.pad_left:-self.pad_right] = input
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,31 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ...Layer import Layer
+from ...activation_functions import ActivationFunctions
+import numpy as np
 from abc import abstractmethod
 
 #The resize Layers
 #Only Height and Width are resized
 #attribut: a lot of stuff
 #input: a tensor to be resized, the desired size or a scale to multiply the size by, the region of interest
 #output:the resized tensor
 ##############  https://onnx.ai/onnx/operators/onnx__Resize.html for more informations
 #The strategie is always to go throught the elements, find the coordinate in the original tensor 
 # and apply a transformation to the value in the original tensor to find the value to enter in the new tensor
 class Resize(Layer):
     
-    def __init__(self,idx,size,input_shape,activation_function,axes=[],coordinate_transformation_mode='half_pixel',exclude_outside=0,
-                 keep_aspect_ratio_policy='stretch',boolean_resize = None,target_size=[],roi=[],extrapolation_value=0, 
-                 nearest_mode = 'round_prefer_floor',cubic_coeff_a = -0.75):
+    def __init__(self, idx:int, size:int, input_shape:list, activation_function:ActivationFunctions, axes:list=[], coordinate_transformation_mode:str='half_pixel', exclude_outside:int=0,
+                 keep_aspect_ratio_policy:str='stretch', boolean_resize:None|bool=None, target_size:list=[], roi:list=[], extrapolation_value:float=0, 
+                 nearest_mode:str='round_prefer_floor', cubic_coeff_a:float=-0.75):
         super().__init__()
         self.idx = idx
         if(type(nearest_mode) == bytes):
             self.nearest_mode = str(nearest_mode)[2:-1]
         else: 
             self.nearest_mode = nearest_mode
         
@@ -82,109 +84,109 @@
             self.output_height = target_size[2]
             self.output_width = target_size[3]
             self.scale[1] = self.output_channels / self.input_channels #should be 1
             self.scale[2] = self.output_height / self.input_height
             self.scale[3] = self.output_width / self.input_width
             
     @abstractmethod
-    def forward_path_layer(self,input):
+    def forward_path_layer(self, input:np.ndarray):
         pass
     
     @abstractmethod
     def generate_inference_code_layer(self):
         pass
 
     #Defining the several coordinate transformations. cf documentation 
-    def half_pixel(self,coord_resized,coord_dim,coord_original):
+    def half_pixel(self, coord_resized:str, coord_dim,coord_original:str):
         s = coord_original + ' = ('+ coord_resized+' + 0.5)/'+ str(self.scale[coord_dim])+' - 0.5;'
         return s
 
-    def half_pixel_implem(self, coordinate, coordinate_dimension):
+    def half_pixel_implem(self, coordinate:int, coordinate_dimension:int):
         return (coordinate + 0.5)/self.scale[coordinate_dimension] - 0.5 
     
-    def half_pixel_symmetric(self,coord_resized,coord_dim,coord_original):
+    def half_pixel_symmetric(self, coord_resized:str, coord_dim,coord_original:str):
         if(coord_dim==2):
             target_length = self.output_height*self.scale[2]
             input_length = self.input_height
         else: 
             target_length = self.output_width*self.scale[3]
             input_length = self.input_width
 
         s = 'float adjustment = ' + str(int(target_length)) + '/' + str(target_length)  +';\n'
         s += '                float center = ' + str(input_length) + '/2;\n'
         s += '                float offset = center*(1 - adjustment);\n'
         s +='                '+ coord_original + ' = offset + ('+ coord_resized+' + 0.5)/'+ str(self.scale[coord_dim])+' - 0.5;'
         return s
     
-    def half_pixel_symmetric_implem(self, coordinate, coordinate_dimension):
+    def half_pixel_symmetric_implem(self, coordinate:int, coordinate_dimension:int):
         if(coordinate_dimension==2):
             target_length = self.output_height*self.scale[2]
             input_length = self.input_height
         else: 
             target_length = self.output_width*self.scale[3]
             input_length = self.input_width
 
         adjustment = int(target_length)/target_length
         center = input_length/2
         offset = center*(1 - adjustment)
         return offset + (coordinate + 0.5)/self.scale[coordinate_dimension] - 0.5 
 
-    def pytorch_half_pixel(self,coord_resized,coord_dim,coord_original):
+    def pytorch_half_pixel(self, coord_resized:str, coord_dim,coord_original:str):
         if(coord_dim==2):
             target_length = self.output_height
         else: 
             target_length = self.output_width
         
         s = coord_original + ' = '
         if (target_length > 1):
             s += '('+ coord_resized+' + 0.5)/'+ str(self.scale[coord_dim])+' - 0.5;'
         else:
             s += '0;' 
         return s
     
-    def pytorch_half_pixel_implem(self, coordinate, coordinate_dimension):
+    def pytorch_half_pixel_implem(self, coordinate:int, coordinate_dimension:int):
         if(coordinate_dimension==2):
             target_length = self.output_height
         else: 
             target_length = self.output_width
         
         if(target_length > 1):
             return (coordinate + 0.5)/self.scale[coordinate_dimension] - 0.5 
         else:
             return 0
 
-    def align_corners(self,coord_resized,coord_dim,coord_original):
+    def align_corners(self, coord_resized:str, coord_dim,coord_original:str):
         if(coord_dim==2):
             length_original = self.input_height
             length_resized = self.output_height
         else: 
             length_original = self.input_width
             length_resized = self.output_width
             
         s = coord_original + ' = ' +coord_resized+'*(' + str(length_original)+' - 1)/(' + str(length_resized)+' - 1);'
         return s
     
-    def align_corners_implem(self, coordinate, coordinate_dimension):
+    def align_corners_implem(self, coordinate:int, coordinate_dimension:int):
         if(coordinate_dimension==2):
             length_original = self.input_height
             length_resized = self.output_height
         else: 
             length_original = self.input_width
             length_resized = self.output_width
         
         return coordinate * (length_original - 1)/(length_resized - 1)
     
-    def asymmetric(self,coord_resized,coord_dim,coord_original):
+    def asymmetric(self, coord_resized:str, coord_dim,coord_original:str):
         s = coord_original + ' = '+ coord_resized+'/'+ str(self.scale[coord_dim]) +';'
         return s
     
-    def asymmetric_implem(self, coordinate, coordinate_dimension):
+    def asymmetric_implem(self, coordinate:int, coordinate_dimension:int):
         return coordinate/self.scale[coordinate_dimension]
     
-    def tf_crop_and_resize(self,coord_resized,coord_dim,coord_original):
+    def tf_crop_and_resize(self, coord_resized:str, coord_dim,coord_original:str):
         if(coord_dim==2):
             length_original = self.input_height
             length_resized = self.output_height
             start = self.roi[2]
             end = self.roi[6]
         else: 
             length_original = self.input_width
@@ -196,15 +198,15 @@
         if(length_resized > 1):
             s+= str(start) + '*('+ str(length_original)+' - 1) + '+ coord_resized+'*(' +str(end)+' - '+str(start)+')*('+str(length_original)+' - 1)/(' + str(length_resized)+' - 1);'
         else:
             s+= '0.5*(' +str(end)+' - '+str(start)+')*('+str(length_original)+' - 1);\n'
         s+= '                if(('+coord_original+' < 0) || ('+coord_original+' > '+str(length_original)+'){'+coord_original+' = '+ str(self.extrapolation_value)+'}'
         return s
 
-    def tf_crop_and_resize_implem(self, coordinate, coordinate_dimension):
+    def tf_crop_and_resize_implem(self, coordinate:int, coordinate_dimension:int):
         if(coordinate_dimension==2):
             length_original = self.input_height
             length_resized = self.output_height
             start = self.roi[2]
             end = self.roi[6]
         else: 
             length_original = self.input_width
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,29 +30,29 @@
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mode = 'cubic'
         self.template_dict = {'1D':self.template_path+'layers/Resize/template_ResizeCubic1D.c.tpl',
                               '2D':self.template_path+'layers/Resize/template_ResizeCubic2D.c.tpl'}
     
-    def cubic_interpolation_1D(self,input,f,x,y,s):
+    def cubic_interpolation_1D(self, input:np.ndarray, f:int, x:int, y:int, s:float):
         col_index = max(0,min(self.input_width-1,y))
         f_1 = input[f,max(0,min(self.input_height-1,x-1)),col_index]
         f0 = input[f,max(0,min(self.input_height-1,x)),col_index]
         f1 = input[f,max(0,min(self.input_height-1,x+1)),col_index]
         f2 = input[f,max(0,min(self.input_height-1,x+2)),col_index]
 
         coeff1 = (((self.cubic_coeff_a*(s + 1) -5*self.cubic_coeff_a)*(s + 1) + 8*self.cubic_coeff_a)*(s + 1) -4*self.cubic_coeff_a)
         coeff2 = (((self.cubic_coeff_a + 2)*(s) - (self.cubic_coeff_a + 3))*s*s + 1)
         coeff3 = (((self.cubic_coeff_a + 2)*(1 - s) - (self.cubic_coeff_a + 3))*(1 - s)*(1 - s) +1)
         coeff4 = (((self.cubic_coeff_a*(2 - s) -5*self.cubic_coeff_a)*(2 - s) + 8*self.cubic_coeff_a)*(2 - s) -4*self.cubic_coeff_a)
 
         return f_1*coeff1 + f0*coeff2 + f1*coeff3 + f2*coeff4
     
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
         output = np.zeros((self.output_channels,self.output_height,self.output_width))
         for f in range(self.output_channels):
             for i in range(self.output_height):
                 for j in range(self.output_width):
                     x = self.coordinate_transformation_mode_implem_mapping[self.coordinate_transformation_mode](i,2)
                     x0 = math.floor(x)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
         with open(self.template_dict[dimension],'r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template,mustach_hash)
 
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
         output = np.zeros((self.output_channels,self.output_height,self.output_width))
         for f in range(self.output_channels):
             for i in range(self.output_height):
                 for j in range(self.output_width):
                     x = self.coordinate_transformation_mode_implem_mapping[self.coordinate_transformation_mode](i,2)
                     x = np.clip(x,0,self.input_height-1)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,30 +37,30 @@
         
         self.nearest_mode_implem_mapping = {"round_prefer_floor":self.round_prefer_floor_implem,
                                             "round_prefer_ceil":self.round_prefer_ceil_implem,
                                             "floor":math.floor,
                                             "ceil":math.ceil}
     
     #Defining the several method to chose the nearest
-    def floor(self,x,y):
+    def floor(self, x:str, y:str):
         return x+' = floor('+y+');'
     
-    def ceil(self,x,y):
+    def ceil(self, x:str, y:str):
         return x+' = ceil('+y+');'
     
-    def round_prefer_floor(self,x,y):
+    def round_prefer_floor(self, x:str, y:str):
         return x+' = floor(ceil(2 * ' + y + ') / 2);'
     
-    def round_prefer_floor_implem(self,x):
+    def round_prefer_floor_implem(self, x:float):
         return math.floor(math.ceil(2*x)/2)
     
-    def round_prefer_ceil(self,x,y):
+    def round_prefer_ceil(self, x:str, y:str):
         return x+' = ceil(floor(2 * ' + y + ') / 2);'
     
-    def round_prefer_ceil_implem(self,x):
+    def round_prefer_ceil_implem(self, x:float):
         return math.ceil(math.floor(2*x)/2)
     
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
@@ -85,15 +85,15 @@
 
         with open(self.template_path+'layers/Resize/template_ResizeNearest.c.tpl') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)    
     
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
         output = np.zeros((self.output_channels,self.output_height,self.output_width))
         for f in range(self.output_channels):
             for i in range(self.output_height):
                 for j in range(self.output_width):
                     x = self.coordinate_transformation_mode_implem_mapping[self.coordinate_transformation_mode](i,2)
                     x0 = self.nearest_mode_implem_mapping[self.nearest_mode](x)
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from ..Layer import Layer
 import numpy as np
 import pystache
 
 class Softmax(Layer):
 
-    def __init__(self, idx, size):
+    def __init__(self, idx:int, size:int):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Softmax'
 
     def generate_inference_code_layer(self):
@@ -47,13 +47,13 @@
 
         with open(self.template_path+'layers/template_Softmax.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
-    def forward_path_layer(self, input):
+    def forward_path_layer(self, input:np.ndarray):
         
         exp = np.exp(input, dtype=np.float)
         output = exp/np.sum(exp)
 
         return output
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ResizeLinear, ResizeCubic, ResizeNearest, 
     Conv2D, Conv2D_6loops, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pooling2D, MaxPooling2D, AveragePooling2D
 )
 
 class CodeGenerator(ABC):
 
-    def __init__(self, file, test_dataset_file = None, function_name = 'inference', nb_tests = None, conv_algorithm = 'conv_gemm_optim', normalize = False, debug_mode = False, debug_target = [],**kwargs):
+    def __init__(self, file:str, test_dataset_file:str = None, function_name:str = 'inference', nb_tests:int = None, conv_algorithm:str = 'std_gemm_nn', normalize:bool = False, debug_mode:str|None = None, debug_target:list|None = None,**kwargs):
 
         self.file = file
         self.test_dataset_file = test_dataset_file
         self.function_name = function_name
         self.nb_tests = nb_tests
         self.conv_algorithm = conv_algorithm
         self.normalize = normalize
@@ -64,18 +64,36 @@
             ds = self.load_test_dataset()
             self.test_dataset = ds
         else:
             print("creating random dataset")
             ds = self.create_test_dataset()
             self.test_dataset = ds
         
-        self.debug_mode = debug_mode
-        self.debug_target = debug_target
+        ##### Debug Mode #####
+        if debug_mode:
+            self.debug_mode = debug_mode
+            self.debug_target = self.load_debug_target(debug_mode, debug_target)
+        ##### Debug Mode #####
 
         self.files_to_gen = ['inference.c', 'inference.h', 'global_vars.c', 'main.c', 'Makefile', 'test_dataset.h', 'test_dataset.c']
+    
+    def load_debug_target(self, debug_mode:str|None, debug_target:list|None):
+        if debug_target != None:
+            return debug_target
+        
+        else:
+            targets = []
+
+            for layer in self.layers[1:]:
+                if debug_mode == 'keras' and layer.name == 'Softmax':
+                    targets[-1] = layer.idx
+                else:
+                    targets.append(layer.idx)
+
+            return targets
         
     def create_test_dataset(self):
         test_dataset = self.data_type_py(np.random.default_rng(seed=10).random((int(self.nb_tests),1,int(self.layers[0].size))))
         return test_dataset 
      
     def load_test_dataset(self):
         
@@ -97,20 +115,22 @@
             f.close()
        
         except TypeError:
             None
         
         return test_dataset
 
-    def compute_inference(self, c_files_directory):
+    def compute_inference(self, c_files_directory:str):
         with open(os.path.join(c_files_directory, 'output_python.txt'), 'w+') as fi:
             for nn_input in self.test_dataset:
-
+                
+                ##### Debug Mode #####
                 if self.debug_mode:
                     debug_output = []
+                ##### Debug Mode #####
 
                 if((self.data_format == 'channels_last') and (len(self.layers[0].input_shape) == 4)): 
                     shape = (self.layers[0].input_shape[2],self.layers[0].input_shape[3],self.layers[0].input_shape[1])
                     nn_input = np.transpose(np.reshape(nn_input, shape), (2,0,1))
 
                 if (self.normalize): nn_input = self.Normalizer.pre_processing(nn_input)
                 previous_layer_result = [nn_input for i in range(self.maxpath)]  # for the very first layer, it is the neural network input
@@ -156,54 +176,62 @@
                     if (len(layer.next_layer) > 1): #if the layer has more than one child, it needs to be stored
                         to_store[layer.idx] = previous_layer_result[layer.path]
                         
                     for prev in layer.previous_layer:
                         if ((prev.sorted == len(prev.next_layer)) and (prev in to_store)):#if all the children of the parent layer are "taken care of", we "forget" the parent's value ( *2 because of the creation of the dict in graph.to_save)
                             to_store.pop(prev.idx)
                     
+                    ##### Debug Mode #####
                     if self.debug_mode:
-                        if layer.idx in self.debug_target or self.debug_target == []:
-                            debug_output.append(previous_layer_result[layer.path].flatten())
-                            
+                        # Add the inference result of the layer to debug_output
+                        if layer.name != 'Input_layer':
+                            if layer.idx in self.debug_target:
+                                debug_output.append(previous_layer_result[layer.path])
+                                if((self.data_format == 'channels_last') and hasattr(layer, 'output_channels')): debug_output[-1] = np.transpose(debug_output[-1], (1,2,0))
+                                debug_output[-1] = debug_output[-1].flatten()
+
+                        # If all the targets are saved, the inference is stopped and the result is given
+                        if len(debug_output) == len(self.debug_target):
+                            targets = [str(self.layers[k].name) + " " + str(self.layers[k].idx) for k in self.debug_target]
+                            return debug_output, targets
+                    ##### Debug Mode #####
+                        
                 nn_output = previous_layer_result[layer.path]
                 # print(nn_output) # write to file instead
                 
                 # Write results in text files to compare prediction.
                 if((self.data_format == 'channels_last') and hasattr(layer, 'output_channels')): nn_output = np.transpose(nn_output, (1,2,0))
                 nn_output = np.reshape(nn_output, -1)
 
                 if(self.normalize):
                     nn_output = self.Normalizer.post_processing(nn_output)
                 
                 for j in range(len(nn_output)):
-                    print('{:.9g}'.format(nn_output[j]), end=' ', file=fi, flush=True)           
+                    print('{:.9g}'.format(nn_output[j]), end=' ', file=fi, flush=True)
                     # print(decimal.Decimal(nn_output[j]), end=' ', file=fi, flush=True)
                 print(" ",file=fi)
         
         fi.close()
 
         print("File output_python.txt generated.")
 
-        if self.debug_mode:
-            return nn_output, debug_output
-        else:
-            return nn_output
+        return nn_output
 
-    def flatten_array_orderc(self, array):
+    def flatten_array_orderc(self, array:np.ndarray):
     
         flattened_aray = array.flatten(order='C')
         s = '\n        {'
         for i in range(flattened_aray.size):
             s += str(flattened_aray[i])+', '
         s = s[:-2]
         s+='}'
         
         return s
     
-    def flatten_array(self,array):
+    def flatten_array(self, array:np.ndarray):
         s = '\n        {'
         shape = array.shape
         if(len(shape)<4):
             for i in range(4-len(shape)):
                 shape = (1,) + shape
             array = np.reshape(array,shape)
         for j in range(shape[3]):
@@ -265,15 +293,15 @@
         with open(self.template_path+'template_Makefile.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         self.makefile.write(pystache.render(template, {'source_files':' '.join(source_files), 'header_files':' '.join(header_files), 'function_name':self.function_name}))
         self.makefile.close()
 
-    def generate_c_files(self, c_files_directory):  
+    def generate_c_files(self, c_files_directory:str):  
 
         self.c_files_directory = c_files_directory
         
         q = 0
         for file in self.files_to_gen:
             filename = Path(os.path.join(self.c_files_directory, file))
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,52 +16,56 @@
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 import keras
 from keras import activations
+from keras.engine.functional import Functional
+from keras.engine.sequential import Sequential
+from keras.engine.base_layer import Layer
+
 from itertools import islice
 import numpy as np
 
 from ...graph import graph_interpretor
 
 from ...code_generator import (
     AveragePooling2D, MaxPooling2D,
     Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
     Constant_Pad,
     Add, Multiply, Subtract, Maximum, Minimum, Average,
-    Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten, BatchNormalization,
+    Concatenate, InputLayer, Dense, Softmax, Flatten, BatchNormalization,
     Linear, ReLu, Sigmoid, TanH, LeakyReLu
 )
 
-def get_layer_size(keras_layer):
+def get_layer_size(keras_layer:Layer):
     size = 1
     if type(keras_layer.output_shape) is list:
         for dim in keras_layer.output_shape[0][1:]:
             size = size*dim
     else:
         for dim in keras_layer.output_shape[1:]:
             size = size*dim
     return size
 
-def get_output_dimensions(output,data_format):
+def get_output_dimensions(output:list, data_format:str):
     if type(output) is list:
         dimensions = output[0]
     else:
         dimensions = output
 
     if(data_format == 'channels_first'):
         return dimensions
     elif(len(dimensions) == 4):
         return (dimensions[0],dimensions[3],dimensions[1],dimensions[2])
     else:
         return dimensions
 
-def get_input_dimensions(input,data_format):
+def get_input_dimensions(input:list, data_format:str):
     if(type(input) == list and len(input) == 1):
         dimensions = input[0]
     else:
         dimensions = input
     
     if(data_format == 'channels_last'):
         if(type(dimensions) == list and len(dimensions[0]) == 4):
@@ -81,26 +85,26 @@
         elif kears_activation_obj == activations.linear:
             return Linear()
         elif kears_activation_obj == activations.leaky_relu:
             return LeakyReLu(0.2)
         elif kears_activation_obj == activations.softmax:
             return Linear()
 
-def create_conv2d_obj(algorithm, **kwargs):
+def create_conv2d_obj(algorithm:str, **kwargs):
        
     if '6loops' in algorithm:
         return Conv2D_6loops(**kwargs)
 
     elif 'std_gemm' in algorithm:
         return Conv2D_std_gemm(**kwargs)   
 
     elif 'indirect_gemm' in algorithm:
         return Conv2D_indirect_gemm(**kwargs)
 
-def load_keras(file_to_parse:keras.Model, conv_algorithm):
+def load_keras(file_to_parse:Functional|Sequential, conv_algorithm:str, debug:None|str):
 
     if(type(file_to_parse) == str): 
         model = keras.models.load_model(file_to_parse)
     else:
         model = file_to_parse
 
     input_layer_size = 1
@@ -294,15 +298,15 @@
                                          pads = pads,
                                          constant_value = 0,
                                          axes = [],
                                          input_shape = get_input_dimensions(layer_keras.input_shape, data_format),
                                          activation_function = Linear())
         
         elif layer_keras.__class__.__name__ == 'BatchNormalization':
-            if(layers[-1].name == 'Conv2D'):
+            if layers[-1].name == 'Conv2D' and not debug:
                 scale = data_type_py(layer_keras.get_weights()[0])
                 bias = data_type_py(layer_keras.get_weights()[1])
                 mean = data_type_py(layer_keras.get_weights()[2])
                 var = data_type_py(layer_keras.get_weights()[3])
 
                 weights = layers[-1].weights
                 biases = layers[-1].biases
@@ -360,19 +364,18 @@
 
             
         l_temp = current_layer
         layers.append(l_temp)
 
         if add_softmax_layer:
             nb_softmax_layers += 1
-            current_layer = Softmax(idx = idx,
+            current_layer = Softmax(idx = idx+1,
                                     size = l_temp.size)
             l_temp.next_layer.append(current_layer)
             current_layer.previous_layer.append(l_temp)
             l_temp = current_layer
             layers.append(l_temp)
         
     layers, listRoad, maxRoad, dict_cst = graph_interpretor.tri_topo(layers)
     layers = list(map(lambda x:x.find_output_str(dict_cst), layers))
     print("Finished model initialization.")
-    return layers, data_type, data_type_py, data_format, maxRoad, dict_cst
-            
+    return layers, data_type, data_type_py, data_format, maxRoad, dict_cst
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,21 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
-
+from keras.engine.functional import Functional
+from keras.engine.sequential import Sequential
 import json
 import numpy as np
 from numpyencoder import NumpyEncoder
 
-def JSON_from_keras_model(keras_model, output_dir_json):
+def JSON_from_keras_model(keras_model:Functional|Sequential, output_dir_json:str):
     model_json = keras_model.to_json()
     model_dict =  json.loads(model_json)
 
     input_layer_size = 1
     for i in range(1, len(keras_model.input.shape)): #start in idx 1 cause idx 0 represents batch size, so it's None in inference phase
         input_layer_size = input_layer_size * keras_model.input.shape[i]
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,50 +30,50 @@
     Constant_Pad,
     Add, Multiply, Subtract, Maximum, Minimum, Average,
     ResizeCubic, ResizeLinear, ResizeNearest,
     Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten, BatchNormalization,
     Linear, ReLu, Sigmoid, TanH, LeakyReLu
 )
 
-def create_actv_function_obj(activation_str):
+def create_actv_function_obj(activation_str:str):
 
         if activation_str == 'sigmoid':
             return Sigmoid()
         elif activation_str == 'relu':
             return ReLu()
         elif activation_str == 'tanh':
             return TanH()
         elif activation_str == 'linear':
             return Linear()
         elif activation_str == 'leaky_relu':
             return LeakyReLu(0.2)
 
-def create_conv2d_obj(algorithm, **kwargs):
+def create_conv2d_obj(algorithm:str, **kwargs):
        
     if '6loops' in algorithm:
         return Conv2D_6loops(**kwargs)
 
     elif 'std_gemm' in algorithm:
         return Conv2D_std_gemm(**kwargs)   
 
     elif 'indirect_gemm' in algorithm:
         return Conv2D_indirect_gemm(**kwargs)
 
-def create_resize_obj(mode, **kwargs):
+def create_resize_obj(mode:str, **kwargs):
 
     if mode == 'bicubic':
         return ResizeCubic(**kwargs)
     
     elif mode == 'bilinear':
         return ResizeLinear(**kwargs)
     
     else:
         return ResizeNearest(**kwargs)
 
-def load_json(file_to_parse, conv_algorithm):
+def load_json(file_to_parse:str, conv_algorithm:str):
         
     file = open(file_to_parse, 'r')
     model = json.load(file)
     data_format = model['config']['data_format'] 
 
     data_type = model['config']['layers'][0]['config']['dtype']
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 import pystache
 import numpy as np
 from abc import ABC
 from ... import templates
 
 class Normalizer(ABC):
 
-    def __init__(self, input_size, output_size, mins, maxes, means, ranges):
+    def __init__(self, input_size:int, output_size:int, mins:list, maxes:list, means:list, ranges:list):
         self.input_size = input_size
         self.output_size = output_size
         self.mins = mins
         self.maxes = maxes
         self.means = means
         self.ranges = ranges
         self.template_path = templates.__file__[:-11]
         super().__init__()
 
-    def array_to_str(self,array):
+    def array_to_str(self, array:list):
         s = "{"
         for element in array:
             s += str(element) + ", "
         s = s[:-2] + "}"
         return s
 
     def write_pre_processing(self):
@@ -81,17 +81,17 @@
 
         with open(self.template_path+'normalization/template_normalization_cst_in_global_var_file.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return  pystache.render(template, mustach_hash)
 
-    def pre_processing(self, nn_input):
+    def pre_processing(self, nn_input:np.ndarray):
         inputs = nn_input.flatten()
         for i in range(self.input_size):
             inputs[i] = (max(self.mins[i],min(self.maxes[i],inputs[i])) - self.means[i]) / self.ranges[i]
         return np.reshape(inputs, nn_input.shape)
 
-    def post_processing(self, nn_output):
+    def post_processing(self, nn_output:np.ndarray):
         for i in range(len(nn_output)):
             nn_output[i] = nn_output[i]*self.ranges[-1] + self.means[-1]
         return nn_output
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from ...code_generator.layers import Dense, InputLayer
 from ...code_generator.activation_functions import Linear, ReLu
 
 keras.backend.set_floatx('float32')
 
 
-def load_nnet(file_to_parse, normalize):
+def load_nnet(file_to_parse:str, normalize:bool):
     """
     Inspired from : # https://github.com/NeuralNetworkVerification/Marabou/blob/master/maraboupy/MarabouNetworkNNet.py
     """
 
     #Recall : Example of nnet file head:
     #7,5,5,50,  numLayers, inputSize, outputSize, maxLayersize
     #5,50,50,50,50,50,50,5,    Layersizes
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,66 +31,66 @@
     Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias, BatchNormalization
 )
 
 from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH, Clip, Exponential, Logarithm, LeakyReLu
 
 ###### Utility functions ######
 
-def create_conv2d_obj(algorithm, **kwargs):
+def create_conv2d_obj(algorithm:str, **kwargs):
        
     if '6loops' in algorithm:
         return Conv2D_6loops(**kwargs)
 
     elif 'std_gemm' in algorithm:
         return Conv2D_std_gemm(**kwargs)   
 
     elif 'indirect_gemm' in algorithm:
         return Conv2D_indirect_gemm(**kwargs)
         
 
-def create_resize_obj(mode, **kwargs):
+def create_resize_obj(mode:bytes, **kwargs):
     if mode == b'nearest':
         return ResizeNearest(**kwargs)
     
     elif mode == b'linear':
         return ResizeLinear(**kwargs)
     
     elif mode == b'cubic':
         return ResizeCubic(**kwargs)
 
-def create_pad_obj(mode, **kwargs):
+def create_pad_obj(mode:bytes, **kwargs):
     if mode == b'constant':
         return Constant_Pad(**kwargs)
     elif mode == b'edge':
         return Edge_pad(**kwargs)
     elif mode == b'wrap':
         return Wrap_pad(**kwargs)
     elif mode == b'reflect':
         return Reflect_pad(**kwargs)
 
 #Go find the constant named initialzer_name in model(an onnx model)
-def look_for_initializer(initializer_name,model):
+def look_for_initializer(initializer_name:str, model:onnx.ModelProto):
     if (initializer_name == ''):
         return []
     for initializer in model.graph.initializer:
         if (initializer.name == initializer_name):
             return initializer
     return []
 
 
 #Return a dictonnary with {attibut: attribut_values}
-def extract_attribut(node):
+def extract_attribut(node:onnx.NodeProto):
     attributes = {}
     for attribute in node.attribute:
         attributes[attribute.name] = onnx.helper.get_attribute_value(attribute)
     return attributes
 
 #Find the shape of shape_name in model (an onnx model)
 #Depend of the carac of the model. Need value_info in the model
-def get_shape(shape_name,model):
+def get_shape(shape_name:str, model:onnx.ModelProto):
     shape = []
     for info in model.graph.value_info:
         if(shape_name == info.name):
             shape = [info.type.tensor_type.shape.dim[i].dim_value for i in range(len(info.type.tensor_type.shape.dim))]
     for input in model.graph.input:
         if(shape_name == input.name):
             shape = [input.type.tensor_type.shape.dim[i].dim_value for i in range(len(input.type.tensor_type.shape.dim))]
@@ -101,44 +101,44 @@
         shape = [1 for i in range(4-len(shape))] + shape
     for i in range(len(shape)):
         if shape[i] == 0:
             shape[i] = 1
     return shape
 
 #Return the size of the layer when given the list output_shape
-def find_size(output_shape):
+def find_size(output_shape:list):
     size = 1
     for i in output_shape:
         if i != 0:
             size*=i
     return size
 
 
 ###### Functions to create a Layer ######
 
 #Create an input layers 
-def create_Input_Layer(input_layer,idx,dict_output):
+def create_Input_Layer(input_layer:onnx.NodeProto, idx:int, dict_output:dict):
         dict_output[input_layer.name] = idx
         output_shape = [input_layer.type.tensor_type.shape.dim[i].dim_value for i in range(len(input_layer.type.tensor_type.shape.dim))]
         size = find_size(output_shape)
         
         return InputLayer(idx,size,output_shape,'channels_first')
 
 #Create a layer Softmax
-def create_Softmax(node,idx,dict_input,dict_output,model):
+def create_Softmax(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     return Softmax(idx = idx,
                             size = size)
 
 
 #Create a layer Conv
-def create_Conv(node,idx,dict_input,dict_output,model,conv_algorithm):
+def create_Conv(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto, conv_algorithm:str):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     initializers = [look_for_initializer(initializer_name,model) for initializer_name in node.input[1:]]
     attributs = extract_attribut(node)
@@ -172,15 +172,15 @@
                                 output_shape= output_shape,
                                 weights= np.moveaxis(onnx.numpy_helper.to_array(initializers[0]), 0,3),
                                 biases= biases,
                                 activation_function= Linear())
     
 
 #Create a layer Concat
-def create_Concat(node,idx,dict_input,dict_output,model):
+def create_Concat(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
@@ -189,15 +189,15 @@
                         size, 
                         attributs['axis'],
                         input_shapes,
                         output_shape,
                         activation_function= Linear())
     
 #Create a layer Resize
-def create_Resize(node,idx,dict_input,dict_output,model):
+def create_Resize(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     initializers = [look_for_initializer(initializer_name,model) for initializer_name in node.input[1:]]
     attributs = extract_attribut(node)
@@ -243,15 +243,15 @@
                              roi = roi,
                              extrapolation_value = attributs['extrapolation_value'],
                              nearest_mode = attributs['nearest_mode'],
                              cubic_coeff_a=attributs['cubic_coeff_a'],
                              activation_function = Linear())
     
 #create a layer Pad
-def create_Pad(node,idx,dict_input,dict_output,model):
+def create_Pad(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     axes = []
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     initializers = [look_for_initializer(initializer_name,model) for initializer_name in node.input[1:]]
@@ -267,15 +267,15 @@
                           constant_value = onnx.numpy_helper.to_array(initializers[1]),
                           axes = axes,
                           input_shape = input_shape,
                           activation_function = Linear())
 
 
 #create a layer Gather
-def create_Gather(node,idx,dict_input,dict_output,model):
+def create_Gather(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     initializer = look_for_initializer(node.input[1],model)
@@ -284,15 +284,15 @@
                     axis = attributs['axis'],
                     indices = onnx.numpy_helper.to_array(initializer),
                     input_shape = input_shape,
                     output_shape = output_shape,
                     activation_function = Linear())
 
 #create a layer Gemm
-def create_Gemm(node,idx,dict_input,dict_output,model):
+def create_Gemm(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     B_tensor = look_for_initializer(node.input[1],model)
@@ -316,15 +316,15 @@
                 transB = attributs['transB'],
                 weights = onnx.numpy_helper.to_array(B_tensor),
                 bias = onnx.numpy_helper.to_array(C_tensor),
                 input_shape = input_shape,
                 output_shape = output_shape,
                 activation_function = Linear())
 
-def create_MatMul(node,idx,dict_input,dict_output,model):
+def create_MatMul(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_output[node.output[0]] = idx
     right_tensor = look_for_initializer(node.input[0],model)
     left_tensor = look_for_initializer(node.input[1],model)
     if(left_tensor or right_tensor):
         if(right_tensor and not left_tensor):
@@ -357,15 +357,15 @@
         return Dot(idx = idx,
                     size = size,
                     axis = [-1,-2],
                     input_shapes = input_shapes,
                     output_shape = output_shape,
                     activation_function = Linear())
 
-def create_BatchNorm(node,idx,dict_input,dict_output,model):
+def create_BatchNorm(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     
     if('epsilon' not in attributs):
@@ -387,15 +387,15 @@
                               activation_function = Linear())
 
 
 
 ### Pooling layers ###
 
 #Create a layer MaxPool
-def create_MaxPool(node,idx,dict_input,dict_output,model):
+def create_MaxPool(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     if ('dilations' not in attributs):
@@ -412,15 +412,15 @@
                         strides = attributs['strides'][0],
                         pool_size = attributs['kernel_shape'][0],
                         input_shape = input_shape,
                         output_shape = output_shape,
                         activation_function = Linear())
 
 #cerate a layer AveragePool
-def create_AveragePool(node,idx,dict_input,dict_output,model):
+def create_AveragePool(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     if ('dilations' not in attributs):
@@ -437,15 +437,15 @@
                             strides=attributs['strides'][0], 
                             pool_size=attributs['kernel_shape'][0], 
                             input_shape=input_shape,
                             output_shape=output_shape,
                             activation_function = Linear())
 
 #Create a layer GlobalAveragePool
-def create_GlobalAveragePool(node,idx,dict_input,dict_output,model):
+def create_GlobalAveragePool(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     return AveragePooling2D(idx = idx,
                             size = size,
@@ -456,15 +456,15 @@
                             output_shape = output_shape,
                             activation_function = Linear())
 
 ### Broadcats layers ###
 
 #create a layer Add_Biass 
 ##### UNUSED #####
-def create_Add_Biass(node,idx,dict_input,dict_output,model):
+def create_Add_Biass(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_output[node.output[0]] = idx
     right_tensor = look_for_initializer(node.input[0],model)
     left_tensor = look_for_initializer(node.input[1],model)
     if(right_tensor):
         biases = onnx.numpy_helper.to_array(right_tensor)
@@ -474,15 +474,15 @@
         dict_input[idx] = [node.input[0]]
     return Add_Bias(idx = idx,
                         size = size,
                         biases = biases,
                         activation_function = Linear())
 
 #create a layer Add
-def create_Add(node,idx,dict_input,dict_output,model):
+def create_Add(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_output[node.output[0]] = idx
     dict_input[idx] = []
     constant = np.zeros(get_shape(node.input[0], model))
     input_shapes =[]
     for input in node.input:
@@ -503,15 +503,15 @@
                 size = size,
                 input_shapes = input_shapes,
                 output_shape = output_shape,
                 activation_function = Linear(),
                 constant = constant)
     
 #create a layer Div
-def create_Div(node,idx,dict_input,dict_output,model):
+def create_Div(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     constant = 1
     dict_input[idx] = []
     for input in node.input:
         factor = look_for_initializer(input,model)
         if(factor):
             constant = constant / onnx.numpy_helper.to_array(factor)
@@ -533,15 +533,15 @@
                     input_shapes=input_shapes,
                     output_shape=output_shape,
                     activation_function= Linear(),
                     constant=constant)
 
 
 #create a layer Mul
-def create_Mul(node,idx,dict_input,dict_output,model):
+def create_Mul(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     constant = 1
     dict_input[idx] = []
     for input in node.input:
         factor = look_for_initializer(input,model)
         if(factor):
             constant = constant * onnx.numpy_helper.to_array(factor)
@@ -562,15 +562,15 @@
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
                     activation_function= Linear(),
                     constant=constant)
 
 #create a layer Sub
-def create_Sub(node,idx,dict_input,dict_output,model):
+def create_Sub(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     constant = 0
     dict_input[idx] = []
     for input in node.input:
         factor = look_for_initializer(input,model)
         if(factor):
             constant = constant - onnx.numpy_helper.to_array(factor)
@@ -591,45 +591,45 @@
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
                     activation_function= Linear(),
                     constant=constant)
     
 #create a layer Max
-def create_Max(node,idx,dict_input,dict_output,model):
+def create_Max(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     return Maximum(idx=idx,
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
                     activation_function= Linear())
 
 #create a layer Min
-def create_Min(node,idx,dict_input,dict_output,model):
+def create_Min(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     return Minimum(idx=idx,
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
                     activation_function= Linear())
 
 #create a layer Average
-def create_Avg(node,idx,dict_input,dict_output,model):
+def create_Avg(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
@@ -659,18 +659,18 @@
          "Min":create_Min,
          "Mean":create_Avg}
 
 
 ###### Function to deal with the 'non important' layers of the graph ######
 
 #Do the opeartion: Dropout.input = Dropout.output
-def bypass(node,dict_output,model):
+def bypass(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto):
     dict_output[node.output[0]] = dict_output.pop(node.input[0])
 
-def create_initializer(node,dict_output,model):
+def create_initializer(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto):
     const = model.graph.initializer.add()
     const.name = node.output[0]
     const.data_type = node.attribute[0].t.data_type
     const.raw_data = node.attribute[0].t.raw_data
 
 ###### Dict of all the functions ######
 unused_layers = {"Dropout":bypass,
@@ -680,58 +680,58 @@
                   "LRN":bypass,
                   "Shape":bypass,
                   "Flatten":bypass}
 
 ###### Function to fuse to ONNX layers ######
 
 #Fuse the activation layer ReLu with the prior layer
-def fuse_ReLu(node,dict_output,model,layers):
+def fuse_ReLu(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto, layers:list):
     layers[dict_output[node.input[0]]].activation_function = ReLu()
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Tanh with the prior layer
-def fuse_Tanh(node,dict_output,model,layers):
+def fuse_Tanh(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto, layers:list):
     layers[dict_output[node.input[0]]].activation_function = TanH()
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Sigmoide with the prior layer
-def fuse_Sigmoid(node,dict_output,model,layers):
+def fuse_Sigmoid(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto, layers:list):
     layers[dict_output[node.input[0]]].activation_function = Sigmoid()
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Sigmoide with the prior layer
-def fuse_Exp(node,dict_output,model,layers):
+def fuse_Exp(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto, layers:list):
     layers[dict_output[node.input[0]]].activation_function = Exponential()
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Sigmoid with the prior layer
-def fuse_Log(node,dict_output,model,layers):
+def fuse_Log(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto, layers:list):
     layers[dict_output[node.input[0]]].activation_function = Logarithm()
     bypass(node,dict_output,model)
 
 #Fuse a layer Clip with the prior layer
-def fuse_Clip(node,dict_output,model,layers):
+def fuse_Clip(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto, layers:list):
     min, max = float('-inf'), float('inf')
     if(node.input[1]):
         min = onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model))[0]
     if(node.input[2]):
         max = onnx.numpy_helper.to_array(look_for_initializer(node.input[2],model))[0]
     layers[dict_output[node.input[0]]].activation_function = Clip(max=max,min=min)
     bypass(node,dict_output,model)
 
 #Fuse the activation layer LeakyRelu with the prior layer
-def fuse_LeakyReLu(node,dict_output,model,layers):
+def fuse_LeakyReLu(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto, layers:list):
     attribut = extract_attribut(node)
     if('alpha' not in attribut):
         attribut['alpha'] = 0.01
     layers[dict_output[node.input[0]]].activation_function = LeakyReLu(alpha=attribut['alpha'])
     bypass(node,dict_output,model)
 
 #Fuse a BatchNormalization layer with the previous Conv2D layer
-def fuse_BatchNormalization(node,dict_output,model,layers):
+def fuse_BatchNormalization(node:onnx.NodeProto, dict_output:dict, model:onnx.ModelProto, layers:list):
     attributs = extract_attribut(node)
     if('epsilon' not in attributs):
         attributs['epsilon'] = 1e-05
     
     scale = onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model))
     bias = onnx.numpy_helper.to_array(look_for_initializer(node.input[2],model))
     mean = onnx.numpy_helper.to_array(look_for_initializer(node.input[3],model))
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 import onnx
 from ..ONNX_importer.create_layer import *
 from ...graph.graph_interpretor import tri_topo
 
-def load_onnx(file_to_parse, conv_algorithm):
+def load_onnx(file_to_parse:str|onnx.ModelProto, conv_algorithm:str, debug:None|str):
     #Loading the model and adding value_info if it's not already in it
     if(type(file_to_parse) == str): 
         model = onnx.load(file_to_parse)
     else:
         model = file_to_parse
         
     if (not model.graph.value_info):
@@ -42,30 +42,30 @@
 
     #Creating and adding all the input layers to the list
     layers.append(create_Input_Layer(model.graph.input[0],idx,dict_output))
     idx+=1
     
     #Going through all the nodes to creat the layers and add them to the list
     for node in model.graph.node:
-        if(node.op_type == 'BatchNormalization'):
-            if(layers[-1].name == 'Conv2D'):
+        if node.op_type == 'BatchNormalization':
+            if layers[-1].name == 'Conv2D' and not debug:
                 fuse_BatchNormalization(node, dict_output, model, layers)
             else:
                 layers.append(create_BatchNorm(node,idx,dict_input,dict_output,model))
                 idx+=1
-        elif(node.op_type in layer_type): #If the node is a useful layer, we add it to the list
-            if(node.op_type == "Conv"):    
+        elif node.op_type in layer_type: #If the node is a useful layer, we add it to the list
+            if node.op_type == "Conv":    
                 layers.append(layer_type[node.op_type](node,idx,dict_input,dict_output,model,conv_algorithm))
                 idx+=1
             else:
                 layers.append(layer_type[node.op_type](node,idx,dict_input,dict_output,model))
                 idx+=1
-        elif(node.op_type in unused_layers): #If the node is a layer only used in trainning, we do layer_input=layer_output
+        elif node.op_type in unused_layers: #If the node is a layer only used in trainning, we do layer_input=layer_output
             unused_layers[node.op_type](node,dict_output,model)
-        elif(node.op_type in activation_layers):
+        elif node.op_type in activation_layers:
             activation_layers[node.op_type](node,dict_output,model,layers)
         else:
             raise TypeError("Error: layer "+node.op_type+" not supported\n")
     
     for layer_idx in dict_input: #Going through all the indices in the list
         layer = layers[layer_idx] #The indice of a layer is the same a it's position in the list
         for input_name in dict_input[layer_idx]: #Going through all the inputs to that layer
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/format_importer/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,46 +24,35 @@
 import onnx
 
 from .JSON_importer.parser_JSON import load_json
 from .ONNX_importer.parser_ONNX import load_onnx
 from .NNET_importer.parser_NNET import load_nnet
 from .H5_importer.parser_h5 import load_keras
 
-def get_path(file, new_type):
-    new_path = ""
-    list_path = file.split("/")
-    file_name = list_path[-1].split(".")[0]
-
-    for dir in list_path[:-1]:
-        new_path += dir+"/"
-    
-    new_path += file_name + "." + new_type
-    return new_path
-
-def parser(file_to_parse, conv_algorithm, normalize=False):
+def parser(file_to_parse:str|onnx.ModelProto|Functional|Sequential, conv_algorithm:str, normalize:bool=False, debug:None|str=None):
 
     if(type(file_to_parse) == str):
         if("json" in  file_to_parse[-4:]):
             return load_json(file_to_parse, conv_algorithm)
         
         elif("onnx" in file_to_parse[-4:]):
-            return load_onnx(file_to_parse, conv_algorithm)
+            return load_onnx(file_to_parse, conv_algorithm, debug)
         
         elif("h5" in file_to_parse[-4:]):
-            return load_keras(file_to_parse, conv_algorithm)
+            return load_keras(file_to_parse, conv_algorithm, debug)
         
         elif("nnet" in file_to_parse[-4:]):
             return load_nnet(file_to_parse,normalize)
         
         else:
             print("\nError: model description ."+file_to_parse[-4:]+" not supported")
             raise TypeError("Error: model description ."+file_to_parse[-4:]+" not supported\nOnly description supported are: .nnet, .h5, .json, .onnx\n")
     
     elif(type(file_to_parse) == onnx.ModelProto):
-        return load_onnx(file_to_parse, conv_algorithm)
+        return load_onnx(file_to_parse, conv_algorithm, debug)
     
     elif(type(file_to_parse) == Functional or type(file_to_parse) == Sequential):
-        return load_keras(file_to_parse, conv_algorithm)
+        return load_keras(file_to_parse, conv_algorithm, debug)
 
     else:
         print("\nError: model description .",type(file_to_parse),"not supported")
         raise TypeError("Error: model description .",type(file_to_parse),"not supported\nOnly description supported are: .nnet, .h5, .json, .onnx\n")
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
+from ..code_generator.Layer import Layer
+
 #Sort the graph (list of nodes) based on the topological sort
-def tri_topo(dnn):
+def tri_topo(dnn:list):
     list_path = []
     #The sorted list to be returned
     list_layers = []
     #the dict stating which layers need to go in a constant
     dict_cst = {}
     for layer in dnn:
         #If the node isn't sorted, we sort it
@@ -32,29 +34,29 @@
     for layer in list_layers:
         updatepath(layer,list_path)
         to_save(layer,dict_cst)
     max_path = list_path[-2] + 1
     return list_layers, list_path, max_path, dict_cst
 
 #Compute the sorting of a node
-def parcours_prof_topo(list_layers,layer):
+def parcours_prof_topo(list_layers:list, layer:Layer):
     #The node is currently being sorted
     layer.sorted = 1
     for nxt_layer in layer.next_layer:
         #The next_layer need to be found and sorted before the current node
         if nxt_layer.sorted == None:
             parcours_prof_topo(list_layers, nxt_layer)
     #The node is sorted
     layer.sorted = 0
     #And is added to the list of sorted nodes
     list_layers.insert(0,layer)
 
 
 #The function to open a new path
-def setNewpath(layer,listCurrentpaths):
+def setNewpath(layer:Layer, listCurrentpaths:list):
     #if the list isn't in the right format, it return -1
     if(len(listCurrentpaths)%2!=0):
         print("Error: listCurrentpaths must be in format:[name_path, is_path_closed, ...]")
         return -1
     else:
         N = len(listCurrentpaths)//2
         #check if there is a previously closed path avialable 
@@ -72,15 +74,15 @@
         #if no previously closed path can fit are avialable, we create a new one
         elif(layer.path == None):
             listCurrentpaths.append(listCurrentpaths[-2]+1)
             listCurrentpaths.append(0)
             layer.path = listCurrentpaths[-2]
         
 #give a layer the right path    
-def updatepath(layer,listCurrentpaths):
+def updatepath(layer:Layer, listCurrentpaths:list):
     if(layer.previous_layer == []):
         #if the layer has no previous one, we creat a new path
         setNewpath(layer,listCurrentpaths)
 
     given = False
     #every next_layer need to have a path 
     for nxt_layer in layer.next_layer:
@@ -100,15 +102,15 @@
             setNewpath(nxt_layer,listCurrentpaths)
     
     #if the path isn't given, it is closed
     if (given == False):
         listCurrentpaths[layer.path*2 + 1] = 1
 
 #Function creating the dict {idx_layer:idx_cst} saying if a layer must be stored
-def to_save(layer,dict_cst):
+def to_save(layer:Layer, dict_cst:dict):
     for parent in layer.previous_layer:
         if(parent in dict_cst):
             #if the previous_layer are in the dict, we add one to the number of next_layer already "taken care of"
             parent.sorted+=1
 
     if((len(layer.next_layer)>1)):
         #if the layer has more than one child, it must be stored.
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2.3
+Version: 0.2.3.dev1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.2.3/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.2.3.dev1/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

