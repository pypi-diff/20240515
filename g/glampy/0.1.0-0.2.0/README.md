# Comparing `tmp/glampy-0.1.0.tar.gz` & `tmp/glampy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glampy-0.1.0.tar", max compression
+gzip compressed data, was "glampy-0.2.0.tar", max compression
```

## Comparing `glampy-0.1.0.tar` & `glampy-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      696 2024-05-15 08:15:37.279274 glampy-0.1.0/README.md
--rw-r--r--   0        0        0       84 2024-05-15 08:15:37.279274 glampy-0.1.0/glampy/__init__.py
--rw-r--r--   0        0        0     2985 2024-05-15 08:15:37.279274 glampy-0.1.0/glampy/logger.py
--rw-r--r--   0        0        0      634 2024-05-15 08:15:37.279274 glampy-0.1.0/glampy/style.py
--rw-r--r--   0        0        0      502 2024-05-15 08:15:37.279274 glampy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 glampy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      696 2024-05-15 12:29:06.235592 glampy-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 12:29:06.235592 glampy-0.2.0/glampy/__init__.py
+-rw-r--r--   0        0        0     2304 2024-05-15 12:29:06.235592 glampy-0.2.0/glampy/io.py
+-rw-r--r--   0        0        0     3884 2024-05-15 12:29:06.235592 glampy-0.2.0/glampy/logging.py
+-rw-r--r--   0        0        0     1291 2024-05-15 12:29:06.235592 glampy-0.2.0/glampy/style.py
+-rw-r--r--   0        0        0      525 2024-05-15 12:29:06.235592 glampy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 glampy-0.2.0/PKG-INFO
```

### Comparing `glampy-0.1.0/README.md` & `glampy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `glampy-0.1.0/glampy/logger.py` & `glampy-0.2.0/glampy/logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,51 @@
 """This module contains logger related utilities."""
 
 from __future__ import annotations
 import logging
 import os
 
 from sys import stdout
-from . import style
+from .style import Foreground_Colour, Style
+
+
+class Formatter(logging.Formatter):
+    """An opinionated formatter for logging messages."""
+
+    def format(self, record: logging.LogRecord):
+        """Formats the log record with colours based on the log level.
+
+        Args:
+            record: The log record to format.
+        """
+        color = {
+            logging.WARNING: Foreground_Colour.YELLOW,
+            logging.ERROR: Foreground_Colour.RED,
+            logging.FATAL: Foreground_Colour.RED,
+            logging.INFO: Foreground_Colour.GREEN,
+            logging.DEBUG: Foreground_Colour.CYAN,
+        }.get(record.levelno, 0)
+        # pylint: disable=protected-access
+        self._style._fmt = f"{color}%(levelname)s{Style.RESET_ALL}: %(message)s"
+        return super().format(record)
 
 
 class Logger:
     """A generic logger class allowing logs to be send to stdout and a log file.
 
     Attributes:
         logger: The logger object.
     """
 
     def __init__(
         self,
         log_name: str,
         log_file: None | str = None,
         log_level: int = logging.CRITICAL,
-        log_format: str = "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+        log_format: str | logging.Formatter | None = None,
     ):
         """Initializes the logger.
 
         Args:
             log_name: A name for the logger, allowing differentiating between logs.
             log_file: The path to the log file.
             log_level: The level threshold of the logs to be displayed.
@@ -36,40 +57,46 @@
         Example using the Logger class to log to stdout only:
         >>> logger = Logger("my_logger", log_level=logging.DEBUG)
         """
         self.logger = logging.getLogger(log_name)
         self.logger.setLevel(log_level)
         console_handler = logging.StreamHandler(stdout)
 
-        console_handler.setFormatter(logging.Formatter(log_format))
+        if isinstance(log_format, logging.Formatter):
+            formatter = log_format
+        elif isinstance(log_format, str):
+            formatter = logging.Formatter(log_format)
+        else:
+            formatter = Formatter()
+        console_handler.setFormatter(formatter)
         self.logger.addHandler(console_handler)
 
         if log_file:
             log_dir = os.path.dirname(log_file)
             if not os.path.exists(log_dir) and len(log_dir.strip()) > 0:
                 os.makedirs(log_dir, exist_ok=True)
             file_handler = logging.FileHandler(log_file, mode="w")
-            file_handler.setFormatter(logging.Formatter(log_format))
+            file_handler.setFormatter(formatter)
             self.logger.addHandler(file_handler)
 
     def _log(self, msg: str, level: str) -> None:
         """Logs a message with a given level.
 
         Args:
             msg: The message to log.
             level: The level of the message.
         """
         if level == "info":
             self.logger.info(msg)
         if level == "debug":
             self.logger.debug(msg)
         if level == "warning":
-            self.logger.warning("%s%s", style.Color.WARNING, msg)
+            self.logger.warning(msg)
         if level == "error":
-            self.logger.error("%s%s", style.Color.ERROR, msg)
+            self.logger.error(msg)
 
     def debug(self, msg: str) -> None:
         """Logs a debug message.
 
         Args:
             msg: The message to log.
         """
```

### Comparing `glampy-0.1.0/PKG-INFO` & `glampy-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glampy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Make your python CLI prints and logs simple but glamorous
 License: MIT
 Author: snaeil
 Author-email: schnegel@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

