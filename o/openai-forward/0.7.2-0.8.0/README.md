# Comparing `tmp/openai_forward-0.7.2.tar.gz` & `tmp/openai_forward-0.8.0.tar.gz`

## Comparing `openai_forward-0.7.2.tar` & `openai_forward-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/__init__.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/__main__.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/app.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/console.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/custom_slowapi.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/decorators.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/helper.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/settings.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/database.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/chat/__init__.py
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/chat/chat_completions.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/chat/response.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/chat/tokenizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/embedding/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/embedding/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/content/config.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/content/helper.py
--rw-r--r--   0        0        0    14539 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/content/openai.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/forward/__init__.py
--rw-r--r--   0        0        0    21936 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/forward/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/chat.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/helper.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/interface.py
--rw-r--r--   0        0        0    14976 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/run.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 openai_forward-0.7.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.7.2/LICENSE
--rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 openai_forward-0.7.2/README.md
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 openai_forward-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    13036 2020-02-02 00:00:00.000000 openai_forward-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/__init__.py
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/__main__.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/app.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/console.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/custom_slowapi.py
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/decorators.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/helper.py
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/settings.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/cache/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/cache/database.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/cache/chat/__init__.py
+-rw-r--r--   0        0        0    11425 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/cache/chat/chat_completions.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/cache/chat/response.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/cache/chat/tokenizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/cache/embedding/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/cache/embedding/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/config/__init__.py
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/config/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/content/config.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/content/helper.py
+-rw-r--r--   0        0        0    14596 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/content/openai.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/forward/__init__.py
+-rw-r--r--   0        0        0    22912 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/forward/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/webui/__init__.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/webui/chat.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/webui/helper.py
+-rw-r--r--   0        0        0    15486 2020-02-02 00:00:00.000000 openai_forward-0.8.0/openai_forward/webui/run.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 openai_forward-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.8.0/LICENSE
+-rw-r--r--   0        0        0    10406 2020-02-02 00:00:00.000000 openai_forward-0.8.0/README.md
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 openai_forward-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 openai_forward-0.8.0/PKG-INFO
```

### Comparing `openai_forward-0.7.2/openai_forward/__main__.py` & `openai_forward-0.8.0/openai_forward/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,23 +62,23 @@
                 ssl_certfile=ssl_certfile,
             )
         else:
             import threading
 
             import zmq
 
-            mq_port = 15555
-
             os.environ['OPENAI_FORWARD_WEBUI'] = 'true'
 
             context = zmq.Context()
             socket = context.socket(zmq.REP)
-            socket.bind(f"tcp://*:{mq_port}")
+            restart_port = int(os.environ.get('WEBUI_RESTART_PORT', 15555))
+            socket.bind(f"tcp://*:{restart_port}")
             log_socket = context.socket(zmq.ROUTER)
-            log_socket.bind(f"tcp://*:{15556}")
+            log_port = int(os.environ.get("WEBUI_LOG_PORT", 15556))
+            log_socket.bind(f"tcp://*:{log_port}")
             subscriber_info = {}
 
             def mq_worker(log_socket: zmq.Socket):
 
                 while True:
                     identity, uid, message = log_socket.recv_multipart()
                     if uid == b"/subscribe":
@@ -223,14 +223,33 @@
                 convert_folder_to_jsonl(log_folder, target_path)
                 print(60 * '-')
         else:
             print(f"Convert {log_folder}/*.log to {target_path}")
             convert_folder_to_jsonl(log_folder, target_path)
             print(60 * '-')
 
+    @staticmethod
+    def gen_config(dir: str = "."):
+        """
+        Generates a .env file in the specified directory.
+        """
+        from pathlib import Path
+
+        from openai_forward.config.interface import Config
+
+        config = Config()
+        env_dict = config.convert_to_env(set_env=False)
+        dir = Path(dir)
+
+        with open(dir / ".env", "w") as f:
+            env_content = "\n".join(
+                [f"{key}={value}" for key, value in env_dict.items()]
+            )
+            f.write(env_content)
+
 
 def main():
     fire.Fire(Cli)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `openai_forward-0.7.2/openai_forward/app.py` & `openai_forward-0.8.0/openai_forward/app.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/console.py` & `openai_forward-0.8.0/openai_forward/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from rich import print
 from rich.panel import Panel
 from rich.table import Table
 
 from . import __version__
```

### Comparing `openai_forward-0.7.2/openai_forward/custom_slowapi.py` & `openai_forward-0.8.0/openai_forward/custom_slowapi.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/decorators.py` & `openai_forward-0.8.0/openai_forward/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -165,14 +165,67 @@
                 yield value
 
         return wrapper
 
     return decorator
 
 
