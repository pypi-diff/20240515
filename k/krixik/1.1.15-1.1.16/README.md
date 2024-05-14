# Comparing `tmp/krixik-1.1.15.tar.gz` & `tmp/krixik-1.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krixik-1.1.15.tar", last modified: Wed May  8 20:30:22 2024, max compression
+gzip compressed data, was "krixik-1.1.16.tar", last modified: Tue May 14 22:06:18 2024, max compression
```

## Comparing `krixik-1.1.15.tar` & `krixik-1.1.16.tar`

### file list

```diff
@@ -1,233 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.473335 krixik-1.1.15/
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 20:30:22.473335 krixik-1.1.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-08 20:30:13.000000 krixik-1.1.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.445335 krixik-1.1.15/krixik/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/__base__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.445335 krixik-1.1.15/krixik/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.445335 krixik-1.1.15/krixik/modules/caption/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/caption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/caption/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/caption/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/caption/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.449335 krixik-1.1.15/krixik/modules/json-to-txt/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/json-to-txt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/json-to-txt/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/json-to-txt/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/json-to-txt/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/json-to-txt/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.449335 krixik-1.1.15/krixik/modules/keyword-db/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/keyword-db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/keyword-db/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/keyword-db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/keyword-db/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.449335 krixik-1.1.15/krixik/modules/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/ocr/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/ocr/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/ocr/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.449335 krixik-1.1.15/krixik/modules/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/parser/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/parser/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/parser/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.449335 krixik-1.1.15/krixik/modules/sentiment/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/sentiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/sentiment/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/sentiment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/sentiment/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.453335 krixik-1.1.15/krixik/modules/summarize/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/summarize/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/summarize/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/summarize/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.453335 krixik-1.1.15/krixik/modules/text-embedder/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/text-embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/text-embedder/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/text-embedder/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/text-embedder/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/text-embedder/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.453335 krixik-1.1.15/krixik/modules/transcribe/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/transcribe/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/transcribe/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/transcribe/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.453335 krixik-1.1.15/krixik/modules/translate/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/translate/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/translate/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/translate/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.453335 krixik-1.1.15/krixik/modules/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/utilities/io_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/utilities/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/utilities/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/utilities/module_selections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/utilities/read_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.457335 krixik-1.1.15/krixik/modules/vector-db/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/vector-db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/vector-db/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/vector-db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/modules/vector-db/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.457335 krixik-1.1.15/krixik/pipeline_builder/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.457335 krixik-1.1.15/krixik/pipeline_builder/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/utilities/chain_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/utilities/config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/utilities/input_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/utilities/name_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/utilities/savepath_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_builder/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.457335 krixik-1.1.15/krixik/pipeline_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.457335 krixik-1.1.15/krixik/pipeline_examples/single_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/caption.yml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/json-to-txt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/keyword-db.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/ocr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/parser.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/sentiment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/summarize.yml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/text-embedder.yml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/transcribe.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/translate.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.457335 krixik-1.1.15/krixik/pipeline_examples/single_module/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/utilities/generate_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/pipeline_examples/single_module/vector-db.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.461335 krixik-1.1.15/krixik/system_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25795 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.461335 krixik-1.1.15/krixik/system_builder/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/check_process_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/fetch_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/keyword_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/list_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/semantic_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/show_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/functions/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.461335 krixik-1.1.15/krixik/system_builder/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/system_builder/utilities/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.461335 krixik-1.1.15/krixik/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/cleaners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.465335 krixik-1.1.15/krixik/utilities/converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/default_clean_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/docx_to_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/pdf_to_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/pptx_to_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/read_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/unclean_to_clean_txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.465335 krixik-1.1.15/krixik/utilities/converters/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/utilities/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/converters/video_to_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/file_name_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/tree_illustrator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1486 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.465335 krixik-1.1.15/krixik/utilities/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.465335 krixik-1.1.15/krixik/utilities/validators/data/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/npy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/pptx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.465335 krixik-1.1.15/krixik/utilities/validators/data/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/utilities/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/utilities/read_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/data/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.465335 krixik-1.1.15/krixik/utilities/validators/system/
--rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.469335 krixik-1.1.15/krixik/utilities/validators/system/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/clean_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/expire_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/extension_enforcer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1237 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/file_description.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2773 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/file_ids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5749 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/file_names.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4957 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/file_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/k_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/local_file_path.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/local_save_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/lower_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/max_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/process_switches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/symbolic_path_splitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9255 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/symbolic_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/timestamp_bookends.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/use_default_clean_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/user_secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.469335 krixik-1.1.15/krixik/utilities/validators/system/base/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/base/wait_for_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.469335 krixik-1.1.15/krixik/utilities/validators/system/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.473335 krixik-1.1.15/krixik/utilities/validators/system/data/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/audio/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/audio/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.473335 krixik-1.1.15/krixik/utilities/validators/system/data/image/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/image/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/image/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/image/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.473335 krixik-1.1.15/krixik/utilities/validators/system/data/json/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/json/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/json/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/json/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.473335 krixik-1.1.15/krixik/utilities/validators/system/data/npy/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/npy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/npy/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/npy/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.473335 krixik-1.1.15/krixik/utilities/validators/system/data/text/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/text/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/text/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/text/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.473335 krixik-1.1.15/krixik/utilities/validators/system/data/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/system/data/utilities/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.473335 krixik-1.1.15/krixik/utilities/validators/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-08 20:30:13.000000 krixik-1.1.15/krixik/utilities/validators/utilities/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:30:22.445335 krixik-1.1.15/krixik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 20:30:22.000000 krixik-1.1.15/krixik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-05-08 20:30:22.000000 krixik-1.1.15/krixik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:30:22.000000 krixik-1.1.15/krixik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-08 20:30:22.000000 krixik-1.1.15/krixik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 20:30:22.000000 krixik-1.1.15/krixik.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:30:22.477335 krixik-1.1.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-08 20:30:13.000000 krixik-1.1.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-14 22:06:18.110043 krixik-1.1.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-05-14 22:06:07.000000 krixik-1.1.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.082043 krixik-1.1.16/krixik/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/__base__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.082043 krixik-1.1.16/krixik/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.082043 krixik-1.1.16/krixik/modules/caption/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/caption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/caption/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/caption/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/caption/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/json-to-txt/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/keyword-db/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/keyword-db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/keyword-db/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/keyword-db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/keyword-db/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/ocr/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/ocr/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/ocr/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/sentiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/sentiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/sentiment/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/sentiment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/sentiment/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/summarize/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/summarize/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/summarize/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/summarize/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/text-embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/transcribe/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/transcribe/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/transcribe/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/transcribe/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/translate/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/translate/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/translate/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/io_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/module_selections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/read_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/vector-db/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/vector-db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/vector-db/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/vector-db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/vector-db/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/pipeline_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/pipeline_builder/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/chain_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/input_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/name_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/savepath_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/pipeline_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/pipeline_examples/single_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/caption.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/json-to-txt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/keyword-db.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/ocr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/parser.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/sentiment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/summarize.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/text-embedder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/transcribe.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/translate.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/pipeline_examples/single_module/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/utilities/generate_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/vector-db.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/system_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26703 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/system_builder/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/check_process_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/fetch_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/keyword_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/semantic_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/show_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/system_builder/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/cleaners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/utilities/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/default_clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/docx_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/pdf_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/pptx_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/read_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/unclean_to_clean_txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/utilities/converters/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/utilities/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/video_to_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/file_name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/tree_illustrator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1486 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.102043 krixik-1.1.16/krixik/utilities/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.102043 krixik-1.1.16/krixik/utilities/validators/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.102043 krixik-1.1.16/krixik/utilities/validators/data/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/utilities/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/utilities/read_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.102043 krixik-1.1.16/krixik/utilities/validators/system/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.106043 krixik-1.1.16/krixik/utilities/validators/system/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/download_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/expire_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/extension_enforcer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1237 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/file_description.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2773 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/file_ids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5749 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/file_names.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4957 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/file_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/k_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/local_file_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/local_save_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/lower_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/max_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/process_switches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/symbolic_path_splitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9255 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/symbolic_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/timestamp_bookends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/use_default_clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/user_secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.106043 krixik-1.1.16/krixik/utilities/validators/system/base/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/wait_for_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.106043 krixik-1.1.16/krixik/utilities/validators/system/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.106043 krixik-1.1.16/krixik/utilities/validators/system/data/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/audio/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/audio/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/image/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/image/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/image/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/json/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/json/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/json/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/json/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/npy/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/npy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/npy/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/npy/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/text/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/text/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/text/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.082043 krixik-1.1.16/krixik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 22:06:18.110043 krixik-1.1.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 22:06:07.000000 krixik-1.1.16/setup.py
```

### Comparing `krixik-1.1.15/PKG-INFO` & `krixik-1.1.16/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krixik
-Version: 1.1.15
+Version: 1.1.16
 Summary: Easily assemble and serverlessly consume modular AI pipelines through secure Python APIs.
 Home-page: https://github.com/krixik-ai/krixik-cli
 Author: Jeremy Watt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: linting
 Provides-Extra: testing
