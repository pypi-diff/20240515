# Comparing `tmp/bioimageio.spec-0.5.2.post4.tar.gz` & `tmp/bioimageio.spec-0.5.2.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.spec-0.5.2.post4.tar", last modified: Wed May  8 13:56:51 2024, max compression
+gzip compressed data, was "bioimageio.spec-0.5.2.post5.tar", last modified: Wed May 15 11:32:41 2024, max compression
```

## Comparing `bioimageio.spec-0.5.2.post4.tar` & `bioimageio.spec-0.5.2.post5.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20231 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.511952 bioimageio.spec-0.5.2.post4/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.519952 bioimageio.spec-0.5.2.post4/bioimageio/spec/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_build_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/_generated_spdx_license_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/common_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/docs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/field_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/field_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    20517 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/packaging_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/root_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validation_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validator_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/warning_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/application/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/application/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/application/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12933 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/v0_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/_v0_2_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/_v0_4_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41555 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)   101042 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/v0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/imjoy/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/imjoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/pretty_validation_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/bioimageio/spec/static/
--rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/static/spdx_licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/static/tag_categories.json
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.515952 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20231 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.515952 bioimageio.spec-0.5.2.post4/example_descriptions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.515952 bioimageio.spec-0.5.2.post4/example_descriptions/collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/collections/unet2d_nuclei_broad_coll/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.515952 bioimageio.spec-0.5.2.post4/example_descriptions/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_diff_output_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_fixed_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_fixed_shape/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_multi_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/upsample_test_model/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/upsample_test_model/upsample_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/compare_yaml_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/generate_dtype_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/generate_spec_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/generate_version_submodule_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/report_invalid_rdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/update_spdx_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_bioimageio_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_example_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/tests/test_generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_generic/test_v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_generic/test_v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/tests/test_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_file_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/tests/test_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_model/test_v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_model/test_v0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_specific_reexports_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.367090 bioimageio.spec-0.5.2.post5/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.375090 bioimageio.spec-0.5.2.post5/bioimageio/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_build_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.375090 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/_generated_spdx_license_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/common_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/field_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/field_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20517 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/packaging_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/root_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validation_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validator_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/warning_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/application/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/application/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12933 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/v0_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/_v0_2_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/_v0_4_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41555 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101042 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/model/v0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/imjoy/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/imjoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/pretty_validation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/bioimageio/spec/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/static/spdx_licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/static/tag_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-05-15 11:32:37.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/bioimageio/spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.371090 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 11:32:41.000000 bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.371090 bioimageio.spec-0.5.2.post5/example_descriptions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.371090 bioimageio.spec-0.5.2.post5/example_descriptions/collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.379089 bioimageio.spec-0.5.2.post5/example_descriptions/collections/unet2d_nuclei_broad_coll/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.371090 bioimageio.spec-0.5.2.post5/example_descriptions/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_diff_output_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_fixed_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-05-15 11:30:16.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_fixed_shape/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_multi_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/example_descriptions/models/upsample_test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/example_descriptions/models/upsample_test_model/upsample_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/compare_yaml_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/generate_dtype_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/generate_spec_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/generate_version_submodule_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/report_invalid_rdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/scripts/update_spdx_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_bioimageio_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_example_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.383089 bioimageio.spec-0.5.2.post5/tests/test_generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_generic/test_v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_generic/test_v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/tests/test_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_internal/test_version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:32:41.387089 bioimageio.spec-0.5.2.post5/tests/test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_model/test_v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_model/test_v0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-15 11:30:17.000000 bioimageio.spec-0.5.2.post5/tests/test_specific_reexports_generics.py
```

### Comparing `bioimageio.spec-0.5.2.post4/LICENSE` & `bioimageio.spec-0.5.2.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/PKG-INFO` & `bioimageio.spec-0.5.2.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.2.post4
+Version: 0.5.2.post5
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -21,17 +21,17 @@
 
 ![License](https://img.shields.io/github/license/bioimage-io/spec-bioimage-io.svg)
 ![PyPI](https://img.shields.io/pypi/v/bioimageio-spec.svg?style=popout)
 ![conda-version](https://anaconda.org/conda-forge/bioimageio.spec/badges/version.svg)
 
 # Specifications for bioimage.io
 
-This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io). 
-Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`. 
-This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik). 
+This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io).
+Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`.
+This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik).
 
 [These](https://github.com/bioimage-io/spec-bioimage-io?tab=readme-ov-file#format-version-overview) are the rules and format that bioimage.io-compatible resources must fulfill.
 
 Note that the Python package PyYAML does not support YAML 1.2 .
 We therefore use and recommend [ruyaml](https://ruyaml.readthedocs.io/en/latest/).
 For differences see <https://ruamelyaml.readthedocs.io/en/latest/pyyaml>.
 
@@ -67,28 +67,27 @@
 These are primarily intended for syntax highlighting and form generation.
 
 ## Examples
 
 We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md),
 and an [example notebook to programmatically access the models, applications, notebooks and datasets descriptions](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example/load_model_and_create_your_own.ipynb).
 
-
 ## 💁 Recommendations
 
 * Due to the limitations of storage services such as Zenodo, which does not support subfolders, it is recommended to place other files in the same directory level of the `rdf.yaml` file and try to avoid using subdirectories.
 * Use the [bioimageio.core Python package](https://github.com/bioimage-io/core-bioimage-io-python) to validate your `rdf.yaml` file.
 * bioimageio.spec keeps evolving. Try to use and upgrade to the most current format version!
 
 ## ⌨ bioimageio command-line interface (CLI)
 
 The bioimageio CLI has moved entirely to [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python).
 
 ## 🖥 Installation
 
-bioimageio.spec can be installed with either `conda` or `pip`. 
+bioimageio.spec can be installed with either `conda` or `pip`.
 We recommend installing `bioimageio.core` instead to get access to the Python programmatic features available in the BioImage.IO community:
 
 ```console
 conda install -c conda-forge bioimageio.core
 ```
 
 or
@@ -105,15 +104,14 @@
 
 or
 
 ```console
 pip install -U bioimageio.spec
 ```
 
-
 ## 🏞 Environment variables
 
 TODO: link to settings in dev docs
 
 ## 🤝 How to contribute
 
 ## ♥ Contributors
@@ -124,14 +122,19 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post5
+
+* added more information to validation summary
+* deprioritize `Path` objects in the `FileSource` union
+
 #### bioimageio.spec 0.5.2post4
 
 * resolve backup DOIs
 * fix resolving relative file paths given as strings
 * allow to bypass download and hashing of known files
 
 #### bioimageio.spec 0.5.2post3
```

### Comparing `bioimageio.spec-0.5.2.post4/README.md` & `bioimageio.spec-0.5.2.post5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ![License](https://img.shields.io/github/license/bioimage-io/spec-bioimage-io.svg)
 ![PyPI](https://img.shields.io/pypi/v/bioimageio-spec.svg?style=popout)
 ![conda-version](https://anaconda.org/conda-forge/bioimageio.spec/badges/version.svg)
 
 # Specifications for bioimage.io
 
-This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io). 
-Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`. 
-This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik). 
+This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io).
+Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`.
+This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik).
 
 [These](https://github.com/bioimage-io/spec-bioimage-io?tab=readme-ov-file#format-version-overview) are the rules and format that bioimage.io-compatible resources must fulfill.
 
 Note that the Python package PyYAML does not support YAML 1.2 .
 We therefore use and recommend [ruyaml](https://ruyaml.readthedocs.io/en/latest/).
 For differences see <https://ruamelyaml.readthedocs.io/en/latest/pyyaml>.
 
@@ -46,28 +46,27 @@
 These are primarily intended for syntax highlighting and form generation.
 
 ## Examples
 
 We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md),
 and an [example notebook to programmatically access the models, applications, notebooks and datasets descriptions](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example/load_model_and_create_your_own.ipynb).
 
-
 ## 💁 Recommendations
 
 * Due to the limitations of storage services such as Zenodo, which does not support subfolders, it is recommended to place other files in the same directory level of the `rdf.yaml` file and try to avoid using subdirectories.
 * Use the [bioimageio.core Python package](https://github.com/bioimage-io/core-bioimage-io-python) to validate your `rdf.yaml` file.
 * bioimageio.spec keeps evolving. Try to use and upgrade to the most current format version!
 
 ## ⌨ bioimageio command-line interface (CLI)
 
 The bioimageio CLI has moved entirely to [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python).
 
 ## 🖥 Installation
 
-bioimageio.spec can be installed with either `conda` or `pip`. 
+bioimageio.spec can be installed with either `conda` or `pip`.
 We recommend installing `bioimageio.core` instead to get access to the Python programmatic features available in the BioImage.IO community:
 
 ```console
 conda install -c conda-forge bioimageio.core
 ```
 
 or
@@ -84,15 +83,14 @@
 
 or
 
 ```console
 pip install -U bioimageio.spec
 ```
 
-
 ## 🏞 Environment variables
 
 TODO: link to settings in dev docs
 
 ## 🤝 How to contribute
 
 ## ♥ Contributors
@@ -103,14 +101,19 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post5
+
+* added more information to validation summary
+* deprioritize `Path` objects in the `FileSource` union
+
 #### bioimageio.spec 0.5.2post4
 
 * resolve backup DOIs
 * fix resolving relative file paths given as strings
 * allow to bypass download and hashing of known files
 
 #### bioimageio.spec 0.5.2post3
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/__init__.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_build_description.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_build_description.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import Any, Callable, List, Mapping, Optional, Type, TypeVar, Union
 
 from ._internal.common_nodes import InvalidDescr, ResourceDescrBase
 from ._internal.io import BioimageioYamlContent
 from ._internal.types import FormatVersionPlaceholder
 from ._internal.validation_context import ValidationContext, validation_context_var
-from .summary import ErrorEntry, ValidationDetail
+from .summary import (
+    WARNING_LEVEL_TO_NAME,
+    ErrorEntry,
+    ValidationContextSummary,
+    ValidationDetail,
+)
 
 ResourceDescrT = TypeVar("ResourceDescrT", bound=ResourceDescrBase)
 
 
 DISCOVER: FormatVersionPlaceholder = "discover"
 """placeholder for whatever format version an RDF specifies"""
 
@@ -78,14 +83,20 @@
     if errors:
         ret = InvalidDescr(**content)  # pyright: ignore[reportArgumentType]
         ret.validation_summary.add_detail(
             ValidationDetail(
                 name="extract fields to chose description class",
                 status="failed",
                 errors=errors,
+                context=ValidationContextSummary(
+                    perform_io_checks=context.perform_io_checks,
+                    known_files=context.known_files,
+                    root=str(context.root),
+                    warning_level=WARNING_LEVEL_TO_NAME[context.warning_level],
+                ),
             )
         )
         return ret
 
     typ = content["type"]
     rd_class = get_rd_class(typ, content["format_version"])
     rd = rd_class.load(content, context=context)
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_description.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/_generated_spdx_license_literals.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/_generated_spdx_license_literals.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/_settings.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/_settings.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/common_nodes.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/common_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     TypeVarTuple,
     Unpack,
 )
 
 from ..summary import (
     WARNING_LEVEL_TO_NAME,
     ErrorEntry,
+    ValidationContextSummary,
     ValidationDetail,
     ValidationSummary,
     WarningEntry,
 )
 from .field_warning import issue_warning
 from .io import BioimageioYamlContent
 from .node import Node as Node
@@ -322,19 +323,22 @@
 
     @model_validator(mode="after")
     def _set_init_validation_summary(self):
         context = validation_context_var.get()
         self._validation_summary = ValidationSummary(
             name="bioimageio validation",
             source_name=context.source_name,
-            status="passed",
+            type=self.type,
+            format_version=self.format_version,
+            status="failed" if isinstance(self, InvalidDescr) else "passed",
             details=[
                 ValidationDetail(
-                    name=f"initialized {self.type} {self.implemented_format_version}",
+                    name=f"initialized {self.__class__.__name__} to describe {self.type} {self.implemented_format_version}",
                     status="passed",
+                    context=None,  # context for format validation detail is identical
                 )
             ],
         )
         return self
 
     @property
     def validation_summary(self) -> ValidationSummary:
@@ -388,14 +392,20 @@
                 errors=errors,
                 name=(
                     "bioimageio.spec format validation"
                     f" {rd.type} {cls.implemented_format_version}"
                 ),
                 status="failed" if errors else "passed",
                 warnings=val_warnings,
+                context=ValidationContextSummary(
+                    perform_io_checks=context.perform_io_checks,
+                    known_files=context.known_files,
+                    root=str(context.root),
+                    warning_level=WARNING_LEVEL_TO_NAME[context.warning_level],
+                ),
             )
         )
 
         return rd
 
     @classmethod
     def _load_impl(
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/constants.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/docs_utils.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/docs_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/field_validation.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/field_validation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/field_warning.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/field_warning.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         ):
             raise ValueError(f"{absolute} does not point to an existing directory")
 
         return absolute
 
 
 FileSource = Annotated[
-    Union[FilePath, HttpUrl, RelativeFilePath, pydantic.HttpUrl],
+    Union[HttpUrl, RelativeFilePath, pydantic.HttpUrl, FilePath],
     Field(union_mode="left_to_right"),
 ]
 PermissiveFileSource = Union[FileSource, str]
 
 V_suffix = TypeVar("V_suffix", bound=FileSource)
 path_or_url_adapter = TypeAdapter(Union[FilePath, DirectoryPath, HttpUrl])
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io_basics.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io_basics.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io_utils.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/io_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/license_id.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/node.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/packaging_context.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/packaging_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/root_url.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/root_url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/types.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/url.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/utils.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validated_string.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validation_context.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validation_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validator_annotations.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/validator_annotations.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/version_type.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/version_type.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/warning_levels.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_internal/warning_levels.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_io.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/_package.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/application/__init__.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/application/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # autogen: start
 """
 implementaions of all released minor versions are available in submodules:
-- application v0_2: `bioimageio.spec.application.v0_2.ApplicationDescr` [user documentation](../../../user_docs/application_descr_v0-2.md)
-- application v0_3: `bioimageio.spec.application.v0_3.ApplicationDescr` [user documentation](../../../user_docs/application_descr_v0-3.md)
+- application v0_2: `bioimageio.spec.application.v0_2.ApplicationDescr`
+- application v0_3: `bioimageio.spec.application.v0_3.ApplicationDescr`
 """
 from typing import Union
 
 from pydantic import Discriminator
 from typing_extensions import Annotated
 
 from .v0_2 import ApplicationDescr as ApplicationDescr_v0_2
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/application/v0_2.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/application/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/application/v0_3.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/application/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/__init__.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # autogen: start
 """
 implementaions of all released minor versions are available in submodules:
-- collection v0_2: `bioimageio.spec.collection.v0_2.CollectionDescr` [user documentation](../../../user_docs/collection_descr_v0-2.md)
-- collection v0_3: `bioimageio.spec.collection.v0_3.CollectionDescr` [user documentation](../../../user_docs/collection_descr_v0-3.md)
+- collection v0_2: `bioimageio.spec.collection.v0_2.CollectionDescr`
+- collection v0_3: `bioimageio.spec.collection.v0_3.CollectionDescr`
 """
 from typing import Union
 
 from pydantic import Discriminator
 from typing_extensions import Annotated
 
 from .v0_2 import CollectionDescr as CollectionDescr_v0_2
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/v0_2.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/v0_3.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/collection/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/common.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/__init__.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # autogen: start
 """
 implementaions of all released minor versions are available in submodules:
-- dataset v0_2: `bioimageio.spec.dataset.v0_2.DatasetDescr` [user documentation](../../../user_docs/dataset_descr_v0-2.md)
-- dataset v0_3: `bioimageio.spec.dataset.v0_3.DatasetDescr` [user documentation](../../../user_docs/dataset_descr_v0-3.md)
+- dataset v0_2: `bioimageio.spec.dataset.v0_2.DatasetDescr`
+- dataset v0_3: `bioimageio.spec.dataset.v0_3.DatasetDescr`
 """
 from typing import Union
 
 from pydantic import Discriminator
 from typing_extensions import Annotated
 
 from .v0_2 import DatasetDescr as DatasetDescr_v0_2
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/v0_2.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/v0_3.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/dataset/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/_v0_2_converter.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/_v0_2_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/_v0_3_converter.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/v0_2.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/v0_3.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/generic/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/__init__.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # autogen: start
 """
 implementaions of all released minor versions are available in submodules:
-- model v0_4: `bioimageio.spec.model.v0_4.ModelDescr` [user documentation](../../../user_docs/model_descr_v0-4.md)
-- model v0_5: `bioimageio.spec.model.v0_5.ModelDescr` [user documentation](../../../user_docs/model_descr_v0-5.md)
+- model v0_4: `bioimageio.spec.model.v0_4.ModelDescr`
+- model v0_5: `bioimageio.spec.model.v0_5.ModelDescr`
 """
 from typing import Union
 
 from pydantic import Discriminator
 from typing_extensions import Annotated
 
 from .v0_4 import ModelDescr as ModelDescr_v0_4
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/_v0_3_converter.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/_v0_4_converter.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/_v0_4_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/v0_4.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/v0_5.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/model/v0_5.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/__init__.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # autogen: start
 """
 implementaions of all released minor versions are available in submodules:
-- notebook v0_2: `bioimageio.spec.notebook.v0_2.NotebookDescr` [user documentation](../../../user_docs/notebook_descr_v0-2.md)
-- notebook v0_3: `bioimageio.spec.notebook.v0_3.NotebookDescr` [user documentation](../../../user_docs/notebook_descr_v0-3.md)
+- notebook v0_2: `bioimageio.spec.notebook.v0_2.NotebookDescr`
+- notebook v0_3: `bioimageio.spec.notebook.v0_3.NotebookDescr`
 """
 from typing import Union
 
 from pydantic import Discriminator
 from typing_extensions import Annotated
 
 from .v0_2 import NotebookDescr as NotebookDescr_v0_2
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/v0_2.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/v0_3.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/notebook/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/pretty_validation_errors.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/pretty_validation_errors.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/static/spdx_licenses.json` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/static/spdx_licenses.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/static/tag_categories.json` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/static/tag_categories.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio/spec/summary.py` & `bioimageio.spec-0.5.2.post5/bioimageio/spec/summary.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 from itertools import chain
 from pathlib import Path
 from types import MappingProxyType
-from typing import Any, Iterable, List, Literal, Mapping, Tuple, Union, no_type_check
+from typing import (
+    Any,
+    Iterable,
+    List,
+    Literal,
+    Mapping,
+    Optional,
+    Tuple,
+    Union,
+    no_type_check,
+)
 
 import rich.console
 import rich.markdown
 from pydantic import BaseModel, Field, model_validator
 from pydantic_core.core_schema import ErrorType
 from typing_extensions import TypedDict, assert_never
 
@@ -93,19 +103,27 @@
 
 
 class InstalledPackage(TypedDict):
     name: str
     version: str
 
 
+class ValidationContextSummary(TypedDict):
+    perform_io_checks: bool
+    known_files: Mapping[str, str]
+    root: str
+    warning_level: str
+
+
 class ValidationDetail(BaseModel, extra="allow"):
     name: str
     status: Literal["passed", "failed"]
     errors: List[ErrorEntry] = Field(default_factory=list)
     warnings: List[WarningEntry] = Field(default_factory=list)
+    context: Optional[ValidationContextSummary] = None
 
     def __str__(self):
         return f"{self.__class__.__name__}:\n" + self.format()
 
     @property
     def status_icon(self):
         if self.status == "passed":
@@ -156,14 +174,16 @@
             else "" + f"\n{indent}warnings:\n{ws}" if ws else ""
         )
 
 
 class ValidationSummary(BaseModel, extra="allow"):
     name: str
     source_name: str
+    type: str
+    format_version: str
     status: Literal["passed", "failed"]
     details: List[ValidationDetail]
     env: List[InstalledPackage] = Field(
         default_factory=lambda: [
             InstalledPackage(name="bioimageio.spec", version=VERSION)
         ]
     )
@@ -200,38 +220,53 @@
             [
                 " | ".join(row[i].ljust(col_widths[i]) for i in range(n_cols))
                 for row in rows[1:]
             ]
         )
         return "\n| " + " |\n| ".join(lines) + " |\n"
 
-    def _format_env(self):
-        if not self.env:
-            return ""
-
-        rows = [["package", "version"]] + [[e["name"], e["version"]] for e in self.env]
-        return self._format_md_table(rows)
-
     def format(
         self,
         hide_tracebacks: bool = False,
         hide_source: bool = False,
         hide_env: bool = False,
         root_loc: Loc = (),
     ) -> str:
-        indent = "   " if root_loc else ""
-        src = "" if hide_source else f"\n{indent}source: {self.source_name}"
-        env = "" if hide_env else self._format_env()
-        details = [["❓", "location", "detail"]]
+        info = self._format_md_table(
+            [[self.status_icon, f"{self.name.strip('.').strip()} {self.status}"]]
+            + ([] if hide_source else [["source", self.source_name]])
+            + [
+                ["format version", f"{self.type} {self.format_version}"],
+            ]
+            + ([] if hide_env else [[e["name"], e["version"]] for e in self.env])
+        )
 
         def format_loc(loc: Loc):
             return "`" + (".".join(map(str, root_loc + loc)) or ".") + "`"
 
-        for d in self.details:
+        details = [["❓", "location", "detail"]]
+        for i, d in enumerate(self.details):
             details.append([d.status_icon, "", d.name])
+            if d.context is not None:
+                details.append(
+                    [
+                        "🔍",
+                        "context.perform_io_checks",
+                        str(d.context["perform_io_checks"]),
+                    ]
+                )
+                if d.context["perform_io_checks"]:
+                    details.append(["🔍", "context.root", d.context["root"]])
+                    for kfn, sha in d.context["known_files"].items():
+                        details.append(["🔍", f"context.known_files.{kfn}", sha])
+
+                details.append(
+                    ["🔍", "context.warning_level", d.context["warning_level"]]
+                )
+
             for entry in d.errors:
                 details.append(["❌", format_loc(entry.loc), entry.msg])
                 if hide_tracebacks:
                     continue
 
                 for tb in entry.traceback:
                     if not (tb_stripped := tb.strip()):
@@ -257,26 +292,21 @@
                     if tb_lines:
                         tb_rest = "<br>`" + "`<br>`".join(tb_lines) + "`"
                     else:
                         tb_rest = ""
 
                     details.append(["", "", first_tb_line + tb_rest])
 
-            if d.errors:
-                details.append(["", "", ""])
-
             for entry in d.warnings:
                 details.append(["⚠", format_loc(entry.loc), entry.msg])
-            if d.warnings:
+
+            if i != len(details) - 1:
                 details.append(["", "", ""])
 
-        return (
-            f"{indent}{self.status_icon} {self.name.strip('.')}: {self.status}\n"
-            + f"{src}{env}\n{self._format_md_table(details)}"
-        )
+        return f"{info}{self._format_md_table(details)}"
 
     @no_type_check
     def display(self) -> None:
         formatted = self.format()
         try:
             from IPython.core.getipython import get_ipython
             from IPython.display import Markdown, display
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/PKG-INFO` & `bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.2.post4
+Version: 0.5.2.post5
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -21,17 +21,17 @@
 
 ![License](https://img.shields.io/github/license/bioimage-io/spec-bioimage-io.svg)
 ![PyPI](https://img.shields.io/pypi/v/bioimageio-spec.svg?style=popout)
 ![conda-version](https://anaconda.org/conda-forge/bioimageio.spec/badges/version.svg)
 
 # Specifications for bioimage.io
 
-This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io). 
-Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`. 
-This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik). 
+This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io).
+Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`.
+This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik).
 
 [These](https://github.com/bioimage-io/spec-bioimage-io?tab=readme-ov-file#format-version-overview) are the rules and format that bioimage.io-compatible resources must fulfill.
 
 Note that the Python package PyYAML does not support YAML 1.2 .
 We therefore use and recommend [ruyaml](https://ruyaml.readthedocs.io/en/latest/).
 For differences see <https://ruamelyaml.readthedocs.io/en/latest/pyyaml>.
 
@@ -67,28 +67,27 @@
 These are primarily intended for syntax highlighting and form generation.
 
 ## Examples
 
 We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md),
 and an [example notebook to programmatically access the models, applications, notebooks and datasets descriptions](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example/load_model_and_create_your_own.ipynb).
 
-
 ## 💁 Recommendations
 
 * Due to the limitations of storage services such as Zenodo, which does not support subfolders, it is recommended to place other files in the same directory level of the `rdf.yaml` file and try to avoid using subdirectories.
 * Use the [bioimageio.core Python package](https://github.com/bioimage-io/core-bioimage-io-python) to validate your `rdf.yaml` file.
 * bioimageio.spec keeps evolving. Try to use and upgrade to the most current format version!
 
 ## ⌨ bioimageio command-line interface (CLI)
 
 The bioimageio CLI has moved entirely to [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python).
 
 ## 🖥 Installation
 
-bioimageio.spec can be installed with either `conda` or `pip`. 
+bioimageio.spec can be installed with either `conda` or `pip`.
 We recommend installing `bioimageio.core` instead to get access to the Python programmatic features available in the BioImage.IO community:
 
 ```console
 conda install -c conda-forge bioimageio.core
 ```
 
 or
@@ -105,15 +104,14 @@
 
 or
 
 ```console
 pip install -U bioimageio.spec
 ```
 
-
 ## 🏞 Environment variables
 
 TODO: link to settings in dev docs
 
 ## 🤝 How to contribute
 
 ## ♥ Contributors
@@ -124,14 +122,19 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post5
+
+* added more information to validation summary
+* deprioritize `Path` objects in the `FileSource` union
+
 #### bioimageio.spec 0.5.2post4
 
 * resolve backup DOIs
 * fix resolving relative file paths given as strings
 * allow to bypass download and hashing of known files
 
 #### bioimageio.spec 0.5.2post3
```

### Comparing `bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/SOURCES.txt` & `bioimageio.spec-0.5.2.post5/bioimageio.spec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py` & `bioimageio.spec-0.5.2.post5/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py` & `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_fixed_shape/unet.py` & `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_fixed_shape/unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py` & `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/unet2d.py` & `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py` & `bioimageio.spec-0.5.2.post5/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/pyproject.toml` & `bioimageio.spec-0.5.2.post5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/scripts/compare_yaml_syntax.py` & `bioimageio.spec-0.5.2.post5/scripts/compare_yaml_syntax.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/scripts/generate_json_schemas.py` & `bioimageio.spec-0.5.2.post5/scripts/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/scripts/generate_spec_documentation.py` & `bioimageio.spec-0.5.2.post5/scripts/generate_spec_documentation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/scripts/generate_version_submodule_imports.py` & `bioimageio.spec-0.5.2.post5/scripts/generate_version_submodule_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,15 @@
         )
         self.all_version_modules_imports = "\n".join(avmi)
 
         self.package_path = (ROOT_PATH / "bioimageio" / "spec" / self.target).resolve()
         self.submodule_list = "\n".join(
             [
                 f"- {self.target} {vm}: `bioimageio.spec.{self.target}.{vm}."
-                + f"{self.target_node}` [user documentation](../../../user_docs/"
-                + f"{self.target}_descr_{vm.replace('_', '-')}.md)"
+                + f"{self.target_node}`"
                 for vm in self.all_version_modules
             ]
         )
 
 
 def process(info: Info, check: bool):
     package_init = info.package_path / "__init__.py"
```

### Comparing `bioimageio.spec-0.5.2.post4/scripts/report_invalid_rdfs.py` & `bioimageio.spec-0.5.2.post5/scripts/report_invalid_rdfs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/scripts/update_spdx_licenses.py` & `bioimageio.spec-0.5.2.post5/scripts/update_spdx_licenses.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/setup.py` & `bioimageio.spec-0.5.2.post5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     packages=find_namespace_packages(exclude=["tests"]),  # Required
     install_requires=[
-        "annotated-types>=0.5.0",
+        "annotated-types>=0.5.0,<1",
         "email_validator",
         "imageio",
         "loguru",
         "numpy>=1.21",
         "packaging>=17.0",
-        "pooch",
+        "pooch>=1.5,<2",
         "pydantic-settings",
-        "pydantic>=2.6.3",
+        "pydantic>=2.6.3,<3",
         "python-dateutil",
         "python-dotenv",
         "requests",
         "rich",
         "ruyaml",
         "tqdm",
         "typing-extensions",
```

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_bioimageio_collection.py` & `bioimageio.spec-0.5.2.post5/tests/test_bioimageio_collection.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_description.py` & `bioimageio.spec-0.5.2.post5/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_example_specs.py` & `bioimageio.spec-0.5.2.post5/tests/test_example_specs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_generic/test_v0_2.py` & `bioimageio.spec-0.5.2.post5/tests/test_generic/test_v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_generic/test_v0_3.py` & `bioimageio.spec-0.5.2.post5/tests/test_generic/test_v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_constants.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_file_source.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_file_source.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_io.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_license_id.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_node.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_types.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_utils.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_validate.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_validate.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_internal/test_validated_string.py` & `bioimageio.spec-0.5.2.post5/tests/test_internal/test_validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_io.py` & `bioimageio.spec-0.5.2.post5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_model/test_v0_4.py` & `bioimageio.spec-0.5.2.post5/tests/test_model/test_v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_model/test_v0_5.py` & `bioimageio.spec-0.5.2.post5/tests/test_model/test_v0_5.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_package.py` & `bioimageio.spec-0.5.2.post5/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post4/tests/test_specific_reexports_generics.py` & `bioimageio.spec-0.5.2.post5/tests/test_specific_reexports_generics.py`

 * *Files identical despite different names*