+def async_token_rate_limit_auth_level(token_rate_limit: dict, key_level_map: dict):
+    """
+    A decorator for rate-limiting requests based on tokens. It limits the rate at which tokens can be consumed
+    for a particular route path.
+
+    Args:
+        token_rate_limit (dict): A dictionary mapping route paths to their respective token intervals (in seconds).
+
+    Yields:
+        value: The value from the wrapped asynchronous generator.
+
+    Note:
+        The 'request' object should be passed either as a keyword argument or as a positional argument to the
+        decorated function.
+    """
+
+    def decorator(async_gen_func):
+        @wraps(async_gen_func)
+        async def wrapper(*args, **kwargs):
+            request: Request = kwargs.get('request')
+            if not request:
+                # Try to find the request argument by position
+                func_argspec = inspect.getfullargspec(async_gen_func)
+                request_index = func_argspec.args.index('request')
+                request = args[request_index]
+
+            route_path = f"{request.scope.get('root_path')}{request.scope.get('path')}"
+            fk_or_sk = request.headers.get("Authorization", "default")
+            level = key_level_map.get(fk_or_sk, 0)
+            default_interval = 0
+            token_level_dict = token_rate_limit.get(
+                route_path, {level: default_interval}
+            )
+            token_interval = token_level_dict[level]
+
+            async_gen = async_gen_func(*args, **kwargs)
+
+            start_time = time.perf_counter()
+            async for value in async_gen:
+                if token_interval > 0:
+                    current_time = time.perf_counter()
+                    delta = current_time - start_time
+                    delay = token_interval - delta
+                    if delay > 0:
+                        await asyncio.sleep(delay)
+                    start_time = time.perf_counter()
+                yield value
+
+        return wrapper
+
+    return decorator
+
+
 def async_random_sleep(min_time=0, max_time=1):
     """
     Decorator that adds a random sleep time between min_time and max_time.
 
     Args:
         min_time (float, optional): The minimum sleep time in seconds.
         max_time (float, optional): The maximum sleep time in seconds.
@@ -186,7 +239,30 @@
             sleep_time = random.uniform(min_time, max_time)
             await asyncio.sleep(sleep_time)
             return await func(*args, **kwargs)
 
         return wrapper
 
     return decorator
+
+
+def random_sleep(min_time=0, max_time=1):
+    """
+    Decorator that adds a random sleep time between min_time and max_time.
+
+    Args:
+        min_time (float, optional): The minimum sleep time in seconds.
+        max_time (float, optional): The maximum sleep time in seconds.
+    """
+
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            if max_time == 0:
+                return func(*args, **kwargs)
+            sleep_time = random.uniform(min_time, max_time)
+            time.sleep(sleep_time)
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
```

### Comparing `openai_forward-0.7.2/openai_forward/helper.py` & `openai_forward-0.8.0/openai_forward/helper.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/settings.py` & `openai_forward-0.8.0/openai_forward/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,28 @@
 from .content.config import setting_log
 from .helper import env2dict, env2list, format_route_prefix, get_client_ip
 
 openai_additional_start_info = {}
 general_additional_start_info = {}
 
 TIMEOUT = float(os.environ.get("TIMEOUT", "").strip() or "10")
+DEFAULT_STREAM_RESPONSE = (
+    os.environ.get("DEFAULT_STREAM_RESPONSE", "True").strip().lower() == "true"
+)
 
 ITER_CHUNK_TYPE = (
     os.environ.get("ITER_CHUNK_TYPE", "").strip() or "efficiency"
 )  # Options: efficiency, one-by-one
 
-CHAT_COMPLETION_ROUTE = "/v1/chat/completions"
-COMPLETION_ROUTE = "/v1/completions"
-EMBEDDING_ROUTE = "/v1/embeddings"
-
+CHAT_COMPLETION_ROUTE = (
+    os.environ.get("CHAT_COMPLETION_ROUTE", "/v1/chat/completions").strip().lower()
+)
+COMPLETION_ROUTE = os.environ.get("COMPLETION_ROUTE", "/v1/completions").strip().lower()
+EMBEDDING_ROUTE = os.environ.get("EMBEDDING_ROUTE", "/v1/embeddings").strip().lower()
+CUSTOM_GENERAL_ROUTE = os.environ.get("CUSTOM_GENERAL_ROUTE", "").strip().lower()
 
 CACHE_ROUTE_SET = set(env2dict("CACHE_ROUTES", []))
 
 openai_additional_start_info['cache_routes'] = CACHE_ROUTE_SET
 general_additional_start_info['cache_routes'] = CACHE_ROUTE_SET
 
 FORWARD_CONFIG = env2dict(
@@ -129,22 +134,29 @@
     os.environ.get("RATE_LIMIT_STRATEGY", "fixed-window").strip() or "fixed-window"
 )
 req_rate_limit_dict = env2dict('REQ_RATE_LIMIT')
 
 
 def get_limiter_key(request: Request):
     limiter_prefix = f"{request.scope.get('root_path')}{request.scope.get('path')}"
-    key = f"{limiter_prefix}-{get_client_ip(request)}"
+    fk_or_sk = request.headers.get("Authorization", "default")
+    key = f"{limiter_prefix},{fk_or_sk}"
     return key
 
 
 def dynamic_request_rate_limit(key: str):
+    limite_prefix, fk_or_sk = key.split(',')
+    key_level = FWD_KEY.get(fk_or_sk, 0)
     for route in req_rate_limit_dict:
         if key.startswith(route):
-            return req_rate_limit_dict[route]
+            for level_dict in req_rate_limit_dict[route]:
+                if level_dict['level'] == key_level:
+                    return level_dict['limit']
+
+            break
     return GLOBAL_RATE_LIMIT
 
 
 def cvt_token_rate_to_interval(token_rate_limit: str):
     if token_rate_limit:
         rate_limit_item = limits.parse(token_rate_limit)
         token_interval = (
@@ -153,16 +165,20 @@
     else:
         token_interval = 0
     return token_interval
 
 
 token_rate_limit_conf = env2dict("TOKEN_RATE_LIMIT")
 token_interval_conf = {}
-for route, rate_limit in token_rate_limit_conf.items():
-    token_interval_conf[route] = cvt_token_rate_to_interval(rate_limit)
+for route, rate_limit_list in token_rate_limit_conf.items():
+    token_interval_conf.setdefault(route, {})
+    for level_dict in rate_limit_list:
+        token_interval_conf[route][level_dict['level']] = cvt_token_rate_to_interval(
+            level_dict['limit']
+        )
 
 styles = itertools.cycle(
     ["#7CD9FF", "#BDADFF", "#9EFFE3", "#f1b8e4", "#F5A88E", "#BBCA89"]
 )
 
 
 def show_startup():
```

### Comparing `openai_forward-0.7.2/openai_forward/cache/__init__.py` & `openai_forward-0.8.0/openai_forward/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/cache/database.py` & `openai_forward-0.8.0/openai_forward/cache/database.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/cache/chat/chat_completions.py` & `openai_forward-0.8.0/openai_forward/cache/chat/chat_completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 from typing import List, Literal, Optional, Union
 
 import attrs
 import orjson
 from fastapi import Request
 from fastapi.responses import Response, StreamingResponse
 
-from ...decorators import async_random_sleep, async_token_rate_limit
+from ...decorators import (
+    async_random_sleep,
+    async_token_rate_limit_auth_level,
+    random_sleep,
+)
 from ...helper import get_unique_id
-from ...settings import token_interval_conf
+from ...settings import FWD_KEY, token_interval_conf
 from .tokenizer import TIKTOKEN_VALID, count_tokens, encode_as_pieces
 
 
 @attrs.define(slots=True)
 class ChatMessage:
     role: Literal["user", "assistant", "system"]
     content: Optional[str] = None
@@ -114,15 +118,15 @@
 "He is so close to her that he can even hear each of her breaths and smell the fragrance that emanates from her. For the remaining years of his life, it is this fragrance by which he identifies her."
  """,
 ]
 
 sentences = cycle(corpus)
 
 
-@async_token_rate_limit(token_interval_conf)
+@async_token_rate_limit_auth_level(token_interval_conf, FWD_KEY)
 async def stream_generate(
     model: str, content: str | None, tool_calls: list | None, request: Request
 ):
     created = int(time.time())
     id = f"chatcmpl-{get_unique_id()}"
 
     if tool_calls:
@@ -202,15 +206,15 @@
 
     delta = DeltaMessage()
     yield serialize_delta(finish_reason="tool_calls" if tool_calls else "stop")
 
     yield b'data: [DONE]\n\n'
 
 
-@async_token_rate_limit(token_interval_conf)
+@async_token_rate_limit_auth_level(token_interval_conf, FWD_KEY)
 async def stream_generate_efficient(
     model: str, content: str | None, tool_calls: list | None, request: Request
 ):
     """More efficient (use dict) version of stream_generate
     Args:
         model (str): The model to use.
         content (str): content.
@@ -288,14 +292,15 @@
 
     delta = {}
     yield serialize_delta(finish_reason="tool_calls" if tool_calls else "stop")
 
     yield b'data: [DONE]\n\n'
 
 
+@random_sleep(min_time=1, max_time=2)
 def generate(model: str, content: str | None, tool_calls: list | None, usage: dict):
     created = int(time.time())
     id = f"chatcmpl-{get_unique_id()}"
 
     choice_data = ChatCompletionChoice(
         index=0,
         message=ChatCompletionMessage(
@@ -332,15 +337,14 @@
         usage = count_tokens(messages, sentence, 'gpt-3.5-turbo')
     else:
         usage = {"prompt_tokens": 0, "completion_tokens": 0, "total_tokens": 0}
 
     return ModelInferResult(content=sentence, usage=usage)
 
 
-@async_random_sleep(min_time=0, max_time=1)
 async def chat_completions_benchmark(request: Request):
     payload = await request.json()
     model = payload.get("model", 'robot')
     stream = payload.get("stream", False)
     messages = payload.get("messages", [])
 
     model_result = model_inference(model, messages)
```

### Comparing `openai_forward-0.7.2/openai_forward/cache/chat/response.py` & `openai_forward-0.8.0/openai_forward/cache/chat/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import random
 from typing import List
 
 from fastapi.responses import Response, StreamingResponse
 from flaxkv.pack import encode
 from loguru import logger
 
-from ...settings import CACHE_OPENAI
+from ...settings import CACHE_OPENAI, FWD_KEY
 from ..database import db_dict
 from .chat_completions import (
-    async_token_rate_limit,
+    async_token_rate_limit_auth_level,
     generate,
     stream_generate_efficient,
     token_interval_conf,
 )
 
 
 def construct_cache_key(payload_info: dict):
@@ -112,15 +112,15 @@
             get_response_from_key(cache_key, payload_info, request, **kwargs),
             cache_key,
         )
 
     return None, cache_key
 
 
-@async_token_rate_limit(token_interval_conf)
+@async_token_rate_limit_auth_level(token_interval_conf, FWD_KEY)
 async def stream_generate(buffer_list: List, request):
     for buffer in buffer_list:
         yield buffer
 
 
 def gen_response(buffer_list, request):
     if len(buffer_list) > 1:
```

### Comparing `openai_forward-0.7.2/openai_forward/cache/chat/tokenizer.py` & `openai_forward-0.8.0/openai_forward/cache/chat/tokenizer.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/cache/embedding/response.py` & `openai_forward-0.8.0/openai_forward/cache/embedding/response.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/content/config.py` & `openai_forward-0.8.0/openai_forward/content/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/content/helper.py` & `openai_forward-0.8.0/openai_forward/content/helper.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/content/openai.py` & `openai_forward-0.8.0/openai_forward/content/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
             self.webui = True
 
             import zmq
             from flaxkv.helper import SimpleQueue
 
             context = zmq.Context()
             socket = context.socket(zmq.DEALER)
-            socket.connect("tcp://localhost:15556")
+            webui_log_port = int(os.environ.get("WEBUI_LOG_PORT", 15556))
+            socket.connect(f"tcp://localhost:{webui_log_port}")
 
             self.q = SimpleQueue(maxsize=200)
 
             def _worker():
                 while True:
                     message: dict = self.q.get(block=True)
                     if message.get("payload"):
@@ -73,15 +74,14 @@
         """
         super().__init__(route_prefix, "_completion")
 
     @staticmethod
     def parse_payload(request: Request, raw_payload):
         uid = get_unique_id()
         payload = orjson.loads(raw_payload)
