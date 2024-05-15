# Comparing `tmp/bambot-0.4.3.tar.gz` & `tmp/bambot-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.4.3.tar", last modified: Fri May  3 06:18:15 2024, max compression
+gzip compressed data, was "bambot-0.4.4.tar", last modified: Wed May 15 07:02:49 2024, max compression
```

## Comparing `bambot-0.4.3.tar` & `bambot-0.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 06:18:15.163607 bambot-0.4.3/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2254 2024-05-03 06:18:15.163394 bambot-0.4.3/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1337 2024-05-03 06:15:50.000000 bambot-0.4.3/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 06:18:15.157008 bambot-0.4.3/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)        0 2024-05-01 04:48:56.000000 bambot-0.4.3/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      468 2024-05-03 04:59:26.000000 bambot-0.4.3/bambot/app.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1427 2024-05-03 06:03:43.000000 bambot-0.4.3/bambot/build.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1325 2024-05-03 05:56:52.000000 bambot-0.4.3/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1590 2024-05-03 04:51:24.000000 bambot-0.4.3/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1609 2024-05-03 06:10:47.000000 bambot-0.4.3/bambot/project.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1457 2024-05-03 05:03:21.000000 bambot-0.4.3/bambot/run.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 06:18:15.162682 bambot-0.4.3/bambot/templates/
--rw-r--r--   0 spencerkinney   (501) staff       (20)      329 2024-05-03 05:52:19.000000 bambot-0.4.3/bambot/templates/Dockerfile
--rw-r--r--   0 spencerkinney   (501) staff       (20)      171 2024-05-02 22:06:34.000000 bambot-0.4.3/bambot/templates/agent_runner.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      942 2024-05-03 01:32:06.000000 bambot-0.4.3/bambot/templates/agent_template.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      528 2024-05-02 21:29:55.000000 bambot-0.4.3/bambot/templates/langchain_template.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)       35 2024-05-03 05:17:39.000000 bambot-0.4.3/bambot/templates/requirements.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)     3875 2024-05-03 06:07:04.000000 bambot-0.4.3/bambot/templates/server.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     3312 2024-05-03 05:35:32.000000 bambot-0.4.3/bambot/utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 06:18:15.163135 bambot-0.4.3/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2254 2024-05-03 06:18:15.000000 bambot-0.4.3/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      530 2024-05-03 06:18:15.000000 bambot-0.4.3/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-05-03 06:18:15.000000 bambot-0.4.3/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       40 2024-05-03 06:18:15.000000 bambot-0.4.3/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       46 2024-05-03 06:18:15.000000 bambot-0.4.3/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-05-03 06:18:15.000000 bambot-0.4.3/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-05-03 06:18:15.163640 bambot-0.4.3/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1234 2024-05-03 06:15:59.000000 bambot-0.4.3/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-15 07:02:49.799245 bambot-0.4.4/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2248 2024-05-15 07:02:49.799015 bambot-0.4.4/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1331 2024-05-15 06:59:48.000000 bambot-0.4.4/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-15 07:02:49.796078 bambot-0.4.4/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        0 2024-05-01 04:48:56.000000 bambot-0.4.4/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      468 2024-05-15 06:26:45.000000 bambot-0.4.4/bambot/app.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1869 2024-05-15 06:54:28.000000 bambot-0.4.4/bambot/build.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1325 2024-05-15 06:26:34.000000 bambot-0.4.4/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1666 2024-05-15 06:40:42.000000 bambot-0.4.4/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1609 2024-05-03 06:10:47.000000 bambot-0.4.4/bambot/project.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1457 2024-05-03 05:03:21.000000 bambot-0.4.4/bambot/run.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-15 07:02:49.798386 bambot-0.4.4/bambot/templates/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      329 2024-05-15 06:38:26.000000 bambot-0.4.4/bambot/templates/Dockerfile
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      171 2024-05-02 22:06:34.000000 bambot-0.4.4/bambot/templates/agent_runner.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      942 2024-05-03 01:32:06.000000 bambot-0.4.4/bambot/templates/agent_template.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      528 2024-05-02 21:29:55.000000 bambot-0.4.4/bambot/templates/langchain_template.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       49 2024-05-15 06:30:42.000000 bambot-0.4.4/bambot/templates/requirements.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     3920 2024-05-15 06:31:49.000000 bambot-0.4.4/bambot/templates/server.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     3326 2024-05-15 06:58:09.000000 bambot-0.4.4/bambot/utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-15 07:02:49.798783 bambot-0.4.4/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2248 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      530 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       40 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       46 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-05-15 07:02:49.000000 bambot-0.4.4/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-05-15 07:02:49.799278 bambot-0.4.4/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1234 2024-05-15 07:02:09.000000 bambot-0.4.4/setup.py
```

### Comparing `bambot-0.4.3/PKG-INFO` & `bambot-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.4.3
+Version: 0.4.4
 Summary: Containers for AI agents
 Home-page: https://github.com/Bam-Corp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 Requires-Dist: tqdm
 Requires-Dist: python-dotenv
 Requires-Dist: halo
 Requires-Dist: colorama
 
 # Bam
 
