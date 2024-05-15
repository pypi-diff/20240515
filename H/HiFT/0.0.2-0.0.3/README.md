# Comparing `tmp/HiFT-0.0.2.tar.gz` & `tmp/HiFT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HiFT-0.0.2.tar", last modified: Sun May 12 21:39:57 2024, max compression
+gzip compressed data, was "dist/HiFT-0.0.3.tar", last modified: Wed May 15 12:42:06 2024, max compression
```

## Comparing `HiFT-0.0.2.tar` & `HiFT-0.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.335502 HiFT-0.0.2/
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.303503 HiFT-0.0.2/HiFT.egg-info/
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-12 21:39:57.000000 HiFT-0.0.2/HiFT.egg-info/PKG-INFO
--rw-r--r--   0 yongkang (31362) cisintern (30001)     1250 2024-05-12 21:39:57.000000 HiFT-0.0.2/HiFT.egg-info/SOURCES.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)        1 2024-05-12 21:39:57.000000 HiFT-0.0.2/HiFT.egg-info/dependency_links.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)       14 2024-05-12 21:39:57.000000 HiFT-0.0.2/HiFT.egg-info/top_level.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)     1159 2024-05-01 15:36:00.000000 HiFT-0.0.2/LICENSE.md
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-12 21:39:57.335502 HiFT-0.0.2/PKG-INFO
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12282 2024-05-01 15:36:00.000000 HiFT-0.0.2/README.md
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.311503 HiFT-0.0.2/examples/
--rw-r--r--   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4137 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/build_dataset.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    21928 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/instruct_tuning.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     8321 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/llama2_flash_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4054 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/llama_flash_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4916 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/llama_xformers_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    30614 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/pretrain_tuning.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    35261 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/run_generation.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    33497 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/run_glue.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    32290 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/run_ner.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    37349 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/run_qa.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    22777 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/utils_qa.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    20707 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/vicuna_train.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.315502 HiFT-0.0.2/hift/
--rw-r--r--   0 yongkang (31362) cisintern (30001)      268 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/__init__.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.323502 HiFT-0.0.2/hift/optimizers/
--rw-r--r--   0 yongkang (31362) cisintern (30001)      644 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14454 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/adagrad.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.331502 HiFT-0.0.2/hift/optimizers/bitsandbytes/
--rw-r--r--   0 yongkang (31362) cisintern (30001)     1001 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7897 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/adagrad.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    23872 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/adam.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14509 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/adamw.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7944 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/lamb.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     9373 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/lars.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    11596 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/lion.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7769 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/rmsprop.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     6444 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/sgd.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    34481 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/optimization.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    74393 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/optimizer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    10583 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/replace_operation.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    15390 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/rmsprop.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14715 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/sgd.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    29623 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/torchAdam.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    29240 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/torchAdamw.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12180 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/qatrainer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    13782 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/registerCallBack.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    30885 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/seqtrainer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    65929 2024-05-12 21:35:57.000000 HiFT-0.0.2/hift/trainer.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.331502 HiFT-0.0.2/hift/utils/
--rw-r--r--   0 yongkang (31362) cisintern (30001)       32 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/utils/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     6997 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/utils/utils.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)       38 2024-05-12 21:39:57.335502 HiFT-0.0.2/setup.cfg
--rw-r--r--   0 yongkang (31362) cisintern (30001)      783 2024-05-12 21:38:15.000000 HiFT-0.0.2/setup.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.140874 HiFT-0.0.3/
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.024879 HiFT-0.0.3/HiFT.egg-info/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-15 12:42:05.000000 HiFT-0.0.3/HiFT.egg-info/PKG-INFO
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1250 2024-05-15 12:42:05.000000 HiFT-0.0.3/HiFT.egg-info/SOURCES.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)        1 2024-05-15 12:42:05.000000 HiFT-0.0.3/HiFT.egg-info/dependency_links.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       14 2024-05-15 12:42:05.000000 HiFT-0.0.3/HiFT.egg-info/top_level.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    11324 2024-05-14 23:32:09.000000 HiFT-0.0.3/LICENSE.md
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-15 12:42:06.136874 HiFT-0.0.3/PKG-INFO
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12282 2024-05-01 15:36:00.000000 HiFT-0.0.3/README.md
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.044878 HiFT-0.0.3/examples/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:30:41.000000 HiFT-0.0.3/examples/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4135 2024-05-14 12:27:27.000000 HiFT-0.0.3/examples/build_dataset.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    23087 2024-05-14 20:25:29.000000 HiFT-0.0.3/examples/instruct_tuning.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     8321 2024-05-12 21:30:41.000000 HiFT-0.0.3/examples/llama2_flash_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4054 2024-05-12 21:30:41.000000 HiFT-0.0.3/examples/llama_flash_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4916 2024-05-12 21:30:42.000000 HiFT-0.0.3/examples/llama_xformers_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    30731 2024-05-14 15:18:26.000000 HiFT-0.0.3/examples/pretrain_tuning.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    35374 2024-05-14 21:31:37.000000 HiFT-0.0.3/examples/run_generation.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    33754 2024-05-14 20:20:10.000000 HiFT-0.0.3/examples/run_glue.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    32543 2024-05-14 20:20:40.000000 HiFT-0.0.3/examples/run_ner.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    37615 2024-05-14 20:20:53.000000 HiFT-0.0.3/examples/run_qa.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    22777 2024-05-12 21:30:42.000000 HiFT-0.0.3/examples/utils_qa.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    20863 2024-05-14 20:21:08.000000 HiFT-0.0.3/examples/vicuna_train.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.048878 HiFT-0.0.3/hift/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      268 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/__init__.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.112875 HiFT-0.0.3/hift/optimizers/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      761 2024-05-14 15:15:35.000000 HiFT-0.0.3/hift/optimizers/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14454 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/adagrad.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.132874 HiFT-0.0.3/hift/optimizers/bitsandbytes/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1001 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7897 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/adagrad.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    23872 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/adam.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14509 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/adamw.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7944 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/lamb.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     9373 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/lars.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    11596 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/lion.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7769 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/rmsprop.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     6444 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/sgd.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    34481 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/optimization.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    74393 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/optimizer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    37568 2024-05-14 15:15:17.000000 HiFT-0.0.3/hift/optimizers/replace_operation.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    15390 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/rmsprop.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14715 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/sgd.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    29623 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/torchAdam.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    29240 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/torchAdamw.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12180 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/qatrainer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12584 2024-05-15 12:39:58.000000 HiFT-0.0.3/hift/registerCallBack.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    30885 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/seqtrainer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    77451 2024-05-14 15:15:05.000000 HiFT-0.0.3/hift/trainer.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.136874 HiFT-0.0.3/hift/utils/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       32 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/utils/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     6997 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/utils/utils.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       38 2024-05-15 12:42:06.140874 HiFT-0.0.3/setup.cfg
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      783 2024-05-15 12:41:58.000000 HiFT-0.0.3/setup.py
```

### Comparing `HiFT-0.0.2/HiFT.egg-info/PKG-INFO` & `HiFT-0.0.3/HiFT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiFT
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.
 Home-page: https://github.com/misonsky/HiFT
 Author: Yongkang Liu
 Author-email: misonsky@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HiFT-0.0.2/HiFT.egg-info/SOURCES.txt` & `HiFT-0.0.3/HiFT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/PKG-INFO` & `HiFT-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiFT
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.
 Home-page: https://github.com/misonsky/HiFT
 Author: Yongkang Liu
 Author-email: misonsky@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HiFT-0.0.2/README.md` & `HiFT-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/examples/build_dataset.py` & `HiFT-0.0.3/examples/build_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         targets = []
         prompt = PROMPT_TEMPLATE
         for instruction, input, output in zip(examples['instruction'],examples['input'],examples['output']):
             if input is not None and input !="":
                 instruction = instruction+'\n'+input
             source = prompt.format_map({'instruction':instruction})
             target = f"{output}{tokenizer.eos_token}"
