# Comparing `tmp/eprllib-1.1.0.tar.gz` & `tmp/eprllib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eprllib-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eprllib-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eprllib-1.1.0.tar` & `eprllib-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     6706 2024-03-22 12:29:57.414473 eprllib-1.1.0/README.md
--rw-r--r--   0        0        0      660 2024-05-10 12:17:44.042500 eprllib-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-28 20:01:08.588762 eprllib-1.1.0/src/eprllib/ExampleFiles/__init__.py
--rw-r--r--   0        0        0  1648753 2024-03-28 20:01:08.599401 eprllib-1.1.0/src/eprllib/ExampleFiles/epw/USA_IL_Chicago-OHare_Intl_AP_725300_TMY3.epw
--rw-r--r--   0        0        0        0 2024-03-28 20:01:08.599401 eprllib-1.1.0/src/eprllib/ExampleFiles/epw/__init__.py
--rw-r--r--   0        0        0   245096 2024-03-28 20:01:08.599401 eprllib-1.1.0/src/eprllib/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf
--rw-r--r--   0        0        0        0 2024-03-28 20:01:08.599401 eprllib-1.1.0/src/eprllib/ExampleFiles/idf/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 13:27:42.113993 eprllib-1.1.0/src/eprllib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 10:07:03.001250 eprllib-1.1.0/src/eprllib/agents/__init__.py
--rw-r--r--   0        0        0     5449 2024-03-14 16:24:23.397736 eprllib-1.1.0/src/eprllib/agents/conventional.py
--rw-r--r--   0        0        0     1028 2024-03-21 08:40:43.671486 eprllib-1.1.0/src/eprllib/agents/holon_config.py
--rw-r--r--   0        0        0     1008 2024-02-12 10:25:28.186353 eprllib-1.1.0/src/eprllib/agents/user.py
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.360381 eprllib-1.1.0/src/eprllib/env/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 19:16:29.819874 eprllib-1.1.0/src/eprllib/env/multiagent/__init__.py
--rw-r--r--   0        0        0     7810 2024-05-10 08:22:29.508886 eprllib-1.1.0/src/eprllib/env/multiagent/marl_ep_gym_env.py
--rw-r--r--   0        0        0    24712 2024-05-10 08:22:29.510903 eprllib-1.1.0/src/eprllib/env/multiagent/marl_ep_runner.py
--rw-r--r--   0        0        0     7670 2024-03-21 15:31:48.407127 eprllib-1.1.0/src/eprllib/env/simpleagent/VENT_ep_gym_env.py
--rw-r--r--   0        0        0    20698 2024-03-21 15:31:48.407127 eprllib-1.1.0/src/eprllib/env/simpleagent/VENT_ep_runner.py
--rw-r--r--   0        0        0        0 2024-03-21 19:16:52.042116 eprllib-1.1.0/src/eprllib/env/simpleagent/__init__.py
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.369889 eprllib-1.1.0/src/eprllib/postprocess/__init__.py
--rw-r--r--   0        0        0     7773 2024-05-04 00:19:40.583732 eprllib-1.1.0/src/eprllib/postprocess/marl_init_conventional.py
--rw-r--r--   0        0        0     8155 2024-05-10 11:58:39.937476 eprllib-1.1.0/src/eprllib/postprocess/marl_init_evaluation.py
--rw-r--r--   0        0        0     7245 2024-05-04 00:19:40.582728 eprllib-1.1.0/src/eprllib/postprocess/marl_init_noventilation.py
--rw-r--r--   0        0        0   448967 2024-05-10 12:09:01.402850 eprllib-1.1.0/src/eprllib/postprocess/marl_results_evaluation.ipynb
--rw-r--r--   0        0        0     3002 2024-02-22 11:24:29.811391 eprllib-1.1.0/src/eprllib/postprocess/neural_networ_analysis.ipynb
--rw-r--r--   0        0        0     1636 2024-04-18 12:01:12.679943 eprllib-1.1.0/src/eprllib/preprocess/IDFProperties.py
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.372239 eprllib-1.1.0/src/eprllib/preprocess/__init__.py
--rw-r--r--   0        0        0     5797 2024-03-21 15:31:48.398206 eprllib-1.1.0/src/eprllib/preprocess/conventional_experience.py
--rw-r--r--   0        0        0        0 2024-02-12 10:39:26.603572 eprllib-1.1.0/src/eprllib/tools/__init__.py
--rw-r--r--   0        0        0      829 2024-03-28 10:22:08.162993 eprllib-1.1.0/src/eprllib/tools/action_transformers.py
--rw-r--r--   0        0        0     1402 2024-02-24 11:12:25.969964 eprllib-1.1.0/src/eprllib/tools/devices_space_action.py
--rw-r--r--   0        0        0    19846 2024-03-21 15:31:48.398206 eprllib-1.1.0/src/eprllib/tools/ep_episode_config.py
--rw-r--r--   0        0        0     7642 2024-05-04 16:21:41.949814 eprllib-1.1.0/src/eprllib/tools/rewards.py
--rw-r--r--   0        0        0     3180 2024-05-10 08:22:29.542577 eprllib-1.1.0/src/eprllib/tools/utils.py
--rw-r--r--   0        0        0     7134 2024-03-21 20:29:35.640440 eprllib-1.1.0/src/eprllib/tools/weather_utils.py
--rw-r--r--   0        0        0     7086 1970-01-01 00:00:00.000000 eprllib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6706 2024-03-22 12:29:57.414473 eprllib-1.1.1/README.md
+-rw-r--r--   0        0        0      660 2024-05-15 12:23:14.428918 eprllib-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-28 20:01:08.588762 eprllib-1.1.1/src/eprllib/ExampleFiles/__init__.py
+-rw-r--r--   0        0        0  1648753 2024-03-28 20:01:08.599401 eprllib-1.1.1/src/eprllib/ExampleFiles/epw/USA_IL_Chicago-OHare_Intl_AP_725300_TMY3.epw
+-rw-r--r--   0        0        0        0 2024-03-28 20:01:08.599401 eprllib-1.1.1/src/eprllib/ExampleFiles/epw/__init__.py
+-rw-r--r--   0        0        0   245096 2024-03-28 20:01:08.599401 eprllib-1.1.1/src/eprllib/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf
+-rw-r--r--   0        0        0        0 2024-03-28 20:01:08.599401 eprllib-1.1.1/src/eprllib/ExampleFiles/idf/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 13:27:42.113993 eprllib-1.1.1/src/eprllib/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:07:03.001250 eprllib-1.1.1/src/eprllib/agents/__init__.py
+-rw-r--r--   0        0        0     5449 2024-03-14 16:24:23.397736 eprllib-1.1.1/src/eprllib/agents/conventional.py
+-rw-r--r--   0        0        0     1028 2024-03-21 08:40:43.671486 eprllib-1.1.1/src/eprllib/agents/holon_config.py
+-rw-r--r--   0        0        0     1008 2024-02-12 10:25:28.186353 eprllib-1.1.1/src/eprllib/agents/user.py
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.360381 eprllib-1.1.1/src/eprllib/env/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 19:16:29.819874 eprllib-1.1.1/src/eprllib/env/multiagent/__init__.py
+-rw-r--r--   0        0        0     8134 2024-05-15 12:08:56.602600 eprllib-1.1.1/src/eprllib/env/multiagent/marl_ep_gym_env.py
+-rw-r--r--   0        0        0    24852 2024-05-15 12:04:18.306197 eprllib-1.1.1/src/eprllib/env/multiagent/marl_ep_runner.py
+-rw-r--r--   0        0        0     7670 2024-03-21 15:31:48.407127 eprllib-1.1.1/src/eprllib/env/simpleagent/VENT_ep_gym_env.py
+-rw-r--r--   0        0        0    20698 2024-03-21 15:31:48.407127 eprllib-1.1.1/src/eprllib/env/simpleagent/VENT_ep_runner.py
+-rw-r--r--   0        0        0        0 2024-03-21 19:16:52.042116 eprllib-1.1.1/src/eprllib/env/simpleagent/__init__.py
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.369889 eprllib-1.1.1/src/eprllib/postprocess/__init__.py
+-rw-r--r--   0        0        0     7929 2024-05-13 20:46:38.662264 eprllib-1.1.1/src/eprllib/postprocess/marl_init_conventional.py
+-rw-r--r--   0        0        0     8313 2024-05-13 20:46:38.679148 eprllib-1.1.1/src/eprllib/postprocess/marl_init_evaluation.py
+-rw-r--r--   0        0        0     7401 2024-05-13 20:46:38.693583 eprllib-1.1.1/src/eprllib/postprocess/marl_init_noventilation.py
+-rw-r--r--   0        0        0   448967 2024-05-10 12:09:01.402850 eprllib-1.1.1/src/eprllib/postprocess/marl_results_evaluation.ipynb
+-rw-r--r--   0        0        0     3002 2024-02-22 11:24:29.811391 eprllib-1.1.1/src/eprllib/postprocess/neural_networ_analysis.ipynb
+-rw-r--r--   0        0        0     1636 2024-04-18 12:01:12.679943 eprllib-1.1.1/src/eprllib/preprocess/IDFProperties.py
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.372239 eprllib-1.1.1/src/eprllib/preprocess/__init__.py
+-rw-r--r--   0        0        0     5797 2024-03-21 15:31:48.398206 eprllib-1.1.1/src/eprllib/preprocess/conventional_experience.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:39:26.603572 eprllib-1.1.1/src/eprllib/tools/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-28 10:22:08.162993 eprllib-1.1.1/src/eprllib/tools/action_transformers.py
+-rw-r--r--   0        0        0     1402 2024-02-24 11:12:25.969964 eprllib-1.1.1/src/eprllib/tools/devices_space_action.py
+-rw-r--r--   0        0        0    19846 2024-03-21 15:31:48.398206 eprllib-1.1.1/src/eprllib/tools/ep_episode_config.py
+-rw-r--r--   0        0        0     7642 2024-05-04 16:21:41.949814 eprllib-1.1.1/src/eprllib/tools/rewards.py
+-rw-r--r--   0        0        0     3180 2024-05-10 08:22:29.542577 eprllib-1.1.1/src/eprllib/tools/utils.py
+-rw-r--r--   0        0        0     7134 2024-03-21 20:29:35.640440 eprllib-1.1.1/src/eprllib/tools/weather_utils.py
+-rw-r--r--   0        0        0     7086 1970-01-01 00:00:00.000000 eprllib-1.1.1/PKG-INFO
```

### Comparing `eprllib-1.1.0/README.md` & `eprllib-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/pyproject.toml` & `eprllib-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "eprllib"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Germán Rodolfo Henderson"},
 ]
 description = "Building control trought DRL."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `eprllib-1.1.0/src/eprllib/ExampleFiles/epw/USA_IL_Chicago-OHare_Intl_AP_725300_TMY3.epw` & `eprllib-1.1.1/src/eprllib/ExampleFiles/epw/USA_IL_Chicago-OHare_Intl_AP_725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf` & `eprllib-1.1.1/src/eprllib/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/agents/conventional.py` & `eprllib-1.1.1/src/eprllib/agents/conventional.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/agents/holon_config.py` & `eprllib-1.1.1/src/eprllib/agents/holon_config.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/agents/user.py` & `eprllib-1.1.1/src/eprllib/agents/user.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/env/multiagent/marl_ep_gym_env.py` & `eprllib-1.1.1/src/eprllib/env/multiagent/marl_ep_gym_env.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 from ray.rllib.env.multi_agent_env import MultiAgentEnv
 # Used to define the environment base and the size of action and observation spaces.
 from queue import Empty, Full, Queue
 # Used to separate the execution in two threads and comunicate EnergyPlus with this environment.
 from typing import Any, Dict, Optional
 # To specify the types of variables espected.
 from eprllib.env.multiagent.marl_ep_runner import EnergyPlusRunner
+from eprllib.tools import rewards
 # The EnergyPlus Runner.
 from gymnasium.spaces import Box
 
 class EnergyPlusEnv_v0(MultiAgentEnv):
     def __init__(
         self,
         env_config: Dict[str, Any]
         ):
-        # super init of the base class gym.Env.
-        super().__init__()
         # asigning the configuration of the environment.
         self.env_config = env_config
         self.env_config['agent_ids'] = list(self.env_config['ep_actuators'].keys())
         # asignation of the agents ids for the environment.
-        self._agent_ids = env_config['agent_ids']
+        self._agent_ids = set(env_config['agent_ids'])
         # asignation of environment spaces.
         self.action_space = self.env_config['action_space']
         
         obs_space_len = sum([
             len(self.env_config['ep_variables']),
             len(self.env_config['ep_meters']),
             len(self.env_config['ep_actuators']),
@@ -37,31 +36,37 @@
             self.env_config['weather_prob_days'] * 144,
             -len(self.env_config['no_observable_variables']),
             1, # (agent_indicator)
         ])
 
         self.observation_space = Box(float("-inf"), float("inf"), (obs_space_len,))
         
+        # super init of the base class gym.Env.
+        super().__init__()
+        
         # EnergyPlus Runner class.
         self.energyplus_runner: Optional[EnergyPlusRunner] = None
         # queues for communication between MDP and EnergyPlus.
         self.obs_queue: Optional[Queue] = None
         self.act_queue: Optional[Queue] = None
         self.infos_queue: Optional[Queue] = None
         
         # ===CONTROLS=== #
         # variable for the registry of the episode number.
         self.episode = -1
+        self.timestep = 0
         # dict to save the last observation and infos in the environment.
         self.last_obs = {}
         self.last_infos = {}
         for agent in self.env_config['agent_ids']:
             self.last_obs[agent] = []
             self.last_infos[agent] = []
-            
+        # list to append, if is needed, the values of PPD and energy
+        self.ppd_list = []
+        self.energy_list = []
 
     def reset(
         self, *,
         seed: Optional[int] = None,
         options: Optional[Dict[str, Any]] = None
     ):
         # Increment the counting of episodes in 1.
@@ -161,16 +166,19 @@
         
         # Raise an exception if the episode is faulty.
         if self.energyplus_runner.failed():
             truncateds = True
             raise Exception("Faulty episode")
         
         # Calculate the reward in the timestep
-        reward_function = self.env_config['reward_function']
-        reward = reward_function(self.env_config, obs, infos)
+        if self.env_config.get('reward_function', False):
+            reward_function = self.env_config['reward_function']
+        else:
+            reward_function = rewards.reward_function_T3_Energy
+        reward = reward_function(self, obs, infos)
         
         reward_dict = {}
         for agent in self.env_config['agent_ids']:
             reward_dict[agent] =  reward
         
         terminated["__all__"] = terminateds
         truncated["__all__"] = truncateds
```

