# Comparing `tmp/llamascript-0.5.0.tar.gz` & `tmp/llamascript-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamascript-0.5.0.tar", last modified: Fri May 10 20:00:14 2024, max compression
+gzip compressed data, was "llamascript-0.6.0.tar", last modified: Wed May 15 15:13:27 2024, max compression
```

## Comparing `llamascript-0.5.0.tar` & `llamascript-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:00:14.238740 llamascript-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-10 20:00:09.000000 llamascript-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-10 20:00:14.238740 llamascript-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-10 20:00:09.000000 llamascript-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:00:14.238740 llamascript-0.5.0/llamascript/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 20:00:09.000000 llamascript-0.5.0/llamascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-10 20:00:09.000000 llamascript-0.5.0/llamascript/embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-10 20:00:09.000000 llamascript-0.5.0/llamascript/lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-10 20:00:09.000000 llamascript-0.5.0/llamascript/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:00:14.238740 llamascript-0.5.0/llamascript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-10 20:00:14.000000 llamascript-0.5.0/llamascript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-10 20:00:14.000000 llamascript-0.5.0/llamascript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:00:14.000000 llamascript-0.5.0/llamascript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 20:00:14.000000 llamascript-0.5.0/llamascript.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 20:00:14.000000 llamascript-0.5.0/llamascript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 20:00:14.000000 llamascript-0.5.0/llamascript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:00:14.238740 llamascript-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-10 20:00:09.000000 llamascript-0.5.0/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-15 15:13:27.148214 llamascript-0.6.0/
+-rw-r--r--   0 lewis-family   (501) staff       (20)    11324 2024-04-30 20:50:05.000000 llamascript-0.6.0/LICENSE
+-rw-r--r--   0 lewis-family   (501) staff       (20)     3084 2024-05-15 15:13:27.147089 llamascript-0.6.0/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2620 2024-05-15 14:46:22.000000 llamascript-0.6.0/README.md
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-15 15:13:27.142538 llamascript-0.6.0/llamascript/
+-rw-r--r--   0 lewis-family   (501) staff       (20)       42 2024-05-15 14:56:58.000000 llamascript-0.6.0/llamascript/__init__.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)     7270 2024-05-15 15:08:50.000000 llamascript-0.6.0/llamascript/lang.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-15 15:13:27.146188 llamascript-0.6.0/llamascript.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     3084 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      282 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       53 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/entry_points.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/requires.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       12 2024-05-15 15:13:27.000000 llamascript-0.6.0/llamascript.egg-info/top_level.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-05-15 15:13:27.148423 llamascript-0.6.0/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)      947 2024-05-15 15:11:10.000000 llamascript-0.6.0/setup.py
```

### Comparing `llamascript-0.5.0/LICENSE` & `llamascript-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llamascript-0.5.0/PKG-INFO` & `llamascript-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.5.0
+Version: 0.6.0
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ollama
 