-        print(f"{payload=}")
 
         content = {
             "prompt": payload['prompt'],
             "model": payload['model'],
             "stream": payload.get("stream", True),
             "temperature": payload.get("temperature", 1),
             "ip": get_client_ip(request) or "",
```

### Comparing `openai_forward-0.7.2/openai_forward/forward/__init__.py` & `openai_forward-0.8.0/openai_forward/forward/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/openai_forward/forward/core.py` & `openai_forward-0.8.0/openai_forward/forward/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,42 +21,102 @@
 )
 from ..content.openai import (
     ChatLogger,
     CompletionLogger,
     EmbeddingLogger,
     WhisperLogger,
 )
-from ..decorators import async_retry, async_token_rate_limit
-from ..helper import InfiniteSet
+from ..decorators import async_retry, async_token_rate_limit_auth_level
+from ..helper import InfiniteSet, get_client_ip, get_unique_id
 from ..settings import *
 
 # from beartype import beartype
 
 
 class GenericForward:
     """
     Base class for handling request forwarding to another service.
     Provides methods for request validation, logging, and proxying.
     """
 
     validate_host = bool(IP_BLACKLIST or IP_WHITELIST)
     timeout = aiohttp.ClientTimeout(connect=TIMEOUT)
 
+    _fk_to_level = FWD_KEY
+    _sk_to_levels = OPENAI_API_KEY
+    _level_to_model_set = {level: set(models) for level, models in LEVEL_MODELS.items()}
+
+    _zero_level_model_set = InfiniteSet()
+
+    _level_to_sks = {}
+    for sk, levels in _sk_to_levels.items():
+        for level in levels:
+            _level_to_sks[level] = _level_to_sks.get(level, []) + [sk]
+
+    _level_to_sk = {}
+    for level, sks in _level_to_sks.items():
+        _level_to_sk[level] = cycle(sks)
+
     def __init__(self, base_url: str, route_prefix: str, proxy=None):
         """
         Args:
             base_url (str): The base URL to which requests will be forwarded.
             route_prefix (str): The prefix of the route.
             proxy (str, optional): The proxy to use for the requests. Defaults to None.
         """
         self.BASE_URL = base_url
         self.PROXY = proxy
         self.ROUTE_PREFIX = route_prefix
         self.client: aiohttp.ClientSession | None = None
 
+    @classmethod
+    def fk_to_sk(cls, forward_key: str):
+        """
+        Convert a forward key to a secret key.
+
+        Args:
+            forward_key (str): The forward key to convert.
+
+        Returns:
+            str: The corresponding secret key, if it exists. Otherwise, None.
+        """
+        level = cls._fk_to_level.get(forward_key)
+        if level is not None:
+            sk = cls._level_to_sk.get(level)
+            if sk:
+                return next(sk), level
+        return None, level
+
+    @classmethod
+    def handle_authorization(cls, client_config):
+        """
+        Handle the authorization for the client.
+
+        Args:
+            client_config (dict): The configuration for the client.
+
+        Returns:
+            str: The authorization string.
+            set: The set of models can be accessed.
+        """
+        auth, auth_prefix = client_config["auth"], "Bearer "
+        model_set = cls._zero_level_model_set
+
+        if auth:
+            fk = auth[len(auth_prefix) :]
+            if fk in FWD_KEY:
+                sk, level = cls.fk_to_sk(fk)
+                assert level is not None
+                if level != 0:
+                    model_set = cls._level_to_model_set[level]
+                if sk:
+                    auth = auth_prefix + sk
+                    client_config["headers"]["Authorization"] = auth
+        return auth, model_set
+
     async def build_client(self):
         """
         Asynchronously build the client for making requests.
         """
         connector = TCPConnector(limit=500, limit_per_host=0, force_close=False)
         self.client = aiohttp.ClientSession(connector=connector, timeout=self.timeout)
 
@@ -80,15 +140,15 @@
             logger.warning(f"IP {ip} is unauthorized")
             raise HTTPException(
                 status_code=status.HTTP_403_FORBIDDEN,
                 detail=f"Forbidden Error",
             )
 
     @staticmethod
-    @async_token_rate_limit(token_interval_conf)
+    @async_token_rate_limit_auth_level(token_interval_conf, FWD_KEY)
     async def aiter_bytes(
         r: aiohttp.ClientResponse,
         request: Request,
         route_path: str,
         cache_key: str | None = None,
     ) -> AsyncGenerator[bytes, Any]:
         """
@@ -198,16 +258,16 @@
             request (Request): The original FastAPI request object.
             return_origin_header (bool, optional): Whether to return the original header. Defaults to False.
 
         Returns:
             dict: The configuration for the client.
         """
         assert self.BASE_URL and self.ROUTE_PREFIX
+        ip = get_client_ip(request)
         if self.validate_host:
-            ip = get_client_ip(request)
             self.validate_request_host(ip)
 
         _url_path = f"{request.scope.get('root_path')}{request.scope.get('path')}"
         route_path = (
             _url_path[len(self.ROUTE_PREFIX) :]
             if self.ROUTE_PREFIX != '/'
             else _url_path
@@ -244,17 +304,39 @@
                     headers[key] = value
 
         return {
             'auth': auth,
             'headers': headers,
             "method": request.method,
             'url': url,
+            'ip': ip,
             'route_path': route_path,
         }
 
+    async def _handle_payload(self, request: Request, route_path: str, model_set):
+
+        if not request.method == "POST":
+            return
+
+        if route_path in (
+            CHAT_COMPLETION_ROUTE,
+            COMPLETION_ROUTE,
+            EMBEDDING_ROUTE,
+            CUSTOM_GENERAL_ROUTE,
+        ):
+            payload = await request.json()
+            model = payload.get("model", None)
+
+            if model is not None and model not in model_set:
+                logger.warning(f"[Auth Warning] model: {model} is not allowed")
+                raise HTTPException(
+                    status_code=status.HTTP_403_FORBIDDEN,
+                    detail=f"model: {model} is not allowed",
+                )
+
     async def reverse_proxy(self, request: Request):
         """
         Asynchronously handle reverse proxying the incoming request.
 
         Args:
             request (Request): The incoming FastAPI request object.
 
@@ -263,17 +345,19 @@
         """
         assert self.client
         data = await request.body()
 
         if LOG_GENERAL:
             logger.debug(f"payload: {data}")
         client_config = self.prepare_client(request, return_origin_header=True)
-
         route_path = client_config["route_path"]
 
+        _, model_set = self.handle_authorization(client_config)
+        payload = await self._handle_payload(request, route_path, model_set)
+
         cached_response, cache_key = get_cached_generic_response(
             data, request, route_path
         )
 
         if cached_response:
             return cached_response
 
@@ -289,29 +373,14 @@
 
 class OpenaiForward(GenericForward):
     """
     Derived class for handling request forwarding specifically for the OpenAI (Style) API.
     Inherits from the GenericForward class and adds specific functionality for the OpenAI API.
     """
 
-    _fk_to_level = FWD_KEY
-    _sk_to_levels = OPENAI_API_KEY
-    _level_to_model_set = {level: set(models) for level, models in LEVEL_MODELS.items()}
-
-    _zero_level_model_set = InfiniteSet()
-
-    _level_to_sks = {}
-    for sk, levels in _sk_to_levels.items():
-        for level in levels:
-            _level_to_sks[level] = _level_to_sks.get(level, []) + [sk]
-
-    _level_to_sk = {}
-    for level, sks in _level_to_sks.items():
-        _level_to_sk[level] = cycle(sks)
-
     def __init__(self, base_url: str, route_prefix: str, proxy=None):
         """
         Initialize the OpenaiForward class.
 
         Args:
             base_url (str): The base URL to which requests will be forwarded.
             route_prefix (str): The prefix of the route.
@@ -320,32 +389,14 @@
         super().__init__(base_url, route_prefix, proxy)
         if LOG_OPENAI or PRINT_CHAT:
             self.chat_logger = ChatLogger(self.ROUTE_PREFIX)
             self.completion_logger = CompletionLogger(self.ROUTE_PREFIX)
             self.whisper_logger = WhisperLogger(self.ROUTE_PREFIX)
             self.embedding_logger = EmbeddingLogger(self.ROUTE_PREFIX)
 
-    @classmethod
-    def fk_to_sk(cls, forward_key: str):
-        """
-        Convert a forward key to a secret key.
-
-        Args:
-            forward_key (str): The forward key to convert.
-
-        Returns:
-            str: The corresponding secret key, if it exists. Otherwise, None.
-        """
-        level = cls._fk_to_level.get(forward_key)
-        if level is not None:
-            sk = cls._level_to_sk.get(level)
-            if sk:
-                return next(sk), level
-        return None, level
-
     def _handle_result(
         self, buffer: bytearray, uid: str, route_path: str, request_method: str
     ):
         """
         Logs the result of the API call.
 
         Args:
@@ -445,15 +496,14 @@
                 f"log chat error:\nhost:{request.client.host} method:{request.method}: {traceback.format_exc()}"
             )
 
         valid = True if payload_log_info['uid'] is not None else False
 
         if valid:
             if payload_log_info["model"] not in model_set:
-                print(f"{model_set=}")
                 logger.warning(
                     f"[Auth Warning] model: {payload_log_info['model']} is not allowed"
                 )
                 raise HTTPException(
                     status_code=status.HTTP_403_FORBIDDEN,
                     detail=f"model: {payload_log_info['model']} is not allowed",
                 )
@@ -483,15 +533,15 @@
         else:
             async for chunk, _ in r.content.iter_chunks():
                 buffer.extend(chunk)
                 await queue.put(chunk)
 
         await queue.put(buffer)  # add all information when the stream ends
 
-    @async_token_rate_limit(token_interval_conf)
+    @async_token_rate_limit_auth_level(token_interval_conf, FWD_KEY)
     async def aiter_bytes(
         self,
         r: aiohttp.ClientResponse,
         request: Request,
         route_path: str,
         uid: str,
         cache_key: str | None = None,
@@ -564,40 +614,14 @@
             elif chunk is not None:
                 logger.warning(
                     f'uid: {uid}\n status: {r.status}\n {chunk.decode("utf-8")}'
                 )
             else:
                 logger.warning(f'uid: {uid}\n' f'{r.status}')
 
-    def handle_authorization(self, client_config):
-        """
-        Handle the authorization for the client.
-
-        Args:
-            client_config (dict): The configuration for the client.
-
-        Returns:
-            str: The authorization string.
-            set: The set of models can be accessed.
-        """
-        auth, auth_prefix = client_config["auth"], "Bearer "
-        model_set = self._zero_level_model_set
-
-        if auth:
-            fk = auth[len(auth_prefix) :]
-            if fk in FWD_KEY:
-                sk, level = self.fk_to_sk(fk)
-                assert level is not None
-                if level != 0:
-                    model_set = self._level_to_model_set[level]
-                if sk:
-                    auth = auth_prefix + sk
-                    client_config["headers"]["Authorization"] = auth
-        return auth, model_set
-
     async def reverse_proxy(self, request: Request):
         """
         Asynchronously handles reverse proxying the incoming request.
 
         Args:
             request (Request): The incoming FastAPI request object.
 
@@ -608,15 +632,15 @@
         route_path = client_config["route_path"]
 
         _, model_set = self.handle_authorization(client_config)
         valid_payload, payload_info, payload = await self._handle_payload(
             request, route_path, model_set
         )
         uid = payload_info["uid"]
-        stream = payload_info.get('stream', None)
+        stream = payload_info.get('stream', DEFAULT_STREAM_RESPONSE)
 
         cached_response, cache_key = get_cached_response(
             payload,
             payload_info,
             valid_payload,
             route_path,
             request,
```

### Comparing `openai_forward-0.7.2/openai_forward/webui/chat.py` & `openai_forward-0.8.0/openai_forward/webui/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-from collections import deque
+from collections import OrderedDict, deque
 from typing import Callable, Dict
 
 import streamlit as st
 
 
-def render_chat_log_message(msg: Dict):
+def render_chat_log_message(msg: Dict, markdown=True):
     msg = msg.copy()
+    render = st.markdown if markdown else st.text
     if msg.get("user_role"):
-        with st.chat_message(name="human"):
-            messages = msg.pop('messages')
+        messages = msg.pop('messages')
+        with st.chat_message(name="user", avatar='🧑'):
             for msg_item in messages:
                 # https://github.com/streamlit/streamlit/issues/7978
-                # st.write(f"`{msg_item['role']}`: {msg_item['content']}")
-                st.text(f"`{msg_item['role']}`: {msg_item['content']}")
+                render(f"`{msg_item['role']}`: {msg_item['content']}")
             st.write(msg)
     elif msg.get("assistant_role"):
-        with st.chat_message(name="ai"):
+        with st.chat_message(name="assistant", avatar='🤖'):
             ass_content = msg.pop('assistant', None)
-            st.write(ass_content)
+            render(ass_content)
             st.write(msg)
     else:
         print(f"{msg=}")
 
 
 class ChatData:
-    def __init__(self, max_len: int, callback: Callable):
-        self.data = deque(maxlen=max_len)
-        self.callback = callback
-
-    def add_message(self, message):
-        self.data.append(message)
-        self.callback(message)
-
-    def render_all_messages(self):
-        for message in self.data:
-            self.callback(message)
+    def __init__(self, max_len: int):
+        self.data = OrderedDict()
+        self.max_len = max_len
+
+    def add_message(self, message, **callback_kwargs):
+        uid = message.pop('uid')
+        if message.get("user_role"):
+            self.data.setdefault(uid, {'user_role': message})
+        else:
+            msg_item = self.data.get(uid, {})
+            msg_item['assistant_role'] = message
+        if len(self.data) >= self.max_len:
+            self.data.popitem(last=False)
+        render_chat_log_message(message, **callback_kwargs)
+
+    def render_all_messages(self, **callback_kwargs):
+        for uid, msg in self.data.items():
+            message = msg.get("user_role")
+            if message:
+                render_chat_log_message(message, **callback_kwargs)
+            message = msg.get("assistant_role")
+            if message:
+                render_chat_log_message(message, **callback_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai_forward-0.7.2/openai_forward/webui/interface.py` & `openai_forward-0.8.0/openai_forward/config/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import json
 import os
 from typing import Dict, List, Literal, Optional, Tuple, Union
 
 from attrs import asdict, define, field, filters
 
-from openai_forward.settings import *
+from ..settings import *
 
 
 class Base:
     def to_dict(self, drop_none=True):
         if drop_none:
             return asdict(self, filter=filters.exclude(type(None)))
         return asdict(self)
 
+    def to_dict_str(self):
+        return {k: str(v) for k, v in self.to_dict(drop_none=True).items()}
+
 
 @define(slots=True)
 class ForwardItem(Base):
     base_url: str
     route: str
     type: Literal["openai", "general"] = field(default="general")
 
@@ -67,29 +70,41 @@
             os.environ.update(env_dict)
         return env_dict
 
 
 @define(slots=True)
 class RateLimitType(Base):
     route: str
-    value: str
+    value: List[Dict[str, str]]
 
 
 @define(slots=True)
 class RateLimit(Base):
     backend: str = ''
     global_rate_limit: str = 'inf'
     token_rate_limit: List[RateLimitType] = [
-        RateLimitType(route="/v1/chat/completions", value="60/second"),
-        RateLimitType(route="/v1/completions", value="60/second"),
+        RateLimitType(
+            route="/v1/chat/completions",
+            value=[{"level": '0', "rate_limit": "60/second"}],
+        ),
+        RateLimitType(
+            route="/v1/completions", value=[{"level": '0', "rate_limit": "60/second"}]
+        ),
     ]
     req_rate_limit: List[RateLimitType] = [
-        RateLimitType(route="/v1/chat/completions", value="100/2minutes"),
-        RateLimitType(route="/v1/completions", value="60/minute"),
-        RateLimitType(route="/v1/embeddings", value="100/2minutes"),
+        RateLimitType(
+            route="/v1/chat/completions",
+            value=[{"level": '0', "rate_limit": "100/2minutes"}],
+        ),
+        RateLimitType(
+            route="/v1/completions", value=[{"level": '0', "rate_limit": "60/minute"}]
+        ),
+        RateLimitType(
+            route="/v1/embeddings", value=[{"level": '0', "rate_limit": "100/2minutes"}]
+        ),
     ]
     iter_chunk: Literal['one-by-one', 'efficiency'] = 'one-by-one'
     strategy: Literal[
         'fixed_window', 'moving-window', 'fixed-window-elastic-expiry'
     ] = 'moving-window'
 
     def convert_to_env(self, set_env=False):
@@ -155,26 +170,33 @@
 
     log: Log = Log()
 
     timezone: str = 'Asia/Shanghai'
     timeout: int = 6
     benchmark_mode: bool = False
     proxy: str = ''
+    webui_restart_port: int = 15555
+    webui_log_port: int = 15556
+    default_stream_response: bool = True
 
     def convert_to_env(self, set_env=False):
         env_dict = {}
         env_dict.update(self.forward.convert_to_env())
         env_dict.update(self.api_key.convert_to_env())
         env_dict.update(self.cache.convert_to_env())
         env_dict.update(self.rate_limit.convert_to_env())
         env_dict.update(self.log.convert_to_env())
 
         env_dict['TZ'] = self.timezone
         env_dict['TIMEOUT'] = str(self.timeout)
         env_dict['BENCHMARK_MODE'] = str(self.benchmark_mode)
+        env_dict['WEBUI_RESTART_PORT'] = str(self.webui_restart_port)
+        env_dict['WEBUI_LOG_PORT'] = str(self.webui_log_port)
+        env_dict['DEFAULT_STREAM_RESPONSE'] = str(self.default_stream_response)
+
         if self.proxy:
             env_dict['PROXY'] = self.proxy
 
         if set_env:
             os.environ.update(env_dict)
         return env_dict
```

### Comparing `openai_forward-0.7.2/openai_forward/webui/run.py` & `openai_forward-0.8.0/openai_forward/webui/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import os
+import ast
 import pickle
 import threading
-import time
 
 import orjson
 import pandas as pd
 import streamlit as st
 import zmq
 from flaxkv.helper import SimpleQueue
 
-from openai_forward.webui.chat import ChatData, render_chat_log_message
+from openai_forward.config.interface import *
+from openai_forward.webui.chat import ChatData
 from openai_forward.webui.helper import mermaid
-from openai_forward.webui.interface import *
 
 st.set_page_config(
     page_title="Openai Forward ",
     page_icon="🚀",
     # layout="wide",
     initial_sidebar_state="expanded",
     menu_items={
@@ -28,30 +27,32 @@
 
 @st.cache_resource
 def get_global_vars():
     context = zmq.Context()
     socket = context.socket(zmq.REQ)
     # socket.setsockopt(zmq.CONNECT_TIMEOUT, 20000) # 20s
     openai_forward_host = os.environ.get("OPENAI_FORWARD_HOST", "localhost")
-    socket.connect(f"tcp://{openai_forward_host}:15555")
+    restart_port = int(os.environ.get('WEBUI_RESTART_PORT', 15555))
+    socket.connect(f"tcp://{openai_forward_host}:{restart_port}")
 
     log_socket = context.socket(zmq.DEALER)
-    log_socket.connect(f"tcp://{openai_forward_host}:15556")
+    webui_log_port = int(os.environ.get("WEBUI_LOG_PORT", 15556))
+    log_socket.connect(f"tcp://{openai_forward_host}:{webui_log_port}")
     log_socket.send_multipart([b"/subscribe", b"0"])
 
     def worker(log_socket: zmq.Socket, q: SimpleQueue):
         while True:
             message = log_socket.recv_multipart()
             uid, msg = message
             q.put((uid, msg))
 
     q = SimpleQueue(maxsize=100)
     threading.Thread(target=worker, args=(log_socket, q)).start()
     config = Config().come_from_env()
-    chat_data = ChatData(100, render_chat_log_message)
+    chat_data = ChatData(100)
     return {
         "socket": socket,
         "log_socket": log_socket,
         "q": q,
         "config": config,
         "chat_data": chat_data,
     }
@@ -151,15 +152,14 @@
                 if row["route"] is not None and row["base_url"] is not None
             ]
 
             print(forward_config.convert_to_env())
 
 
 def display_api_key_configuration():
-
     with st.expander("See explanation"):
         st.write(
             """
 > - 不同level对应不同权限，可以定义不同权限可以访问哪些模型。 例如, level为1，只可访问gpt-3.5-turbo；level为2，可访问embedding 和tts等等。(level为0，全权限，可访问任何模型，不可更改)
 > - 对于api key而言，level的意义是区分该api key自身是否有权限访问哪些模型。每个api key可对应多个level，因为这些level不必是从属关系。
 > - 对于forward key而言，每个key对应一个level，level表示它可以访问该level对应的所有api key。
 """
@@ -180,37 +180,46 @@
 fk(FK_x) --> level_n(Level n)
 level_n --> sk_n(SK_n)
 """
         )
 
     # check openai models:
     # from openai import OpenAI
