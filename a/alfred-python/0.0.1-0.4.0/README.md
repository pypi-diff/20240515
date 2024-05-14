# Comparing `tmp/alfred_python-0.0.1.tar.gz` & `tmp/alfred_python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred_python-0.0.1.tar", last modified: Thu Apr 18 16:16:44 2024, max compression
+gzip compressed data, was "alfred_python-0.4.0.tar", last modified: Tue May 14 23:43:37 2024, max compression
```

## Comparing `alfred_python-0.0.1.tar` & `alfred_python-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,50 @@
-drwxr-xr-x   0 raulroa    (501) staff       (20)        0 2024-04-18 16:16:44.784742 alfred_python-0.0.1/
--rw-r--r--   0 raulroa    (501) staff       (20)     1073 2024-04-18 16:06:17.000000 alfred_python-0.0.1/LICENSE
--rw-r--r--   0 raulroa    (501) staff       (20)     1157 2024-04-18 16:16:44.784541 alfred_python-0.0.1/PKG-INFO
--rw-r--r--   0 raulroa    (501) staff       (20)      657 2024-04-18 16:03:44.000000 alfred_python-0.0.1/README.md
-drwxr-xr-x   0 raulroa    (501) staff       (20)        0 2024-04-18 16:16:44.784344 alfred_python-0.0.1/alfred_python.egg-info/
--rw-r--r--   0 raulroa    (501) staff       (20)     1157 2024-04-18 16:16:44.000000 alfred_python-0.0.1/alfred_python.egg-info/PKG-INFO
--rw-r--r--   0 raulroa    (501) staff       (20)      329 2024-04-18 16:16:44.000000 alfred_python-0.0.1/alfred_python.egg-info/SOURCES.txt
--rw-r--r--   0 raulroa    (501) staff       (20)        1 2024-04-18 16:16:44.000000 alfred_python-0.0.1/alfred_python.egg-info/dependency_links.txt
--rw-r--r--   0 raulroa    (501) staff       (20)        4 2024-04-18 16:16:44.000000 alfred_python-0.0.1/alfred_python.egg-info/top_level.txt
-drwxr-xr-x   0 raulroa    (501) staff       (20)        0 2024-04-18 16:16:44.783339 alfred_python-0.0.1/app/
--rw-r--r--   0 raulroa    (501) staff       (20)      511 2024-04-18 16:03:44.000000 alfred_python-0.0.1/app/__init__.py
-drwxr-xr-x   0 raulroa    (501) staff       (20)        0 2024-04-18 16:16:44.783565 alfred_python-0.0.1/app/config/
--rw-r--r--   0 raulroa    (501) staff       (20)       41 2024-04-18 16:03:44.000000 alfred_python-0.0.1/app/config/__init__.py
--rw-r--r--   0 raulroa    (501) staff       (20)      639 2024-04-18 16:03:44.000000 alfred_python-0.0.1/app/config/settings.py
-drwxr-xr-x   0 raulroa    (501) staff       (20)        0 2024-04-18 16:16:44.783942 alfred_python-0.0.1/app/typings/
--rw-r--r--   0 raulroa    (501) staff       (20)       31 2024-04-18 16:03:44.000000 alfred_python-0.0.1/app/typings/__init__.py
--rw-r--r--   0 raulroa    (501) staff       (20)      194 2024-04-18 16:03:44.000000 alfred_python-0.0.1/app/typings/misc.py
-drwxr-xr-x   0 raulroa    (501) staff       (20)        0 2024-04-18 16:16:44.784180 alfred_python-0.0.1/app/utils/
--rw-r--r--   0 raulroa    (501) staff       (20)       32 2024-04-18 16:03:44.000000 alfred_python-0.0.1/app/utils/__init__.py
--rw-r--r--   0 raulroa    (501) staff       (20)     2271 2024-04-18 16:03:44.000000 alfred_python-0.0.1/app/utils/logging.py
--rw-r--r--   0 raulroa    (501) staff       (20)      491 2024-04-18 16:16:40.000000 alfred_python-0.0.1/pyproject.toml
--rw-r--r--   0 raulroa    (501) staff       (20)       38 2024-04-18 16:16:44.784785 alfred_python-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.518888 alfred_python-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 23:43:29.000000 alfred_python-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-14 23:43:37.518888 alfred_python-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-14 23:43:29.000000 alfred_python-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-14 23:43:29.000000 alfred_python-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:43:37.518888 alfred_python-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.510888 alfred_python-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.510888 alfred_python-0.4.0/src/alfred/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.510888 alfred_python-0.4.0/src/alfred/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/base/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/http/typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/data_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/data_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/data_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/data_points/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/files/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/files/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/jobs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/jobs/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/jobs/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/sessions/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.518888 alfred_python-0.4.0/src/alfred/typings/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/typings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/typings/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.518888 alfred_python-0.4.0/src/alfred/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.518888 alfred_python-0.4.0/src/alfred_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/top_level.txt
```

### Comparing `alfred_python-0.0.1/LICENSE` & `alfred_python-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred_python-0.0.1/app/utils/logging.py` & `alfred_python-0.4.0/src/alfred/utils/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # Native imports
 import json