### Comparing `eprllib-1.1.0/src/eprllib/env/multiagent/marl_ep_runner.py` & `eprllib-1.1.1/src/eprllib/env/multiagent/marl_ep_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,44 +246,46 @@
             for variable in weather_variables_list:
                 weather_variables_dict[variable] = weather_variables_methods[variable]
             
             obs.update(weather_variables_dict)
             
         # Set the variables in the infos dict before to delete from the obs dict.
         infos_dict = {}
-        for variable in self.env_config['infos_variables']:
-            infos_dict[variable] = obs[variable]
+        if self.env_config.get('infos_variables', False):
+            for variable in self.env_config['infos_variables']:
+                infos_dict[variable] = obs[variable]
         
         infos = {}
         for agent in self.env_config['agent_ids']:
             infos[agent] = infos_dict
         
         self.infos_queue.put(infos)
         self.infos_event.set()
         
-        for variable in self.env_config['no_observable_variables']:
-            del obs[variable]
+        if self.env_config.get('no_observable_variables', False):
+            for variable in self.env_config['no_observable_variables']:
+                del obs[variable]
         
         # save the last obs and infos dicts.
         self.obs = obs
         self.infos = infos
         
         # Transform the observation in a numpy array to meet the condition expected in a RLlib Environment
         next_obs = np.array(list(obs.values()))
         
         # Consult the stadistics of the weather to put into the obs array. This add 1440 elements 
         # to the observation.
         weather_prob = self.weather_stats.n_days_predictions(api.exchange.day_of_year(state_argument), self.env_config.get('weather_prob_days', 2))
         next_obs = np.concatenate([next_obs, weather_prob])
         
         next_obs_dict = {}
