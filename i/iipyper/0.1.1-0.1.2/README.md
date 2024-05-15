# Comparing `tmp/iipyper-0.1.1.tar.gz` & `tmp/iipyper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iipyper-0.1.1.tar", max compression
+gzip compressed data, was "iipyper-0.1.2.tar", max compression
```

## Comparing `iipyper-0.1.1.tar` & `iipyper-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.521024 iipyper-0.1.1/LICENSE
--rw-r--r--   0        0        0     2127 2023-11-28 17:22:02.521113 iipyper-0.1.1/README.md
--rw-r--r--   0        0        0      984 2024-03-16 00:15:32.993388 iipyper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4057 2024-03-15 23:43:00.590525 iipyper-0.1.1/src/iipyper/__init__.py
--rw-r--r--   0        0        0     1011 2024-03-15 23:43:00.590729 iipyper-0.1.1/src/iipyper/audio.py
--rw-r--r--   0        0        0     9045 2024-03-15 23:43:00.590978 iipyper-0.1.1/src/iipyper/midi.py
--rw-r--r--   0        0        0    32516 2024-02-20 14:04:12.786364 iipyper-0.1.1/src/iipyper/osc.py
--rw-r--r--   0        0        0      213 2023-11-28 17:22:02.524007 iipyper-0.1.1/src/iipyper/state.py
--rw-r--r--   0        0        0     1311 2023-12-07 13:43:17.591203 iipyper-0.1.1/src/iipyper/timing.py
--rw-r--r--   0        0        0     4920 2023-11-28 17:22:02.524135 iipyper-0.1.1/src/iipyper/tui.py
--rw-r--r--   0        0        0     1795 2024-01-04 17:20:53.154026 iipyper-0.1.1/src/iipyper/types.py
--rw-r--r--   0        0        0      871 2023-12-05 15:55:26.909601 iipyper-0.1.1/src/iipyper/util.py
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 iipyper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.521024 iipyper-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2138 2024-03-16 00:39:01.445389 iipyper-0.1.2/README.md
+-rw-r--r--   0        0        0      984 2024-05-15 20:37:51.251964 iipyper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4057 2024-03-15 23:43:00.590525 iipyper-0.1.2/src/iipyper/__init__.py
+-rw-r--r--   0        0        0     1011 2024-03-15 23:43:00.590729 iipyper-0.1.2/src/iipyper/audio.py
+-rw-r--r--   0        0        0     9349 2024-05-15 20:17:34.072216 iipyper-0.1.2/src/iipyper/midi.py
+-rw-r--r--   0        0        0    32977 2024-05-15 20:17:34.072636 iipyper-0.1.2/src/iipyper/osc.py
+-rw-r--r--   0        0        0      213 2023-11-28 17:22:02.524007 iipyper-0.1.2/src/iipyper/state.py
+-rw-r--r--   0        0        0     1311 2023-12-07 13:43:17.591203 iipyper-0.1.2/src/iipyper/timing.py
+-rw-r--r--   0        0        0     5108 2024-05-15 20:17:34.072912 iipyper-0.1.2/src/iipyper/tui.py
+-rw-r--r--   0        0        0     1795 2024-01-04 17:20:53.154026 iipyper-0.1.2/src/iipyper/types.py
+-rw-r--r--   0        0        0      937 2024-05-15 20:17:34.073139 iipyper-0.1.2/src/iipyper/util.py
+-rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 iipyper-0.1.2/PKG-INFO
```

### Comparing `iipyper-0.1.1/LICENSE` & `iipyper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.1/README.md` & `iipyper-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 pip install iipyper
 ```
 
 ## Develop
 
 ```sh
 git clone git@github.com:Intelligent-Instruments-Lab/iipyper.git