-import socket
 import logging
-from typing import List, Union
+import socket
 from logging.handlers import SysLogHandler
+from typing import Union
 
 # Project imports
-from app.typings import LoggingOptions
+from src.alfred.typings import LoggingOptions
 
 
-def init_loggers(loggers: List[logging.Logger], options: LoggingOptions):
+def setup_logger(options: LoggingOptions):
     """
-    Setup a custom logger with JSON formatting and handler
+    Set up a custom logger with JSON formatting and handler
     based on application environment.
     """
-    env = options.get("env")
+    logger = logging.getLogger("alfred-python")
     name = options.get("name")
     pt_host = options.get("papertrail_host")
     pt_port = options.get("papertrail_port")
+    _format = options.get("format")
 
     class ContextFilter(logging.Filter):
         hostname = socket.gethostname()
 
         def filter(self, record):
             record.hostname = ContextFilter.hostname
             return True
 
     class PapertrailFormatter(logging.Formatter):
         def __init__(
-            self,
-            fmt: Union[str, None] = ...,
-            datefmt: Union[str, None] = ...,
+                self,
+                fmt: Union[str, None] = _format,
+                datefmt: Union[str, None] = ...,
         ) -> None:
-            super().__init__(datefmt=datefmt)
+            super().__init__(datefmt=datefmt, fmt=fmt)
 
         def format(self, record):
             is_text = isinstance(record.msg, (str))
             record.message = record.getMessage() if is_text else record.msg
             record.asctime = self.formatTime(record, self.datefmt)
             record.stack_info = self.formatStack(record.stack_info)
             if record.exc_info:
@@ -44,30 +45,32 @@
                     record.exc_text = self.formatException(record.exc_info)
 
             # Prepare json logging
             data = {"msg": record.message, "level": record.levelname}
             if record.exc_text:
                 data["exception"] = record.exc_text
 
-            return f"{record.asctime} {name} {name}-{env} {json.dumps(data)}"
+            return f"{record.asctime} {name} {json.dumps(data)}"
 
-    # Setup handler based on env
-    if options.get("env") == "dev":
-        handler = logging.StreamHandler()
-    else:
-        handler = SysLogHandler(address=(pt_host, pt_port))
+    # Setup handlers based on env
+    handlers = [logging.StreamHandler()]
+    if pt_host and pt_port:
+        handlers.append(SysLogHandler(address=(pt_host, pt_port)))
 
-    # Add filter to handler
-    handler.addFilter(ContextFilter())
+    # Remove all logger existing handlers
+    logger.handlers = []
 
-    # Setup handler formatter
-    handler.setFormatter(PapertrailFormatter(datefmt="%b %d %H:%M:%S"))
+    # Set logger level
+    logger.setLevel(options["level"])
 
-    for logger in loggers:
-        # Remove all logger existing handlers
-        logger.handlers = []
+    # Set logger handler
+    for handler in handlers:
+        # Add filter to handler
+        handler.addFilter(ContextFilter())
 
-        # Set logger level
-        logger.setLevel(options["level"])
+        # Setup handler formatter
+        handler.setFormatter(PapertrailFormatter(datefmt="%b %d %H:%M:%S"))
 
-        # Set logger handler
+        # Add handler
         logger.addHandler(handler)
+
+    return logger
```