-
             sources.append(source)
             targets.append(target)
 
         tokenized_sources = tokenizer(sources,return_attention_mask=False)
         tokenized_targets = tokenizer(targets,return_attention_mask=False,add_special_tokens=False)
 
         all_input_ids = []
```

### Comparing `HiFT-0.0.2/examples/instruct_tuning.py` & `HiFT-0.0.3/examples/instruct_tuning.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # You can also adapt this script on your own causal language modeling task. Pointers for this are left as comments.
 
 import logging
 import math
 import os
 import sys
 from dataclasses import dataclass, field
-from typing import Optional,Tuple,List
+from typing import Optional,Tuple,List,Dict
 from pathlib import Path
 import datasets
 import torch
 from build_dataset import build_instruction_dataset, DataCollatorForSupervisedDataset
 import transformers
 from transformers import (
     CONFIG_MAPPING,
@@ -74,18 +74,17 @@
 from transformers.utils.versions import require_version
 
 
 from transformers.trainer_utils import PREFIX_CHECKPOINT_DIR
 
 sys.path.append(os.path.abspath('.'))
 from hift import HiFTSeq2SeqTrainer,GetCallBack,peft_function,Seq2SeqTrainer
-from peft import PeftModel, get_peft_model_state_dict
+from peft import PeftModel
 
 from llama2_flash_attn_monkey_patch import replace_llama_attn_with_flash_attn
-
 replace_llama_attn_with_flash_attn()
 
 MAX_LENGTH = int(10000)  # Hardcoded max length to avoid infinite loop
 IGNORE_INDEX = -100
 DEFAULT_PAD_TOKEN = "[PAD]"
 DEFAULT_EOS_TOKEN = "</s>"
 DEFAULT_BOS_TOKEN = "<s>"
@@ -112,14 +111,18 @@
 class TrainingArguments(Seq2SeqTrainingArguments):
     model_max_length: int = field(
         default=512,
         metadata={
             "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
+    optim: str = field(
+        default="adamw_torch",
+        metadata={"help": "The optimizer to use."},
+    )
     pretraining_tp: int = field(
         default=1,
         metadata={
             "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
 
@@ -314,14 +317,36 @@
         return control
 
     def on_train_end(self, args, state, control, **kwargs):
         peft_model_path = os.path.join(args.output_dir, "sft_peft_model")
         kwargs["model"].save_pretrained(peft_model_path)
         kwargs["tokenizer"].save_pretrained(peft_model_path)
 
+def smart_tokenizer_and_embedding_resize(
+    special_tokens_dict: Dict,
+    tokenizer: transformers.PreTrainedTokenizer,
+    model: transformers.PreTrainedModel,
+):
+    """Resize tokenizer and embedding.
+
+    Note: This is the unoptimized version that may make your embedding size not be divisible by 64.
+    """
+    num_new_tokens = tokenizer.add_special_tokens(special_tokens_dict)
+    model.resize_token_embeddings(len(tokenizer))
+
+    if num_new_tokens > 0:
+        input_embeddings = model.get_input_embeddings().weight.data
+        output_embeddings = model.get_output_embeddings().weight.data
+
+        input_embeddings_avg = input_embeddings[:-num_new_tokens].mean(dim=0, keepdim=True)
+        output_embeddings_avg = output_embeddings[:-num_new_tokens].mean(dim=0, keepdim=True)
+
+        input_embeddings[-num_new_tokens:] = input_embeddings_avg
+        output_embeddings[-num_new_tokens:] = output_embeddings_avg
+
 def main():
 
     parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, TrainingArguments))
     if len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
         # If we pass only one argument to the script and it's the path to a json file,
         # let's parse it to get our arguments.
         model_args, data_args, training_args = parser.parse_json_file(json_file=os.path.abspath(sys.argv[1]))
@@ -389,17 +414,23 @@
         use_fast=model_args.use_fast_tokenizer,
         revision=model_args.model_revision,
         model_max_length=training_args.model_max_length,
         padding_side=model_args.padding_side,
         use_auth_token=True if model_args.use_auth_token else None,
     )
     
+    special_tokens_dict = dict()
     if tokenizer.pad_token is None:
-        print(f"Adding pad token {DEFAULT_PAD_TOKEN}")
-        tokenizer.add_special_tokens(dict(pad_token=DEFAULT_PAD_TOKEN))
+        special_tokens_dict["pad_token"] = DEFAULT_PAD_TOKEN
+    if tokenizer.eos_token is None:
+        special_tokens_dict["eos_token"] = DEFAULT_EOS_TOKEN
+    if tokenizer.bos_token is None:
+        special_tokens_dict["bos_token"] = DEFAULT_BOS_TOKEN
+    if tokenizer.unk_token is None:
+        special_tokens_dict["unk_token"] = DEFAULT_UNK_TOKEN
     
     torch_dtype = (
             model_args.torch_dtype
             if model_args.torch_dtype in ["auto", None]
             else getattr(torch, model_args.torch_dtype)
         )
     model = model_class.from_pretrained(
@@ -423,19 +454,19 @@
                     task_type = model_args.HiTaskType,
                     rank=model_args.lora_rank,
                     virtual_tokens=model_args.virtual_tokens,
                     tokenizer_name_or_path=model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path,
                     init_text=model_args.init_text if model_args.peft_type=="prompt_tuning" else None,
                     peft_config=None)
     
-    logger.info(f"len(tokenizer):{len(tokenizer)}")
-    embedding_size = model.get_input_embeddings().weight.shape[0]
-    if len(tokenizer) != embedding_size:
-        logger.info("resize the embedding size by the size of the tokenizer")
-        model.resize_token_embeddings(len(tokenizer))
+    smart_tokenizer_and_embedding_resize(
+        special_tokens_dict=special_tokens_dict,
+        tokenizer=tokenizer,
+        model=model,
+    )
     
     data_collator = DataCollatorForSupervisedDataset(tokenizer=tokenizer)
     eval_dataset=None
     train_dataset = None
 
     if training_args.do_train:
         with training_args.main_process_first(desc="loading and tokenization"):
```

### Comparing `HiFT-0.0.2/examples/llama2_flash_attn_monkey_patch.py` & `HiFT-0.0.3/examples/llama2_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/examples/llama_flash_attn_monkey_patch.py` & `HiFT-0.0.3/examples/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/examples/llama_xformers_attn_monkey_patch.py` & `HiFT-0.0.3/examples/llama_xformers_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/examples/pretrain_tuning.py` & `HiFT-0.0.3/examples/pretrain_tuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,14 +348,18 @@
 class TrainingArguments(Seq2SeqTrainingArguments):
     model_max_length: int = field(
         default=512,
         metadata={
             "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
+    optim: str = field(
+        default="adamw_torch",
+        metadata={"help": "The optimizer to use."},
+    )
     debug_mode: bool = field(default=False)
     pretraining_tp: int = field(
         default=1,
         metadata={
             "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
```

### Comparing `HiFT-0.0.2/examples/run_generation.py` & `HiFT-0.0.3/examples/run_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,14 +357,18 @@
 class TrainingArguments(Seq2SeqTrainingArguments):
     model_max_length: int = field(
         default=512,
         metadata={
             "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
+    optim: str = field(
+        default="adamw_torch",
+        metadata={"help": "The optimizer to use."},
+    )
     pretraining_tp: int = field(
         default=1,
         metadata={
             "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
```

### Comparing `HiFT-0.0.2/examples/run_glue.py` & `HiFT-0.0.3/examples/run_glue.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,24 @@
     "sst2": ("sentence", None),
     "stsb": ("sentence1", "sentence2"),
     "wnli": ("sentence1", "sentence2"),
 }
 
 logger = logging.getLogger(__name__)
 
+
+
+@dataclass
+class MyTrainingArguments(TrainingArguments):
+    optim: str = field(
+        default="adamw_torch",
+        metadata={"help": "The optimizer to use."},
+    )
+
+
 @dataclass
 class DataTrainingArguments:
     """
     Arguments pertaining to what data we are going to input our model for training and eval.
 
     Using `HfArgumentParser` we can turn this class
     into argparse arguments to be able to specify them on
@@ -293,15 +303,15 @@
         kwargs["tokenizer"].save_pretrained(peft_model_path)
 
 def main():
     # See all possible arguments in src/transformers/training_args.py
     # or by passing the --help flag to this script.
     # We now keep distinct sets of args, for a cleaner separation of concerns.
 
-    parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, TrainingArguments))
+    parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, MyTrainingArguments))
     if len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
         # If we pass only one argument to the script and it's the path to a json file,
         # let's parse it to get our arguments.
         model_args, data_args, training_args = parser.parse_json_file(json_file=os.path.abspath(sys.argv[1]))
     else:
         model_args, data_args, training_args = parser.parse_args_into_dataclasses()
 
@@ -661,14 +671,16 @@
             model=model,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
             compute_metrics=compute_metrics,
             tokenizer=tokenizer,
             data_collator=data_collator,
         )
+    if model_args.peft_type:
+        trainer.add_callback(SavePeftModelCallback)
     # Training
     if training_args.do_train:
         checkpoint = None
         if training_args.resume_from_checkpoint is not None:
             checkpoint = training_args.resume_from_checkpoint
         elif last_checkpoint is not None:
             checkpoint = last_checkpoint
```

### Comparing `HiFT-0.0.2/examples/run_ner.py` & `HiFT-0.0.3/examples/run_ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 # Will error if the minimal version of Transformers is not installed. Remove at your own risks.
 check_min_version("4.36.0")
 
 require_version("datasets>=1.8.0", "To fix: pip install -r examples/pytorch/token-classification/requirements.txt")
 
 logger = logging.getLogger(__name__)
 
+@dataclass
+class MyTrainingArguments(TrainingArguments):
+    optim: str = field(
+        default="adamw_torch",
+        metadata={"help": "The optimizer to use."},
+    )
 
 @dataclass
 class ModelArguments:
     """
     Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
     """
 
@@ -295,15 +301,15 @@
         kwargs["tokenizer"].save_pretrained(peft_model_path)
 
 def main():
     # See all possible arguments in src/transformers/training_args.py
     # or by passing the --help flag to this script.
     # We now keep distinct sets of args, for a cleaner separation of concerns.
 
-    parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, TrainingArguments))
+    parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, MyTrainingArguments))
     if len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
         # If we pass only one argument to the script and it's the path to a json file,
         # let's parse it to get our arguments.
         model_args, data_args, training_args = parser.parse_json_file(json_file=os.path.abspath(sys.argv[1]))
     else:
         model_args, data_args, training_args = parser.parse_args_into_dataclasses()
 
@@ -687,14 +693,16 @@
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
             tokenizer=tokenizer,
             data_collator=data_collator,
             compute_metrics=compute_metrics,
         )
 
+    if model_args.peft_type:
+        trainer.add_callback(SavePeftModelCallback)
     # Training
     if training_args.do_train:
         checkpoint = None
         if training_args.resume_from_checkpoint is not None:
             checkpoint = training_args.resume_from_checkpoint
         elif last_checkpoint is not None:
             checkpoint = last_checkpoint
```

### Comparing `HiFT-0.0.2/examples/run_qa.py` & `HiFT-0.0.3/examples/run_qa.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,20 @@
 # Will error if the minimal version of Transformers is not installed. Remove at your own risks.
 check_min_version("4.36.0")
 
 require_version("datasets>=1.8.0", "To fix: pip install -r examples/pytorch/question-answering/requirements.txt")
 
 logger = logging.getLogger(__name__)
 
+@dataclass
+class MyTrainingArguments(TrainingArguments):
+    optim: str = field(
+        default="adamw_torch",
+        metadata={"help": "The optimizer to use."},
+    )
 
 @dataclass
 class ModelArguments:
     """
     Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
     """
 
@@ -304,15 +310,15 @@
         kwargs["tokenizer"].save_pretrained(peft_model_path)
 
 def main():
     # See all possible arguments in src/transformers/training_args.py
     # or by passing the --help flag to this script.
     # We now keep distinct sets of args, for a cleaner separation of concerns.
 
-    parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, TrainingArguments))
+    parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, MyTrainingArguments))
     if len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
         # If we pass only one argument to the script and it's the path to a json file,
         # let's parse it to get our arguments.
         model_args, data_args, training_args = parser.parse_json_file(json_file=os.path.abspath(sys.argv[1]))
     else:
         model_args, data_args, training_args = parser.parse_args_into_dataclasses()
 
@@ -745,14 +751,17 @@
             args=training_args,
             model=model,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
             tokenizer=tokenizer,
             data_collator=data_collator,
             compute_metrics=compute_metrics)
+            
+    if model_args.peft_type:
+        trainer.add_callback(SavePeftModelCallback)
 
     # Training
     if training_args.do_train:
         checkpoint = None
         if training_args.resume_from_checkpoint is not None:
             checkpoint = training_args.resume_from_checkpoint
         elif last_checkpoint is not None:
```

### Comparing `HiFT-0.0.2/examples/utils_qa.py` & `HiFT-0.0.3/examples/utils_qa.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/examples/vicuna_train.py` & `HiFT-0.0.3/examples/vicuna_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,18 @@
 class TrainingArguments(Seq2SeqTrainingArguments):
     model_max_length: int = field(
         default=512,
         metadata={
             "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
+    optim: str = field(
+        default="adamw_torch",
+        metadata={"help": "The optimizer to use."},
+    )
     pretraining_tp: int = field(
         default=1,
         metadata={
             "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
 
@@ -314,23 +318,23 @@
             parts = turn.split(sep)
             if len(parts) != 2:
                 break
             parts[0] += sep
             # "-2" is hardcoded for the Llama tokenizer to make the offset correct.
             instruction_len = len(tokenizer(parts[0]).input_ids) - 2
 
-            if i != 0 and not tokenizer.legacy:
+            if i != 0 and hasattr(tokenizer,"legacy") and not tokenizer.legacy:
                 # The legacy and non-legacy modes handle special tokens differently
                 instruction_len -= 1
 
             # Ignore the user instructions
             target[cur_len : cur_len + instruction_len] = IGNORE_TOKEN_ID
             cur_len += turn_len
 
-            if i != 0 and not tokenizer.legacy:
+            if i != 0 and hasattr(tokenizer,"legacy") and not tokenizer.legacy:
                 # The legacy and non-legacy modes handle special tokens differently
                 cur_len -= 1
 
         target[cur_len:] = IGNORE_TOKEN_ID
 
         if False:  # Inspect and check the correctness of masking
             z = target.clone()
@@ -438,15 +442,15 @@
     parser = transformers.HfArgumentParser(
         (HiFTArguments, DataArguments, TrainingArguments)
     )
     model_args, data_args, training_args = parser.parse_args_into_dataclasses()
     local_rank = training_args.local_rank
 
     model_class, tokenizer_class,model_config = MODEL_CLASSES[model_args.model_type]
-    # Set RoPE scaling factor
+    
     config = model_config.from_pretrained(
         model_args.config_name if model_args.config_name else model_args.model_name_or_path,
         cache_dir=model_args.cache_dir,
         revision=model_args.model_revision,
         use_auth_token=True if model_args.use_auth_token else None,
     )
     orig_ctx_len = getattr(config, "max_position_embeddings", None)
```

### Comparing `HiFT-0.0.2/hift/optimizers/adagrad.py` & `HiFT-0.0.3/hift/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/__init__.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/__init__.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/adagrad.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/adagrad.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/adam.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/adam.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/adamw.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/adamw.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/lamb.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/lamb.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/lars.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/lars.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/lion.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/lion.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/rmsprop.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/rmsprop.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/bitsandbytes/sgd.py` & `HiFT-0.0.3/hift/optimizers/bitsandbytes/sgd.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/optimization.py` & `HiFT-0.0.3/hift/optimizers/optimization.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/optimizer.py` & `HiFT-0.0.3/hift/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/rmsprop.py` & `HiFT-0.0.3/hift/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/sgd.py` & `HiFT-0.0.3/hift/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/torchAdam.py` & `HiFT-0.0.3/hift/optimizers/torchAdam.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/optimizers/torchAdamw.py` & `HiFT-0.0.3/hift/optimizers/torchAdamw.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/qatrainer.py` & `HiFT-0.0.3/hift/qatrainer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/registerCallBack.py` & `HiFT-0.0.3/hift/registerCallBack.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,16 +55,14 @@
         special_layers.extend(self.others_pattern)
         special_layers.extend(self.causal_head)
         return special_layers
     def check_selection(self,elements,name_search):
         if len(name_search)<=0:
             return False
         elements = elements = [element if '\\' in element else re.escape(element) for element in elements]
-        # print("elements",elements)
-        # print("name_search",name_search)
         signal_value = [1 if len(re.compile(element).findall(name_search[0]))>0 else 0 for element in elements]
         if sum(signal_value)<=0:
             return False
         else:
             return True
     def check_task_type(self,taskType,model_name,TaskTInterface):
         logger.warning("For {} the HiTaskType should be {}".format(model_name," , ".join(TaskTInterface)))
@@ -102,19 +100,17 @@
             random.shuffle(group_parameters)
         elif self.strategy != "down2up":
             raise ValueError("providing proper strategy")
         print(group_parameters)
         return group_parameters
 
 class RobertaCallBack(HiFTCallBack):
-    LayerNumbers = {"lora":5,"adalora":5,"ia3":5,"p_tuning":3,"prefix_tuning":5,"prompt_tuning":-1}
     def __init__(self,freeze_layers,strategy,taskType,peft_type=None):
         super().__init__(freeze_layers,strategy,taskType,peft_type)
         self.TaskTInterface = [TaskType.SEQ_CLS,TaskType.TOKEN_CLS,TaskType.QUESTION_ANS]
-        # self.number_position = RobertaCallBack.LayerNumbers[peft_type] if peft_type else 3
         self.check_task_type(taskType,"RoBERTa",self.TaskTInterface)
     @property
     def emb_pattern(self):
         if self.peft_type:
             return [rf'\.embedding\.']
         else:
             return [rf'\.embeddings\.']
@@ -139,19 +135,17 @@
     @property
     def others_pattern(self):
         if self.peft_type:
             return [rf'\.\d+\.']
         else:
             return [rf'\.\d+\.']
 class BERTCallBack(HiFTCallBack):
-    LayerNumbers = {"lora":5,"adalora":5,"ia3":5,"p_tuning":3,"prefix_tuning":5,"prompt_tuning":-1}
     def __init__(self,freeze_layers,strategy,taskType,peft_type=None):
         super().__init__(freeze_layers,strategy,taskType,peft_type)
         self.TaskTInterface = [TaskType.SEQ_CLS,TaskType.TOKEN_CLS,TaskType.QUESTION_ANS]
-        # self.number_position = BERTCallBack.LayerNumbers[peft_type] if peft_type else 3
         self.check_task_type(taskType,"BERTa",self.TaskTInterface)
     @property
     def emb_pattern(self):
         if self.peft_type:
             return [rf'\.embedding\.']
         else:
             return [rf'\.embeddings\.']
@@ -176,19 +170,17 @@
     @property
     def others_pattern(self):
         if self.peft_type:
             return [rf'\.\d+\.']
         else:
             return [rf'\.\d+\.']
 class GPT2CallBack(HiFTCallBack):
-    LayerNumbers = {"lora":4,"adalora":4,"ia3":4,"p_tuning":3,"prefix_tuning":4,"prompt_tuning":-1}
     def __init__(self,freeze_layers,strategy,taskType,peft_type=None):
         super().__init__(freeze_layers,strategy,taskType,peft_type)
         self.TaskTInterface = [TaskType.SEQ_CLS,TaskType.TOKEN_CLS,TaskType.QUESTION_ANS,TaskType.CAUSAL_LM]
-        # self.number_position = GPT2CallBack.LayerNumbers[peft_type] if peft_type else 2
         self.check_task_type(taskType,"GPT2",self.TaskTInterface)
     def merge_param(self,group_parameters):
         group_parameters = self.emb_pattern + [param for param in group_parameters if len(re.compile(self.emb_pattern[0]).findall(param))<=0]
         
         return group_parameters
     @property
     def emb_pattern(self):
@@ -224,19 +216,17 @@
     def others_pattern(self):
         if self.peft_type:
             return [rf'\.\d+\.']
         else:
             return [rf'\.\d+\.']
             
 class GPTNeoXCallBack(HiFTCallBack):
-    LayerNumbers = {"lora":4,"adalora":4,"ia3":4,"p_tuning":3,"prefix_tuning":4,"prompt_tuning":-1}
     def __init__(self,freeze_layers,strategy,taskType,peft_type=None):
         super().__init__(freeze_layers,strategy,taskType,peft_type)
         self.TaskTInterface = [TaskType.SEQ_CLS,TaskType.TOKEN_CLS,TaskType.QUESTION_ANS,TaskType.CAUSAL_LM]
-        # self.number_position = GPTNeoXCallBack.LayerNumbers[peft_type] if peft_type else 2
         self.check_task_type(taskType,"GPTNeoX",self.TaskTInterface)
     def merge_param(self,group_parameters):
         group_parameters = self.emb_pattern + [param for param in group_parameters if len(re.compile(self.emb_pattern[0]).findall(param))<=0]
         
         return group_parameters
     @property
     def emb_pattern(self):
@@ -272,19 +262,17 @@
     def others_pattern(self):
         if self.peft_type:
             return [rf'\.\d+\.']
         else:
             return [rf'\.\d+\.']
 
 class OPTCallBack(HiFTCallBack):
-    LayerNumbers = {"lora":5,"adalora":5,"ia3":5,"p_tuning":3,"prefix_tuning":5,"prompt_tuning":-1}
     def __init__(self,freeze_layers,strategy,taskType,peft_type=None):
         super().__init__(freeze_layers,strategy,taskType,peft_type)
         self.TaskTInterface = [TaskType.SEQ_CLS,TaskType.QUESTION_ANS,TaskType.CAUSAL_LM]
-        # self.number_position = OPTCallBack.LayerNumbers[peft_type] if peft_type else 3
         self.check_task_type(taskType,"OPT",self.TaskTInterface)
     
     def merge_param(self,group_parameters):
         group_parameters = self.emb_pattern + [param for param in group_parameters if len(re.compile(self.emb_pattern[0]).findall(param))<=0]
         return group_parameters
     @property
     def emb_pattern(self):
@@ -314,38 +302,36 @@
     def others_pattern(self):
         if self.peft_type:
             return [rf'\.\d+\.']
         else:
             return [rf'\.\d+\.']
 
 class LLaMaFamilyCallBack(HiFTCallBack):
-    LayerNumbers = {"lora":4,"adalora":4,"ia3":4,"p_tuning":3,"prefix_tuning":4,"prompt_tuning":-1}
     def __init__(self,freeze_layers,strategy,taskType,peft_type=None):
         super().__init__(freeze_layers,strategy,taskType,peft_type)
         self.TaskTInterface = [TaskType.SEQ_CLS,TaskType.CAUSAL_LM]
-        # self.number_position = OPTCallBack.LayerNumbers[peft_type] if peft_type else 2
         self.check_task_type(taskType,"LLaMA",self.TaskTInterface)
     @property
     def emb_pattern(self):
         if self.peft_type:
             return [rf"\.embedding\."]
         else:
             return ["embed_tokens"]
     @property
     def seq_cls_head(self):
         if self.peft_type:
             return ["score"]
         else:
-            return ["norm","score"]
+            return ["model.norm.weight","score"]
     @property
     def causal_head(self):
         if self.peft_type:
             return ["lm_head"]
         else:
-            return ["norm","lm_head"]
+            return ["model.norm.weight","lm_head"]
     @property
     def others_pattern(self):
         if self.peft_type:
             return [rf'\.\d+\.']
         else:
             return [rf'\.\d+\.']
```

### Comparing `HiFT-0.0.2/hift/seqtrainer.py` & `HiFT-0.0.3/hift/seqtrainer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/hift/trainer.py` & `HiFT-0.0.3/hift/trainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,16 +55,15 @@
     is_deepspeed_available,
     is_deepspeed_zero3_enabled
 )
 from transformers.pytorch_utils import (
     ALL_LAYERNORM_LAYERS, 
     is_torch_less_than_1_11)
 from transformers.training_args import (
-    TrainingArguments,
-    OptimizerNames)
+    TrainingArguments)
 from .optimizers.optimization import Adafactor, get_scheduler
 from .optimizers import ExtendOptimizerNames as OptimizerNames
 from transformers.utils.import_utils import (
     is_bitsandbytes_available,
 )
 from transformers.debug_utils import DebugOption, DebugUnderflowOverflow
 ###
@@ -115,14 +114,58 @@
 logger = logging.get_logger(__name__)
 from .optimizers import replace_backward
 
 class PEFTrainer(Trainer):
     def __init__(self,peft_type=None,*args,**kwargs):
         super().__init__(*args, **kwargs)
         self.peft_type = peft_type
+    def create_optimizer(self):
+        """
+        Setup the optimizer.
+
+        We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
+        Trainer's init through `optimizers`, or subclass and override this method in a subclass.
+        """
+        opt_model = self.model_wrapped if is_sagemaker_mp_enabled() else self.model
+        if self.optimizer is None:
+            decay_parameters = self.get_decay_parameter_names(opt_model)
+            optimizer_grouped_parameters = [
+                {
+                    "params": [
+                        p for n, p in opt_model.named_parameters() if (n in decay_parameters and p.requires_grad)
+                    ],
+                    "weight_decay": self.args.weight_decay,
+                },
+                {
+                    "params": [
+                        p for n, p in opt_model.named_parameters() if (n not in decay_parameters and p.requires_grad)
+                    ],
+                    "weight_decay": 0.0,
+                },
+            ]
+
+            optimizer_cls, optimizer_kwargs = PEFTrainer.get_optimizer_cls_and_kwargs(self.args)
+
+            self.optimizer = optimizer_cls(optimizer_grouped_parameters, **optimizer_kwargs)
+            if optimizer_cls.__name__ == "Adam8bit":
+                import bitsandbytes
+
+                manager = bitsandbytes.optim.GlobalOptimManager.get_instance()
+
+                skipped = 0
+                for module in opt_model.modules():
+                    if isinstance(module, nn.Embedding):
+                        skipped += sum({p.data_ptr(): p.numel() for p in module.parameters()}.values())
+                        logger.info(f"skipped {module}: {skipped/2**20}M params")
+                        manager.register_module_override(module, "weight", {"optim_bits": 32})
+                        logger.debug(f"bitsandbytes: will optimize {module} in fp32")
+                logger.info(f"skipped: {skipped/2**20}M params")
+        if is_sagemaker_mp_enabled():
+            self.optimizer = smp.DistributedOptimizer(self.optimizer)
+        return self.optimizer
     def training_step(self, model: nn.Module, inputs: Dict[str, Union[torch.Tensor, Any]]) -> torch.Tensor:
         return super().training_step(model, inputs)
     def _inner_training_loop(
         self, batch_size=None, args=None, resume_from_checkpoint=None, trial=None, ignore_keys_for_eval=None
     ):
         self.accelerator.free_memory()
         self._train_batch_size = batch_size
@@ -584,14 +627,212 @@
 
         # After training we make sure to retrieve back the original forward pass method
         # for the embedding layer by removing the forward post hook.
         if self.neftune_noise_alpha is not None:
             self._deactivate_neftune(self.model)
 
         return TrainOutput(self.state.global_step, train_loss, metrics)
+
+    @staticmethod
+    def get_optimizer_cls_and_kwargs(args: TrainingArguments) -> Tuple[Any, Any]:
+        """
+        Returns the optimizer class and optimizer parameters based on the training arguments.
+
+        Args:
+            args (`transformers.training_args.TrainingArguments`):
+                The training arguments for the training session.
+
+        """
+
+        for optimizer in OptimizerNames:
+            print(optimizer.name, optimizer.value)
+        # parse args.optim_args
+        optim_args = {}
+        if args.optim_args:
+            for mapping in args.optim_args.replace(" ", "").split(","):
+                key, value = mapping.split("=")
+                optim_args[key] = value
+
+        optimizer_kwargs = {"lr": args.learning_rate}
+
+        adam_kwargs = {
+            "betas": (args.adam_beta1, args.adam_beta2),
+            "eps": args.adam_epsilon,
+        }
+        if args.optim == OptimizerNames.ADAFACTOR:
+            optimizer_cls = Adafactor
+            optimizer_kwargs.update({"scale_parameter": False, "relative_step": False})
+        elif args.optim == OptimizerNames.ADAMW_HF:
+            from .optimizers.optimization import AdamW
+
+            optimizer_cls = AdamW
+            optimizer_kwargs.update(adam_kwargs)
+        elif args.optim in [OptimizerNames.ADAMW_TORCH, OptimizerNames.ADAMW_TORCH_FUSED]:
+            from .optimizers.torchAdamw import AdamW
+
+            optimizer_cls = AdamW
+            optimizer_kwargs.update(adam_kwargs)
+            if args.optim == OptimizerNames.ADAMW_TORCH_FUSED:
+                optimizer_kwargs.update({"fused": True})
+        elif args.optim == OptimizerNames.ADAMW_TORCH_XLA:
+            try:
+                from torch_xla.amp.syncfree import AdamW
+
+                optimizer_cls = AdamW
+                optimizer_kwargs.update(adam_kwargs)
+            except ImportError:
+                raise ValueError("Trainer failed to import syncfree AdamW from torch_xla.")
+        elif args.optim == OptimizerNames.ADAMW_TORCH_NPU_FUSED:
+            try:
+                from torch_npu.optim import NpuFusedAdamW
+
+                optimizer_cls = NpuFusedAdamW
+                optimizer_kwargs.update(adam_kwargs)
+            except ImportError:
+                raise ValueError("Trainer failed to import FusedAdamW from torch_npu.")
+        elif args.optim == OptimizerNames.ADAMW_APEX_FUSED:
+            try:
+                from apex.optimizers import FusedAdam
+
+                optimizer_cls = FusedAdam
+                optimizer_kwargs.update(adam_kwargs)
+            except ImportError:
+                raise ValueError("Trainer tried to instantiate apex FusedAdam but apex is not installed!")
+        
+        elif args.optim in [
+            OptimizerNames.ADAMW_BNB,
+            OptimizerNames.ADAMW_8BIT,
+            OptimizerNames.PAGED_ADAMW,
+            OptimizerNames.PAGED_ADAMW_8BIT,
+            OptimizerNames.LION,
+            OptimizerNames.LION_8BIT,
+            OptimizerNames.PAGED_LION,
+            OptimizerNames.PAGED_LION_8BIT,
+        ]:
+            from .optimizers import BitAdamW, BitLion
+            is_paged = False
+            optim_bits = 32
+            optimizer_cls = None
+            additional_optim_kwargs = adam_kwargs
+            if "paged" in args.optim:
+                is_paged = True
+            if "8bit" in args.optim:
+                optim_bits = 8
+            if "adam" in args.optim:
+                optimizer_cls = BitAdamW
+            elif "lion" in args.optim:
+                optimizer_cls = BitLion
+                additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
+            bnb_kwargs = {"is_paged": is_paged, "optim_bits": optim_bits}
+            optimizer_kwargs.update(additional_optim_kwargs)
+            optimizer_kwargs.update(bnb_kwargs)
+        elif args.optim in [
+            OptimizerNames.ADAM,
+            OptimizerNames.ADAM_32BIT,
+            OptimizerNames.ADAM_8BIT,
+            OptimizerNames.PAGED_ADAM,
+            OptimizerNames.PAGED_ADAM_32BIT,
+            OptimizerNames.PAGED_ADAM_8BIT
+        ]:
+            from .optimizers import Adam32bit,Adam8bit,PagedAdam8bit,PagedAdam32bit
+            
+            additional_optim_kwargs = adam_kwargs
+            if "paged" in args.optim:
+                if "8bit" in args.optim:
+                    optimizer_cls = PagedAdam8bit
+                else:
+                    optimizer_cls = PagedAdam32bit
+            else:
+                if "8bit" in args.optim:
+                    optimizer_cls = Adam8bit
+                else:
+                    optimizer_cls = Adam32bit
+            optimizer_kwargs.update(additional_optim_kwargs)
+        elif args.optim in [
+            OptimizerNames.LAMB,
+            OptimizerNames.LAMB_32BIT,
+            OptimizerNames.LAMB_8BIT
+        ]:
+            from .optimizers import BitLAMB,LAMB32bit,LAMB8bit
+            if "8bit" in args.optim:
+                optimizer_cls = LAMB8bit
+            else:
+                ## bitsandbytes only support 8-bit lamb
+                optimizer_cls = LAMB8bit
+            additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
+            optimizer_kwargs.update(additional_optim_kwargs)
+        elif args.optim in [
+            OptimizerNames.LARS,
+            OptimizerNames.LARS_32BIT,
+            OptimizerNames.LARS_8BIT
+        ]:
+            from .optimizers import BitLARS,LARS8bit,LARS32bit
+            if "8bit" in args.optim:
+                optimizer_cls = LARS8bit
+            else:
+                ## bitsandbytes only support 8-bit lars
+                optimizer_cls = LARS8bit
+            additional_optim_kwargs = {"momentum": args.adam_beta1}
+            optimizer_kwargs.update(additional_optim_kwargs)
+        elif args.optim in [
+            OptimizerNames.BSGD,
+            OptimizerNames.BSGD_32BIT,
+            OptimizerNames.BSGD_8BIT
+        ]:
+            from .optimizers import BitSGD,SGD8bit,SGD32bit
+            if "8bit" in args.optim:
+                optimizer_cls = SGD8bit
+            else:
+                ## bitsandbytes only support 8-bit lars
+                optimizer_cls = SGD32bit
+        elif args.optim in [
+            OptimizerNames.BRMSPROP,
+            OptimizerNames.BRMSPROP_32BIT,
+            OptimizerNames.BRMSPROP_8BIT
+        ]:
+            from .optimizers import BitRMSprop,RMSprop8bit,RMSprop32bit
+            if "8bit" in args.optim:
+                optimizer_cls = RMSprop8bit
+            else:
+                ## bitsandbytes only support 8-bit lars
+                optimizer_cls = RMSprop32bit
+        elif args.optim == OptimizerNames.ADAMW_ANYPRECISION:
+            try:
+                from torchdistx.optimizers import AnyPrecisionAdamW
+
+                optimizer_cls = AnyPrecisionAdamW
+                optimizer_kwargs.update(adam_kwargs)
+
+                # TODO Change dtypes back to M=FP32, Var = BF16, Kahan = False once they can be cast together in torchdistx.
+                optimizer_kwargs.update(
+                    {
+                        "use_kahan_summation": strtobool(optim_args.get("use_kahan_summation", "False")),
+                        "momentum_dtype": getattr(torch, optim_args.get("momentum_dtype", "float32")),
+                        "variance_dtype": getattr(torch, optim_args.get("variance_dtype", "float32")),
+                        "compensation_buffer_dtype": getattr(
+                            torch, optim_args.get("compensation_buffer_dtype", "bfloat16")
+                        ),
+                    }
+                )
+            except ImportError:
+                raise ValueError("Please install https://github.com/pytorch/torchdistx")
+        elif args.optim == OptimizerNames.SGD:
+            from .optimizers.sgd import SGD
+            optimizer_cls = SGD
+        
+        elif args.optim == OptimizerNames.ADAGRAD:
+            from .optimizers.adagrad import Adagrad
+            optimizer_cls = Adagrad
+        elif args.optim == OptimizerNames.RMSPROP:
+            from .optimizers.rmsprop import RMSprop
+            optimizer_cls = RMSprop
+        else:
+            raise ValueError(f"Trainer cannot instantiate unsupported optimizer: {args.optim}")
+        logger.info(f"the optimizer you are using: {optimizer_cls}")
+        return optimizer_cls, optimizer_kwargs
     
 
 class HiFTrainer(Trainer):
     def __init__(self,
                 hiFThandler,
                 HiTaskType,
                 group_element=1,
@@ -1250,75 +1491,112 @@
             try:
                 from apex.optimizers import FusedAdam
 
                 optimizer_cls = FusedAdam
                 optimizer_kwargs.update(adam_kwargs)
             except ImportError:
                 raise ValueError("Trainer tried to instantiate apex FusedAdam but apex is not installed!")
+        
         elif args.optim in [
             OptimizerNames.ADAMW_BNB,
             OptimizerNames.ADAMW_8BIT,
             OptimizerNames.PAGED_ADAMW,
             OptimizerNames.PAGED_ADAMW_8BIT,
             OptimizerNames.LION,
             OptimizerNames.LION_8BIT,
             OptimizerNames.PAGED_LION,
             OptimizerNames.PAGED_LION_8BIT,
+        ]:
+            from .optimizers import BitAdamW, BitLion
+            is_paged = False
+            optim_bits = 32
+            optimizer_cls = None
+            additional_optim_kwargs = adam_kwargs
+            if "paged" in args.optim:
+                is_paged = True
+            if "8bit" in args.optim:
+                optim_bits = 8
+            if "adam" in args.optim:
+                optimizer_cls = BitAdamW
+            elif "lion" in args.optim:
+                optimizer_cls = BitLion
+                additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
+            bnb_kwargs = {"is_paged": is_paged, "optim_bits": optim_bits}
+            optimizer_kwargs.update(additional_optim_kwargs)
+            optimizer_kwargs.update(bnb_kwargs)
+        elif args.optim in [
+            OptimizerNames.ADAM,
+            OptimizerNames.ADAM_32BIT,
+            OptimizerNames.ADAM_8BIT,
+            OptimizerNames.PAGED_ADAM,
+            OptimizerNames.PAGED_ADAM_32BIT,
+            OptimizerNames.PAGED_ADAM_8BIT
+        ]:
+            from .optimizers import Adam32bit,Adam8bit,PagedAdam8bit,PagedAdam32bit
+            
+            additional_optim_kwargs = adam_kwargs
+            if "paged" in args.optim:
+                if "8bit" in args.optim:
+                    optimizer_cls = PagedAdam8bit
+                else:
+                    optimizer_cls = PagedAdam32bit
+            else:
+                if "8bit" in args.optim:
+                    optimizer_cls = Adam8bit
+                else:
+                    optimizer_cls = Adam32bit
+            optimizer_kwargs.update(additional_optim_kwargs)
+        elif args.optim in [
             OptimizerNames.LAMB,
-            OptimizerNames.LAMB_8BIT,
+            OptimizerNames.LAMB_32BIT,
+            OptimizerNames.LAMB_8BIT
+        ]:
+            from .optimizers import BitLAMB,LAMB32bit,LAMB8bit
+            if "8bit" in args.optim:
+                optimizer_cls = LAMB8bit
+            else:
+                ## bitsandbytes only support 8-bit lamb
+                optimizer_cls = LAMB8bit
+            additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
+            optimizer_kwargs.update(additional_optim_kwargs)
+        elif args.optim in [
             OptimizerNames.LARS,
-            OptimizerNames.LARS_8BIT,
-            OptimizerNames.BRMSPROP,
-            OptimizerNames.BRMSPROP_8BIT,
+            OptimizerNames.LARS_32BIT,
+            OptimizerNames.LARS_8BIT
+        ]:
+            from .optimizers import BitLARS,LARS8bit,LARS32bit
+            if "8bit" in args.optim:
+                optimizer_cls = LARS8bit
+            else:
+                ## bitsandbytes only support 8-bit lars
+                optimizer_cls = LARS8bit
+            additional_optim_kwargs = {"momentum": args.adam_beta1}
+            optimizer_kwargs.update(additional_optim_kwargs)
+        elif args.optim in [
             OptimizerNames.BSGD,
-            OptimizerNames.BSGD_8BIT,
-            OptimizerNames.BADAGRAD,
-            OptimizerNames.BADAGRAD_8BIT
+            OptimizerNames.BSGD_32BIT,
+            OptimizerNames.BSGD_8BIT
         ]:
-            try:
-                from .optimizers import BitAdamW, BitLion,BitAdagrad,BitAdam,BitLAMB,BitLARS,BitRMSprop,BitSGD
-
-                is_paged = False
-                optim_bits = 32
-                optimizer_cls = None
-                additional_optim_kwargs = adam_kwargs
-                if "paged" in args.optim:
-                    is_paged = True
-                if "8bit" in args.optim:
-                    optim_bits = 8
-                if "adamw" in args.optim:
-                    optimizer_cls = BitAdamW
-                if "adam" in args.optim:
-                    optimizer_cls = BitAdam
-                elif "lion" in args.optim:
-                    optimizer_cls = BitLion
-                    additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
-                elif "lamb" in args.optim:
-                    optimizer_cls = BitLAMB
-                    additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
-                elif "lars" in args.optim:
-                    optimizer_cls = BitLARS
-                elif "rmsprop" in args.optim:
-                    optimizer_cls = BitRMSprop
-                elif "sgd" in args.optim:
-                    optimizer_cls = BitSGD
-                elif "adagrad" in args.optim:
-                    optimizer_cls = BitAdagrad
-                bnb_kwargs = {"is_paged": is_paged, "optim_bits": optim_bits}
-                optimizer_kwargs.update(additional_optim_kwargs)
-                optimizer_kwargs.update(bnb_kwargs)
-            except ImportError:
-                raise ValueError("Trainer tried to instantiate bnb optimizer but bnb is not installed!")
-            if is_bitsandbytes_available() and version.parse(
-                importlib.metadata.version("bitsandbytes")
-            ) < version.parse("0.41.1"):
-                logger.warning(
-                    "You are using 8-bit optimizers with a version of `bitsandbytes` < 0.41.1. "
-                    "It is recommended to update your version as a major bug has been fixed in 8-bit optimizers."
-                )
+            from .optimizers import BitSGD,SGD8bit,SGD32bit
+            if "8bit" in args.optim:
+                optimizer_cls = SGD8bit
+            else:
+                ## bitsandbytes only support 8-bit lars
+                optimizer_cls = SGD32bit
+        elif args.optim in [
+            OptimizerNames.BRMSPROP,
+            OptimizerNames.BRMSPROP_32BIT,
+            OptimizerNames.BRMSPROP_8BIT
+        ]:
+            from .optimizers import BitRMSprop,RMSprop8bit,RMSprop32bit
+            if "8bit" in args.optim:
+                optimizer_cls = RMSprop8bit
+            else:
+                ## bitsandbytes only support 8-bit lars
+                optimizer_cls = RMSprop32bit
         elif args.optim == OptimizerNames.ADAMW_ANYPRECISION:
             try:
                 from torchdistx.optimizers import AnyPrecisionAdamW
 
                 optimizer_cls = AnyPrecisionAdamW
                 optimizer_kwargs.update(adam_kwargs)
 
@@ -1343,9 +1621,9 @@
             from .optimizers.adagrad import Adagrad
             optimizer_cls = Adagrad
         elif args.optim == OptimizerNames.RMSPROP:
             from .optimizers.rmsprop import RMSprop
             optimizer_cls = RMSprop
         else:
             raise ValueError(f"Trainer cannot instantiate unsupported optimizer: {args.optim}")
-        logger.info(f"the optimizer you are using is {optimizer_cls}")
+        logger.info(f"the optimizer you are using: {optimizer_cls}")
         return optimizer_cls, optimizer_kwargs
```

### Comparing `HiFT-0.0.2/hift/utils/utils.py` & `HiFT-0.0.3/hift/utils/utils.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.2/setup.py` & `HiFT-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="HiFT",
-    version="0.0.2",
+    version="0.0.3",
     author="Yongkang Liu",
     author_email="misonsky@163.com",
     description="PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/misonsky/HiFT",
     packages=setuptools.find_packages(),
```