@@ -94,26 +94,26 @@
 If you've misplaced your secrets, please reach out to us directly.
 
 
 ### Building your first pipeline
 
 Let's build a simple transcription pipeline consisting of a single `transcribe` module.
 
-Import the required Krixik module and pipeline tooling required to instantiate modules and create custom pipelines: the `Module` and `CreatePipeline` class objects. Then create your module and your pipeline.
+Import the required Krixik module and pipeline tooling required to instantiate modules and create custom pipelines: the `Module` and `BuildPipeline` class objects. Then create your module and your pipeline.
 
 ```python
 # import custom pipeline builder tools
 from krixik.pipeline_builder.module import Module
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 
 # instantiate module
 module_1 = Module(name="transcribe")
 
 # create custom pipeline object with above module
-custom_pipeline_1 = CreatePipeline(name='my-transcribe-pipeline-1', 
+custom_pipeline_1 = BuildPipeline(name='my-transcribe-pipeline-1', 
                                    module_chain=[module_1])
 ```
 
 With your custom pipeline defined you can load it for use with the `load_pipeline` method.
 
 ```python
 my_pipeline_1 = krixik.load_pipeline(pipeline=custom_pipeline_1)
@@ -142,25 +142,25 @@
 
 Locally creating and testing this sequence of steps would be time consuming—orchestrating them in a secure production service even more so. And that's without trying to make it all serverless.
 
 With **Krixik**, however, you can rapidly add this functionality to your original pipeline by just adding a few modules. Syntax remains as above:
 
 ```python
 from krixik.pipeline_builder.module import Module
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 
 # instantiate modules
 module_a = Module(name="transcribe")
 module_b = Module(name="json-to-txt")
 module_c = Module(name="parser")
 module_d = Module(name="text-embedder")
 module_e = Module(name="vector-search")
 
 # create custom pipeline object with the above modules in sequence
