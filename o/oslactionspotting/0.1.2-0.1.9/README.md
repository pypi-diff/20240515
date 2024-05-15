# Comparing `tmp/oslactionspotting-0.1.2.tar.gz` & `tmp/oslactionspotting-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslactionspotting-0.1.2.tar", last modified: Mon May  6 17:53:30 2024, max compression
+gzip compressed data, was "oslactionspotting-0.1.9.tar", last modified: Wed May 15 12:13:25 2024, max compression
```

## Comparing `oslactionspotting-0.1.2.tar` & `oslactionspotting-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:53:29.997608 oslactionspotting-0.1.2/oslactionspotting/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/oslactionspotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/oslactionspotting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.154826 oslactionspotting-0.1.9/oslactionspotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.154826 oslactionspotting-0.1.9/oslactionspotting/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/apis/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.154826 oslactionspotting-0.1.9/oslactionspotting/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.154826 oslactionspotting-0.1.9/oslactionspotting/core/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/loss/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/loss/calf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/loss/ce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/loss/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/loss/nll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.154826 oslactionspotting-0.1.9/oslactionspotting/core/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14209 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.154826 oslactionspotting-0.1.9/oslactionspotting/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.158826 oslactionspotting-0.1.9/oslactionspotting/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/dali.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/default_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37267 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/core/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.158826 oslactionspotting-0.1.9/oslactionspotting/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38740 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/datasets/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22211 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/datasets/soccernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/datasets/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/oslactionspotting/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/oslactionspotting/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/contextaware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/e2espot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/oslactionspotting/models/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/heads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/oslactionspotting/models/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/impl/asformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/impl/calf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/impl/gsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15399 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/impl/gtad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/impl/tsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/learnablepooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/litebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/oslactionspotting/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/necks/calf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/necks/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/oslactionspotting/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/oslactionspotting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-15 12:13:25.000000 oslactionspotting-0.1.9/oslactionspotting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 12:13:25.000000 oslactionspotting-0.1.9/oslactionspotting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:13:25.000000 oslactionspotting-0.1.9/oslactionspotting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 12:13:25.000000 oslactionspotting-0.1.9/oslactionspotting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 12:13:25.000000 oslactionspotting-0.1.9/oslactionspotting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:13:25.162826 oslactionspotting-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 12:13:14.000000 oslactionspotting-0.1.9/tests/test_simple.py
```

### Comparing `oslactionspotting-0.1.2/LICENSE` & `oslactionspotting-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oslactionspotting-0.1.2/PKG-INFO` & `oslactionspotting-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslactionspotting
-Version: 0.1.2
+Version: 0.1.9
 Summary: Action Spotting SDK
 Home-page: https://github.com/OpenSportsLab/OSL-ActionSpotting
 Author: ['Silvio Giancola', 'Yassine Benzakour']
 Author-email: ['silvio.giancola@kaust.edu.sa', 'yassine.benzakour@student.uliege.be']
 License: MIT
 Keywords: SoccerNet,SDK,Spotting,Football,Soccer,Video
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,19 @@
 Requires-Dist: SoccerNet
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: mmengine
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: pytorch-lightning
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: moviepy
+Requires-Dist: tabulate
+Requires-Dist: timm
 
 # OSL-ActionSpotting: A Unified Library for Action Spotting in Sports Videos
 
 [![ArXiv](https://img.shields.io/badge/arXiv-xxx.xxx-b31b1b.svg?style=flat)](https://arxiv.org/abs/xxx.xxx)
 [![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)](https://github.com/SoccerNet/sn-spotting-pip/blob/main/LICENSE)
 
 OSL-ActionSpotting is a plug-and-play library that unifies action
```

### Comparing `oslactionspotting-0.1.2/README.md` & `oslactionspotting-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oslactionspotting-0.1.2/oslactionspotting.egg-info/PKG-INFO` & `oslactionspotting-0.1.9/oslactionspotting.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslactionspotting
-Version: 0.1.2
+Version: 0.1.9
 Summary: Action Spotting SDK
 Home-page: https://github.com/OpenSportsLab/OSL-ActionSpotting
 Author: ['Silvio Giancola', 'Yassine Benzakour']
 Author-email: ['silvio.giancola@kaust.edu.sa', 'yassine.benzakour@student.uliege.be']
 License: MIT
 Keywords: SoccerNet,SDK,Spotting,Football,Soccer,Video
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,19 @@
 Requires-Dist: SoccerNet
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: mmengine
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: pytorch-lightning
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: moviepy
+Requires-Dist: tabulate
+Requires-Dist: timm
 
 # OSL-ActionSpotting: A Unified Library for Action Spotting in Sports Videos
 
 [![ArXiv](https://img.shields.io/badge/arXiv-xxx.xxx-b31b1b.svg?style=flat)](https://arxiv.org/abs/xxx.xxx)
 [![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)](https://github.com/SoccerNet/sn-spotting-pip/blob/main/LICENSE)
 
 OSL-ActionSpotting is a plug-and-play library that unifies action
```

### Comparing `oslactionspotting-0.1.2/setup.py` & `oslactionspotting-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from oslactionspotting import __version__, __authors__, __author_email__, __github__
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='oslactionspotting',         # How you named your package folder (MyLib)
-    packages=['oslactionspotting'],   # Chose the same as "name"
+    packages= find_packages(),
+    # packages=['oslactionspotting'],   # Chose the same as "name"
     # Start with a small number and increase it with every change you make
     version=__version__,
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     description='Action Spotting SDK',   # Give a short description about your library
     long_description=readme + '\n\n',
     long_description_content_type='text/markdown',
@@ -32,15 +33,20 @@
         'tqdm',
         'SoccerNet',
         'matplotlib',
         'scikit-learn',
         'mmengine',
         'torch',
         'torchvision',
-        'pytorch-lightning'
+        'pytorch-lightning',
+        'numpy',
+        'opencv-python',
+        'moviepy',
+        'tabulate',
+        'timm'
         # 'scikit-video',
         # 'matplotlib',
         # 'google-measurement-protocol',
         # 'pycocoevalcap',
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

