# Comparing `tmp/miniogre-0.6.0.tar.gz` & `tmp/miniogre-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniogre-0.6.0.tar", max compression
+gzip compressed data, was "miniogre-0.7.0.tar", max compression
```

## Comparing `miniogre-0.6.0.tar` & `miniogre-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7173 2024-05-08 05:44:36.958871 miniogre-0.6.0/.env
--rw-r--r--   0        0        0    11357 2024-05-08 05:44:36.958871 miniogre-0.6.0/LICENSE
--rw-r--r--   0        0        0     4134 2024-05-08 05:44:36.958871 miniogre-0.6.0/README.md
--rw-r--r--   0        0        0      125 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/__init__.py
--rw-r--r--   0        0        0    20236 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/actions.py
--rw-r--r--   0        0        0     4564 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/config.py
--rw-r--r--   0        0        0    10561 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/constants.py
--rw-r--r--   0        0        0     3044 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/main.py
--rw-r--r--   0        0        0      792 2024-05-08 05:44:36.958871 miniogre-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 miniogre-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 05:54:31.301456 miniogre-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4134 2024-05-15 05:54:31.301456 miniogre-0.7.0/README.md
+-rw-r--r--   0        0        0      125 2024-05-15 05:54:31.301456 miniogre-0.7.0/miniogre/__init__.py
+-rw-r--r--   0        0        0    22222 2024-05-15 05:54:31.305456 miniogre-0.7.0/miniogre/actions.py
+-rw-r--r--   0        0        0     4564 2024-05-15 05:54:31.305456 miniogre-0.7.0/miniogre/config.py
+-rw-r--r--   0        0        0    11469 2024-05-15 05:54:31.305456 miniogre-0.7.0/miniogre/constants.py
+-rw-r--r--   0        0        0  1681126 2024-05-15 05:54:31.313456 miniogre-0.7.0/miniogre/encodings/9b5ad71b2ce5302211f9c61530b329a4922fc6a4
+-rw-r--r--   0        0        0     3152 2024-05-15 05:54:31.313456 miniogre-0.7.0/miniogre/main.py
+-rw-r--r--   0        0        0      902 2024-05-15 05:54:31.313456 miniogre-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5308 1970-01-01 00:00:00.000000 miniogre-0.7.0/PKG-INFO
```

### Comparing `miniogre-0.6.0/LICENSE` & `miniogre-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniogre-0.6.0/README.md` & `miniogre-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `miniogre-0.6.0/miniogre/actions.py` & `miniogre-0.7.0/miniogre/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ast
 import os
 import platform
 import subprocess
-
+import tiktoken
 import emoji
+import google.generativeai as googleai
 from groq import Groq
 # from groq.cloud.core import Completion
 from mistralai.client import MistralClient
 from mistralai.models.chat_completion import ChatMessage
 from octoai.client import Client as OctoAiClient
 from openai import OpenAI
 from pyfiglet import Figlet
@@ -284,52 +285,69 @@
 #    return response
 
 
 def clean_requirements(provider, requirements):
     cleaning_requirements_emoji()
     if provider == "openai":
         res = clean_requirements_openai(requirements)
+    if provider == "gemini":
+        res = clean_requirements_gemini(requirements)
     elif provider == "ollama":
         res = clean_requirements_ollama(requirements)
     elif provider == "octoai":
         res = clean_requirements_octoai(requirements)
     elif provider == "groq":
         res = clean_requirements_groq(requirements)
     elif provider == "mistral":
         res = clean_requirements_mistral(requirements)
     return res
 
 
-def clean_requirements_ollama(requirements):
-    model = os.getenv("OLLAMA_MODEL", OLLAMA_MODEL)
+def clean_requirements_openai(requirements):
+    model = os.getenv("OPENAI_MODEL", OPENAI_MODEL)
     prompt = os.getenv(
         "CLEAN_REQUIREMENTS_SECRET_PROMPT", CLEAN_REQUIREMENTS_SECRET_PROMPT
     )
-    api_server = os.getenv("OLLAMA_API_SERVER", OLLAMA_API_SERVER)
-    # print(f"{api_server=} {model=} {prompt=}")
-    client = OpenAI(base_url=api_server, api_key="ollama")
+    # print(f"{model=} {prompt=}")
+    client = OpenAI()
     completion = client.chat.completions.create(
         model=model,
         messages=[
             {"role": "system", "content": prompt},
             {"role": "user", "content": requirements},
         ],
     )
     requirements = completion.choices[0].message.content
+    # print(f"{requirements=}")
+    return requirements
 
+
+def clean_requirements_gemini(requirements):
+    model = os.getenv("GEMINI_MODEL", GEMINI_MODEL)
+    prompt = os.getenv(
+        "CLEAN_REQUIREMENTS_SECRET_PROMPT", CLEAN_REQUIREMENTS_SECRET_PROMPT
+    )
+    # print(f"{model=}")
+    client = googleai.GenerativeModel(model)
+    full_prompt = f"{prompt}\n---\n{requirements}"
+    # print(f"{full_prompt=}")
+    response = client.generate_content(full_prompt)
+    requirements = response.text
+    # print(f"{requirements=}")
     return requirements
 
 
-def clean_requirements_openai(requirements):
-    model = os.getenv("OPENAI_MODEL", OPENAI_MODEL)
+def clean_requirements_ollama(requirements):
+    model = os.getenv("OLLAMA_MODEL", OLLAMA_MODEL)
     prompt = os.getenv(
         "CLEAN_REQUIREMENTS_SECRET_PROMPT", CLEAN_REQUIREMENTS_SECRET_PROMPT
     )
-    # print(f"{model=} {prompt=}")
-    client = OpenAI()
+    api_server = os.getenv("OLLAMA_API_SERVER", OLLAMA_API_SERVER)
+    # print(f"{api_server=} {model=} {prompt=}")
+    client = OpenAI(base_url=api_server, api_key="ollama")
     completion = client.chat.completions.create(
         model=model,
         messages=[
             {"role": "system", "content": prompt},
             {"role": "user", "content": requirements},
         ],
     )
@@ -413,68 +431,101 @@
 def save_requirements(requirements, ogre_dir_path):
     requirements_fullpath = os.path.join(ogre_dir_path, "requirements.txt")
     with open(requirements_fullpath, "w") as f:
         f.write(requirements)
     return requirements_fullpath
 
 
+def count_tokens(string) -> int:
+    from importlib.resources import files
+    tiktoken_cache_dir = str(files('miniogre').joinpath('encodings'))
+    os.environ["TIKTOKEN_CACHE_DIR"] = tiktoken_cache_dir
+    cache_key = "9b5ad71b2ce5302211f9c61530b329a4922fc6a4" # cl100k_base
+    assert os.path.exists(os.path.join(tiktoken_cache_dir, cache_key))
+    encoding = tiktoken.get_encoding("cl100k_base")
+    num_tokens = len(encoding.encode(string))
+    return num_tokens
+
+
 def rewrite_readme(provider, readme):
     readme_emoji()
 
     if provider == "openai":
         res = rewrite_readme_openai(readme)
+    elif provider == "gemini":
+        res = rewrite_readme_gemini(readme)
     elif provider == "ollama":
         res = rewrite_readme_ollama(readme)
     elif provider == "octoai":
         res = rewrite_readme_octoai(readme)
     elif provider == "groq":
         res = rewrite_readme_groq(readme)
     elif provider == "mistral":
         res = rewrite_readme_mistral(readme)
     return res
 
 
 def rewrite_readme_openai(readme):
     model = os.getenv("OPENAI_MODEL", OPENAI_MODEL)
     prompt = os.getenv("REWRITE_README_PROMPT", REWRITE_README_PROMPT)
-    client = OpenAI()
+    # print(f"{model=} {prompt=}")
+    new_readme = ""
     if "OPENAI_API_KEY" not in os.environ:
         raise EnvironmentError("OPENAI_API_KEY environment variable not defined")
-
     try:
+        client = OpenAI()
         completion = client.chat.completions.create(
             model=model,
             messages=[
                 {"role": "system", "content": prompt},
                 {"role": "user", "content": readme},
             ],
         )
         # print(completion)
         new_readme = completion.choices[0].message.content
     except Exception as e:
         print(e)
+    return new_readme
 
+
+def rewrite_readme_gemini(readme):
+    model = os.getenv("GEMINI_MODEL", GEMINI_MODEL)
+    prompt = os.getenv("REWRITE_README_PROMPT", REWRITE_README_PROMPT)
+    full_prompt = f"{prompt}\n---\n{readme}"
+    # print(f"{model=} {full_prompt=}")
+    new_readme = ""
+    if "GOOGLE_API_KEY" not in os.environ:
+        raise EnvironmentError("GOOGLE_API_KEY environment variable not defined")
+    try:
+        client = googleai.GenerativeModel(model)
+        response = client.generate_content(full_prompt)
+        new_readme = response.text
+    except Exception as e:
+        print(e)
     return new_readme
 
 
 def rewrite_readme_ollama(readme):
     model = os.getenv("OLLAMA_MODEL", OLLAMA_MODEL)
     prompt = os.getenv("REWRITE_README_PROMPT", REWRITE_README_PROMPT)
     api_server = os.getenv("OLLAMA_API_SERVER", OLLAMA_API_SERVER)
     # print(f"{api_server=} {model=} {prompt=}")
-    client = OpenAI(base_url=api_server, api_key="ollama")
-    completion = client.chat.completions.create(
-        model=model,
-        messages=[
-            {"role": "system", "content": prompt},
-            {"role": "user", "content": readme},
-        ],
-    )
-    new_readme = completion.choices[0].message.content
-
+    new_readme = ""
+    try:
+        client = OpenAI(base_url=api_server, api_key="ollama")
+        completion = client.chat.completions.create(
+            model=model,
+            messages=[
+                {"role": "system", "content": prompt},
+                {"role": "user", "content": readme},
+            ],
+        )
+        new_readme = completion.choices[0].message.content
+    except Exception as e:
+        print(e)
     return new_readme
 
 
 def rewrite_readme_octoai(readme):
     raise NotImplementedError("rewrite_readme_octoai is not implemented.")
 
 
@@ -573,15 +624,15 @@
     spinup_emoji()
 
     project_name = image_name
     container_name = "miniogre-{}".format(image_name.lower())
     image_name = "miniogre/{}:{}".format(image_name.lower(), "latest")
     # cmd = "uv venv; source .venv/bin/activate; cat ./{}/requirements.txt | xargs -L 1 uv pip install; exit 0;"
     # cmd = "cat ./ogre_dir/requirements.txt | xargs -L 1 uv pip install; exit 0"
-    spin_up_cmd = "docker run -it --rm -v {}:/opt/{} -p {} --name {} {}".format(
+    spin_up_cmd = "docker run -it --rm -v {}:/opt/{} -p {} --name {} {} bash".format(
         project_path, project_name, port_map, container_name, image_name
     )
 
     print("   spin up command = {}".format(spin_up_cmd))
     subprocess.call(spin_up_cmd.split())
     # p = subprocess.Popen(spin_up_cmd, stdout=subprocess.PIPE, shell=True)
     # (out, err) = p.communicate()
```

