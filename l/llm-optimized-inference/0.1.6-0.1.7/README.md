# Comparing `tmp/llm_optimized_inference-0.1.6-py3-none-any.whl.zip` & `tmp/llm_optimized_inference-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,38 @@
-Zip file size: 66548 bytes, number of entries: 36
--rw-rw-r--  2.0 unx      249 b- defN 24-May-07 17:22 llm/__init__.py
--rw-rw-r--  2.0 unx      249 b- defN 24-May-07 17:22 llm/optimized/__init__.py
--rw-rw-r--  2.0 unx      703 b- defN 24-May-07 17:22 llm/optimized/inference/__init__.py
--rw-rw-r--  2.0 unx      204 b- defN 24-May-07 17:22 llm/optimized/inference/_version.py
--rw-rw-r--  2.0 unx    28243 b- defN 24-May-07 17:22 llm/optimized/inference/api_server.py
--rw-rw-r--  2.0 unx     3203 b- defN 24-May-07 17:22 llm/optimized/inference/configs.py
--rw-rw-r--  2.0 unx     5617 b- defN 24-May-07 17:22 llm/optimized/inference/constants.py
--rw-rw-r--  2.0 unx     3255 b- defN 24-May-07 17:22 llm/optimized/inference/conversation.py
--rw-rw-r--  2.0 unx     5802 b- defN 24-May-07 17:22 llm/optimized/inference/fm_score.py
--rw-rw-r--  2.0 unx      664 b- defN 24-May-07 17:22 llm/optimized/inference/logging_config.py
--rw-rw-r--  2.0 unx     9028 b- defN 24-May-07 17:22 llm/optimized/inference/managed_inference.py
--rw-rw-r--  2.0 unx     1369 b- defN 24-May-07 17:22 llm/optimized/inference/model_config_factory.py
--rw-rw-r--  2.0 unx     6638 b- defN 24-May-07 17:22 llm/optimized/inference/model_utils.py
--rw-rw-r--  2.0 unx     1575 b- defN 24-May-07 17:22 llm/optimized/inference/prompt_formatter.py
--rw-rw-r--  2.0 unx    12420 b- defN 24-May-07 17:22 llm/optimized/inference/replica_manager.py
--rw-rw-r--  2.0 unx    18786 b- defN 24-May-07 17:22 llm/optimized/inference/score.py
--rw-rw-r--  2.0 unx     4731 b- defN 24-May-07 17:22 llm/optimized/inference/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-May-07 17:22 llm/optimized/inference/api_server_setup/__init__.py
--rw-rw-r--  2.0 unx     9502 b- defN 24-May-07 17:22 llm/optimized/inference/api_server_setup/openapi.json
--rw-rw-r--  2.0 unx     1878 b- defN 24-May-07 17:22 llm/optimized/inference/api_server_setup/protocol.py
--rw-rw-r--  2.0 unx      131 b- defN 24-May-07 17:22 llm/optimized/inference/custom_model_configurations/__init__.py
--rw-rw-r--  2.0 unx     2725 b- defN 24-May-07 17:22 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
--rw-rw-r--  2.0 unx     8806 b- defN 24-May-07 17:22 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
--rw-rw-r--  2.0 unx     1047 b- defN 24-May-07 17:22 llm/optimized/inference/custom_model_configurations/schema_output.py
--rw-rw-r--  2.0 unx      259 b- defN 24-May-07 17:22 llm/optimized/inference/engine/__init__.py
--rw-rw-r--  2.0 unx    38577 b- defN 24-May-07 17:22 llm/optimized/inference/engine/_hf_predictors.py
--rw-rw-r--  2.0 unx     4583 b- defN 24-May-07 17:22 llm/optimized/inference/engine/engine.py
--rw-rw-r--  2.0 unx     8617 b- defN 24-May-07 17:22 llm/optimized/inference/engine/hf_engine.py
--rw-rw-r--  2.0 unx    10797 b- defN 24-May-07 17:22 llm/optimized/inference/engine/mii_engine.py
--rw-rw-r--  2.0 unx     7971 b- defN 24-May-07 17:22 llm/optimized/inference/engine/mii_engine_v2.py
--rw-rw-r--  2.0 unx    14762 b- defN 24-May-07 17:22 llm/optimized/inference/engine/vllm_engine.py
--rw-rw-r--  2.0 unx        0 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3107 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3599 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/RECORD
-36 files, 219193 bytes uncompressed, 60564 bytes compressed:  72.4%
+Zip file size: 67086 bytes, number of entries: 36
+-rw-rw-r--  2.0 unx      249 b- defN 24-May-15 09:10 llm/__init__.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-May-15 09:10 llm/optimized/__init__.py
+-rw-rw-r--  2.0 unx      703 b- defN 24-May-15 09:10 llm/optimized/inference/__init__.py
+-rw-rw-r--  2.0 unx      204 b- defN 24-May-15 09:10 llm/optimized/inference/_version.py
+-rw-rw-r--  2.0 unx    28243 b- defN 24-May-15 09:10 llm/optimized/inference/api_server.py
+-rw-rw-r--  2.0 unx     3203 b- defN 24-May-15 09:10 llm/optimized/inference/configs.py
+-rw-rw-r--  2.0 unx     7071 b- defN 24-May-15 09:10 llm/optimized/inference/constants.py
+-rw-rw-r--  2.0 unx     3255 b- defN 24-May-15 09:10 llm/optimized/inference/conversation.py
+-rw-rw-r--  2.0 unx     5802 b- defN 24-May-15 09:10 llm/optimized/inference/fm_score.py
+-rw-rw-r--  2.0 unx      664 b- defN 24-May-15 09:10 llm/optimized/inference/logging_config.py
+-rw-rw-r--  2.0 unx     9028 b- defN 24-May-15 09:10 llm/optimized/inference/managed_inference.py
+-rw-rw-r--  2.0 unx     1369 b- defN 24-May-15 09:10 llm/optimized/inference/model_config_factory.py
+-rw-rw-r--  2.0 unx     6814 b- defN 24-May-15 09:10 llm/optimized/inference/model_utils.py
+-rw-rw-r--  2.0 unx     1575 b- defN 24-May-15 09:10 llm/optimized/inference/prompt_formatter.py
+-rw-rw-r--  2.0 unx    12420 b- defN 24-May-15 09:10 llm/optimized/inference/replica_manager.py
+-rw-rw-r--  2.0 unx    18786 b- defN 24-May-15 09:10 llm/optimized/inference/score.py
+-rw-rw-r--  2.0 unx     4731 b- defN 24-May-15 09:10 llm/optimized/inference/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-15 09:10 llm/optimized/inference/api_server_setup/__init__.py
+-rw-rw-r--  2.0 unx     9502 b- defN 24-May-15 09:10 llm/optimized/inference/api_server_setup/openapi.json
+-rw-rw-r--  2.0 unx     1878 b- defN 24-May-15 09:10 llm/optimized/inference/api_server_setup/protocol.py
+-rw-rw-r--  2.0 unx      131 b- defN 24-May-15 09:10 llm/optimized/inference/custom_model_configurations/__init__.py
+-rw-rw-r--  2.0 unx     2725 b- defN 24-May-15 09:10 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
+-rw-rw-r--  2.0 unx     8806 b- defN 24-May-15 09:10 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-May-15 09:10 llm/optimized/inference/custom_model_configurations/schema_output.py
+-rw-rw-r--  2.0 unx      259 b- defN 24-May-15 09:10 llm/optimized/inference/engine/__init__.py
+-rw-rw-r--  2.0 unx    38577 b- defN 24-May-15 09:10 llm/optimized/inference/engine/_hf_predictors.py
+-rw-rw-r--  2.0 unx     4583 b- defN 24-May-15 09:10 llm/optimized/inference/engine/engine.py
+-rw-rw-r--  2.0 unx     8617 b- defN 24-May-15 09:10 llm/optimized/inference/engine/hf_engine.py
+-rw-rw-r--  2.0 unx    10797 b- defN 24-May-15 09:10 llm/optimized/inference/engine/mii_engine.py
+-rw-rw-r--  2.0 unx     7971 b- defN 24-May-15 09:10 llm/optimized/inference/engine/mii_engine_v2.py
+-rw-rw-r--  2.0 unx    16005 b- defN 24-May-15 09:10 llm/optimized/inference/engine/vllm_engine.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-15 09:13 llm_optimized_inference-0.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3107 b- defN 24-May-15 09:13 llm_optimized_inference-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-15 09:13 llm_optimized_inference-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 24-May-15 09:13 llm_optimized_inference-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3599 b- defN 24-May-15 09:13 llm_optimized_inference-0.1.7.dist-info/RECORD
+36 files, 222066 bytes uncompressed, 61102 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -87,23 +87,23 @@
 
 Filename: llm/optimized/inference/engine/mii_engine_v2.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/vllm_engine.py
 Comment: 
 
