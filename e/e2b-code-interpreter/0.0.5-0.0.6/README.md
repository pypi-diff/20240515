# Comparing `tmp/e2b_code_interpreter-0.0.5.tar.gz` & `tmp/e2b_code_interpreter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b_code_interpreter-0.0.5.tar", max compression
+gzip compressed data, was "e2b_code_interpreter-0.0.6.tar", max compression
```

## Comparing `e2b_code_interpreter-0.0.5.tar` & `e2b_code_interpreter-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2331 2024-05-02 05:31:11.046967 e2b_code_interpreter-0.0.5/README.md
--rw-r--r--   0        0        0      149 2024-05-02 05:31:11.046967 e2b_code_interpreter-0.0.5/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0    11061 2024-05-02 05:31:11.046967 e2b_code_interpreter-0.0.5/e2b_code_interpreter/main.py
--rw-r--r--   0        0        0     9056 2024-05-02 05:31:11.046967 e2b_code_interpreter-0.0.5/e2b_code_interpreter/messaging.py
--rw-r--r--   0        0        0     7884 2024-05-02 05:31:11.046967 e2b_code_interpreter-0.0.5/e2b_code_interpreter/models.py
--rw-r--r--   0        0        0      766 2024-05-02 05:31:34.646743 e2b_code_interpreter-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2331 2024-05-14 23:43:53.442159 e2b_code_interpreter-0.0.6/README.md
+-rw-r--r--   0        0        0      149 2024-05-14 23:43:53.442159 e2b_code_interpreter-0.0.6/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    11079 2024-05-14 23:43:53.442159 e2b_code_interpreter-0.0.6/e2b_code_interpreter/main.py
+-rw-r--r--   0        0        0     8821 2024-05-14 23:43:53.446159 e2b_code_interpreter-0.0.6/e2b_code_interpreter/messaging.py
+-rw-r--r--   0        0        0     7884 2024-05-14 23:43:53.446159 e2b_code_interpreter-0.0.6/e2b_code_interpreter/models.py
+-rw-r--r--   0        0        0      766 2024-05-14 23:44:20.110434 e2b_code_interpreter-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.6/PKG-INFO
```

### Comparing `e2b_code_interpreter-0.0.5/README.md` & `e2b_code_interpreter-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.5/e2b_code_interpreter/main.py` & `e2b_code_interpreter-0.0.6/e2b_code_interpreter/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,21 +48,21 @@
         )
         self.notebook = JupyterExtension(self, timeout=timeout)
         # Close all the websocket connections when the interpreter is closed
         self._process_cleanup.append(self.notebook.close)
 
 
 class JupyterExtension:
-    _default_kernel_id: Optional[str] = None
-    _connected_kernels: Dict[str, Future[JupyterKernelWebSocket]] = {}
 
     def __init__(self, sandbox: CodeInterpreter, timeout: Optional[float] = TIMEOUT):
         self._sandbox = sandbox
         self._kernel_id_set = Future()
         self._start_connecting_to_default_kernel(timeout=timeout)
+        self._connected_kernels: Dict[str, Future[JupyterKernelWebSocket]] = {}
+        self._default_kernel_id: Optional[str] = None
 
     def exec_cell(
         self,
         code: str,
         kernel_id: Optional[str] = None,
         on_stdout: Optional[Callable[[ProcessMessage], Any]] = None,
         on_stderr: Optional[Callable[[ProcessMessage], Any]] = None,
```

### Comparing `e2b_code_interpreter-0.0.5/e2b_code_interpreter/messaging.py` & `e2b_code_interpreter-0.0.6/e2b_code_interpreter/messaging.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,63 +39,62 @@
         self.partial_result = Execution()
         self.execution = Future()
         self.on_stdout = on_stdout
         self.on_stderr = on_stderr
         self.on_result = on_result
 
 
-class JupyterKernelWebSocket(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True)
+class JupyterKernelWebSocket:
 
-    url: str
-
-    _cells: Dict[str, CellExecution] = {}
-    _waiting_for_replies: Dict[str, DeferredFuture] = PrivateAttr(default_factory=dict)
-    _queue_in: Queue = PrivateAttr(default_factory=Queue)
-    _queue_out: Queue = PrivateAttr(default_factory=Queue)
-    _process_cleanup: List[Callable[[], Any]] = PrivateAttr(default_factory=list)
-    _closed: bool = PrivateAttr(default=False)
+    def __init__(self, url: str):
+        self.url = url
+        self._cells: Dict[str, CellExecution] = {}
+        self._waiting_for_replies: Dict[str, DeferredFuture] = {}
+        self._queue_in = Queue()
+        self._queue_out = Queue()
+        self._stopped = threading.Event()
 
     def process_messages(self):
-        while True:
-            data = self._queue_out.get()
+        while not self._stopped.is_set():
+            if self._queue_out.empty():
+                time.sleep(0.01)
+                continue
 
+            data = self._queue_out.get()
             logger.debug(f"WebSocket received message: {data}".strip())
             self._receive_message(json.loads(data))
             self._queue_out.task_done()
 
     def connect(self, timeout: float = TIMEOUT):
         started = threading.Event()
-        stopped = threading.Event()
-        self._process_cleanup.append(stopped.set)
 
         threading.Thread(
             target=self.process_messages, daemon=True, name="e2b-process-messages"
         ).start()
 
         threading.Thread(
             target=WebSocket(
                 url=self.url,
                 queue_in=self._queue_in,
                 queue_out=self._queue_out,
                 started=started,
-                stopped=stopped,
+                stopped=self._stopped
             ).run,
             daemon=True,
             name="e2b-code-interpreter-websocket",
         ).start()
 
         logger.debug("WebSocket waiting to start")
 
         try:
             start_time = time.time()
             while (
                 not started.is_set()
                 and time.time() - start_time < timeout
-                and not self._closed
+                and not self._stopped.is_set()
             ):
                 time.sleep(0.1)
 
             if not started.is_set():
                 raise TimeoutException("WebSocket failed to start")
         except BaseException as e:
             self.close()
@@ -241,18 +240,13 @@
             logger.debug(f"Input accepted for {parent_msg_ig}")
             cell.input_accepted = True
         else:
             logger.warning(f"[UNHANDLED MESSAGE TYPE]: {data['msg_type']}")
 
     def close(self):
         logger.debug("Closing WebSocket")
-        self._closed = True
-
-        for cancel in self._process_cleanup:
-            cancel()
-
-        self._process_cleanup.clear()
+        self._stopped.set()
 
         for handler in self._waiting_for_replies.values():
             logger.debug(f"Cancelling waiting for execution result for {handler}")
             handler.cancel()
             del handler
```

### Comparing `e2b_code_interpreter-0.0.5/e2b_code_interpreter/models.py` & `e2b_code_interpreter-0.0.6/e2b_code_interpreter/models.py`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.5/pyproject.toml` & `e2b_code_interpreter-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "e2b-code-interpreter"
-version = "0.0.5"
+version = "0.0.6"
 description = "E2B Code Interpreter - Stateful code execution"
 authors = ["e2b <hello@e2b.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b-code-interpreter/tree/python"
 packages = [{ include = "e2b_code_interpreter" }]
```

### Comparing `e2b_code_interpreter-0.0.5/PKG-INFO` & `e2b_code_interpreter-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2b-code-interpreter
-Version: 0.0.5
+Version: 0.0.6
 Summary: E2B Code Interpreter - Stateful code execution
 Home-page: https://e2b.dev/
 License: Apache-2.0
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