-        agent_indicator = 10
+        agent_indicator = 1
         for agent in self.env_config['agent_ids']:
             next_obs_dict[agent] = np.concatenate(([agent_indicator], next_obs))
-            agent_indicator += 10
+            agent_indicator += 1
         
         # Set the observation to communicate with the MDP.
         self.obs_queue.put(next_obs_dict)
         self.obs_event.set()
 
     def _collect_first_obs(self, state_argument):
         """This method is used to collect only the first observation of the environment when the episode beggins.
```

### Comparing `eprllib-1.1.0/src/eprllib/env/simpleagent/VENT_ep_gym_env.py` & `eprllib-1.1.1/src/eprllib/env/simpleagent/VENT_ep_gym_env.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/env/simpleagent/VENT_ep_runner.py` & `eprllib-1.1.1/src/eprllib/env/simpleagent/VENT_ep_runner.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/postprocess/marl_init_conventional.py` & `eprllib-1.1.1/src/eprllib/postprocess/marl_init_conventional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """# RUN CONVENTIONAL CONTROLS
 
 This script execute the conventional controls in the evaluation scenario.
 """
 import sys
 sys.path.insert(0, 'C:/Users/grhen/Documents/GitHub/natural_ventilation_EP_RLlib')
+import os
 import csv
 from eprllib.env.multiagent.marl_ep_gym_env import EnergyPlusEnv_v0
 from eprllib.agents.conventional import Conventional
 
 
 def init_rb_evaluation(
     env_config: dict,
@@ -67,15 +68,17 @@
     """
     # se importan las políticas convencionales para la configuracion especificada
     policy = Conventional(policy_config)
     # se inicia el entorno con la configuración especificada
     env = EnergyPlusEnv_v0(env_config)
     _agents_id = env.get_agent_ids()
     _agents_id_list = list(_agents_id)
