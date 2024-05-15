# Comparing `tmp/bioimageio.core-0.6.3.tar.gz` & `tmp/bioimageio.core-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.core-0.6.3.tar", last modified: Thu May  2 13:04:05 2024, max compression
+gzip compressed data, was "bioimageio.core-0.6.4.tar", last modified: Wed May 15 11:46:26 2024, max compression
```

## Comparing `bioimageio.core-0.6.3.tar` & `bioimageio.core-0.6.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-02 13:04:02.000000 bioimageio.core-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.107979 bioimageio.core-0.6.3/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.111980 bioimageio.core-0.6.3/bioimageio/core/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 13:04:02.000000 bioimageio.core-0.6.3/bioimageio/core/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/_magic_tensor_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/_op_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-02 13:04:02.000000 bioimageio.core-0.6.3/bioimageio/core/_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/block_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/model_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_keras_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_onnx_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_pytorch_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_torchscript_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/proc_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/weight_converter/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/keras/_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.111980 bioimageio.core-0.6.3/bioimageio.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-02 13:04:05.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/scripts/setup_dev_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/scripts/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_any_model_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_bioimageio_spec_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_prediction_pipeline_device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/tests/weight_converter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/tests/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/weight_converter/keras/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/weight_converter/test_add_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/tests/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/weight_converter/torch/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/weight_converter/torch/test_torchscript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-15 11:46:23.000000 bioimageio.core-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.134239 bioimageio.core-0.6.4/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.138239 bioimageio.core-0.6.4/bioimageio/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 11:46:23.000000 bioimageio.core-0.6.4/bioimageio/core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_magic_tensor_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_op_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/block_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/model_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_keras_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_onnx_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_pytorch_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_torchscript_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/proc_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/weight_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/keras/_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.134239 bioimageio.core-0.6.4/bioimageio.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-15 11:46:26.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/scripts/setup_dev_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/scripts/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 11:46:23.000000 bioimageio.core-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_any_model_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_bioimageio_spec_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_prediction_pipeline_device_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/tests/weight_converter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/tests/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/weight_converter/keras/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/weight_converter/test_add_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/tests/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/weight_converter/torch/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/weight_converter/torch/test_torchscript.py
```

### Comparing `bioimageio.core-0.6.3/LICENSE` & `bioimageio.core-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/PKG-INFO` & `bioimageio.core-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
@@ -129,14 +129,19 @@
         
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.4
+        
+        * add `bioimageio validate-format` command
+        * improve error messages and display of command results
+        
         ### 0.6.3
         
         * Fix [#386](https://github.com/bioimage-io/core-bioimage-io-python/issues/386)
         * (in model inference testing) stop assuming model inputs are tileable
         
         ### 0.6.2
```

### Comparing `bioimageio.core-0.6.3/README.md` & `bioimageio.core-0.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,19 @@
 
 ## Model Specification
 
 The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
 
 ## Changelog
 
+### 0.6.4
+
+* add `bioimageio validate-format` command
+* improve error messages and display of command results
+
 ### 0.6.3
 
 * Fix [#386](https://github.com/bioimage-io/core-bioimage-io-python/issues/386)
 * (in model inference testing) stop assuming model inputs are tileable
 
 ### 0.6.2
```

### Comparing `bioimageio.core-0.6.3/bioimageio/core/__init__.py` & `bioimageio.core-0.6.4/bioimageio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/_magic_tensor_ops.py` & `bioimageio.core-0.6.4/bioimageio/core/_magic_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/_op_base.py` & `bioimageio.core-0.6.4/bioimageio/core/_op_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/_prediction_pipeline.py` & `bioimageio.core-0.6.4/bioimageio/core/_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/_resource_tests.py` & `bioimageio.core-0.6.4/bioimageio/core/_resource_tests.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/axis.py` & `bioimageio.core-0.6.4/bioimageio/core/axis.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/block.py` & `bioimageio.core-0.6.4/bioimageio/core/block.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/block_meta.py` & `bioimageio.core-0.6.4/bioimageio/core/block_meta.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/commands.py` & `bioimageio.core-0.6.4/bioimageio/core/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 import sys
 from pathlib import Path
 from typing import List, Optional, Union
 
 import fire
 
 from bioimageio.core import __version__, test_description
-from bioimageio.spec import save_bioimageio_package
+from bioimageio.spec import (
+    load_description_and_validate_format_only,
+    save_bioimageio_package,
+)
 from bioimageio.spec.collection import CollectionDescr
 from bioimageio.spec.dataset import DatasetDescr
 from bioimageio.spec.model import ModelDescr
 from bioimageio.spec.model.v0_5 import WeightsFormat
 from bioimageio.spec.notebook import NotebookDescr
 
 
@@ -50,22 +53,37 @@
         Args:
             source: Path or URL to the bioimageio resource description file
                     (bioimageio.yaml or rdf.yaml) or to a zipped resource
             weight_format: (model only) The weight format to use
             devices: Device(s) to use for testing
             decimal: Precision for numerical comparisons
         """
+        print(f"\ntesting {source}...")
         summary = test_description(
             source,
             weight_format=None if weight_format is None else weight_format,
             devices=[devices] if isinstance(devices, str) else devices,
             decimal=decimal,
         )
-        print(f"\ntesting model {source}...")
-        print(summary.format())
+        summary.display()
+        sys.exit(0 if summary.status == "passed" else 1)
+
+    @staticmethod
+    def validate_format(
+        source: str,
+    ):
+        """validate the meta data format of a bioimageio resource description
+
+        Args:
+            source: Path or URL to the bioimageio resource description file
+                    (bioimageio.yaml or rdf.yaml) or to a zipped resource
+        """
+        print(f"\validating meta data format of {source}...")
+        summary = load_description_and_validate_format_only(source)
+        summary.display()
         sys.exit(0 if summary.status == "passed" else 1)
 
 
 assert isinstance(Bioimageio.__doc__, str)
 Bioimageio.__doc__ += f"""
 
 library versions:
```

### Comparing `bioimageio.core-0.6.3/bioimageio/core/common.py` & `bioimageio.core-0.6.4/bioimageio/core/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/digest_spec.py` & `bioimageio.core-0.6.4/bioimageio/core/digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/io.py` & `bioimageio.core-0.6.4/bioimageio/core/io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_keras_model_adapter.py` & `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_keras_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_model_adapter.py` & `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_model_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 import warnings
 from abc import ABC, abstractmethod
 from typing import List, Optional, Sequence, Tuple, Union, final
 
 from bioimageio.spec.model import v0_4, v0_5
 
 from ..tensor import Tensor
@@ -72,45 +73,45 @@
 
                     return PytorchModelAdapter(
                         outputs=model_description.outputs,
                         weights=weights.pytorch_state_dict,
                         devices=devices,
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}")
+                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
             elif (
                 wf == "tensorflow_saved_model_bundle"
                 and weights.tensorflow_saved_model_bundle is not None
             ):
                 try:
                     from ._tensorflow_model_adapter import TensorflowModelAdapter
 
                     return TensorflowModelAdapter(
                         model_description=model_description, devices=devices
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}")
+                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
             elif wf == "onnx" and weights.onnx is not None:
                 try:
                     from ._onnx_model_adapter import ONNXModelAdapter
 
                     return ONNXModelAdapter(
                         model_description=model_description, devices=devices
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}")
+                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
             elif wf == "torchscript" and weights.torchscript is not None:
                 try:
                     from ._torchscript_model_adapter import TorchscriptModelAdapter
 
                     return TorchscriptModelAdapter(
                         model_description=model_description, devices=devices
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}")
+                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
             elif wf == "keras_hdf5" and weights.keras_hdf5 is not None:
                 # keras can either be installed as a separate package or used as part of tensorflow
                 # we try to first import the keras model adapter using the separate package and,
                 # if it is not available, try to load the one using tf
                 try:
                     from ._keras_model_adapter import (
                         KerasModelAdapter,
@@ -120,15 +121,15 @@
                     if keras is None:
                         from ._tensorflow_model_adapter import KerasModelAdapter
 
                     return KerasModelAdapter(
                         model_description=model_description, devices=devices
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}")
+                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
 
         assert errors
         error_list = "\n - ".join(errors)
         raise ValueError(
             "None of the weight format specific model adapters could be created for"
             + f" '{model_description.id or model_description.name}'"
             + f" in this environment. Errors are:\n\n{error_list}.\n\n"
```

### Comparing `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_onnx_model_adapter.py` & `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_onnx_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_pytorch_model_adapter.py` & `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_pytorch_model_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         ],
         weights: Union[
             v0_4.PytorchStateDictWeightsDescr, v0_5.PytorchStateDictWeightsDescr
         ],
         devices: Optional[Sequence[str]] = None,
     ):
         if torch is None:
-            raise ImportError("torch")
+            raise ImportError("failed to import torch")
         super().__init__()
         self.output_dims = [tuple(a.id for a in get_axes_infos(out)) for out in outputs]
         self._network = self.get_network(weights)
         self._devices = self.get_devices(devices)
         self._network = self._network.to(self._devices[0])
 
         self._primary_device = self._devices[0]
```

### Comparing `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_tensorflow_model_adapter.py` & `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_tensorflow_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_torchscript_model_adapter.py` & `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_torchscript_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/proc_ops.py` & `bioimageio.core-0.6.4/bioimageio/core/proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/proc_setup.py` & `bioimageio.core-0.6.4/bioimageio/core/proc_setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/sample.py` & `bioimageio.core-0.6.4/bioimageio/core/sample.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/stat_calculators.py` & `bioimageio.core-0.6.4/bioimageio/core/stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/stat_measures.py` & `bioimageio.core-0.6.4/bioimageio/core/stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/tensor.py` & `bioimageio.core-0.6.4/bioimageio/core/tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/utils/testing.py` & `bioimageio.core-0.6.4/bioimageio/core/utils/testing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/weight_converter/keras/_tensorflow.py` & `bioimageio.core-0.6.4/bioimageio/core/weight_converter/keras/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_onnx.py` & `bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_torchscript.py` & `bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_torchscript.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_utils.py` & `bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/bioimageio.core.egg-info/PKG-INFO` & `bioimageio.core-0.6.4/bioimageio.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
@@ -129,14 +129,19 @@
         
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.4
+        
+        * add `bioimageio validate-format` command
+        * improve error messages and display of command results
+        
         ### 0.6.3
         
         * Fix [#386](https://github.com/bioimage-io/core-bioimage-io-python/issues/386)
         * (in model inference testing) stop assuming model inputs are tileable
         
         ### 0.6.2
```

### Comparing `bioimageio.core-0.6.3/bioimageio.core.egg-info/SOURCES.txt` & `bioimageio.core-0.6.4/bioimageio.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/pyproject.toml` & `bioimageio.core-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/scripts/setup_dev_env.py` & `bioimageio.core-0.6.4/scripts/setup_dev_env.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/scripts/show_diff.py` & `bioimageio.core-0.6.4/scripts/show_diff.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/setup.py` & `bioimageio.core-0.6.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     packages=find_namespace_packages(exclude=["tests"]),
     install_requires=[
-        "bioimageio.spec==0.5.2.*",
+        "bioimageio.spec>=0.5.2.post5,<0.6",
         "fire",
         "imageio>=2.5",
         "loguru",
         "numpy",
         "pydantic-settings",
         "pydantic",
         "python-dotenv",
```

### Comparing `bioimageio.core-0.6.3/tests/test_bioimageio_spec_version.py` & `bioimageio.core-0.6.4/tests/test_bioimageio_spec_version.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_cli.py` & `bioimageio.core-0.6.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_digest_spec.py` & `bioimageio.core-0.6.4/tests/test_digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_prediction.py` & `bioimageio.core-0.6.4/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_prediction_pipeline.py` & `bioimageio.core-0.6.4/tests/test_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_prediction_pipeline_device_management.py` & `bioimageio.core-0.6.4/tests/test_prediction_pipeline_device_management.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_proc_ops.py` & `bioimageio.core-0.6.4/tests/test_proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_resource_tests.py` & `bioimageio.core-0.6.4/tests/test_resource_tests.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_stat_calculators.py` & `bioimageio.core-0.6.4/tests/test_stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_stat_measures.py` & `bioimageio.core-0.6.4/tests/test_stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/test_tensor.py` & `bioimageio.core-0.6.4/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/weight_converter/keras/test_tensorflow.py` & `bioimageio.core-0.6.4/tests/weight_converter/keras/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/weight_converter/test_add_weights.py` & `bioimageio.core-0.6.4/tests/weight_converter/test_add_weights.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/weight_converter/torch/test_onnx.py` & `bioimageio.core-0.6.4/tests/weight_converter/torch/test_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.3/tests/weight_converter/torch/test_torchscript.py` & `bioimageio.core-0.6.4/tests/weight_converter/torch/test_torchscript.py`

 * *Files identical despite different names*