-Filename: llm_optimized_inference-0.1.6.dist-info/LICENSE
+Filename: llm_optimized_inference-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: llm_optimized_inference-0.1.6.dist-info/METADATA
+Filename: llm_optimized_inference-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: llm_optimized_inference-0.1.6.dist-info/WHEEL
+Filename: llm_optimized_inference-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: llm_optimized_inference-0.1.6.dist-info/top_level.txt
+Filename: llm_optimized_inference-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_optimized_inference-0.1.6.dist-info/RECORD
+Filename: llm_optimized_inference-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llm/optimized/inference/_version.py

```diff
@@ -1,5 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
```

## llm/optimized/inference/api_server.py

 * *Ordering differences only*

```diff
@@ -339,16 +339,16 @@
     updated_params = {}
     # map 'max_gen_len' to 'max_new_tokens' if present
     if "max_gen_len" in params:
         logger.warning("max_gen_len is deprecated. Use max_new_tokens")
         params["max_new_tokens"] = params["max_gen_len"]
         del params["max_gen_len"]
 
-    updated_params.update(params)
     updated_params.update(g_generation_config)
+    updated_params.update(params)
     return updated_params
 
 
 def _init_cuda_visible_devices():
     import torch
 
     if "CUDA_VISIBLE_DEVICES" in os.environ:
```