-[![PyPI version](https://badge.fury.io/py/bambot.svg)](https://badge.fury.io/py/bambot)
+[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bam)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Bam is a lightweight and easy-to-use command-line interface (CLI) tool for creating and running AI agent containers. It is currently Docker-based.
 
 ## Installation
 
 You can install Bam using pip:
```

### Comparing `bambot-0.4.3/README.md` & `bambot-0.4.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Bam
 
-[![PyPI version](https://badge.fury.io/py/bambot.svg)](https://badge.fury.io/py/bambot)
+[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bam)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Bam is a lightweight and easy-to-use command-line interface (CLI) tool for creating and running AI agent containers. It is currently Docker-based.
 
 ## Installation
 
 You can install Bam using pip:
```

### Comparing `bambot-0.4.3/bambot/build.py` & `bambot-0.4.4/bambot/build.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,23 +8,36 @@
     """Build the Bam project"""
     project_dir = os.getcwd()
     container_name = os.path.basename(project_dir)
 
     with contextmanager_spinner(f"Building Docker image for '{container_name}'...") as spinner:
         try:
             docker_client = docker.from_env()
-            image, _ = docker_client.images.build(path=project_dir, tag=f"{container_name}:latest", dockerfile="Dockerfile")
+            response = docker_client.api.build(
+                path=project_dir, 
+                tag=f"{os.path.basename(project_dir)}:latest", 
+                dockerfile="Dockerfile", 
+                rm=True,
+                decode=True
+            )
+
+            # Process and print build logs as they arrive
+            for output in response:
+                if 'stream' in output:
+                    print(output['stream'].strip())
+                if 'error' in output:
+                    echo_error(f"Error during build: {output['errorDetail']['message']}")
+                    break
             spinner.stop()
             echo_success("Docker image built successfully!")
 
             # Create the container and mount the project directory as a volume
             container = docker_client.containers.create(
                 f"{container_name}:latest",
                 name=container_name,
-                detach=True,
                 tty=True,
                 stdin_open=True,
                 ports={'1337/tcp': ('127.0.0.1', 1337)},
                 volumes={project_dir: {'bind': '/app', 'mode': 'rw'}}
             )
             echo_success(f"Container '{container_name}' created successfully!")
         except docker.errors.BuildError as e:
```

### Comparing `bambot-0.4.3/bambot/cli.py` & `bambot-0.4.4/bambot/cli.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.3/bambot/docker_utils.py` & `bambot-0.4.4/bambot/docker_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 
 def build_image(container_dir):
     """Build a Docker image for an AI agent"""
     docker_client = docker.from_env()
     image, _ = docker_client.images.build(path=container_dir, tag=f"{os.path.basename(container_dir)}:latest", dockerfile="Dockerfile")
     return image
 
-def create_docker_container(container_name, env_vars=None):
+def create_docker_container(container_name, project_dir, env_vars=None):
     """Create a Docker container for an AI agent"""
     docker_client = docker.from_env()
     container = docker_client.containers.create(
         f"{container_name}:latest",
         name=container_name,
         environment=env_vars,
         detach=True,
         tty=True,
         stdin_open=True,
         ports={'1337/tcp': ('127.0.0.1', 1337)},
+        volumes={project_dir: {'bind': '/app', 'mode': 'rw'}},
     )
     return container
 
 def prune_system(progress_bar=None):
     """Prune Docker system resources"""
     docker_client = docker.from_env()
     tasks = [
```

### Comparing `bambot-0.4.3/bambot/project.py` & `bambot-0.4.4/bambot/project.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.3/bambot/run.py` & `bambot-0.4.4/bambot/run.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.3/bambot/templates/agent_template.py` & `bambot-0.4.4/bambot/templates/agent_template.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.3/bambot/templates/langchain_template.py` & `bambot-0.4.4/bambot/templates/langchain_template.py`

 * *Files identical despite different names*

### Comparing `bambot-0.4.3/bambot/templates/server.py` & `bambot-0.4.4/bambot/templates/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # bambot/templates/server.py
 import logging
 from colorama import Fore, Style
 from flask import Flask, render_template_string, jsonify, request
 from flask_cors import CORS
 import datetime
+from dotenv import load_dotenv
+load_dotenv()
 
 from agent_runner import Agent
 
 # Custom logging formatter for color-coded logs
 class ColoredFormatter(logging.Formatter):
     def __init__(self, msg, use_color=True):
         super().__init__(msg)
```

### Comparing `bambot-0.4.3/bambot/utils.py` & `bambot-0.4.4/bambot/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from colorama import Fore, Style
 from halo import Halo
 import docker
 from contextlib import contextmanager
 
 
 def generate_app_name():
-    prefix = "bam"
-    adjectives = ["brave", "clever", "friendly", "gentle", "kind", "lucky", "silly", "witty"]
-    nouns = ["panda", "tiger", "lion", "eagle", "owl", "dolphin", "turtle", "penguin", "koala", "kangaroo"]
-    adjective = random.choice(adjectives)
-    noun = random.choice(nouns)
-    number = ''.join(random.choices(string.digits, k=4))
-    return f"{prefix}-{adjective}-{noun}-{number}"
+    # Simplified structure with less verbosity
+    prefix = "bambot"
+    # Combine adjectives and nouns for more combinations with fewer parts
+    descriptors = ["cool", "smart", "super", "zap", "zip", "jet", "jam", "pod"]
+    # Generate a two-digit number to reduce length but maintain uniqueness
+    number = random.choices(string.digits, k=2)
+    return f"{prefix}-{random.choice(descriptors)}-{'' .join(number)}"
 
 def setup_logging():
     """Set up colored logging for better visual feedback"""
     logger = logging.getLogger("bam_logger")
     logger.setLevel(logging.DEBUG)
     console_handler = logging.StreamHandler()
     console_handler.setFormatter(ColoredFormatter("[%(levelname)s] %(message)s"))
```

### Comparing `bambot-0.4.3/bambot.egg-info/PKG-INFO` & `bambot-0.4.4/bambot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.4.3
+Version: 0.4.4
 Summary: Containers for AI agents
 Home-page: https://github.com/Bam-Corp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 Requires-Dist: tqdm
 Requires-Dist: python-dotenv
 Requires-Dist: halo
 Requires-Dist: colorama
 
 # Bam
 
-[![PyPI version](https://badge.fury.io/py/bambot.svg)](https://badge.fury.io/py/bambot)
+[![PyPI version](https://badge.fury.io/py/bam.svg)](https://badge.fury.io/py/bam)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Bam is a lightweight and easy-to-use command-line interface (CLI) tool for creating and running AI agent containers. It is currently Docker-based.
 
 ## Installation
 
 You can install Bam using pip:
```

### Comparing `bambot-0.4.3/bambot.egg-info/SOURCES.txt` & `bambot-0.4.4/bambot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambot-0.4.3/setup.py` & `bambot-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bambot",
-    version="0.4.3",
+    version="0.4.4",
     author="Bam Corp",
     author_email="spencer@bam.bot",
     description="Containers for AI agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bam-Corp/bambot",
     packages=find_packages(),
```

