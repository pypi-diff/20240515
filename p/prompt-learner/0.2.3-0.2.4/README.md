# Comparing `tmp/prompt_learner-0.2.3.tar.gz` & `tmp/prompt_learner-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_learner-0.2.3.tar", max compression
+gzip compressed data, was "prompt_learner-0.2.4.tar", max compression
```

## Comparing `prompt_learner-0.2.3.tar` & `prompt_learner-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2140 2024-05-07 04:41:30.281248 prompt_learner-0.2.3/README.md
--rw-r--r--   0        0        0     6148 2024-05-07 04:41:30.293507 prompt_learner-0.2.3/prompt_learner/.DS_Store
--rw-r--r--   0        0        0       28 2024-05-07 04:41:30.293626 prompt_learner-0.2.3/prompt_learner/adapters/__init__.py
--rw-r--r--   0        0        0      394 2024-05-07 04:41:30.293694 prompt_learner-0.2.3/prompt_learner/adapters/adapter.py
--rw-r--r--   0        0        0     1291 2024-05-07 04:41:30.293764 prompt_learner-0.2.3/prompt_learner/adapters/anthropic.py
--rw-r--r--   0        0        0      659 2024-05-07 04:52:50.363858 prompt_learner-0.2.3/prompt_learner/adapters/llama.py
--rw-r--r--   0        0        0      662 2024-05-07 04:41:30.293913 prompt_learner-0.2.3/prompt_learner/adapters/openai.py
--rw-r--r--   0        0        0     1278 2024-05-09 05:51:03.447015 prompt_learner-0.2.3/prompt_learner/evals/metrics/accuracy.py
--rw-r--r--   0        0        0       29 2024-05-07 04:41:30.294168 prompt_learner-0.2.3/prompt_learner/examples/__init__.py
--rw-r--r--   0        0        0      316 2024-05-07 04:41:30.294240 prompt_learner-0.2.3/prompt_learner/examples/example.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294327 prompt_learner-0.2.3/prompt_learner/examples/manipulation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294404 prompt_learner-0.2.3/prompt_learner/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294446 prompt_learner-0.2.3/prompt_learner/inference/predict.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294532 prompt_learner-0.2.3/prompt_learner/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294619 prompt_learner-0.2.3/prompt_learner/optimizers/descriptors/__init__.py
--rw-r--r--   0        0        0      165 2024-05-07 04:41:30.294703 prompt_learner-0.2.3/prompt_learner/optimizers/descriptors/descriptor.py
--rw-r--r--   0        0        0       34 2024-05-07 04:41:30.294768 prompt_learner-0.2.3/prompt_learner/optimizers/optimizer.py
--rw-r--r--   0        0        0       30 2024-05-07 04:41:30.294865 prompt_learner-0.2.3/prompt_learner/optimizers/selectors/__init__.py
--rw-r--r--   0        0        0     1537 2024-05-07 04:41:30.294949 prompt_learner-0.2.3/prompt_learner/optimizers/selectors/diverse_sampler.py
--rw-r--r--   0        0        0      624 2024-05-07 04:41:30.295030 prompt_learner-0.2.3/prompt_learner/optimizers/selectors/random_sampler.py
--rw-r--r--   0        0        0      873 2024-05-07 04:41:30.295104 prompt_learner-0.2.3/prompt_learner/optimizers/selectors/selector.py
--rw-r--r--   0        0        0      888 2024-05-07 04:41:30.295186 prompt_learner-0.2.3/prompt_learner/optimizers/selectors/stratified_sampler.py
--rw-r--r--   0        0        0       26 2024-05-07 04:41:30.295292 prompt_learner-0.2.3/prompt_learner/prompts/__init__.py
--rw-r--r--   0        0        0      597 2024-05-07 04:41:30.295363 prompt_learner-0.2.3/prompt_learner/prompts/cot.py
--rw-r--r--   0        0        0     1136 2024-05-07 04:41:30.295433 prompt_learner-0.2.3/prompt_learner/prompts/prompt.py
--rw-r--r--   0        0        0       22 2024-05-07 04:41:30.295534 prompt_learner-0.2.3/prompt_learner/tasks/__init__.py
--rw-r--r--   0        0        0      625 2024-05-07 04:41:30.295599 prompt_learner-0.2.3/prompt_learner/tasks/classification.py
--rw-r--r--   0        0        0      400 2024-05-07 04:41:30.295663 prompt_learner-0.2.3/prompt_learner/tasks/sql_generation.py
--rw-r--r--   0        0        0      529 2024-05-07 04:41:30.295736 prompt_learner-0.2.3/prompt_learner/tasks/tagging.py
--rw-r--r--   0        0        0     1589 2024-05-07 04:41:30.295807 prompt_learner-0.2.3/prompt_learner/tasks/task.py
--rw-r--r--   0        0        0       30 2024-05-07 04:41:30.295907 prompt_learner-0.2.3/prompt_learner/templates/__init__.py
--rw-r--r--   0        0        0     2863 2024-05-10 05:00:14.745809 prompt_learner-0.2.3/prompt_learner/templates/claude_template.py
--rw-r--r--   0        0        0     2648 2024-05-10 04:59:21.271133 prompt_learner-0.2.3/prompt_learner/templates/gpt_template.py
--rw-r--r--   0        0        0     1570 2024-05-07 04:41:30.296119 prompt_learner-0.2.3/prompt_learner/templates/template.py
--rw-r--r--   0        0        0     3373 2024-05-07 04:41:30.296253 prompt_learner-0.2.3/prompt_learner/translator/translate.py
--rw-r--r--   0        0        0      485 2024-05-10 05:01:03.392037 prompt_learner-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 prompt_learner-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2246 2024-05-15 04:01:12.814625 prompt_learner-0.2.4/README.md
+-rw-r--r--   0        0        0     6148 2024-05-07 04:41:30.293507 prompt_learner-0.2.4/prompt_learner/.DS_Store
+-rw-r--r--   0        0        0       28 2024-05-07 04:41:30.293626 prompt_learner-0.2.4/prompt_learner/adapters/__init__.py
+-rw-r--r--   0        0        0      521 2024-05-15 05:15:42.566078 prompt_learner-0.2.4/prompt_learner/adapters/adapter.py
+-rw-r--r--   0        0        0     1291 2024-05-07 04:41:30.293764 prompt_learner-0.2.4/prompt_learner/adapters/anthropic.py
+-rw-r--r--   0        0        0      659 2024-05-07 04:52:50.363858 prompt_learner-0.2.4/prompt_learner/adapters/llama.py
+-rw-r--r--   0        0        0      662 2024-05-07 04:41:30.293913 prompt_learner-0.2.4/prompt_learner/adapters/openai.py
+-rw-r--r--   0        0        0     1278 2024-05-09 05:51:03.447015 prompt_learner-0.2.4/prompt_learner/evals/metrics/accuracy.py
+-rw-r--r--   0        0        0       29 2024-05-07 04:41:30.294168 prompt_learner-0.2.4/prompt_learner/examples/__init__.py
+-rw-r--r--   0        0        0      316 2024-05-07 04:41:30.294240 prompt_learner-0.2.4/prompt_learner/examples/example.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294327 prompt_learner-0.2.4/prompt_learner/examples/manipulation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294404 prompt_learner-0.2.4/prompt_learner/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294446 prompt_learner-0.2.4/prompt_learner/inference/predict.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294532 prompt_learner-0.2.4/prompt_learner/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294619 prompt_learner-0.2.4/prompt_learner/optimizers/descriptors/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-07 04:41:30.294703 prompt_learner-0.2.4/prompt_learner/optimizers/descriptors/descriptor.py
+-rw-r--r--   0        0        0       34 2024-05-07 04:41:30.294768 prompt_learner-0.2.4/prompt_learner/optimizers/optimizer.py
+-rw-r--r--   0        0        0       30 2024-05-07 04:41:30.294865 prompt_learner-0.2.4/prompt_learner/optimizers/selectors/__init__.py
+-rw-r--r--   0        0        0     1537 2024-05-07 04:41:30.294949 prompt_learner-0.2.4/prompt_learner/optimizers/selectors/diverse_sampler.py
+-rw-r--r--   0        0        0      624 2024-05-07 04:41:30.295030 prompt_learner-0.2.4/prompt_learner/optimizers/selectors/random_sampler.py
+-rw-r--r--   0        0        0      873 2024-05-07 04:41:30.295104 prompt_learner-0.2.4/prompt_learner/optimizers/selectors/selector.py
+-rw-r--r--   0        0        0      888 2024-05-07 04:41:30.295186 prompt_learner-0.2.4/prompt_learner/optimizers/selectors/stratified_sampler.py
+-rw-r--r--   0        0        0       26 2024-05-07 04:41:30.295292 prompt_learner-0.2.4/prompt_learner/prompts/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-07 04:41:30.295363 prompt_learner-0.2.4/prompt_learner/prompts/cot.py
+-rw-r--r--   0        0        0     1136 2024-05-07 04:41:30.295433 prompt_learner-0.2.4/prompt_learner/prompts/prompt.py
+-rw-r--r--   0        0        0       22 2024-05-07 04:41:30.295534 prompt_learner-0.2.4/prompt_learner/tasks/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-07 04:41:30.295599 prompt_learner-0.2.4/prompt_learner/tasks/classification.py
+-rw-r--r--   0        0        0      400 2024-05-07 04:41:30.295663 prompt_learner-0.2.4/prompt_learner/tasks/sql_generation.py
+-rw-r--r--   0        0        0      529 2024-05-07 04:41:30.295736 prompt_learner-0.2.4/prompt_learner/tasks/tagging.py
+-rw-r--r--   0        0        0     1589 2024-05-07 04:41:30.295807 prompt_learner-0.2.4/prompt_learner/tasks/task.py
+-rw-r--r--   0        0        0       30 2024-05-07 04:41:30.295907 prompt_learner-0.2.4/prompt_learner/templates/__init__.py
+-rw-r--r--   0        0        0     2863 2024-05-10 05:00:14.745809 prompt_learner-0.2.4/prompt_learner/templates/claude_template.py
+-rw-r--r--   0        0        0     2648 2024-05-10 04:59:21.271133 prompt_learner-0.2.4/prompt_learner/templates/gpt_template.py
+-rw-r--r--   0        0        0     1570 2024-05-07 04:41:30.296119 prompt_learner-0.2.4/prompt_learner/templates/template.py
+-rw-r--r--   0        0        0     3373 2024-05-07 04:41:30.296253 prompt_learner-0.2.4/prompt_learner/translator/translate.py
+-rw-r--r--   0        0        0      485 2024-05-15 05:16:33.973124 prompt_learner-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2970 1970-01-01 00:00:00.000000 prompt_learner-0.2.4/PKG-INFO
```

### Comparing `prompt_learner-0.2.3/README.md` & `prompt_learner-0.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Prompt Learner
 
 [![Documentation](https://img.shields.io/badge/docs-promptlearner.attuna.xyz-blue.svg)](https://promptlearner.attuna.xyz/)
+[![Web App](https://img.shields.io/badge/app-streamlit-black.svg)](https://prompt-learner.streamlit.app/)
 [![Discord](https://img.shields.io/badge/discord-prompt_learner-blue?logo=discord&logoColor=white&color=5d68e8)](https://discord.gg/FST9HRNKYX)
 
 
 ## What is Prompt Learner?
 ![A Modular Approach To Prompting](docs/concepts/images/anatomy.png)
 
 Prompt Learner is designed to make prompts modular.\
```

### Comparing `prompt_learner-0.2.3/prompt_learner/.DS_Store` & `prompt_learner-0.2.4/prompt_learner/.DS_Store`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/adapters/anthropic.py` & `prompt_learner-0.2.4/prompt_learner/adapters/anthropic.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/adapters/llama.py` & `prompt_learner-0.2.4/prompt_learner/adapters/llama.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/adapters/openai.py` & `prompt_learner-0.2.4/prompt_learner/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/evals/metrics/accuracy.py` & `prompt_learner-0.2.4/prompt_learner/evals/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/optimizers/selectors/diverse_sampler.py` & `prompt_learner-0.2.4/prompt_learner/optimizers/selectors/diverse_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/optimizers/selectors/random_sampler.py` & `prompt_learner-0.2.4/prompt_learner/optimizers/selectors/random_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/optimizers/selectors/selector.py` & `prompt_learner-0.2.4/prompt_learner/optimizers/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/optimizers/selectors/stratified_sampler.py` & `prompt_learner-0.2.4/prompt_learner/optimizers/selectors/stratified_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/prompts/cot.py` & `prompt_learner-0.2.4/prompt_learner/prompts/cot.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/prompts/prompt.py` & `prompt_learner-0.2.4/prompt_learner/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/tasks/classification.py` & `prompt_learner-0.2.4/prompt_learner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/tasks/tagging.py` & `prompt_learner-0.2.4/prompt_learner/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/tasks/task.py` & `prompt_learner-0.2.4/prompt_learner/tasks/task.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/templates/claude_template.py` & `prompt_learner-0.2.4/prompt_learner/templates/claude_template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/templates/gpt_template.py` & `prompt_learner-0.2.4/prompt_learner/templates/gpt_template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/templates/template.py` & `prompt_learner-0.2.4/prompt_learner/templates/template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/prompt_learner/translator/translate.py` & `prompt_learner-0.2.4/prompt_learner/translator/translate.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.3/PKG-INFO` & `prompt_learner-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-learner
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Aditya Lahiri
 Author-email: adityalahiri13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -17,14 +17,15 @@
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Prompt Learner
 
 [![Documentation](https://img.shields.io/badge/docs-promptlearner.attuna.xyz-blue.svg)](https://promptlearner.attuna.xyz/)
+[![Web App](https://img.shields.io/badge/app-streamlit-black.svg)](https://prompt-learner.streamlit.app/)
 [![Discord](https://img.shields.io/badge/discord-prompt_learner-blue?logo=discord&logoColor=white&color=5d68e8)](https://discord.gg/FST9HRNKYX)
 
 
 ## What is Prompt Learner?
 ![A Modular Approach To Prompting](docs/concepts/images/anatomy.png)
 
 Prompt Learner is designed to make prompts modular.\
```