-    # client = OpenAI(api_key=)
+    # from rich import print
+    # client = OpenAI(api_key="sk-")
     # openai_model_list = [i.id for i in client.models.list()]
     # openai_model_list.sort()
+    # print(openai_model_list)
+    # print(len(openai_model_list))
 
     openai_model_list = [
         'babbage-002',
         'dall-e-2',
         'dall-e-3',
         'davinci-002',
         'gpt-3.5-turbo',
+        'gpt-3.5-turbo-0125',
         'gpt-3.5-turbo-0301',
         'gpt-3.5-turbo-0613',
         'gpt-3.5-turbo-1106',
         'gpt-3.5-turbo-16k',
         'gpt-3.5-turbo-16k-0613',
         'gpt-3.5-turbo-instruct',
         'gpt-3.5-turbo-instruct-0914',
         'gpt-4',
         'gpt-4-0125-preview',
         'gpt-4-0613',
         'gpt-4-1106-preview',
+        'gpt-4-1106-vision-preview',
+        'gpt-4-turbo',
+        'gpt-4-turbo-2024-04-09',
         'gpt-4-turbo-preview',
         'gpt-4-vision-preview',
+        'gpt-4o',
+        'gpt-4o-2024-05-13',
         'text-embedding-3-large',
         'text-embedding-3-small',
         'text-embedding-ada-002',
         'tts-1',
         'tts-1-1106',
         'tts-1-hd',
         'tts-1-hd-1106',
@@ -350,46 +359,46 @@
                 'moving-window',
                 'fixed-window-elastic-expiry',
             ].index(rate_limit.strategy),
         )
 
         st.subheader("Token Rate Limit")
         token_rate_limit_df = pd.DataFrame(
-            [i.to_dict() for i in rate_limit.token_rate_limit]
+            [i.to_dict_str() for i in rate_limit.token_rate_limit]
         )
         edited_token_rate_limit_df = st.data_editor(
             token_rate_limit_df,
             num_rows="dynamic",
             key="editor_token_rate_limit",
             use_container_width=True,
         )
 
         st.subheader("Request Rate Limit")
         req_rate_limit_df = pd.DataFrame(
-            [i.to_dict() for i in rate_limit.req_rate_limit]
+            [i.to_dict_str() for i in rate_limit.req_rate_limit]
         )
         edited_req_rate_limit_df = st.data_editor(
             req_rate_limit_df,
             num_rows="dynamic",
             key="editor_req_rate_limit",
             use_container_width=True,
         )
 
         if st.form_submit_button("Save", use_container_width=True):
             rate_limit.global_rate_limit = global_rate_limit
             rate_limit.iter_chunk = iter_chunk
             rate_limit.strategy = strategy
 
             rate_limit.token_rate_limit = [
-                RateLimitType(row["route"], row["value"])
+                RateLimitType(row["route"], ast.literal_eval(row["value"]))
                 for _, row in edited_token_rate_limit_df.iterrows()
             ]
 
             rate_limit.req_rate_limit = [
-                RateLimitType(row["route"], row["value"])
+                RateLimitType(row["route"], ast.literal_eval(row["value"]))
                 for _, row in edited_req_rate_limit_df.iterrows()
             ]
 
             print(rate_limit.convert_to_env())
 
 
 def display_other_configuration():