### Comparing `miniogre-0.6.0/miniogre/config.py` & `miniogre-0.7.0/miniogre/config.py`

 * *Files identical despite different names*

### Comparing `miniogre-0.6.0/miniogre/constants.py` & `miniogre-0.7.0/miniogre/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,26 +163,38 @@
     ".cpy",
     ".ipynb",
 ]
 
 OGRE_DIR = "ogre_dir"
 OGRE_BASEIMAGE = "ogrerun/base:ubuntu22.04-{}"
 
-OPENAI_MODEL = "gpt-4-turbo"
+OPENAI_MODEL = "gpt-4o"
 OPENAI_SECRET_PROMPT = """You are a Python requirements generator.
 You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
 The raw text sent by the user consists of a combination of the README file contents and the source code contents.
 You generate only the file contents as answer.
 If the text sent by the user is invalid or is empty, just generate an empty content.
 You should ignore the Python version 2 or 3.
 The python package should not be included in the requirements file.
 Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
 Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
 Your output should be a raw ASCII text file."""
 
+GEMINI_MODEL = "gemini-1.0-pro"
+# GEMINI_SECRET_PROMPT = """You are a Python requirements generator.
+# You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
+# The raw text sent by the user consists of a combination of the README file contents and the source code contents.
+# You generate only the file contents as answer.
+# If the text sent by the user is invalid or is empty, just generate an empty content.
+# You should ignore the Python version 2 or 3.
+# The python package should not be included in the requirements file.
+# Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
+# Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
+# Your output should be a raw ASCII text file."""
+
 # OLLAMA_MODEL = "mistral:7b"
 OLLAMA_MODEL = "phi3"
 OLLAMA_API_SERVER = "http://localhost:11434/v1"
 # OLLAMA_SECRET_PROMPT = '''You are a Python requirements generator.
 # You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
 # The raw text sent by the user consists of a combination of the README file contents and the source code contents.
 # You generate only the file contents as answer.
