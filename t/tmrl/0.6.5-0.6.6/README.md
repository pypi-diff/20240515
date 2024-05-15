# Comparing `tmp/tmrl-0.6.5.tar.gz` & `tmp/tmrl-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmrl-0.6.5.tar", last modified: Sun May  5 19:20:00 2024, max compression
+gzip compressed data, was "tmrl-0.6.6.tar", last modified: Wed May 15 20:29:44 2024, max compression
```

## Comparing `tmrl-0.6.5.tar` & `tmrl-0.6.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.432227 tmrl-0.6.5/
--rw-rw-rw-   0        0        0     1089 2024-04-08 03:24:28.000000 tmrl-0.6.5/LICENSE
--rw-rw-rw-   0        0        0       43 2024-04-08 03:28:54.000000 tmrl-0.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2052 2024-05-05 19:20:00.432227 tmrl-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0    31211 2024-04-30 04:38:25.000000 tmrl-0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.085892 tmrl-0.6.5/readme/
--rw-rw-rw-   0        0        0     1067 2024-04-08 03:28:54.000000 tmrl-0.6.5/readme/pypi.md
--rw-rw-rw-   0        0        0       42 2024-05-05 19:20:00.432227 tmrl-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     6314 2024-05-05 19:09:31.000000 tmrl-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.164882 tmrl-0.6.5/tmrl/
--rw-rw-rw-   0        0        0     1590 2024-05-05 18:46:33.000000 tmrl-0.6.5/tmrl/__init__.py
--rw-rw-rw-   0        0        0     4415 2024-05-05 19:05:48.000000 tmrl-0.6.5/tmrl/__main__.py
--rw-rw-rw-   0        0        0     5386 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/actor.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.217887 tmrl-0.6.5/tmrl/config/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/config/__init__.py
--rw-rw-rw-   0        0        0     6165 2024-04-23 05:21:02.000000 tmrl-0.6.5/tmrl/config/config_constants.py
--rw-rw-rw-   0        0        0     8564 2024-05-05 18:46:28.000000 tmrl-0.6.5/tmrl/config/config_objects.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.274840 tmrl-0.6.5/tmrl/custom/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/custom/__init__.py
--rw-rw-rw-   0        0        0    18803 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/custom/custom_algorithms.py
--rw-rw-rw-   0        0        0     9431 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/custom/custom_checkpoints.py
--rw-rw-rw-   0        0        0    12796 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/custom/custom_gym_interfaces.py
--rw-rw-rw-   0        0        0    23958 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/custom/custom_memories.py
--rw-rw-rw-   0        0        0    29938 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/custom/custom_models.py
--rw-rw-rw-   0        0        0     1387 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/custom/custom_preprocessors.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.369096 tmrl-0.6.5/tmrl/custom/utils/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/custom/utils/__init__.py
--rw-rw-rw-   0        0        0     5463 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/custom/utils/compute_reward.py
--rw-rw-rw-   0        0        0     2248 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/custom/utils/control_gamepad.py
--rw-rw-rw-   0        0        0     3981 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/custom/utils/control_keyboard.py
--rw-rw-rw-   0        0        0     1710 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/custom/utils/control_mouse.py
--rw-rw-rw-   0        0        0     9041 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/custom/utils/nn.py
--rw-rw-rw-   0        0        0     5019 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/custom/utils/tools.py
--rw-rw-rw-   0        0        0     9247 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/custom/utils/window.py
--rw-rw-rw-   0        0        0     1291 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/envs.py
--rw-rw-rw-   0        0        0     9555 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/memory.py
--rw-rw-rw-   0        0        0    41597 2024-04-08 03:28:54.000000 tmrl-0.6.5/tmrl/networking.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.400261 tmrl-0.6.5/tmrl/tools/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/tools/__init__.py
--rw-rw-rw-   0        0        0     2922 2024-04-26 07:47:33.000000 tmrl-0.6.5/tmrl/tools/check_environment.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.418215 tmrl-0.6.5/tmrl/tools/init_package/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/tools/init_package/__init__.py
--rw-rw-rw-   0        0        0    27288 2024-04-23 05:21:02.000000 tmrl-0.6.5/tmrl/tools/init_package/init_pywin32.py
--rw-rw-rw-   0        0        0     4882 2024-04-23 05:21:02.000000 tmrl-0.6.5/tmrl/tools/init_package/init_tmrl.py
--rw-rw-rw-   0        0        0     3235 2024-05-05 19:00:47.000000 tmrl-0.6.5/tmrl/tools/record.py
--rw-rw-rw-   0        0        0     1279 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/tools/save_replays.py
--rw-rw-rw-   0        0        0     1390 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/training.py
--rw-rw-rw-   0        0        0    10895 2024-05-05 18:46:41.000000 tmrl-0.6.5/tmrl/training_offline.py
--rw-rw-rw-   0        0        0    10255 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/util.py
--rw-rw-rw-   0        0        0     2031 2024-04-08 03:24:28.000000 tmrl-0.6.5/tmrl/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:20:00.199142 tmrl-0.6.5/tmrl.egg-info/
--rw-rw-rw-   0        0        0     2052 2024-05-05 19:19:59.000000 tmrl-0.6.5/tmrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2024-05-05 19:20:00.000000 tmrl-0.6.5/tmrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:19:59.000000 tmrl-0.6.5/tmrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2024-05-05 19:19:59.000000 tmrl-0.6.5/tmrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-05 19:19:59.000000 tmrl-0.6.5/tmrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.294027 tmrl-0.6.6/
+-rw-rw-rw-   0        0        0     1089 2024-04-08 03:24:28.000000 tmrl-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-04-08 03:28:54.000000 tmrl-0.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2052 2024-05-15 20:29:44.287217 tmrl-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0    31211 2024-05-15 20:18:54.000000 tmrl-0.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:43.796996 tmrl-0.6.6/readme/
+-rw-rw-rw-   0        0        0     1067 2024-04-08 03:28:54.000000 tmrl-0.6.6/readme/pypi.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:29:44.294027 tmrl-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     6314 2024-05-15 20:20:07.000000 tmrl-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:43.928089 tmrl-0.6.6/tmrl/
+-rw-rw-rw-   0        0        0     1590 2024-05-15 20:16:29.000000 tmrl-0.6.6/tmrl/__init__.py
+-rw-rw-rw-   0        0        0     4415 2024-05-15 20:18:54.000000 tmrl-0.6.6/tmrl/__main__.py
+-rw-rw-rw-   0        0        0     5386 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/actor.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:43.971545 tmrl-0.6.6/tmrl/config/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/config/__init__.py
+-rw-rw-rw-   0        0        0     6165 2024-04-23 05:21:02.000000 tmrl-0.6.6/tmrl/config/config_constants.py
+-rw-rw-rw-   0        0        0     8564 2024-05-05 18:46:28.000000 tmrl-0.6.6/tmrl/config/config_objects.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.065686 tmrl-0.6.6/tmrl/custom/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/custom/__init__.py
+-rw-rw-rw-   0        0        0    18803 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/custom/custom_algorithms.py
+-rw-rw-rw-   0        0        0     9431 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/custom/custom_checkpoints.py
+-rw-rw-rw-   0        0        0    12796 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/custom/custom_gym_interfaces.py
+-rw-rw-rw-   0        0        0    23958 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/custom/custom_memories.py
+-rw-rw-rw-   0        0        0    29938 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/custom/custom_models.py
+-rw-rw-rw-   0        0        0     1387 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/custom/custom_preprocessors.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.222529 tmrl-0.6.6/tmrl/custom/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/custom/utils/__init__.py
+-rw-rw-rw-   0        0        0     5463 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/custom/utils/compute_reward.py
+-rw-rw-rw-   0        0        0     2248 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/custom/utils/control_gamepad.py
+-rw-rw-rw-   0        0        0     3981 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/custom/utils/control_keyboard.py
+-rw-rw-rw-   0        0        0     1710 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/custom/utils/control_mouse.py
+-rw-rw-rw-   0        0        0     9041 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/custom/utils/nn.py
+-rw-rw-rw-   0        0        0     5019 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/custom/utils/tools.py
+-rw-rw-rw-   0        0        0     9247 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/custom/utils/window.py
+-rw-rw-rw-   0        0        0     1291 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/envs.py
+-rw-rw-rw-   0        0        0     9555 2024-04-08 03:28:54.000000 tmrl-0.6.6/tmrl/memory.py
+-rw-rw-rw-   0        0        0    41787 2024-05-15 20:19:23.000000 tmrl-0.6.6/tmrl/networking.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.238551 tmrl-0.6.6/tmrl/tools/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/tools/__init__.py
+-rw-rw-rw-   0        0        0     2922 2024-05-15 20:18:54.000000 tmrl-0.6.6/tmrl/tools/check_environment.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.285565 tmrl-0.6.6/tmrl/tools/init_package/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/tools/init_package/__init__.py
+-rw-rw-rw-   0        0        0    27288 2024-04-23 05:21:02.000000 tmrl-0.6.6/tmrl/tools/init_package/init_pywin32.py
+-rw-rw-rw-   0        0        0     4882 2024-04-23 05:21:02.000000 tmrl-0.6.6/tmrl/tools/init_package/init_tmrl.py
+-rw-rw-rw-   0        0        0     3235 2024-05-15 20:18:54.000000 tmrl-0.6.6/tmrl/tools/record.py
+-rw-rw-rw-   0        0        0     1279 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/tools/save_replays.py
+-rw-rw-rw-   0        0        0     1390 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/training.py
+-rw-rw-rw-   0        0        0    10895 2024-05-05 18:46:41.000000 tmrl-0.6.6/tmrl/training_offline.py
+-rw-rw-rw-   0        0        0    10255 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/util.py
+-rw-rw-rw-   0        0        0     2031 2024-04-08 03:24:28.000000 tmrl-0.6.6/tmrl/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:43.955622 tmrl-0.6.6/tmrl.egg-info/
+-rw-rw-rw-   0        0        0     2052 2024-05-15 20:29:43.000000 tmrl-0.6.6/tmrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2024-05-15 20:29:43.000000 tmrl-0.6.6/tmrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:29:43.000000 tmrl-0.6.6/tmrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-05-15 20:29:43.000000 tmrl-0.6.6/tmrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 20:29:43.000000 tmrl-0.6.6/tmrl.egg-info/top_level.txt
```

### Comparing `tmrl-0.6.5/LICENSE` & `tmrl-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/PKG-INFO` & `tmrl-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tmrl
-Version: 0.6.5
+Version: 0.6.6
 Summary: Network-based framework for real-time robot learning
 Home-page: https://github.com/trackmania-rl/tmrl
-Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.5.tar.gz
+Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.6.tar.gz
 Author: Yann Bouteiller, Edouard Geze
 Author-email: yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr
 License: MIT
 Keywords: reinforcement learning,robot learning,trackmania,self driving,roborace
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `tmrl-0.6.5/README.md` & `tmrl-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/readme/pypi.md` & `tmrl-0.6.6/readme/pypi.md`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/setup.py` & `tmrl-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,21 +133,21 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 README_FOLDER = os.path.join(HERE, "readme")
 with open(os.path.join(README_FOLDER, "pypi.md")) as fid:
     README = fid.read()
 
 setup(
     name='tmrl',
-    version='0.6.5',
+    version='0.6.6',
     description='Network-based framework for real-time robot learning',
     long_description=README,
     long_description_content_type='text/markdown',
     keywords='reinforcement learning, robot learning, trackmania, self driving, roborace',
     url='https://github.com/trackmania-rl/tmrl',
-    download_url='https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.5.tar.gz',
+    download_url='https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.6.tar.gz',
     author='Yann Bouteiller, Edouard Geze',
     author_email='yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr',
     license='MIT',
     install_requires=install_req,
     classifiers=[
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
```

### Comparing `tmrl-0.6.5/tmrl/__init__.py` & `tmrl-0.6.6/tmrl/__init__.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/__main__.py` & `tmrl-0.6.6/tmrl/__main__.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/actor.py` & `tmrl-0.6.6/tmrl/actor.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/config/config_constants.py` & `tmrl-0.6.6/tmrl/config/config_constants.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/config/config_objects.py` & `tmrl-0.6.6/tmrl/config/config_objects.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/custom_algorithms.py` & `tmrl-0.6.6/tmrl/custom/custom_algorithms.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/custom_checkpoints.py` & `tmrl-0.6.6/tmrl/custom/custom_checkpoints.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/custom_gym_interfaces.py` & `tmrl-0.6.6/tmrl/custom/custom_gym_interfaces.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/custom_memories.py` & `tmrl-0.6.6/tmrl/custom/custom_memories.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/custom_models.py` & `tmrl-0.6.6/tmrl/custom/custom_models.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/custom_preprocessors.py` & `tmrl-0.6.6/tmrl/custom/custom_preprocessors.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/utils/compute_reward.py` & `tmrl-0.6.6/tmrl/custom/utils/compute_reward.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/utils/control_gamepad.py` & `tmrl-0.6.6/tmrl/custom/utils/control_gamepad.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/utils/control_keyboard.py` & `tmrl-0.6.6/tmrl/custom/utils/control_keyboard.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/utils/control_mouse.py` & `tmrl-0.6.6/tmrl/custom/utils/control_mouse.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/utils/nn.py` & `tmrl-0.6.6/tmrl/custom/utils/nn.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/utils/tools.py` & `tmrl-0.6.6/tmrl/custom/utils/tools.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/custom/utils/window.py` & `tmrl-0.6.6/tmrl/custom/utils/window.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/envs.py` & `tmrl-0.6.6/tmrl/envs.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/memory.py` & `tmrl-0.6.6/tmrl/memory.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/networking.py` & `tmrl-0.6.6/tmrl/networking.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import socket
 import time
 import atexit
 import json
 import shutil
 import tempfile
+import itertools
 from os.path import exists
 
 # third-party imports
 import numpy as np
 from requests import get
 from tlspyo import Relay, Endpoint
 
@@ -637,18 +638,20 @@
         Args:
             max_samples (int): if the environment is not `terminated` after `max_samples` time steps,
                 it is forcefully reset and `truncated` is set to True.
         """
         if max_samples is None:
             max_samples = self.max_samples_per_episode
 
+        iterator = range(max_samples) if max_samples != np.inf else itertools.count()
+
         ret = 0.0
         steps = 0
         obs, info = self.reset(collect_samples=True)
-        for i in range(max_samples):
+        for i in iterator:
             obs, rew, terminated, truncated, info = self.step(obs=obs, test=False, collect_samples=True, last_step=i == max_samples - 1)
             ret += rew
             steps += 1
             if terminated or truncated:
                 break
         self.buffer.stat_train_return = ret
         self.buffer.stat_train_steps = steps
@@ -661,36 +664,38 @@
             max_samples_per_episode (int): same as run_episode
             nb_episodes (int): total number of episodes to collect
             train (bool): same as run_episode
         """
         if max_samples_per_episode is None:
             max_samples_per_episode = self.max_samples_per_episode
 
-        counter = 0
-        while counter < nb_episodes:
+        iterator = range(nb_episodes) if nb_episodes != np.inf else itertools.count()
+
+        for _ in iterator:
             self.run_episode(max_samples_per_episode, train=train)
-            counter += 1
 
     def run_episode(self, max_samples=None, train=False):
         """
         Collects a maximum of `max_samples` test transitions (from reset to terminated or truncated).
 
         Args:
             max_samples (int): At most `max_samples` samples are collected per episode.
                 If the episode is longer, it is forcefully reset and `truncated` is set to True.
             train (bool): whether the episode is a training or a test episode.
                 `step` is called with `test=not train`.
         """
         if max_samples is None:
             max_samples = self.max_samples_per_episode
 
+        iterator = range(max_samples) if max_samples != np.inf else itertools.count()
+
         ret = 0.0
         steps = 0
         obs, info = self.reset(collect_samples=False)
-        for _ in range(max_samples):
+        for _ in iterator:
             obs, rew, terminated, truncated, info = self.step(obs=obs, test=not train, collect_samples=False)
             ret += rew
             steps += 1
             if terminated or truncated:
                 break
         self.buffer.stat_test_return = ret
         self.buffer.stat_test_steps = steps
@@ -707,57 +712,53 @@
             test_episode_interval (int): a test episode is collected for every `test_episode_interval` train episodes;
                 set to 0 to not collect test episodes.
             nb_episodes (int): maximum number of train episodes to collect.
             verbose (bool): whether to log INFO messages.
             expert (bool): experts send training samples without updating their model nor running test episodes.
         """
 
-        episode = 0
+        iterator = range(nb_episodes) if nb_episodes != np.inf else itertools.count()
+
         if expert:
             if not verbose:
-                while episode < nb_episodes:
+                for _ in iterator:
                     self.collect_train_episode(self.max_samples_per_episode)
                     self.send_and_clear_buffer()
                     self.ignore_actor_weights()
-                    episode += 1
             else:
-                while episode < nb_episodes:
+                for _ in iterator:
                     print_with_timestamp("collecting expert episode")
                     self.collect_train_episode(self.max_samples_per_episode)
                     print_with_timestamp("copying buffer for sending")
                     self.send_and_clear_buffer()
                     self.ignore_actor_weights()
-                    episode += 1
         elif not verbose:
             if not test_episode_interval:
-                while episode < nb_episodes:
+                for _ in iterator:
                     self.collect_train_episode(self.max_samples_per_episode)
                     self.send_and_clear_buffer()
                     self.update_actor_weights(verbose=False)
-                    episode += 1
             else:
-                while episode < nb_episodes:
+                for episode in iterator:
                     if episode % test_episode_interval == 0 and not self.crc_debug:
                         self.run_episode(self.max_samples_per_episode, train=False)
                     self.collect_train_episode(self.max_samples_per_episode)
                     self.send_and_clear_buffer()
                     self.update_actor_weights(verbose=False)
-                    episode += 1
         else:
-            while episode < nb_episodes:
+            for episode in iterator:
                 if test_episode_interval and episode % test_episode_interval == 0 and not self.crc_debug:
                     print_with_timestamp("running test episode")
                     self.run_episode(self.max_samples_per_episode, train=False)
                 print_with_timestamp("collecting train episode")
                 self.collect_train_episode(self.max_samples_per_episode)
                 print_with_timestamp("copying buffer for sending")
                 self.send_and_clear_buffer()
                 print_with_timestamp("checking for new weights")
                 self.update_actor_weights(verbose=True)
-                episode += 1
 
     def run_synchronous(self,
                         test_episode_interval=0,
                         nb_steps=np.inf,
                         initial_steps=1,
                         max_steps_per_update=np.inf,
                         end_episodes=True,
@@ -904,14 +905,17 @@
         .. _rtgym: https://github.com/yannbouteiller/rtgym
 
         Args:
             nb_steps (int): number of steps to perform to compute the benchmark
             test (int): whether the actor is called in test or train mode
             verbose (bool): whether to log INFO messages
         """
+        if nb_steps == np.inf or nb_steps < 0:
+            raise RuntimeError(f"Invalid number of steps: {nb_steps}")
+
         obs, info = self.reset(collect_samples=False)
         for _ in range(nb_steps):
             obs, rew, terminated, truncated, info = self.step(obs=obs, test=test, collect_samples=False)
             if terminated or truncated:
                 break
         res = self.env.benchmarks()
         if verbose:
```

### Comparing `tmrl-0.6.5/tmrl/tools/check_environment.py` & `tmrl-0.6.6/tmrl/tools/check_environment.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/tools/init_package/init_pywin32.py` & `tmrl-0.6.6/tmrl/tools/init_package/init_pywin32.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/tools/init_package/init_tmrl.py` & `tmrl-0.6.6/tmrl/tools/init_package/init_tmrl.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/tools/record.py` & `tmrl-0.6.6/tmrl/tools/record.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/tools/save_replays.py` & `tmrl-0.6.6/tmrl/tools/save_replays.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/training.py` & `tmrl-0.6.6/tmrl/training.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/training_offline.py` & `tmrl-0.6.6/tmrl/training_offline.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/util.py` & `tmrl-0.6.6/tmrl/util.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl/wrappers.py` & `tmrl-0.6.6/tmrl/wrappers.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.5/tmrl.egg-info/PKG-INFO` & `tmrl-0.6.6/tmrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tmrl
-Version: 0.6.5
+Version: 0.6.6
 Summary: Network-based framework for real-time robot learning
 Home-page: https://github.com/trackmania-rl/tmrl
-Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.5.tar.gz
+Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.6.tar.gz
 Author: Yann Bouteiller, Edouard Geze
 Author-email: yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr
 License: MIT
 Keywords: reinforcement learning,robot learning,trackmania,self driving,roborace
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `tmrl-0.6.5/tmrl.egg-info/SOURCES.txt` & `tmrl-0.6.6/tmrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