-
+    # create the output folder if it doesn't exist
+    if not os.path.exists(env_config['output']):
+        os.makedirs(env_config['output'])
     # open the file in the write mode
     data = open(env_config['output']+'/'+name+'.csv', 'w')
     # create the csv writer
     writer = csv.writer(data)
     terminated = {}
     terminated["__all__"] = False # variable de control de lazo (es verdadera cuando termina un episodio)
     episode_reward = 0
@@ -188,8 +191,8 @@
     }
     try:
         os.makedirs(env_config['output'])
     except OSError:
         pass
     
     episode_reward = init_rb_evaluation(env_config, policy_config, name)
-    print(f"Episode reward is: {episode_reward}.")
+    print(f"Episode reward is: {episode_reward}.")
```

### Comparing `eprllib-1.1.0/src/eprllib/postprocess/marl_init_evaluation.py` & `eprllib-1.1.1/src/eprllib/postprocess/marl_init_evaluation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """# RUN DRL CONTROLS
 
 This script execute the conventional controls in the evaluation scenario.
 """
 import sys
 sys.path.insert(0, 'C:/Users/grhen/Documents/GitHub/natural_ventilation_EP_RLlib')
+import os
 import csv
 from ray.rllib.policy.policy import Policy
 from eprllib.env.multiagent.marl_ep_gym_env import EnergyPlusEnv_v0
 
 
 def init_drl_evaluation(
     env_config: dict,
@@ -61,14 +62,17 @@
     """
     # Use the `from_checkpoint` utility of the Policy class:
     policy = Policy.from_checkpoint(checkpoint_path)
     # se inicia el entorno con la configuración especificada
     env = EnergyPlusEnv_v0(env_config)
     _agents_id = env.get_agent_ids()
     _agents_id_list = list(_agents_id)
+    # create the output folder if it doesn't exist
+    if not os.path.exists(env_config['output']):
+        os.makedirs(env_config['output'])
     # open the file in the write mode
     data = open(env_config['output']+'/'+name+'.csv', 'w')
     # create the csv writer
     writer = csv.writer(data)
     terminated = {}
     terminated["__all__"] = False # variable de control de lazo (es verdadera cuando termina un episodio)
     episode_reward = 0
@@ -189,8 +193,8 @@
     
     episode_reward = init_drl_evaluation(
         env_config,
         checkpoint_path,
         name
     )
     
-    print(f"Episode reward is: {episode_reward}.")
+    print(f"Episode reward is: {episode_reward}.")
```

### Comparing `eprllib-1.1.0/src/eprllib/postprocess/marl_init_noventilation.py` & `eprllib-1.1.1/src/eprllib/postprocess/marl_init_noventilation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """# RUN CONVENTIONAL CONTROLS
 
 This script execute the conventional controls in the evaluation scenario.
 """
 import sys
 sys.path.insert(0, 'C:/Users/grhen/Documents/GitHub/natural_ventilation_EP_RLlib')
+import os
 import csv
 from eprllib.env.multiagent.marl_ep_gym_env import EnergyPlusEnv_v0
 
 def init_rb_evaluation(
     env_config: dict,
     policy_config: dict,
     name: str
@@ -63,15 +64,17 @@
     print(f"Episode reward is: {episode_reward}.")
     ```
     """
     # se inicia el entorno con la configuración especificada
     env = EnergyPlusEnv_v0(env_config)
     _agents_id = env.get_agent_ids()
     _agents_id_list = list(_agents_id)
-
+    # create the output folder if it doesn't exist
+    if not os.path.exists(env_config['output']):
+        os.makedirs(env_config['output'])
     # open the file in the write mode
     data = open(env_config['output']+'/'+name+'.csv', 'w')
     # create the csv writer
     writer = csv.writer(data)
     terminated = {}
     terminated["__all__"] = False # variable de control de lazo (es verdadera cuando termina un episodio)
     episode_reward = 0
@@ -180,8 +183,8 @@
     }
     try:
         os.makedirs(env_config['output'])
     except OSError:
         pass
     
     episode_reward = init_rb_evaluation(env_config, policy_config, name)
