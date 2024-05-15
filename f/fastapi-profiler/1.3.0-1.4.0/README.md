# Comparing `tmp/fastapi_profiler-1.3.0-py3-none-any.whl.zip` & `tmp/fastapi_profiler-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4421 bytes, number of entries: 8
--rwxrwxrwx  2.0 unx       99 b- defN 24-Mar-04 09:18 fastapi_profiler/__init__.py
--rwxrwxrwx  2.0 unx       51 b- defN 24-Mar-04 09:18 fastapi_profiler/_version.py
--rwxrwxrwx  2.0 unx     6039 b- defN 24-Mar-04 09:18 fastapi_profiler/profiler.py
--rwxrwxrwx  2.0 unx     1063 b- defN 24-Mar-04 09:19 fastapi_profiler-1.3.0.dist-info/LICENSE
--rwxrwxrwx  2.0 unx      974 b- defN 24-Mar-04 09:19 fastapi_profiler-1.3.0.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 24-Mar-04 09:19 fastapi_profiler-1.3.0.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       17 b- defN 24-Mar-04 09:19 fastapi_profiler-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      681 b- defN 24-Mar-04 09:19 fastapi_profiler-1.3.0.dist-info/RECORD
-8 files, 9016 bytes uncompressed, 3215 bytes compressed:  64.3%
+Zip file size: 4521 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      101 b- defN 24-May-14 07:48 fastapi_profiler/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 24-May-14 07:55 fastapi_profiler/_version.py
+-rw-rw-rw-  2.0 fat     6935 b- defN 24-May-14 07:49 fastapi_profiler/profiler.py
+-rw-rw-rw-  2.0 fat     1084 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1001 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      683 b- defN 24-May-14 07:56 fastapi_profiler-1.4.0.dist-info/RECORD
+8 files, 9966 bytes uncompressed, 3315 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: fastapi_profiler/_version.py
 Comment: 
 
 Filename: fastapi_profiler/profiler.py
 Comment: 
 
-Filename: fastapi_profiler-1.3.0.dist-info/LICENSE
+Filename: fastapi_profiler-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_profiler-1.3.0.dist-info/METADATA
+Filename: fastapi_profiler-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_profiler-1.3.0.dist-info/WHEEL
+Filename: fastapi_profiler-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_profiler-1.3.0.dist-info/top_level.txt
+Filename: fastapi_profiler-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fastapi_profiler-1.3.0.dist-info/RECORD
+Filename: fastapi_profiler-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_profiler/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-from ._version import __version__, __author__
-from .profiler import PyInstrumentProfilerMiddleware
+from ._version import __version__, __author__
+from .profiler import PyInstrumentProfilerMiddleware
```

## fastapi_profiler/_version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "1.3.0"
-__author__ = "sunhailin-Leo"
+__version__ = "1.4.0"
+__author__ = "sunhailin-Leo"
```

## fastapi_profiler/profiler.py