@@ -207,15 +219,15 @@
 Only return the list of requirements. No other text like the filename at the top of the response or symbols are allowed."""
 
 REWRITE_README_PROMPT = """You are a specialist in understanding and explaining source code. 
 You are also a specialist in writing clear documentation (e.g README files) that helps people to understand the source code.
 Your task is to take a text input containing the current README and the code and use it to write an updated version of the README file.
 The README file should highlight the actual requirements that need to be installed."""
 
-#GROQ_MODEL = "mixtral-8x7b-32768"
+# GROQ_MODEL = "mixtral-8x7b-32768"
 GROQ_MODEL = "llama3-70b-8192"
 GROQ_SECRET_PROMPT = """You are a Python requirements generator.
 You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
 The raw text sent by the user consists of a combination of the README file contents and the source code contents.
 If the text sent by the user is invalid or is empty, just generate an empty content.
 You should ignore the Python version 2 or 3.
 The python package should not be included in the requirements file.
```

### Comparing `miniogre-0.6.0/miniogre/main.py` & `miniogre-0.7.0/miniogre/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,18 @@
 
     display_figlet()
     starting_emoji()
 
     ogre_dir_path = config_ogre_dir(
         os.path.join(project_path, os.getenv("OGRE_DIR", OGRE_DIR))
     )