-custom_pipeline_2 = CreatePipeline(name='my-transcribe-pipeline-2', 
+custom_pipeline_2 = BuildPipeline(name='my-transcribe-pipeline-2', 
                         module_chain=[module_a, module_b, module_c, module_d, module_e])
 
 # pass the custom object to the krixik operator
 my_pipeline_2 = krixik.load_pipeline(pipeline=custom_pipeline_2)
 ```
 
 Let's process a file through your new pipeline.
```

### Comparing `krixik-1.1.15/README.md` & `krixik-1.1.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,26 +83,26 @@
 If you've misplaced your secrets, please reach out to us directly.
 
 
 ### Building your first pipeline
 
 Let's build a simple transcription pipeline consisting of a single `transcribe` module.
 
-Import the required Krixik module and pipeline tooling required to instantiate modules and create custom pipelines: the `Module` and `CreatePipeline` class objects. Then create your module and your pipeline.
+Import the required Krixik module and pipeline tooling required to instantiate modules and create custom pipelines: the `Module` and `BuildPipeline` class objects. Then create your module and your pipeline.
 
 ```python
 # import custom pipeline builder tools
 from krixik.pipeline_builder.module import Module
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 
 # instantiate module
 module_1 = Module(name="transcribe")
 
 # create custom pipeline object with above module
-custom_pipeline_1 = CreatePipeline(name='my-transcribe-pipeline-1', 
+custom_pipeline_1 = BuildPipeline(name='my-transcribe-pipeline-1', 
                                    module_chain=[module_1])
 ```
 
 With your custom pipeline defined you can load it for use with the `load_pipeline` method.
 
 ```python
 my_pipeline_1 = krixik.load_pipeline(pipeline=custom_pipeline_1)
@@ -131,25 +131,25 @@
 
 Locally creating and testing this sequence of steps would be time consuming—orchestrating them in a secure production service even more so. And that's without trying to make it all serverless.
 
 With **Krixik**, however, you can rapidly add this functionality to your original pipeline by just adding a few modules. Syntax remains as above:
 
 ```python
 from krixik.pipeline_builder.module import Module
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 
 # instantiate modules
 module_a = Module(name="transcribe")
 module_b = Module(name="json-to-txt")
 module_c = Module(name="parser")
 module_d = Module(name="text-embedder")
 module_e = Module(name="vector-search")
 
 # create custom pipeline object with the above modules in sequence
-custom_pipeline_2 = CreatePipeline(name='my-transcribe-pipeline-2', 
+custom_pipeline_2 = BuildPipeline(name='my-transcribe-pipeline-2', 
                         module_chain=[module_a, module_b, module_c, module_d, module_e])
 
 # pass the custom object to the krixik operator
 my_pipeline_2 = krixik.load_pipeline(pipeline=custom_pipeline_2)
 ```
 
 Let's process a file through your new pipeline.
```

### Comparing `krixik-1.1.15/krixik/main.py` & `krixik-1.1.16/krixik/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Optional
 from krixik.__version__ import __version__
 import tempfile
 import types
 from krixik.utilities.utilities import classproperty
 from krixik.modules import available_modules, get_module_details
 from krixik.system_builder.functions.checkin import checkin
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 from krixik.system_builder.base import KrixikBasePipeline
 from krixik.system_builder.functions.semantic_search import semantic_search
 from krixik.system_builder.functions.keyword_search import keyword_search
 from krixik.pipeline_builder.utilities.config_checker import config_check
 from krixik.pipeline_builder.module import Module
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 
 
 class krixik:
     """Main class for krixik pipeline selection and initialization"""
 
     __api_key = None
     __api_url = None
@@ -63,41 +63,41 @@
             raise TypeError("module_chain must be a list of strings")
         for item in module_chain:
             if not isinstance(item, str):
                 raise TypeError(f"module_chain must be a list of strings - the following item in it is not a string - {item}")
             if item not in available_modules:
                 raise ValueError(f"module_chain item - {item} - is not a currently one of the currently available modules -{available_modules}")
         module_chain_ = [Module(m_name) for m_name in module_chain]
-        custom = CreatePipeline(name=name, module_chain=module_chain_)
+        custom = BuildPipeline(name=name, module_chain=module_chain_)
         return cls.load_pipeline(pipeline=custom)
 
     @classmethod
-    def load_pipeline(cls, *, config_path: Optional[str] = None, pipeline: Optional[CreatePipeline] = None) -> object:
+    def load_pipeline(cls, *, config_path: Optional[str] = None, pipeline: Optional[BuildPipeline] = None) -> object:
         """load pipeline: from object or configuration file
 
         Parameters
         ----------
         config_path : str
             path to pipeline configuration file
-        pipeline: CreatePipeline
+        pipeline: BuildPipeline
             pipeline object
         """
         # only one of config_path or pipeline can be passed
         if config_path is None and pipeline is None:
             raise ValueError("config_path or pipeline must be passed")
 
         if config_path is not None and pipeline is not None:
             raise ValueError("only one of config_path or pipeline can be passed, not both")
 
         if config_path is not None:
             config_check(config_path)
-            custom_pipeline = CreatePipeline(config_path=config_path)
+            custom_pipeline = BuildPipeline(config_path=config_path)
         else:
-            if not isinstance(pipeline, CreatePipeline):
-                raise TypeError(f"pipeline - {pipeline} not proper CreatePipeline object")
+            if not isinstance(pipeline, BuildPipeline):
+                raise TypeError(f"input pipeline not proper BuildPipeline object")
             custom_pipeline = pipeline
 
         # pass init
         init_data = cls.check_init_data()
 
         # instantiate krixik server pipeline object
         pipeline_object = KrixikBasePipeline(
```

### Comparing `krixik-1.1.15/krixik/modules/__init__.py` & `krixik-1.1.16/krixik/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/caption/io.py` & `krixik-1.1.16/krixik/modules/caption/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/caption/models.py` & `krixik-1.1.16/krixik/modules/caption/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/json-to-txt/io.py` & `krixik-1.1.16/krixik/modules/json-to-txt/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/json-to-txt/models.py` & `krixik-1.1.16/krixik/modules/json-to-txt/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/json-to-txt/params.py` & `krixik-1.1.16/krixik/modules/json-to-txt/params.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/keyword-db/io.py` & `krixik-1.1.16/krixik/modules/keyword-db/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
     @property
     def process_type(self):
         return str(self.__annotations__[self.process_key]) if self.process_key is not None else None
 
     @property
     def data_example(self):
-        return None
+        return "this will be a database"
```

### Comparing `krixik-1.1.15/krixik/modules/keyword-db/models.py` & `krixik-1.1.16/krixik/modules/keyword-db/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/ocr/io.py` & `krixik-1.1.16/krixik/modules/ocr/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/ocr/models.py` & `krixik-1.1.16/krixik/modules/ocr/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/parser/io.py` & `krixik-1.1.16/krixik/modules/parser/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/parser/models.py` & `krixik-1.1.16/krixik/modules/parser/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/parser/params.py` & `krixik-1.1.16/krixik/modules/parser/params.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/sentiment/io.py` & `krixik-1.1.16/krixik/modules/translate/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Literal, Any, Optional
+from typing import Any, Literal, Optional
 
 
 @dataclass
 class InputStructure:
     format: Literal["json"] = "json"
     filename: str = "filename_example.json"
     process_key: str = "snippet"
```

### Comparing `krixik-1.1.15/krixik/modules/sentiment/models.py` & `krixik-1.1.16/krixik/modules/sentiment/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/summarize/io.py` & `krixik-1.1.16/krixik/modules/summarize/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/summarize/models.py` & `krixik-1.1.16/krixik/modules/summarize/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/text-embedder/io.py` & `krixik-1.1.16/krixik/modules/text-embedder/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/text-embedder/models.py` & `krixik-1.1.16/krixik/modules/text-embedder/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/text-embedder/module.yml` & `krixik-1.1.16/krixik/modules/text-embedder/module.yml`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/transcribe/io.py` & `krixik-1.1.16/krixik/modules/transcribe/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/transcribe/models.py` & `krixik-1.1.16/krixik/modules/transcribe/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/translate/io.py` & `krixik-1.1.16/krixik/modules/sentiment/io.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, Literal, Optional
+from typing import Literal, Any, Optional
 
 
 @dataclass
 class InputStructure:
     format: Literal["json"] = "json"
     filename: str = "filename_example.json"
     process_key: str = "snippet"
@@ -32,11 +32,8 @@
 
     @property
     def process_type(self):
         return str(self.__annotations__[self.process_key]) if self.process_key is not None else None
 
     @property
     def data_example(self):
-        return {
-            "snippet": self.snippet,
-            "other": self.other,
-        }
+        return {"snippet": self.snippet, "positive": 0.33, "negative": 0.33, "neutral": 0.33}
```

### Comparing `krixik-1.1.15/krixik/modules/translate/models.py` & `krixik-1.1.16/krixik/modules/translate/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/utilities/decorators.py` & `krixik-1.1.16/krixik/modules/utilities/decorators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import inspect
 from functools import wraps
 from krixik.modules.utilities.module_selections import (
     pipeline_selection_setup,
 )
 from krixik.utilities.utilities import get_input
 from krixik.utilities.utilities import vprint
@@ -21,14 +22,21 @@
             verbose = get_input("verbose", signature, kwargs, default_value=True)
             hydrated_modules = pipeline_selection_setup(pipeline_ordered_modules, modules)
             kwargs["modules"] = hydrated_modules
 
             if "local_file_path" in list(kwargs.keys()):
                 local_file_path = get_input("local_file_path", signature, kwargs)
                 is_valid_json_input(pipeline_ordered_modules[0], local_file_path)
+                if pipeline_ordered_modules[0] == "summarize":
+                    file_size = os.path.getsize(local_file_path) / (1024 * 1024)
+                    summarizer_limit = 0.25
+                    if file_size > summarizer_limit:
+                        raise ValueError(
+                            f"summarize models can only intake files with a maximum size of {summarizer_limit}MB at present, the size of your input is {round(file_size,2)}MB"
+                        )
 
             if modules != hydrated_modules:
                 vprint(
                     f"INFO: hydrated input modules: {hydrated_modules}",
                     verbose=verbose,
                 )
```

### Comparing `krixik-1.1.15/krixik/modules/utilities/io_validator.py` & `krixik-1.1.16/krixik/modules/utilities/io_validator.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/utilities/model.py` & `krixik-1.1.16/krixik/modules/utilities/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     if model not in available_models:
         raise ValueError(f"model: must be one of {available_models} - the model entered is not in this required form - {model}")
 
 
 def model_standardizer(model_selection: dict, default_model: str, default_params: dict) -> dict:
     if not isinstance(model_selection, dict):
         raise TypeError(
-            f"model_selection: must be a dictionary with unique key(s): model, params - the model_selection entered is not in this required form - {model_selection}"
+            f"a module's model selection must have only two keys: model, params - the model_selection entered is not in this required form - {model_selection}"
         )
     keys = list(model_selection.keys())
     if len(keys) > 2:
         raise ValueError(
-            f"model_selection: must have only two keys: model, params - the model_selection entered is not in this required form - {model_selection}"
+            f"a module's model selection must have only two keys: model, params - the model_selection entered is not in this required form - {model_selection}"
         )
     if len(set(keys) - set(["model", "params"])) > 0:
         raise ValueError(
-            f"model_selection: must have only two keys: model, params - the model_selection entered is not in this required form - {model_selection}"
+            f"a module's model selection must have only two keys: model, params - the model_selection entered is not in this required form - {model_selection}"
         )
     if "model" not in keys:
         model_selection["model"] = default_model
     if "params" not in keys:
         model_selection["params"] = default_params
     if len(model_selection["params"]) == 0:
         model_selection["params"] = default_params
```

### Comparing `krixik-1.1.15/krixik/modules/utilities/module_selections.py` & `krixik-1.1.16/krixik/modules/utilities/module_selections.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/utilities/read_config.py` & `krixik-1.1.16/krixik/modules/utilities/read_config.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/modules/vector-db/io.py` & `krixik-1.1.16/krixik/modules/vector-db/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
     @property
     def process_type(self):
         return str(self.__annotations__[self.process_key]) if self.process_key is not None else None
 
     @property
     def data_example(self):
-        return None
+        return "this will be a database"
```

### Comparing `krixik-1.1.15/krixik/modules/vector-db/models.py` & `krixik-1.1.16/krixik/modules/vector-db/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/pipeline_builder/module.py` & `krixik-1.1.16/krixik/pipeline_builder/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if not isinstance(module_type, str):
             raise ValueError("module_type must be a string")
 
         self.name = module_type
 
         # check validity of input module
         if self.name not in available_modules:
-            raise Exception(f"user defined module {self.name} does not exist")
+            raise Exception(f"user defined module '{self.name}' does not exist")
 
         # define config and io paths
         self.__module_config_path = library_base_dir + f"/modules/{self.name}/module.yml"
         self.__io_module_path = f"krixik.modules.{self.name}.io"
 
         # load in module config
         self.__module_config = None
```

### Comparing `krixik-1.1.15/krixik/pipeline_builder/pipeline.py` & `krixik-1.1.16/krixik/pipeline_builder/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import yaml
 from typing import Optional, List
 from collections import OrderedDict
 from krixik.pipeline_builder.module import Module
 from krixik.utilities.validators.data.utilities.decorators import datatype_validator
 from krixik.utilities.validators.data.utilities.read_config import check_inverse_config
 from krixik.pipeline_builder.utilities.config_checker import config_check
@@ -29,28 +30,31 @@
         return {key: convert_to_dict(value) for key, value in obj.items()}
     elif isinstance(obj, list):
         return [convert_to_dict(item) for item in obj]
     else:
         return obj
 
 
-class CreatePipeline:
+class BuildPipeline:
     def __init__(
         self,
         name: Optional[str] = None,
         module_chain: Optional[List[Module]] = None,
         config_path: Optional[str] = None,
     ) -> None:
         self.name = name
         self.__module_chain = []
         self.__module_chain_names = []
         self.__module_chain_output_process_keys = []
         self.__pipeline_config = None
         self.__module_chain_configs = []
 
+        if module_chain is not None and config_path is not None:
+            raise ValueError("you cannot enter in both a module_chain and a config_path - please enter in one or the other")
+
         if self.name is not None:
             name_check(self.name)
 
         if config_path is not None:
             self.load(config_path)
 
         if module_chain is not None:
@@ -112,16 +116,23 @@
             self.__module_chain_configs.pop(index)
 
         # test connections
         self.test_connections()
 
     @datatype_validator
     def test_input(self, *, local_file_path: str) -> None:
+        """test input file will flow through pipeline correctly via simulation (currently in beta)
+
+        Parameters
+        ----------
+        local_file_path : str
+            path to local file to test for pipeline threadthrough
+        """
         input_check(local_file_path, self.__module_chain)
-        print(f"SUCCESS: local file {local_file_path} passed pipeline input test passed")
+        print(f"SUCCESS: local file '{local_file_path}' passed pipeline input test passed")
 
     @property
     def module_chain(self) -> list:
         return self.__module_chain_names
 
     @property
     def module_chain_output_process_keys(self) -> list:
```

### Comparing `krixik-1.1.15/krixik/pipeline_builder/utilities/chain_checker.py` & `krixik-1.1.16/krixik/pipeline_builder/utilities/chain_checker.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/pipeline_builder/utilities/input_checker.py` & `krixik-1.1.16/krixik/pipeline_builder/utilities/input_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 from krixik.pipeline_builder.utilities.chain_checker import chain_check
 from krixik.utilities.validators.data.utilities.read_config import check_inverse_config
 from krixik.modules.utilities.io_validator import is_valid
 
 
 def input_check(local_file_path: str, module_chain: list) -> None:
+    if not isinstance(local_file_path, str):
+        raise TypeError(f"local_file_path must be a string: {local_file_path}")
+
     if not os.path.exists(local_file_path):
         raise FileExistsError(f"FAILURE: local_file_path does not exist - {local_file_path}")
     chain_check(module_chain)
 
     first_module = module_chain[0]
     first_module_input_format = first_module.input_format
     file_ext = "." + local_file_path.split(".")[-1]
     file_ext_format = check_inverse_config(file_ext)
     if file_ext_format != first_module_input_format:
-        raise TypeError(f"file extension {file_ext} does not match the expected input format {first_module_input_format}")
+        raise TypeError(f"file extension '{file_ext}' does not match the expected input format {first_module_input_format}")
     is_valid(first_module.name, local_file_path)
```

### Comparing `krixik-1.1.15/krixik/pipeline_builder/utilities.py` & `krixik-1.1.16/krixik/pipeline_builder/utilities.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/pipeline_examples/single_module/text-embedder.yml` & `krixik-1.1.16/krixik/pipeline_examples/single_module/text-embedder.yml`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/pipeline_examples/single_module/utilities/generate_examples.py` & `krixik-1.1.16/krixik/pipeline_examples/single_module/utilities/generate_examples.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 from krixik.pipeline_builder.module import Module
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 from krixik.modules import available_modules
 from krixik.__base__ import library_base_dir
 
 save_directory = library_base_dir + "/pipeline_examples/single_module"
 
 
 def generate():
     try:
         for file in os.listdir(save_directory):
             if file.endswith(".yml"):
                 os.remove(os.path.join(save_directory, file))
 
-        pipeline = CreatePipeline()
+        pipeline = BuildPipeline()
         for module_name in available_modules:
             module = Module(module_name)
-            pipeline = CreatePipeline(name=f"{module_name}-pipeline", module_chain=[module])
+            pipeline = BuildPipeline(name=f"{module_name}-pipeline", module_chain=[module])
             pipeline.save(config_path=f"{save_directory}/{module_name}.yml")
 
     except Exception as e:
         raise e
```

### Comparing `krixik-1.1.15/krixik/system_builder/base.py` & `krixik-1.1.16/krixik/system_builder/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             last_updated_end=last_updated_end,
             verbose=verbose,
         )
 
     @kwargs_checker
     @check_init_decorator
     @type_check_inputs
-    def fetch_output(self, *, file_id: str, local_save_directory: str = os.getcwd()) -> dict | None:
+    def fetch_output(self, *, file_id: str, local_save_directory: str = os.path.abspath("")) -> dict | None:
         """fetch the output of a file from the server via its file_id for a given pipeline
 
         Parameters
         ----------
         file_id : str
             the file_id of the file to be fetched, by default None
         local_save_directory: str, optional
@@ -404,15 +404,16 @@
         local_file_path: Optional[str] = None,
         file_tags: Optional[list] = None,
         file_description: Optional[str] = None,
         modules: Optional[dict] = {},
         expire_time: Optional[int] = None,
         verbose: bool = True,
         wait_for_process: bool = True,
-        local_save_directory: str = os.getcwd(),
+        local_save_directory: str = os.path.abspath(""),
+        download_output: bool = True,
         og_local_file_path: Optional[str] = None,
     ) -> dict | None:
         """process a file to the server for a given pipeline
 
         Parameters
         ----------
         file_name : str, optional
@@ -435,14 +436,16 @@
             the expire time of the file, by default None
         verbose : bool, optional
             whether to print verbose output, by default True
         wait_for_process : bool, optional
             whether to process the file asynchronously, by default False
         local_save_directory: str
             local directory for process output, by default os.getcwd()
+        download_output: bool
+            boolean switch, download process output (set True) or not (set False)
         og_local_file_path: str, optional
             local file path used for any file conversion (e.g., mp4 to mp3, controlled internally
         Returns
         -------
         dict | None
             a dictionary containing the status_code, request_id, and message indicating success or failure
         """
@@ -546,23 +549,26 @@
 
         # reset class variables
         self._reset_class_variables()
 
         if not self.wait_for_process:
             return output_data
 
-        if output_data is not None:
+        if not download_output:
+            vprint("INFO: downlaod_output set to False, not fetching output", verbose=verbose)
+
+        if download_output and output_data is not None:
             try:
                 file_id = output_data["file_id"]
                 file_output = self.fetch_output(file_id=file_id, local_save_directory=local_save_directory)
                 vprint("SUCCESS: process output downloaded", verbose=verbose)
                 return file_output
             except Exception as e:
                 raise e
-
+        output_data["status_code"] = 200
         return output_data
 
     @kwargs_checker
     @check_init_decorator
     @type_check_inputs
     def show_tree(
         self,
@@ -647,7 +653,18 @@
             report["process_status"] = cleaned_process_status
             return report
         if failure_status is not None:
             report["failure_status"] = failure_status
             report["overall_status"] = "failed"
             return report
         return report
+
+    def __getattr__(self, attr):
+        if attr == "keyword_search":
+            raise AttributeError(
+                f"your pipeline has no attribute '{attr}' because its module_chain does not end with keyword-db: - {self.module_chain}"
+            )
+        if attr == "semantic_search":
+            raise AttributeError(
+                f"your pipeline has no attribute '{attr}' because its module_chain does not end with vector-db: - {self.module_chain}"
+            )
+        raise AttributeError(f"pipelines do not have the attribute '{attr}'")
```

### Comparing `krixik-1.1.15/krixik/system_builder/functions/check_process_status.py` & `krixik-1.1.16/krixik/system_builder/functions/check_process_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 def check_process_status(self, *, process_id: str) -> tuple:
     max_count = 9
     start_count = 0
     backoff_schedule = [1, 2, 4, 8, 16, 32, 64, 128, 256]
     while start_count < max_count:
         try:
             if process_id is None:
-                raise ValueError("process_id cannot be none when checking process_status")
+                raise ValueError("request_id cannot be none when checking process_status")
 
             if hasattr(self, "_KrixikBasePipeline__pipeline"):
                 pipeline = self._KrixikBasePipeline__pipeline
             elif hasattr(self, "_KrixikSearchPipeline__pipeline"):
                 pipeline = self._KrixikSearchPipeline__pipeline
             else:
                 raise ValueError("pipeline not found in self")
```

### Comparing `krixik-1.1.15/krixik/system_builder/functions/checkin.py` & `krixik-1.1.16/krixik/system_builder/functions/checkin.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 
 def check_init(self):
     if not (hasattr(self, "_KrixikBasePipeline__api_check_val") or hasattr(self, "_KrixikSearchPipeline__api_check_val")):
         raise ValueError("you are not authenticated - call init() to authenticate using your API key and url")
     else:
         if hasattr(self, "_KrixikBasePipeline__api_check_val"):
             if self._KrixikBasePipeline__api_check_val == 1:
-                raise ValueError("you are not authenticated - all init() to authenticate using your API key and url")
+                raise ValueError("you are not authenticated - call init() to authenticate using your API key and url")
             if self._KrixikBasePipeline__api_check_val is None:
                 raise ValueError("you are not authenticated - call init() to authenticate using your API key and url")
         if hasattr(self, "_KrixikSearchPipeline__api_check_val"):
             if self._KrixikSearchPipeline__api_check_val == 1:
-                raise ValueError("you are not authenticated - all init() to authenticate using your API key and url")
+                raise ValueError("you are not authenticated - call init() to authenticate using your API key and url")
             if self._KrixikSearchPipeline__api_check_val is None:
                 raise ValueError("you are not authenticated - call init() to authenticate using your API key and url")
 
 
 def check_init_decorator(func: Callable) -> Callable:
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs):
```

### Comparing `krixik-1.1.15/krixik/system_builder/functions/delete.py` & `krixik-1.1.16/krixik/system_builder/functions/delete.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/system_builder/functions/fetch_output.py` & `krixik-1.1.16/krixik/system_builder/functions/fetch_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,21 +82,27 @@
                 save_path = save_output(
                     output["url"],
                     file_id,
                     output["extension"],
                     local_save_directory,
                 )
                 save_paths.append(save_path)
-
             results["process_output_files"] = save_paths
             results["message"] += "Output saved to location(s) listed in process_output_files."
+
             if len(process_output) == 1:
                 if process_output[0]["extension"] == ".json":
-                    with open(save_paths[0], "r") as file:
-                        results["process_output"] = json.load(file)
+                    file_size_bytes = os.path.getsize(save_paths[0])
+                    file_size_mb = file_size_bytes / (1024 * 1024)
+                    if file_size_mb >= 0.5:
+                        print("INFO: output json downloaded but larger than 0.5MB and will not be returned with .process output")
+                        results["process_output"] = None
+                    else:
+                        with open(save_paths[0], "r") as file:
+                            results["process_output"] = json.load(file)
                 else:
                     results["process_output"] = None
             else:
                 results["process_output"] = None
         status_code_dict = {"status_code": response.status_code}
         status_code_dict.update(results)
         return status_code_dict
```

### Comparing `krixik-1.1.15/krixik/system_builder/functions/keyword_search.py` & `krixik-1.1.16/krixik/system_builder/functions/keyword_search.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/system_builder/functions/list_files.py` & `krixik-1.1.16/krixik/system_builder/functions/list_files.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/system_builder/functions/process.py` & `krixik-1.1.16/krixik/system_builder/functions/process.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/system_builder/functions/semantic_search.py` & `krixik-1.1.16/krixik/system_builder/functions/semantic_search.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/system_builder/functions/show_tree.py` & `krixik-1.1.16/krixik/system_builder/functions/show_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import requests
 import json
 from krixik.utilities.tree_illustrator import show_symbolic_file_tree
 from krixik.system_builder.functions import show_tree_endpoint
-from krixik.utilities.utilities import vprint
 
 
 def show_post(self, *, symbolic_directory_path: str, max_files: int = 1000, verbose: bool = True):
     if hasattr(self, "_KrixikBasePipeline__version"):
         version = self._KrixikBasePipeline__version
     elif hasattr(self, "_KrixikSearchPipeline__version"):
         version = self._KrixikSearchPipeline__version
```

### Comparing `krixik-1.1.15/krixik/system_builder/functions/update.py` & `krixik-1.1.16/krixik/system_builder/functions/update.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/system_builder/utilities/decorators.py` & `krixik-1.1.16/krixik/system_builder/utilities/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         "file_description",
         "modules",
         "expire_time",
         "verbose",
         "wait_for_process",
         "local_save_directory",
         "og_local_file_path",
+        "download_output",
     },
     "show_tree": {"symbolic_directory_path", "max_files", "verbose"},
     "process_status": {"request_id"},
     "keyword_search": {
         "query",
         "file_ids",
         "file_names",
```

### Comparing `krixik-1.1.15/krixik/utilities/converters/default_clean_options.py` & `krixik-1.1.16/krixik/utilities/converters/default_clean_options.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/converters/docx_to_txt.py` & `krixik-1.1.16/krixik/utilities/converters/docx_to_txt.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/converters/pdf_to_txt.py` & `krixik-1.1.16/krixik/utilities/converters/pdf_to_txt.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/converters/pptx_to_txt.py` & `krixik-1.1.16/krixik/utilities/converters/pptx_to_txt.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/converters/unclean_to_clean_txt.py` & `krixik-1.1.16/krixik/utilities/converters/unclean_to_clean_txt.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/converters/utilities/decorators.py` & `krixik-1.1.16/krixik/utilities/converters/utilities/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import copy
 import inspect
 import tempfile
+from functools import wraps
 from krixik.utilities.converters.read_config import convert_extension
 from krixik.utilities.converters.unclean_to_clean_txt import (
     convert as convert_unclean_text,
 )
 from krixik.utilities.converters.docx_to_txt import convert as convert_docx
 from krixik.utilities.converters.pdf_to_txt import convert as convert_pdf
 from krixik.utilities.converters.pptx_to_txt import convert as convert_pptx
 from krixik.utilities.converters.video_to_audio import convert as convert_video
 from krixik.utilities.utilities import vprint, get_input
 
 
 def datatype_converter_wrapper(func):
+    @wraps(func)
     def converter_wrapper(*args, **kwargs):
         try:
             signature = inspect.signature(func)
             verbose = get_input("verbose", signature, kwargs, default_value=True)
             local_file_path = get_input("local_file_path", signature, kwargs, default_value=True)
 
             if local_file_path is not None:
```

### Comparing `krixik-1.1.15/krixik/utilities/converters/video_to_audio.py` & `krixik-1.1.16/krixik/utilities/converters/video_to_audio.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/file_name_generator.py` & `krixik-1.1.16/krixik/utilities/file_name_generator.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/tree_illustrator.py` & `krixik-1.1.16/krixik/utilities/tree_illustrator.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/utilities.py` & `krixik-1.1.16/krixik/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/audio.py` & `krixik-1.1.16/krixik/utilities/validators/data/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,22 +54,22 @@
 
         # compute file size
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
         # compute length of audio file in seconds
         audio_duration = compute_duration(local_file_path)
 
         # check that audio file is  greater than minimum_seconds and less than maximum_seconds
         if audio_duration < minimum_seconds or audio_duration > maximum_seconds:
             raise ValueError(
-                f"audio file is {audio_duration} seconds - this is either less than {minimum_seconds} seconds (current minimum size allowable) or greater than {maximum_seconds} seconds (current maximum size allowable)"
+                f"audio file is {round(audio_duration,2)} seconds - this is either less than {minimum_seconds} seconds (current minimum size allowable) or greater than {maximum_seconds} seconds (current maximum size allowable)"
             )
     except ValueError as ve:
         raise ve
     except Exception as e:
         raise ValueError(f"audio extraction failed with exception {e}")
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/docx.py` & `krixik-1.1.16/krixik/utilities/validators/data/docx.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         # compute file size in megabytes
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
         # compute word count
         file_word_count = compute_word_count(local_file_path)
 
         # check that word count is greater than minimum_word_count
         if file_word_count < minimum_word_count:
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/image.py` & `krixik-1.1.16/krixik/utilities/validators/data/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             # Use imghdr to determine the image type
             image_type = imghdr.what(None, header)
 
             # Check if the image type is JPEG or PNG
             if image_type in ["jpg", "jpeg", "png"]:
                 return True
             else:
-                raise ValueError(f"The file '{local_file_path}' does not represent a valid image.")
+                raise ValueError(f"The file '{local_file_path}' does not represent a valid image - its type is being read as {image_type}.")
     except FileNotFoundError:
         raise FileNotFoundError(f"The file '{local_file_path}' does not exist.")
     except Exception as e:
         raise ValueError(f"Error reading image: {e}")
 
 
 def is_proportionally_acceptable(local_file_path: str) -> None:
@@ -65,15 +65,15 @@
         # check that local_file_path represents a valid json file
         is_valid(local_file_path)
 
         # check size of input json file
         file_size = compute_size(local_file_path)
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
     except ValueError as ve:
         raise ve
     except Exception as e:
         raise ValueError(f"invalid local_file_path: {e}")
 
     # check proportion of input image file
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/json.py` & `krixik-1.1.16/krixik/utilities/validators/data/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,18 @@
         # Check if the loaded object is a dictionary
         if isinstance(json_object, list):
             # check that json_object has at least one key
             if len(json_object) < 1:
                 raise ValueError("JSON file does not represent a dictionary.")
             for v in json_object:
                 if not isinstance(v, dict):
-                    raise ValueError("JSON file does not represent a dictionary.")
+                    raise ValueError(f"object in JSON file does not represent a valid dictionary: {v}")
             return True
         else:
-            raise ValueError("JSON file does not represent a dictionary.")
+            raise ValueError("JSON file must consist of a list of dictionaries.")
     except json.JSONDecodeError as e:
         raise ValueError(f"Invalid JSON file - your file is not a valid JSON file: {e}")
     except FileNotFoundError:
         raise FileNotFoundError(f"The file '{local_file_path}' does not exist.")
     except Exception as e:
         raise ValueError(f"Error reading JSON file: {e}")
 
@@ -107,15 +107,15 @@
         # check that local_file_path represents a valid json file
         is_valid(local_file_path)
 
         # check size of input json file
         file_size = compute_size(local_file_path)
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
         (
             maximum_key_length,
             largest_key,
             minimum_token_count,
             maximum_token_count,
@@ -131,18 +131,18 @@
 
         if snippet_count > snippet_max_count:
             raise ValueError(
                 f"there are too many key-value pairs in your input local_file_path {local_file_path} - total count must be less than {snippet_max_count}"
             )
         if minimum_token_count < snippet_min_token_count:
             raise ValueError(
-                f"too few tokens - the value in the following key-value pair {minimum_token_count_key_value} has too few tokens (at present the minimum is {snippet_min_token_count} - please check this key-value pair in your input local_file_path {local_file_path}"
+                f"too few tokens - the value in the following key-value pair has too few tokens (at present the minimum is {snippet_min_token_count} - please check this key-value pair in your input local_file_path {local_file_path} - {minimum_token_count_key_value}"
             )
         if maximum_token_count > snippet_max_token_count:
             raise ValueError(
-                f"too many tokens - the value in the following key-value pair {maximum_token_count_key_value} has too many tokens (at present the minimum is {snippet_max_token_count} - please check this key-value pair in your input local_file_path {local_file_path}"
+                f"too many tokens - the value in the following key-value pair has too many tokens (at present the maximum is {snippet_max_token_count} - please check this key-value pair in your input local_file_path {local_file_path} - {maximum_token_count_key_value} "
             )
 
     except ValueError as ve:
         raise ve
     except Exception as e:
         raise ValueError(f"invalid local_file_path: {e}")
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/npy.py` & `krixik-1.1.16/krixik/utilities/validators/data/npy.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         # compute file size in megabytes
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
         if file_size > maximum_file_size:
             raise ValueError(f"file size is greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}")
 
     except ValueError as ve:
         raise ve
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/pdf.py` & `krixik-1.1.16/krixik/utilities/validators/data/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         # compute file size in megabytes
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
         # compute word count
         file_word_count = compute_word_count(local_file_path)
 
         # check that word count is greater than minimum_word_count
         if file_word_count < minimum_word_count:
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/pptx.py` & `krixik-1.1.16/krixik/utilities/validators/data/pptx.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         # compute file size in megabytes
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
         # compute word count
         file_word_count = compute_word_count(local_file_path)
 
         # check that word count is greater than minimum_word_count
         if file_word_count < minimum_word_count:
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/text.py` & `krixik-1.1.16/krixik/utilities/validators/data/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         # compute file size in megabytes
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
         # compute word count
         file_word_count, file_line_count = compute_word_line_count(local_file_path)
 
         # check that word count is greater than minimum_word_count
         if file_word_count < minimum_word_count:
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/utilities/decorators.py` & `krixik-1.1.16/krixik/utilities/validators/data/utilities/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
+from functools import wraps
+
 from krixik.utilities.validators.data.audio import is_size as is_audio_size
 from krixik.utilities.validators.data.video import is_size as is_video_size
 from krixik.utilities.validators.data.text import is_size as is_text_size
 from krixik.utilities.validators.data.pdf import is_size as is_pdf_size
 from krixik.utilities.validators.data.json import is_size as is_json_size
 from krixik.utilities.validators.data.image import is_size as is_image_size
 from krixik.utilities.validators.data.docx import is_size as is_docx_size
 from krixik.utilities.validators.data.pptx import is_size as is_pptx_size
 from krixik.utilities.validators.data.npy import is_size as is_npy_size
 
 from krixik.utilities.validators.data.utilities.read_config import get_all_allowable_extensions
 
 
 def datatype_validator(func):
+    @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             if "local_file_path" in list(kwargs.keys()):
                 local_file_path = kwargs["local_file_path"]
                 extension = local_file_path.split(".")[-1]
                 allowable_extensions = get_all_allowable_extensions()
                 if "." + extension not in allowable_extensions:
-                    raise ValueError(f"invalid file extension: {extension} - currently only {get_all_allowable_extensions} are allowed.")
+                    raise ValueError(f"invalid file extension: '{extension}' - currently only {allowable_extensions} are allowed.")
 
                 if extension == "txt":
                     is_text_size(local_file_path=local_file_path)
                 elif extension == "pdf":
                     is_pdf_size(local_file_path=local_file_path)
                 elif extension == "json":
                     is_json_size(local_file_path=local_file_path)
@@ -36,15 +39,15 @@
                 elif extension == "mp3":
                     is_audio_size(local_file_path=local_file_path)
                 elif extension == "mp4":
                     is_video_size(local_file_path=local_file_path)
                 elif extension == "npy":
                     is_npy_size(local_file_path=local_file_path)
                 else:
-                    raise ValueError(f"invalid file extension: {extension}")
+                    raise ValueError(f"invalid file extension: '{extension}'")
             return func(*args, **kwargs)
         except ValueError as e:
             raise ValueError(e)
         except Exception as e:
             raise Exception(e)
 
     return wrapper
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/utilities/read_config.py` & `krixik-1.1.16/krixik/utilities/validators/data/utilities/read_config.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/data/video.py` & `krixik-1.1.16/krixik/utilities/validators/data/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     try:
         # compute file size
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
-                f"input file size is {file_size} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
+                f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
         # compute length of audio file in seconds
         audio_duration = compute_duration(local_file_path)
 
         # check that audio file is  greater than minimum_seconds and less than maximum_seconds
         if audio_duration < minimum_seconds:
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/clean_options.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/clean_options.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/expire_time.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/expire_time.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,10 +8,10 @@
         raise ValueError(f"input expire_time must be an int - INFO: input expire_time type: {type(expire_time)}")
 
     if not isinstance(expire_time, int):
         raise ValueError(f"input expire_time must be an int - INFO: input expire_time type: {type(expire_time)}")
 
     # check that expire_time falls with in EXPIRE_TIME_MIN and EXPIRE_TIME_MAX
     if expire_time < EXPIRE_TIME_MIN:
-        raise ValueError(f"expire_time {expire_time} must be at least {EXPIRE_TIME_MIN} seconds in the future")
+        raise ValueError(f"input expire_time -- {expire_time} -- is too low, it must be at least {EXPIRE_TIME_MIN} seconds")
     if expire_time > EXPIRE_TIME_MAX:
-        raise ValueError(f"expire_time {expire_time} must be at most {EXPIRE_TIME_MAX} seconds in the future")
+        raise ValueError(f"input expire_time -- {expire_time} -- is to large, it can be at most {EXPIRE_TIME_MAX} seconds")
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/file_description.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/file_description.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/file_ids.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/file_ids.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/file_names.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/file_tags.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/file_tags.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/k_nn.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/k_nn.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/local_save_directory.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/local_save_directory.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/lower_case.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/lower_case.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/max_files.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/max_files.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/process_switches.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/process_switches.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/query.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/query.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/request_id.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/request_id.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/sort_order.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/sort_order.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/symbolic_paths.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/symbolic_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/timestamp_bookends.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/timestamp_bookends.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/user_secrets.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/user_secrets.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/base/utilities/decorators.py` & `krixik-1.1.16/krixik/utilities/validators/system/base/utilities/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,24 +35,24 @@
 from krixik.utilities.validators.system.base.expire_time import expire_time_checker
 from krixik.utilities.validators.system.base.query import query_checker
 from krixik.utilities.validators.system.base.k_nn import k_checker
 from krixik.utilities.validators.system.base.user_secrets import (
     api_key_checker,
     api_url_checker,
 )
+from krixik.utilities.validators.system.base.download_output import download_output_checker
 
 from krixik.utilities.utilities import get_input
 from typing import Callable
 
 
 def type_check_inputs(func: Callable) -> Callable:
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
-            func_name = func.__name__
             signature = inspect.signature(func)
 
             verbose = get_input("verbose", signature, kwargs, default_value=True)
             verbose_checker(verbose)
 
             if "api_key" in list(kwargs.keys()):
                 api_key_checker(kwargs["api_key"])
@@ -93,14 +93,17 @@
 
             if "local_save_directory" in list(kwargs.keys()):
                 local_save_directory_checker(kwargs["local_save_directory"])
 
             if "file_description" in list(kwargs.keys()):
                 file_description_checker(kwargs["file_description"])
 
+            download_output = get_input("download_output", signature, kwargs, default_value=True)
+            download_output_checker(download_output)
+
             max_files = get_input("max_files", signature, kwargs)
             if max_files is not None:
                 max_files_checker(max_files)
 
             wait_for_process = get_input("wait_for_process", signature, kwargs, default_value=False)
             wait_for_process_checker(wait_for_process)
```

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/audio/file_names.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/audio/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/audio/local_file_path.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/audio/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/image/file_names.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/image/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/image/local_file_path.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/image/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/image/symbolic_file_paths.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/image/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/json/file_names.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/json/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/json/local_file_path.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/json/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/json/symbolic_file_paths.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/json/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/npy/file_names.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/npy/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/npy/local_file_path.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/npy/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/text/file_names.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/text/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/text/local_file_path.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/text/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/text/symbolic_file_paths.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/text/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/system/data/utilities/decorators.py` & `krixik-1.1.16/krixik/utilities/validators/system/data/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik/utilities/validators/utilities/decorators.py` & `krixik-1.1.16/krixik/utilities/validators/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.15/krixik.egg-info/PKG-INFO` & `krixik-1.1.16/krixik.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krixik
-Version: 1.1.15
+Version: 1.1.16
 Summary: Easily assemble and serverlessly consume modular AI pipelines through secure Python APIs.
 Home-page: https://github.com/krixik-ai/krixik-cli
 Author: Jeremy Watt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: linting
 Provides-Extra: testing
@@ -94,26 +94,26 @@
 If you've misplaced your secrets, please reach out to us directly.
 
 
 ### Building your first pipeline
 
 Let's build a simple transcription pipeline consisting of a single `transcribe` module.
 
-Import the required Krixik module and pipeline tooling required to instantiate modules and create custom pipelines: the `Module` and `CreatePipeline` class objects. Then create your module and your pipeline.
+Import the required Krixik module and pipeline tooling required to instantiate modules and create custom pipelines: the `Module` and `BuildPipeline` class objects. Then create your module and your pipeline.
 
 ```python
 # import custom pipeline builder tools
 from krixik.pipeline_builder.module import Module
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 
 # instantiate module
 module_1 = Module(name="transcribe")
 
 # create custom pipeline object with above module
-custom_pipeline_1 = CreatePipeline(name='my-transcribe-pipeline-1', 
+custom_pipeline_1 = BuildPipeline(name='my-transcribe-pipeline-1', 
                                    module_chain=[module_1])
 ```
 
 With your custom pipeline defined you can load it for use with the `load_pipeline` method.
 
 ```python
 my_pipeline_1 = krixik.load_pipeline(pipeline=custom_pipeline_1)
@@ -142,25 +142,25 @@
 
 Locally creating and testing this sequence of steps would be time consuming—orchestrating them in a secure production service even more so. And that's without trying to make it all serverless.
 
 With **Krixik**, however, you can rapidly add this functionality to your original pipeline by just adding a few modules. Syntax remains as above:
 
 ```python
 from krixik.pipeline_builder.module import Module
-from krixik.pipeline_builder.pipeline import CreatePipeline
+from krixik.pipeline_builder.pipeline import BuildPipeline
 
 # instantiate modules
 module_a = Module(name="transcribe")
 module_b = Module(name="json-to-txt")
 module_c = Module(name="parser")
 module_d = Module(name="text-embedder")
 module_e = Module(name="vector-search")
 
 # create custom pipeline object with the above modules in sequence
-custom_pipeline_2 = CreatePipeline(name='my-transcribe-pipeline-2', 
+custom_pipeline_2 = BuildPipeline(name='my-transcribe-pipeline-2', 
                         module_chain=[module_a, module_b, module_c, module_d, module_e])
 
 # pass the custom object to the krixik operator
 my_pipeline_2 = krixik.load_pipeline(pipeline=custom_pipeline_2)
 ```
 
 Let's process a file through your new pipeline.
```

### Comparing `krixik-1.1.15/krixik.egg-info/SOURCES.txt` & `krixik-1.1.16/krixik.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 krixik/utilities/validators/data/utilities/__init__.py
 krixik/utilities/validators/data/utilities/config.yml
 krixik/utilities/validators/data/utilities/decorators.py
 krixik/utilities/validators/data/utilities/read_config.py
 krixik/utilities/validators/system/__init__.py
 krixik/utilities/validators/system/base/__init__.py
 krixik/utilities/validators/system/base/clean_options.py
+krixik/utilities/validators/system/base/download_output.py
 krixik/utilities/validators/system/base/expire_time.py
 krixik/utilities/validators/system/base/extension_enforcer.py
 krixik/utilities/validators/system/base/file_description.py
 krixik/utilities/validators/system/base/file_ids.py
 krixik/utilities/validators/system/base/file_names.py
 krixik/utilities/validators/system/base/file_tags.py
 krixik/utilities/validators/system/base/k_nn.py
```

### Comparing `krixik-1.1.15/setup.py` & `krixik-1.1.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from setuptools import find_packages
 
 setup(
     name="krixik",
-    version="1.1.15",
+    version="1.1.16",
     description="Easily assemble and serverlessly consume modular AI pipelines through secure Python APIs.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Jeremy Watt",
     email="jeremy@krixik.com",
     url="https://github.com/krixik-ai/krixik-cli",
     packages=find_packages(include=["krixik*"]),
```

