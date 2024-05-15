# Comparing `tmp/deeprecsys-0.2.2.tar.gz` & `tmp/deeprecsys-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeprecsys-0.2.2.tar", max compression
+gzip compressed data, was "deeprecsys-0.2.3.tar", max compression
```

## Comparing `deeprecsys-0.2.2.tar` & `deeprecsys-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    35149 2024-05-15 10:55:37.210672 deeprecsys-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2024-05-15 16:09:12.343607 deeprecsys-0.2.2/deeprecsys/__init__.py
--rw-r--r--   0        0        0     2950 2024-05-15 14:12:38.674073 deeprecsys-0.2.2/deeprecsys/neural_networks/base_network.py
--rw-r--r--   0        0        0     1204 2022-09-08 14:25:26.828117 deeprecsys-0.2.2/deeprecsys/neural_networks/binary_classifier.py
--rw-r--r--   0        0        0     3564 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/neural_networks/deep_q_network.py
--rw-r--r--   0        0        0     6820 2024-05-15 18:50:07.998955 deeprecsys-0.2.2/deeprecsys/neural_networks/dueling.py
--rw-r--r--   0        0        0     3781 2022-09-06 10:54:03.210188 deeprecsys-0.2.2/deeprecsys/neural_networks/gaussian_actor.py
--rw-r--r--   0        0        0     1726 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/neural_networks/noisy_layer.py
--rw-r--r--   0        0        0     2960 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/neural_networks/policy_estimator.py
--rw-r--r--   0        0        0     3195 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/neural_networks/q_value_estimator.py
--rw-r--r--   0        0        0     1607 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/neural_networks/value_estimator.py
--rw-r--r--   0        0        0      800 2022-07-16 21:28:54.122713 deeprecsys-0.2.2/deeprecsys/rl/__init__.py
--rw-r--r--   0        0        0     3723 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/rl/agents/actor_critic.py
--rw-r--r--   0        0        0     1683 2024-05-15 16:29:25.290698 deeprecsys-0.2.2/deeprecsys/rl/agents/agent.py
--rw-r--r--   0        0        0     3322 2024-05-15 14:01:13.059895 deeprecsys-0.2.2/deeprecsys/rl/agents/dqn.py
--rw-r--r--   0        0        0     1719 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/rl/agents/epsilon_greedy.py
--rw-r--r--   0        0        0     4344 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/rl/agents/rainbow.py
--rw-r--r--   0        0        0     3806 2024-05-15 14:12:38.670073 deeprecsys-0.2.2/deeprecsys/rl/agents/reinforce.py
--rw-r--r--   0        0        0     6452 2024-05-15 18:02:33.063231 deeprecsys-0.2.2/deeprecsys/rl/agents/soft_actor_critic.py
--rw-r--r--   0        0        0     1340 2024-05-15 14:08:52.604309 deeprecsys-0.2.2/deeprecsys/rl/experience_replay/buffer_parameters.py
--rw-r--r--   0        0        0     2829 2024-05-15 18:39:34.983609 deeprecsys-0.2.2/deeprecsys/rl/experience_replay/experience_buffer.py
--rw-r--r--   0        0        0     4982 2024-05-15 18:51:46.223338 deeprecsys-0.2.2/deeprecsys/rl/experience_replay/priority_replay_buffer.py
--rw-r--r--   0        0        0     3157 2024-05-15 14:01:13.059895 deeprecsys-0.2.2/deeprecsys/rl/learning_statistics.py
--rw-r--r--   0        0        0     9864 2024-05-15 18:59:59.601655 deeprecsys-0.2.2/deeprecsys/rl/manager.py
--rw-r--r--   0        0        0     1694 2024-05-15 21:17:20.576905 deeprecsys-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 deeprecsys-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2079 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/deeprecsys/__init__.py
+-rw-r--r--   0        0        0     2950 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/deeprecsys/neural_networks/base_network.py
+-rw-r--r--   0        0        0     1204 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/deeprecsys/neural_networks/binary_classifier.py
+-rw-r--r--   0        0        0     3564 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/deeprecsys/neural_networks/deep_q_network.py
+-rw-r--r--   0        0        0     6820 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/deeprecsys/neural_networks/dueling.py
+-rw-r--r--   0        0        0     3781 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/deeprecsys/neural_networks/gaussian_actor.py
+-rw-r--r--   0        0        0     1726 2024-05-15 21:41:16.863534 deeprecsys-0.2.3/deeprecsys/neural_networks/noisy_layer.py
+-rw-r--r--   0        0        0     2960 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/neural_networks/policy_estimator.py
+-rw-r--r--   0        0        0     3195 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/neural_networks/q_value_estimator.py
+-rw-r--r--   0        0        0     1607 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/neural_networks/value_estimator.py
+-rw-r--r--   0        0        0      800 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/__init__.py
+-rw-r--r--   0        0        0     3723 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/agents/actor_critic.py
+-rw-r--r--   0        0        0     1683 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/agents/agent.py
+-rw-r--r--   0        0        0     3322 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/agents/dqn.py
+-rw-r--r--   0        0        0     1719 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/agents/epsilon_greedy.py
+-rw-r--r--   0        0        0     4344 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/agents/rainbow.py
+-rw-r--r--   0        0        0     3806 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/agents/reinforce.py
+-rw-r--r--   0        0        0     6452 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/agents/soft_actor_critic.py
+-rw-r--r--   0        0        0     1340 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/experience_replay/buffer_parameters.py
+-rw-r--r--   0        0        0     2829 2024-05-15 21:41:16.864534 deeprecsys-0.2.3/deeprecsys/rl/experience_replay/experience_buffer.py
+-rw-r--r--   0        0        0     4982 2024-05-15 21:41:16.865534 deeprecsys-0.2.3/deeprecsys/rl/experience_replay/priority_replay_buffer.py
+-rw-r--r--   0        0        0     3157 2024-05-15 21:41:16.865534 deeprecsys-0.2.3/deeprecsys/rl/learning_statistics.py
+-rw-r--r--   0        0        0     9864 2024-05-15 21:41:16.865534 deeprecsys-0.2.3/deeprecsys/rl/manager.py
+-rw-r--r--   0        0        0     2048 2024-05-15 21:43:28.546043 deeprecsys-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 deeprecsys-0.2.3/PKG-INFO
```

### Comparing `deeprecsys-0.2.2/LICENSE` & `deeprecsys-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/base_network.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/base_network.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/binary_classifier.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/deep_q_network.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/deep_q_network.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/dueling.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/dueling.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/gaussian_actor.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/gaussian_actor.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/noisy_layer.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/noisy_layer.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/policy_estimator.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/policy_estimator.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/q_value_estimator.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/q_value_estimator.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/neural_networks/value_estimator.py` & `deeprecsys-0.2.3/deeprecsys/neural_networks/value_estimator.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/__init__.py` & `deeprecsys-0.2.3/deeprecsys/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/agents/actor_critic.py` & `deeprecsys-0.2.3/deeprecsys/rl/agents/actor_critic.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/agents/agent.py` & `deeprecsys-0.2.3/deeprecsys/rl/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/agents/dqn.py` & `deeprecsys-0.2.3/deeprecsys/rl/agents/dqn.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/agents/epsilon_greedy.py` & `deeprecsys-0.2.3/deeprecsys/rl/agents/epsilon_greedy.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/agents/rainbow.py` & `deeprecsys-0.2.3/deeprecsys/rl/agents/rainbow.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/agents/reinforce.py` & `deeprecsys-0.2.3/deeprecsys/rl/agents/reinforce.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/agents/soft_actor_critic.py` & `deeprecsys-0.2.3/deeprecsys/rl/agents/soft_actor_critic.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/experience_replay/buffer_parameters.py` & `deeprecsys-0.2.3/deeprecsys/rl/experience_replay/buffer_parameters.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/experience_replay/experience_buffer.py` & `deeprecsys-0.2.3/deeprecsys/rl/experience_replay/experience_buffer.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/experience_replay/priority_replay_buffer.py` & `deeprecsys-0.2.3/deeprecsys/rl/experience_replay/priority_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/learning_statistics.py` & `deeprecsys-0.2.3/deeprecsys/rl/learning_statistics.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/deeprecsys/rl/manager.py` & `deeprecsys-0.2.3/deeprecsys/rl/manager.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.2/pyproject.toml` & `deeprecsys-0.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 [tool.poetry]
 name = "deeprecsys"
-version = "0.2.2"
+version = "0.2.3"
 description = "deeprecsys is an open tool belt to speed up the development of modern data science projects at an enterprise level"
 authors = ["Lucas Farris <lucas@farris.com.br>"]
-license = "MIT"
+license = "GPL-3.0-or-later"
+readme = "README.md"
+homepage = "https://deeprecsys.com"
+repository = "https://github.com/luksfarris/deeprecsys"
+documentation = "https://deeprecsys.com"
+keywords = ["machinelearning", "reinforcementlearning", "recommmendersystems", "deeplearning", "datascience"]
+classifiers = ["Topic :: Scientific/Engineering :: Artificial Intelligence"]
 
 [[tool.poetry.source]]
 name = "cputorch"
 url = "https://download.pytorch.org/whl/cpu"
 priority = "supplemental"
```

