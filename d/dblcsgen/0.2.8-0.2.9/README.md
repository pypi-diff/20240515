# Comparing `tmp/dblcsgen-0.2.8.tar.gz` & `tmp/dblcsgen-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblcsgen-0.2.8.tar", last modified: Tue May 14 07:09:12 2024, max compression
+gzip compressed data, was "dblcsgen-0.2.9.tar", last modified: Tue May 14 07:20:40 2024, max compression
```

## Comparing `dblcsgen-0.2.8.tar` & `dblcsgen-0.2.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 07:09:10.000000 dblcsgen-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-14 07:09:10.000000 dblcsgen-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/dblcsgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 07:09:12.000000 dblcsgen-0.2.8/dblcsgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.718622 dblcsgen-0.2.8/sglang/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.718622 dblcsgen-0.2.8/sglang/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/backend/runtime_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/global_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.718622 dblcsgen-0.2.8/sglang/lang/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/chat_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27999 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11522 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/lang/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/launch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.722622 dblcsgen-0.2.8/sglang/srt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.722622 dblcsgen-0.2.8/sglang/srt/constrained/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/constrained/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/constrained/fsm_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/constrained/jump_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/flush_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/hf_transformers_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.722622 dblcsgen-0.2.8/sglang/srt/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/context_flashattention_nopad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/extend_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/logits_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/radix_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/layers/token_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.722622 dblcsgen-0.2.8/sglang/srt/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/detokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/io_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.726622 dblcsgen-0.2.8/sglang/srt/managers/router/
--rw-r--r--   0 runner    (1001) docker     (127)    20204 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/infer_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    29381 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/model_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/radix_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/router/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/managers/tokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/memory_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/mm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.726622 dblcsgen-0.2.8/sglang/srt/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/commandr.py
--rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/dbrx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/dbrx_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/mixtral.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/qwen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/stablelm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/models/yivl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/openai_api_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/openai_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/sampling_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/server_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/srt/weight_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:09:12.730622 dblcsgen-0.2.8/sglang/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/test/test_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/test/test_openai_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/test/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-14 07:09:06.000000 dblcsgen-0.2.8/sglang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.900650 dblcsgen-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 07:20:38.000000 dblcsgen-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-14 07:20:40.900650 dblcsgen-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-14 07:20:38.000000 dblcsgen-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.896650 dblcsgen-0.2.9/dblcsgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-14 07:20:40.000000 dblcsgen-0.2.9/dblcsgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-14 07:20:40.000000 dblcsgen-0.2.9/dblcsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:20:40.000000 dblcsgen-0.2.9/dblcsgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 07:20:40.000000 dblcsgen-0.2.9/dblcsgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 07:20:40.000000 dblcsgen-0.2.9/dblcsgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:20:40.900650 dblcsgen-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.880650 dblcsgen-0.2.9/sglang/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.880650 dblcsgen-0.2.9/sglang/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/backend/runtime_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/global_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.880650 dblcsgen-0.2.9/sglang/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/lang/chat_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/lang/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27999 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/lang/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11522 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/lang/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/lang/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/launch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.884650 dblcsgen-0.2.9/sglang/srt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.888651 dblcsgen-0.2.9/sglang/srt/constrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/constrained/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/constrained/fsm_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/constrained/jump_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/flush_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/hf_transformers_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.888651 dblcsgen-0.2.9/sglang/srt/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/layers/context_flashattention_nopad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/layers/extend_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/layers/logits_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/layers/radix_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/layers/token_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.888651 dblcsgen-0.2.9/sglang/srt/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/detokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/io_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.892650 dblcsgen-0.2.9/sglang/srt/managers/router/
+-rw-r--r--   0 runner    (1001) docker     (127)    20204 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/router/infer_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/router/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29381 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/router/model_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/router/model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/router/radix_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/router/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/managers/tokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/memory_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/mm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.896650 dblcsgen-0.2.9/sglang/srt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/commandr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/dbrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/dbrx_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/qwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/qwen2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/stablelm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/models/yivl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/openai_api_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/sampling_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/server_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/srt/weight_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:20:40.896650 dblcsgen-0.2.9/sglang/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/test/test_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/test/test_openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/test/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-14 07:20:32.000000 dblcsgen-0.2.9/sglang/utils.py
```

### Comparing `dblcsgen-0.2.8/LICENSE` & `dblcsgen-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/PKG-INFO` & `dblcsgen-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.8
+Version: 0.2.9
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.2.8/README.md` & `dblcsgen-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/dblcsgen.egg-info/PKG-INFO` & `dblcsgen-0.2.9/dblcsgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.8
+Version: 0.2.9
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.2.8/dblcsgen.egg-info/SOURCES.txt` & `dblcsgen-0.2.9/dblcsgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/pyproject.toml` & `dblcsgen-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblcsgen"
-version = "0.2.8"
+version = "0.2.9"
 description = "DBLC Fast Structured Generation"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `dblcsgen-0.2.8/sglang/__init__.py` & `dblcsgen-0.2.9/sglang/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 # SGL API Components
 from sglang.api import (
     Runtime,
     assistant,
     assistant_begin,
     assistant_end,
```