-pip install -e iipyper
+cd iipyper
+poetry install iipyper
 ```
 
 ## Contact
 
 `iipyper` is developed by the [Intelligent Instruments Lab](https://iil.is/about). Get in touch to [collaborate](https://iil.is/collaborate):
 
  ◦ <a href="https://iil.is" target="_blank" rel="noopener" title="Intelligent Instrumets Lab">iil.is</a> ◦
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 Control](https://en.wikipedia.org/wiki/Open_Sound_Control) (OSC) and [MIDI]
 (https://en.wikipedia.org/wiki/MIDI)-based event loops. It is designed for
 creatives who want to explore the Python ecosystem and experiment with music
 and, for example, machine learning. For examples and tutorials of how to use
 `iipyper`, see our [examples repo](https://github.com/intelligent-instruments-
 lab/iil-examples) (TBC). ## Install `iipyper` can be installed via [PyPI]
 (https://pypi.org/project/iipyper): ```sh pip install iipyper ``` ## Develop
-```sh git clone git@github.com:Intelligent-Instruments-Lab/iipyper.git pip
-install -e iipyper ``` ## Contact `iipyper` is developed by the [Intelligent
-Instruments Lab](https://iil.is/about). Get in touch to [collaborate](https://
-iil.is/collaborate): â¦ _i_i_l_._i_s â¦ _F_a_c_e_b_o_o_k â¦ _I_n_s_t_a_g_r_a_m â¦ _X_ _(_T_w_i_t_t_e_r_) â¦
-_Y_o_u_T_u_b_e â¦ _D_i_s_c_o_r_d â¦ _G_i_t_H_u_b â¦ _L_i_n_k_e_d_I_n â¦ _E_m_a_i_l â¦ ## Funding The
-Intelligent Instruments project (INTENT) is funded by the European Research
-Council (ERC) under the European Unionâs Horizon 2020 research and innovation
-programme (Grant agreement No. 101001848).
+```sh git clone git@github.com:Intelligent-Instruments-Lab/iipyper.git cd
+iipyper poetry install iipyper ``` ## Contact `iipyper` is developed by the
+[Intelligent Instruments Lab](https://iil.is/about). Get in touch to
+[collaborate](https://iil.is/collaborate): â¦ _i_i_l_._i_s â¦ _F_a_c_e_b_o_o_k â¦
+_I_n_s_t_a_g_r_a_m â¦ _X_ _(_T_w_i_t_t_e_r_) â¦ _Y_o_u_T_u_b_e â¦ _D_i_s_c_o_r_d â¦ _G_i_t_H_u_b â¦ _L_i_n_k_e_d_I_n â¦
+_E_m_a_i_l â¦ ## Funding The Intelligent Instruments project (INTENT) is funded by
+the European Research Council (ERC) under the European Unionâs Horizon 2020
+research and innovation programme (Grant agreement No. 101001848).
```

### Comparing `iipyper-0.1.1/pyproject.toml` & `iipyper-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iipyper"
-version = "0.1.1"
+version = "0.1.2"
 description = "python package for easy MIDI, OSC, event loops"
 authors = ["Victor Shepardson <victor.shepardson@gmail.com>", "Jack Armitage <jack.armitage@me.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Intelligent-Instruments-Lab/iipyper"
 documentation = "https://intelligent-instruments-lab.github.io/iipyper/"
```

### Comparing `iipyper-0.1.1/src/iipyper/__init__.py` & `iipyper-0.1.2/src/iipyper/__init__.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.1/src/iipyper/audio.py` & `iipyper-0.1.2/src/iipyper/audio.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.1/src/iipyper/midi.py` & `iipyper-0.1.2/src/iipyper/midi.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         self.running = False
 
         self.verbose = int(verbose)
         # self.sleep_time = sleep_time
         # type -> list[Optional[set[port], Optional[set[channel]], function]
         self.handlers = []
 
+        self.handler_docs = []
+
         if isinstance(in_ports, str):
             in_ports = in_ports.split(',')
         if isinstance(out_ports, str):
             out_ports = out_ports.split(',')
 
         # TODO: fuzzy match port names
 
@@ -163,18 +165,29 @@
                     'note', 'velocity', 'value', 
                     'control', 'program'
                     }, f'unknown MIDI message filter "{k}"'
             filters = {k:_get_filter(v) for k,v in kw.items()}
             f = None
 
         def decorator(f):