@@ -428,30 +437,30 @@
 
 elif selected_section == "Other":
     display_other_configuration()
 
 elif selected_section == "Real-time Logs":
     st.write("### Real-time Logs")
     st.write("\n")
+    render_with_markdown = st.toggle("Using Markdown to render", value=True)
+    st.write("\n")
 
-    with st.container():
-
-        q = st.session_state['q']
-        chat_data: ChatData = st.session_state['chat_data']
-        chat_data.render_all_messages()
-        while True:
-            uid, msg = q.get()
-            uid: bytes
-            print(f"{uid=}")
-            item = orjson.loads(msg)
-            if uid.startswith(b"0"):
-                item['user_role'] = True
-            else:
-                item['assistant_role'] = True
+    q = st.session_state['q']
+    chat_data: ChatData = st.session_state['chat_data']
+    chat_data.render_all_messages(markdown=render_with_markdown)
+    while True:
+        uid, msg = q.get()
+        uid: bytes
+        item = orjson.loads(msg)
+        item['uid'] = uid[1:].decode()
+        if uid.startswith(b"0"):
+            item['user_role'] = True
+        else:
+            item['assistant_role'] = True
 
-            chat_data.add_message(item)
+        chat_data.add_message(item, markdown=render_with_markdown)
 
 elif selected_section == "Playground":
     st.write("## todo")
 
 elif selected_section == "Statistics":
     st.write("## todo")
```

### Comparing `openai_forward-0.7.2/.gitignore` & `openai_forward-0.8.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .github/release-template.ejs
 .github/workflows/doc.yml
 
-scripts/release.sh
 node_modules
 package-lock.json
 package.json
 .idea/
 .vscode/
 .DS_Store
 third-party/