## llm/optimized/inference/constants.py

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """This module defines the EngineName and TaskType enums."""
 from enum import Enum
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 
 class EngineName(str, Enum):
     """Enum representing the names of the engines."""
 
     HF = "hf"
     VLLM = "vllm"
@@ -92,14 +92,15 @@
         "Qwen2ForCausalLM",
         "RWForCausalLM",
         "StableLmForCausalLM",
         "DbrxForCausalLM",
         "PhiForCausalLM",
         "Phi3ForCausalLM",
         "Phi3SmallForCausalLM",
+        "Phi3VForCausalLM",
         "YakForCausalLM"
     }
 
 
 class MIISupportedModels:
     """MII Supported Models."""
 
@@ -122,37 +123,58 @@
 
 
 class VLLMSpecialModels:
     """Models Types that require additional parameters to work with vllm."""
 
     # TODO: Remove "RefinedWebModel" and "RefinedWeb" once falcon models are updated to latest huggingface commit
 
-    Models = {
+    ModelTypes = {
         "falcon": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "RefinedWebModel": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "RefinedWeb": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "dbrx": {"args": ["trust-remote-code"]},
         "deci_lm": {"args": ["trust-remote-code"]},
         "phi": {"args": ["trust-remote-code"]},
         "phi3": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]},
-        "phi3small": {"args": ["trust-remote-code"]},
+        "phi3small": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]},
+        "phi3_v": {
+            "kwargs": {"tensor-parallel-size": 2, "gpu-memory-utilization": .95,
+                       "image-input-type": "pixel_values", "image-token-id": 32044,
+                       "image-openai": "phi3v_single_image", "image-input-shape": "1,3,336,336",
+                       "image-feature-size": 2509},
+            "args": ["trust-remote-code"]
+        },
         "yak": {"kwargs": {"quantization": "yq"}}
     }
 
+    # Phi-*-128k models may eventually need tp-sizes of 2 instead of 1. For now only Phi-medium-128k has tp_size > 1
+    Models = {
+        "microsoft/phi-3-mini-4k-instruct": {"kwargs": {"tensor-parallel-size": 1}},
+        "microsoft/phi-3-mini-128k-instruct": {"kwargs": {"tensor-parallel-size": 1}},
+        "microsoft/phi-3-small-8k-instruct": {"kwargs": {"tensor-parallel-size": 1}},
+        "microsoft/phi-3-small-128k-instruct": {"kwargs": {"tensor-parallel-size": 1}},
+        "microsoft/phi-3-medium-4k-instruct": {"kwargs": {"tensor-parallel-size": 1}},
+        "microsoft/phi-3-medium-128k-instruct": {"kwargs": {"tensor-parallel-size": 2}}
+    }
+
     @classmethod