### Comparing `dblcsgen-0.2.8/sglang/api.py` & `dblcsgen-0.2.9/sglang/api.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/backend/base_backend.py` & `dblcsgen-0.2.9/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/backend/runtime_endpoint.py` & `dblcsgen-0.2.9/sglang/backend/runtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/global_config.py` & `dblcsgen-0.2.9/sglang/global_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/lang/chat_template.py` & `dblcsgen-0.2.9/sglang/lang/chat_template.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/lang/compiler.py` & `dblcsgen-0.2.9/sglang/lang/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import multiprocessing
 from concurrent.futures import ThreadPoolExecutor
 from queue import Queue
 from typing import List, Union
 
 from sglang.global_config import global_config
-from sglang.lang.interpreter import ProgramState, StreamExecutor, pin_program
+from sglang.lang.interpreter import ProgramState, StreamExecutor
 from sglang.lang.ir import (
     SglArgument,
     SglConstantText,
     SglExpr,
     SglSamplingParams,
     SglVariable,
 )
 
+from sglang.lang.interpreter import cache_program
+
 
 def compile_func(function, backend):
     tracer = function.trace(backend=backend)
     compiler = CompiledFunction(tracer, function)
     return compiler
 
 
@@ -178,17 +180,17 @@
             temperature=temperature,
             top_p=top_p,
             top_k=top_k,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
         )
 
-        # Extract prefix by tracing and cache it
-        if len(batch_kwargs) > 1:
-            pin_program(self.function, backend)
+        # Pre-cache the common prefix for a batch. The prefix is extracted by tracing the program.
+        if global_config.enable_precache_with_tracing and len(batch_kwargs) > 1:
+            cache_program(self.function, backend)
 
         # Run all programs
         if num_threads == "auto":
             num_threads = multiprocessing.cpu_count()
         num_threads = min(num_threads, len(batch_kwargs))
 
         if num_threads == 1:
```

### Comparing `dblcsgen-0.2.8/sglang/lang/interpreter.py` & `dblcsgen-0.2.9/sglang/lang/interpreter.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/lang/ir.py` & `dblcsgen-0.2.9/sglang/lang/ir.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/lang/tracer.py` & `dblcsgen-0.2.9/sglang/lang/tracer.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/constrained/__init__.py` & `dblcsgen-0.2.9/sglang/srt/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/constrained/base_cache.py` & `dblcsgen-0.2.9/sglang/srt/constrained/base_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/constrained/fsm_cache.py` & `dblcsgen-0.2.9/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/constrained/jump_forward.py` & `dblcsgen-0.2.9/sglang/srt/constrained/jump_forward.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/conversation.py` & `dblcsgen-0.2.9/sglang/srt/conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/hf_transformers_utils.py` & `dblcsgen-0.2.9/sglang/srt/hf_transformers_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/layers/context_flashattention_nopad.py` & `dblcsgen-0.2.9/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/layers/extend_attention.py` & `dblcsgen-0.2.9/sglang/srt/layers/extend_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/layers/logits_processor.py` & `dblcsgen-0.2.9/sglang/srt/layers/logits_processor.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/layers/radix_attention.py` & `dblcsgen-0.2.9/sglang/srt/layers/radix_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/layers/token_attention.py` & `dblcsgen-0.2.9/sglang/srt/layers/token_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/detokenizer_manager.py` & `dblcsgen-0.2.9/sglang/srt/managers/detokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/io_struct.py` & `dblcsgen-0.2.9/sglang/srt/managers/io_struct.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/router/infer_batch.py` & `dblcsgen-0.2.9/sglang/srt/managers/router/infer_batch.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/router/manager.py` & `dblcsgen-0.2.9/sglang/srt/managers/router/manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/router/model_rpc.py` & `dblcsgen-0.2.9/sglang/srt/managers/router/model_rpc.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/router/model_runner.py` & `dblcsgen-0.2.9/sglang/srt/managers/router/model_runner.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/router/radix_cache.py` & `dblcsgen-0.2.9/sglang/srt/managers/router/radix_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/router/scheduler.py` & `dblcsgen-0.2.9/sglang/srt/managers/router/scheduler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/managers/tokenizer_manager.py` & `dblcsgen-0.2.9/sglang/srt/managers/tokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/memory_pool.py` & `dblcsgen-0.2.9/sglang/srt/memory_pool.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/mm_utils.py` & `dblcsgen-0.2.9/sglang/srt/mm_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/model_config.py` & `dblcsgen-0.2.9/sglang/srt/model_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/commandr.py` & `dblcsgen-0.2.9/sglang/srt/models/commandr.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/dbrx.py` & `dblcsgen-0.2.9/sglang/srt/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/dbrx_config.py` & `dblcsgen-0.2.9/sglang/srt/models/dbrx_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/gemma.py` & `dblcsgen-0.2.9/sglang/srt/models/gemma.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/llama2.py` & `dblcsgen-0.2.9/sglang/srt/models/llama2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/llava.py` & `dblcsgen-0.2.9/sglang/srt/models/llava.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/mixtral.py` & `dblcsgen-0.2.9/sglang/srt/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/qwen.py` & `dblcsgen-0.2.9/sglang/srt/models/qwen.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/qwen2.py` & `dblcsgen-0.2.9/sglang/srt/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/stablelm.py` & `dblcsgen-0.2.9/sglang/srt/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/models/yivl.py` & `dblcsgen-0.2.9/sglang/srt/models/yivl.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/openai_api_adapter.py` & `dblcsgen-0.2.9/sglang/srt/openai_api_adapter.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/openai_protocol.py` & `dblcsgen-0.2.9/sglang/srt/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/sampling_params.py` & `dblcsgen-0.2.9/sglang/srt/sampling_params.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/server.py` & `dblcsgen-0.2.9/sglang/srt/server.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/server_args.py` & `dblcsgen-0.2.9/sglang/srt/server_args.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/utils.py` & `dblcsgen-0.2.9/sglang/srt/utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/srt/weight_utils.py` & `dblcsgen-0.2.9/sglang/srt/weight_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/test/test_conversation.py` & `dblcsgen-0.2.9/sglang/test/test_conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/test/test_openai_protocol.py` & `dblcsgen-0.2.9/sglang/test/test_openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/test/test_programs.py` & `dblcsgen-0.2.9/sglang/test/test_programs.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/test/test_utils.py` & `dblcsgen-0.2.9/sglang/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.8/sglang/utils.py` & `dblcsgen-0.2.9/sglang/utils.py`

 * *Files identical despite different names*