+            self.handler_docs.append((kw, f.__doc__))
+
             self.handlers.append((filters, f))
             return f
         
         return decorator if f is None else decorator(f)
+    
+    def get_docs(self):
+        s = ''
+        for filters,doc in self.handler_docs:
+            s += str(filters)
+            if doc is not None: 
+                s += doc
+            s += '\n'
+        return s
 
     def get_callback(self, port_name):
         if self.verbose>1: print(f'handler for MIDI port {port_name}')
         def callback(msg):
             if self.verbose > 1:
                 print(f'filtering MIDI {msg} port={port_name}')
             if not self.running:
```

### Comparing `iipyper-0.1.1/src/iipyper/osc.py` & `iipyper-0.1.2/src/iipyper/osc.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,14 +276,16 @@
         self.host = host
         self.port = port
         self.dispatcher = Dispatcher()
         self.server = None
         self.clients = {} # (host,port) -> client
         self.client_names = {} # (name) -> (host,port)
 
+        self.handler_docs = []
+
         self.create_server()
 
     def create_server(self):#, host=None, port=None):
         """
         Create the server
         """
         # if (host is None):
@@ -388,15 +390,15 @@
             route = '/'+route
         client.send_message(route, msg)
         if self.verbose > 0:
             print(f"OSC message sent {route}:{msg}")
     
     def handle(self, 
             route:str=None, return_host:str=None, return_port:int=None,
-            allow_pos=None, allow_kw=True, lock=True):
+            allow_pos=None, allow_kw=True, lock=True, doc:str=None):
         """
         OSC handler decorator supporting mixed args and kwargs, typing.
 
         The decorated function will receive the OSC route as its first argument.
         Further arguments will be the elements of the OSC message, which can be
         converted in various ways by supplying type annotations (see below).
 
@@ -415,14 +417,15 @@
                 if not given, reply to sender port.
                 NOTE: replying on the same port seems to work with SuperCollider,
                 but not with Max.
             kwargs: if True (default), parse OSC message for key-value pairs
                 corresponding to named arguments of the decorated function.
             lock: if True (default), use the global iipyper lock around the
                 decorated function
+            doc: replace the docstring of the decorated function
 
         keyword arguments of the decorated function:
             if a string with the same name as a parameter is found, 
             the following item in the OSC message will be used as the value.
             positional arguments can still be used before any keyword pairs,
             like in Python.
 
@@ -491,15 +494,15 @@
             f = route
             route = None
         else:
             f = None
 
         def decorator(f, route=route, 
                 return_host=return_host, return_port=return_port,
-                allow_pos=allow_pos, allow_kw=allow_kw):
+                allow_pos=allow_pos, allow_kw=allow_kw, doc=doc):
             # default_route = f'/{f.__name__}/*'
             if route is None:
                 route = f'/{f.__name__}'
             # print(route)
             assert isinstance(route, str) and route.startswith('/')
 
             # get info out of function signature
@@ -542,26 +545,28 @@
                 but the decorated function has a ** argument
                 """)
             if has_varp and not allow_pos:
                 raise ValueError(f"""
                 ERROR: iipyper: OSC handler {f} was created with args=False,
                 but the decorated function has a * argument
                 """)
+            
+            doc = doc or f.__doc__
+            self.handler_docs.append((route, doc))
 
             # wrap with pydantic validation decorator
             f = pydantic.validate_call(f)
 
             def handler(client, address, *osc_items):
                 """
                 Args:
                     client: (host,port) of sender
                     address: full OSC address
                     *args: content of OSC message
                 """
-                # print(f'{osc_items=}')
                 try:
                     args, kw = _parse_osc_items(
                         osc_items, 
                         (positional_params, named_params, has_varp, has_varkw), 
                         allow_pos, allow_kw,
                         self.verbose
                     )