+
     context_contents = run_gptify(os.getcwd())
+    num_tokens = count_tokens(context_contents)
+    print("Total number of tokens: {}".format(num_tokens))
     new_readme = rewrite_readme(provider, context_contents)
     readme_path = save_readme(new_readme, ogre_dir_path)
     end_emoji()
 
     return 0
```

### Comparing `miniogre-0.6.0/pyproject.toml` & `miniogre-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "miniogre"
-version = "0.6.0"
+version = "0.7.0"
 description = "miniogre: from source code to reproducible environment, in seconds."
 readme = "README.md"
 authors = ["Wilder Lopes <wilder@ogre.run>"]
-include = [".env"]
+include = [
+    { path = "miniogre/encodings", format = ["sdist", "wheel"] }
+]
 homepage = "https://github.com/ogre-run/miniogre"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 typer = "0.9.0"
 docker = "^5.0.0"
 python-dotenv = "^0.19.0"
@@ -19,15 +21,17 @@
 groq = "0.5.0"
 yaspin = "^3.0.1"
 octoai-sdk = "^0.9.0"
 mistralai = "^0.1.3"
 autopep8 = "^2.0.4"
 cyclonedx-py = "^1.0.1"
 pip-licenses = "^4.3.4"
-gptify = "0.3.2"
+gptify = "^0.3.4"
+tiktoken = "0.6.0"
+google-generativeai = "0.5.2"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `miniogre-0.6.0/PKG-INFO` & `miniogre-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: miniogre
-Version: 0.6.0
+Version: 0.7.0
 Summary: miniogre: from source code to reproducible environment, in seconds.
 Home-page: https://github.com/ogre-run/miniogre
 Author: Wilder Lopes
 Author-email: wilder@ogre.run
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: autopep8 (>=2.0.4,<3.0.0)
 Requires-Dist: cyclonedx-py (>=1.0.1,<2.0.0)
 Requires-Dist: docker (>=5.0.0,<6.0.0)
 Requires-Dist: emoji (>=2.10.1,<3.0.0)
-Requires-Dist: gptify (==0.3.2)
+Requires-Dist: google-generativeai (==0.5.2)
+Requires-Dist: gptify (>=0.3.4,<0.4.0)
 Requires-Dist: groq (==0.5.0)
 Requires-Dist: mistralai (>=0.1.3,<0.2.0)
 Requires-Dist: octoai-sdk (>=0.9.0,<0.10.0)
 Requires-Dist: openai (==1.21.2)
 Requires-Dist: pip-licenses (>=4.3.4,<5.0.0)
 Requires-Dist: pyfiglet (>=1.0.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: tiktoken (==0.6.0)
 Requires-Dist: typer (==0.9.0)
 Requires-Dist: yaspin (>=3.0.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # miniogre
 
 **miniogre** automates the management of software dependencies with AI, to ensure your Python code runs on any computer. It is a command-line application that analyzes a Python codebase to automatically generate a Dockerfile, requirements.txt file, and SBOM files, expediting the process of packaging any Python application. Additionally, it is able to update the README (documentation) file to comply with what really happens in the source code.
```