+<div style="border-radius: 20px;" align="center">
+  <img width="128" height="128" src="https://github.com/Project-Llama/.github/blob/main/profile/IMG_1443.png">
+</div>
+
 # LlamaScript
 
 [Medium Post](https://medium.com/@wolfthedev/llamascript-simple-ai-builder-74442dc9b090)
 
-[![Black Format](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml)
-[![Upload to PyPi](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml)
-[![CodeQL](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql)
-[![Tests](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml)
+[![Black Format](https://github.com/Project-Llama/llamascript/actions/workflows/format.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml)
+[![Upload to PyPi](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml)
+[![CodeQL](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql)
 
 [![VS Code Extension Downloads](https://img.shields.io/visual-studio-marketplace/d/WolfTheDev.llamascript?label=VS-Code%20Downloads)](https://marketplace.visualstudio.com/items?itemName=WolfTheDev.llamascript)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/w/WolfTheDeveloper/llamascript?label=Commits)
-![GitHub License](https://img.shields.io/github/license/WolfTheDeveloper/llamascript?label=License)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/Project-Llama/llamascript?label=Commits)
+![GitHub License](https://img.shields.io/github/license/Project-Llama/llamascript?label=License)
 
 LlamaScript is a no-code AI chatbot using Ollama.
 
 ## Table of Contents
 - [LlamaScript](#llamascript)
   - [Installation](#installation)
   - [Usage](#usage)
   - [License](#license)
   - [Roadmap](#roadmap)
+  - [Examples](examples/)
 
 ## Installation
 
 You can install LlamaScript using pip:
 
 ```bash
 pip install llamascript
@@ -76,8 +80,9 @@
 ## License
 LlamaScript is licensed under the Apache 2.0 License.
 
 ## Roadmap
 Things to come in the future:
 
 - An `API` command to serve on Flask
+- Plugins/Extensions handling (Help Wanted)
```

### Comparing `llamascript-0.5.0/README.md` & `llamascript-0.6.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+<div style="border-radius: 20px;" align="center">
+  <img width="128" height="128" src="https://github.com/Project-Llama/.github/blob/main/profile/IMG_1443.png">
+</div>
+
 # LlamaScript
 
 [Medium Post](https://medium.com/@wolfthedev/llamascript-simple-ai-builder-74442dc9b090)
 
-[![Black Format](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml)
-[![Upload to PyPi](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml)
-[![CodeQL](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql)
-[![Tests](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml)
+[![Black Format](https://github.com/Project-Llama/llamascript/actions/workflows/format.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml)
+[![Upload to PyPi](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml)
+[![CodeQL](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql)
 
 [![VS Code Extension Downloads](https://img.shields.io/visual-studio-marketplace/d/WolfTheDev.llamascript?label=VS-Code%20Downloads)](https://marketplace.visualstudio.com/items?itemName=WolfTheDev.llamascript)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/w/WolfTheDeveloper/llamascript?label=Commits)
-![GitHub License](https://img.shields.io/github/license/WolfTheDeveloper/llamascript?label=License)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/Project-Llama/llamascript?label=Commits)
+![GitHub License](https://img.shields.io/github/license/Project-Llama/llamascript?label=License)
 
 LlamaScript is a no-code AI chatbot using Ollama.
 
 ## Table of Contents
 - [LlamaScript](#llamascript)
   - [Installation](#installation)
   - [Usage](#usage)
   - [License](#license)
   - [Roadmap](#roadmap)
+  - [Examples](examples/)
 
 ## Installation
 
 You can install LlamaScript using pip:
 
 ```bash
 pip install llamascript
@@ -61,8 +65,9 @@
 ## License
 LlamaScript is licensed under the Apache 2.0 License.
 
 ## Roadmap
 Things to come in the future:
 
 - An `API` command to serve on Flask
+- Plugins/Extensions handling (Help Wanted)
```

### Comparing `llamascript-0.5.0/llamascript/lang.py` & `llamascript-0.6.0/llamascript/lang.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 class llama:
     def __init__(self):
         self.model = ""
         self.data = ""
         self.system = []
-        self.ignore = False
 
     def USE(self, line):
         if line.split(" ")[0] == "USE":
             self.model = line.split(" ")[1].strip()
         else:
             raise ValueError("Invalid model")
 
@@ -95,25 +94,48 @@
                         print(stdout.decode())
             print("Removing Modelfile...")
             os.remove(filename)
 
         except Exception as e:
             logging.error("Error creating model file: %s", e)
             print(f"Error creating model file {filename}.")
+        
+    def REPEAT(self, command, repeat_count):
+        for _ in range(repeat_count):
+            self.execute_command(command)
+
+    def execute_command(self, command):
+        if command.startswith("PROMPT INPUT"):
+            self.INPUT("PROMPT")
+        elif command.startswith("CHAT"):
+            self.CHAT()
+        else:
+            raise ValueError("Invalid command to repeat")
 
     async def read(self, filename):
         try:
             with open(filename, "r") as file:
-                for line in file:
-                    line = line.strip()
+                lines = file.readlines()
+                i = 0
+                while i < len(lines):
+                    line = lines[i].strip()
                     if not line:
+                        i += 1
                         continue
                     command = line.split(" ")
-                    if command[0] == "IGNORE":
-                        self.ignore = True
+                    if command[0] == "REPEAT":
+                        repeat_count = int(command[1]) if len(command) > 1 else 1
+                        repeat_commands = []
+                        i += 1
+                        while i < len(lines) and not lines[i].strip().startswith("ENDREPEAT"):
+                            repeat_commands.append(lines[i].strip())
+                            i += 1
+                        for _ in range(repeat_count):
+                            for repeat_command in repeat_commands:
+                                self.execute_command(repeat_command)
                     elif command[0] == "USE":
                         self.USE(line)
                     elif len(command) > 1 and command[1] == "INPUT":
                         self.INPUT(command[0])
                     elif command[0] == "SYSTEM":
                         self.SYSTEM(line=line)
                     elif command[0] == "PROMPT":
@@ -131,20 +153,19 @@
                         }
                         self.CREATE_MODEL("Modelfile", parameters, model_name)
                     elif command[0] == "CHAT":
                         if len(command) > 1 and command[1] == "STREAM":
                             stream = command[1] == True
                         else:
                             stream = False
-                        if not self.ignore:
-                            print(
-                                '=================\nThanks for using llama, a no-code AI chatbot. Please ensure Ollama (https://ollama.com) is running. To get started, type "USE" followed by the model you want to use. Then, type "PROMPT" followed by the prompt you want to use. Finally, type "CHAT" to chat with the AI. To run a script, type "llamascript" to run your script. To ignore this message, add "IGNORE" to the beginning of your llama file.\n================='
-                            )
-                            self.ignore = True
                         self.CHAT(stream=stream)
+                    elif command[0] == "REPEAT":
+                        repeat_count = int(command[1]) if len(command) > 1 else 1
+                        repeat_command = " ".join(command[2:])
+                        self.REPEAT(repeat_command, repeat_count)
                     else:
                         raise ValueError("Invalid command")
         except FileNotFoundError:
             logging.error("File %s not found.", filename)
             print(f"File {filename} not found.")
```

### Comparing `llamascript-0.5.0/llamascript.egg-info/PKG-INFO` & `llamascript-0.6.0/llamascript.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.5.0
+Version: 0.6.0
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ollama
 
+<div style="border-radius: 20px;" align="center">
+  <img width="128" height="128" src="https://github.com/Project-Llama/.github/blob/main/profile/IMG_1443.png">
+</div>
+
 # LlamaScript
 
 [Medium Post](https://medium.com/@wolfthedev/llamascript-simple-ai-builder-74442dc9b090)
 
-[![Black Format](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml)
-[![Upload to PyPi](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml)
-[![CodeQL](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql)
-[![Tests](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/test.yml)
+[![Black Format](https://github.com/Project-Llama/llamascript/actions/workflows/format.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/format.yml)
+[![Upload to PyPi](https://github.com/Project-Llama/llamascript/actions/workflows/python-publish.yml/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/python-publish.yml)
+[![CodeQL](https://github.com/Project-Llama/llamascript/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/WolfTheDeveloper/llamascript/actions/workflows/github-code-scanning/codeql)
 
 [![VS Code Extension Downloads](https://img.shields.io/visual-studio-marketplace/d/WolfTheDev.llamascript?label=VS-Code%20Downloads)](https://marketplace.visualstudio.com/items?itemName=WolfTheDev.llamascript)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/w/WolfTheDeveloper/llamascript?label=Commits)
-![GitHub License](https://img.shields.io/github/license/WolfTheDeveloper/llamascript?label=License)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/Project-Llama/llamascript?label=Commits)
+![GitHub License](https://img.shields.io/github/license/Project-Llama/llamascript?label=License)
 
 LlamaScript is a no-code AI chatbot using Ollama.
 
 ## Table of Contents
 - [LlamaScript](#llamascript)
   - [Installation](#installation)
   - [Usage](#usage)
   - [License](#license)
   - [Roadmap](#roadmap)
+  - [Examples](examples/)
 
 ## Installation
 
 You can install LlamaScript using pip:
 
 ```bash
 pip install llamascript
@@ -76,8 +80,9 @@
 ## License
 LlamaScript is licensed under the Apache 2.0 License.
 
 ## Roadmap
 Things to come in the future:
 
 - An `API` command to serve on Flask
+- Plugins/Extensions handling (Help Wanted)
```

