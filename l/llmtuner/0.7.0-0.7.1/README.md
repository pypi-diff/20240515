# Comparing `tmp/llmtuner-0.7.0.tar.gz` & `tmp/llmtuner-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.7.0.tar", last modified: Sat Apr 27 19:49:59 2024, max compression
+gzip compressed data, was "llmtuner-0.7.1.tar", last modified: Wed May 15 16:56:04 2024, max compression
```

## Comparing `llmtuner-0.7.0.tar` & `llmtuner-0.7.1.tar`

### file list

```diff
@@ -1,131 +1,130 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:58.951033 llmtuner-0.7.0/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2024-04-27 19:49:37.000000 llmtuner-0.7.0/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    36078 2024-04-27 19:49:58.915033 llmtuner-0.7.0/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    33563 2024-04-27 19:49:37.000000 llmtuner-0.7.0/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      641 2024-04-27 19:49:37.000000 llmtuner-0.7.0/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2024-04-27 19:49:58.951033 llmtuner-0.7.0/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2529 2024-04-27 19:49:38.000000 llmtuner-0.7.0/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:53.827016 llmtuner-0.7.0/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:53.999016 llmtuner-0.7.0/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      389 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:54.391018 llmtuner-0.7.0/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       55 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8717 2024-04-27 19:49:24.000000 llmtuner-0.7.0/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3127 2024-04-27 19:49:24.000000 llmtuner-0.7.0/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:54.631018 llmtuner-0.7.0/src/llmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      110 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1896 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/base_engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3578 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/chat_model.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11272 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/hf_engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8237 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/chat/vllm_engine.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:54.995020 llmtuner-0.7.0/src/llmtuner/data/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      377 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6621 2024-04-27 19:49:25.000000 llmtuner-0.7.0/src/llmtuner/data/aligner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2140 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6528 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/formatter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7451 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5033 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13825 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/preprocess.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    32979 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/template.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3698 2024-04-27 19:49:26.000000 llmtuner-0.7.0/src/llmtuner/data/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:55.207020 llmtuner-0.7.0/src/llmtuner/eval/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       59 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/eval/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5776 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/eval/evaluator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2419 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/eval/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:55.443021 llmtuner-0.7.0/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6495 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    40195 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1117 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7450 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1662 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/packages.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1824 2024-04-27 19:49:27.000000 llmtuner-0.7.0/src/llmtuner/extras/ploting.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:55.691022 llmtuner-0.7.0/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      494 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3882 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1462 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/evaluation_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    12586 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1917 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8174 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/model_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15072 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/hparams/parser.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:55.859023 llmtuner-0.7.0/src/llmtuner/model/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      294 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8911 2024-04-27 19:49:28.000000 llmtuner-0.7.0/src/llmtuner/model/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6222 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5551 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/patcher.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:56.459025 llmtuner-0.7.0/src/llmtuner/model/utils/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1998 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/attention.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4028 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/checkpointing.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2344 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/embedding.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13800 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/longlora.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3061 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      832 2024-04-27 19:49:29.000000 llmtuner-0.7.0/src/llmtuner/model/utils/mod.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2063 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/moe.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6262 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/quantization.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1711 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/rope.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2886 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/unsloth.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2311 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/valuehead.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      887 2024-04-27 19:49:30.000000 llmtuner-0.7.0/src/llmtuner/model/utils/visual.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:56.595025 llmtuner-0.7.0/src/llmtuner/train/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:56.771026 llmtuner-0.7.0/src/llmtuner/train/dpo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/dpo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7577 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/dpo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3152 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/dpo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:56.907026 llmtuner-0.7.0/src/llmtuner/train/orpo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/orpo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5763 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/orpo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2717 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/orpo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:57.195027 llmtuner-0.7.0/src/llmtuner/train/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    20807 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2380 2024-04-27 19:49:31.000000 llmtuner-0.7.0/src/llmtuner/train/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2696 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:57.339028 llmtuner-0.7.0/src/llmtuner/train/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1348 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/pt/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2501 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:57.531028 llmtuner-0.7.0/src/llmtuner/train/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      267 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5318 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3103 2024-04-27 19:49:32.000000 llmtuner-0.7.0/src/llmtuner/train/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:57.679029 llmtuner-0.7.0/src/llmtuner/train/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2247 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5314 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4479 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/sft/workflow.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3927 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/tuner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    16575 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/train/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:58.179031 llmtuner-0.7.0/src/llmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       95 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5235 2024-04-27 19:49:33.000000 llmtuner-0.7.0/src/llmtuner/webui/chatter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4986 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:58.731032 llmtuner-0.7.0/src/llmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      362 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2389 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2776 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4218 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/export.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1566 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2605 2024-04-27 19:49:34.000000 llmtuner-0.7.0/src/llmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     9925 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/components/train.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      567 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2757 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2563 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    43606 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2055 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15827 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3313 2024-04-27 19:49:35.000000 llmtuner-0.7.0/src/llmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:54.255017 llmtuner-0.7.0/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    36078 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3408 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      541 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2024-04-27 19:49:52.000000 llmtuner-0.7.0/src/llmtuner.egg-info/top_level.txt
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-27 19:49:58.883033 llmtuner-0.7.0/tests/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2311 2024-04-27 19:49:36.000000 llmtuner-0.7.0/tests/test_attn.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1691 2024-04-27 19:49:36.000000 llmtuner-0.7.0/tests/test_galore.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      933 2024-04-27 19:49:36.000000 llmtuner-0.7.0/tests/test_throughput.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2566 2024-04-27 19:49:36.000000 llmtuner-0.7.0/tests/test_toolcall.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.688996 llmtuner-0.7.1/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    11524 2024-05-15 16:55:52.000000 llmtuner-0.7.1/LICENSE
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    38004 2024-05-15 16:56:04.688996 llmtuner-0.7.1/PKG-INFO
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    36700 2024-05-15 16:55:53.000000 llmtuner-0.7.1/README.md
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      641 2024-05-15 16:55:52.000000 llmtuner-0.7.1/pyproject.toml
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)       38 2024-05-15 16:56:04.688996 llmtuner-0.7.1/setup.cfg
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2644 2024-05-15 16:55:53.000000 llmtuner-0.7.1/setup.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.676996 llmtuner-0.7.1/src/
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.680996 llmtuner-0.7.1/src/llmtuner/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      128 2024-05-15 16:55:51.000000 llmtuner-0.7.1/src/llmtuner/__init__.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.680996 llmtuner-0.7.1/src/llmtuner/api/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/api/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3489 2024-05-15 16:55:41.000000 llmtuner-0.7.1/src/llmtuner/api/app.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     7176 2024-05-15 16:55:41.000000 llmtuner-0.7.1/src/llmtuner/api/chat.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      580 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/api/common.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3009 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/api/protocol.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.680996 llmtuner-0.7.1/src/llmtuner/chat/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      110 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/chat/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1896 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/chat/base_engine.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     4887 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/chat/chat_model.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    11701 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/chat/hf_engine.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     8638 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/chat/vllm_engine.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2139 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/cli.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.680996 llmtuner-0.7.1/src/llmtuner/data/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      377 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     6621 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/aligner.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2140 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/collator.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     6528 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/formatter.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     7387 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/loader.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     5012 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/parser.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    13825 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/preprocess.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    33737 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/template.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3132 2024-05-15 16:55:42.000000 llmtuner-0.7.1/src/llmtuner/data/utils.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.680996 llmtuner-0.7.1/src/llmtuner/eval/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/eval/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     5747 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/eval/evaluator.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2419 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/eval/template.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.680996 llmtuner-0.7.1/src/llmtuner/extras/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/extras/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     8362 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/extras/callbacks.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    42269 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/extras/constants.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1928 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/extras/logging.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     7470 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/extras/misc.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1663 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/extras/packages.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2641 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/extras/ploting.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.680996 llmtuner-0.7.1/src/llmtuner/hparams/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      494 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/hparams/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3882 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/hparams/data_args.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1462 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/hparams/evaluation_args.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    13012 2024-05-15 16:55:43.000000 llmtuner-0.7.1/src/llmtuner/hparams/finetuning_args.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1917 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/hparams/generating_args.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     8174 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/hparams/model_args.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    15191 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/hparams/parser.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/model/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      294 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/model/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    10115 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/model/adapter.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     6521 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/model/loader.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     5814 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/model/patcher.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/model/utils/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1998 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/model/utils/attention.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     4028 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/model/utils/checkpointing.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2344 2024-05-15 16:55:44.000000 llmtuner-0.7.1/src/llmtuner/model/utils/embedding.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    14136 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/longlora.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3061 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/misc.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      832 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/mod.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2063 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/moe.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     6339 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/quantization.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1711 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/rope.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2886 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/unsloth.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2262 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/valuehead.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3643 2024-05-15 16:55:45.000000 llmtuner-0.7.1/src/llmtuner/model/utils/visual.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/train/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/__init__.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/train/dpo/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)       54 2024-05-15 16:55:46.000000 llmtuner-0.7.1/src/llmtuner/train/dpo/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     8051 2024-05-15 16:55:46.000000 llmtuner-0.7.1/src/llmtuner/train/dpo/trainer.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3151 2024-05-15 16:55:46.000000 llmtuner-0.7.1/src/llmtuner/train/dpo/workflow.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/train/orpo/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)       56 2024-05-15 16:55:46.000000 llmtuner-0.7.1/src/llmtuner/train/orpo/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     6110 2024-05-15 16:55:46.000000 llmtuner-0.7.1/src/llmtuner/train/orpo/trainer.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2647 2024-05-15 16:55:46.000000 llmtuner-0.7.1/src/llmtuner/train/orpo/workflow.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/train/ppo/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)       54 2024-05-15 16:55:47.000000 llmtuner-0.7.1/src/llmtuner/train/ppo/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    21330 2024-05-15 16:55:46.000000 llmtuner-0.7.1/src/llmtuner/train/ppo/trainer.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2380 2024-05-15 16:55:46.000000 llmtuner-0.7.1/src/llmtuner/train/ppo/utils.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2695 2024-05-15 16:55:47.000000 llmtuner-0.7.1/src/llmtuner/train/ppo/workflow.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/train/pt/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)       52 2024-05-15 16:55:47.000000 llmtuner-0.7.1/src/llmtuner/train/pt/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1862 2024-05-15 16:55:47.000000 llmtuner-0.7.1/src/llmtuner/train/pt/trainer.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2500 2024-05-15 16:55:47.000000 llmtuner-0.7.1/src/llmtuner/train/pt/workflow.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/train/rm/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)       52 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/rm/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      267 2024-05-15 16:55:47.000000 llmtuner-0.7.1/src/llmtuner/train/rm/metric.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     5783 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/rm/trainer.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3102 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/rm/workflow.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/train/sft/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)       54 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/sft/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2247 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/sft/metric.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     5822 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/sft/trainer.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     4478 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/sft/workflow.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     4415 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/tuner.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    16569 2024-05-15 16:55:48.000000 llmtuner-0.7.1/src/llmtuner/train/utils.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.684996 llmtuner-0.7.1/src/llmtuner/webui/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:55:51.000000 llmtuner-0.7.1/src/llmtuner/webui/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     5235 2024-05-15 16:55:49.000000 llmtuner-0.7.1/src/llmtuner/webui/chatter.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     5177 2024-05-15 16:55:49.000000 llmtuner-0.7.1/src/llmtuner/webui/common.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.688996 llmtuner-0.7.1/src/llmtuner/webui/components/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      362 2024-05-15 16:55:50.000000 llmtuner-0.7.1/src/llmtuner/webui/components/__init__.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2437 2024-05-15 16:55:49.000000 llmtuner-0.7.1/src/llmtuner/webui/components/chatbot.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3839 2024-05-15 16:55:49.000000 llmtuner-0.7.1/src/llmtuner/webui/components/data.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2854 2024-05-15 16:55:50.000000 llmtuner-0.7.1/src/llmtuner/webui/components/eval.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     4224 2024-05-15 16:55:50.000000 llmtuner-0.7.1/src/llmtuner/webui/components/export.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     1566 2024-05-15 16:55:50.000000 llmtuner-0.7.1/src/llmtuner/webui/components/infer.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2605 2024-05-15 16:55:50.000000 llmtuner-0.7.1/src/llmtuner/webui/components/top.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    11042 2024-05-15 16:55:50.000000 llmtuner-0.7.1/src/llmtuner/webui/components/train.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      567 2024-05-15 16:55:49.000000 llmtuner-0.7.1/src/llmtuner/webui/css.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2759 2024-05-15 16:55:50.000000 llmtuner-0.7.1/src/llmtuner/webui/engine.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2952 2024-05-15 16:55:51.000000 llmtuner-0.7.1/src/llmtuner/webui/interface.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    47520 2024-05-15 16:55:51.000000 llmtuner-0.7.1/src/llmtuner/webui/locales.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     2055 2024-05-15 16:55:51.000000 llmtuner-0.7.1/src/llmtuner/webui/manager.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    16091 2024-05-15 16:55:51.000000 llmtuner-0.7.1/src/llmtuner/webui/runner.py
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3604 2024-05-15 16:55:51.000000 llmtuner-0.7.1/src/llmtuner/webui/utils.py
+drwxrwxr-x   0 zhangrichong  (1006) zhangrichong  (1006)        0 2024-05-15 16:56:04.680996 llmtuner-0.7.1/src/llmtuner.egg-info/
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)    38004 2024-05-15 16:56:04.000000 llmtuner-0.7.1/src/llmtuner.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)     3431 2024-05-15 16:56:04.000000 llmtuner-0.7.1/src/llmtuner.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)        1 2024-05-15 16:56:04.000000 llmtuner-0.7.1/src/llmtuner.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)       55 2024-05-15 16:56:04.000000 llmtuner-0.7.1/src/llmtuner.egg-info/entry_points.txt
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)      573 2024-05-15 16:56:04.000000 llmtuner-0.7.1/src/llmtuner.egg-info/requires.txt
+-rw-rw-r--   0 zhangrichong  (1006) zhangrichong  (1006)        9 2024-05-15 16:56:04.000000 llmtuner-0.7.1/src/llmtuner.egg-info/top_level.txt
```

### Comparing `llmtuner-0.7.0/LICENSE` & `llmtuner-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/PKG-INFO` & `llmtuner-0.7.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.7.0
+Version: 0.7.1
 Summary: Easy-to-use LLM fine-tuning framework
 Home-page: https://github.com/hiyouga/LLaMA-Factory
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -17,77 +17,46 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch>=1.13.1
-Requires-Dist: transformers>=4.37.2
-Requires-Dist: datasets>=2.14.3
-Requires-Dist: accelerate>=0.27.2
-Requires-Dist: peft>=0.10.0
-Requires-Dist: trl>=0.8.1
-Requires-Dist: gradio>=4.0.0
-Requires-Dist: scipy
-Requires-Dist: einops
-Requires-Dist: sentencepiece
-Requires-Dist: protobuf
-Requires-Dist: uvicorn
-Requires-Dist: pydantic
-Requires-Dist: fastapi
-Requires-Dist: sse-starlette
-Requires-Dist: matplotlib
-Requires-Dist: fire
-Requires-Dist: packaging
-Provides-Extra: deepspeed
-Requires-Dist: deepspeed>=0.10.0; extra == "deepspeed"
+Provides-Extra: torch
 Provides-Extra: metrics
-Requires-Dist: nltk; extra == "metrics"
-Requires-Dist: jieba; extra == "metrics"
-Requires-Dist: rouge-chinese; extra == "metrics"
+Provides-Extra: deepspeed
+Provides-Extra: bitsandbytes
+Provides-Extra: vllm
 Provides-Extra: galore
-Requires-Dist: galore-torch; extra == "galore"
 Provides-Extra: badam
-Requires-Dist: badam; extra == "badam"
-Provides-Extra: vllm
-Requires-Dist: vllm>=0.4.0; extra == "vllm"
-Provides-Extra: bitsandbytes
-Requires-Dist: bitsandbytes>=0.39.0; extra == "bitsandbytes"
 Provides-Extra: gptq
-Requires-Dist: optimum>=1.16.0; extra == "gptq"
-Requires-Dist: auto-gptq>=0.5.0; extra == "gptq"
 Provides-Extra: awq
-Requires-Dist: autoawq; extra == "awq"
 Provides-Extra: aqlm
-Requires-Dist: aqlm[gpu]>=1.1.0; extra == "aqlm"
 Provides-Extra: qwen
-Requires-Dist: tiktoken; extra == "qwen"
-Requires-Dist: transformers_stream_generator; extra == "qwen"
 Provides-Extra: modelscope
-Requires-Dist: modelscope; extra == "modelscope"
 Provides-Extra: quality