-    print(f"Episode reward is: {episode_reward}.")
+    print(f"Episode reward is: {episode_reward}.")
```

### Comparing `eprllib-1.1.0/src/eprllib/postprocess/marl_results_evaluation.ipynb` & `eprllib-1.1.1/src/eprllib/postprocess/marl_results_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/postprocess/neural_networ_analysis.ipynb` & `eprllib-1.1.1/src/eprllib/postprocess/neural_networ_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/preprocess/IDFProperties.py` & `eprllib-1.1.1/src/eprllib/preprocess/IDFProperties.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/preprocess/conventional_experience.py` & `eprllib-1.1.1/src/eprllib/preprocess/conventional_experience.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/tools/action_transformers.py` & `eprllib-1.1.1/src/eprllib/tools/action_transformers.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/tools/devices_space_action.py` & `eprllib-1.1.1/src/eprllib/tools/devices_space_action.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/tools/ep_episode_config.py` & `eprllib-1.1.1/src/eprllib/tools/ep_episode_config.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/tools/rewards.py` & `eprllib-1.1.1/src/eprllib/tools/rewards.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/tools/utils.py` & `eprllib-1.1.1/src/eprllib/tools/utils.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/src/eprllib/tools/weather_utils.py` & `eprllib-1.1.1/src/eprllib/tools/weather_utils.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.1.0/PKG-INFO` & `eprllib-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eprllib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Building control trought DRL.
 Author: Germán Rodolfo Henderson
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