@@ -631,14 +636,24 @@
             replace `json_keys` with type annotation of arguments as `object`.
             consider using `OSC.handle` instead of `OSC.kwargs`.
             """)
         return self.handle(
             route, return_host, return_port,
             allow_pos=False, allow_kw=True)
 
+    def get_docs(self):
+        """return a string built from routes and docstrings of osc handlers"""
+        s = ''
+        for route,doc in self.handler_docs:
+            s += route
+            if doc is not None: 
+                s += doc
+            s += '\n'
+        return s
+
     def __call__(self, client:str, *a, **kw):
         """
         alternate syntax for `send` with client name first
 
         `osc('my_client_name', 0, 1, 'message contents', None)`
 
         Args:
```

### Comparing `iipyper-0.1.1/src/iipyper/timing.py` & `iipyper-0.1.2/src/iipyper/timing.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.1/src/iipyper/tui.py` & `iipyper-0.1.2/src/iipyper/tui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import sys
+import threading
 try:
     from rich.panel import Panel
     from rich.pretty import Pretty
 
     from textual.app import App, ComposeResult
     from textual.reactive import reactive
-    from textual.widgets import Header, Footer, Static, Button, RichLog, Label
+    from textual.widgets import Header, Footer, Static, Button, Log, RichLog, Label
     from textual.css.query import NoMatches, TooManyMatches
 
     class TUI(App):
         """Base Textual app for iipyper programs."""
         ## e.g.
         # CSS_PATH = 'my_tui.css'
         # BINDINGS = [
         #     ("a", "my_a_action", "Do something when A is pressed"),
         #     ("b", "my_b_action", "Do somethign when B is pressed")]
 
         def __init__(self):
             super().__init__()
-            self.std_log = RichLog(id='std_log')
+            # self.std_log = RichLog(id='std_log')
+            self.std_log = Log(id='std_log')
+            self.buffered_writes = []
 
         def compose(self) -> ComposeResult:
             """Create child widgets for the Textual App.
             
             override this to build the TUI for your iipyper app.
             """
             yield Header()
@@ -51,55 +54,49 @@
                 self._mount = f
             else:
                 # this doesn't work for on_mount for whatever reason
                 setattr(self, f'on_{f.__name__}', f)
             return f
         
         def on_mount(self):
-            # self.std_log.write('MOUNT')
+            self.print('', end='') # flush buffered_writes to std_log
             try:
                 self._mount()
             except Exception as e:
                 print(e)
                 pass
         
         def set_mouse_move(self, f):
             self.on_mouse_move = f
             return f
 
         def on_button_pressed(self, event: Button.Pressed) -> None:
             getattr(self, f'action_{event.button.id}')()
 
-
-        # def _print(self, k, *v):
-        #     for s in (k, *v):
-        #         self.std_log.write(s)
-        #    # self.std_log.write(' '.join(str(s) for s in (k, *v)))
-
         def flush(self): pass
         def write(self, s):
             """for redirecting stdout to a file-like"""
             if self.is_running:
+                if len(self.buffered_writes):
+                    s = '\n'.join(self.buffered_writes)
+                    self.buffered_writes = []
                 return self.call_from_anywhere(self.std_log.write, s)
             else:
-                # TODO: buffer and write after start
+                self.buffered_writes.append(s)
                 return sys.__stdout__.write(s)
 
         def print(self, *a, **kw):
             """redirects to the UI's default std output log"""
             kw['file'] = self
             print(*a, **kw)
-            # if self.is_running:
-            #     self.call_from_anywhere(self._print, *a, **kw)
-            #     # try:
-            #     #     self.call_from_thread(self._print, *a, **kw)
-            #     # except:
-            #     #     self._print(*a, **kw)
-            # else:
-            #     print(*a, **kw)
+        
+        def print_defer(self, *a, **kw):
+            """redirects to the UI's default std output log"""
+            kw['file'] = self
+            threading.Thread(target=print, args=a, kwargs=kw).start()
 
         def call_from_anywhere(self, f, *a, **kw):
             try:
                 return self.call_from_thread(f, *a, **kw)
             except RuntimeError as e:
                 return f(*a, **kw)
 
@@ -111,14 +108,18 @@
                 # except:
                 #     self.do_call(*a, **kw)
             else:
                 print(*a)
                 for k,v in kw.items():
                     print(k, '->', v)
 