-Requires-Dist: ruff; extra == "quality"
+License-File: LICENSE
 
 ![# LLaMA Factory](assets/logo.png)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Factory)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Factory)](https://github.com/hiyouga/LLaMA-Factory/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![Downloads](https://static.pepy.tech/badge/llmtuner)](https://pypi.org/project/llmtuner/)
-[![Citation](https://img.shields.io/badge/citation-34-green)](#projects-using-llama-factory)
+[![Citation](https://img.shields.io/badge/citation-44-green)](#projects-using-llama-factory)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
 [![Discord](https://dcbadge.vercel.app/api/server/rKfvV9r9FK?compact=true&style=flat)](https://discord.gg/rKfvV9r9FK)
 [![Twitter](https://img.shields.io/twitter/follow/llamafactory_ai)](https://twitter.com/llamafactory_ai)
 [![Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue)](https://huggingface.co/spaces/hiyouga/LLaMA-Board)
 [![Studios](https://img.shields.io/badge/ModelScope-Open%20in%20Studios-blue)](https://modelscope.cn/studios/hiyouga/LLaMA-Board)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)
 
+[![GitHub Tread](https://trendshift.io/api/badge/repositories/4535)](https://trendshift.io/repositories/4535)
+
 👋 Join our [WeChat](assets/wechat.jpg).
 
 \[ English | [中文](README_zh.md) \]
 
 **Fine-tuning a large language model can be easy as...**
 
 https://github.com/hiyouga/LLaMA-Factory/assets/16256802/9840a653-7e9c-41c8-ae89-7ace5698baf6
@@ -135,90 +104,94 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
-[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See `examples/lora_single_gpu/sft_mllm.sh` for usage.
+[24/05/14] We supported training and inference on the Ascend NPU devices. Check [installation](#installation) section for details.
+
+[24/05/13] We supported fine-tuning the **Yi-1.5** series models.
+
+[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See [examples](examples/README.md) for usage.
+
+<details><summary>Full Changelog</summary>
 
 [24/04/22] We provided a **[Colab notebook](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)** for fine-tuning the Llama-3 model on a free T4 GPU. Two Llama-3-derived models fine-tuned using LLaMA Factory are available at Hugging Face, check [Llama3-8B-Chinese-Chat](https://huggingface.co/shenzhi-wang/Llama3-8B-Chinese-Chat) and [Llama3-Chinese](https://huggingface.co/zhichen/Llama3-Chinese) for details.
 
-[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See [examples](examples/README.md) for usage.
 
-[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
+[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See [examples](examples/README.md) for usage.
 
 [24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
 
-<details><summary>Full Changelog</summary>
-
-[24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See `examples/lora_single_gpu` for usage.
+[24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See [examples](examples/README.md) for usage.
 
 [24/03/21] Our paper "[LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models](https://arxiv.org/abs/2403.13372)" is available at arXiv!
 
-[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/extras/fsdp_qlora` for usage.
+[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See [examples](examples/README.md) for usage.
 
-[24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See `examples/extras/loraplus` for usage.
+[24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See [examples](examples/README.md) for usage.
 
-[24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See `examples/extras/galore` for usage.
+[24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See [examples](examples/README.md) for usage.
 
-[24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `--infer_backend vllm` to enjoy **270%** inference speed. (LoRA is not yet supported, merge it first.)
+[24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `infer_backend: vllm` to enjoy **270%** inference speed.
 
-[24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `--use_dora` to activate DoRA training.
+[24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `use_dora: true` to activate DoRA training.
 
-[24/02/15] We supported **block expansion** proposed by [LLaMA Pro](https://github.com/TencentARC/LLaMA-Pro). See `examples/extras/llama_pro` for usage.
+[24/02/15] We supported **block expansion** proposed by [LLaMA Pro](https://github.com/TencentARC/LLaMA-Pro). See [examples](examples/README.md) for usage.
 
 [24/02/05] Qwen1.5 (Qwen2 beta version) series models are supported in LLaMA-Factory. Check this [blog post](https://qwenlm.github.io/blog/qwen1.5/) for details.
 
-[24/01/18] We supported **agent tuning** for most models, equipping model with tool using abilities by fine-tuning with `--dataset glaive_toolcall`.
+[24/01/18] We supported **agent tuning** for most models, equipping model with tool using abilities by fine-tuning with `dataset: glaive_toolcall`.
 
-[23/12/23] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s implementation to boost LoRA tuning for the LLaMA, Mistral and Yi models. Try `--use_unsloth` argument to activate unsloth patch. It achieves **170%** speed in our benchmark, check [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison) for details.
+[23/12/23] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s implementation to boost LoRA tuning for the LLaMA, Mistral and Yi models. Try `use_unsloth: true` argument to activate unsloth patch. It achieves **170%** speed in our benchmark, check [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison) for details.
 
 [23/12/12] We supported fine-tuning the latest MoE model **[Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-v0.1)** in our framework. See hardware requirement [here](#hardware-requirement).
 
-[23/12/01] We supported downloading pre-trained models and datasets from the **[ModelScope Hub](https://modelscope.cn/models)** for Chinese mainland users. See [this tutorial](#use-modelscope-hub-optional) for usage.
+[23/12/01] We supported downloading pre-trained models and datasets from the **[ModelScope Hub](https://modelscope.cn/models)** for Chinese mainland users. See [this tutorial](#download-from-modelscope-hub) for usage.
 
-[23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `--neftune_noise_alpha` argument to activate NEFTune, e.g., `--neftune_noise_alpha 5`.
+[23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `neftune_noise_alpha: 5` argument to activate NEFTune.
 
-[23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `--shift_attn` argument to enable shift short attention.
+[23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `shift_attn: true` argument to enable shift short attention.
 
-[23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [this example](#evaluation) to evaluate your models.
+[23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [examples](examples/README.md) for usage.
 
-[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
+[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `flash_attn: fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
 
-[23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `--rope_scaling linear` argument in training and `--rope_scaling dynamic` argument at inference to extrapolate the position embeddings.
+[23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `rope_scaling: linear` argument in training and `rope_scaling: dynamic` argument at inference to extrapolate the position embeddings.
 
-[23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [this example](#dpo-training) to train your models.
+[23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [examples](examples/README.md) for usage.
 
-[23/07/31] We supported **dataset streaming**. Try `--streaming` and `--max_steps 10000` arguments to load your dataset in streaming mode.
+[23/07/31] We supported **dataset streaming**. Try `streaming: true` and `max_steps: 10000` arguments to load your dataset in streaming mode.
 
 [23/07/29] We released two instruction-tuned 13B models at Hugging Face. See these Hugging Face Repos ([LLaMA-2](https://huggingface.co/hiyouga/Llama-2-Chinese-13b-chat) / [Baichuan](https://huggingface.co/hiyouga/Baichuan-13B-sft)) for details.
 
 [23/07/18] We developed an **all-in-one Web UI** for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
 [23/07/09] We released **[FastEdit](https://github.com/hiyouga/FastEdit)** ⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/06/29] We provided a **reproducible example** of training a chat model using instruction-following datasets, see [Baichuan-7B-sft](https://huggingface.co/hiyouga/Baichuan-7B-sft) for details.
 
 [23/06/22] We aligned the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
-[23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
+[23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). See [examples](examples/README.md) for usage.
 
 </details>
 
 ## Supported Models
 
 | Model                                                    | Model size                       | Default module    | Template  |
 | -------------------------------------------------------- | -------------------------------- | ----------------- | --------- |
 | [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                           | W_pack            | baichuan2 |
 | [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
 | [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
 | [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                               | query_key_value   | chatglm3  |
 | [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                         | q_proj,v_proj     | cohere    |
-| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                       | q_proj,v_proj     | deepseek  |
+| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B/236B                  | q_proj,v_proj     | deepseek  |
 | [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                      | query_key_value   | falcon    |
 | [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                            | q_proj,v_proj     | gemma     |
 | [InternLM2](https://huggingface.co/internlm)             | 7B/20B                           | wqkv              | intern2   |
 | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B                   | q_proj,v_proj     | -         |
 | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                       | q_proj,v_proj     | llama2    |
 | [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                           | q_proj,v_proj     | llama3    |
 | [LLaVA-1.5](https://huggingface.co/llava-hf)             | 7B/13B                           | q_proj,v_proj     | vicuna    |
@@ -226,15 +199,16 @@
 | [OLMo](https://huggingface.co/allenai)                   | 1B/7B                            | q_proj,v_proj     | -         |
 | [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                        | q_proj,v_proj     | -         |
 | [Phi-3](https://huggingface.co/microsoft)                | 3.8B                             | qkv_proj          | phi       |
 | [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B                  | c_attn            | qwen      |
 | [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B/110B | q_proj,v_proj     | qwen      |
 | [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                        | q_proj,v_proj     | -         |
 | [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                       | q_proj,v_proj     | xverse    |
-| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yi (1/1.5)](https://huggingface.co/01-ai)               | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yi-VL](https://huggingface.co/01-ai)                    | 6B/34B                           | q_proj,v_proj     | yi_vl     |
 | [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                      | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
 > **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules for better convergence.
 >
 > For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "instruct/chat" models.
 >
@@ -272,16 +246,16 @@
 </details>
 
 <details><summary>Supervised fine-tuning datasets</summary>
 
 - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
 - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [Alpaca GPT4 (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-- [Self Cognition (zh)](data/self_cognition.json)
-- [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+- [Identity (en&zh)](data/identity.json)
+- [Open Assistant (zh)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
 - [Guanaco Dataset (multilingual)](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
 - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
 - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
 - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
 - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
 - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
@@ -321,19 +295,19 @@
 - [Ultrachat (de)](https://huggingface.co/datasets/mayflowergmbh/ultra-chat_de)
 
 </details>
 
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
-- [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
 - [DPO mixed (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
+- [Open Assistant (zh)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -343,26 +317,27 @@
 
 ## Requirement
 
 | Mandatory    | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | python       | 3.8     | 3.10      |
 | torch        | 1.13.1  | 2.2.0     |
-| transformers | 4.37.2  | 4.39.3    |
-| datasets     | 2.14.3  | 2.18.0    |
-| accelerate   | 0.27.2  | 0.28.0    |
+| transformers | 4.37.2  | 4.40.1    |
+| datasets     | 2.14.3  | 2.19.1    |
+| accelerate   | 0.27.2  | 0.30.0    |
 | peft         | 0.9.0   | 0.10.0    |
-| trl          | 0.8.1   | 0.8.1     |
+| trl          | 0.8.1   | 0.8.6     |
 
 | Optional     | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | CUDA         | 11.6    | 12.2      |
 | deepspeed    | 0.10.0  | 0.14.0    |
-| bitsandbytes | 0.39.0  | 0.43.0    |
-| flash-attn   | 2.3.0   | 2.5.6     |
+| bitsandbytes | 0.39.0  | 0.43.1    |
+| vllm         | 0.4.0   | 0.4.2     |
+| flash-attn   | 2.3.0   | 2.5.8     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
 | Method            | Bits |   7B  |  13B  |  30B  |   70B  |  110B  |  8x7B |  8x22B |
 | ----------------- | ---- | ----- | ----- | ----- | ------ | ------ | ----- | ------ |
@@ -372,64 +347,109 @@
 | LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB |  240GB | 120GB |  320GB |
 | QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  140GB |  60GB |  160GB |
 | QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |   72GB |  30GB |   96GB |
 | QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |   48GB |  18GB |   48GB |
 
 ## Getting Started
 
-### Data Preparation
-
-Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
-
-> [!NOTE]
-> Please update `data/dataset_info.json` to use your custom dataset.
+### Installation
 
-### Dependence Installation
+> [!IMPORTANT]
+> Installation is mandatory.
 
 ```bash
 git clone https://github.com/hiyouga/LLaMA-Factory.git
-conda create -n llama_factory python=3.10
-conda activate llama_factory
 cd LLaMA-Factory
-pip install -e .[metrics]
+pip install -e .[torch,metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: torch, metrics, deepspeed, bitsandbytes, vllm, galore, badam, gptq, awq, aqlm, qwen, modelscope, quality
+
+> [!TIP]
+> Use `pip install --no-deps -e .` to resolve package conflicts.
 
 <details><summary>For Windows users</summary>
 
-If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
+If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you need to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
 ```
 
 To enable FlashAttention-2 on the Windows platform, you need to install the precompiled `flash-attn` library, which supports CUDA 12.1 to 12.2. Please download the corresponding version from [flash-attention](https://github.com/bdashore3/flash-attention/releases) based on your requirements.
 
 </details>
 
-### Train with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
+<details><summary>For Ascend NPU users</summary>
+
+To utilize Ascend NPU devices for (distributed) training and inference, you need to install the **[torch-npu](https://gitee.com/ascend/pytorch)** library and the **[Ascend CANN Kernels](https://www.hiascend.com/developer/download/community/result?module=cann)**.
+
+| Requirement  | Minimum | Recommend |
+| ------------ | ------- | --------- |
+| CANN         | 8.0.RC1 | 8.0.RC1   |
+| torch        | 2.2.0   | 2.2.0     |
+| torch-npu    | 2.2.0   | 2.2.0     |
+| deepspeed    | 0.13.2  | 0.13.2    |
+
+Docker image:
+
+- 32GB: [Download page](http://mirrors.cn-central-221.ovaijisuan.com/detail/130.html)
+- 64GB: Coming soon
+
+Remember to use `ASCEND_RT_VISIBLE_DEVICES` instead of `CUDA_VISIBLE_DEVICES` to specify the device to use.
+
+If you cannot infer model on NPU devices, try setting `do_sample: false` in the configurations.
+
+</details>
+
+### Data Preparation
+
+Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
+
+> [!NOTE]
+> Please update `data/dataset_info.json` to use your custom dataset.
+
+### Quickstart
+
+Use the following 3 commands to run LoRA **fine-tuning**, **inference** and **merging** of the Llama3-8B-Instruct model, respectively.
+
+```bash
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli train examples/lora_single_gpu/llama3_lora_sft.yaml
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli chat examples/inference/llama3_lora_sft.yaml
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli export examples/merge_lora/llama3_lora_sft.yaml
+```
+
+See [examples/README.md](examples/README.md) for advanced usage (including distributed training).
+
+> [!TIP]
+> Use `llamafactory-cli help` to show help information.
+
+### Fine-Tuning with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
 
 > [!IMPORTANT]
-> LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
+> LLaMA Board GUI only supports training on a single GPU.
 
 #### Use local environment
 
 ```bash
-export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
-export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
-python src/train_web.py # or python -m llmtuner.webui.interface
+CUDA_VISIBLE_DEVICES=0 GRADIO_SHARE=1 llamafactory-cli webui
 ```
 
-<details><summary>For Alibaba Cloud users</summary>
+<details><summary>For Alibaba Cloud PAI or AutoDL users</summary>
 
-If you encountered display problems in LLaMA Board on Alibaba Cloud, try using the following command to set environment variables before starting LLaMA Board:
+If you encountered display problems in LLaMA Board on Alibaba Cloud PAI, try using the following command to set environment variables before starting LLaMA Board:
 
 ```bash
-export GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+export GRADIO_SERVER_PORT=7860 GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+```
+
+If you are using AutoDL, please install a specific version of Gradio:
+
+```bash
+pip install gradio==4.10.0
 ```
 
 </details>
 
 #### Use Docker
 
 ```bash
@@ -455,28 +475,18 @@
 
 - hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
 - data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
 - output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
 
 </details>
 
-### Train with Command Line Interface
-
-See [examples/README.md](examples/README.md) for usage.
-
-Use `python src/train_bash.py -h` to display arguments description.
-
 ### Deploy with OpenAI-style API and vLLM
 
 ```bash
-CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 python src/api_demo.py \
-    --model_name_or_path meta-llama/Meta-Llama-3-8B-Instruct \
-    --template llama3 \
-    --infer_backend vllm \
-    --vllm_enforce_eager
+CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 llamafactory-cli api examples/inference/llama3_vllm.yaml
 ```
 
 ### Download from ModelScope Hub
 
 If you have trouble with downloading models and datasets from Hugging Face, you can use ModelScope.
 
 ```bash
@@ -508,35 +518,45 @@
 1. Cao et al. Head-wise Shareable Attention for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.11819)
 1. Zhang et al. Enhancing Multilingual Capabilities of Large Language Models through Self-Distillation from Resource-Rich Languages. 2024. [[arxiv]](https://arxiv.org/abs/2402.12204)
 1. Kim et al. Efficient and Effective Vocabulary Expansion Towards Multilingual Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.14714)
 1. Yu et al. KIEval: A Knowledge-grounded Interactive Evaluation Framework for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.15043)
 1. Huang et al. Key-Point-Driven Data Synthesis with its Enhancement on Mathematical Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2403.02333)
 1. Duan et al. Negating Negatives: Alignment without Human Positive Samples via Distributional Dispreference Optimization. 2024. [[arxiv]](https://arxiv.org/abs/2403.03419)
 1. Xie and Schwertfeger. Empowering Robotics with Large Language Models: osmAG Map Comprehension with LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2403.08228)
+1. Wu et al. Large Language Models are Parallel Multilingual Learners. 2024. [[arxiv]](https://arxiv.org/abs/2403.09073)
 1. Zhang et al. EDT: Improving Large Language Models' Generation by Entropy-based Dynamic Temperature Sampling. 2024. [[arxiv]](https://arxiv.org/abs/2403.14541)
 1. Weller et al. FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions. 2024. [[arxiv]](https://arxiv.org/abs/2403.15246)
 1. Hongbin Na. CBT-LLM: A Chinese Large Language Model for Cognitive Behavioral Therapy-based Mental Health Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2403.16008)
 1. Zan et al. CodeS: Natural Language to Code Repository via Multi-Layer Sketch. 2024. [[arxiv]](https://arxiv.org/abs/2403.16443)
 1. Liu et al. Extensive Self-Contrast Enables Feedback-Free Language Model Alignment. 2024. [[arxiv]](https://arxiv.org/abs/2404.00604)
 1. Luo et al. BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.02827)
 1. Du et al. Chinese Tiny LLM: Pretraining a Chinese-Centric Large Language Model. 2024. [[arxiv]](https://arxiv.org/abs/2404.04167)
+1. Ma et al. Parameter Efficient Quasi-Orthogonal Fine-Tuning via Givens Rotation. 2024. [[arxiv]](https://arxiv.org/abs/2404.04316)
 1. Liu et al. Dynamic Generation of Personalities with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.07084)
+1. Shang et al. How Far Have We Gone in Stripped Binary Code Understanding Using Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.09836)
+1. Huang et al. LLMTune: Accelerate Database Knob Tuning with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.11581)
+1. Deng et al. Text-Tuple-Table: Towards Information Integration in Text-to-Table Generation via Global Tuple Extraction. 2024. [[arxiv]](https://arxiv.org/abs/2404.14215)
+1. Acikgoz et al. Hippocrates: An Open-Source Framework for Advancing Large Language Models in Healthcare. 2024. [[arxiv]](https://arxiv.org/abs/2404.16621)
+1. Zhang et al. Small Language Models Need Strong Verifiers to Self-Correct Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2404.17140)
+1. Zhou et al. FREB-TQA: A Fine-Grained Robustness Evaluation Benchmark for Table Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2404.18585)
 1. **[StarWhisper](https://github.com/Yu-Yang-Li/StarWhisper)**: A large language model for Astronomy, based on ChatGLM2-6B and Qwen-14B.
 1. **[DISC-LawLLM](https://github.com/FudanDISC/DISC-LawLLM)**: A large language model specialized in Chinese legal domain, based on Baichuan-13B, is capable of retrieving and reasoning on legal knowledge.
 1. **[Sunsimiao](https://github.com/thomas-yanxin/Sunsimiao)**: A large language model specialized in Chinese medical domain, based on Baichuan-7B and ChatGLM-6B.
 1. **[CareGPT](https://github.com/WangRongsheng/CareGPT)**: A series of large language models for Chinese medical domain, based on LLaMA2-7B and Baichuan-13B.
 1. **[MachineMindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)**: A series of MBTI Personality large language models, capable of giving any LLM 16 different personality types based on different datasets and training methods.
+1. **[Luminia-13B-v3](https://huggingface.co/Nekochu/Luminia-13B-v3)**: A large language model specialized in generate metadata for stable diffusion. [[🤗Demo]](https://huggingface.co/spaces/Nekochu/Luminia-13B_SD_Prompt)
+1. **[Chinese-LLaVA-Med](https://github.com/BUAADreamer/Chinese-LLaVA-Med)**: A multimodal large language model specialized in Chinese medical domain, based on LLaVA-1.5-7B.
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2/LLaVA-1.5](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2 (LLaVA-1.5)](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yi-1.5](LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.7.0/README.md` & `llmtuner-0.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 ![# LLaMA Factory](assets/logo.png)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Factory)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Factory)](https://github.com/hiyouga/LLaMA-Factory/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![Downloads](https://static.pepy.tech/badge/llmtuner)](https://pypi.org/project/llmtuner/)
-[![Citation](https://img.shields.io/badge/citation-34-green)](#projects-using-llama-factory)
+[![Citation](https://img.shields.io/badge/citation-44-green)](#projects-using-llama-factory)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
 [![Discord](https://dcbadge.vercel.app/api/server/rKfvV9r9FK?compact=true&style=flat)](https://discord.gg/rKfvV9r9FK)
 [![Twitter](https://img.shields.io/twitter/follow/llamafactory_ai)](https://twitter.com/llamafactory_ai)
 [![Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue)](https://huggingface.co/spaces/hiyouga/LLaMA-Board)
 [![Studios](https://img.shields.io/badge/ModelScope-Open%20in%20Studios-blue)](https://modelscope.cn/studios/hiyouga/LLaMA-Board)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)
 
+[![GitHub Tread](https://trendshift.io/api/badge/repositories/4535)](https://trendshift.io/repositories/4535)
+
 👋 Join our [WeChat](assets/wechat.jpg).
 
 \[ English | [中文](README_zh.md) \]
 
 **Fine-tuning a large language model can be easy as...**
 
 https://github.com/hiyouga/LLaMA-Factory/assets/16256802/9840a653-7e9c-41c8-ae89-7ace5698baf6
@@ -64,90 +66,94 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
-[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See `examples/lora_single_gpu/sft_mllm.sh` for usage.
+[24/05/14] We supported training and inference on the Ascend NPU devices. Check [installation](#installation) section for details.
+
+[24/05/13] We supported fine-tuning the **Yi-1.5** series models.
+
+[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See [examples](examples/README.md) for usage.
+
+<details><summary>Full Changelog</summary>
 
 [24/04/22] We provided a **[Colab notebook](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)** for fine-tuning the Llama-3 model on a free T4 GPU. Two Llama-3-derived models fine-tuned using LLaMA Factory are available at Hugging Face, check [Llama3-8B-Chinese-Chat](https://huggingface.co/shenzhi-wang/Llama3-8B-Chinese-Chat) and [Llama3-Chinese](https://huggingface.co/zhichen/Llama3-Chinese) for details.
 
-[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See [examples](examples/README.md) for usage.
 
-[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
+[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See [examples](examples/README.md) for usage.
 
 [24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
 
-<details><summary>Full Changelog</summary>
-
-[24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See `examples/lora_single_gpu` for usage.
+[24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See [examples](examples/README.md) for usage.
 
 [24/03/21] Our paper "[LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models](https://arxiv.org/abs/2403.13372)" is available at arXiv!
 
-[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/extras/fsdp_qlora` for usage.
+[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See [examples](examples/README.md) for usage.
 
-[24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See `examples/extras/loraplus` for usage.
+[24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See [examples](examples/README.md) for usage.
 
-[24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See `examples/extras/galore` for usage.
+[24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See [examples](examples/README.md) for usage.
 
-[24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `--infer_backend vllm` to enjoy **270%** inference speed. (LoRA is not yet supported, merge it first.)
+[24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `infer_backend: vllm` to enjoy **270%** inference speed.
 
-[24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `--use_dora` to activate DoRA training.
+[24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `use_dora: true` to activate DoRA training.
 
-[24/02/15] We supported **block expansion** proposed by [LLaMA Pro](https://github.com/TencentARC/LLaMA-Pro). See `examples/extras/llama_pro` for usage.
+[24/02/15] We supported **block expansion** proposed by [LLaMA Pro](https://github.com/TencentARC/LLaMA-Pro). See [examples](examples/README.md) for usage.
 
 [24/02/05] Qwen1.5 (Qwen2 beta version) series models are supported in LLaMA-Factory. Check this [blog post](https://qwenlm.github.io/blog/qwen1.5/) for details.
 
-[24/01/18] We supported **agent tuning** for most models, equipping model with tool using abilities by fine-tuning with `--dataset glaive_toolcall`.
+[24/01/18] We supported **agent tuning** for most models, equipping model with tool using abilities by fine-tuning with `dataset: glaive_toolcall`.
 
-[23/12/23] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s implementation to boost LoRA tuning for the LLaMA, Mistral and Yi models. Try `--use_unsloth` argument to activate unsloth patch. It achieves **170%** speed in our benchmark, check [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison) for details.
+[23/12/23] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s implementation to boost LoRA tuning for the LLaMA, Mistral and Yi models. Try `use_unsloth: true` argument to activate unsloth patch. It achieves **170%** speed in our benchmark, check [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison) for details.
 
 [23/12/12] We supported fine-tuning the latest MoE model **[Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-v0.1)** in our framework. See hardware requirement [here](#hardware-requirement).
 
-[23/12/01] We supported downloading pre-trained models and datasets from the **[ModelScope Hub](https://modelscope.cn/models)** for Chinese mainland users. See [this tutorial](#use-modelscope-hub-optional) for usage.
+[23/12/01] We supported downloading pre-trained models and datasets from the **[ModelScope Hub](https://modelscope.cn/models)** for Chinese mainland users. See [this tutorial](#download-from-modelscope-hub) for usage.
 
-[23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `--neftune_noise_alpha` argument to activate NEFTune, e.g., `--neftune_noise_alpha 5`.
+[23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `neftune_noise_alpha: 5` argument to activate NEFTune.
 
-[23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `--shift_attn` argument to enable shift short attention.
+[23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `shift_attn: true` argument to enable shift short attention.
 
-[23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [this example](#evaluation) to evaluate your models.
+[23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [examples](examples/README.md) for usage.
 
-[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
+[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `flash_attn: fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
 
-[23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `--rope_scaling linear` argument in training and `--rope_scaling dynamic` argument at inference to extrapolate the position embeddings.
+[23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `rope_scaling: linear` argument in training and `rope_scaling: dynamic` argument at inference to extrapolate the position embeddings.
 
-[23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [this example](#dpo-training) to train your models.
+[23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [examples](examples/README.md) for usage.
 
-[23/07/31] We supported **dataset streaming**. Try `--streaming` and `--max_steps 10000` arguments to load your dataset in streaming mode.
+[23/07/31] We supported **dataset streaming**. Try `streaming: true` and `max_steps: 10000` arguments to load your dataset in streaming mode.
 
 [23/07/29] We released two instruction-tuned 13B models at Hugging Face. See these Hugging Face Repos ([LLaMA-2](https://huggingface.co/hiyouga/Llama-2-Chinese-13b-chat) / [Baichuan](https://huggingface.co/hiyouga/Baichuan-13B-sft)) for details.
 
 [23/07/18] We developed an **all-in-one Web UI** for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
 [23/07/09] We released **[FastEdit](https://github.com/hiyouga/FastEdit)** ⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/06/29] We provided a **reproducible example** of training a chat model using instruction-following datasets, see [Baichuan-7B-sft](https://huggingface.co/hiyouga/Baichuan-7B-sft) for details.
 
 [23/06/22] We aligned the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
-[23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
+[23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). See [examples](examples/README.md) for usage.
 
 </details>
 
 ## Supported Models
 
 | Model                                                    | Model size                       | Default module    | Template  |
 | -------------------------------------------------------- | -------------------------------- | ----------------- | --------- |
 | [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                           | W_pack            | baichuan2 |
 | [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
 | [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
 | [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                               | query_key_value   | chatglm3  |
 | [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                         | q_proj,v_proj     | cohere    |
-| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                       | q_proj,v_proj     | deepseek  |
+| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B/236B                  | q_proj,v_proj     | deepseek  |
 | [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                      | query_key_value   | falcon    |
 | [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                            | q_proj,v_proj     | gemma     |
 | [InternLM2](https://huggingface.co/internlm)             | 7B/20B                           | wqkv              | intern2   |
 | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B                   | q_proj,v_proj     | -         |
 | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                       | q_proj,v_proj     | llama2    |
 | [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                           | q_proj,v_proj     | llama3    |
 | [LLaVA-1.5](https://huggingface.co/llava-hf)             | 7B/13B                           | q_proj,v_proj     | vicuna    |
@@ -155,15 +161,16 @@
 | [OLMo](https://huggingface.co/allenai)                   | 1B/7B                            | q_proj,v_proj     | -         |
 | [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                        | q_proj,v_proj     | -         |
 | [Phi-3](https://huggingface.co/microsoft)                | 3.8B                             | qkv_proj          | phi       |
 | [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B                  | c_attn            | qwen      |
 | [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B/110B | q_proj,v_proj     | qwen      |
 | [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                        | q_proj,v_proj     | -         |
 | [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                       | q_proj,v_proj     | xverse    |
-| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yi (1/1.5)](https://huggingface.co/01-ai)               | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yi-VL](https://huggingface.co/01-ai)                    | 6B/34B                           | q_proj,v_proj     | yi_vl     |
 | [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                      | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
 > **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules for better convergence.
 >
 > For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "instruct/chat" models.
 >
@@ -201,16 +208,16 @@
 </details>
 
 <details><summary>Supervised fine-tuning datasets</summary>
 
 - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
 - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [Alpaca GPT4 (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-- [Self Cognition (zh)](data/self_cognition.json)
-- [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+- [Identity (en&zh)](data/identity.json)
+- [Open Assistant (zh)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
 - [Guanaco Dataset (multilingual)](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
 - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
 - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
 - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
 - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
 - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
@@ -250,19 +257,19 @@
 - [Ultrachat (de)](https://huggingface.co/datasets/mayflowergmbh/ultra-chat_de)
 
 </details>
 
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
-- [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
 - [DPO mixed (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
+- [Open Assistant (zh)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -272,26 +279,27 @@
 
 ## Requirement
 
 | Mandatory    | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | python       | 3.8     | 3.10      |
 | torch        | 1.13.1  | 2.2.0     |
-| transformers | 4.37.2  | 4.39.3    |
-| datasets     | 2.14.3  | 2.18.0    |
-| accelerate   | 0.27.2  | 0.28.0    |
+| transformers | 4.37.2  | 4.40.1    |
+| datasets     | 2.14.3  | 2.19.1    |
+| accelerate   | 0.27.2  | 0.30.0    |
 | peft         | 0.9.0   | 0.10.0    |
-| trl          | 0.8.1   | 0.8.1     |
+| trl          | 0.8.1   | 0.8.6     |
 
 | Optional     | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | CUDA         | 11.6    | 12.2      |
 | deepspeed    | 0.10.0  | 0.14.0    |
-| bitsandbytes | 0.39.0  | 0.43.0    |
-| flash-attn   | 2.3.0   | 2.5.6     |
+| bitsandbytes | 0.39.0  | 0.43.1    |
+| vllm         | 0.4.0   | 0.4.2     |
+| flash-attn   | 2.3.0   | 2.5.8     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
 | Method            | Bits |   7B  |  13B  |  30B  |   70B  |  110B  |  8x7B |  8x22B |
 | ----------------- | ---- | ----- | ----- | ----- | ------ | ------ | ----- | ------ |
@@ -301,64 +309,109 @@
 | LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB |  240GB | 120GB |  320GB |
 | QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  140GB |  60GB |  160GB |
 | QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |   72GB |  30GB |   96GB |
 | QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |   48GB |  18GB |   48GB |
 
 ## Getting Started
 
-### Data Preparation
-
-Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
+### Installation
 
-> [!NOTE]
-> Please update `data/dataset_info.json` to use your custom dataset.
-
-### Dependence Installation
+> [!IMPORTANT]
+> Installation is mandatory.
 
 ```bash
 git clone https://github.com/hiyouga/LLaMA-Factory.git
-conda create -n llama_factory python=3.10
-conda activate llama_factory
 cd LLaMA-Factory
-pip install -e .[metrics]
+pip install -e .[torch,metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: torch, metrics, deepspeed, bitsandbytes, vllm, galore, badam, gptq, awq, aqlm, qwen, modelscope, quality
+
+> [!TIP]
+> Use `pip install --no-deps -e .` to resolve package conflicts.
 
 <details><summary>For Windows users</summary>
 
-If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
+If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you need to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
 ```
 
 To enable FlashAttention-2 on the Windows platform, you need to install the precompiled `flash-attn` library, which supports CUDA 12.1 to 12.2. Please download the corresponding version from [flash-attention](https://github.com/bdashore3/flash-attention/releases) based on your requirements.
 
 </details>
 
-### Train with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
+<details><summary>For Ascend NPU users</summary>
+
+To utilize Ascend NPU devices for (distributed) training and inference, you need to install the **[torch-npu](https://gitee.com/ascend/pytorch)** library and the **[Ascend CANN Kernels](https://www.hiascend.com/developer/download/community/result?module=cann)**.
+
+| Requirement  | Minimum | Recommend |
+| ------------ | ------- | --------- |
+| CANN         | 8.0.RC1 | 8.0.RC1   |
+| torch        | 2.2.0   | 2.2.0     |
+| torch-npu    | 2.2.0   | 2.2.0     |
+| deepspeed    | 0.13.2  | 0.13.2    |
+
+Docker image:
+
+- 32GB: [Download page](http://mirrors.cn-central-221.ovaijisuan.com/detail/130.html)
+- 64GB: Coming soon
+
+Remember to use `ASCEND_RT_VISIBLE_DEVICES` instead of `CUDA_VISIBLE_DEVICES` to specify the device to use.
+
+If you cannot infer model on NPU devices, try setting `do_sample: false` in the configurations.
+
+</details>
+
+### Data Preparation
+
+Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
+
+> [!NOTE]
+> Please update `data/dataset_info.json` to use your custom dataset.
+
+### Quickstart
+
+Use the following 3 commands to run LoRA **fine-tuning**, **inference** and **merging** of the Llama3-8B-Instruct model, respectively.
+
+```bash
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli train examples/lora_single_gpu/llama3_lora_sft.yaml
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli chat examples/inference/llama3_lora_sft.yaml
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli export examples/merge_lora/llama3_lora_sft.yaml
+```
+
+See [examples/README.md](examples/README.md) for advanced usage (including distributed training).
+
+> [!TIP]
+> Use `llamafactory-cli help` to show help information.
+
+### Fine-Tuning with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
 
 > [!IMPORTANT]
-> LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
+> LLaMA Board GUI only supports training on a single GPU.
 
 #### Use local environment
 
 ```bash
-export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
-export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
-python src/train_web.py # or python -m llmtuner.webui.interface
+CUDA_VISIBLE_DEVICES=0 GRADIO_SHARE=1 llamafactory-cli webui
 ```
 
-<details><summary>For Alibaba Cloud users</summary>
+<details><summary>For Alibaba Cloud PAI or AutoDL users</summary>
 
-If you encountered display problems in LLaMA Board on Alibaba Cloud, try using the following command to set environment variables before starting LLaMA Board:
+If you encountered display problems in LLaMA Board on Alibaba Cloud PAI, try using the following command to set environment variables before starting LLaMA Board:
 
 ```bash
-export GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+export GRADIO_SERVER_PORT=7860 GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+```
+
+If you are using AutoDL, please install a specific version of Gradio:
+
+```bash
+pip install gradio==4.10.0
 ```
 
 </details>
 
 #### Use Docker
 
 ```bash
@@ -384,28 +437,18 @@
 
 - hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
 - data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
 - output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
 
 </details>
 
-### Train with Command Line Interface
-
-See [examples/README.md](examples/README.md) for usage.
-
-Use `python src/train_bash.py -h` to display arguments description.
-
 ### Deploy with OpenAI-style API and vLLM
 
 ```bash
-CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 python src/api_demo.py \
-    --model_name_or_path meta-llama/Meta-Llama-3-8B-Instruct \
-    --template llama3 \
-    --infer_backend vllm \
-    --vllm_enforce_eager
+CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 llamafactory-cli api examples/inference/llama3_vllm.yaml
 ```
 
 ### Download from ModelScope Hub
 
 If you have trouble with downloading models and datasets from Hugging Face, you can use ModelScope.
 
 ```bash
@@ -437,35 +480,45 @@
 1. Cao et al. Head-wise Shareable Attention for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.11819)
 1. Zhang et al. Enhancing Multilingual Capabilities of Large Language Models through Self-Distillation from Resource-Rich Languages. 2024. [[arxiv]](https://arxiv.org/abs/2402.12204)
 1. Kim et al. Efficient and Effective Vocabulary Expansion Towards Multilingual Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.14714)
 1. Yu et al. KIEval: A Knowledge-grounded Interactive Evaluation Framework for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.15043)
 1. Huang et al. Key-Point-Driven Data Synthesis with its Enhancement on Mathematical Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2403.02333)
 1. Duan et al. Negating Negatives: Alignment without Human Positive Samples via Distributional Dispreference Optimization. 2024. [[arxiv]](https://arxiv.org/abs/2403.03419)
 1. Xie and Schwertfeger. Empowering Robotics with Large Language Models: osmAG Map Comprehension with LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2403.08228)
+1. Wu et al. Large Language Models are Parallel Multilingual Learners. 2024. [[arxiv]](https://arxiv.org/abs/2403.09073)
 1. Zhang et al. EDT: Improving Large Language Models' Generation by Entropy-based Dynamic Temperature Sampling. 2024. [[arxiv]](https://arxiv.org/abs/2403.14541)
 1. Weller et al. FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions. 2024. [[arxiv]](https://arxiv.org/abs/2403.15246)
 1. Hongbin Na. CBT-LLM: A Chinese Large Language Model for Cognitive Behavioral Therapy-based Mental Health Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2403.16008)
 1. Zan et al. CodeS: Natural Language to Code Repository via Multi-Layer Sketch. 2024. [[arxiv]](https://arxiv.org/abs/2403.16443)
 1. Liu et al. Extensive Self-Contrast Enables Feedback-Free Language Model Alignment. 2024. [[arxiv]](https://arxiv.org/abs/2404.00604)
 1. Luo et al. BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.02827)
 1. Du et al. Chinese Tiny LLM: Pretraining a Chinese-Centric Large Language Model. 2024. [[arxiv]](https://arxiv.org/abs/2404.04167)
+1. Ma et al. Parameter Efficient Quasi-Orthogonal Fine-Tuning via Givens Rotation. 2024. [[arxiv]](https://arxiv.org/abs/2404.04316)
 1. Liu et al. Dynamic Generation of Personalities with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.07084)
+1. Shang et al. How Far Have We Gone in Stripped Binary Code Understanding Using Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.09836)
+1. Huang et al. LLMTune: Accelerate Database Knob Tuning with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.11581)
+1. Deng et al. Text-Tuple-Table: Towards Information Integration in Text-to-Table Generation via Global Tuple Extraction. 2024. [[arxiv]](https://arxiv.org/abs/2404.14215)
+1. Acikgoz et al. Hippocrates: An Open-Source Framework for Advancing Large Language Models in Healthcare. 2024. [[arxiv]](https://arxiv.org/abs/2404.16621)
+1. Zhang et al. Small Language Models Need Strong Verifiers to Self-Correct Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2404.17140)
+1. Zhou et al. FREB-TQA: A Fine-Grained Robustness Evaluation Benchmark for Table Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2404.18585)
 1. **[StarWhisper](https://github.com/Yu-Yang-Li/StarWhisper)**: A large language model for Astronomy, based on ChatGLM2-6B and Qwen-14B.
 1. **[DISC-LawLLM](https://github.com/FudanDISC/DISC-LawLLM)**: A large language model specialized in Chinese legal domain, based on Baichuan-13B, is capable of retrieving and reasoning on legal knowledge.
 1. **[Sunsimiao](https://github.com/thomas-yanxin/Sunsimiao)**: A large language model specialized in Chinese medical domain, based on Baichuan-7B and ChatGLM-6B.
 1. **[CareGPT](https://github.com/WangRongsheng/CareGPT)**: A series of large language models for Chinese medical domain, based on LLaMA2-7B and Baichuan-13B.
 1. **[MachineMindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)**: A series of MBTI Personality large language models, capable of giving any LLM 16 different personality types based on different datasets and training methods.
+1. **[Luminia-13B-v3](https://huggingface.co/Nekochu/Luminia-13B-v3)**: A large language model specialized in generate metadata for stable diffusion. [[🤗Demo]](https://huggingface.co/spaces/Nekochu/Luminia-13B_SD_Prompt)
+1. **[Chinese-LLaVA-Med](https://github.com/BUAADreamer/Chinese-LLaVA-Med)**: A multimodal large language model specialized in Chinese medical domain, based on LLaVA-1.5-7B.
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2/LLaVA-1.5](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2 (LLaVA-1.5)](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yi-1.5](LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.7.0/pyproject.toml` & `llmtuner-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/setup.py` & `llmtuner-0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import os
 import re
 
 from setuptools import find_packages, setup
 
 
 def get_version():
-    with open(os.path.join("src", "llmtuner", "__init__.py"), "r", encoding="utf-8") as f:
+    with open(os.path.join("src", "llmtuner", "cli.py"), "r", encoding="utf-8") as f:
         file_content = f.read()
-        pattern = r"{0}\W*=\W*\"([^\"]+)\"".format("__version__")
+        pattern = r"{}\W*=\W*\"([^\"]+)\"".format("VERSION")
         (version,) = re.findall(pattern, file_content)
         return version
 
 
 def get_requires():
     with open("requirements.txt", "r", encoding="utf-8") as f:
         file_content = f.read()
         lines = [line.strip() for line in file_content.strip().split("\n") if not line.startswith("#")]
         return lines
 
 
 extra_require = {
-    "deepspeed": ["deepspeed>=0.10.0"],
+    "torch": ["torch>=1.13.1"],
     "metrics": ["nltk", "jieba", "rouge-chinese"],
+    "deepspeed": ["deepspeed>=0.10.0,<=0.14.0"],
+    "bitsandbytes": ["bitsandbytes>=0.39.0"],
+    "vllm": ["vllm>=0.4.0"],
     "galore": ["galore-torch"],
     "badam": ["badam"],
-    "vllm": ["vllm>=0.4.0"],
-    "bitsandbytes": ["bitsandbytes>=0.39.0"],
     "gptq": ["optimum>=1.16.0", "auto-gptq>=0.5.0"],
     "awq": ["autoawq"],
     "aqlm": ["aqlm[gpu]>=1.1.0"],
     "qwen": ["tiktoken", "transformers_stream_generator"],
     "modelscope": ["modelscope"],
     "quality": ["ruff"],
 }
@@ -48,14 +49,15 @@
         license="Apache 2.0 License",
         url="https://github.com/hiyouga/LLaMA-Factory",
         package_dir={"": "src"},
         packages=find_packages("src"),
         python_requires=">=3.8.0",
         install_requires=get_requires(),
         extras_require=extra_require,
+        entry_points={"console_scripts": ["llamafactory-cli = llmtuner.cli:main"]},
         classifiers=[
             "Development Status :: 4 - Beta",
             "Intended Audience :: Developers",
             "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
```

### Comparing `llmtuner-0.7.0/src/llmtuner/api/app.py` & `llmtuner-0.7.1/src/llmtuner/api/chat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,230 +1,186 @@
 import json
-import os
-from contextlib import asynccontextmanager
-from typing import Any, Dict, Sequence
+import uuid
+from typing import TYPE_CHECKING, AsyncGenerator, Dict, List, Optional, Tuple
 
-from pydantic import BaseModel
-
-from ..chat import ChatModel
 from ..data import Role as DataRole
-from ..extras.misc import torch_gc
-from ..extras.packages import is_fastapi_availble, is_starlette_available, is_uvicorn_available
+from ..extras.logging import get_logger
+from ..extras.packages import is_fastapi_available
+from .common import dictify, jsonify
 from .protocol import (
     ChatCompletionMessage,
-    ChatCompletionRequest,
     ChatCompletionResponse,
     ChatCompletionResponseChoice,
-    ChatCompletionResponseStreamChoice,
     ChatCompletionResponseUsage,
     ChatCompletionStreamResponse,
+    ChatCompletionStreamResponseChoice,
     Finish,
     Function,
     FunctionCall,
-    ModelCard,
-    ModelList,
     Role,
-    ScoreEvaluationRequest,
     ScoreEvaluationResponse,
 )
 
 
-if is_fastapi_availble():
-    from fastapi import FastAPI, HTTPException, status
-    from fastapi.middleware.cors import CORSMiddleware
-
-
-if is_starlette_available():
-    from sse_starlette import EventSourceResponse
-
-
-if is_uvicorn_available():
-    import uvicorn
-
+if is_fastapi_available():
+    from fastapi import HTTPException, status
 
-@asynccontextmanager
-async def lifespan(app: "FastAPI"):  # collects GPU memory
-    yield
-    torch_gc()
-
-
-def dictify(data: "BaseModel") -> Dict[str, Any]:
-    try:  # pydantic v2
-        return data.model_dump(exclude_unset=True)
-    except AttributeError:  # pydantic v1
-        return data.dict(exclude_unset=True)
 
+if TYPE_CHECKING:
+    from ..chat import ChatModel
+    from .protocol import ChatCompletionRequest, ScoreEvaluationRequest
+
+
+logger = get_logger(__name__)
+ROLE_MAPPING = {
+    Role.USER: DataRole.USER.value,
+    Role.ASSISTANT: DataRole.ASSISTANT.value,
+    Role.SYSTEM: DataRole.SYSTEM.value,
+    Role.FUNCTION: DataRole.FUNCTION.value,
+    Role.TOOL: DataRole.OBSERVATION.value,
+}
+
+
+def _process_request(request: "ChatCompletionRequest") -> Tuple[List[Dict[str, str]], str, str]:
+    logger.info("==== request ====\n{}".format(json.dumps(dictify(request), indent=2, ensure_ascii=False)))
+
+    if len(request.messages) == 0:
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid length")
+
+    if request.messages[0].role == Role.SYSTEM:
+        system = request.messages.pop(0).content
+    else:
+        system = ""
+
+    if len(request.messages) % 2 == 0:
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Only supports u/a/u/a/u...")
+
+    input_messages = []
+    for i, message in enumerate(request.messages):
+        if i % 2 == 0 and message.role not in [Role.USER, Role.TOOL]:
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid role")
+        elif i % 2 == 1 and message.role not in [Role.ASSISTANT, Role.FUNCTION]:
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid role")
+
+        if message.role == Role.ASSISTANT and isinstance(message.tool_calls, list) and len(message.tool_calls):
+            name = message.tool_calls[0].function.name
+            arguments = message.tool_calls[0].function.arguments
+            content = json.dumps({"name": name, "argument": arguments}, ensure_ascii=False)
+            input_messages.append({"role": ROLE_MAPPING[Role.FUNCTION], "content": content})
+        else:
+            input_messages.append({"role": ROLE_MAPPING[message.role], "content": message.content})
 
-def jsonify(data: "BaseModel") -> str:
-    try:  # pydantic v2
-        return json.dumps(data.model_dump(exclude_unset=True), ensure_ascii=False)
-    except AttributeError:  # pydantic v1
-        return data.json(exclude_unset=True, ensure_ascii=False)
+    tool_list = request.tools
+    if isinstance(tool_list, list) and len(tool_list):
+        try:
+            tools = json.dumps([dictify(tool.function) for tool in tool_list], ensure_ascii=False)
+        except Exception:
+            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid tools")
+    else:
+        tools = ""
+
+    return input_messages, system, tools
+
+
+def _create_stream_chat_completion_chunk(
+    completion_id: str,
+    model: str,
+    delta: "ChatCompletionMessage",
+    index: Optional[int] = 0,
+    finish_reason: Optional["Finish"] = None,
+) -> str:
+    choice_data = ChatCompletionStreamResponseChoice(index=index, delta=delta, finish_reason=finish_reason)
+    chunk = ChatCompletionStreamResponse(id=completion_id, model=model, choices=[choice_data])
+    return jsonify(chunk)
+
+
+async def create_chat_completion_response(
+    request: "ChatCompletionRequest", chat_model: "ChatModel"
+) -> "ChatCompletionResponse":
+    completion_id = "chatcmpl-{}".format(uuid.uuid4().hex)
+    input_messages, system, tools = _process_request(request)
+    responses = await chat_model.achat(
+        input_messages,
+        system,
+        tools,
+        do_sample=request.do_sample,
+        temperature=request.temperature,
+        top_p=request.top_p,
+        max_new_tokens=request.max_tokens,
+        num_return_sequences=request.n,
+        stop=request.stop,
+    )
 
+    prompt_length, response_length = 0, 0
+    choices = []
+    for i, response in enumerate(responses):
+        if tools:
+            result = chat_model.engine.template.format_tools.extract(response.response_text)
+        else:
+            result = response.response_text
 
-def create_app(chat_model: "ChatModel") -> "FastAPI":
-    app = FastAPI(lifespan=lifespan)
+        if isinstance(result, tuple):
+            name, arguments = result
+            function = Function(name=name, arguments=arguments)
+            tool_call = FunctionCall(id="call_{}".format(uuid.uuid4().hex), function=function)
+            response_message = ChatCompletionMessage(role=Role.ASSISTANT, tool_calls=[tool_call])
+            finish_reason = Finish.TOOL
+        else:
+            response_message = ChatCompletionMessage(role=Role.ASSISTANT, content=result)
+            finish_reason = Finish.STOP if response.finish_reason == "stop" else Finish.LENGTH
 
-    app.add_middleware(
-        CORSMiddleware,
-        allow_origins=["*"],
-        allow_credentials=True,
-        allow_methods=["*"],
-        allow_headers=["*"],
+        choices.append(ChatCompletionResponseChoice(index=i, message=response_message, finish_reason=finish_reason))
+        prompt_length = response.prompt_length
+        response_length += response.response_length
+
+    usage = ChatCompletionResponseUsage(
+        prompt_tokens=prompt_length,
+        completion_tokens=response_length,
+        total_tokens=prompt_length + response_length,
     )
 
-    role_mapping = {
-        Role.USER: DataRole.USER.value,
-        Role.ASSISTANT: DataRole.ASSISTANT.value,
-        Role.SYSTEM: DataRole.SYSTEM.value,
-        Role.FUNCTION: DataRole.FUNCTION.value,
-        Role.TOOL: DataRole.OBSERVATION.value,
-    }
-
-    @app.get("/v1/models", response_model=ModelList)
-    async def list_models():
-        model_card = ModelCard(id="gpt-3.5-turbo")
-        return ModelList(data=[model_card])
-
-    @app.post("/v1/chat/completions", response_model=ChatCompletionResponse, status_code=status.HTTP_200_OK)
-    async def create_chat_completion(request: ChatCompletionRequest):
-        if not chat_model.engine.can_generate:
-            raise HTTPException(status_code=status.HTTP_405_METHOD_NOT_ALLOWED, detail="Not allowed")
-
-        if len(request.messages) == 0:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid length")
-
-        if request.messages[0].role == Role.SYSTEM:
-            system = request.messages.pop(0).content
-        else:
-            system = ""
+    return ChatCompletionResponse(id=completion_id, model=request.model, choices=choices, usage=usage)
 
-        if len(request.messages) % 2 == 0:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Only supports u/a/u/a/u...")
 
-        input_messages = []
-        for i, message in enumerate(request.messages):
-            if i % 2 == 0 and message.role not in [Role.USER, Role.TOOL]:
-                raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid role")
-            elif i % 2 == 1 and message.role not in [Role.ASSISTANT, Role.FUNCTION]:
-                raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid role")
-
-            if message.role == Role.ASSISTANT and isinstance(message.tool_calls, list) and len(message.tool_calls):
-                name = message.tool_calls[0].function.name
-                arguments = message.tool_calls[0].function.arguments
-                content = json.dumps({"name": name, "argument": arguments}, ensure_ascii=False)
-                input_messages.append({"role": role_mapping[Role.FUNCTION], "content": content})
-            else:
-                input_messages.append({"role": role_mapping[message.role], "content": message.content})
-
-        tool_list = request.tools
-        if isinstance(tool_list, list) and len(tool_list):
-            try:
-                tools = json.dumps([dictify(tool.function) for tool in tool_list], ensure_ascii=False)
-            except Exception:
-                raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid tools")
-        else:
-            tools = ""
+async def create_stream_chat_completion_response(
+    request: "ChatCompletionRequest", chat_model: "ChatModel"
+) -> AsyncGenerator[str, None]:
+    completion_id = "chatcmpl-{}".format(uuid.uuid4().hex)
+    input_messages, system, tools = _process_request(request)
+    if tools:
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Cannot stream function calls.")
 
-        if request.stream:
-            if tools:
-                raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Cannot stream function calls.")
-
-            generate = stream_chat_completion(input_messages, system, tools, request)
-            return EventSourceResponse(generate, media_type="text/event-stream")
-
-        responses = await chat_model.achat(
-            input_messages,
-            system,
-            tools,
-            do_sample=request.do_sample,
-            temperature=request.temperature,
-            top_p=request.top_p,
-            max_new_tokens=request.max_tokens,
-            num_return_sequences=request.n,
-        )
-
-        prompt_length, response_length = 0, 0
-        choices = []
-        for i, response in enumerate(responses):
-            if tools:
-                result = chat_model.engine.template.format_tools.extract(response.response_text)
-            else:
-                result = response.response_text
-
-            if isinstance(result, tuple):
-                name, arguments = result
-                function = Function(name=name, arguments=arguments)
-                response_message = ChatCompletionMessage(
-                    role=Role.ASSISTANT, tool_calls=[FunctionCall(function=function)]
-                )
-                finish_reason = Finish.TOOL
-            else:
-                response_message = ChatCompletionMessage(role=Role.ASSISTANT, content=result)
-                finish_reason = Finish.STOP if response.finish_reason == "stop" else Finish.LENGTH
+    if request.n > 1:
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Cannot stream multiple responses.")
 
-            choices.append(
-                ChatCompletionResponseChoice(index=i, message=response_message, finish_reason=finish_reason)
+    yield _create_stream_chat_completion_chunk(
+        completion_id=completion_id, model=request.model, delta=ChatCompletionMessage(role=Role.ASSISTANT, content="")
+    )
+    async for new_token in chat_model.astream_chat(
+        input_messages,
+        system,
+        tools,
+        do_sample=request.do_sample,
+        temperature=request.temperature,
+        top_p=request.top_p,
+        max_new_tokens=request.max_tokens,
+        stop=request.stop,
+    ):
+        if len(new_token) != 0:
+            yield _create_stream_chat_completion_chunk(
+                completion_id=completion_id, model=request.model, delta=ChatCompletionMessage(content=new_token)
             )
-            prompt_length = response.prompt_length
-            response_length += response.response_length
 
-        usage = ChatCompletionResponseUsage(
-            prompt_tokens=prompt_length,
-            completion_tokens=response_length,
-            total_tokens=prompt_length + response_length,
-        )
+    yield _create_stream_chat_completion_chunk(
+        completion_id=completion_id, model=request.model, delta=ChatCompletionMessage(), finish_reason=Finish.STOP
+    )
+    yield "[DONE]"
 
-        return ChatCompletionResponse(model=request.model, choices=choices, usage=usage)
 
-    async def stream_chat_completion(
-        messages: Sequence[Dict[str, str]], system: str, tools: str, request: ChatCompletionRequest
-    ):
-        choice_data = ChatCompletionResponseStreamChoice(
-            index=0, delta=ChatCompletionMessage(role=Role.ASSISTANT, content=""), finish_reason=None
-        )
-        chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data])
-        yield jsonify(chunk)
-
-        async for new_token in chat_model.astream_chat(
-            messages,
-            system,
-            tools,
-            do_sample=request.do_sample,
-            temperature=request.temperature,
-            top_p=request.top_p,
-            max_new_tokens=request.max_tokens,
-        ):
-            if len(new_token) == 0:
-                continue
-
-            choice_data = ChatCompletionResponseStreamChoice(
-                index=0, delta=ChatCompletionMessage(content=new_token), finish_reason=None
-            )
-            chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data])
-            yield jsonify(chunk)
+async def create_score_evaluation_response(
+    request: "ScoreEvaluationRequest", chat_model: "ChatModel"
+) -> "ScoreEvaluationResponse":
+    if len(request.messages) == 0:
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid request")
 
-        choice_data = ChatCompletionResponseStreamChoice(
-            index=0, delta=ChatCompletionMessage(), finish_reason=Finish.STOP
-        )
-        chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data])
-        yield jsonify(chunk)
-        yield "[DONE]"
-
-    @app.post("/v1/score/evaluation", response_model=ScoreEvaluationResponse, status_code=status.HTTP_200_OK)
-    async def create_score_evaluation(request: ScoreEvaluationRequest):
-        if chat_model.engine.can_generate:
-            raise HTTPException(status_code=status.HTTP_405_METHOD_NOT_ALLOWED, detail="Not allowed")
-
-        if len(request.messages) == 0:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid request")
-
-        scores = await chat_model.aget_scores(request.messages, max_length=request.max_length)
-        return ScoreEvaluationResponse(model=request.model, scores=scores)
-
-    return app
-
-
-if __name__ == "__main__":
-    chat_model = ChatModel()
-    app = create_app(chat_model)
-    uvicorn.run(app, host="0.0.0.0", port=int(os.environ.get("API_PORT", 8000)), workers=1)
+    scores = await chat_model.aget_scores(request.messages, max_length=request.max_length)
+    return ScoreEvaluationResponse(model=request.model, scores=scores)
```

### Comparing `llmtuner-0.7.0/src/llmtuner/api/protocol.py` & `llmtuner-0.7.1/src/llmtuner/api/protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from enum import Enum, unique
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field
 from typing_extensions import Literal
 
 
 @unique
 class Role(str, Enum):
@@ -47,15 +47,15 @@
 
 class FunctionAvailable(BaseModel):
     type: Literal["function", "code_interpreter"] = "function"
     function: Optional[FunctionDefinition] = None
 
 
 class FunctionCall(BaseModel):
-    id: Literal["call_default"] = "call_default"
+    id: str
     type: Literal["function"] = "function"
     function: Function
 
 
 class ChatMessage(BaseModel):
     role: Role
     content: Optional[str] = None
@@ -73,56 +73,57 @@
     messages: List[ChatMessage]
     tools: Optional[List[FunctionAvailable]] = None
     do_sample: bool = True
     temperature: Optional[float] = None
     top_p: Optional[float] = None
     n: int = 1
     max_tokens: Optional[int] = None
+    stop: Optional[Union[str, List[str]]] = None
     stream: bool = False
 
 
 class ChatCompletionResponseChoice(BaseModel):
     index: int
     message: ChatCompletionMessage
     finish_reason: Finish
 
 
-class ChatCompletionResponseStreamChoice(BaseModel):
+class ChatCompletionStreamResponseChoice(BaseModel):
     index: int
     delta: ChatCompletionMessage
     finish_reason: Optional[Finish] = None
 
 
 class ChatCompletionResponseUsage(BaseModel):
     prompt_tokens: int
     completion_tokens: int
     total_tokens: int
 
 
 class ChatCompletionResponse(BaseModel):
-    id: Literal["chatcmpl-default"] = "chatcmpl-default"
+    id: str
     object: Literal["chat.completion"] = "chat.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
     model: str
     choices: List[ChatCompletionResponseChoice]
     usage: ChatCompletionResponseUsage
 
 
 class ChatCompletionStreamResponse(BaseModel):
-    id: Literal["chatcmpl-default"] = "chatcmpl-default"
+    id: str
     object: Literal["chat.completion.chunk"] = "chat.completion.chunk"
     created: int = Field(default_factory=lambda: int(time.time()))
     model: str
-    choices: List[ChatCompletionResponseStreamChoice]
+    choices: List[ChatCompletionStreamResponseChoice]
 
 
 class ScoreEvaluationRequest(BaseModel):
     model: str
     messages: List[str]
     max_length: Optional[int] = None
 
 
 class ScoreEvaluationResponse(BaseModel):
-    id: Literal["scoreeval-default"] = "scoreeval-default"
+    id: str
     object: Literal["score.evaluation"] = "score.evaluation"
     model: str
     scores: List[float]
```

### Comparing `llmtuner-0.7.0/src/llmtuner/chat/base_engine.py` & `llmtuner-0.7.1/src/llmtuner/chat/base_engine.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/chat/hf_engine.py` & `llmtuner-0.7.1/src/llmtuner/chat/hf_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,39 +61,50 @@
         paired_messages = messages + [{"role": "assistant", "content": ""}]
         prompt_ids, _ = template.encode_oneturn(
             tokenizer=tokenizer, messages=paired_messages, system=system, tools=tools
         )
         prompt_length = len(prompt_ids)
         inputs = torch.tensor([prompt_ids], device=model.device)
 
-        do_sample = input_kwargs.pop("do_sample", None)
-        temperature = input_kwargs.pop("temperature", None)
-        top_p = input_kwargs.pop("top_p", None)
-        top_k = input_kwargs.pop("top_k", None)
-        num_return_sequences = input_kwargs.pop("num_return_sequences", None)
-        repetition_penalty = input_kwargs.pop("repetition_penalty", None)
+        do_sample = input_kwargs.pop("do_sample", generating_args["do_sample"])
+        temperature = input_kwargs.pop("temperature", generating_args["temperature"])
+        top_p = input_kwargs.pop("top_p", generating_args["top_p"])
+        top_k = input_kwargs.pop("top_k", generating_args["top_k"])
+        num_return_sequences = input_kwargs.pop("num_return_sequences", 1)
+        repetition_penalty = input_kwargs.pop("repetition_penalty", generating_args["repetition_penalty"])
+        length_penalty = input_kwargs.pop("length_penalty", generating_args["length_penalty"])
         max_length = input_kwargs.pop("max_length", None)
         max_new_tokens = input_kwargs.pop("max_new_tokens", None)
+        stop = input_kwargs.pop("stop", None)
 
+        if stop is not None:
+            raise ValueError("Stop parameter is not supported in Huggingface engine yet.")
+
+        generating_args = generating_args.copy()
         generating_args.update(
             dict(
-                do_sample=do_sample if do_sample is not None else generating_args["do_sample"],
-                temperature=temperature or generating_args["temperature"],
-                top_p=top_p or generating_args["top_p"],
-                top_k=top_k or generating_args["top_k"],
-                num_return_sequences=num_return_sequences or 1,
-                repetition_penalty=repetition_penalty or generating_args["repetition_penalty"],
+                do_sample=do_sample,
+                temperature=temperature,
+                top_p=top_p,
+                top_k=top_k,
+                num_return_sequences=num_return_sequences,
+                repetition_penalty=repetition_penalty,
+                length_penalty=length_penalty,
                 eos_token_id=[tokenizer.eos_token_id] + tokenizer.additional_special_tokens_ids,
                 pad_token_id=tokenizer.pad_token_id,
             )
         )
 
         if isinstance(num_return_sequences, int) and num_return_sequences > 1:
             generating_args["do_sample"] = True
 
+        if not generating_args["do_sample"]:
+            generating_args.pop("temperature", None)
+            generating_args.pop("top_p", None)
+
         if max_length:
             generating_args.pop("max_new_tokens", None)
             generating_args["max_length"] = max_length
 
         if max_new_tokens:
             generating_args.pop("max_length", None)
             generating_args["max_new_tokens"] = max_new_tokens
```

### Comparing `llmtuner-0.7.0/src/llmtuner/chat/vllm_engine.py` & `llmtuner-0.7.1/src/llmtuner/chat/vllm_engine.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import uuid
 from typing import TYPE_CHECKING, AsyncGenerator, AsyncIterator, Dict, List, Optional, Sequence
 
 from ..data import get_template_and_fix_tokenizer
+from ..extras.logging import get_logger
 from ..extras.misc import get_device_count, infer_optim_dtype
 from ..extras.packages import is_vllm_available
 from ..model import load_config, load_tokenizer
+from ..model.utils.visual import LlavaMultiModalProjectorForYiVLForVLLM
 from .base_engine import BaseEngine, Response
 
 
 if is_vllm_available():
     from vllm import AsyncEngineArgs, AsyncLLMEngine, RequestOutput, SamplingParams
     from vllm.lora.request import LoRARequest
     from vllm.sequence import MultiModalData
@@ -18,14 +20,17 @@
     import torch
     from numpy.typing import NDArray
     from transformers.image_processing_utils import BaseImageProcessor
 
     from ..hparams import DataArguments, FinetuningArguments, GeneratingArguments, ModelArguments
 
 
+logger = get_logger(__name__)
+
+
 class VllmEngine(BaseEngine):
     def __init__(
         self,
         model_args: "ModelArguments",
         data_args: "DataArguments",
         finetuning_args: "FinetuningArguments",
         generating_args: "GeneratingArguments",
@@ -53,21 +58,27 @@
             "disable_log_stats": True,
             "disable_log_requests": True,
             "enforce_eager": model_args.vllm_enforce_eager,
             "enable_lora": model_args.adapter_name_or_path is not None,
         }
 
         if model_args.visual_inputs:
-            # TODO: auto derive from config
-            # https://github.com/vllm-project/vllm/pull/3042#issuecomment-1984893549
-            self.image_feature_size = 576
+            image_size = config.vision_config.image_size
+            patch_size = config.vision_config.patch_size
+            self.image_feature_size = (image_size // patch_size) ** 2
             engine_args["image_input_type"] = "pixel_values"
             engine_args["image_token_id"] = self.tokenizer.convert_tokens_to_ids("<image>")
-            engine_args["image_input_shape"] = "1,3,336,336"
+            engine_args["image_input_shape"] = "1,3,{},{}".format(image_size, image_size)
             engine_args["image_feature_size"] = self.image_feature_size
+            if getattr(config, "is_yi_vl_derived_model", None):
+                # bug in vllm 0.4.2, see: https://github.com/vllm-project/vllm/pull/4828
+                import vllm.model_executor.models.llava
+
+                logger.info("Detected Yi-VL model, applying projector patch.")
+                vllm.model_executor.models.llava.LlavaMultiModalProjector = LlavaMultiModalProjectorForYiVLForVLLM
 
         self.model = AsyncLLMEngine.from_engine_args(AsyncEngineArgs(**engine_args))
         if model_args.adapter_name_or_path is not None:
             self.lora_request = LoRARequest("default", 1, model_args.adapter_name_or_path[0])
         else:
             self.lora_request = None
 
@@ -85,49 +96,43 @@
 
         paired_messages = messages + [{"role": "assistant", "content": ""}]
         prompt_ids, _ = self.template.encode_oneturn(
             tokenizer=self.tokenizer, messages=paired_messages, system=system, tools=tools
         )
         prompt_length = len(prompt_ids)
 
-        temperature = input_kwargs.pop("temperature", None)
-        top_p = input_kwargs.pop("top_p", None)
-        top_k = input_kwargs.pop("top_k", None)
-        num_return_sequences = input_kwargs.pop("num_return_sequences", None)
-        repetition_penalty = input_kwargs.pop("repetition_penalty", None)
+        use_beam_search = self.generating_args["num_beams"] > 1
+        temperature = input_kwargs.pop("temperature", self.generating_args["temperature"])
+        top_p = input_kwargs.pop("top_p", self.generating_args["top_p"])
+        top_k = input_kwargs.pop("top_k", self.generating_args["top_k"])
+        num_return_sequences = input_kwargs.pop("num_return_sequences", 1)
+        repetition_penalty = input_kwargs.pop("repetition_penalty", self.generating_args["repetition_penalty"])
+        length_penalty = input_kwargs.pop("length_penalty", self.generating_args["length_penalty"])
         max_length = input_kwargs.pop("max_length", None)
         max_new_tokens = input_kwargs.pop("max_new_tokens", None)
+        stop = input_kwargs.pop("stop", None)
 
-        generating_args = self.generating_args.copy()
-        generating_args.update(
-            dict(
-                temperature=temperature or generating_args["temperature"],
-                top_p=top_p or generating_args["top_p"],
-                top_k=top_k or generating_args["top_k"],
-                num_return_sequences=num_return_sequences or 1,
-                repetition_penalty=repetition_penalty or generating_args["repetition_penalty"],
-            )
-        )
-
+        max_tokens = self.generating_args["max_new_tokens"] or self.generating_args["max_length"]
         if max_length:
-            generating_args["max_new_tokens"] = max_length - prompt_length
+            max_tokens = max_length - prompt_length if max_length > prompt_length else 1
 
         if max_new_tokens:
-            generating_args["max_new_tokens"] = max_new_tokens
+            max_tokens = max_new_tokens
 
         sampling_params = SamplingParams(
-            n=generating_args["num_return_sequences"],
-            repetition_penalty=generating_args["repetition_penalty"],
-            temperature=generating_args["temperature"],
-            top_p=generating_args["top_p"],
-            top_k=generating_args["top_k"],
-            use_beam_search=generating_args["num_beams"] > 1,
-            length_penalty=generating_args["length_penalty"],
+            n=num_return_sequences,
+            repetition_penalty=repetition_penalty,
+            temperature=temperature,
+            top_p=top_p,
+            top_k=top_k,
+            use_beam_search=use_beam_search,
+            length_penalty=length_penalty,
+            stop=stop,
             stop_token_ids=[self.tokenizer.eos_token_id] + self.tokenizer.additional_special_tokens_ids,
-            max_tokens=generating_args["max_new_tokens"],
+            max_tokens=max_tokens,
             skip_special_tokens=True,
         )
 
         if self.processor is not None and image is not None:
             image_processor: "BaseImageProcessor" = getattr(self.processor, "image_processor")
             pixel_values: "torch.Tensor" = image_processor(image, return_tensors="pt")["pixel_values"]
             multi_modal_data = MultiModalData(type=MultiModalData.Type.IMAGE, data=pixel_values)
```

### Comparing `llmtuner-0.7.0/src/llmtuner/data/aligner.py` & `llmtuner-0.7.1/src/llmtuner/data/aligner.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/data/collator.py` & `llmtuner-0.7.1/src/llmtuner/data/collator.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/data/formatter.py` & `llmtuner-0.7.1/src/llmtuner/data/formatter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/data/loader.py` & `llmtuner-0.7.1/src/llmtuner/data/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..extras.constants import FILEEXT2TYPE
 from ..extras.logging import get_logger
 from ..extras.misc import has_tokenized_data
 from .aligner import align_dataset
 from .parser import get_dataset_list
 from .preprocess import get_preprocess_and_print_func
 from .template import get_template_and_fix_tokenizer
-from .utils import checksum, merge_dataset
+from .utils import merge_dataset
 
 
 if TYPE_CHECKING:
     from datasets import Dataset, IterableDataset
     from transformers import ProcessorMixin, Seq2SeqTrainingArguments
     from transformers.tokenization_utils import PreTrainedTokenizer
 
@@ -57,16 +57,14 @@
             data_files.append(local_path)
             data_path = FILEEXT2TYPE.get(local_path.split(".")[-1], None)
         else:
             raise ValueError("File not found.")
 
         if data_path is None:
             raise ValueError("File extension must be txt, csv, json or jsonl.")
-
-        checksum(data_files, dataset_attr.file_sha1)
     else:
         raise NotImplementedError
 
     if dataset_attr.load_from == "ms_hub":
         try:
             from modelscope import MsDataset
             from modelscope.utils.config_ds import MS_DATASETS_CACHE
```

### Comparing `llmtuner-0.7.0/src/llmtuner/data/parser.py` & `llmtuner-0.7.1/src/llmtuner/data/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,27 @@
     Dataset attributes.
     """
 
     """ basic configs """
     load_from: Literal["hf_hub", "ms_hub", "script", "file"]
     dataset_name: str
     """ extra configs """
-    file_sha1: Optional[str] = None
     subset: Optional[str] = None
     folder: Optional[str] = None
     ranking: bool = False
     formatting: Literal["alpaca", "sharegpt"] = "alpaca"
     """ columns """
     system: Optional[str] = None
     images: Optional[str] = None
     """ columns for the alpaca format """
     prompt: Optional[str] = "instruction"
     query: Optional[str] = "input"
     response: Optional[str] = "output"
+    chosen: Optional[str] = "chosen"
+    rejected: Optional[str] = "rejected"
     history: Optional[str] = None
     """ columns for the sharegpt format """
     messages: Optional[str] = "conversations"
     tools: Optional[str] = None
     """ tags for the sharegpt format """
     role_tag: Optional[str] = "from"
     content_tag: Optional[str] = "value"
@@ -95,15 +96,14 @@
             else:
                 dataset_attr = DatasetAttr("hf_hub", dataset_name=dataset_info[name]["hf_hub_url"])
         elif "script_url" in dataset_info[name]:
             dataset_attr = DatasetAttr("script", dataset_name=dataset_info[name]["script_url"])
         else:
             dataset_attr = DatasetAttr("file", dataset_name=dataset_info[name]["file_name"])
 
-        dataset_attr.set_attr("file_sha1", dataset_info[name])
         dataset_attr.set_attr("subset", dataset_info[name])
         dataset_attr.set_attr("folder", dataset_info[name])
         dataset_attr.set_attr("ranking", dataset_info[name], default=False)
         dataset_attr.set_attr("formatting", dataset_info[name], default="alpaca")
 
         if "columns" in dataset_info[name]:
             column_names = ["system", "images"]
```

### Comparing `llmtuner-0.7.0/src/llmtuner/data/preprocess.py` & `llmtuner-0.7.1/src/llmtuner/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/data/template.py` & `llmtuner-0.7.1/src/llmtuner/data/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
 def _get_jinja_template(template: "Template", tokenizer: "PreTrainedTokenizer") -> str:
     jinja_template = ""
 
     if template.default_system:
         jinja_template += "{% set system_message = '" + _jinja_escape(template.default_system) + "' %}"
 
     jinja_template += (
-        "{% if messages[0]['role'] == 'system' %}" "{% set system_message = messages[0]['content'] %}" "{% endif %}"
+        "{% if messages[0]['role'] == 'system' %}{% set system_message = messages[0]['content'] %}{% endif %}"
     )
 
     system_message = _convert_slots_to_jinja(template.format_system.apply(), tokenizer, placeholder="system_message")
     if isinstance(template, Llama2Template):
         pass
     elif template.force_system:
         jinja_template += "{{ " + system_message + " }}"
@@ -853,14 +853,30 @@
     format_separator=EmptyFormatter(slots=["\n"]),
     stop_words=["<|im_end|>"],
     replace_eos=True,
 )
 
 
 _register_template(
+    name="yi_vl",
+    format_user=StringFormatter(slots=["### Human: {{content}}\n### Assistant:"]),
+    format_separator=EmptyFormatter(slots=["\n"]),
+    default_system=(
+        "This is a chat between an inquisitive human and an AI assistant. "
+        "Assume the role of the AI assistant. Read all the images carefully, "
+        "and respond to the human's questions with informative, helpful, detailed and polite answers. "
+        "这是一个好奇的人类和一个人工智能助手之间的对话。假设你扮演这个AI助手的角色。"
+        "仔细阅读所有的图像，并对人类的问题做出信息丰富、有帮助、详细的和礼貌的回答。\n\n"
+    ),
+    stop_words=["###"],
+    efficient_eos=True,
+)
+
+
+_register_template(
     name="yuan",
     format_user=StringFormatter(slots=["{{content}}", {"token": "<sep>"}]),
     format_separator=EmptyFormatter(slots=["\n"]),
     stop_words=["<eod>"],
     replace_eos=True,
 )
```

### Comparing `llmtuner-0.7.0/src/llmtuner/data/utils.py` & `llmtuner-0.7.1/src/llmtuner/data/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import hashlib
 from enum import Enum, unique
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Dict, List, Tuple, Union
 
 from datasets import concatenate_datasets, interleave_datasets
 
 from ..extras.logging import get_logger
 
 
 if TYPE_CHECKING:
@@ -22,29 +21,14 @@
     USER = "user"
     ASSISTANT = "assistant"
     SYSTEM = "system"
     FUNCTION = "function"
     OBSERVATION = "observation"
 
 
-def checksum(data_files: List[str], file_sha1: Optional[str] = None) -> None:
-    if file_sha1 is None:
-        logger.warning("Checksum failed: missing SHA-1 hash value in dataset_info.json.")
-        return
-
-    if len(data_files) != 1:
-        logger.warning("Checksum failed: too many files.")
-        return
-
-    with open(data_files[0], "rb") as f:
-        sha1 = hashlib.sha1(f.read()).hexdigest()
-        if sha1 != file_sha1:
-            logger.warning("Checksum failed: mismatched SHA-1 hash value at {}.".format(data_files[0]))
-
-
 def infer_max_len(source_len: int, target_len: int, max_len: int, reserved_label_len: int) -> Tuple[int, int]:
     max_target_len = int(max_len * (target_len / (source_len + target_len)))
     max_target_len = max(max_target_len, reserved_label_len)
     max_source_len = max_len - min(max_target_len, target_len)
     return max_source_len, max_target_len
```

### Comparing `llmtuner-0.7.0/src/llmtuner/eval/evaluator.py` & `llmtuner-0.7.1/src/llmtuner/eval/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,10 +114,9 @@
             with open(os.path.join(self.eval_args.save_dir, "results.json"), "w", encoding="utf-8", newline="\n") as f:
                 json.dump(results, f, indent=2)
 
             with open(os.path.join(self.eval_args.save_dir, "results.log"), "w", encoding="utf-8", newline="\n") as f:
                 f.write(score_info)
 
 
-if __name__ == "__main__":
-    evaluator = Evaluator()
-    evaluator.eval()
+def run_eval() -> None:
+    Evaluator().eval()
```

### Comparing `llmtuner-0.7.0/src/llmtuner/eval/template.py` & `llmtuner-0.7.1/src/llmtuner/eval/template.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/extras/constants.py` & `llmtuner-0.7.1/src/llmtuner/extras/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,30 @@
     "txt": "text",
 }
 
 IGNORE_INDEX = -100
 
 LAYERNORM_NAMES = {"norm", "ln"}
 
-LOG_FILE_NAME = "trainer_log.jsonl"
-
 METHODS = ["full", "freeze", "lora"]
 
-MLLM_LIST = ["LLaVA1.5"]
-
 MOD_SUPPORTED_MODELS = ["bloom", "falcon", "gemma", "llama", "mistral", "mixtral", "phi", "starcoder2"]
 
 PEFT_METHODS = ["lora"]
 
+RUNNING_LOG = "running_log.txt"
+
 SUBJECTS = ["Average", "STEM", "Social Sciences", "Humanities", "Other"]
 
 SUPPORTED_MODELS = OrderedDict()
 
+TRAINER_CONFIG = "trainer_config.yaml"
+
+TRAINER_LOG = "trainer_log.jsonl"
+
 TRAINING_STAGES = {
     "Supervised Fine-Tuning": "sft",
     "Reward Modeling": "rm",
     "PPO": "ppo",
     "DPO": "dpo",
     "ORPO": "orpo",
     "Pre-Training": "pt",
@@ -51,36 +53,41 @@
 
 SUPPORTED_CLASS_FOR_S2ATTN = ["llama"]
 
 V_HEAD_WEIGHTS_NAME = "value_head.bin"
 
 V_HEAD_SAFE_WEIGHTS_NAME = "value_head.safetensors"
 
+VISION_MODELS = set()
+
 
 class DownloadSource(str, Enum):
     DEFAULT = "hf"
     MODELSCOPE = "ms"
 
 
 def register_model_group(
     models: Dict[str, Dict[DownloadSource, str]],
     module: Optional[str] = None,
     template: Optional[str] = None,
+    vision: bool = False,
 ) -> None:
     prefix = None
     for name, path in models.items():
         if prefix is None:
             prefix = name.split("-")[0]
         else:
             assert prefix == name.split("-")[0], "prefix should be identical."
         SUPPORTED_MODELS[name] = path
     if module is not None:
         DEFAULT_MODULE[prefix] = module
     if template is not None:
         DEFAULT_TEMPLATE[prefix] = template
+    if vision:
+        VISION_MODELS.add(prefix)
 
 
 register_model_group(
     models={
         "Baichuan-7B-Base": {
             DownloadSource.DEFAULT: "baichuan-inc/Baichuan-7B",
             DownloadSource.MODELSCOPE: "baichuan-inc/baichuan-7B",
@@ -312,18 +319,26 @@
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-math-7b-instruct",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-math-7b-instruct",
         },
         "DeepSeek-MoE-16B-Base": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-moe-16b-base",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-moe-16b-base",
         },
+        "DeepSeek-MoE-236B-Base": {
+            DownloadSource.DEFAULT: "deepseek-ai/DeepSeek-V2",
+            DownloadSource.MODELSCOPE: "deepseek-ai/DeepSeek-V2",
+        },
         "DeepSeek-MoE-16B-Chat": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-moe-16b-chat",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-moe-16b-chat",
         },
+        "DeepSeek-MoE-236B-Chat": {
+            DownloadSource.DEFAULT: "deepseek-ai/DeepSeek-V2-Chat",
+            DownloadSource.MODELSCOPE: "deepseek-ai/DeepSeek-V2-Chat",
+        },
     },
     template="deepseek",
 )
 
 
 register_model_group(
     models={
@@ -408,21 +423,21 @@
     template="gemma",
 )
 
 
 register_model_group(
     models={
         "CodeGemma-2B": {
-            DownloadSource.DEFAULT: "google/codegemma-2b",
+            DownloadSource.DEFAULT: "google/codegemma-1.1-2b",
         },
         "CodeGemma-7B": {
             DownloadSource.DEFAULT: "google/codegemma-7b",
         },
         "CodeGemma-7B-Chat": {
-            DownloadSource.DEFAULT: "google/codegemma-7b-it",
+            DownloadSource.DEFAULT: "google/codegemma-1.1-7b-it",
             DownloadSource.MODELSCOPE: "AI-ModelScope/codegemma-7b-it",
         },
     },
     template="gemma",
 )
 
 
@@ -561,14 +576,21 @@
             DownloadSource.DEFAULT: "meta-llama/Meta-Llama-3-8B-Instruct",
             DownloadSource.MODELSCOPE: "LLM-Research/Meta-Llama-3-8B-Instruct",
         },
         "LLaMA3-70B-Chat": {
             DownloadSource.DEFAULT: "meta-llama/Meta-Llama-3-70B-Instruct",
             DownloadSource.MODELSCOPE: "LLM-Research/Meta-Llama-3-70B-Instruct",
         },
+        "LLaMA3-8B-Chinese-Chat": {
+            DownloadSource.DEFAULT: "shenzhi-wang/Llama3-8B-Chinese-Chat",
+            DownloadSource.MODELSCOPE: "LLM-Research/Llama3-8B-Chinese-Chat",
+        },
+        "LLaMA3-70B-Chinese-Chat": {
+            DownloadSource.DEFAULT: "shenzhi-wang/Llama3-70B-Chinese-Chat",
+        },
     },
     template="llama3",
 )
 
 
 register_model_group(
     models={
@@ -576,14 +598,15 @@
             DownloadSource.DEFAULT: "llava-hf/llava-1.5-7b-hf",
         },
         "LLaVA1.5-13B-Chat": {
             DownloadSource.DEFAULT: "llava-hf/llava-1.5-13b-hf",
         },
     },
     template="vicuna",
+    vision=True,
 )
 
 
 register_model_group(
     models={
         "Mistral-7B-v0.1": {
             DownloadSource.DEFAULT: "mistralai/Mistral-7B-v0.1",
@@ -695,19 +718,19 @@
 )
 
 
 register_model_group(
     models={
         "Phi3-3.8B-4k-Chat": {
             DownloadSource.DEFAULT: "microsoft/Phi-3-mini-4k-instruct",
-            DownloadSource.DEFAULT: "LLM-Research/Phi-3-mini-4k-instruct",
+            DownloadSource.MODELSCOPE: "LLM-Research/Phi-3-mini-4k-instruct",
         },
         "Phi3-3.8B-128k-Chat": {
             DownloadSource.DEFAULT: "microsoft/Phi-3-mini-128k-instruct",
-            DownloadSource.DEFAULT: "LLM-Research/Phi-3-mini-128k-instruct",
+            DownloadSource.MODELSCOPE: "LLM-Research/Phi-3-mini-128k-instruct",
         },
     },
     module="qkv_proj",
     template="phi",
 )
 
 
@@ -1154,21 +1177,59 @@
             DownloadSource.DEFAULT: "01-ai/Yi-34B-Chat-8bits",
             DownloadSource.MODELSCOPE: "01ai/Yi-34B-Chat-8bits",
         },
         "Yi-34B-int4-Chat": {
             DownloadSource.DEFAULT: "01-ai/Yi-34B-Chat-4bits",
             DownloadSource.MODELSCOPE: "01ai/Yi-34B-Chat-4bits",
         },
+        "Yi-1.5-6B": {
+            DownloadSource.DEFAULT: "01-ai/Yi-1.5-6B",
+            DownloadSource.MODELSCOPE: "01ai/Yi-1.5-6B",
+        },
+        "Yi-1.5-9B": {
+            DownloadSource.DEFAULT: "01-ai/Yi-1.5-9B",
+            DownloadSource.MODELSCOPE: "01ai/Yi-1.5-9B",
+        },
+        "Yi-1.5-34B": {
+            DownloadSource.DEFAULT: "01-ai/Yi-1.5-34B",
+            DownloadSource.MODELSCOPE: "01ai/Yi-1.5-34B",
+        },
+        "Yi-1.5-6B-Chat": {
+            DownloadSource.DEFAULT: "01-ai/Yi-1.5-6B-Chat",
+            DownloadSource.MODELSCOPE: "01ai/Yi-1.5-6B-Chat",
+        },
+        "Yi-1.5-9B-Chat": {
+            DownloadSource.DEFAULT: "01-ai/Yi-1.5-9B-Chat",
+            DownloadSource.MODELSCOPE: "01ai/Yi-1.5-9B-Chat",
+        },
+        "Yi-1.5-34B-Chat": {
+            DownloadSource.DEFAULT: "01-ai/Yi-1.5-34B-Chat",
+            DownloadSource.MODELSCOPE: "01ai/Yi-1.5-34B-Chat",
+        },
     },
     template="yi",
 )
 
 
 register_model_group(
     models={
+        "YiVL-6B-Chat": {
+            DownloadSource.DEFAULT: "BUAADreamer/Yi-VL-6B-hf",
+        },
+        "YiVL-34B-Chat": {
+            DownloadSource.DEFAULT: "BUAADreamer/Yi-VL-34B-hf",
+        },
+    },
+    template="yi_vl",
+    vision=True,
+)
+
+
+register_model_group(
+    models={
         "Yuan2-2B-Chat": {
             DownloadSource.DEFAULT: "IEITYuan/Yuan2-2B-hf",
             DownloadSource.MODELSCOPE: "YuanLLM/Yuan2.0-2B-hf",
         },
         "Yuan2-51B-Chat": {
             DownloadSource.DEFAULT: "IEITYuan/Yuan2-51B-hf",
             DownloadSource.MODELSCOPE: "YuanLLM/Yuan2.0-51B-hf",
```

### Comparing `llmtuner-0.7.0/src/llmtuner/extras/misc.py` & `llmtuner-0.7.1/src/llmtuner/extras/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.val = val
         self.sum += val * n
         self.count += n
         self.avg = self.sum / self.count
 
 
 def check_dependencies() -> None:
-    if int(os.environ.get("DISABLE_VERSION_CHECK", "0")):
+    if os.environ.get("DISABLE_VERSION_CHECK", "0").lower() in ["true", "1"]:
         logger.warning("Version checking has been disabled, may lead to unexpected behaviors.")
     else:
         require_version("transformers>=4.37.2", "To fix: pip install transformers>=4.37.2")
         require_version("datasets>=2.14.3", "To fix: pip install datasets>=2.14.3")
         require_version("accelerate>=0.27.2", "To fix: pip install accelerate>=0.27.2")
         require_version("peft>=0.10.0", "To fix: pip install peft>=0.10.0")
         require_version("trl>=0.8.1", "To fix: pip install trl>=0.8.1")
```

### Comparing `llmtuner-0.7.0/src/llmtuner/extras/packages.py` & `llmtuner-0.7.1/src/llmtuner/extras/packages.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def _get_package_version(name: str) -> "Version":
     try:
         return version.parse(importlib.metadata.version(name))
     except Exception:
         return version.parse("0.0.0")
 
 
-def is_fastapi_availble():
+def is_fastapi_available():
     return _is_package_available("fastapi")
 
 
 def is_flash_attn2_available():
     return _is_package_available("flash_attn") and _get_package_version("flash_attn") > version.parse("2.0.0")
```

### Comparing `llmtuner-0.7.0/src/llmtuner/hparams/data_args.py` & `llmtuner-0.7.1/src/llmtuner/hparams/data_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/hparams/evaluation_args.py` & `llmtuner-0.7.1/src/llmtuner/hparams/evaluation_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.7.1/src/llmtuner/hparams/finetuning_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,68 @@
-import json
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 from typing import Literal, Optional
 
 
 @dataclass
 class FreezeArguments:
     r"""
     Arguments pertaining to the freeze (partial-parameter) training.
     """
 
-    name_module_trainable: str = field(
+    freeze_trainable_layers: int = field(
+        default=2,
+        metadata={
+            "help": (
+                "The number of trainable layers for freeze (partial-parameter) fine-tuning. "
+                "Positive numbers mean the last n layers are set as trainable, "
+                "negative numbers mean the first n layers are set as trainable."
+            )
+        },
+    )
+    freeze_trainable_modules: str = field(
         default="all",
         metadata={
-            "help": """Name of trainable modules for partial-parameter (freeze) fine-tuning. \
-                    Use commas to separate multiple modules. \
-                    Use "all" to specify all the available modules. \
-                    LLaMA choices: ["mlp", "self_attn"], \
-                    BLOOM & Falcon & ChatGLM choices: ["mlp", "self_attention"], \
-                    Qwen choices: ["mlp", "attn"], \
-                    InternLM2 choices: ["feed_forward", "attention"], \
-                    Others choices: the same as LLaMA."""
+            "help": (
+                "Name(s) of trainable modules for freeze (partial-parameter) fine-tuning. "
+                "Use commas to separate multiple modules. "
+                "Use `all` to specify all the available modules. "
+                "LLaMA choices: [`mlp`, `self_attn`], "
+                "BLOOM & Falcon & ChatGLM choices: [`mlp`, `self_attention`], "
+                "Qwen choices: [`mlp`, `attn`], "
+                "InternLM2 choices: [`feed_forward`, `attention`], "
+                "Others choices: the same as LLaMA."
+            )
         },
     )
-    num_layer_trainable: int = field(
-        default=2,
-        metadata={"help": "The number of trainable layers for partial-parameter (freeze) fine-tuning."},
+    freeze_extra_modules: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": (
+                "Name(s) of modules apart from hidden layers to be set as trainable "
+                "for freeze (partial-parameter) fine-tuning. "
+                "Use commas to separate multiple modules."
+            )
+        },
     )
 
 
 @dataclass
 class LoraArguments:
     r"""
     Arguments pertaining to the LoRA training.
     """
 
     additional_target: Optional[str] = field(
         default=None,
         metadata={
-            "help": "Name(s) of modules apart from LoRA layers to be set as trainable and saved in the final checkpoint."
+            "help": (
+                "Name(s) of modules apart from LoRA layers to be set as trainable "
+                "and saved in the final checkpoint. "
+                "Use commas to separate multiple modules."
+            )
         },
     )
     lora_alpha: Optional[int] = field(
         default=None,
         metadata={"help": "The scale factor for LoRA fine-tuning (default: lora_rank * 2)."},
     )
     lora_dropout: float = field(
@@ -51,23 +72,25 @@
     lora_rank: int = field(
         default=8,
         metadata={"help": "The intrinsic dimension for LoRA fine-tuning."},
     )
     lora_target: str = field(
         default="all",
         metadata={
-            "help": """Name(s) of target modules to apply LoRA. \
-                    Use commas to separate multiple modules. \
-                    Use "all" to specify all the linear modules. \
-                    LLaMA choices: ["q_proj", "k_proj", "v_proj", "o_proj", "gate_proj", "up_proj", "down_proj"], \
-                    BLOOM & Falcon & ChatGLM choices: ["query_key_value", "dense", "dense_h_to_4h", "dense_4h_to_h"], \
-                    Baichuan choices: ["W_pack", "o_proj", "gate_proj", "up_proj", "down_proj"], \
-                    Qwen choices: ["c_attn", "attn.c_proj", "w1", "w2", "mlp.c_proj"], \
-                    InternLM2 choices: ["wqkv", "wo", "w1", "w2", "w3"], \
-                    Others choices: the same as LLaMA."""
+            "help": (
+                "Name(s) of target modules to apply LoRA. "
+                "Use commas to separate multiple modules. "
+                "Use `all` to specify all the linear modules. "
+                "LLaMA choices: [`q_proj`, `k_proj`, `v_proj`, `o_proj`, `gate_proj`, `up_proj`, `down_proj`], "
+                "BLOOM & Falcon & ChatGLM choices: [`query_key_value`, `dense`, `dense_h_to_4h`, `dense_4h_to_h`], "
+                "Baichuan choices: [`W_pack`, `o_proj`, `gate_proj`, `up_proj`, `down_proj`], "
+                "Qwen choices: [`c_attn`, `attn.c_proj`, `w1`, `w2`, `mlp.c_proj`], "
+                "InternLM2 choices: [`wqkv`, `wo`, `w1`, `w2`, `w3`], "
+                "Others choices: the same as LLaMA."
+            )
         },
     )
     loraplus_lr_ratio: Optional[float] = field(
         default=None,
         metadata={"help": "LoRA plus learning rate ratio (lr_B / lr_A)."},
     )
     loraplus_lr_embedding: float = field(
@@ -173,16 +196,18 @@
     use_galore: bool = field(
         default=False,
         metadata={"help": "Whether or not to use the gradient low-Rank projection (GaLore)."},
     )
     galore_target: str = field(
         default="all",
         metadata={
-            "help": """Name(s) of modules to apply GaLore. Use commas to separate multiple modules. \
-                    Use "all" to specify all the linear modules."""
+            "help": (
+                "Name(s) of modules to apply GaLore. Use commas to separate multiple modules. "
+                "Use `all` to specify all the linear modules."
+            )
         },
     )
     galore_rank: int = field(
         default=16,
         metadata={"help": "The rank of GaLore gradients."},
     )
     galore_update_interval: int = field(
@@ -217,39 +242,45 @@
         default="layer",
         metadata={"help": "Whether to use layer-wise or ratio-wise BAdam optimizer."},
     )
     badam_start_block: Optional[int] = field(
         default=None,
         metadata={"help": "The starting block index for layer-wise BAdam."},
     )
-    badam_switch_block_every: Optional[int] = field(
-        default=50,
-        metadata={"help": "How often to switch model's block update. Set to -1 to disable the block update."},
-    )
     badam_switch_mode: Optional[Literal["ascending", "descending", "random", "fixed"]] = field(
         default="ascending",
         metadata={"help": "the strategy of picking block to update for layer-wise BAdam."},
     )
+    badam_switch_interval: Optional[int] = field(
+        default=50,
+        metadata={
+            "help": "Number of steps to update the block for layer-wise BAdam. Use -1 to disable the block update."
+        },
+    )
     badam_update_ratio: float = field(
-        default=0.0,
+        default=0.05,
         metadata={"help": "The ratio of the update for ratio-wise BAdam."},
     )
     badam_mask_mode: Literal["adjacent", "scatter"] = field(
         default="adjacent",
         metadata={
-            "help": """The mode of the mask for BAdam optimizer. \
-                    `adjacent` means that the trainable parameters are adjacent to each other, \
-                    `scatter` means that trainable parameters are randomly choosed from the weight."""
+            "help": (
+                "The mode of the mask for BAdam optimizer. "
+                "`adjacent` means that the trainable parameters are adjacent to each other, "
+                "`scatter` means that trainable parameters are randomly choosed from the weight."
+            )
         },
     )
     badam_verbose: int = field(
         default=0,
         metadata={
-            "help": """The verbosity level of BAdam optimizer. \
-                    0 for no print, 1 for print the block prefix, 2 for print trainable parameters"""
+            "help": (
+                "The verbosity level of BAdam optimizer. "
+                "0 for no print, 1 for print the block prefix, 2 for print trainable parameters."
+            )
         },
     )
 
 
 @dataclass
 class FinetuningArguments(FreezeArguments, LoraArguments, RLHFArguments, GaloreArguments, BAdamArgument):
     r"""
@@ -279,15 +310,16 @@
 
     def __post_init__(self):
         def split_arg(arg):
             if isinstance(arg, str):
                 return [item.strip() for item in arg.split(",")]
             return arg
 
-        self.name_module_trainable = split_arg(self.name_module_trainable)
+        self.freeze_trainable_modules = split_arg(self.freeze_trainable_modules)
+        self.freeze_extra_modules = split_arg(self.freeze_extra_modules)
         self.lora_alpha = self.lora_alpha or self.lora_rank * 2
         self.lora_target = split_arg(self.lora_target)
         self.additional_target = split_arg(self.additional_target)
         self.galore_target = split_arg(self.galore_target)
 
         assert self.finetuning_type in ["lora", "freeze", "full"], "Invalid fine-tuning method."
         assert self.ref_model_quantization_bit in [None, 8, 4], "We only accept 4-bit or 8-bit quantization."
@@ -304,23 +336,12 @@
 
         if self.use_llama_pro and self.finetuning_type == "full":
             raise ValueError("`use_llama_pro` is only valid for the Freeze or LoRA training.")
 
         if self.use_galore and self.finetuning_type == "lora":
             raise ValueError("Cannot use LoRA with GaLore together.")
 
+        if self.use_galore and self.use_badam:
+            raise ValueError("Cannot use GaLore with BAdam together.")
+
         if self.loraplus_lr_ratio is not None and self.finetuning_type != "lora":
             raise ValueError("`loraplus_lr_ratio` is only valid for the LoRA training.")
-
-    def save_to_json(self, json_path: str):
-        r"""Saves the content of this instance in JSON format inside `json_path`."""
-        json_string = json.dumps(asdict(self), indent=2, sort_keys=True) + "\n"
-        with open(json_path, "w", encoding="utf-8") as f:
-            f.write(json_string)
-
-    @classmethod
-    def load_from_json(cls, json_path: str):
-        r"""Creates an instance from the content of `json_path`."""
-        with open(json_path, "r", encoding="utf-8") as f:
-            text = f.read()
-
-        return cls(**json.loads(text))
```

### Comparing `llmtuner-0.7.0/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.7.1/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/hparams/model_args.py` & `llmtuner-0.7.1/src/llmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/hparams/parser.py` & `llmtuner-0.7.1/src/llmtuner/hparams/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import torch
 import transformers
 from transformers import HfArgumentParser, Seq2SeqTrainingArguments
 from transformers.trainer_utils import get_last_checkpoint
 from transformers.utils import is_torch_bf16_gpu_available
 from transformers.utils.versions import require_version
 
+from ..extras.constants import TRAINER_CONFIG
 from ..extras.logging import get_logger
 from ..extras.misc import check_dependencies, get_current_device
 from .data_args import DataArguments
 from .evaluation_args import EvaluationArguments
 from .finetuning_args import FinetuningArguments
 from .generating_args import GeneratingArguments
 from .model_args import ModelArguments
@@ -247,15 +248,16 @@
         training_args.resume_from_checkpoint is None
         and training_args.do_train
         and os.path.isdir(training_args.output_dir)
         and not training_args.overwrite_output_dir
         and can_resume_from_checkpoint
     ):
         last_checkpoint = get_last_checkpoint(training_args.output_dir)
-        if last_checkpoint is None and len(os.listdir(training_args.output_dir)) > 0:
+        files = os.listdir(training_args.output_dir)
+        if last_checkpoint is None and len(files) > 0 and (len(files) != 1 or files[0] != TRAINER_CONFIG):
             raise ValueError("Output directory already exists and is not empty. Please set `overwrite_output_dir`.")
 
         if last_checkpoint is not None:
             training_args.resume_from_checkpoint = last_checkpoint
             logger.info(
                 "Resuming training from {}. Change `output_dir` or use `overwrite_output_dir` to avoid.".format(
                     training_args.resume_from_checkpoint
@@ -279,15 +281,15 @@
     elif training_args.fp16:
         model_args.compute_dtype = torch.float16
 
     model_args.device_map = {"": get_current_device()}
     model_args.model_max_length = data_args.cutoff_len
     data_args.packing = data_args.packing if data_args.packing is not None else finetuning_args.stage == "pt"
 
-    # Log on each process the small summary:
+    # Log on each process the small summary
     logger.info(
         "Process rank: {}, device: {}, n_gpu: {}, distributed training: {}, compute dtype: {}".format(
             training_args.local_rank,
             training_args.device,
             training_args.n_gpu,
             training_args.parallel_mode.value == "distributed",
             str(model_args.compute_dtype),
```

### Comparing `llmtuner-0.7.0/src/llmtuner/model/adapter.py` & `llmtuner-0.7.1/src/llmtuner/model/adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import re
 from typing import TYPE_CHECKING
 
 import torch
 from peft import LoraConfig, LoraModel, PeftModel, TaskType, get_peft_model
-from transformers.integrations import is_deepspeed_zero3_enabled
+from transformers.integrations import deepspeed_config, is_deepspeed_zero3_enabled
+from transformers.modeling_utils import is_fsdp_enabled
 
 from ..extras.logging import get_logger
 from .utils.misc import find_all_linear_modules, find_expanded_modules
 from .utils.quantization import QuantizationMethod
 from .utils.unsloth import get_unsloth_peft_model, load_unsloth_peft_model
 
 
@@ -37,64 +39,89 @@
     if (not is_trainable) and model_args.adapter_name_or_path is None:
         logger.info("Adapter is not found at evaluation, load the base model.")
         return model
 
     if finetuning_args.finetuning_type != "lora" and getattr(model, "quantization_method", None):
         raise ValueError("You can only use lora for quantized models.")
 
+    if deepspeed_config() is not None or is_fsdp_enabled() or finetuning_args.pure_bf16 or finetuning_args.use_badam:
+        logger.info("DeepSpeed/FSDP/PureBF16/BAdam detected, remaining trainable params in half precision.")
+        cast_trainable_params_to_fp32 = False
+    else:
+        logger.info("Upcasting trainable params to float32.")
+        cast_trainable_params_to_fp32 = True
+
     if finetuning_args.finetuning_type == "full" and is_trainable:
         logger.info("Fine-tuning method: Full")
-        if (not finetuning_args.pure_bf16) and (not finetuning_args.use_badam):
+        if cast_trainable_params_to_fp32:
             model = model.float()
 
+        if model_args.visual_inputs and hasattr(model, "vision_tower"):  # freeze vision model
+            model.vision_tower.requires_grad_(False)
+
     if finetuning_args.finetuning_type == "freeze" and is_trainable:
         logger.info("Fine-tuning method: Freeze")
         num_layers = (
             getattr(model.config, "num_hidden_layers", None)
             or getattr(model.config, "num_layers", None)
             or getattr(model.config, "n_layer", None)
         )
         if not num_layers:
             raise ValueError("Current model does not support freeze tuning.")
 
         if finetuning_args.use_llama_pro:
-            if num_layers % finetuning_args.num_layer_trainable != 0:
+            if num_layers % finetuning_args.freeze_trainable_layers != 0:
                 raise ValueError(
                     "`num_layers` {} should be divisible by `num_layer_trainable` {}.".format(
-                        num_layers, finetuning_args.num_layer_trainable
+                        num_layers, finetuning_args.freeze_trainable_layers
                     )
                 )
 
-            stride = num_layers // finetuning_args.num_layer_trainable
+            stride = num_layers // finetuning_args.freeze_trainable_layers
             trainable_layer_ids = range(stride - 1, num_layers + stride - 1, stride)
-        elif finetuning_args.num_layer_trainable > 0:  # fine-tuning the last n layers if num_layer_trainable > 0
-            trainable_layer_ids = range(num_layers - finetuning_args.num_layer_trainable, num_layers)
+        elif finetuning_args.freeze_trainable_layers > 0:  # fine-tuning the last n layers if num_layer_trainable > 0
+            trainable_layer_ids = range(max(0, num_layers - finetuning_args.freeze_trainable_layers), num_layers)
         else:  # fine-tuning the first n layers if num_layer_trainable < 0
-            trainable_layer_ids = range(-finetuning_args.num_layer_trainable)
+            trainable_layer_ids = range(min(-finetuning_args.freeze_trainable_layers, num_layers))
 
-        freeze_modules = {"all"}
-        for name, _ in model.named_modules():
+        hidden_modules = set()
+        non_hidden_modules = set()
+        for name, _ in model.named_parameters():
             if ".0." in name:
-                freeze_modules.add(name.split(".0.")[-1].split(".")[0])
+                hidden_modules.add(name.split(".0.")[-1].split(".")[0])
             elif ".1." in name:  # MoD starts from layer 1
-                freeze_modules.add(name.split(".1.")[-1].split(".")[0])
+                hidden_modules.add(name.split(".1.")[-1].split(".")[0])
+
+            if re.search(r"\.\d+\.", name) is None:
+                non_hidden_modules.add(name.split(".")[-2])
 
         trainable_layers = []
-        for module_name in finetuning_args.name_module_trainable:
-            if module_name not in freeze_modules:
+        for module_name in finetuning_args.freeze_trainable_modules:
+            if module_name != "all" and module_name not in hidden_modules:
                 raise ValueError(
-                    "Module {} is not found, please choose from {}".format(module_name, ", ".join(freeze_modules))
+                    "Module {} is not found, please choose from {}".format(module_name, ", ".join(hidden_modules))
                 )
 
             for idx in trainable_layer_ids:
                 trainable_layers.append(".{:d}.{}".format(idx, module_name if module_name != "all" else ""))
 
+        if finetuning_args.freeze_extra_modules:
+            for module_name in finetuning_args.freeze_extra_modules:
+                if module_name not in non_hidden_modules:
+                    raise ValueError(
+                        "Module {} is not found, please choose from {}".format(
+                            module_name, ", ".join(non_hidden_modules)
+                        )
+                    )
+
+                trainable_layers.append(module_name)
+
         for name, param in model.named_parameters():
             if any(trainable_layer in name for trainable_layer in trainable_layers):
-                if (not finetuning_args.pure_bf16) and (not finetuning_args.use_badam):
+                if cast_trainable_params_to_fp32:
                     param.data = param.data.to(torch.float32)
             else:
                 param.requires_grad_(False)
 
         logger.info("Set trainable layers: {}".format(",".join(map(str, trainable_layer_ids))))
 
     if finetuning_args.finetuning_type == "lora":
@@ -184,15 +211,15 @@
                     task_type=TaskType.CAUSAL_LM,
                     inference_mode=False,
                     use_dora=finetuning_args.use_dora,
                     **peft_kwargs,
                 )
                 model = get_peft_model(model, lora_config)
 
-        if (not finetuning_args.pure_bf16) and (not finetuning_args.use_badam):
+        if cast_trainable_params_to_fp32:
             for param in filter(lambda p: p.requires_grad, model.parameters()):
                 param.data = param.data.to(torch.float32)
 
         if model_args.adapter_name_or_path is not None:
             logger.info("Loaded adapter(s): {}".format(",".join(model_args.adapter_name_or_path)))
 
     return model
```

### Comparing `llmtuner-0.7.0/src/llmtuner/model/loader.py` & `llmtuner-0.7.1/src/llmtuner/model/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,16 +74,23 @@
         if num_added_tokens > 0 and not model_args.resize_vocab:
             model_args.resize_vocab = True
             logger.warning("New tokens have been added, changed `resize_vocab` to True.")
 
     patch_tokenizer(tokenizer)
 
     if model_args.visual_inputs:
-        processor = AutoProcessor.from_pretrained(model_args.model_name_or_path, **init_kwargs)
-        setattr(processor, "tokenizer", tokenizer)
+        try:
+            processor = AutoProcessor.from_pretrained(model_args.model_name_or_path, **init_kwargs)
+            setattr(processor, "tokenizer", tokenizer)
+        except Exception:
+            raise ValueError(
+                "This multimodal LLM is not supported.\n"
+                "Download LLaVA-1.5 models from: https://huggingface.co/llava-hf\n"
+                "Download Yi-VL models from: https://huggingface.co/BUAADreamer"
+            )
     else:
         processor = None
 
     return {"tokenizer": tokenizer, "processor": processor}
 
 
 def load_config(model_args: "ModelArguments") -> "PretrainedConfig":
@@ -102,15 +109,15 @@
     add_valuehead: bool = False,
 ) -> "PreTrainedModel":
     r"""
     Loads pretrained model.
     """
     init_kwargs = _get_init_kwargs(model_args)
     config = load_config(model_args)
-    patch_config(config, tokenizer, model_args, init_kwargs, is_trainable, add_valuehead)
+    patch_config(config, tokenizer, model_args, init_kwargs, is_trainable)
 
     model = None
     lazy_load = False
     if model_args.use_unsloth:
         if model_args.adapter_name_or_path is not None:
             lazy_load = True
         elif is_trainable:
```

### Comparing `llmtuner-0.7.0/src/llmtuner/model/patcher.py` & `llmtuner-0.7.1/src/llmtuner/model/patcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+import os
 from types import MethodType
 from typing import TYPE_CHECKING, Any, Dict
 
 import torch
 from peft import PeftModel
-from transformers import PreTrainedModel, PreTrainedTokenizerBase
+from transformers import PreTrainedModel, PreTrainedTokenizerBase, is_torch_npu_available
 from transformers.integrations import is_deepspeed_zero3_enabled
+from transformers.modeling_utils import is_fsdp_enabled
 
 from ..extras.logging import get_logger
 from ..extras.misc import infer_optim_dtype
 from .utils.attention import configure_attn_implementation, print_attn_implementation
 from .utils.checkpointing import prepare_model_for_training
 from .utils.embedding import resize_embedding_layer
 from .utils.longlora import configure_longlora
 from .utils.moe import add_z3_leaf_module, configure_moe
 from .utils.quantization import configure_quantization
 from .utils.rope import configure_rope
-from .utils.valuehead import configure_valuehead, prepare_valuehead_model
-from .utils.visual import autocast_projector_dtype
+from .utils.valuehead import prepare_valuehead_model
+from .utils.visual import autocast_projector_dtype, configure_visual_model
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedTokenizer
     from trl import AutoModelForCausalLMWithValueHead
 
     from ..hparams import ModelArguments
@@ -36,42 +38,43 @@
 
 def patch_config(
     config: "PretrainedConfig",
     tokenizer: "PreTrainedTokenizer",
     model_args: "ModelArguments",
     init_kwargs: Dict[str, Any],
     is_trainable: bool,
-    add_valuehead: bool,
 ) -> None:
     if model_args.compute_dtype is None:  # priority: bf16 > fp16 > fp32
         model_args.compute_dtype = infer_optim_dtype(model_dtype=getattr(config, "torch_dtype", None))
 
+    if is_torch_npu_available():
+        use_jit_compile = os.environ.get("JIT_COMPILE", "0").lower() in ["true", "1"]
+        torch.npu.set_compile_mode(jit_compile=use_jit_compile)
+
     configure_attn_implementation(config, model_args)
     configure_rope(config, model_args, is_trainable)
     configure_longlora(config, model_args, is_trainable)
     configure_quantization(config, tokenizer, model_args, init_kwargs)
     configure_moe(config, model_args, is_trainable)
-
-    if add_valuehead:
-        configure_valuehead(config)
+    configure_visual_model(config)
 
     if model_args.use_cache and not is_trainable:
         setattr(config, "use_cache", True)
         logger.info("Using KV cache for faster generation.")
 
     if getattr(config, "model_type", None) == "qwen":
-        setattr(config, "use_flash_attn", model_args.flash_attn)
+        setattr(config, "use_flash_attn", model_args.flash_attn == "fa2")
         for dtype_name, dtype in [("fp16", torch.float16), ("bf16", torch.bfloat16), ("fp32", torch.float32)]:
             setattr(config, dtype_name, model_args.compute_dtype == dtype)
 
     if getattr(config, "model_type", None) == "qwen2" and is_trainable and model_args.flash_attn:
         setattr(config, "use_cache", False)  # qwen2 does not support use_cache when using flashattn
 
     init_kwargs["torch_dtype"] = model_args.compute_dtype
-    if not is_deepspeed_zero3_enabled():
+    if not is_deepspeed_zero3_enabled() and not is_fsdp_enabled():
         init_kwargs["low_cpu_mem_usage"] = model_args.low_cpu_mem_usage
         if init_kwargs["low_cpu_mem_usage"]:
             if "device_map" not in init_kwargs and model_args.device_map:
                 init_kwargs["device_map"] = model_args.device_map
 
             if init_kwargs["device_map"] == "auto":
                 init_kwargs["offload_folder"] = model_args.offload_folder
```

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/attention.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         return
 
     elif model_args.flash_attn == "off":
         requested_attn_implementation = "eager"
 
     elif model_args.flash_attn == "sdpa":
         if not is_sdpa_available():
-            logger.warning("Torch>=2.1.1 is required for SDPA attention.")
+            logger.warning("torch>=2.1.1 is required for SDPA attention.")
             return
 
         requested_attn_implementation = "sdpa"
     elif model_args.flash_attn == "fa2":
         if not is_flash_attn2_available():
             logger.warning("FlashAttention-2 is not installed.")
             return
@@ -48,8 +48,8 @@
         attn_implementation = getattr(config, "_attn_implementation", None)
 
     if attn_implementation == "flash_attention_2":
         logger.info("Using FlashAttention-2 for faster training and inference.")
     elif attn_implementation == "sdpa":
         logger.info("Using torch SDPA for faster training and inference.")
     else:
-        logger.info("Using vanilla Attention implementation.")
+        logger.info("Using vanilla attention implementation.")
```

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/checkpointing.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/embedding.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/longlora.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/longlora.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     apply_rotary_pos_emb,
     repeat_kv,
 )
 from transformers.utils import logging
 from transformers.utils.versions import require_version
 
 from ...extras.constants import SUPPORTED_CLASS_FOR_S2ATTN
+from ...extras.logging import get_logger
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig
 
     from ...hparams import ModelArguments
 
@@ -36,17 +37,17 @@
     past_key_value: Optional["Cache"] = None,
     output_attentions: bool = False,
     cache_position: Optional[torch.LongTensor] = None,
     **kwargs,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
     bsz, q_len, _ = hidden_states.size()
 
-    query_states = self.q_proj(hidden_states)
-    key_states = self.k_proj(hidden_states)
-    value_states = self.v_proj(hidden_states)
+    query_states: "torch.Tensor" = self.q_proj(hidden_states)
+    key_states: "torch.Tensor" = self.k_proj(hidden_states)
+    value_states: "torch.Tensor" = self.v_proj(hidden_states)
 
     query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
     key_states = key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
     value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
 
     cos, sin = self.rotary_emb(value_states, position_ids)
     query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
@@ -82,15 +83,15 @@
     if attention_mask is not None:  # no matter the length, we just slice it
         causal_mask = attention_mask[:, :, :, : key_states.shape[-2]]
         attn_weights = attn_weights + causal_mask
 
     # upcast attention to fp32
     attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
     attn_weights = nn.functional.dropout(attn_weights, p=self.attention_dropout, training=self.training)
-    attn_output = torch.matmul(attn_weights, value_states)  # (bsz, :, seq_len, :) or (bsz*n_group, :, groupsz, :)
+    attn_output = torch.matmul(attn_weights, value_states)  # (bsz, :, seq_len, :) or (bsz * n_group, :, groupsz, :)
     attn_output = attn_output.transpose(1, 2).contiguous()
 
     if getattr(self.config, "group_size_ratio", None) and self.training:  # shift back
         attn_output.reshape(bsz, q_len, self.num_heads, self.head_dim)
         attn_output = torch.cat(
             (
                 attn_output[:, :, : self.num_heads // 2],
@@ -120,17 +121,17 @@
     **kwargs,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
     # LlamaFlashAttention2 attention does not support output_attentions
     output_attentions = False
 
     bsz, q_len, _ = hidden_states.size()
 
-    query_states = self.q_proj(hidden_states)
-    key_states = self.k_proj(hidden_states)
-    value_states = self.v_proj(hidden_states)
+    query_states: "torch.Tensor" = self.q_proj(hidden_states)
+    key_states: "torch.Tensor" = self.k_proj(hidden_states)
+    value_states: "torch.Tensor" = self.v_proj(hidden_states)
 
     query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
     key_states = key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
     value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
 
     cos, sin = self.rotary_emb(value_states, position_ids)
     query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
@@ -175,18 +176,20 @@
                 (state[:, :, : self.num_heads // 2], state[:, :, self.num_heads // 2 :].roll(-groupsz // 2, dims=1)),
                 dim=2,
             )
             return state.reshape(bsz * num_groups, groupsz, self.num_heads, self.head_dim)
 
         query_states, key_states, value_states = shift(query_states), shift(key_states), shift(value_states)
         if attention_mask is not None:
-            attention_mask = attention_mask[:, :, :groupsz, :groupsz].repeat(num_groups, 1, 1, 1)
+            attention_mask = attention_mask[:, :groupsz].repeat(num_groups, 1)
+    else:
+        groupsz = q_len
 
     attn_output: torch.Tensor = self._flash_attention_forward(
-        query_states, key_states, value_states, attention_mask, q_len, dropout=dropout_rate
+        query_states, key_states, value_states, attention_mask, groupsz, dropout=dropout_rate
     )
 
     if getattr(self.config, "group_size_ratio", None) and self.training:  # shift back
         attn_output.reshape(bsz, q_len, self.num_heads, self.head_dim)
         attn_output = torch.cat(
             (
                 attn_output[:, :, : self.num_heads // 2],
@@ -226,17 +229,17 @@
             output_attentions=output_attentions,
             cache_position=cache_position,
             **kwargs,
         )
 
     bsz, q_len, _ = hidden_states.size()
 
-    query_states = self.q_proj(hidden_states)
-    key_states = self.k_proj(hidden_states)
-    value_states = self.v_proj(hidden_states)
+    query_states: "torch.Tensor" = self.q_proj(hidden_states)
+    key_states: "torch.Tensor" = self.k_proj(hidden_states)
+    value_states: "torch.Tensor" = self.v_proj(hidden_states)
 
     query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
     key_states = key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
     value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
 
     cos, sin = self.rotary_emb(value_states, position_ids)
     query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
@@ -263,19 +266,20 @@
 
         query_states, key_states, value_states = shift(query_states), shift(key_states), shift(value_states)
         if attention_mask is not None:
             attention_mask = attention_mask[:, :, :groupsz, :groupsz].repeat(num_groups, 1, 1, 1)
 
     causal_mask = attention_mask
     if attention_mask is not None:
-        causal_mask = causal_mask[:, :, :, :groupsz]
+        causal_mask = causal_mask[:, :, :, : key_states.shape[-2]]
 
-    query_states = query_states.contiguous()
-    key_states = key_states.contiguous()
-    value_states = value_states.contiguous()
+    if query_states.device.type == "cuda" and causal_mask is not None:
+        query_states = query_states.contiguous()
+        key_states = key_states.contiguous()
+        value_states = value_states.contiguous()
 
     attn_output = torch.nn.functional.scaled_dot_product_attention(
         query_states,
         key_states,
         value_states,
         attn_mask=causal_mask,
         dropout_p=self.attention_dropout if self.training else 0.0,
@@ -295,23 +299,25 @@
     attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
     attn_output = self.o_proj(attn_output)
 
     return attn_output, None, past_key_value
 
 
 def _apply_llama_patch() -> None:
-    require_version("transformers==4.40.0", "To fix: pip install transformers==4.40.0")
+    require_version("transformers==4.40.2", "To fix: pip install transformers==4.40.2")
     LlamaAttention.forward = llama_attention_forward
     LlamaFlashAttention2.forward = llama_flash_attention_2_forward
     LlamaSdpaAttention.forward = llama_sdpa_attention_forward
 
 
 def configure_longlora(config: "PretrainedConfig", model_args: "ModelArguments", is_trainable: bool) -> None:
     if not is_trainable or not model_args.shift_attn:
         return
 
+    logger = get_logger(__name__)
+
     if getattr(config, "model_type", None) in SUPPORTED_CLASS_FOR_S2ATTN:
         setattr(config, "group_size_ratio", 0.25)
         _apply_llama_patch()
         logger.info("Using shift short attention with group_size_ratio=1/4.")
     else:
         logger.warning("Current model does not support shift short attention.")
```

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/misc.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/misc.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/mod.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/mod.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/moe.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/moe.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/quantization.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from enum import Enum, unique
 from typing import TYPE_CHECKING, Any, Dict, List
 
 import torch
 from datasets import load_dataset
 from transformers import BitsAndBytesConfig, GPTQConfig
 from transformers.integrations import is_deepspeed_zero3_enabled
+from transformers.modeling_utils import is_fsdp_enabled
 from transformers.utils.versions import require_version
 
 from ...extras.constants import FILEEXT2TYPE
 from ...extras.logging import get_logger
 from ...extras.misc import get_current_device
 
 
@@ -129,15 +130,15 @@
                 load_in_4bit=True,
                 bnb_4bit_compute_dtype=model_args.compute_dtype,
                 bnb_4bit_use_double_quant=model_args.double_quantization,
                 bnb_4bit_quant_type=model_args.quantization_type,
                 bnb_4bit_quant_storage=model_args.compute_dtype,  # crucial for fsdp qlora
             )
 
-        if is_deepspeed_zero3_enabled() or model_args.quantization_device_map == "auto":
+        if is_deepspeed_zero3_enabled() or is_fsdp_enabled() or model_args.quantization_device_map == "auto":
             if model_args.quantization_bit != 4:
                 raise ValueError("Only 4-bit quantized model can use auto device map.")
 
             require_version("transformers>=4.39.0", "To fix: pip install transformers>=4.39.0")
             require_version("accelerate>=0.28.0", "To fix: pip install accelerate>=0.28.0")
             require_version("bitsandbytes>=0.43.0", "To fix: pip install bitsandbytes>=0.43.0")
         else:
```

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/rope.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/rope.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/unsloth.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/unsloth.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/model/utils/valuehead.py` & `llmtuner-0.7.1/src/llmtuner/model/utils/valuehead.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,22 @@
 from transformers.utils import cached_file
 
 from ...extras.constants import V_HEAD_SAFE_WEIGHTS_NAME, V_HEAD_WEIGHTS_NAME
 from ...extras.logging import get_logger
 
 
 if TYPE_CHECKING:
-    from transformers import PretrainedConfig, PreTrainedModel
+    from transformers import PreTrainedModel
 
     from ...hparams import ModelArguments
 
 
 logger = get_logger(__name__)
 
 
-def configure_valuehead(config: "PretrainedConfig") -> None:
-    if getattr(config, "model_type", None) == "llava":
-        setattr(config, "hidden_size", getattr(config.vision_config, "intermediate_size", None))
-
-
 def load_valuehead_params(path_or_repo_id: str, model_args: "ModelArguments") -> Dict[str, torch.Tensor]:
     r"""
     Loads value head parameters from Hugging Face Hub or local disk.
 
     Returns: dict with keys `v_head.summary.weight` and `v_head.summary.bias`.
     """
     kwargs = {"path_or_repo_id": path_or_repo_id, "cache_dir": model_args.cache_dir, "token": model_args.hf_hub_token}
@@ -53,7 +48,11 @@
     if getattr(model.config, "model_type", None) == "llava":
         setattr(model, "lm_head", model.language_model.get_output_embeddings())
         setattr(model, "_keys_to_ignore_on_save", ["lm_head.weight"])
 
     if getattr(model.config, "model_type", None) == "chatglm":
         setattr(model, "lm_head", model.transformer.output_layer)
         setattr(model, "_keys_to_ignore_on_save", ["lm_head.weight"])
+
+    if getattr(model.config, "model_type", None) == "internlm2":
+        setattr(model, "lm_head", model.output)
+        setattr(model, "_keys_to_ignore_on_save", ["lm_head.weight"])
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/dpo/trainer.py` & `llmtuner-0.7.1/src/llmtuner/train/dpo/trainer.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,34 +9,36 @@
 from trl.trainer.utils import disable_dropout_in_model
 
 from ...extras.constants import IGNORE_INDEX
 from ..utils import create_custom_optimzer, create_custom_scheduler
 
 
 if TYPE_CHECKING:
-    from transformers import PreTrainedModel
+    from transformers import PreTrainedModel, ProcessorMixin
 
     from ...hparams import FinetuningArguments
 
 
 class CustomDPOTrainer(DPOTrainer):
     def __init__(
         self,
         model: Union["PreTrainedModel", torch.nn.Module],
         ref_model: Optional[Union["PreTrainedModel", torch.nn.Module]],
         finetuning_args: "FinetuningArguments",
+        processor: Optional["ProcessorMixin"],
         disable_dropout: bool = True,
         **kwargs,
     ):
         if disable_dropout:
             disable_dropout_in_model(model)
             if ref_model is not None:
                 disable_dropout_in_model(ref_model)
 
         self.finetuning_args = finetuning_args
+        self.processor = processor
         self.reference_free = False
         self.use_dpo_data_collator = True  # hack to avoid warning
         self.generate_during_eval = False  # disable at evaluation
         self.label_pad_token_id = IGNORE_INDEX
         self.padding_value = 0
         self.is_encoder_decoder = model.config.is_encoder_decoder
         self.precompute_ref_log_probs = False
@@ -76,14 +78,20 @@
 
     def create_scheduler(
         self, num_training_steps: int, optimizer: Optional["torch.optim.Optimizer"] = None
     ) -> "torch.optim.lr_scheduler.LRScheduler":
         create_custom_scheduler(self.args, num_training_steps, optimizer)
         return super().create_scheduler(num_training_steps, optimizer)
 
+    def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, "torch.Tensor"]] = None) -> None:
+        super()._save(output_dir, state_dict)
+        if self.processor is not None:
+            output_dir = output_dir if output_dir is not None else self.args.output_dir
+            getattr(self.processor, "image_processor").save_pretrained(output_dir)
+
     def sft_loss(self, chosen_logits: "torch.FloatTensor", chosen_labels: "torch.LongTensor") -> "torch.Tensor":
         r"""
         Computes supervised cross-entropy loss of given labels under the given logits.
 
         Returns:
             A tensor of shape (batch_size,) containing the cross-entropy loss of each samples.
         """
@@ -161,17 +169,17 @@
             batch_size = batch["input_ids"].size(0) // 2
             chosen_labels, _ = batch["labels"].split(batch_size, dim=0)
             losses += self.ftx_gamma * self.sft_loss(policy_chosen_logits, chosen_labels)
 
         reward_accuracies = (chosen_rewards > rejected_rewards).float()
 
         prefix = "eval_" if train_eval == "eval" else ""
-        metrics["{}rewards/chosen".format(prefix)] = chosen_rewards.cpu().mean()
-        metrics["{}rewards/rejected".format(prefix)] = rejected_rewards.cpu().mean()
-        metrics["{}rewards/accuracies".format(prefix)] = reward_accuracies.cpu().mean()
-        metrics["{}rewards/margins".format(prefix)] = (chosen_rewards - rejected_rewards).cpu().mean()
-        metrics["{}logps/rejected".format(prefix)] = policy_rejected_logps.detach().cpu().mean()
-        metrics["{}logps/chosen".format(prefix)] = policy_chosen_logps.detach().cpu().mean()
-        metrics["{}logits/rejected".format(prefix)] = policy_rejected_logits.detach().cpu().mean()
-        metrics["{}logits/chosen".format(prefix)] = policy_chosen_logits.detach().cpu().mean()
+        metrics["{}rewards/chosen".format(prefix)] = chosen_rewards.mean().cpu()
+        metrics["{}rewards/rejected".format(prefix)] = rejected_rewards.mean().cpu()
+        metrics["{}rewards/accuracies".format(prefix)] = reward_accuracies.mean().cpu()
+        metrics["{}rewards/margins".format(prefix)] = (chosen_rewards - rejected_rewards).mean().cpu()
+        metrics["{}logps/rejected".format(prefix)] = policy_rejected_logps.detach().mean().cpu()
+        metrics["{}logps/chosen".format(prefix)] = policy_chosen_logps.detach().mean().cpu()
+        metrics["{}logits/rejected".format(prefix)] = policy_rejected_logits.detach().mean().cpu()
+        metrics["{}logits/chosen".format(prefix)] = policy_chosen_logits.detach().mean().cpu()
 
         return losses.mean(), metrics
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/dpo/workflow.py` & `llmtuner-0.7.1/src/llmtuner/train/dpo/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
     # Initialize our Trainer
     trainer = CustomDPOTrainer(
         model=model,
         ref_model=ref_model,
         args=training_args,
         finetuning_args=finetuning_args,
-        tokenizer=tokenizer,
         data_collator=data_collator,
         callbacks=callbacks,
+        **tokenizer_module,
         **split_dataset(dataset, data_args, training_args),
     )
 
     # Training
     if training_args.do_train:
         train_result = trainer.train(resume_from_checkpoint=training_args.resume_from_checkpoint)
         trainer.save_model()
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/orpo/trainer.py` & `llmtuner-0.7.1/src/llmtuner/train/orpo/trainer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,135 @@
-from collections import defaultdict
-from types import MethodType
-from typing import TYPE_CHECKING, Dict, Literal, Optional, Tuple, Union
-
-import torch
-import torch.nn.functional as F
-from transformers import Trainer
-from trl import DPOTrainer
-from trl.trainer.utils import disable_dropout_in_model
-
-from ...extras.constants import IGNORE_INDEX
-from ..utils import create_custom_optimzer, create_custom_scheduler
-
-
-if TYPE_CHECKING:
-    from transformers import PreTrainedModel
-
-    from ...hparams import FinetuningArguments
-
-
-class CustomORPOTrainer(DPOTrainer):
-    def __init__(
-        self,
-        model: Union["PreTrainedModel", "torch.nn.Module"],
-        finetuning_args: "FinetuningArguments",
-        disable_dropout: bool = True,
-        **kwargs,
-    ):
-        if disable_dropout:
-            disable_dropout_in_model(model)
-
-        self.finetuning_args = finetuning_args
-        self.reference_free = False
-        self.use_dpo_data_collator = True  # hack to avoid warning
-        self.generate_during_eval = False  # disable at evaluation
-        self.label_pad_token_id = IGNORE_INDEX
-        self.padding_value = 0
-        self.is_encoder_decoder = model.config.is_encoder_decoder
-        self.precompute_ref_log_probs = False
-        self._precomputed_train_ref_log_probs = False
-        self._precomputed_eval_ref_log_probs = False
-        self._peft_has_been_casted_to_bf16 = False
-
-        self.beta = finetuning_args.orpo_beta
-        self._stored_metrics = defaultdict(lambda: defaultdict(list))
-
-        Trainer.__init__(self, model=model, **kwargs)
-        if finetuning_args.use_badam:
-            from badam import clip_grad_norm_for_sparse_tensor
-
-            self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
-
-    def create_optimizer(self) -> "torch.optim.Optimizer":
-        if self.optimizer is None:
-            self.optimizer = create_custom_optimzer(self.model, self.args, self.finetuning_args)
-        return super().create_optimizer()
-
-    def create_scheduler(
-        self, num_training_steps: int, optimizer: Optional["torch.optim.Optimizer"] = None
-    ) -> "torch.optim.lr_scheduler.LRScheduler":
-        create_custom_scheduler(self.args, num_training_steps, optimizer)
-        return super().create_scheduler(num_training_steps, optimizer)
-
-    def odds_ratio_loss(self, chosen_logps: "torch.Tensor", rejected_logps: "torch.Tensor") -> "torch.Tensor":
-        r"""
-        Computes ORPO's odds ratio (OR) loss.
-        """
-        log_odds = (chosen_logps - rejected_logps) - (
-            torch.log1p(-torch.exp(chosen_logps)) - torch.log1p(-torch.exp(rejected_logps))
-        )
-        odds_ratio_loss = -F.logsigmoid(log_odds)
-        return odds_ratio_loss
-
-    def concatenated_forward(
-        self, model: "PreTrainedModel", batch: Dict[str, "torch.Tensor"]
-    ) -> Tuple["torch.Tensor", "torch.Tensor", "torch.Tensor", "torch.Tensor"]:
-        r"""
-        Computes the average log probabilities of the labels under the given logits.
-        """
-        all_logits: "torch.Tensor" = model(
-            input_ids=batch["input_ids"], attention_mask=batch["attention_mask"], return_dict=True, use_cache=False
-        ).logits.to(torch.float32)
-
-        all_logps = self.get_batch_logps(
-            logits=all_logits,
-            labels=batch["labels"],
-            average_log_prob=True,
-            is_encoder_decoder=self.is_encoder_decoder,
-            label_pad_token_id=self.label_pad_token_id,
-        )
-        batch_size = batch["input_ids"].size(0) // 2
-        chosen_logps, rejected_logps = all_logps.split(batch_size, dim=0)
-        chosen_logits, rejected_logits = all_logits.split(batch_size, dim=0)
-        return chosen_logps, rejected_logps, chosen_logits, rejected_logits
-
-    def get_batch_loss_metrics(
-        self,
-        model: "PreTrainedModel",
-        batch: Dict[str, "torch.Tensor"],
-        train_eval: Literal["train", "eval"] = "train",
-    ) -> Tuple["torch.Tensor", Dict[str, "torch.Tensor"]]:
-        r"""
-        Computes the ORPO loss and other metrics for the given batch of inputs for train or test.
-        """
-        metrics = {}
-        chosen_logps, rejected_logps, chosen_logits, rejected_logits = self.concatenated_forward(model, batch)
-        sft_loss = -chosen_logps
-        odds_ratio_loss = self.odds_ratio_loss(chosen_logps, rejected_logps)
-        batch_loss = (sft_loss + self.beta * odds_ratio_loss).mean()
-
-        chosen_rewards = self.beta * chosen_logps.detach()
-        rejected_rewards = self.beta * rejected_logps.detach()
-        reward_accuracies = (chosen_rewards > rejected_rewards).float()
-
-        prefix = "eval_" if train_eval == "eval" else ""
-        metrics["{}rewards/chosen".format(prefix)] = chosen_rewards.cpu().mean()
-        metrics["{}rewards/rejected".format(prefix)] = rejected_rewards.cpu().mean()
-        metrics["{}rewards/accuracies".format(prefix)] = reward_accuracies.cpu().mean()
-        metrics["{}rewards/margins".format(prefix)] = (chosen_rewards - rejected_rewards).cpu().mean()
-        metrics["{}logps/rejected".format(prefix)] = rejected_logps.detach().cpu().mean()
-        metrics["{}logps/chosen".format(prefix)] = chosen_logps.detach().cpu().mean()
-        metrics["{}logits/rejected".format(prefix)] = rejected_logits.detach().cpu().mean()
-        metrics["{}logits/chosen".format(prefix)] = chosen_logits.detach().cpu().mean()
-        metrics["{}sft_loss".format(prefix)] = sft_loss.detach().cpu().mean()
-        metrics["{}odds_ratio_loss".format(prefix)] = odds_ratio_loss.detach().cpu().mean()
-
-        return batch_loss, metrics
+from collections import defaultdict
+from types import MethodType
+from typing import TYPE_CHECKING, Dict, Literal, Optional, Tuple, Union
+
+import torch
+import torch.nn.functional as F
+from transformers import Trainer
+from trl import DPOTrainer
+from trl.trainer.utils import disable_dropout_in_model
+
+from ...extras.constants import IGNORE_INDEX
+from ..utils import create_custom_optimzer, create_custom_scheduler
+
+
+if TYPE_CHECKING:
+    from transformers import PreTrainedModel, ProcessorMixin
+
+    from ...hparams import FinetuningArguments
+
+
+class CustomORPOTrainer(DPOTrainer):
+    def __init__(
+        self,
+        model: Union["PreTrainedModel", "torch.nn.Module"],
+        finetuning_args: "FinetuningArguments",
+        processor: Optional["ProcessorMixin"],
+        disable_dropout: bool = True,
+        **kwargs,
+    ):
+        if disable_dropout:
+            disable_dropout_in_model(model)
+
+        self.finetuning_args = finetuning_args
+        self.processor = processor
+        self.reference_free = False
+        self.use_dpo_data_collator = True  # hack to avoid warning
+        self.generate_during_eval = False  # disable at evaluation
+        self.label_pad_token_id = IGNORE_INDEX
+        self.padding_value = 0
+        self.is_encoder_decoder = model.config.is_encoder_decoder
+        self.precompute_ref_log_probs = False
+        self._precomputed_train_ref_log_probs = False
+        self._precomputed_eval_ref_log_probs = False
+        self._peft_has_been_casted_to_bf16 = False
+
+        self.beta = finetuning_args.orpo_beta
+        self._stored_metrics = defaultdict(lambda: defaultdict(list))
+
+        Trainer.__init__(self, model=model, **kwargs)
+        if finetuning_args.use_badam:
+            from badam import clip_grad_norm_for_sparse_tensor
+
+            self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
+
+    def create_optimizer(self) -> "torch.optim.Optimizer":
+        if self.optimizer is None:
+            self.optimizer = create_custom_optimzer(self.model, self.args, self.finetuning_args)
+        return super().create_optimizer()
+
+    def create_scheduler(
+        self, num_training_steps: int, optimizer: Optional["torch.optim.Optimizer"] = None
+    ) -> "torch.optim.lr_scheduler.LRScheduler":
+        create_custom_scheduler(self.args, num_training_steps, optimizer)
+        return super().create_scheduler(num_training_steps, optimizer)
+
+    def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, "torch.Tensor"]] = None) -> None:
+        super()._save(output_dir, state_dict)
+        if self.processor is not None:
+            output_dir = output_dir if output_dir is not None else self.args.output_dir
+            getattr(self.processor, "image_processor").save_pretrained(output_dir)
+
+    def odds_ratio_loss(self, chosen_logps: "torch.Tensor", rejected_logps: "torch.Tensor") -> "torch.Tensor":
+        r"""
+        Computes ORPO's odds ratio (OR) loss.
+        """
+        log_odds = (chosen_logps - rejected_logps) - (
+            torch.log1p(-torch.exp(chosen_logps)) - torch.log1p(-torch.exp(rejected_logps))
+        )
+        odds_ratio_loss = -F.logsigmoid(log_odds)
+        return odds_ratio_loss
+
+    def concatenated_forward(
+        self, model: "PreTrainedModel", batch: Dict[str, "torch.Tensor"]
+    ) -> Tuple["torch.Tensor", "torch.Tensor", "torch.Tensor", "torch.Tensor"]:
+        r"""
+        Computes the average log probabilities of the labels under the given logits.
+        """
+        all_logits: "torch.Tensor" = model(
+            input_ids=batch["input_ids"], attention_mask=batch["attention_mask"], return_dict=True, use_cache=False
+        ).logits.to(torch.float32)
+
+        all_logps = self.get_batch_logps(
+            logits=all_logits,
+            labels=batch["labels"],
+            average_log_prob=True,
+            is_encoder_decoder=self.is_encoder_decoder,
+            label_pad_token_id=self.label_pad_token_id,
+        )
+        batch_size = batch["input_ids"].size(0) // 2
+        chosen_logps, rejected_logps = all_logps.split(batch_size, dim=0)
+        chosen_logits, rejected_logits = all_logits.split(batch_size, dim=0)
+        return chosen_logps, rejected_logps, chosen_logits, rejected_logits
+
+    def get_batch_loss_metrics(
+        self,
+        model: "PreTrainedModel",
+        batch: Dict[str, "torch.Tensor"],
+        train_eval: Literal["train", "eval"] = "train",
+    ) -> Tuple["torch.Tensor", Dict[str, "torch.Tensor"]]:
+        r"""
+        Computes the ORPO loss and other metrics for the given batch of inputs for train or test.
+        """
+        metrics = {}
+        chosen_logps, rejected_logps, chosen_logits, rejected_logits = self.concatenated_forward(model, batch)
+        sft_loss = -chosen_logps
+        odds_ratio_loss = self.odds_ratio_loss(chosen_logps, rejected_logps)
+        batch_loss = (sft_loss + self.beta * odds_ratio_loss).mean()
+
+        chosen_rewards = self.beta * chosen_logps.detach()
+        rejected_rewards = self.beta * rejected_logps.detach()
+        reward_accuracies = (chosen_rewards > rejected_rewards).float()
+
+        prefix = "eval_" if train_eval == "eval" else ""
+        metrics["{}rewards/chosen".format(prefix)] = chosen_rewards.mean().cpu()
+        metrics["{}rewards/rejected".format(prefix)] = rejected_rewards.mean().cpu()
+        metrics["{}rewards/accuracies".format(prefix)] = reward_accuracies.mean().cpu()
+        metrics["{}rewards/margins".format(prefix)] = (chosen_rewards - rejected_rewards).mean().cpu()
+        metrics["{}logps/rejected".format(prefix)] = rejected_logps.detach().mean().cpu()
+        metrics["{}logps/chosen".format(prefix)] = chosen_logps.detach().mean().cpu()
+        metrics["{}logits/rejected".format(prefix)] = rejected_logits.detach().mean().cpu()
+        metrics["{}logits/chosen".format(prefix)] = chosen_logits.detach().mean().cpu()
+        metrics["{}sft_loss".format(prefix)] = sft_loss.detach().mean().cpu()
+        metrics["{}odds_ratio_loss".format(prefix)] = odds_ratio_loss.detach().mean().cpu()
+
+        return batch_loss, metrics
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/orpo/workflow.py` & `llmtuner-0.7.1/src/llmtuner/train/orpo/workflow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# Inspired by: https://github.com/huggingface/trl/blob/main/examples/research_projects/stack_llama_2/scripts/dpo_llama2.py
-
-from typing import TYPE_CHECKING, List, Optional
-
-from ...data import PairwiseDataCollatorWithPadding, get_dataset, split_dataset
-from ...extras.constants import IGNORE_INDEX
-from ...extras.ploting import plot_loss
-from ...hparams import ModelArguments
-from ...model import load_model, load_tokenizer
-from ..utils import create_modelcard_and_push
-from .trainer import CustomORPOTrainer
-
-
-if TYPE_CHECKING:
-    from transformers import Seq2SeqTrainingArguments, TrainerCallback
-
-    from ...hparams import DataArguments, FinetuningArguments
-
-
-def run_orpo(
-    model_args: "ModelArguments",
-    data_args: "DataArguments",
-    training_args: "Seq2SeqTrainingArguments",
-    finetuning_args: "FinetuningArguments",
-    callbacks: Optional[List["TrainerCallback"]] = None,
-):
-    tokenizer_module = load_tokenizer(model_args)
-    tokenizer = tokenizer_module["tokenizer"]
-    dataset = get_dataset(model_args, data_args, training_args, stage="rm", **tokenizer_module)
-    model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train)
-
-    data_collator = PairwiseDataCollatorWithPadding(
-        tokenizer=tokenizer,
-        pad_to_multiple_of=8,
-        label_pad_token_id=IGNORE_INDEX if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id,
-    )
-
-    # Update arguments
-    training_args.remove_unused_columns = False  # important for pairwise dataset
-
-    # Initialize our Trainer
-    trainer = CustomORPOTrainer(
-        model=model,
-        args=training_args,
-        finetuning_args=finetuning_args,
-        tokenizer=tokenizer,
-        data_collator=data_collator,
-        callbacks=callbacks,
-        **split_dataset(dataset, data_args, training_args),
-    )
-
-    # Training
-    if training_args.do_train:
-        train_result = trainer.train(resume_from_checkpoint=training_args.resume_from_checkpoint)
-        trainer.save_model()
-        trainer.log_metrics("train", train_result.metrics)
-        trainer.save_metrics("train", train_result.metrics)
-        trainer.save_state()
-        if trainer.is_world_process_zero() and finetuning_args.plot_loss:
-            plot_loss(training_args.output_dir, keys=["loss", "eval_loss", "rewards/accuracies", "sft_loss"])
-
-    # Evaluation
-    if training_args.do_eval:
-        metrics = trainer.evaluate(metric_key_prefix="eval")
-        trainer.log_metrics("eval", metrics)
-        trainer.save_metrics("eval", metrics)
-
-    # Create model card
-    create_modelcard_and_push(trainer, model_args, data_args, training_args, finetuning_args)
+# Inspired by: https://github.com/huggingface/trl/blob/main/examples/research_projects/stack_llama_2/scripts/dpo_llama2.py
+
+from typing import TYPE_CHECKING, List, Optional
+
+from ...data import PairwiseDataCollatorWithPadding, get_dataset, split_dataset
+from ...extras.constants import IGNORE_INDEX
+from ...extras.ploting import plot_loss
+from ...hparams import ModelArguments
+from ...model import load_model, load_tokenizer
+from ..utils import create_modelcard_and_push
+from .trainer import CustomORPOTrainer
+
+
+if TYPE_CHECKING:
+    from transformers import Seq2SeqTrainingArguments, TrainerCallback
+
+    from ...hparams import DataArguments, FinetuningArguments
+
+
+def run_orpo(
+    model_args: "ModelArguments",
+    data_args: "DataArguments",
+    training_args: "Seq2SeqTrainingArguments",
+    finetuning_args: "FinetuningArguments",
+    callbacks: Optional[List["TrainerCallback"]] = None,
+):
+    tokenizer_module = load_tokenizer(model_args)
+    tokenizer = tokenizer_module["tokenizer"]
+    dataset = get_dataset(model_args, data_args, training_args, stage="rm", **tokenizer_module)
+    model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train)
+
+    data_collator = PairwiseDataCollatorWithPadding(
+        tokenizer=tokenizer,
+        pad_to_multiple_of=8,
+        label_pad_token_id=IGNORE_INDEX if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id,
+    )
+
+    # Update arguments
+    training_args.remove_unused_columns = False  # important for pairwise dataset
+
+    # Initialize our Trainer
+    trainer = CustomORPOTrainer(
+        model=model,
+        args=training_args,
+        finetuning_args=finetuning_args,
+        data_collator=data_collator,
+        callbacks=callbacks,
+        **tokenizer_module,
+        **split_dataset(dataset, data_args, training_args),
+    )
+
+    # Training
+    if training_args.do_train:
+        train_result = trainer.train(resume_from_checkpoint=training_args.resume_from_checkpoint)
+        trainer.save_model()
+        trainer.log_metrics("train", train_result.metrics)
+        trainer.save_metrics("train", train_result.metrics)
+        trainer.save_state()
+        if trainer.is_world_process_zero() and finetuning_args.plot_loss:
+            plot_loss(training_args.output_dir, keys=["loss", "eval_loss", "rewards/accuracies", "sft_loss"])
+
+    # Evaluation
+    if training_args.do_eval:
+        metrics = trainer.evaluate(metric_key_prefix="eval")
+        trainer.log_metrics("eval", metrics)
+        trainer.save_metrics("eval", metrics)
+
+    # Create model card
+    create_modelcard_and_push(trainer, model_args, data_args, training_args, finetuning_args)
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/ppo/trainer.py` & `llmtuner-0.7.1/src/llmtuner/train/ppo/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 from ...extras.misc import AverageMeter, count_parameters, get_current_device, get_logits_processor
 from ..utils import create_custom_optimzer, create_custom_scheduler
 from .utils import dump_layernorm, get_rewards_from_server, replace_model, restore_layernorm
 
 
 if TYPE_CHECKING:
     from datasets import Dataset
-    from transformers import DataCollatorWithPadding, PreTrainedTokenizer, Seq2SeqTrainingArguments, TrainerCallback
+    from transformers import (
+        DataCollatorWithPadding,
+        PreTrainedTokenizer,
+        ProcessorMixin,
+        Seq2SeqTrainingArguments,
+        TrainerCallback,
+    )
     from trl import AutoModelForCausalLMWithValueHead
 
     from ...hparams import FinetuningArguments, GeneratingArguments, ModelArguments
 
 
 logger = get_logger(__name__)
 
@@ -44,14 +50,15 @@
         finetuning_args: "FinetuningArguments",
         generating_args: "GeneratingArguments",
         callbacks: List["TrainerCallback"],
         model: "AutoModelForCausalLMWithValueHead",
         reward_model: Optional["AutoModelForCausalLMWithValueHead"],
         ref_model: Optional["AutoModelForCausalLMWithValueHead"],
         tokenizer: "PreTrainedTokenizer",
+        processor: Optional["ProcessorMixin"],
         dataset: "Dataset",
         data_collator: "DataCollatorWithPadding",
     ):
         backward_batch_size = training_args.per_device_train_batch_size * training_args.gradient_accumulation_steps
         ppo_config = PPOConfig(
             model_name=model_args.model_name_or_path,
             learning_rate=training_args.learning_rate,
@@ -93,14 +100,15 @@
         )
 
         self.args = training_args
         self.model_args = model_args
         self.finetuning_args = finetuning_args
         self.reward_model = reward_model
         self.current_device = get_current_device()  # patch for deepspeed training
+        self.processor = processor
 
         self.generation_config = GenerationConfig(
             pad_token_id=self.tokenizer.pad_token_id,
             eos_token_id=[self.tokenizer.eos_token_id] + self.tokenizer.additional_special_tokens_ids,
             **generating_args.to_dict(),
         )
 
@@ -291,14 +299,20 @@
             training_args.lr_scheduler_type,
             optimizer=optimizer,
             num_warmup_steps=training_args.get_warmup_steps(num_training_steps),
             num_training_steps=num_training_steps,
         )
         return lr_scheduler
 
+    def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, "torch.Tensor"]] = None) -> None:
+        super()._save(output_dir, state_dict)
+        if self.processor is not None:
+            output_dir = output_dir if output_dir is not None else self.args.output_dir
+            getattr(self.processor, "image_processor").save_pretrained(output_dir)
+
     @torch.no_grad()
     def get_inputs(self, batch: Dict[str, torch.Tensor]) -> Tuple[List[torch.Tensor], List[torch.Tensor]]:
         r"""
         Generates model's responses given queries.
         """
         if self.model_args.upcast_layernorm:
             layernorm_params = dump_layernorm(self.model)
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/ppo/utils.py` & `llmtuner-0.7.1/src/llmtuner/train/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/train/ppo/workflow.py` & `llmtuner-0.7.1/src/llmtuner/train/ppo/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         training_args=training_args,
         finetuning_args=finetuning_args,
         generating_args=generating_args,
         callbacks=callbacks + [FixValueHeadModelCallback()],
         model=model,
         reward_model=reward_model,
         ref_model=ref_model,
-        tokenizer=tokenizer,
         dataset=dataset,
         data_collator=data_collator,
+        **tokenizer_module,
     )
 
     # Training
     if training_args.do_train:
         ppo_trainer.ppo_train(resume_from_checkpoint=training_args.resume_from_checkpoint)
         ppo_trainer.save_model()
         if training_args.should_save:
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/pt/trainer.py` & `llmtuner-0.7.1/src/llmtuner/train/pt/trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from types import MethodType
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Dict, Optional
 
 from transformers import Trainer
 
 from ...extras.logging import get_logger
 from ..utils import create_custom_optimzer, create_custom_scheduler
 
 
 if TYPE_CHECKING:
     import torch
+    from transformers import ProcessorMixin
 
     from ...hparams import FinetuningArguments
 
 
 logger = get_logger(__name__)
 
 
 class CustomTrainer(Trainer):
     r"""
     Inherits Trainer for custom optimizer.
     """
 
-    def __init__(self, finetuning_args: "FinetuningArguments", **kwargs) -> None:
+    def __init__(
+        self, finetuning_args: "FinetuningArguments", processor: Optional["ProcessorMixin"], **kwargs
+    ) -> None:
         super().__init__(**kwargs)
         self.finetuning_args = finetuning_args
+        self.processor = processor
         if finetuning_args.use_badam:
             from badam import clip_grad_norm_for_sparse_tensor
 
             self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
 
     def create_optimizer(self) -> "torch.optim.Optimizer":
         if self.optimizer is None:
@@ -35,7 +39,13 @@
         return super().create_optimizer()
 
     def create_scheduler(
         self, num_training_steps: int, optimizer: Optional["torch.optim.Optimizer"] = None
     ) -> "torch.optim.lr_scheduler.LRScheduler":
         create_custom_scheduler(self.args, num_training_steps, optimizer)
         return super().create_scheduler(num_training_steps, optimizer)
+
+    def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, "torch.Tensor"]] = None) -> None:
+        super()._save(output_dir, state_dict)
+        if self.processor is not None:
+            output_dir = output_dir if output_dir is not None else self.args.output_dir
+            getattr(self.processor, "image_processor").save_pretrained(output_dir)
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/pt/workflow.py` & `llmtuner-0.7.1/src/llmtuner/train/pt/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     data_collator = DataCollatorForLanguageModeling(tokenizer=tokenizer, mlm=False)
 
     # Initialize our Trainer
     trainer = CustomTrainer(
         model=model,
         args=training_args,
         finetuning_args=finetuning_args,
-        tokenizer=tokenizer,
         data_collator=data_collator,
         callbacks=callbacks,
+        **tokenizer_module,
         **split_dataset(dataset, data_args, training_args),
     )
 
     # Training
     if training_args.do_train:
         train_result = trainer.train(resume_from_checkpoint=training_args.resume_from_checkpoint)
         trainer.save_model()
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/rm/trainer.py` & `llmtuner-0.7.1/src/llmtuner/train/rm/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 from transformers import Trainer
 
 from ...extras.logging import get_logger
 from ..utils import create_custom_optimzer, create_custom_scheduler
 
 
 if TYPE_CHECKING:
-    from transformers.modeling_utils import PreTrainedModel
+    from transformers import PreTrainedModel, ProcessorMixin
     from transformers.trainer import PredictionOutput
 
     from ...hparams import FinetuningArguments
 
 
 logger = get_logger(__name__)
 
 
 class PairwiseTrainer(Trainer):
     r"""
     Inherits Trainer to compute pairwise loss.
     """
 
-    def __init__(self, finetuning_args: "FinetuningArguments", **kwargs) -> None:
+    def __init__(
+        self, finetuning_args: "FinetuningArguments", processor: Optional["ProcessorMixin"], **kwargs
+    ) -> None:
         super().__init__(**kwargs)
         self.finetuning_args = finetuning_args
+        self.processor = processor
         self.can_return_loss = True  # override property to return eval_loss
         if finetuning_args.use_badam:
             from badam import clip_grad_norm_for_sparse_tensor
 
             self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
 
     def create_optimizer(self) -> "torch.optim.Optimizer":
@@ -41,14 +44,20 @@
 
     def create_scheduler(
         self, num_training_steps: int, optimizer: Optional["torch.optim.Optimizer"] = None
     ) -> "torch.optim.lr_scheduler.LRScheduler":
         create_custom_scheduler(self.args, num_training_steps, optimizer)
         return super().create_scheduler(num_training_steps, optimizer)
 
+    def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, "torch.Tensor"]] = None) -> None:
+        super()._save(output_dir, state_dict)
+        if self.processor is not None:
+            output_dir = output_dir if output_dir is not None else self.args.output_dir
+            getattr(self.processor, "image_processor").save_pretrained(output_dir)
+
     def compute_loss(
         self, model: "PreTrainedModel", inputs: Dict[str, torch.Tensor], return_outputs: bool = False
     ) -> Union[torch.Tensor, Tuple[torch.Tensor, List[torch.Tensor]]]:
         r"""
         Computes pairwise loss. The first n examples are chosen and the last n examples are rejected.
 
         Subclass and override to inject custom behavior.
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/rm/workflow.py` & `llmtuner-0.7.1/src/llmtuner/train/rm/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
     training_args.remove_unused_columns = False  # important for pairwise dataset
 
     # Initialize our Trainer
     trainer = PairwiseTrainer(
         model=model,
         args=training_args,
         finetuning_args=finetuning_args,
-        tokenizer=tokenizer,
         data_collator=data_collator,
         callbacks=callbacks + [FixValueHeadModelCallback()],
         compute_metrics=compute_accuracy,
+        **tokenizer_module,
         **split_dataset(dataset, data_args, training_args),
     )
 
     # Training
     if training_args.do_train:
         train_result = trainer.train(resume_from_checkpoint=training_args.resume_from_checkpoint)
         trainer.save_model()
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/sft/metric.py` & `llmtuner-0.7.1/src/llmtuner/train/sft/metric.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/train/sft/trainer.py` & `llmtuner-0.7.1/src/llmtuner/train/sft/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 
 from ...extras.constants import IGNORE_INDEX
 from ...extras.logging import get_logger
 from ..utils import create_custom_optimzer, create_custom_scheduler
 
 
 if TYPE_CHECKING:
+    from transformers import ProcessorMixin
     from transformers.trainer import PredictionOutput
 
     from ...hparams import FinetuningArguments
 
 
 logger = get_logger(__name__)
 
 
 class CustomSeq2SeqTrainer(Seq2SeqTrainer):
     r"""
     Inherits Seq2SeqTrainer to compute generative metrics such as BLEU and ROUGE.
     """
 
-    def __init__(self, finetuning_args: "FinetuningArguments", **kwargs) -> None:
+    def __init__(
+        self, finetuning_args: "FinetuningArguments", processor: Optional["ProcessorMixin"], **kwargs
+    ) -> None:
         super().__init__(**kwargs)
         self.finetuning_args = finetuning_args
+        self.processor = processor
         if finetuning_args.use_badam:
             from badam import clip_grad_norm_for_sparse_tensor
 
             self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
 
     def create_optimizer(self) -> "torch.optim.Optimizer":
         if self.optimizer is None:
@@ -41,14 +45,20 @@
 
     def create_scheduler(
         self, num_training_steps: int, optimizer: Optional["torch.optim.Optimizer"] = None
     ) -> "torch.optim.lr_scheduler.LRScheduler":
         create_custom_scheduler(self.args, num_training_steps, optimizer)
         return super().create_scheduler(num_training_steps, optimizer)
 
+    def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, "torch.Tensor"]] = None) -> None:
+        super()._save(output_dir, state_dict)
+        if self.processor is not None:
+            output_dir = output_dir if output_dir is not None else self.args.output_dir
+            getattr(self.processor, "image_processor").save_pretrained(output_dir)
+
     def prediction_step(
         self,
         model: "torch.nn.Module",
         inputs: Dict[str, Union[torch.Tensor, Any]],
         prediction_loss_only: bool,
         ignore_keys: Optional[List[str]] = None,
     ) -> Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]:
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/sft/workflow.py` & `llmtuner-0.7.1/src/llmtuner/train/sft/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,18 @@
     training_args.remove_unused_columns = False if model_args.visual_inputs else training_args.remove_unused_columns
 
     # Initialize our Trainer
     trainer = CustomSeq2SeqTrainer(
         model=model,
         args=training_args,
         finetuning_args=finetuning_args,
-        tokenizer=tokenizer,
         data_collator=data_collator,
         callbacks=callbacks,
         compute_metrics=ComputeMetrics(tokenizer) if training_args.predict_with_generate else None,
+        **tokenizer_module,
         **split_dataset(dataset, data_args, training_args),
     )
 
     # Keyword arguments for `model.generate`
     gen_kwargs = generating_args.to_dict()
     gen_kwargs["eos_token_id"] = [tokenizer.eos_token_id] + tokenizer.additional_special_tokens_ids
     gen_kwargs["pad_token_id"] = tokenizer.pad_token_id
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/tuner.py` & `llmtuner-0.7.1/src/llmtuner/train/tuner.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 if TYPE_CHECKING:
     from transformers import TrainerCallback
 
 
 logger = get_logger(__name__)
 
 
-def run_exp(args: Optional[Dict[str, Any]] = None, callbacks: Optional[List["TrainerCallback"]] = None):
+def run_exp(args: Optional[Dict[str, Any]] = None, callbacks: List["TrainerCallback"] = []) -> None:
     model_args, data_args, training_args, finetuning_args, generating_args = get_train_args(args)
-    callbacks = [LogCallback()] if callbacks is None else callbacks
+    callbacks.append(LogCallback(training_args.output_dir))
 
     if finetuning_args.stage == "pt":
         run_pt(model_args, data_args, training_args, finetuning_args, callbacks)
     elif finetuning_args.stage == "sft":
         run_sft(model_args, data_args, training_args, finetuning_args, generating_args, callbacks)
     elif finetuning_args.stage == "rm":
         run_rm(model_args, data_args, training_args, finetuning_args, callbacks)
@@ -39,37 +39,41 @@
         run_dpo(model_args, data_args, training_args, finetuning_args, callbacks)
     elif finetuning_args.stage == "orpo":
         run_orpo(model_args, data_args, training_args, finetuning_args, callbacks)
     else:
         raise ValueError("Unknown task.")
 
 
-def export_model(args: Optional[Dict[str, Any]] = None):
+def export_model(args: Optional[Dict[str, Any]] = None) -> None:
     model_args, data_args, finetuning_args, _ = get_infer_args(args)
 
     if model_args.export_dir is None:
         raise ValueError("Please specify `export_dir` to save model.")
 
     if model_args.adapter_name_or_path is not None and model_args.export_quantization_bit is not None:
         raise ValueError("Please merge adapters before quantizing the model.")
 
-    tokenizer = load_tokenizer(model_args)["tokenizer"]
+    tokenizer_module = load_tokenizer(model_args)
+    tokenizer = tokenizer_module["tokenizer"]
+    processor = tokenizer_module["processor"]
     get_template_and_fix_tokenizer(tokenizer, data_args.template)
     model = load_model(tokenizer, model_args, finetuning_args)  # must after fixing tokenizer to resize vocab
 
     if getattr(model, "quantization_method", None) and model_args.adapter_name_or_path is not None:
         raise ValueError("Cannot merge adapters to a quantized model.")
 
     if not isinstance(model, PreTrainedModel):
         raise ValueError("The model is not a `PreTrainedModel`, export aborted.")
 
     if getattr(model, "quantization_method", None) is None:  # cannot convert dtype of a quantized model
         output_dtype = getattr(model.config, "torch_dtype", torch.float16)
         setattr(model.config, "torch_dtype", output_dtype)
         model = model.to(output_dtype)
+    else:
+        setattr(model.config, "torch_dtype", torch.float16)
 
     model.save_pretrained(
         save_directory=model_args.export_dir,
         max_shard_size="{}GB".format(model_args.export_size),
         safe_serialization=(not model_args.export_legacy_format),
     )
     if model_args.export_hub_model_id is not None:
@@ -82,13 +86,16 @@
 
     try:
         tokenizer.padding_side = "left"  # restore padding side
         tokenizer.init_kwargs["padding_side"] = "left"
         tokenizer.save_pretrained(model_args.export_dir)
         if model_args.export_hub_model_id is not None:
             tokenizer.push_to_hub(model_args.export_hub_model_id, token=model_args.hf_hub_token)
+
+        if model_args.visual_inputs and processor is not None:
+            getattr(processor, "image_processor").save_pretrained(model_args.export_dir)
+            if model_args.export_hub_model_id is not None:
+                getattr(processor, "image_processor").push_to_hub(
+                    model_args.export_hub_model_id, token=model_args.hf_hub_token
+                )
     except Exception:
         logger.warning("Cannot save tokenizer, please copy the files manually.")
-
-
-if __name__ == "__main__":
-    run_exp()
```

### Comparing `llmtuner-0.7.0/src/llmtuner/train/utils.py` & `llmtuner-0.7.1/src/llmtuner/train/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,22 +313,22 @@
         from badam import BlockOptimizer
 
         base_optimizer = optim_class(param_groups, **optim_kwargs)
         optimizer = BlockOptimizer(
             base_optimizer=base_optimizer,
             named_parameters_list=list(model.named_parameters()),
             block_prefix_list=None,
-            switch_block_every=finetuning_args.badam_switch_block_every,
+            switch_block_every=finetuning_args.badam_switch_interval,
             start_block=finetuning_args.badam_start_block,
             switch_mode=finetuning_args.badam_switch_mode,
             verbose=finetuning_args.badam_verbose,
         )
         logger.info(
             f"Using BAdam optimizer with layer-wise update, switch mode is {finetuning_args.badam_switch_mode}, "
-            f"switch block every {finetuning_args.badam_switch_block_every} steps, "
+            f"switch block every {finetuning_args.badam_switch_interval} steps, "
             f"default start block is {finetuning_args.badam_start_block}"
         )
 
     elif finetuning_args.badam_mode == "ratio":
         from badam import BlockOptimizerRatio
 
         assert finetuning_args.badam_update_ratio > 1e-6
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/chatter.py` & `llmtuner-0.7.1/src/llmtuner/webui/chatter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/common.py` & `llmtuner-0.7.1/src/llmtuner/webui/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import json
 import os
 from collections import defaultdict
 from typing import Any, Dict, Optional
 
 from peft.utils import SAFETENSORS_WEIGHTS_NAME, WEIGHTS_NAME
+from yaml import safe_dump, safe_load
 
 from ..extras.constants import (
     DATA_CONFIG,
     DEFAULT_MODULE,
     DEFAULT_TEMPLATE,
-    MLLM_LIST,
     PEFT_METHODS,
     STAGES_USE_PAIR_DATA,
     SUPPORTED_MODELS,
     TRAINING_STAGES,
+    VISION_MODELS,
     DownloadSource,
 )
+from ..extras.logging import get_logger
 from ..extras.misc import use_modelscope
 from ..extras.packages import is_gradio_available
 
 
 if is_gradio_available():
     import gradio as gr
 
 
+logger = get_logger(__name__)
+
+
 ADAPTER_NAMES = {WEIGHTS_NAME, SAFETENSORS_WEIGHTS_NAME}
 DEFAULT_CACHE_DIR = "cache"
 DEFAULT_CONFIG_DIR = "config"
 DEFAULT_DATA_DIR = "data"
 DEFAULT_SAVE_DIR = "saves"
-USER_CONFIG = "user.config"
+USER_CONFIG = "user_config.yaml"
 
 
 def get_save_dir(*args) -> os.PathLike:
     return os.path.join(DEFAULT_SAVE_DIR, *args)
 
 
 def get_config_path() -> os.PathLike:
@@ -43,42 +48,42 @@
 def get_save_path(config_path: str) -> os.PathLike:
     return os.path.join(DEFAULT_CONFIG_DIR, config_path)
 
 
 def load_config() -> Dict[str, Any]:
     try:
         with open(get_config_path(), "r", encoding="utf-8") as f:
-            return json.load(f)
+            return safe_load(f)
     except Exception:
         return {"lang": None, "last_model": None, "path_dict": {}, "cache_dir": None}
 
 
 def save_config(lang: str, model_name: Optional[str] = None, model_path: Optional[str] = None) -> None:
     os.makedirs(DEFAULT_CACHE_DIR, exist_ok=True)
     user_config = load_config()
     user_config["lang"] = lang or user_config["lang"]
     if model_name:
         user_config["last_model"] = model_name
         user_config["path_dict"][model_name] = model_path
     with open(get_config_path(), "w", encoding="utf-8") as f:
-        json.dump(user_config, f, indent=2, ensure_ascii=False)
+        safe_dump(user_config, f)
 
 
 def load_args(config_path: str) -> Optional[Dict[str, Any]]:
     try:
         with open(get_save_path(config_path), "r", encoding="utf-8") as f:
-            return json.load(f)
+            return safe_load(f)
     except Exception:
         return None
 
 
 def save_args(config_path: str, config_dict: Dict[str, Any]) -> str:
     os.makedirs(DEFAULT_CONFIG_DIR, exist_ok=True)
     with open(get_save_path(config_path), "w", encoding="utf-8") as f:
-        json.dump(config_dict, f, indent=2, ensure_ascii=False)
+        safe_dump(config_dict, f)
 
     return str(get_save_path(config_path))
 
 
 def get_model_path(model_name: str) -> str:
     user_config = load_config()
     path_dict: Dict[DownloadSource, str] = SUPPORTED_MODELS.get(model_name, defaultdict(str))
@@ -103,15 +108,15 @@
 def get_template(model_name: str) -> str:
     if model_name and model_name.endswith("Chat") and get_prefix(model_name) in DEFAULT_TEMPLATE:
         return DEFAULT_TEMPLATE[get_prefix(model_name)]
     return "default"
 
 
 def get_visual(model_name: str) -> bool:
-    return get_prefix(model_name) in MLLM_LIST
+    return get_prefix(model_name) in VISION_MODELS
 
 
 def list_adapters(model_name: str, finetuning_type: str) -> "gr.Dropdown":
     if finetuning_type not in PEFT_METHODS:
         return gr.Dropdown(value=[], choices=[], interactive=False)
 
     adapters = []
@@ -123,19 +128,23 @@
                     os.path.isfile(os.path.join(save_dir, adapter, name)) for name in ADAPTER_NAMES
                 ):
                     adapters.append(adapter)
     return gr.Dropdown(value=[], choices=adapters, interactive=True)
 
 
 def load_dataset_info(dataset_dir: str) -> Dict[str, Dict[str, Any]]:
+    if dataset_dir == "ONLINE":
+        logger.info("dataset_dir is ONLINE, using online dataset.")
+        return {}
+
     try:
         with open(os.path.join(dataset_dir, DATA_CONFIG), "r", encoding="utf-8") as f:
             return json.load(f)
     except Exception as err:
-        print("Cannot open {} due to {}.".format(os.path.join(dataset_dir, DATA_CONFIG), str(err)))
+        logger.warning("Cannot open {} due to {}.".format(os.path.join(dataset_dir, DATA_CONFIG), str(err)))
         return {}
 
 
 def list_dataset(dataset_dir: str = None, training_stage: str = list(TRAINING_STAGES.keys())[0]) -> "gr.Dropdown":
     dataset_info = load_dataset_info(dataset_dir if dataset_dir is not None else DEFAULT_DATA_DIR)
     ranking = TRAINING_STAGES[training_stage] in STAGES_USE_PAIR_DATA
     datasets = [k for k, v in dataset_info.items() if v.get("ranking", False) == ranking]
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/components/chatbot.py` & `llmtuner-0.7.1/src/llmtuner/webui/components/chatbot.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,17 +32,17 @@
                     with gr.Column() as image_box:
                         image = gr.Image(sources=["upload"], type="numpy")
 
                 query = gr.Textbox(show_label=False, lines=8)
                 submit_btn = gr.Button(variant="primary")
 
             with gr.Column(scale=1):
-                max_new_tokens = gr.Slider(8, 4096, value=512, step=1)
-                top_p = gr.Slider(0.01, 1.0, value=0.7, step=0.01)
-                temperature = gr.Slider(0.01, 1.5, value=0.95, step=0.01)
+                max_new_tokens = gr.Slider(minimum=8, maximum=4096, value=512, step=1)
+                top_p = gr.Slider(minimum=0.01, maximum=1.0, value=0.7, step=0.01)
+                temperature = gr.Slider(minimum=0.01, maximum=1.5, value=0.95, step=0.01)
                 clear_btn = gr.Button()
 
     tools.input(check_json_schema, inputs=[tools, engine.manager.get_elem_by_id("top.lang")])
 
     submit_btn.click(
         engine.chatter.append,
         [chatbot, messages, role, query],
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/components/data.py` & `llmtuner-0.7.1/src/llmtuner/webui/components/data.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/components/eval.py` & `llmtuner-0.7.1/src/llmtuner/webui/components/eval.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,58 +17,58 @@
 
 def create_eval_tab(engine: "Engine") -> Dict[str, "Component"]:
     input_elems = engine.manager.get_base_elems()
     elem_dict = dict()
 
     with gr.Row():
         dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=2)
-        dataset = gr.Dropdown(multiselect=True, scale=4)
+        dataset = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=4)
         preview_elems = create_preview_box(dataset_dir, dataset)
 
     input_elems.update({dataset_dir, dataset})
     elem_dict.update(dict(dataset_dir=dataset_dir, dataset=dataset, **preview_elems))
 
     with gr.Row():
-        cutoff_len = gr.Slider(value=1024, minimum=4, maximum=8192, step=1)
+        cutoff_len = gr.Slider(minimum=4, maximum=65536, value=1024, step=1)
         max_samples = gr.Textbox(value="100000")
-        batch_size = gr.Slider(value=8, minimum=1, maximum=512, step=1)
+        batch_size = gr.Slider(minimum=1, maximum=1024, value=2, step=1)
         predict = gr.Checkbox(value=True)
 
     input_elems.update({cutoff_len, max_samples, batch_size, predict})
     elem_dict.update(dict(cutoff_len=cutoff_len, max_samples=max_samples, batch_size=batch_size, predict=predict))
 
     with gr.Row():
-        max_new_tokens = gr.Slider(10, 2048, value=128, step=1)
-        top_p = gr.Slider(0.01, 1, value=0.7, step=0.01)
-        temperature = gr.Slider(0.01, 1.5, value=0.95, step=0.01)
+        max_new_tokens = gr.Slider(minimum=8, maximum=4096, value=512, step=1)
+        top_p = gr.Slider(minimum=0.01, maximum=1, value=0.7, step=0.01)
+        temperature = gr.Slider(minimum=0.01, maximum=1.5, value=0.95, step=0.01)
         output_dir = gr.Textbox()
 
     input_elems.update({max_new_tokens, top_p, temperature, output_dir})
     elem_dict.update(dict(max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature, output_dir=output_dir))
 
     with gr.Row():
         cmd_preview_btn = gr.Button()
         start_btn = gr.Button(variant="primary")
         stop_btn = gr.Button(variant="stop")
 
     with gr.Row():
         resume_btn = gr.Checkbox(visible=False, interactive=False)
-        process_bar = gr.Slider(visible=False, interactive=False)
+        progress_bar = gr.Slider(visible=False, interactive=False)
 
     with gr.Row():
         output_box = gr.Markdown()
 
-    output_elems = [output_box, process_bar]
+    output_elems = [output_box, progress_bar]
     elem_dict.update(
         dict(
             cmd_preview_btn=cmd_preview_btn,
             start_btn=start_btn,
             stop_btn=stop_btn,
             resume_btn=resume_btn,
-            process_bar=process_bar,
+            progress_bar=progress_bar,
             output_box=output_box,
         )
     )
 
     cmd_preview_btn.click(engine.runner.preview_eval, input_elems, output_elems, concurrency_limit=None)
     start_btn.click(engine.runner.run_eval, input_elems, output_elems)
     stop_btn.click(engine.runner.set_abort)
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/components/export.py` & `llmtuner-0.7.1/src/llmtuner/webui/components/export.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Dict, Generator, List
 
 from ...extras.misc import torch_gc
 from ...extras.packages import is_gradio_available
-from ...train import export_model
+from ...train.tuner import export_model
 from ..common import get_save_dir
 from ..locales import ALERTS
 
 
 if is_gradio_available():
     import gradio as gr
 
@@ -81,15 +81,15 @@
     export_model(args)
     torch_gc()
     yield ALERTS["info_exported"][lang]
 
 
 def create_export_tab(engine: "Engine") -> Dict[str, "Component"]:
     with gr.Row():
-        export_size = gr.Slider(value=1, minimum=1, maximum=100, step=1)
+        export_size = gr.Slider(minimum=1, maximum=100, value=1, step=1)
         export_quantization_bit = gr.Dropdown(choices=["none", "8", "4", "3", "2"], value="none")
         export_quantization_dataset = gr.Textbox(value="data/c4_demo.json")
         export_device = gr.Radio(choices=["cpu", "cuda"], value="cpu")
         export_legacy_format = gr.Checkbox()
 
     with gr.Row():
         export_dir = gr.Textbox()
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/components/infer.py` & `llmtuner-0.7.1/src/llmtuner/webui/components/infer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/components/top.py` & `llmtuner-0.7.1/src/llmtuner/webui/components/top.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/components/train.py` & `llmtuner-0.7.1/src/llmtuner/webui/components/train.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     elem_dict = dict()
 
     with gr.Row():
         training_stage = gr.Dropdown(
             choices=list(TRAINING_STAGES.keys()), value=list(TRAINING_STAGES.keys())[0], scale=1
         )
         dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=1)
-        dataset = gr.Dropdown(multiselect=True, scale=4)
+        dataset = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=4)
         preview_elems = create_preview_box(dataset_dir, dataset)
 
     input_elems.update({training_stage, dataset_dir, dataset})
     elem_dict.update(dict(training_stage=training_stage, dataset_dir=dataset_dir, dataset=dataset, **preview_elems))
 
     with gr.Row():
         learning_rate = gr.Textbox(value="5e-5")
@@ -48,18 +48,18 @@
             max_grad_norm=max_grad_norm,
             max_samples=max_samples,
             compute_type=compute_type,
         )
     )
 
     with gr.Row():
-        cutoff_len = gr.Slider(value=1024, minimum=4, maximum=16384, step=1)
-        batch_size = gr.Slider(value=2, minimum=1, maximum=1024, step=1)
-        gradient_accumulation_steps = gr.Slider(value=8, minimum=1, maximum=1024, step=1)
-        val_size = gr.Slider(value=0, minimum=0, maximum=1, step=0.001)
+        cutoff_len = gr.Slider(minimum=4, maximum=65536, value=1024, step=1)
+        batch_size = gr.Slider(minimum=1, maximum=1024, value=2, step=1)
+        gradient_accumulation_steps = gr.Slider(minimum=1, maximum=1024, value=8, step=1)
+        val_size = gr.Slider(minimum=0, maximum=1, value=0, step=0.001)
         lr_scheduler_type = gr.Dropdown(choices=[scheduler.value for scheduler in SchedulerType], value="cosine")
 
     input_elems.update({cutoff_len, batch_size, gradient_accumulation_steps, val_size, lr_scheduler_type})
     elem_dict.update(
         dict(
             cutoff_len=cutoff_len,
             batch_size=batch_size,
@@ -67,18 +67,18 @@
             val_size=val_size,
             lr_scheduler_type=lr_scheduler_type,
         )
     )
 
     with gr.Accordion(open=False) as extra_tab:
         with gr.Row():
-            logging_steps = gr.Slider(value=5, minimum=5, maximum=1000, step=5)
-            save_steps = gr.Slider(value=100, minimum=10, maximum=5000, step=10)
-            warmup_steps = gr.Slider(value=0, minimum=0, maximum=5000, step=1)
-            neftune_alpha = gr.Slider(value=0, minimum=0, maximum=10, step=0.1)
+            logging_steps = gr.Slider(minimum=1, maximum=1000, value=5, step=5)
+            save_steps = gr.Slider(minimum=10, maximum=5000, value=100, step=10)
+            warmup_steps = gr.Slider(minimum=0, maximum=5000, value=0, step=1)
+            neftune_alpha = gr.Slider(minimum=0, maximum=10, value=0, step=0.1)
             optim = gr.Textbox(value="adamw_torch")
 
         with gr.Row():
             with gr.Column():
                 resize_vocab = gr.Checkbox()
                 packing = gr.Checkbox()
 
@@ -120,30 +120,34 @@
             shift_attn=shift_attn,
             report_to=report_to,
         )
     )
 
     with gr.Accordion(open=False) as freeze_tab:
         with gr.Row():
-            num_layer_trainable = gr.Slider(value=3, minimum=1, maximum=128, step=1)
-            name_module_trainable = gr.Textbox(value="all")
+            freeze_trainable_layers = gr.Slider(minimum=-128, maximum=128, value=2, step=1)
+            freeze_trainable_modules = gr.Textbox(value="all")
+            freeze_extra_modules = gr.Textbox()
 
-    input_elems.update({num_layer_trainable, name_module_trainable})
+    input_elems.update({freeze_trainable_layers, freeze_trainable_modules, freeze_extra_modules})
     elem_dict.update(
         dict(
-            freeze_tab=freeze_tab, num_layer_trainable=num_layer_trainable, name_module_trainable=name_module_trainable
+            freeze_tab=freeze_tab,
+            freeze_trainable_layers=freeze_trainable_layers,
+            freeze_trainable_modules=freeze_trainable_modules,
+            freeze_extra_modules=freeze_extra_modules,
         )
     )
 
     with gr.Accordion(open=False) as lora_tab:
         with gr.Row():
-            lora_rank = gr.Slider(value=8, minimum=1, maximum=1024, step=1)
-            lora_alpha = gr.Slider(value=16, minimum=1, maximum=2048, step=1)
-            lora_dropout = gr.Slider(value=0, minimum=0, maximum=1, step=0.01)
-            loraplus_lr_ratio = gr.Slider(value=0, minimum=0, maximum=64, step=0.01)
+            lora_rank = gr.Slider(minimum=1, maximum=1024, value=8, step=1)
+            lora_alpha = gr.Slider(minimum=1, maximum=2048, value=16, step=1)
+            lora_dropout = gr.Slider(minimum=0, maximum=1, value=0, step=0.01)
+            loraplus_lr_ratio = gr.Slider(minimum=0, maximum=64, value=0, step=0.01)
             create_new_adapter = gr.Checkbox()
 
         with gr.Row():
             with gr.Column(scale=1):
                 use_rslora = gr.Checkbox()
                 use_dora = gr.Checkbox()
 
@@ -176,44 +180,64 @@
             lora_target=lora_target,
             additional_target=additional_target,
         )
     )
 
     with gr.Accordion(open=False) as rlhf_tab:
         with gr.Row():
-            dpo_beta = gr.Slider(value=0.1, minimum=0, maximum=1, step=0.01)
-            dpo_ftx = gr.Slider(value=0, minimum=0, maximum=10, step=0.01)
-            orpo_beta = gr.Slider(value=0.1, minimum=0, maximum=1, step=0.01)
+            dpo_beta = gr.Slider(minimum=0, maximum=1, value=0.1, step=0.01)
+            dpo_ftx = gr.Slider(minimum=0, maximum=10, value=0, step=0.01)
+            orpo_beta = gr.Slider(minimum=0, maximum=1, value=0.1, step=0.01)
             reward_model = gr.Dropdown(multiselect=True, allow_custom_value=True)
 
     input_elems.update({dpo_beta, dpo_ftx, orpo_beta, reward_model})
     elem_dict.update(
         dict(rlhf_tab=rlhf_tab, dpo_beta=dpo_beta, dpo_ftx=dpo_ftx, orpo_beta=orpo_beta, reward_model=reward_model)
     )
 
     with gr.Accordion(open=False) as galore_tab:
         with gr.Row():
             use_galore = gr.Checkbox()
-            galore_rank = gr.Slider(value=16, minimum=1, maximum=1024, step=1)
-            galore_update_interval = gr.Slider(value=200, minimum=1, maximum=1024, step=1)
-            galore_scale = gr.Slider(value=0.25, minimum=0, maximum=1, step=0.01)
+            galore_rank = gr.Slider(minimum=1, maximum=1024, value=16, step=1)
+            galore_update_interval = gr.Slider(minimum=1, maximum=1024, value=200, step=1)
+            galore_scale = gr.Slider(minimum=0, maximum=1, value=0.25, step=0.01)
             galore_target = gr.Textbox(value="all")
 
     input_elems.update({use_galore, galore_rank, galore_update_interval, galore_scale, galore_target})
     elem_dict.update(
         dict(
             galore_tab=galore_tab,
             use_galore=use_galore,
             galore_rank=galore_rank,
             galore_update_interval=galore_update_interval,
             galore_scale=galore_scale,
             galore_target=galore_target,
         )
     )
 
+    with gr.Accordion(open=False) as badam_tab:
+        with gr.Row():
+            use_badam = gr.Checkbox()
+            badam_mode = gr.Dropdown(choices=["layer", "ratio"], value="layer")
+            badam_switch_mode = gr.Dropdown(choices=["ascending", "descending", "random", "fixed"], value="ascending")
+            badam_switch_interval = gr.Slider(minimum=1, maximum=1024, value=50, step=1)
+            badam_update_ratio = gr.Slider(minimum=0, maximum=1, value=0.05, step=0.01)
+
+    input_elems.update({use_badam, badam_mode, badam_switch_mode, badam_switch_interval, badam_update_ratio})
+    elem_dict.update(
+        dict(
+            badam_tab=badam_tab,
+            use_badam=use_badam,
+            badam_mode=badam_mode,
+            badam_switch_mode=badam_switch_mode,
+            badam_switch_interval=badam_switch_interval,
+            badam_update_ratio=badam_update_ratio,
+        )
+    )
+
     with gr.Row():
         cmd_preview_btn = gr.Button()
         arg_save_btn = gr.Button()
         arg_load_btn = gr.Button()
         start_btn = gr.Button(variant="primary")
         stop_btn = gr.Button(variant="stop")
 
@@ -221,15 +245,15 @@
         with gr.Column(scale=3):
             with gr.Row():
                 output_dir = gr.Textbox()
                 config_path = gr.Textbox()
 
             with gr.Row():
                 resume_btn = gr.Checkbox(visible=False, interactive=False)
-                process_bar = gr.Slider(visible=False, interactive=False)
+                progress_bar = gr.Slider(visible=False, interactive=False)
 
             with gr.Row():
                 output_box = gr.Markdown()
 
         with gr.Column(scale=1):
             loss_viewer = gr.Plot()
 
@@ -239,22 +263,22 @@
             arg_save_btn=arg_save_btn,
             arg_load_btn=arg_load_btn,
             start_btn=start_btn,
             stop_btn=stop_btn,
             output_dir=output_dir,
             config_path=config_path,
             resume_btn=resume_btn,
-            process_bar=process_bar,
+            progress_bar=progress_bar,
             output_box=output_box,
             loss_viewer=loss_viewer,
         )
     )
 
     input_elems.update({output_dir, config_path})
-    output_elems = [output_box, process_bar, loss_viewer]
+    output_elems = [output_box, progress_bar, loss_viewer]
 
     cmd_preview_btn.click(engine.runner.preview_train, input_elems, output_elems, concurrency_limit=None)
     arg_save_btn.click(engine.runner.save_args, input_elems, output_elems, concurrency_limit=None)
     arg_load_btn.click(
         engine.runner.load_args,
         [engine.manager.get_elem_by_id("top.lang"), config_path],
         list(input_elems) + [output_box],
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/css.py` & `llmtuner-0.7.1/src/llmtuner/webui/css.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/engine.py` & `llmtuner-0.7.1/src/llmtuner/webui/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 
         init_dict = {"top.lang": {"value": lang}, "infer.chat_box": {"visible": self.chatter.loaded}}
 
         if not self.pure_chat:
             init_dict["train.dataset"] = {"choices": list_dataset().choices}
             init_dict["eval.dataset"] = {"choices": list_dataset().choices}
             init_dict["train.output_dir"] = {"value": "train_{}".format(get_time())}
-            init_dict["train.config_path"] = {"value": "{}.json".format(get_time())}
+            init_dict["train.config_path"] = {"value": "{}.yaml".format(get_time())}
             init_dict["eval.output_dir"] = {"value": "eval_{}".format(get_time())}
             init_dict["infer.image_box"] = {"visible": False}
 
             if user_config.get("last_model", None):
                 init_dict["top.model_name"] = {"value": user_config["last_model"]}
                 init_dict["top.model_path"] = {"value": get_model_path(user_config["last_model"])}
 
         yield self._update_component(init_dict)
 
-        if self.runner.alive and not self.demo_mode and not self.pure_chat:
+        if self.runner.running and not self.demo_mode and not self.pure_chat:
             yield {elem: elem.__class__(value=value) for elem, value in self.runner.running_data.items()}
             if self.runner.do_train:
                 yield self._update_component({"train.resume_btn": {"value": True}})
             else:
                 yield self._update_component({"eval.resume_btn": {"value": True}})
 
     def change_lang(self, lang: str):
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/locales.py` & `llmtuner-0.7.1/src/llmtuner/webui/locales.py`

 * *Files 4% similar despite different names*

```diff
@@ -568,42 +568,62 @@
         "ru": {
             "label": "конфигурации для настройки заморозки",
         },
         "zh": {
             "label": "部分参数微调设置",
         },
     },
-    "num_layer_trainable": {
+    "freeze_trainable_layers": {
         "en": {
             "label": "Trainable layers",
-            "info": "The number of trainable layers.",
+            "info": "Number of the last(+)/first(-) hidden layers to be set as trainable.",
         },
         "ru": {
             "label": "Обучаемые слои",
-            "info": "Количество обучаемых слоев.",
+            "info": "Количество последних (+)/первых (-) скрытых слоев, которые будут установлены как обучаемые.",
         },
         "zh": {
             "label": "可训练层数",
-            "info": "可训练模型层的数量。",
+            "info": "最末尾（+）/最前端（-）可训练隐藏层的数量。",
         },
     },
-    "name_module_trainable": {
+    "freeze_trainable_modules": {
         "en": {
             "label": "Trainable modules",
-            "info": "The name of trainable modules. Use commas to separate multiple modules.",
+            "info": "Name(s) of trainable modules. Use commas to separate multiple modules.",
         },
         "ru": {
             "label": "Обучаемые модули",
             "info": "Название обучаемых модулей. Используйте запятые для разделения нескольких модулей.",
         },
         "zh": {
             "label": "可训练模块",
             "info": "可训练模块的名称。使用英文逗号分隔多个名称。",
         },
     },
+    "freeze_extra_modules": {
+        "en": {
+            "label": "Extra modules (optional)",
+            "info": (
+                "Name(s) of modules apart from hidden layers to be set as trainable. "
+                "Use commas to separate multiple modules."
+            ),
+        },
+        "ru": {
+            "label": "Дополнительные модули (опционально)",
+            "info": (
+                "Имена модулей, кроме скрытых слоев, которые следует установить в качестве обучаемых. "
+                "Используйте запятые для разделения нескольких модулей."
+            ),
+        },
+        "zh": {
+            "label": "额外模块（非必填）",
+            "info": "除隐藏层以外的可训练模块名称。使用英文逗号分隔多个名称。",
+        },
+    },
     "lora_tab": {
         "en": {
             "label": "LoRA configurations",
         },
         "ru": {
             "label": "Конфигурации LoRA",
         },
@@ -887,14 +907,95 @@
             "info": "Имена модулей для применения GaLore. Используйте запятые для разделения нескольких модулей.",
         },
         "zh": {
             "label": "GaLore 作用模块",
             "info": "应用 GaLore 的模块名称。使用英文逗号分隔多个名称。",
         },
     },
+    "badam_tab": {
+        "en": {
+            "label": "BAdam configurations",
+        },
+        "ru": {
+            "label": "Конфигурации BAdam",
+        },
+        "zh": {
+            "label": "BAdam 参数设置",
+        },
+    },
+    "use_badam": {
+        "en": {
+            "label": "Use BAdam",
+            "info": "Enable the BAdam optimizer.",
+        },
+        "ru": {
+            "label": "Использовать BAdam",
+            "info": "Включите оптимизатор BAdam.",
+        },
+        "zh": {
+            "label": "使用 BAdam",
+            "info": "使用 BAdam 优化器。",
+        },
+    },
+    "badam_mode": {
+        "en": {
+            "label": "BAdam mode",
+            "info": "Whether to use layer-wise or ratio-wise BAdam optimizer.",
+        },
+        "ru": {
+            "label": "Режим BAdam",
+            "info": "Использовать ли оптимизатор BAdam с послоевой или пропорциональной настройкой.",
+        },
+        "zh": {
+            "label": "BAdam 模式",
+            "info": "使用 layer-wise 或 ratio-wise BAdam 优化器。",
+        },
+    },
+    "badam_switch_mode": {
+        "en": {
+            "label": "Switch mode",
+            "info": "The strategy of picking block to update for layer-wise BAdam.",
+        },
+        "ru": {
+            "label": "Режим переключения",
+            "info": "Стратегия выбора блока для обновления для послойного BAdam.",
+        },
+        "zh": {
+            "label": "切换策略",
+            "info": "Layer-wise BAdam 优化器的块切换策略。",
+        },
+    },
+    "badam_switch_interval": {
+        "en": {
+            "label": "Switch interval",
+            "info": "Number of steps to update the block for layer-wise BAdam.",
+        },
+        "ru": {
+            "label": "Интервал переключения",
+            "info": "количество шагов для обновления блока для пошагового BAdam.",
+        },
+        "zh": {
+            "label": "切换频率",
+            "info": "Layer-wise BAdam 优化器的块切换频率。",
+        },
+    },
+    "badam_update_ratio": {
+        "en": {
+            "label": "Update ratio",
+            "info": "The ratio of the update for ratio-wise BAdam.",
+        },
+        "ru": {
+            "label": "Коэффициент обновления",
+            "info": "Коэффициент обновления для BAdam с учётом соотношений.",
+        },
+        "zh": {
+            "label": "Block 更新比例",
+            "info": "Ratio-wise BAdam 优化器的更新比例。",
+        },
+    },
     "cmd_preview_btn": {
         "en": {
             "value": "Preview command",
         },
         "ru": {
             "value": "Просмотр команды",
         },
@@ -1364,15 +1465,15 @@
         "en": "CUDA environment was not detected.",
         "ru": "Среда CUDA не обнаружена.",
         "zh": "未检测到 CUDA 环境。",
     },
     "info_aborting": {
         "en": "Aborted, wait for terminating...",
         "ru": "Прервано, ожидание завершения...",
-        "zh": "训练中断，正在等待线程结束……",
+        "zh": "训练中断，正在等待进程结束……",
     },
     "info_aborted": {
         "en": "Ready.",
         "ru": "Готово.",
         "zh": "准备就绪。",
     },
     "info_finished": {
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/manager.py` & `llmtuner-0.7.1/src/llmtuner/webui/manager.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/runner.py` & `llmtuner-0.7.1/src/llmtuner/webui/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-import logging
 import os
-import time
-from threading import Thread
-from typing import TYPE_CHECKING, Any, Dict, Generator
+import signal
+from copy import deepcopy
+from subprocess import Popen, TimeoutExpired
+from typing import TYPE_CHECKING, Any, Dict, Generator, Optional
 
-import transformers
+import psutil
 from transformers.trainer import TRAINING_ARGS_NAME
 from transformers.utils import is_torch_cuda_available
 
-from ..extras.callbacks import LogCallback
 from ..extras.constants import TRAINING_STAGES
-from ..extras.logging import LoggerHandler
 from ..extras.misc import get_device_count, torch_gc
 from ..extras.packages import is_gradio_available
-from ..train import run_exp
 from .common import get_module, get_save_dir, load_args, load_config, save_args
 from .locales import ALERTS
-from .utils import gen_cmd, gen_plot, get_eval_results, update_process_bar
+from .utils import gen_cmd, get_eval_results, get_trainer_info, save_cmd
 
 
 if is_gradio_available():
     import gradio as gr
 
 
 if TYPE_CHECKING:
@@ -30,32 +27,26 @@
 
 
 class Runner:
     def __init__(self, manager: "Manager", demo_mode: bool = False) -> None:
         self.manager = manager
         self.demo_mode = demo_mode
         """ Resume """
-        self.thread: "Thread" = None
+        self.trainer: Optional["Popen"] = None
         self.do_train = True
         self.running_data: Dict["Component", Any] = None
         """ State """
         self.aborted = False
         self.running = False
-        """ Handler """
-        self.logger_handler = LoggerHandler()
-        self.logger_handler.setLevel(logging.INFO)
-        logging.root.addHandler(self.logger_handler)
-        transformers.logging.add_handler(self.logger_handler)
-
-    @property
-    def alive(self) -> bool:
-        return self.thread is not None
 
     def set_abort(self) -> None:
         self.aborted = True
+        if self.trainer is not None:
+            for children in psutil.Process(self.trainer.pid).children():  # abort the child process
+                os.kill(children.pid, signal.SIGABRT)
 
     def _initialize(self, data: Dict["Component", Any], do_train: bool, from_preview: bool) -> str:
         get = lambda elem_id: data[self.manager.get_elem_by_id(elem_id)]
         lang, model_name, model_path = get("top.lang"), get("top.model_name"), get("top.model_path")
         dataset = get("train.dataset") if do_train else get("eval.dataset")
 
         if self.running:
@@ -81,21 +72,19 @@
             reward_model = get("train.reward_model")
             if stage == "ppo" and not reward_model:
                 return ALERTS["err_no_reward_model"][lang]
 
         if not from_preview and not is_torch_cuda_available():
             gr.Warning(ALERTS["warn_no_cuda"][lang])
 
-        self.logger_handler.reset()
-        self.trainer_callback = LogCallback(self)
         return ""
 
     def _finalize(self, lang: str, finish_info: str) -> str:
         finish_info = ALERTS["info_aborted"][lang] if self.aborted else finish_info
-        self.thread = None
+        self.trainer = None
         self.aborted = False
         self.running = False
         self.running_data = None
         torch_gc()
         return finish_info
 
     def _parse_train_args(self, data: Dict["Component", Any]) -> Dict[str, Any]:
@@ -114,14 +103,15 @@
 
         args = dict(
             stage=TRAINING_STAGES[get("train.training_stage")],
             do_train=True,
             model_name_or_path=get("top.model_path"),
             adapter_name_or_path=adapter_name_or_path,
             cache_dir=user_config.get("cache_dir", None),
+            preprocessing_num_workers=16,
             finetuning_type=get("top.finetuning_type"),
             quantization_bit=int(get("top.quantization_bit")) if get("top.quantization_bit") in ["8", "4"] else None,
             template=get("top.template"),
             rope_scaling=get("top.rope_scaling") if get("top.rope_scaling") in ["linear", "dynamic"] else None,
             flash_attn="fa2" if get("top.booster") == "flashattn2" else "auto",
             use_unsloth=(get("top.booster") == "unsloth"),
             visual_inputs=get("top.visual_inputs"),
@@ -143,24 +133,26 @@
             resize_vocab=get("train.resize_vocab"),
             packing=get("train.packing"),
             upcast_layernorm=get("train.upcast_layernorm"),
             use_llama_pro=get("train.use_llama_pro"),
             shift_attn=get("train.shift_attn"),
             report_to="all" if get("train.report_to") else "none",
             use_galore=get("train.use_galore"),
+            use_badam=get("train.use_badam"),
             output_dir=get_save_dir(get("top.model_name"), get("top.finetuning_type"), get("train.output_dir")),
             fp16=(get("train.compute_type") == "fp16"),
             bf16=(get("train.compute_type") == "bf16"),
             pure_bf16=(get("train.compute_type") == "pure_bf16"),
+            plot_loss=True,
         )
-        args["disable_tqdm"] = True
 
         if args["finetuning_type"] == "freeze":
-            args["num_layer_trainable"] = get("train.num_layer_trainable")
-            args["name_module_trainable"] = get("train.name_module_trainable")
+            args["freeze_trainable_layers"] = get("train.freeze_trainable_layers")
+            args["freeze_trainable_modules"] = get("train.freeze_trainable_modules")
+            args["freeze_extra_modules"] = get("train.freeze_extra_modules") or None
         elif args["finetuning_type"] == "lora":
             args["lora_rank"] = get("train.lora_rank")
             args["lora_alpha"] = get("train.lora_alpha")
             args["lora_dropout"] = get("train.lora_dropout")
             args["loraplus_lr_ratio"] = get("train.loraplus_lr_ratio") or None
             args["create_new_adapter"] = get("train.create_new_adapter")
             args["use_rslora"] = get("train.use_rslora")
@@ -194,14 +186,20 @@
 
         if args["use_galore"]:
             args["galore_rank"] = get("train.galore_rank")
             args["galore_update_interval"] = get("train.galore_update_interval")
             args["galore_scale"] = get("train.galore_scale")
             args["galore_target"] = get("train.galore_target")
 
+        if args["use_badam"]:
+            args["badam_mode"] = get("train.badam_mode")
+            args["badam_switch_mode"] = get("train.badam_switch_mode")
+            args["badam_switch_interval"] = get("train.badam_switch_interval")
+            args["badam_update_ratio"] = get("train.badam_update_ratio")
+
         return args
 
     def _parse_eval_args(self, data: Dict["Component", Any]) -> Dict[str, Any]:
         get = lambda elem_id: data[self.manager.get_elem_by_id(elem_id)]
         user_config = load_config()
 
         if get("top.adapter_path"):
@@ -215,14 +213,15 @@
             adapter_name_or_path = None
 
         args = dict(
             stage="sft",
             model_name_or_path=get("top.model_path"),
             adapter_name_or_path=adapter_name_or_path,
             cache_dir=user_config.get("cache_dir", None),
+            preprocessing_num_workers=16,
             finetuning_type=get("top.finetuning_type"),
             quantization_bit=int(get("top.quantization_bit")) if get("top.quantization_bit") in ["8", "4"] else None,
             template=get("top.template"),
             rope_scaling=get("top.rope_scaling") if get("top.rope_scaling") in ["linear", "dynamic"] else None,
             flash_attn="fa2" if get("top.booster") == "flashattn2" else "auto",
             use_unsloth=(get("top.booster") == "unsloth"),
             visual_inputs=get("top.visual_inputs"),
@@ -233,15 +232,14 @@
             per_device_eval_batch_size=get("eval.batch_size"),
             predict_with_generate=True,
             max_new_tokens=get("eval.max_new_tokens"),
             top_p=get("eval.top_p"),
             temperature=get("eval.temperature"),
             output_dir=get_save_dir(get("top.model_name"), get("top.finetuning_type"), get("eval.output_dir")),
         )
-        args["disable_tqdm"] = True
 
         if get("eval.predict"):
             args["do_predict"] = True
         else:
             args["do_eval"] = True
 
         return args
@@ -259,19 +257,20 @@
     def _launch(self, data: Dict["Component", Any], do_train: bool) -> Generator[Dict["Component", Any], None, None]:
         output_box = self.manager.get_elem_by_id("{}.output_box".format("train" if do_train else "eval"))
         error = self._initialize(data, do_train, from_preview=False)
         if error:
             gr.Warning(error)
             yield {output_box: error}
         else:
-            args = self._parse_train_args(data) if do_train else self._parse_eval_args(data)
-            run_kwargs = dict(args=args, callbacks=[self.trainer_callback])
             self.do_train, self.running_data = do_train, data
-            self.thread = Thread(target=run_exp, kwargs=run_kwargs)
-            self.thread.start()
+            args = self._parse_train_args(data) if do_train else self._parse_eval_args(data)
+            env = deepcopy(os.environ)
+            env["CUDA_VISIBLE_DEVICES"] = os.environ.get("CUDA_VISIBLE_DEVICES", "0")
+            env["LLAMABOARD_ENABLED"] = "1"
+            self.trainer = Popen("llamafactory-cli train {}".format(save_cmd(args)), env=env, shell=True)
             yield from self.monitor()
 
     def preview_train(self, data):
         yield from self._preview(data, do_train=True)
 
     def preview_eval(self, data):
         yield from self._preview(data, do_train=False)
@@ -279,71 +278,69 @@
     def run_train(self, data):
         yield from self._launch(data, do_train=True)
 
     def run_eval(self, data):
         yield from self._launch(data, do_train=False)
 
     def monitor(self):
-        get = lambda elem_id: self.running_data[self.manager.get_elem_by_id(elem_id)]
         self.aborted = False
         self.running = True
 
+        get = lambda elem_id: self.running_data[self.manager.get_elem_by_id(elem_id)]
         lang = get("top.lang")
         model_name = get("top.model_name")
         finetuning_type = get("top.finetuning_type")
         output_dir = get("{}.output_dir".format("train" if self.do_train else "eval"))
         output_path = get_save_dir(model_name, finetuning_type, output_dir)
 
         output_box = self.manager.get_elem_by_id("{}.output_box".format("train" if self.do_train else "eval"))
-        process_bar = self.manager.get_elem_by_id("{}.process_bar".format("train" if self.do_train else "eval"))
+        progress_bar = self.manager.get_elem_by_id("{}.progress_bar".format("train" if self.do_train else "eval"))
         loss_viewer = self.manager.get_elem_by_id("train.loss_viewer") if self.do_train else None
 
-        while self.thread is not None and self.thread.is_alive():
+        while self.trainer is not None:
             if self.aborted:
                 yield {
                     output_box: ALERTS["info_aborting"][lang],
-                    process_bar: gr.Slider(visible=False),
+                    progress_bar: gr.Slider(visible=False),
                 }
             else:
+                running_log, running_progress, running_loss = get_trainer_info(output_path, self.do_train)
                 return_dict = {
-                    output_box: self.logger_handler.log,
-                    process_bar: update_process_bar(self.trainer_callback),
+                    output_box: running_log,
+                    progress_bar: running_progress,
                 }
-                if self.do_train:
-                    plot = gen_plot(output_path)
-                    if plot is not None:
-                        return_dict[loss_viewer] = plot
+                if running_loss is not None:
+                    return_dict[loss_viewer] = running_loss
 
                 yield return_dict
 
-            time.sleep(2)
+            try:
+                self.trainer.wait(2)
+                self.trainer = None
+            except TimeoutExpired:
+                continue
 
         if self.do_train:
             if os.path.exists(os.path.join(output_path, TRAINING_ARGS_NAME)):
                 finish_info = ALERTS["info_finished"][lang]
             else:
                 finish_info = ALERTS["err_failed"][lang]
         else:
             if os.path.exists(os.path.join(output_path, "all_results.json")):
                 finish_info = get_eval_results(os.path.join(output_path, "all_results.json"))
             else:
                 finish_info = ALERTS["err_failed"][lang]
 
         return_dict = {
             output_box: self._finalize(lang, finish_info),
-            process_bar: gr.Slider(visible=False),
+            progress_bar: gr.Slider(visible=False),
         }
-        if self.do_train:
-            plot = gen_plot(output_path)
-            if plot is not None:
-                return_dict[loss_viewer] = plot
-
         yield return_dict
 
-    def save_args(self, data):
+    def save_args(self, data: dict):
         output_box = self.manager.get_elem_by_id("train.output_box")
         error = self._initialize(data, do_train=True, from_preview=True)
         if error:
             gr.Warning(error)
             return {output_box: error}
 
         config_dict: Dict[str, Any] = {}
```

### Comparing `llmtuner-0.7.0/src/llmtuner/webui/utils.py` & `llmtuner-0.7.1/src/llmtuner/extras/ploting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,87 @@
 import json
+import math
 import os
-from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import Any, Dict, List
 
-from ..extras.packages import is_gradio_available, is_matplotlib_available
-from ..extras.ploting import smooth
-from .locales import ALERTS
+from transformers.trainer import TRAINER_STATE_NAME
 
-
-if is_gradio_available():
-    import gradio as gr
+from .logging import get_logger
+from .packages import is_matplotlib_available
 
 
 if is_matplotlib_available():
     import matplotlib.figure
     import matplotlib.pyplot as plt
 
 
-if TYPE_CHECKING:
-    from ..extras.callbacks import LogCallback
-
+logger = get_logger(__name__)
 
-def update_process_bar(callback: "LogCallback") -> "gr.Slider":
-    if not callback.max_steps:
-        return gr.Slider(visible=False)
-
-    percentage = round(100 * callback.cur_steps / callback.max_steps, 0) if callback.max_steps != 0 else 100.0
-    label = "Running {:d}/{:d}: {} < {}".format(
-        callback.cur_steps, callback.max_steps, callback.elapsed_time, callback.remaining_time
-    )
-    return gr.Slider(label=label, value=percentage, visible=True)
-
-
-def get_time() -> str:
-    return datetime.now().strftime(r"%Y-%m-%d-%H-%M-%S")
-
-
-def can_quantize(finetuning_type: str) -> "gr.Dropdown":
-    if finetuning_type != "lora":
-        return gr.Dropdown(value="none", interactive=False)
-    else:
-        return gr.Dropdown(interactive=True)
-
-
-def check_json_schema(text: str, lang: str) -> None:
-    try:
-        tools = json.loads(text)
-        if tools:
-            assert isinstance(tools, list)
-            for tool in tools:
-                if "name" not in tool:
-                    raise NotImplementedError("Name not found.")
-    except NotImplementedError:
-        gr.Warning(ALERTS["err_tool_name"][lang])
-    except Exception:
-        gr.Warning(ALERTS["err_json_schema"][lang])
-
-
-def gen_cmd(args: Dict[str, Any]) -> str:
-    args.pop("disable_tqdm", None)
-    args["plot_loss"] = args.get("do_train", None)
-    current_devices = os.environ.get("CUDA_VISIBLE_DEVICES", "0")
-    cmd_lines = ["CUDA_VISIBLE_DEVICES={} python src/train_bash.py ".format(current_devices)]
-    for k, v in args.items():
-        if v is not None and v is not False and v != "":
-            cmd_lines.append("    --{} {} ".format(k, str(v)))
-    cmd_text = "\\\n".join(cmd_lines)
-    cmd_text = "```bash\n{}\n```".format(cmd_text)
-    return cmd_text
-
-
-def get_eval_results(path: os.PathLike) -> str:
-    with open(path, "r", encoding="utf-8") as f:
-        result = json.dumps(json.load(f), indent=4)
-    return "```json\n{}\n```\n".format(result)
-
-
-def gen_plot(output_path: str) -> Optional["matplotlib.figure.Figure"]:
-    log_file = os.path.join(output_path, "trainer_log.jsonl")
-    if not os.path.isfile(log_file) or not is_matplotlib_available():
-        return
 
+def smooth(scalars: List[float]) -> List[float]:
+    r"""
+    EMA implementation according to TensorBoard.
+    """
+    if len(scalars) == 0:
+        return []
+
+    last = scalars[0]
+    smoothed = []
+    weight = 1.8 * (1 / (1 + math.exp(-0.05 * len(scalars))) - 0.5)  # a sigmoid function
+    for next_val in scalars:
+        smoothed_val = last * weight + (1 - weight) * next_val
+        smoothed.append(smoothed_val)
+        last = smoothed_val
+    return smoothed
+
+
+def gen_loss_plot(trainer_log: List[Dict[str, Any]]) -> "matplotlib.figure.Figure":
+    r"""
+    Plots loss curves in LlamaBoard.
+    """
     plt.close("all")
     plt.switch_backend("agg")
     fig = plt.figure()
     ax = fig.add_subplot(111)
     steps, losses = [], []
-    with open(log_file, "r", encoding="utf-8") as f:
-        for line in f:
-            log_info: Dict[str, Any] = json.loads(line)
-            if log_info.get("loss", None):
-                steps.append(log_info["current_steps"])
-                losses.append(log_info["loss"])
-
-    if len(losses) == 0:
-        return
+    for log in trainer_log:
+        if log.get("loss", None):
+            steps.append(log["current_steps"])
+            losses.append(log["loss"])
 
     ax.plot(steps, losses, color="#1f77b4", alpha=0.4, label="original")
     ax.plot(steps, smooth(losses), color="#1f77b4", label="smoothed")
     ax.legend()
     ax.set_xlabel("step")
     ax.set_ylabel("loss")
     return fig
+
+
+def plot_loss(save_dictionary: os.PathLike, keys: List[str] = ["loss"]) -> None:
+    r"""
+    Plots loss curves and saves the image.
+    """
+    plt.switch_backend("agg")
+    with open(os.path.join(save_dictionary, TRAINER_STATE_NAME), "r", encoding="utf-8") as f:
+        data = json.load(f)
+
+    for key in keys:
+        steps, metrics = [], []
+        for i in range(len(data["log_history"])):
+            if key in data["log_history"][i]:
+                steps.append(data["log_history"][i]["step"])
+                metrics.append(data["log_history"][i][key])
+
+        if len(metrics) == 0:
+            logger.warning(f"No metric {key} to plot.")
+            continue
+
+        plt.figure()
+        plt.plot(steps, metrics, color="#1f77b4", alpha=0.4, label="original")
+        plt.plot(steps, smooth(metrics), color="#1f77b4", label="smoothed")
+        plt.title("training {} of {}".format(key, save_dictionary))
+        plt.xlabel("step")
+        plt.ylabel(key)
+        plt.legend()
+        figure_path = os.path.join(save_dictionary, "training_{}.png".format(key.replace("/", "_")))
+        plt.savefig(figure_path, format="png", dpi=100)
+        print("Figure saved at:", figure_path)
```

### Comparing `llmtuner-0.7.0/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.7.1/src/llmtuner.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.7.0
+Version: 0.7.1
 Summary: Easy-to-use LLM fine-tuning framework
 Home-page: https://github.com/hiyouga/LLaMA-Factory
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -17,77 +17,46 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch>=1.13.1
-Requires-Dist: transformers>=4.37.2
-Requires-Dist: datasets>=2.14.3
-Requires-Dist: accelerate>=0.27.2
-Requires-Dist: peft>=0.10.0
-Requires-Dist: trl>=0.8.1
-Requires-Dist: gradio>=4.0.0
-Requires-Dist: scipy
-Requires-Dist: einops
-Requires-Dist: sentencepiece
-Requires-Dist: protobuf
-Requires-Dist: uvicorn
-Requires-Dist: pydantic
-Requires-Dist: fastapi
-Requires-Dist: sse-starlette
-Requires-Dist: matplotlib
-Requires-Dist: fire
-Requires-Dist: packaging
-Provides-Extra: deepspeed
-Requires-Dist: deepspeed>=0.10.0; extra == "deepspeed"
+Provides-Extra: torch
 Provides-Extra: metrics
-Requires-Dist: nltk; extra == "metrics"
-Requires-Dist: jieba; extra == "metrics"
-Requires-Dist: rouge-chinese; extra == "metrics"
+Provides-Extra: deepspeed
+Provides-Extra: bitsandbytes
+Provides-Extra: vllm
 Provides-Extra: galore
-Requires-Dist: galore-torch; extra == "galore"
 Provides-Extra: badam
-Requires-Dist: badam; extra == "badam"
-Provides-Extra: vllm
-Requires-Dist: vllm>=0.4.0; extra == "vllm"
-Provides-Extra: bitsandbytes
-Requires-Dist: bitsandbytes>=0.39.0; extra == "bitsandbytes"
 Provides-Extra: gptq
-Requires-Dist: optimum>=1.16.0; extra == "gptq"
-Requires-Dist: auto-gptq>=0.5.0; extra == "gptq"
 Provides-Extra: awq
-Requires-Dist: autoawq; extra == "awq"
 Provides-Extra: aqlm
-Requires-Dist: aqlm[gpu]>=1.1.0; extra == "aqlm"
 Provides-Extra: qwen
-Requires-Dist: tiktoken; extra == "qwen"
-Requires-Dist: transformers_stream_generator; extra == "qwen"
 Provides-Extra: modelscope
-Requires-Dist: modelscope; extra == "modelscope"
 Provides-Extra: quality
-Requires-Dist: ruff; extra == "quality"
+License-File: LICENSE
 
 ![# LLaMA Factory](assets/logo.png)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Factory)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Factory)](https://github.com/hiyouga/LLaMA-Factory/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![Downloads](https://static.pepy.tech/badge/llmtuner)](https://pypi.org/project/llmtuner/)
-[![Citation](https://img.shields.io/badge/citation-34-green)](#projects-using-llama-factory)
+[![Citation](https://img.shields.io/badge/citation-44-green)](#projects-using-llama-factory)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
 [![Discord](https://dcbadge.vercel.app/api/server/rKfvV9r9FK?compact=true&style=flat)](https://discord.gg/rKfvV9r9FK)
 [![Twitter](https://img.shields.io/twitter/follow/llamafactory_ai)](https://twitter.com/llamafactory_ai)
 [![Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue)](https://huggingface.co/spaces/hiyouga/LLaMA-Board)
 [![Studios](https://img.shields.io/badge/ModelScope-Open%20in%20Studios-blue)](https://modelscope.cn/studios/hiyouga/LLaMA-Board)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)
 
+[![GitHub Tread](https://trendshift.io/api/badge/repositories/4535)](https://trendshift.io/repositories/4535)
+
 👋 Join our [WeChat](assets/wechat.jpg).
 
 \[ English | [中文](README_zh.md) \]
 
 **Fine-tuning a large language model can be easy as...**
 
 https://github.com/hiyouga/LLaMA-Factory/assets/16256802/9840a653-7e9c-41c8-ae89-7ace5698baf6
@@ -135,90 +104,94 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
-[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See `examples/lora_single_gpu/sft_mllm.sh` for usage.
+[24/05/14] We supported training and inference on the Ascend NPU devices. Check [installation](#installation) section for details.
+
+[24/05/13] We supported fine-tuning the **Yi-1.5** series models.
+
+[24/04/26] We supported fine-tuning the **LLaVA-1.5** multimodal LLMs. See [examples](examples/README.md) for usage.
+
+<details><summary>Full Changelog</summary>
 
 [24/04/22] We provided a **[Colab notebook](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)** for fine-tuning the Llama-3 model on a free T4 GPU. Two Llama-3-derived models fine-tuned using LLaMA Factory are available at Hugging Face, check [Llama3-8B-Chinese-Chat](https://huggingface.co/shenzhi-wang/Llama3-8B-Chinese-Chat) and [Llama3-Chinese](https://huggingface.co/zhichen/Llama3-Chinese) for details.
 
-[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See [examples](examples/README.md) for usage.
 
-[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
+[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See [examples](examples/README.md) for usage.
 
 [24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
 
-<details><summary>Full Changelog</summary>
-
-[24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See `examples/lora_single_gpu` for usage.
+[24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See [examples](examples/README.md) for usage.
 
 [24/03/21] Our paper "[LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models](https://arxiv.org/abs/2403.13372)" is available at arXiv!
 
-[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/extras/fsdp_qlora` for usage.
+[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See [examples](examples/README.md) for usage.
 
-[24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See `examples/extras/loraplus` for usage.
+[24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See [examples](examples/README.md) for usage.
 
-[24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See `examples/extras/galore` for usage.
+[24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See [examples](examples/README.md) for usage.
 
-[24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `--infer_backend vllm` to enjoy **270%** inference speed. (LoRA is not yet supported, merge it first.)
+[24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `infer_backend: vllm` to enjoy **270%** inference speed.
 
-[24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `--use_dora` to activate DoRA training.
+[24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `use_dora: true` to activate DoRA training.
 
-[24/02/15] We supported **block expansion** proposed by [LLaMA Pro](https://github.com/TencentARC/LLaMA-Pro). See `examples/extras/llama_pro` for usage.
+[24/02/15] We supported **block expansion** proposed by [LLaMA Pro](https://github.com/TencentARC/LLaMA-Pro). See [examples](examples/README.md) for usage.
 
 [24/02/05] Qwen1.5 (Qwen2 beta version) series models are supported in LLaMA-Factory. Check this [blog post](https://qwenlm.github.io/blog/qwen1.5/) for details.
 
-[24/01/18] We supported **agent tuning** for most models, equipping model with tool using abilities by fine-tuning with `--dataset glaive_toolcall`.
+[24/01/18] We supported **agent tuning** for most models, equipping model with tool using abilities by fine-tuning with `dataset: glaive_toolcall`.
 
-[23/12/23] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s implementation to boost LoRA tuning for the LLaMA, Mistral and Yi models. Try `--use_unsloth` argument to activate unsloth patch. It achieves **170%** speed in our benchmark, check [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison) for details.
+[23/12/23] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s implementation to boost LoRA tuning for the LLaMA, Mistral and Yi models. Try `use_unsloth: true` argument to activate unsloth patch. It achieves **170%** speed in our benchmark, check [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison) for details.
 
 [23/12/12] We supported fine-tuning the latest MoE model **[Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-v0.1)** in our framework. See hardware requirement [here](#hardware-requirement).
 
-[23/12/01] We supported downloading pre-trained models and datasets from the **[ModelScope Hub](https://modelscope.cn/models)** for Chinese mainland users. See [this tutorial](#use-modelscope-hub-optional) for usage.
+[23/12/01] We supported downloading pre-trained models and datasets from the **[ModelScope Hub](https://modelscope.cn/models)** for Chinese mainland users. See [this tutorial](#download-from-modelscope-hub) for usage.
 
-[23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `--neftune_noise_alpha` argument to activate NEFTune, e.g., `--neftune_noise_alpha 5`.
+[23/10/21] We supported **[NEFTune](https://arxiv.org/abs/2310.05914)** trick for fine-tuning. Try `neftune_noise_alpha: 5` argument to activate NEFTune.
 
-[23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `--shift_attn` argument to enable shift short attention.
+[23/09/27] We supported **$S^2$-Attn** proposed by [LongLoRA](https://github.com/dvlab-research/LongLoRA) for the LLaMA models. Try `shift_attn: true` argument to enable shift short attention.
 
-[23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [this example](#evaluation) to evaluate your models.
+[23/09/23] We integrated MMLU, C-Eval and CMMLU benchmarks in this repo. See [examples](examples/README.md) for usage.
 
-[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `--flash_attn fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
+[23/09/10] We supported **[FlashAttention-2](https://github.com/Dao-AILab/flash-attention)**. Try `flash_attn: fa2` argument to enable FlashAttention-2 if you are using RTX4090, A100 or H100 GPUs.
 
-[23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `--rope_scaling linear` argument in training and `--rope_scaling dynamic` argument at inference to extrapolate the position embeddings.
+[23/08/12] We supported **RoPE scaling** to extend the context length of the LLaMA models. Try `rope_scaling: linear` argument in training and `rope_scaling: dynamic` argument at inference to extrapolate the position embeddings.
 
-[23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [this example](#dpo-training) to train your models.
+[23/08/11] We supported **[DPO training](https://arxiv.org/abs/2305.18290)** for instruction-tuned models. See [examples](examples/README.md) for usage.
 
-[23/07/31] We supported **dataset streaming**. Try `--streaming` and `--max_steps 10000` arguments to load your dataset in streaming mode.
+[23/07/31] We supported **dataset streaming**. Try `streaming: true` and `max_steps: 10000` arguments to load your dataset in streaming mode.
 
 [23/07/29] We released two instruction-tuned 13B models at Hugging Face. See these Hugging Face Repos ([LLaMA-2](https://huggingface.co/hiyouga/Llama-2-Chinese-13b-chat) / [Baichuan](https://huggingface.co/hiyouga/Baichuan-13B-sft)) for details.
 
 [23/07/18] We developed an **all-in-one Web UI** for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
 [23/07/09] We released **[FastEdit](https://github.com/hiyouga/FastEdit)** ⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/06/29] We provided a **reproducible example** of training a chat model using instruction-following datasets, see [Baichuan-7B-sft](https://huggingface.co/hiyouga/Baichuan-7B-sft) for details.
 
 [23/06/22] We aligned the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
-[23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
+[23/06/03] We supported quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). See [examples](examples/README.md) for usage.
 
 </details>
 
 ## Supported Models
 
 | Model                                                    | Model size                       | Default module    | Template  |
 | -------------------------------------------------------- | -------------------------------- | ----------------- | --------- |
 | [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                           | W_pack            | baichuan2 |
 | [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
 | [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B      | query_key_value   | -         |
 | [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                               | query_key_value   | chatglm3  |
 | [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                         | q_proj,v_proj     | cohere    |
-| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                       | q_proj,v_proj     | deepseek  |
+| [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B/236B                  | q_proj,v_proj     | deepseek  |
 | [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                      | query_key_value   | falcon    |
 | [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                            | q_proj,v_proj     | gemma     |
 | [InternLM2](https://huggingface.co/internlm)             | 7B/20B                           | wqkv              | intern2   |
 | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B                   | q_proj,v_proj     | -         |
 | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                       | q_proj,v_proj     | llama2    |
 | [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                           | q_proj,v_proj     | llama3    |
 | [LLaVA-1.5](https://huggingface.co/llava-hf)             | 7B/13B                           | q_proj,v_proj     | vicuna    |
@@ -226,15 +199,16 @@
 | [OLMo](https://huggingface.co/allenai)                   | 1B/7B                            | q_proj,v_proj     | -         |
 | [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                        | q_proj,v_proj     | -         |
 | [Phi-3](https://huggingface.co/microsoft)                | 3.8B                             | qkv_proj          | phi       |
 | [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B                  | c_attn            | qwen      |
 | [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B/110B | q_proj,v_proj     | qwen      |
 | [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                        | q_proj,v_proj     | -         |
 | [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                       | q_proj,v_proj     | xverse    |
-| [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yi (1/1.5)](https://huggingface.co/01-ai)               | 6B/9B/34B                        | q_proj,v_proj     | yi        |
+| [Yi-VL](https://huggingface.co/01-ai)                    | 6B/34B                           | q_proj,v_proj     | yi_vl     |
 | [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                      | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
 > **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules for better convergence.
 >
 > For the "base" models, the `--template` argument can be chosen from `default`, `alpaca`, `vicuna` etc. But make sure to use the **corresponding template** for the "instruct/chat" models.
 >
@@ -272,16 +246,16 @@
 </details>
 
 <details><summary>Supervised fine-tuning datasets</summary>
 
 - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
 - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [Alpaca GPT4 (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-- [Self Cognition (zh)](data/self_cognition.json)
-- [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+- [Identity (en&zh)](data/identity.json)
+- [Open Assistant (zh)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
 - [Guanaco Dataset (multilingual)](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
 - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
 - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
 - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
 - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
 - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
@@ -321,19 +295,19 @@
 - [Ultrachat (de)](https://huggingface.co/datasets/mayflowergmbh/ultra-chat_de)
 
 </details>
 
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
-- [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
 - [DPO mixed (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
+- [Open Assistant (zh)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -343,26 +317,27 @@
 
 ## Requirement
 
 | Mandatory    | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | python       | 3.8     | 3.10      |
 | torch        | 1.13.1  | 2.2.0     |
-| transformers | 4.37.2  | 4.39.3    |
-| datasets     | 2.14.3  | 2.18.0    |
-| accelerate   | 0.27.2  | 0.28.0    |
+| transformers | 4.37.2  | 4.40.1    |
+| datasets     | 2.14.3  | 2.19.1    |
+| accelerate   | 0.27.2  | 0.30.0    |
 | peft         | 0.9.0   | 0.10.0    |
-| trl          | 0.8.1   | 0.8.1     |
+| trl          | 0.8.1   | 0.8.6     |
 
 | Optional     | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | CUDA         | 11.6    | 12.2      |
 | deepspeed    | 0.10.0  | 0.14.0    |
-| bitsandbytes | 0.39.0  | 0.43.0    |
-| flash-attn   | 2.3.0   | 2.5.6     |
+| bitsandbytes | 0.39.0  | 0.43.1    |
+| vllm         | 0.4.0   | 0.4.2     |
+| flash-attn   | 2.3.0   | 2.5.8     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
 | Method            | Bits |   7B  |  13B  |  30B  |   70B  |  110B  |  8x7B |  8x22B |
 | ----------------- | ---- | ----- | ----- | ----- | ------ | ------ | ----- | ------ |
@@ -372,64 +347,109 @@
 | LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB |  240GB | 120GB |  320GB |
 | QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  140GB |  60GB |  160GB |
 | QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |   72GB |  30GB |   96GB |
 | QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |   48GB |  18GB |   48GB |
 
 ## Getting Started
 
-### Data Preparation
-
-Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
-
-> [!NOTE]
-> Please update `data/dataset_info.json` to use your custom dataset.
+### Installation
 
-### Dependence Installation
+> [!IMPORTANT]
+> Installation is mandatory.
 
 ```bash
 git clone https://github.com/hiyouga/LLaMA-Factory.git
-conda create -n llama_factory python=3.10
-conda activate llama_factory
 cd LLaMA-Factory
-pip install -e .[metrics]
+pip install -e .[torch,metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: torch, metrics, deepspeed, bitsandbytes, vllm, galore, badam, gptq, awq, aqlm, qwen, modelscope, quality
+
+> [!TIP]
+> Use `pip install --no-deps -e .` to resolve package conflicts.
 
 <details><summary>For Windows users</summary>
 
-If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
+If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you need to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
 ```
 
 To enable FlashAttention-2 on the Windows platform, you need to install the precompiled `flash-attn` library, which supports CUDA 12.1 to 12.2. Please download the corresponding version from [flash-attention](https://github.com/bdashore3/flash-attention/releases) based on your requirements.
 
 </details>
 
-### Train with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
+<details><summary>For Ascend NPU users</summary>
+
+To utilize Ascend NPU devices for (distributed) training and inference, you need to install the **[torch-npu](https://gitee.com/ascend/pytorch)** library and the **[Ascend CANN Kernels](https://www.hiascend.com/developer/download/community/result?module=cann)**.
+
+| Requirement  | Minimum | Recommend |
+| ------------ | ------- | --------- |
+| CANN         | 8.0.RC1 | 8.0.RC1   |
+| torch        | 2.2.0   | 2.2.0     |
+| torch-npu    | 2.2.0   | 2.2.0     |
+| deepspeed    | 0.13.2  | 0.13.2    |
+
+Docker image:
+
+- 32GB: [Download page](http://mirrors.cn-central-221.ovaijisuan.com/detail/130.html)
+- 64GB: Coming soon
+
+Remember to use `ASCEND_RT_VISIBLE_DEVICES` instead of `CUDA_VISIBLE_DEVICES` to specify the device to use.
+
+If you cannot infer model on NPU devices, try setting `do_sample: false` in the configurations.
+
+</details>
+
+### Data Preparation
+
+Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
+
+> [!NOTE]
+> Please update `data/dataset_info.json` to use your custom dataset.
+
+### Quickstart
+
+Use the following 3 commands to run LoRA **fine-tuning**, **inference** and **merging** of the Llama3-8B-Instruct model, respectively.
+
+```bash
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli train examples/lora_single_gpu/llama3_lora_sft.yaml
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli chat examples/inference/llama3_lora_sft.yaml
+CUDA_VISIBLE_DEVICES=0 llamafactory-cli export examples/merge_lora/llama3_lora_sft.yaml
+```
+
+See [examples/README.md](examples/README.md) for advanced usage (including distributed training).
+
+> [!TIP]
+> Use `llamafactory-cli help` to show help information.
+
+### Fine-Tuning with LLaMA Board GUI (powered by [Gradio](https://github.com/gradio-app/gradio))
 
 > [!IMPORTANT]
-> LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
+> LLaMA Board GUI only supports training on a single GPU.
 
 #### Use local environment
 
 ```bash
-export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
-export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
-python src/train_web.py # or python -m llmtuner.webui.interface
+CUDA_VISIBLE_DEVICES=0 GRADIO_SHARE=1 llamafactory-cli webui
 ```
 
-<details><summary>For Alibaba Cloud users</summary>
+<details><summary>For Alibaba Cloud PAI or AutoDL users</summary>
 
-If you encountered display problems in LLaMA Board on Alibaba Cloud, try using the following command to set environment variables before starting LLaMA Board:
+If you encountered display problems in LLaMA Board on Alibaba Cloud PAI, try using the following command to set environment variables before starting LLaMA Board:
 
 ```bash
-export GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+export GRADIO_SERVER_PORT=7860 GRADIO_ROOT_PATH=/${JUPYTER_NAME}/proxy/7860/
+```
+
+If you are using AutoDL, please install a specific version of Gradio:
+
+```bash
+pip install gradio==4.10.0
 ```
 
 </details>
 
 #### Use Docker
 
 ```bash
@@ -455,28 +475,18 @@
 
 - hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
 - data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
 - output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
 
 </details>
 
-### Train with Command Line Interface
-
-See [examples/README.md](examples/README.md) for usage.
-
-Use `python src/train_bash.py -h` to display arguments description.
-
 ### Deploy with OpenAI-style API and vLLM
 
 ```bash
-CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 python src/api_demo.py \
-    --model_name_or_path meta-llama/Meta-Llama-3-8B-Instruct \
-    --template llama3 \
-    --infer_backend vllm \
-    --vllm_enforce_eager
+CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 llamafactory-cli api examples/inference/llama3_vllm.yaml
 ```
 
 ### Download from ModelScope Hub
 
 If you have trouble with downloading models and datasets from Hugging Face, you can use ModelScope.
 
 ```bash
@@ -508,35 +518,45 @@
 1. Cao et al. Head-wise Shareable Attention for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.11819)
 1. Zhang et al. Enhancing Multilingual Capabilities of Large Language Models through Self-Distillation from Resource-Rich Languages. 2024. [[arxiv]](https://arxiv.org/abs/2402.12204)
 1. Kim et al. Efficient and Effective Vocabulary Expansion Towards Multilingual Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.14714)
 1. Yu et al. KIEval: A Knowledge-grounded Interactive Evaluation Framework for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.15043)
 1. Huang et al. Key-Point-Driven Data Synthesis with its Enhancement on Mathematical Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2403.02333)
 1. Duan et al. Negating Negatives: Alignment without Human Positive Samples via Distributional Dispreference Optimization. 2024. [[arxiv]](https://arxiv.org/abs/2403.03419)
 1. Xie and Schwertfeger. Empowering Robotics with Large Language Models: osmAG Map Comprehension with LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2403.08228)
+1. Wu et al. Large Language Models are Parallel Multilingual Learners. 2024. [[arxiv]](https://arxiv.org/abs/2403.09073)
 1. Zhang et al. EDT: Improving Large Language Models' Generation by Entropy-based Dynamic Temperature Sampling. 2024. [[arxiv]](https://arxiv.org/abs/2403.14541)
 1. Weller et al. FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions. 2024. [[arxiv]](https://arxiv.org/abs/2403.15246)
 1. Hongbin Na. CBT-LLM: A Chinese Large Language Model for Cognitive Behavioral Therapy-based Mental Health Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2403.16008)
 1. Zan et al. CodeS: Natural Language to Code Repository via Multi-Layer Sketch. 2024. [[arxiv]](https://arxiv.org/abs/2403.16443)
 1. Liu et al. Extensive Self-Contrast Enables Feedback-Free Language Model Alignment. 2024. [[arxiv]](https://arxiv.org/abs/2404.00604)
 1. Luo et al. BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.02827)
 1. Du et al. Chinese Tiny LLM: Pretraining a Chinese-Centric Large Language Model. 2024. [[arxiv]](https://arxiv.org/abs/2404.04167)
+1. Ma et al. Parameter Efficient Quasi-Orthogonal Fine-Tuning via Givens Rotation. 2024. [[arxiv]](https://arxiv.org/abs/2404.04316)
 1. Liu et al. Dynamic Generation of Personalities with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.07084)
+1. Shang et al. How Far Have We Gone in Stripped Binary Code Understanding Using Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.09836)
+1. Huang et al. LLMTune: Accelerate Database Knob Tuning with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.11581)
+1. Deng et al. Text-Tuple-Table: Towards Information Integration in Text-to-Table Generation via Global Tuple Extraction. 2024. [[arxiv]](https://arxiv.org/abs/2404.14215)
+1. Acikgoz et al. Hippocrates: An Open-Source Framework for Advancing Large Language Models in Healthcare. 2024. [[arxiv]](https://arxiv.org/abs/2404.16621)
+1. Zhang et al. Small Language Models Need Strong Verifiers to Self-Correct Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2404.17140)
+1. Zhou et al. FREB-TQA: A Fine-Grained Robustness Evaluation Benchmark for Table Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2404.18585)
 1. **[StarWhisper](https://github.com/Yu-Yang-Li/StarWhisper)**: A large language model for Astronomy, based on ChatGLM2-6B and Qwen-14B.
 1. **[DISC-LawLLM](https://github.com/FudanDISC/DISC-LawLLM)**: A large language model specialized in Chinese legal domain, based on Baichuan-13B, is capable of retrieving and reasoning on legal knowledge.
 1. **[Sunsimiao](https://github.com/thomas-yanxin/Sunsimiao)**: A large language model specialized in Chinese medical domain, based on Baichuan-7B and ChatGLM-6B.
 1. **[CareGPT](https://github.com/WangRongsheng/CareGPT)**: A series of large language models for Chinese medical domain, based on LLaMA2-7B and Baichuan-13B.
 1. **[MachineMindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)**: A series of MBTI Personality large language models, capable of giving any LLM 16 different personality types based on different datasets and training methods.
+1. **[Luminia-13B-v3](https://huggingface.co/Nekochu/Luminia-13B-v3)**: A large language model specialized in generate metadata for stable diffusion. [[🤗Demo]](https://huggingface.co/spaces/Nekochu/Luminia-13B_SD_Prompt)
+1. **[Chinese-LLaVA-Med](https://github.com/BUAADreamer/Chinese-LLaVA-Med)**: A multimodal large language model specialized in Chinese medical domain, based on LLaVA-1.5-7B.
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2/LLaVA-1.5](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2 (LLaVA-1.5)](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Phi-3](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/LICENSE) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yi-1.5](LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.7.0/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.7.1/src/llmtuner.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/llmtuner/__init__.py
+src/llmtuner/cli.py
 src/llmtuner.egg-info/PKG-INFO
 src/llmtuner.egg-info/SOURCES.txt
 src/llmtuner.egg-info/dependency_links.txt
+src/llmtuner.egg-info/entry_points.txt
 src/llmtuner.egg-info/requires.txt
 src/llmtuner.egg-info/top_level.txt
 src/llmtuner/api/__init__.py
 src/llmtuner/api/app.py
+src/llmtuner/api/chat.py
+src/llmtuner/api/common.py
 src/llmtuner/api/protocol.py
 src/llmtuner/chat/__init__.py
 src/llmtuner/chat/base_engine.py
 src/llmtuner/chat/chat_model.py
 src/llmtuner/chat/hf_engine.py
 src/llmtuner/chat/vllm_engine.py
 src/llmtuner/data/__init__.py
@@ -96,12 +100,8 @@
 src/llmtuner/webui/components/__init__.py
 src/llmtuner/webui/components/chatbot.py
 src/llmtuner/webui/components/data.py
 src/llmtuner/webui/components/eval.py
 src/llmtuner/webui/components/export.py
 src/llmtuner/webui/components/infer.py
 src/llmtuner/webui/components/top.py
-src/llmtuner/webui/components/train.py
-tests/test_attn.py
-tests/test_galore.py
-tests/test_throughput.py
-tests/test_toolcall.py
+src/llmtuner/webui/components/train.py
```

### Comparing `llmtuner-0.7.0/src/llmtuner.egg-info/requires.txt` & `llmtuner-0.7.1/src/llmtuner.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-torch>=1.13.1
 transformers>=4.37.2
 datasets>=2.14.3
 accelerate>=0.27.2
 peft>=0.10.0
 trl>=0.8.1
 gradio>=4.0.0
 scipy
 einops
 sentencepiece
 protobuf
 uvicorn
 pydantic
 fastapi
 sse-starlette
-matplotlib
+matplotlib>=3.7.0
 fire
 packaging
+pyyaml
 
 [aqlm]
 aqlm[gpu]>=1.1.0
 
 [awq]
 autoawq
 
 [badam]
 badam
 
 [bitsandbytes]
 bitsandbytes>=0.39.0
 
 [deepspeed]
-deepspeed>=0.10.0
+deepspeed<=0.14.0,>=0.10.0
 
 [galore]
 galore-torch
 
 [gptq]
 optimum>=1.16.0
 auto-gptq>=0.5.0
@@ -50,9 +50,12 @@
 [quality]
 ruff
 
 [qwen]
 tiktoken
 transformers_stream_generator
 
+[torch]
+torch>=1.13.1
+
 [vllm]
 vllm>=0.4.0
```

