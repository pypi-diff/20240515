# Comparing `tmp/dailalib-2.3.2.tar.gz` & `tmp/dailalib-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dailalib-2.3.2.tar", last modified: Tue Apr  2 03:55:05 2024, max compression
+gzip compressed data, was "dailalib-2.4.0.tar", last modified: Wed May 15 19:39:59 2024, max compression
```

## Comparing `dailalib-2.3.2.tar` & `dailalib-2.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-02 03:55:05.045104 dailalib-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-02 03:55:01.000000 dailalib-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib/
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib/api/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/ai_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib/api/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/openai/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/api/openai/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib/binsync_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/ai_bs_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/ai_user_config_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/openai_bs_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/binsync_plugin/varmodel_bs_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/daila_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-02 03:55:01.000000 dailalib-2.3.2/dailalib/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:55:05.045104 dailalib-2.3.2/dailalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 03:55:05.000000 dailalib-2.3.2/dailalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 03:55:05.049104 dailalib-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:55:01.000000 dailalib-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:59.220367 dailalib-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-15 19:39:59.220367 dailalib-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-15 19:39:52.000000 dailalib-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:59.216367 dailalib-2.4.0/dailalib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:59.216367 dailalib-2.4.0/dailalib/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/api/ai_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:59.216367 dailalib-2.4.0/dailalib/api/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/api/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/api/openai/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/api/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/api/openai/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:59.220367 dailalib-2.4.0/dailalib/binsync_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/binsync_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/binsync_plugin/ai_bs_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/binsync_plugin/ai_user_config_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/binsync_plugin/openai_bs_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/binsync_plugin/varmodel_bs_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/daila_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-15 19:39:52.000000 dailalib-2.4.0/dailalib/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:59.220367 dailalib-2.4.0/dailalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-15 19:39:59.000000 dailalib-2.4.0/dailalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-15 19:39:59.000000 dailalib-2.4.0/dailalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:39:59.000000 dailalib-2.4.0/dailalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 19:39:59.000000 dailalib-2.4.0/dailalib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 19:39:59.000000 dailalib-2.4.0/dailalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:39:59.000000 dailalib-2.4.0/dailalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-15 19:39:59.220367 dailalib-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:39:52.000000 dailalib-2.4.0/setup.py
```

### Comparing `dailalib-2.3.2/PKG-INFO` & `dailalib-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailalib
-Version: 2.3.2
+Version: 2.4.0
 Summary: The Decompiler Artificial Intelligence Language Assistant (DAILA) is a tool for adding AI to decompilers.
 Home-page: https://github.com/mahaloz/DAILA
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
```

### Comparing `dailalib-2.3.2/README.md` & `dailalib-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/__init__.py` & `dailalib-2.4.0/dailalib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.3.2"
+__version__ = "2.4.0"
 
 from .api import AIAPI, OpenAIAPI
 from libbs.api import DecompilerInterface
 
 
 def create_plugin(*args, **kwargs):
```

### Comparing `dailalib-2.3.2/dailalib/__main__.py` & `dailalib-2.4.0/dailalib/__main__.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/api/ai_api.py` & `dailalib-2.4.0/dailalib/api/ai_api.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/api/openai/openai_api.py` & `dailalib-2.4.0/dailalib/api/openai/openai_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from dailalib.api.ai_api import AIAPI
 if typing.TYPE_CHECKING:
     from dailalib.api.openai.prompt import Prompt
 
 
 class OpenAIAPI(AIAPI):
     prompts_by_name = []
-    DEFAULT_MODEL = "gpt-4"
+    DEFAULT_MODEL = "gpt-4o"
     MODEL_TO_TOKENS = {
+        "gpt-4o": 8000,
         "gpt-4": 8000,
         "gpt-3.5-turbo": 4096
     }
 
     # replacement strings for API calls
     def __init__(self, api_key: Optional[str] = None, model: str = DEFAULT_MODEL, prompts: Optional[list] = None, **kwargs):
         super().__init__(**kwargs)
@@ -78,15 +79,15 @@
         except (KeyError, IndexError) as e:
             answer = None
 
         return answer
 
     @staticmethod
     def estimate_token_amount(content: str, model=DEFAULT_MODEL):
-        enc = tiktoken.encoding_for_model(model)
+        enc = tiktoken.encoding_for_model("gpt-4" if model.startswith("gpt-4") else model)
         tokens = enc.encode(content)
         return len(tokens)
 
     @staticmethod
     def content_fits_tokens(content: str, model=DEFAULT_MODEL):
         max_token_count = OpenAIAPI.MODEL_TO_TOKENS[model]
         token_count = OpenAIAPI.estimate_token_amount(content, model=model)