+        def defer(self, *a, **kw):
+            """__call__, but do it from a new thread and return immediately"""
+            threading.Thread(target=self, args=a, kwargs=kw, daemon=True).start()
+
         def _call(self, **kw):
             """
             by default, expects your TUI to have child nodes
             with a reactive `value` attribute, which updates the node when set.
             then calling my_tui(my_node_id=my_value) will update the node.
             """
             if not self.is_running:
```

### Comparing `iipyper-0.1.1/src/iipyper/types.py` & `iipyper-0.1.2/src/iipyper/types.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.1/src/iipyper/util.py` & `iipyper-0.1.2/src/iipyper/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import time
 from contextlib import contextmanager
 
 from .state import _lock
 
 @contextmanager
-def profile(label, print=print):
+def profile(label, print=print, enable=True):
+    if not enable:
+        yield None
+        return
     t = time.perf_counter_ns()
     yield None
     dt = (time.perf_counter_ns() - t)*1e-9
     print(f'{label}:\t {int(1000*dt)} ms')
 
 def maybe_lock(f, lock, *a, **kw):
     if lock:
```

### Comparing `iipyper-0.1.1/PKG-INFO` & `iipyper-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iipyper
-Version: 0.1.1
+Version: 0.1.2
 Summary: python package for easy MIDI, OSC, event loops
 Home-page: https://github.com/Intelligent-Instruments-Lab/iipyper
 License: MIT
 Author: Victor Shepardson
 Author-email: victor.shepardson@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,16 @@
 pip install iipyper
 ```
 
 ## Develop
 
 ```sh
 git clone git@github.com:Intelligent-Instruments-Lab/iipyper.git
-pip install -e iipyper
+cd iipyper
+poetry install iipyper
 ```
 
 ## Contact
 
 `iipyper` is developed by the [Intelligent Instruments Lab](https://iil.is/about). Get in touch to [collaborate](https://iil.is/collaborate):
 
  ◦ <a href="https://iil.is" target="_blank" rel="noopener" title="Intelligent Instrumets Lab">iil.is</a> ◦
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iipyper Version: 0.1.1 Summary: python package for
+Metadata-Version: 2.1 Name: iipyper Version: 0.1.2 Summary: python package for
 easy MIDI, OSC, event loops Home-page: https://github.com/Intelligent-
 Instruments-Lab/iipyper License: MIT Author: Victor Shepardson Author-email:
 victor.shepardson@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: mido (>=1.3.0,<2.0.0)
@@ -17,14 +17,14 @@
 [MIDI](https://en.wikipedia.org/wiki/MIDI)-based event loops. It is designed
 for creatives who want to explore the Python ecosystem and experiment with
 music and, for example, machine learning. For examples and tutorials of how to
 use `iipyper`, see our [examples repo](https://github.com/intelligent-
 instruments-lab/iil-examples) (TBC). ## Install `iipyper` can be installed via
 [PyPI](https://pypi.org/project/iipyper): ```sh pip install iipyper ``` ##
 Develop ```sh git clone git@github.com:Intelligent-Instruments-Lab/iipyper.git
-pip install -e iipyper ``` ## Contact `iipyper` is developed by the
+cd iipyper poetry install iipyper ``` ## Contact `iipyper` is developed by the
 [Intelligent Instruments Lab](https://iil.is/about). Get in touch to
 [collaborate](https://iil.is/collaborate): â¦ _i_i_l_._i_s â¦ _F_a_c_e_b_o_o_k â¦
 _I_n_s_t_a_g_r_a_m â¦ _X_ _(_T_w_i_t_t_e_r_) â¦ _Y_o_u_T_u_b_e â¦ _D_i_s_c_o_r_d â¦ _G_i_t_H_u_b â¦ _L_i_n_k_e_d_I_n â¦
 _E_m_a_i_l â¦ ## Funding The Intelligent Instruments project (INTENT) is funded by
 the European Research Council (ERC) under the European Unionâs Horizon 2020
 research and innovation programme (Grant agreement No. 101001848).
```