```

### Comparing `openai_forward-0.7.2/LICENSE` & `openai_forward-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/README.md` & `openai_forward-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 **简体中文** | [**English**](https://github.com/KenyonY/openai-forward/blob/main/README_EN.md)
 
 <h1 align="center">
-    <a href="https://github.com/KenyonY/openai-forward"> 🌠 OpenAI Forward </a>
+    <a href="https://github.com/KenyonY/openai-forward">  OpenAI Forward </a>
     <br>
     <br>
 </h1>
 
 <p align="center">
     <a href="https://pypi.org/project/openai-forward/">
         <img src="https://img.shields.io/pypi/v/openai-forward?color=brightgreen&style=flat-square" alt="PyPI version" >
@@ -22,16 +22,14 @@
     <a href="https://pypistats.org/packages/openai-forward">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward?style=flat-square">
     </a>
 </p>
 
 <div align="center">
 
-[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/KenyonY/openai-forward)
-
 [特点](#主要特性) |
 [部署指南](deploy.md) |
 [使用指南](#使用指南) |
 [配置](#配置) |
 [对话日志](#对话日志)
 
 
@@ -159,59 +157,36 @@
   from openai import OpenAI  # pip install openai>=1.0.0
   client = OpenAI(
 +     base_url="https://api.openai-forward.com/v1", 
       api_key="sk-******"
   )
 ```
 
-<details >
-   <summary> 更多</summary>  
-
-#### 在三方应用中使用
-
-基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)中接入:   
-替换docker启动命令中的 `BASE_URL`为自己搭建的代理服务地址
-
-```bash 
-docker run -d \
-    -p 3000:3000 \
-    -e OPENAI_API_KEY="sk-******" \
-    -e BASE_URL="https://api.openai-forward.com" \
-    -e CODE="******" \
-    yidadaa/chatgpt-next-web 
-``` 
-
-**Image Generation (DALL-E)**
-
-```bash
-curl --location 'https://api.openai-forward.com/v1/images/generations' \
---header 'Authorization: Bearer sk-******' \
---header 'Content-Type: application/json' \
---data '{
-    "prompt": "A photo of a cat",
-    "n": 1,
-    "size": "512x512"
-}'
-```
-
-</details>
 
 ### 代理本地模型
 
 - **适用场景：** 与 [LocalAI](https://github.com/go-skynet/LocalAI)，
   [api-for-open-llm](https://github.com/xusenlinzy/api-for-open-llm)等项目一起使用
 
 - **如何操作：**
   以LocalAI为例，如果已在 http://localhost:8080 部署了LocalAI服务，仅需在环境变量或 .env
   文件中设置 `FORWARD_CONFIG=[{"base_url":"http://localhost:8080","route":"/localai","type":"openai"}]`。
   然后即可通过访问 http://localhost:8000/localai 使用LocalAI。
 
 (更多)
 
-### 代理其它云端模型
+### 代理任意云端模型
+
+#### 代理[gemini pro](https://ai.google.dev/)
+配置环境变量或 .env 文件如下：
+```env
+FORWARD_CONFIG=[{"base_url":"https://generativelanguage.googleapis.com","route":"/gemini","type":"general"}]
+```
+说明：`aidf run`启动后，即可通过访问 http://localhost:8000/gemini 使用gemini pro。
+
 
 - **场景1:**
   使用通用转发,可对任意来源服务进行转发，
   可获得请求速率控制与token速率控制；但通用转发不支持自定义秘钥.
 
 - **场景2：**
   可通过 [LiteLLM](https://github.com/BerriAI/litellm) 可以将 众多云模型的 API 格式转换为 openai
```

#### html2text {}

```diff
@@ -1,15 +1,13 @@
 **ç®ä½ä¸­æ** | [**English**](https://github.com/KenyonY/openai-forward/
 blob/main/README_EN.md)
-                          ************ _?ð_?_?_? _ _OO_pp_ee_nn_AA_II_ _FF_oo_rr_ww_aa_rr_dd
+                             ************ _OO_pp_ee_nn_AA_II_ _FF_oo_rr_ww_aa_rr_dd
 
                                      ************
           _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_d_o_c_k_e_r_ _p_u_l_l_]_[_t_e_s_t_s_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]
- [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)]
-  (https://render.com/deploy?repo=https://github.com/KenyonY/openai-forward)
      [ç¹ç¹](#ä¸»è¦ç¹æ§) | [é¨ç½²æå](deploy.md) | [ä½¿ç¨æå]
       (#ä½¿ç¨æå) | [éç½®](#éç½®) | [å¯¹è¯æ¥å¿](#å¯¹è¯æ¥å¿)
 > [!IMPORTANT] > >
 å¨v0.7.0ä»¥åå¨éç½®æ¹é¢ä¼æè¾å¤§è°æ´ï¼å¹¶ä¸ä¹åçæ¬ä¸å¼å®¹ãéè¿UIéç½®èµ·æ¥ä¼æ´å æ¹ä¾¿ï¼ä¸æä¾äºæ´å¼ºå¤§çéç½®éé¡¹ã
 **OpenAI-Forward**
 æ¯ä¸ºå¤§åè¯­è¨æ¨¡åå®ç°çé«æè½¬åæå¡ãå¶æ ¸å¿åè½åæ¬
 ç¨æ·è¯·æ±éçæ§å¶ãTokenéçéå¶ãæºè½é¢æµç¼å­ãæ¥å¿ç®¡çåAPIå¯é¥ç®¡çç­ï¼æ¨å¨æä¾é«æãä¾¿æ·çæ¨¡åè½¬åæå¡ã
@@ -59,31 +57,27 @@
 INFO: Started server process [191471] INFO: Waiting for application startup.
 INFO: Application startup complete. INFO: Uvicorn running on http://0.0.0.0:
 8000 (Press CTRL+C to quit) ``` ### ä»£çOpenAIæ¨¡å: `aifd
 run`çé»è®¤éé¡¹ä¾¿æ¯ä»£ç`https://api.openai.com`
 ä¸é¢ä»¥æ­å»ºå¥½çæå¡å°å`https://api.openai-forward.com` ä¸ºä¾
 **Python** ```diff from openai import OpenAI # pip install openai>=1.0.0 client
 = OpenAI( + base_url="https://api.openai-forward.com/v1", api_key="sk-******" )
-``` æ´å¤ #### å¨ä¸æ¹åºç¨ä¸­ä½¿ç¨ åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web]
-(https://github.com/Yidadaa/ChatGPT-Next-Web)ä¸­æ¥å¥:
-æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç `BASE_URL`ä¸ºèªå·±æ­å»ºçä»£çæå¡å°å
-```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
-e BASE_URL="https://api.openai-forward.com" \ -e CODE="******" \ yidadaa/
-chatgpt-next-web ``` **Image Generation (DALL-E)** ```bash curl --location
-'https://api.openai-forward.com/v1/images/generations' \ --header
-'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
---data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
-ä»£çæ¬å°æ¨¡å - **éç¨åºæ¯ï¼** ä¸ [LocalAI](https://github.com/go-
-skynet/LocalAI)ï¼ [api-for-open-llm](https://github.com/xusenlinzy/api-for-
-open-llm)ç­é¡¹ç®ä¸èµ·ä½¿ç¨ - **å¦ä½æä½ï¼**
+``` ### ä»£çæ¬å°æ¨¡å - **éç¨åºæ¯ï¼** ä¸ [LocalAI](https://
+github.com/go-skynet/LocalAI)ï¼ [api-for-open-llm](https://github.com/
+xusenlinzy/api-for-open-llm)ç­é¡¹ç®ä¸èµ·ä½¿ç¨ - **å¦ä½æä½ï¼**
 ä»¥LocalAIä¸ºä¾ï¼å¦æå·²å¨ http://localhost:8080
 é¨ç½²äºLocalAIæå¡ï¼ä»éå¨ç¯å¢åéæ .env æä»¶ä¸­è®¾ç½®
 `FORWARD_CONFIG=[{"base_url":"http://localhost:8080","route":"/localai","type":
 "openai"}]`ã ç¶åå³å¯éè¿è®¿é® http://localhost:8000/localai
-ä½¿ç¨LocalAIã (æ´å¤) ### ä»£çå¶å®äºç«¯æ¨¡å - **åºæ¯1:**
+ä½¿ç¨LocalAIã (æ´å¤) ### ä»£çä»»æäºç«¯æ¨¡å #### ä»£ç[gemini pro]
+(https://ai.google.dev/) éç½®ç¯å¢åéæ .env æä»¶å¦ä¸ï¼ ```env
+FORWARD_CONFIG=[{"base_url":"https://
+generativelanguage.googleapis.com","route":"/gemini","type":"general"}] ```
+è¯´æï¼`aidf run`å¯å¨åï¼å³å¯éè¿è®¿é® http://localhost:8000/gemini
+ä½¿ç¨gemini proã - **åºæ¯1:**
 ä½¿ç¨éç¨è½¬å,å¯å¯¹ä»»ææ¥æºæå¡è¿è¡è½¬åï¼
 å¯è·å¾è¯·æ±éçæ§å¶ä¸tokenéçæ§å¶ï¼ä½éç¨è½¬åä¸æ¯æèªå®ä¹ç§é¥.
 - **åºæ¯2ï¼** å¯éè¿ [LiteLLM](https://github.com/BerriAI/litellm)
 å¯ä»¥å° ä¼å¤äºæ¨¡åç API æ ¼å¼è½¬æ¢ä¸º openai
 çapiæ ¼å¼ï¼ç¶åä½¿ç¨openaié£æ ¼è½¬å (æ´å¤) [https://
 raw.githubusercontent.com/KenyonY/openai-forward/main/.github/images/
 separators/aqua.png]## éç½® æ§è¡ `aifd run --webui` è¿å¥éç½®é¡µé¢
```

### Comparing `openai_forward-0.7.2/pyproject.toml` & `openai_forward-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.2/PKG-INFO` & `openai_forward-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openai_forward
-Version: 0.7.2
+Version: 0.8.0
 Summary: 🚀 OpenAI-Forward 是一个专为大型语言模型设计的高级转发代理，提供包括用户请求速率控制、Token速率限制和自定义API密钥等增强功能。该服务可用于代理本地模型和云端模型。OpenAI API Reverse Proxy
 Project-URL: Homepage, https://github.com/KenyonY/openai-forward
 Project-URL: Documentation, https://github.com/KenyonY/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/KenyonY/openai-forward/issues
 Project-URL: Source, https://github.com/KenyonY/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-Expression: MIT
@@ -47,15 +47,15 @@
 Provides-Extra: webui
 Requires-Dist: streamlit~=1.30.0; extra == 'webui'
 Description-Content-Type: text/markdown
 
 **简体中文** | [**English**](https://github.com/KenyonY/openai-forward/blob/main/README_EN.md)
 
 <h1 align="center">
-    <a href="https://github.com/KenyonY/openai-forward"> 🌠 OpenAI Forward </a>
+    <a href="https://github.com/KenyonY/openai-forward">  OpenAI Forward </a>
     <br>
     <br>
 </h1>
 
 <p align="center">
     <a href="https://pypi.org/project/openai-forward/">
         <img src="https://img.shields.io/pypi/v/openai-forward?color=brightgreen&style=flat-square" alt="PyPI version" >
@@ -72,16 +72,14 @@
     <a href="https://pypistats.org/packages/openai-forward">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward?style=flat-square">
     </a>
 </p>
 
 <div align="center">
 
-[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/KenyonY/openai-forward)
-
 [特点](#主要特性) |
 [部署指南](deploy.md) |
 [使用指南](#使用指南) |
 [配置](#配置) |
 [对话日志](#对话日志)
 
 
@@ -209,59 +207,36 @@
   from openai import OpenAI  # pip install openai>=1.0.0
   client = OpenAI(
 +     base_url="https://api.openai-forward.com/v1", 
       api_key="sk-******"
   )
 ```
 
-<details >
-   <summary> 更多</summary>  
-
-#### 在三方应用中使用
-
-基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)中接入:   
-替换docker启动命令中的 `BASE_URL`为自己搭建的代理服务地址
-
-```bash 
-docker run -d \
-    -p 3000:3000 \
-    -e OPENAI_API_KEY="sk-******" \
-    -e BASE_URL="https://api.openai-forward.com" \
-    -e CODE="******" \
-    yidadaa/chatgpt-next-web 
-``` 
-
-**Image Generation (DALL-E)**
-
-```bash
-curl --location 'https://api.openai-forward.com/v1/images/generations' \
---header 'Authorization: Bearer sk-******' \
---header 'Content-Type: application/json' \
---data '{
-    "prompt": "A photo of a cat",
-    "n": 1,
-    "size": "512x512"
-}'
-```
-
-</details>
 
 ### 代理本地模型
 
 - **适用场景：** 与 [LocalAI](https://github.com/go-skynet/LocalAI)，
   [api-for-open-llm](https://github.com/xusenlinzy/api-for-open-llm)等项目一起使用
 
 - **如何操作：**
   以LocalAI为例，如果已在 http://localhost:8080 部署了LocalAI服务，仅需在环境变量或 .env
   文件中设置 `FORWARD_CONFIG=[{"base_url":"http://localhost:8080","route":"/localai","type":"openai"}]`。
   然后即可通过访问 http://localhost:8000/localai 使用LocalAI。
 
 (更多)
 
-### 代理其它云端模型
+### 代理任意云端模型
+
+#### 代理[gemini pro](https://ai.google.dev/)
+配置环境变量或 .env 文件如下：
+```env
+FORWARD_CONFIG=[{"base_url":"https://generativelanguage.googleapis.com","route":"/gemini","type":"general"}]
+```
+说明：`aidf run`启动后，即可通过访问 http://localhost:8000/gemini 使用gemini pro。
+
 
 - **场景1:**
   使用通用转发,可对任意来源服务进行转发，
   可获得请求速率控制与token速率控制；但通用转发不支持自定义秘钥.
 
 - **场景2：**
   可通过 [LiteLLM](https://github.com/BerriAI/litellm) 可以将 众多云模型的 API 格式转换为 openai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: openai_forward Version: 0.7.2 Summary: ð OpenAI-
+Metadata-Version: 2.3 Name: openai_forward Version: 0.8.0 Summary: ð OpenAI-
 Forward
 æ¯ä¸ä¸ªä¸ä¸ºå¤§åè¯­è¨æ¨¡åè®¾è®¡çé«çº§è½¬åä»£çï¼æä¾åæ¬ç¨æ·è¯·æ±éçæ§å¶ãTokenéçéå¶åèªå®ä¹APIå¯é¥ç­å¢å¼ºåè½ãè¯¥æå¡å¯ç¨äºä»£çæ¬å°æ¨¡ååäºç«¯æ¨¡åãOpenAI
 API Reverse Proxy Project-URL: Homepage, https://github.com/KenyonY/openai-
 forward Project-URL: Documentation, https://github.com/KenyonY/openai-
 forward#openai-forward Project-URL: Issues, https://github.com/KenyonY/openai-
 forward/issues Project-URL: Source, https://github.com/KenyonY/openai-forward
 Author-email: kunyuan
@@ -22,20 +22,18 @@
 Dist: sparrow-python; extra == 'dev' Provides-Extra: test Requires-Dist:
 openai>=1.3.0; extra == 'test' Requires-Dist: psutil; extra == 'test' Requires-
 Dist: pytest; extra == 'test' Requires-Dist: pytest-aiohttp; extra == 'test'
 Requires-Dist: trio; extra == 'test' Requires-Dist: twisted; extra == 'test'
 Provides-Extra: webui Requires-Dist: streamlit~=1.30.0; extra == 'webui'
 Description-Content-Type: text/markdown **ç®ä½ä¸­æ** | [**English**](https:
 //github.com/KenyonY/openai-forward/blob/main/README_EN.md)
-                          ************ _?ð_?_?_? _ _OO_pp_ee_nn_AA_II_ _FF_oo_rr_ww_aa_rr_dd
+                             ************ _OO_pp_ee_nn_AA_II_ _FF_oo_rr_ww_aa_rr_dd
 
                                      ************
           _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_d_o_c_k_e_r_ _p_u_l_l_]_[_t_e_s_t_s_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]
- [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)]
-  (https://render.com/deploy?repo=https://github.com/KenyonY/openai-forward)
      [ç¹ç¹](#ä¸»è¦ç¹æ§) | [é¨ç½²æå](deploy.md) | [ä½¿ç¨æå]
       (#ä½¿ç¨æå) | [éç½®](#éç½®) | [å¯¹è¯æ¥å¿](#å¯¹è¯æ¥å¿)
 > [!IMPORTANT] > >
 å¨v0.7.0ä»¥åå¨éç½®æ¹é¢ä¼æè¾å¤§è°æ´ï¼å¹¶ä¸ä¹åçæ¬ä¸å¼å®¹ãéè¿UIéç½®èµ·æ¥ä¼æ´å æ¹ä¾¿ï¼ä¸æä¾äºæ´å¼ºå¤§çéç½®éé¡¹ã
 **OpenAI-Forward**
 æ¯ä¸ºå¤§åè¯­è¨æ¨¡åå®ç°çé«æè½¬åæå¡ãå¶æ ¸å¿åè½åæ¬
 ç¨æ·è¯·æ±éçæ§å¶ãTokenéçéå¶ãæºè½é¢æµç¼å­ãæ¥å¿ç®¡çåAPIå¯é¥ç®¡çç­ï¼æ¨å¨æä¾é«æãä¾¿æ·çæ¨¡åè½¬åæå¡ã
@@ -85,31 +83,27 @@
 INFO: Started server process [191471] INFO: Waiting for application startup.
 INFO: Application startup complete. INFO: Uvicorn running on http://0.0.0.0:
 8000 (Press CTRL+C to quit) ``` ### ä»£çOpenAIæ¨¡å: `aifd
 run`çé»è®¤éé¡¹ä¾¿æ¯ä»£ç`https://api.openai.com`
 ä¸é¢ä»¥æ­å»ºå¥½çæå¡å°å`https://api.openai-forward.com` ä¸ºä¾
 **Python** ```diff from openai import OpenAI # pip install openai>=1.0.0 client
 = OpenAI( + base_url="https://api.openai-forward.com/v1", api_key="sk-******" )
-``` æ´å¤ #### å¨ä¸æ¹åºç¨ä¸­ä½¿ç¨ åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web]
-(https://github.com/Yidadaa/ChatGPT-Next-Web)ä¸­æ¥å¥:
-æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç `BASE_URL`ä¸ºèªå·±æ­å»ºçä»£çæå¡å°å
-```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
-e BASE_URL="https://api.openai-forward.com" \ -e CODE="******" \ yidadaa/
-chatgpt-next-web ``` **Image Generation (DALL-E)** ```bash curl --location
-'https://api.openai-forward.com/v1/images/generations' \ --header
-'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
---data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
-ä»£çæ¬å°æ¨¡å - **éç¨åºæ¯ï¼** ä¸ [LocalAI](https://github.com/go-
-skynet/LocalAI)ï¼ [api-for-open-llm](https://github.com/xusenlinzy/api-for-
-open-llm)ç­é¡¹ç®ä¸èµ·ä½¿ç¨ - **å¦ä½æä½ï¼**
+``` ### ä»£çæ¬å°æ¨¡å - **éç¨åºæ¯ï¼** ä¸ [LocalAI](https://
+github.com/go-skynet/LocalAI)ï¼ [api-for-open-llm](https://github.com/
+xusenlinzy/api-for-open-llm)ç­é¡¹ç®ä¸èµ·ä½¿ç¨ - **å¦ä½æä½ï¼**
 ä»¥LocalAIä¸ºä¾ï¼å¦æå·²å¨ http://localhost:8080
 é¨ç½²äºLocalAIæå¡ï¼ä»éå¨ç¯å¢åéæ .env æä»¶ä¸­è®¾ç½®
 `FORWARD_CONFIG=[{"base_url":"http://localhost:8080","route":"/localai","type":
 "openai"}]`ã ç¶åå³å¯éè¿è®¿é® http://localhost:8000/localai
-ä½¿ç¨LocalAIã (æ´å¤) ### ä»£çå¶å®äºç«¯æ¨¡å - **åºæ¯1:**
+ä½¿ç¨LocalAIã (æ´å¤) ### ä»£çä»»æäºç«¯æ¨¡å #### ä»£ç[gemini pro]
+(https://ai.google.dev/) éç½®ç¯å¢åéæ .env æä»¶å¦ä¸ï¼ ```env
+FORWARD_CONFIG=[{"base_url":"https://
+generativelanguage.googleapis.com","route":"/gemini","type":"general"}] ```
+è¯´æï¼`aidf run`å¯å¨åï¼å³å¯éè¿è®¿é® http://localhost:8000/gemini
+ä½¿ç¨gemini proã - **åºæ¯1:**
 ä½¿ç¨éç¨è½¬å,å¯å¯¹ä»»ææ¥æºæå¡è¿è¡è½¬åï¼
 å¯è·å¾è¯·æ±éçæ§å¶ä¸tokenéçæ§å¶ï¼ä½éç¨è½¬åä¸æ¯æèªå®ä¹ç§é¥.
 - **åºæ¯2ï¼** å¯éè¿ [LiteLLM](https://github.com/BerriAI/litellm)
 å¯ä»¥å° ä¼å¤äºæ¨¡åç API æ ¼å¼è½¬æ¢ä¸º openai
 çapiæ ¼å¼ï¼ç¶åä½¿ç¨openaié£æ ¼è½¬å (æ´å¤) [https://
 raw.githubusercontent.com/KenyonY/openai-forward/main/.github/images/
 separators/aqua.png]## éç½® æ§è¡ `aifd run --webui` è¿å¥éç½®é¡µé¢
```