```

### Comparing `dailalib-2.3.2/dailalib/api/openai/prompt.py` & `dailalib-2.4.0/dailalib/api/openai/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,11 +74,11 @@
                     response = {}
             else:
                 response += self._posttext_response if self._pretext_response else ""
 
             if ai_api.has_decompiler_gui and response:
                 self._gui_result_callback(response, function, ai_api)
 
-            ai_api.info(f"Reponse recieved...")
+            ai_api.info(f"Response recieved...")
             return response
         return _query_model(ai_api=self.ai_api, function=function, dec_text=dec_text, use_dec=use_dec)
```

### Comparing `dailalib-2.3.2/dailalib/api/openai/prompts.py` & `dailalib-2.4.0/dailalib/api/openai/prompts.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ai_api._dec_interface.comments[function.addr] = Comment(function.addr, comment=result, func_addr=function.addr)
 
 
 PROMPTS = [
     Prompt(
         "summarize",
         f'''
-        You are C expert that summarizes code. When given code, you summarize at a high level what the function does 
+        You are decompiled C expert that summarizes code. When given code, you summarize at a high level what the function does 
         and you identify if known algorithms are used in the function. As an example:
         """
         int sub_404000(int a0, char** a1) 
         {{
             int v1; // rax 
             v1 = sub_404100(a0[1]) % 2 == 0 
             return v1;
@@ -39,23 +39,22 @@
 
         You responded with:
         This function takes two arguments and implements the is_even check on second argument
 
         Here is another example:
         {Prompt.DECOMP_TEXT}
 
-        You responded with:
         ''',
         desc="Summarize the function",
         gui_result_callback=comment_function
     ),
     Prompt(
         "identify_source",
         f'''
-        You are a C expert that identifies the original source given decompilation. Upon discovering the source,
+        You are a decompiled C expert that identifies the original source given decompilation. Upon discovering the source,
         you give a link to the code. You only respond with a json. As an example:
         """
         void __fastcall __noreturn usage(int status)
         {{
             v2 = program_name;
             if ( status )
             {{
@@ -79,15 +78,15 @@
         desc="Identify the original source",
         json_response=True,
         gui_result_callback=comment_function
     ),
     Prompt(
         "rename_variables",
         f'''
-        You are C expert that renames variables in code. When given code, you rename variables according to the
+        You are decompiled C expert that renames variables in code. When given code, you rename variables according to the
         meaning of the function or its use. You only respond with a json. As an example:
 
         int sub_404000(int a0, char** a1) 
         {{
             int v1; // rax 
             v1 = sub_404100(a0[1]) % 2 == 0 
             return v1;
@@ -104,15 +103,15 @@
         desc="Suggest variable names",
         json_response=True,
         gui_result_callback=rename_variables,
     ),
     Prompt(
         "rename_function",
         f'''
-        You are C expert that renames functions. When given a function, you rename it according to the
+        You are decompiled C expert that renames functions. When given a function, you rename it according to the
         meaning of the function or its use. You only respond with a json. As an example:
 
         int sub_404000(int a0, char** a1) 
         {{
             int is_even; // rax 
             is_even = sub_404100(a0[1]) % 2 == 0 
             return is_even;
```

### Comparing `dailalib-2.3.2/dailalib/binsync_plugin/__init__.py` & `dailalib-2.4.0/dailalib/binsync_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/binsync_plugin/ai_bs_user.py` & `dailalib-2.4.0/dailalib/binsync_plugin/ai_bs_user.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/binsync_plugin/ai_user_config_ui.py` & `dailalib-2.4.0/dailalib/binsync_plugin/ai_user_config_ui.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/binsync_plugin/openai_bs_user.py` & `dailalib-2.4.0/dailalib/binsync_plugin/openai_bs_user.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/binsync_plugin/varmodel_bs_user.py` & `dailalib-2.4.0/dailalib/binsync_plugin/varmodel_bs_user.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/daila_plugin.py` & `dailalib-2.4.0/dailalib/daila_plugin.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib/installer.py` & `dailalib-2.4.0/dailalib/installer.py`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/dailalib.egg-info/PKG-INFO` & `dailalib-2.4.0/dailalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailalib
-Version: 2.3.2
+Version: 2.4.0
 Summary: The Decompiler Artificial Intelligence Language Assistant (DAILA) is a tool for adding AI to decompilers.
 Home-page: https://github.com/mahaloz/DAILA
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
```

### Comparing `dailalib-2.3.2/dailalib.egg-info/SOURCES.txt` & `dailalib-2.4.0/dailalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dailalib-2.3.2/setup.cfg` & `dailalib-2.4.0/setup.cfg`

 * *Files identical despite different names*