```diff
@@ -1,160 +1,175 @@
-import os
-import time
-import codecs
-import cProfile
-from io import StringIO
-from typing import Optional
-from logging import getLogger
-
-from pyinstrument import Profiler
-from pyinstrument.renderers import HTMLRenderer, JSONRenderer
-
-from starlette.routing import Router
-from starlette.requests import Request
-from starlette.types import ASGIApp, Message, Receive, Scope, Send
-
-
-logger = getLogger("profiler")
-
-
-class PyInstrumentProfilerMiddleware:
-    DEFAULT_HTML_FILENAME = "./fastapi-profiler.html"
-    DEFAULT_PROF_FILENAME = "./fastapi-profiler.prof"
-    DEFAULT_JSON_FILENAME = "./fastapi-profiler.json"
-
-    def __init__(
-        self,
-        app: ASGIApp,
-        *,
-        server_app: Optional[Router] = None,
-        profiler_interval: float = 0.0001,
-        profiler_output_type: str = "text",
-        is_print_each_request: bool = True,
-        async_mode: str = "enabled",
-        html_file_name: Optional[str] = None,
-        prof_file_name: Optional[str] = None,
-        open_in_browser: bool = False,
-        **profiler_kwargs,
-    ):
-        self.app = app
-        self._output_type = profiler_output_type
-        self._print_each_request = is_print_each_request
-        self._html_file_name: Optional[str] = html_file_name
-        self._prof_file_name: Optional[str] = prof_file_name
-        self._open_in_browser: bool = open_in_browser
-        self._profiler_kwargs: dict = profiler_kwargs
-
-        if profiler_output_type == "html" and server_app is None:
-            raise RuntimeError(
-                "If profiler_output_type=html, must provide server_app argument "
-                "to set shutdown event handler to output profile."
-            )
-
-        if profiler_output_type == "prof":
-            self._profiler = cProfile.Profile()
-            self._start_profiler = self._profiler.enable
-            self._stop_profiler = self._profiler.disable
-        else:
-            self._profiler = Profiler(interval=profiler_interval, async_mode=async_mode)
-            self._start_profiler = self._profiler.start
-            self._stop_profiler = self._profiler.stop
-
-        # register an event handler for profiler stop
-        if server_app is not None:
-            server_app.add_event_handler("shutdown", self.get_profiler_result)
-
-    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        if scope["type"] != "http":
-            await self.app(scope, receive, send)
-            return
-
-        self._start_profiler()
-
-        request = Request(scope, receive=receive)
-        method = request.method
-        path = request.url.path
-        begin = time.perf_counter()
-
-        # Default status code used when the application does not return a valid response
-        # or an unhandled exception occurs.
-        status_code = 500
-
-        async def wrapped_send(message: Message) -> None:
-            if message["type"] == "http.response.start":
-                nonlocal status_code
-                status_code = message["status"]
-            await send(message)
-
-        try:
-            await self.app(scope, receive, wrapped_send)
-        finally:
-            if scope["type"] == "http":
-                self._stop_profiler()
-                end = time.perf_counter()
-                if self._print_each_request:
-                    print(
-                        f"Method: {method}, "
-                        f"Path: {path}, "
-                        f"Duration: {end - begin}, "
-                        f"Status: {status_code}"
-                    )
-
-                    if self._output_type == "prof":
-                        s = StringIO()
-                        self._profiler.print_stats(stream=s)
-                        print(s.getvalue())
-                    else:
-                        print(self._profiler.output_text(**self._profiler_kwargs))
-
-    async def get_profiler_result(self):
-        if self._output_type == "text":
-            logger.info("Compiling and printing final profile")
-            print(self._profiler.output_text(**self._profiler_kwargs))
-        elif self._output_type == "html":
-            html_file_name = self.DEFAULT_HTML_FILENAME
-            if self._html_file_name is not None:
-                html_file_name = self._html_file_name
-
-            logger.info(
-                "Compiling and dumping final profile to %r - this may take some time",
-                html_file_name,
-            )
-
-            renderer = HTMLRenderer()
-            if self._open_in_browser:
-                renderer.open_in_browser(
-                    session=self._profiler.last_session,
-                    output_filename=os.path.abspath(html_file_name),
-                )
-            else:
-                html_code = renderer.render(session=self._profiler.last_session)
-                with codecs.open(html_file_name, "w", "utf-8") as f:
-                    f.write(html_code)
-
-            logger.info("Done writing profile to %r", html_file_name)
-        elif self._output_type == "prof":
-            prof_file_name = self.DEFAULT_PROF_FILENAME
-            if self._prof_file_name is not None:
-                prof_file_name = self._prof_file_name
-
-            logger.info(
-                "Compiling and dumping final profile to %r - this may take some time",
-                prof_file_name,
-            )
-
-            self._profiler.dump_stats(prof_file_name)
-            logger.info("Done writing profile to %r", prof_file_name)
-        elif self._output_type == "json":
-            prof_file_name = self.DEFAULT_JSON_FILENAME
-            if self._prof_file_name is not None:
-                prof_file_name = self._prof_file_name
-
-            logger.info(
-                "Compiling and dumping final profile to %r - this may take some time",
-                prof_file_name,
-            )
-
-            renderer = JSONRenderer()
-            with codecs.open(prof_file_name, "w", "utf-8") as f:
-                f.write(renderer.render(session=self._profiler.last_session))
-            logger.info("Done writing profile to %r", prof_file_name)
+import os
+import time
+import codecs
+import cProfile
+from io import StringIO
+from typing import Optional
+from logging import getLogger
+
+from pyinstrument import Profiler
+from pyinstrument.renderers import HTMLRenderer, JSONRenderer, SpeedscopeRenderer
+
+from starlette.routing import Router
+from starlette.requests import Request
+from starlette.types import ASGIApp, Message, Receive, Scope, Send
+
+
+logger = getLogger("profiler")
+
+
+class PyInstrumentProfilerMiddleware:
+    DEFAULT_HTML_FILENAME = "./fastapi-profiler.html"
+    DEFAULT_PROF_FILENAME = "./fastapi-profiler.prof"
+    DEFAULT_JSON_FILENAME = "./fastapi-profiler.json"
+    DEFAULT_SPEEDSCOPE_FILENAME = "./fastapi-profiler-speedscope.json"
+
+    def __init__(
+        self,
+        app: ASGIApp,
+        *,
+        server_app: Optional[Router] = None,
+        profiler_interval: float = 0.0001,
+        profiler_output_type: str = "text",
+        is_print_each_request: bool = True,
+        async_mode: str = "enabled",
+        html_file_name: Optional[str] = None,
+        prof_file_name: Optional[str] = None,
+        open_in_browser: bool = False,
+        **profiler_kwargs,
+    ):
+        self.app = app
+        self._output_type = profiler_output_type
+        self._print_each_request = is_print_each_request
+        self._html_file_name: Optional[str] = html_file_name
+        self._prof_file_name: Optional[str] = prof_file_name
+        self._open_in_browser: bool = open_in_browser
+        self._profiler_kwargs: dict = profiler_kwargs
+
+        if profiler_output_type == "html" and server_app is None:
+            raise RuntimeError(
+                "If profiler_output_type=html, must provide server_app argument "
+                "to set shutdown event handler to output profile."
+            )
+
+        if profiler_output_type == "prof":
+            self._profiler = cProfile.Profile()
+            self._start_profiler = self._profiler.enable
+            self._stop_profiler = self._profiler.disable
+        else:
+            self._profiler = Profiler(interval=profiler_interval, async_mode=async_mode)
+            self._start_profiler = self._profiler.start
+            self._stop_profiler = self._profiler.stop
+
+        # register an event handler for profiler stop
+        if server_app is not None:
+            server_app.add_event_handler("shutdown", self.get_profiler_result)
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
+        if scope["type"] != "http":
+            await self.app(scope, receive, send)
+            return
+
+        self._start_profiler()
+
+        request = Request(scope, receive=receive)
+        method = request.method
+        path = request.url.path
+        begin = time.perf_counter()
+
+        # Default status code used when the application does not return a valid response
+        # or an unhandled exception occurs.
+        status_code = 500
+
+        async def wrapped_send(message: Message) -> None:
+            if message["type"] == "http.response.start":
+                nonlocal status_code
+                status_code = message["status"]
+            await send(message)
+
+        try:
+            await self.app(scope, receive, wrapped_send)
+        finally:
+            if scope["type"] == "http":
+                self._stop_profiler()
+                end = time.perf_counter()
+                if self._print_each_request:
+                    print(
+                        f"Method: {method}, "
+                        f"Path: {path}, "
+                        f"Duration: {end - begin}, "
+                        f"Status: {status_code}"
+                    )
+
+                    if self._output_type == "prof":
+                        s = StringIO()
+                        self._profiler.print_stats(stream=s)
+                        print(s.getvalue())
+                    else:
+                        print(self._profiler.output_text(**self._profiler_kwargs))
+
+    async def get_profiler_result(self):
+        if self._output_type == "text":
+            logger.info("Compiling and printing final profile")
+            print(self._profiler.output_text(**self._profiler_kwargs))
+        elif self._output_type == "html":
+            html_file_name = self.DEFAULT_HTML_FILENAME
+            if self._html_file_name is not None:
+                html_file_name = self._html_file_name
+
+            logger.info(
+                "Compiling and dumping final profile to %r - this may take some time",
+                html_file_name,
+            )
+
+            renderer = HTMLRenderer()
+            if self._open_in_browser:
+                renderer.open_in_browser(
+                    session=self._profiler.last_session,
+                    output_filename=os.path.abspath(html_file_name),
+                )
+            else:
+                html_code = renderer.render(session=self._profiler.last_session)
+                with codecs.open(html_file_name, "w", "utf-8") as f:
+                    f.write(html_code)
+
+            logger.info("Done writing profile to %r", html_file_name)
+        elif self._output_type == "prof":
+            prof_file_name = self.DEFAULT_PROF_FILENAME
+            if self._prof_file_name is not None:
+                prof_file_name = self._prof_file_name
+
+            logger.info(
+                "Compiling and dumping final profile to %r - this may take some time",
+                prof_file_name,
+            )
+
+            self._profiler.dump_stats(prof_file_name)
+            logger.info("Done writing profile to %r", prof_file_name)
+        elif self._output_type == "json":
+            prof_file_name = self.DEFAULT_JSON_FILENAME
+            if self._prof_file_name is not None:
+                prof_file_name = self._prof_file_name
+
+            logger.info(
+                "Compiling and dumping final profile to %r - this may take some time",
+                prof_file_name,
+            )
+
+            renderer = JSONRenderer()
+            with codecs.open(prof_file_name, "w", "utf-8") as f:
+                f.write(renderer.render(session=self._profiler.last_session))
+            logger.info("Done writing profile to %r", prof_file_name)
+        elif self._output_type == "speedscope":
+            prof_file_name = self.DEFAULT_SPEEDSCOPE_FILENAME
+            if self._prof_file_name is not None:
+                prof_file_name = self._prof_file_name
+
+            logger.info(
+                "Compiling and dumping final profile to %r - this may take some time",
+                prof_file_name,
+            )
+
+            renderer = SpeedscopeRenderer()
+            with codecs.open(prof_file_name, "w", "utf-8") as f:
+                f.write(renderer.render(session=self._profiler.last_session))
+            logger.info("Done writing profile to %r", prof_file_name)
```

## Comparing `fastapi_profiler-1.3.0.dist-info/METADATA` & `fastapi_profiler-1.4.0.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
-Name: fastapi-profiler
-Version: 1.3.0
-Summary: A FastAPI Middleware of pyinstrument to check your service performance.
-Home-page: https://github.com/sunhailin-Leo/fastapi_profiler
-Author: sunhailin-Leo
-Author-email: 379978424@qq.com
-License: MIT
-Keywords: fastapi,pyinstrument,profiler
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries
-License-File: LICENSE
-Requires-Dist: fastapi
-Requires-Dist: pyinstrument >=4.4.0
-
+Metadata-Version: 2.1
+Name: fastapi-profiler
+Version: 1.4.0
+Summary: A FastAPI Middleware of pyinstrument to check your service performance.
+Home-page: https://github.com/sunhailin-Leo/fastapi_profiler
+Author: sunhailin-Leo
+Author-email: 379978424@qq.com
+License: MIT
+Keywords: fastapi,pyinstrument,profiler
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+Requires-Dist: fastapi
+Requires-Dist: pyinstrument (>=4.4.0)
+
```