-    def get_kwargs(cls, model_type: str) -> Dict:
-        """Get the kwargs the vllm server needs for the model type."""
-        params = cls.Models.get(model_type, {})
-        return params.get("kwargs", {})
+    def get_kwargs(cls, model_type: str, model_name: Optional[str]) -> Dict:
+        """Get the kwargs the vllm server needs for the given model."""
+        kwargs = cls.ModelTypes.get(model_type, {}).get("kwargs", {})
+        model_specific_kwargs = cls.Models.get(model_name, {}).get("kwargs", {})
+        kwargs.update(model_specific_kwargs)
+        return kwargs
 
     @classmethod
-    def get_args(cls, model_type: str) -> List:
-        """Get the args the vllm server needs for the model type."""
-        params = cls.Models.get(model_type, {})
-        return params.get("args", [])
+    def get_args(cls, model_type: str, model_name: Optional[str]) -> List:
+        """Get the args the vllm server needs for the given model."""
+        args = cls.ModelTypes.get(model_type, {}).get("args", [])
+        model_specific_args = cls.Models.get(model_name, {}).get("args", [])
+        args.extend(model_specific_args)
+        return args
 
 
 ALL_TASKS = [
     SupportedTask.TEXT_TO_IMAGE,
     SupportedTask.TEXT_CLASSIFICATION,
     SupportedTask.TEXT_CLASSIFICATION_MULTILABEL,
     SupportedTask.NER,
```

## llm/optimized/inference/model_utils.py

```diff
@@ -101,33 +101,34 @@
         elif "hftransformersv2" in flavors:
             task_type = flavors["hftransformersv2"]["task_type"]
             ml_model_info = flavors["hftransformersv2"].copy()
             if task_type not in ALL_TASKS:
                 raise Exception(f"Unsupported task_type {task_type}")
         elif "python_function" in flavors:
             task_type = mlmodel["metadata"]["base_model_task"]
-            if task_type not in [TaskType.TEXT_TO_IMAGE, TaskType.TEXT_TO_IMAGE_INPAINTING]:
+            if task_type not in [TaskType.TEXT_TO_IMAGE, TaskType.TEXT_TO_IMAGE_INPAINTING, TaskType.CHAT_COMPLETION]:
                 raise Exception(f"Unsupported task_type {task_type}")
 
-            model_type = mlmodel["metadata"].get("model_type", "")
+            if task_type in [TaskType.TEXT_TO_IMAGE, TaskType.TEXT_TO_IMAGE_INPAINTING]:
+                model_type = mlmodel["metadata"].get("model_type", "")
 
-            model_config_builder = ModelConfigFactory.get_config_builder(task=task_type, model_type=model_type)
-            engine_config.update(
-                {
-                    "engine_name": model_config_builder.engine,
-                    "mii_config": model_config_builder.get_optimization_config(),
-                    "custom_model_config_builder": model_config_builder,
-                    "model_id": os.path.join(os.getenv("AZUREML_MODEL_DIR", ""), model_config_builder.model_path),
-                    "tokenizer": os.path.join(os.getenv("AZUREML_MODEL_DIR", ""),
-                                              model_config_builder.MLFLOW_MODEL_PATH,
-                                              "tokenizer"),
-                    "tensor_parallel": model_config_builder.tensor_parallel
-                }
-            )
-            task_config = model_config_builder.get_task_config()
+                model_config_builder = ModelConfigFactory.get_config_builder(task=task_type, model_type=model_type)
+                engine_config.update(
+                    {
+                        "engine_name": model_config_builder.engine,
+                        "mii_config": model_config_builder.get_optimization_config(),
+                        "custom_model_config_builder": model_config_builder,
+                        "model_id": os.path.join(os.getenv("AZUREML_MODEL_DIR", ""), model_config_builder.model_path),
+                        "tokenizer": os.path.join(os.getenv("AZUREML_MODEL_DIR", ""),
+                                                  model_config_builder.MLFLOW_MODEL_PATH,
+                                                  "tokenizer"),
+                        "tensor_parallel": model_config_builder.tensor_parallel
+                    }
+                )
+                task_config = model_config_builder.get_task_config()
 
     if task_type != TaskType.TEXT_TO_IMAGE:
         if engine_config["engine_name"] in [EngineName.MII, EngineName.VLLM] and task_type not in VLLM_MII_TASKS:
             engine_config["engine_name"] = EngineName.HF
 
     if engine_config["engine_name"] == EngineName.MII or engine_config["engine_name"] == EngineName.MII_V1:
         mii_engine_config = {
```

## llm/optimized/inference/engine/vllm_engine.py

```diff
@@ -103,25 +103,35 @@
             )
         if "model" not in self._vllm_args:
             self._vllm_args["model"] = self.engine_config.model_id
 
         if "tokenizer" not in self._vllm_args:
             self._vllm_args["tokenizer"] = self.engine_config.tokenizer
 
+        model_name = self.engine_config.ml_model_info.get("model_id", None)
+        kwargs = VLLMSpecialModels.get_kwargs(self._model_type, model_name)
+        args = VLLMSpecialModels.get_args(self._model_type, model_name)
+
+        if "tensor-parallel-size" in kwargs:
+            user_tensor_parallel = os.getenv("TENSOR_PARALLEL", None)
+            
+            # Use user's tensor parallel size only if it is bigger than than default tensor-parallel
+            if user_tensor_parallel:
+                custom_tensor_parallel = kwargs["tensor-parallel-size"]
+                try:
+                    user_tensor_parallel = int(user_tensor_parallel)
+                except:
+                    user_tensor_parallel = custom_tensor_parallel
+                kwargs.update({"tensor-parallel-size": max(user_tensor_parallel, custom_tensor_parallel)})
+                if user_tensor_parallel < custom_tensor_parallel:
+                    logger.info(f"TENSOR_PARALLEL was set to {user_tensor_parallel}. The model {model_name} requires a"
+                                f" tensor parallel of {custom_tensor_parallel} and will be deployed with a tensor "
+                                f"parallel of {custom_tensor_parallel}. Consider increasing TENSOR_PARALLEL to be "
+                                f"equal to or greater than {custom_tensor_parallel}")
 
-        kwargs = VLLMSpecialModels.get_kwargs(self._model_type)
-        args = VLLMSpecialModels.get_args(self._model_type)
-        if self._model_type == "phi3":
-            full_model_name = self.engine_config.ml_model_info.get("model_id", None)
-
-            # Phi-3 models share the same model type names but phi-3-medium-128k requires a different
-            # tensor parallel size than the other Phi-3 models
-            if full_model_name == "microsoft/phi-3-medium-128k-instruct":
-                kwargs.update({"tensor-parallel-size": 2})
-    
         self._vllm_args.update(kwargs)
         self._vllm_additional_args.extend(args)
         self._vllm_additional_args.append("disable-log-requests")
 
     def _verify_and_convert_float_type(self):
         """Check to see whether the model's float type is compatible with the compute type selected.
 
@@ -143,35 +153,41 @@
                     f"{compute_capability[0]}.{compute_capability[1]}. "
                     f"bfloat16 will be converted to float16.",
                 )
 
     def _verify_and_modify_tensor_parallel_size(self):
         """Check to see if the tensor parallel size is compatible with the models's number of attention heads."""
         num_attention_heads = self._model_config.get("num_attention_heads", 1)
+        num_key_value_heads = self._model_config.get("num_key_value_heads", 1)
 
         # TODO: Remove if statement once falcon models are updated to latest huggingface commit
-        if self._model_type == "RefinedWebModel" or self._model_type == "RefinedWeb":
+        if self._model_type == "falcon" or self._model_type == "RefinedWebModel" or self._model_type == "RefinedWeb":
             num_attention_heads = self._model_config.get("n_head", 1)
-        
+            num_key_value_heads = (
+                1 
+                if self._model_config.get("multi_query", False) 
+                else self._model_config.get("n_head_kv", 1)
+            )
         if self._model_type == "dbrx":
             num_attention_heads = self._model_config.get("n_heads", 1)
+            num_key_value_heads = self._model_config.get("attn_config", {}).get("kv_n_heads", 1)
 
         tensor_parallel_size = self._vllm_args["tensor-parallel-size"]
         new_tensor_parallel_size = tensor_parallel_size
         if tensor_parallel_size != 0:
-            while num_attention_heads % new_tensor_parallel_size != 0:
+            while (num_attention_heads % new_tensor_parallel_size != 0 or 
+                   num_key_value_heads % new_tensor_parallel_size != 0):
                 new_tensor_parallel_size -= 1
         if tensor_parallel_size != new_tensor_parallel_size:
             logger.warning(
-                "Tensor parallel size was incompatible with the number of attention heads the model has. "
-                f"Number of attention heads ({num_attention_heads}) must be divisible by "
-                f"tensor-parallel-size ({tensor_parallel_size}). To make them compatible, "
-                f"tensor-parallel-size was reduced from {tensor_parallel_size} to "
-                f"{new_tensor_parallel_size}. If deploying Falcon-7b or Falcon-7b-Instruct, consider "
-                "choosing a Standard_NC6s_v3 sku as tensor-parallel-size must be 1 for those models.",
+                f"Tensor parallel size was incompatible with either the number of attention heads or the number of "
+                f"key value heads the model has in its config.json. Number of attention heads ({num_attention_heads})"
+                f" and number of key value heads ({num_key_value_heads}) must be divisible by tensor-parallel-size "
+                f"({tensor_parallel_size}). To make them compatible, tensor-parallel-size was reduced from "
+                f"{tensor_parallel_size} to {new_tensor_parallel_size}."
             )
         self._vllm_args["tensor-parallel-size"] = new_tensor_parallel_size
 
     def _start_server(self, server_kwargs: Dict, server_args: List, env: Dict):
         """Start the VLLM server with the given arguments."""
         cmd = ["python", "-m", "vllm.entrypoints.api_server"]
         cmd.extend([f"--{k}={v}" for k, v in server_kwargs.items()])
```

## Comparing `llm_optimized_inference-0.1.6.dist-info/METADATA` & `llm_optimized_inference-0.1.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-optimized-inference
-Version: 0.1.6
+Version: 0.1.7
 Home-page: 
 Author: Microsoft
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `llm_optimized_inference-0.1.6.dist-info/RECORD` & `llm_optimized_inference-0.1.7.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 llm/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/inference/__init__.py,sha256=rGZODP-qE2NOlUgdbmxhfuS3svmx9gM-kU97d9-jb50,703
-llm/optimized/inference/_version.py,sha256=E33LCXtRMMIS-GExLNxF_yCpQ1D-zJrxuCDiZv6aGI4,204
-llm/optimized/inference/api_server.py,sha256=kyUIykJuk9jPajQyUqqMl4FEQKLZV57LykfGY0Z99Ak,28243
+llm/optimized/inference/_version.py,sha256=CAbM--HL8LeeWoO-6se_tFB4w6PBXJyYx-rammaJ6S4,204
+llm/optimized/inference/api_server.py,sha256=4-u4nLP5coq0h4Z1iNgFP2fDWwcIdn6e77WtcE74gZg,28243
 llm/optimized/inference/configs.py,sha256=d5NKbQlfYVkUQ4SL03KVBQekdOG4VrcD0xGxVeHESeQ,3203
-llm/optimized/inference/constants.py,sha256=8hpMpT0RwWeqqKoAa4TTD0MXQNdq5bpcwBXF0JdaCcc,5617
+llm/optimized/inference/constants.py,sha256=t_KwZlui9K9Rr_c9ocOioTRosDobFsIVIxT_EZdgYSw,7071
 llm/optimized/inference/conversation.py,sha256=cBrHv1sI1hrOQB57sSZKAarplKRgqQWqmYxT-wkZHLM,3255
 llm/optimized/inference/fm_score.py,sha256=7z7ZbLMXUXH6gp1-G_l3rOus9r9vSpIm5-wOj5X17aQ,5802
 llm/optimized/inference/logging_config.py,sha256=egtAiGCNVNoU8E_JPhp2aGJVIJ_QkTwLhkNjpVKjICI,664
 llm/optimized/inference/managed_inference.py,sha256=O_HlOPNl24Uoy68gFKrSM_gOG-rg4P_lishBQFAXyC8,9028
 llm/optimized/inference/model_config_factory.py,sha256=EpHH8QyUaE5DC6A5O5nKbie_kMEpfeqmufbOn0U6jFI,1369
-llm/optimized/inference/model_utils.py,sha256=W9nLxInrhuPnmhvZldBpS2POB7-u_SST7ostxatAYrA,6638
+llm/optimized/inference/model_utils.py,sha256=-PzBYNX9PCmmIKlxH4J4E7BDHKHU63nW6x_VH03oX_c,6814
 llm/optimized/inference/prompt_formatter.py,sha256=xxM4MbvvPL6jQcLB37uKA9-wCHXTZUL9l5GiUu3r964,1575
 llm/optimized/inference/replica_manager.py,sha256=AUQn9IWFgdsHEQpHDqQVMjnGdZFdzr55IQnVmXFHefA,12420
 llm/optimized/inference/score.py,sha256=RWEaCZ4Akig88ErqshDD8KFCF-YDwMJvsRJjeBWR-WM,18786
 llm/optimized/inference/utils.py,sha256=STENfqDoR8otc2Ig8MN-nERR-y6O6Nl3gpIOZ8A8fbo,4731
 llm/optimized/inference/api_server_setup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 llm/optimized/inference/api_server_setup/openapi.json,sha256=SMtuKvJK58zuxDig48iZ2GMggHxvCpBx5KgYXVAWtoA,9502
 llm/optimized/inference/api_server_setup/protocol.py,sha256=0WmY2-1iQrCsDXXanqIwM7klNBU3skm6tZMxOMPTrWk,1878
@@ -24,13 +24,13 @@
 llm/optimized/inference/custom_model_configurations/schema_output.py,sha256=JIpThLkAPoO7MlhaJVSxP2RYVwYzIpw3R3k-nraLq9k,1047
 llm/optimized/inference/engine/__init__.py,sha256=8GqGW53dbRlGShwO11h5HQH4KjnUzoW0t0cChUUFDPY,259
 llm/optimized/inference/engine/_hf_predictors.py,sha256=AwQTIpmOHb7h31H2DF2Jx-9b03lcB5DOrgSbXGpamIk,38577
 llm/optimized/inference/engine/engine.py,sha256=xbpEVJBjovFyACw6WF8uqnmyodRWqb52oaR3s3pr8Sc,4583
 llm/optimized/inference/engine/hf_engine.py,sha256=4rRldNod-pMDJ_-3q0RDWEkigCTr6I62HyJspb01lAs,8617
 llm/optimized/inference/engine/mii_engine.py,sha256=TBfc_wt4-NKTzkjHCie5YpqRGS6pvBNigyYpTHt_jII,10797
 llm/optimized/inference/engine/mii_engine_v2.py,sha256=rI4tjRyj-dCZBDAiN0YNPKMBtkD3MXxcbucuSlHg6lI,7971
-llm/optimized/inference/engine/vllm_engine.py,sha256=_-q0S8ewaLJR7dN0I2nTY19hbuqwD4SOxVGibJc4Y4k,14762
-llm_optimized_inference-0.1.6.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-llm_optimized_inference-0.1.6.dist-info/METADATA,sha256=H9_Ix9Km_7FfmJFeTbnQO40MYTtDj_a64zb-F-0Yg8I,3107
-llm_optimized_inference-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-llm_optimized_inference-0.1.6.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
-llm_optimized_inference-0.1.6.dist-info/RECORD,,
+llm/optimized/inference/engine/vllm_engine.py,sha256=rCbYccKLwxYo92n_n4USs5zgQJq04fYnfvWihsIRltA,16005
+llm_optimized_inference-0.1.7.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+llm_optimized_inference-0.1.7.dist-info/METADATA,sha256=Hd2D_m1-BGNQtUYE5-pYm0TxxlYYg8wlbWkOeqFtJUU,3107
+llm_optimized_inference-0.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+llm_optimized_inference-0.1.7.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
+llm_optimized_inference-0.1.7.dist-info/RECORD,,
```

