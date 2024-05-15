# Comparing `tmp/ucam_faas-0.1.2.tar.gz` & `tmp/ucam_faas-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam_faas-0.1.2.tar", max compression
+gzip compressed data, was "ucam_faas-0.4.1.tar", max compression
```

## Comparing `ucam_faas-0.1.2.tar` & `ucam_faas-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     3834 2024-04-22 13:48:04.561369 ucam_faas-0.1.2/README.md
--rw-r--r--   0        0        0     2616 2024-05-07 14:41:56.615617 ucam_faas-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6088 2024-05-07 14:54:14.597728 ucam_faas-0.1.2/ucam_faas/__init__.py
--rw-r--r--   0        0        0      348 2024-05-07 14:54:14.597728 ucam_faas-0.1.2/ucam_faas/testing.py
--rw-r--r--   0        0        0        0 2024-05-08 10:34:54.471645 ucam_faas-0.1.2/ucam_faas/tests/__init__.py
--rw-r--r--   0        0        0      526 2024-04-15 16:20:03.808097 ucam_faas-0.1.2/ucam_faas/tests/test_ucam_faas.py
--rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 ucam_faas-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3834 2024-04-22 13:48:02.497353 ucam_faas-0.4.1/README.md
+-rw-r--r--   0        0        0     3131 2024-05-15 15:44:32.120793 ucam_faas-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7220 2024-05-14 20:50:10.382759 ucam_faas-0.4.1/ucam_faas/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-13 15:59:51.022836 ucam_faas-0.4.1/ucam_faas/exceptions.py
+-rw-r--r--   0        0        0      581 2024-05-14 20:50:10.382759 ucam_faas-0.4.1/ucam_faas/testing.py
+-rw-r--r--   0        0        0        0 2024-05-15 18:04:14.574051 ucam_faas-0.4.1/ucam_faas/tests/__init__.py
+-rw-r--r--   0        0        0     2557 2024-05-15 12:27:32.119929 ucam_faas-0.4.1/ucam_faas/tests/test_ucam_faas.py
+-rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 ucam_faas-0.4.1/PKG-INFO
```

### Comparing `ucam_faas-0.1.2/README.md` & `ucam_faas-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ucam_faas-0.1.2/pyproject.toml` & `ucam_faas-0.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ucam-faas"
-version = "0.1.2"
+version = "0.4.1"
 description = "Opinionated FaaS support framework extending Google's functions-framework"
 authors = ["University of Cambridge Information Services <devops-wilson@uis.cam.ac.uk>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.developers.cam.ac.uk/uis/devops/ucam-faas-python/ucam-faas"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -48,34 +48,51 @@
 
 [tool.poe.tasks."tox:local"]
 help = "Run the Python test suite via tox using the locally installed Python version"
 cmd = "tox"
 
 [tool.poe.tasks."pytest:local"]
 help = "Run the Python test suite via pytest using the locally installed Python version"
-cmd = "pytest example/tests.py"
+cmd = "pytest"
+
+[tool.poe.tasks."terraform:auth"]
+cmd = "gcloud auth application-default login"
+
+[tool.poe.tasks."terraform:dev:init"]
+cmd = "logan --workspace=development terraform init"
+cwd = "terraform"
+
+[tool.poe.tasks."terraform:dev:apply"]
+cmd = "logan --workspace=development terraform apply"
+cwd = "terraform"
+
+[tool.poe.tasks."terraform:dev"]
+cmd = "logan --workspace=development terraform"
+cwd = "terraform"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.9.1"
 requests = "^2.31.0"
 structlog = "^24.1.0"
 functions-framework = "^3.5.0"
 click = "^8.1.7"
 gunicorn = "^22.0.0"
 flask = "^3.0.3"
 pytest = {version = "^8.1.1", optional = true}
-cloudevents = "^1.10.1"
+polyfactory = {version = "^2.16.0", optional = true}
+cloudevents = {extras = ["pydantic"], version = "^1.10.1"}
+ucam-observe = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
 tox = "^4.14.2"
 
 [tool.poetry.extras]
-testing = ["pytest"]
+testing = ["pytest", "polyfactory"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `ucam_faas-0.1.2/ucam_faas/__init__.py` & `ucam_faas-0.4.1/ucam_faas/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,65 @@
 import click
 import flask
 import functions_framework
 import gunicorn.app.base
 import structlog
 from cloudevents.http.event import CloudEvent
 from gunicorn.config import get_default_config_file
+from ucam_observe import get_structlog_logger
+from werkzeug.exceptions import InternalServerError
+
+from .exceptions import UCAMFAASException
+
+logger = get_structlog_logger(__name__)
+
+
+def _common_function_wrapper(function):
+    def _common_function_wrapper_internal(*args, **kwargs):
+        try:
+            return function(*args, **kwargs)
+        except UCAMFAASException as exception:
+            exception_name = exception.__class__.__name__
+
+            logger.warning("function_failed_gracefully", exception_name=exception_name)
+
+            raise InternalServerError(description=f"The function raised {exception_name}.")
+
+        except Exception as exception:
+            exception_name = exception.__class__.__name__
+
+            logger.error("function_failed_uncaught_exception", exception_name=exception_name)
+
+            # FIXME dump stack trace into logs for unhandled exception
+
+            raise exception
+
+    return _common_function_wrapper_internal
 
 
 def raw_event(function):
+    @_common_function_wrapper
     def _raw_event_internal(request: flask.Request) -> flask.typing.ResponseReturnValue:
-        return function(request.data)
+        return_value = function(request.data)
+
+        if return_value is not None:
+            return return_value
+
+        return "", 200
 
     _raw_event_internal.__name__ = function.__name__
     _raw_event_internal = functions_framework.http(_raw_event_internal)
 
     _raw_event_internal.__wrapped__ = function
+
     return _raw_event_internal
 
 
 def cloud_event(function):
+    @_common_function_wrapper
     def _cloud_event_internal(event: CloudEvent) -> None:
         return function(event.data)
 
     _cloud_event_internal.__name__ = function.__name__
     _cloud_event_internal = functions_framework.cloud_event(_cloud_event_internal)
 
     _cloud_event_internal.__wrapped__ = function
```

### Comparing `ucam_faas-0.1.2/PKG-INFO` & `ucam_faas-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: ucam-faas
-Version: 0.1.2
+Version: 0.4.1
 Summary: Opinionated FaaS support framework extending Google's functions-framework
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/ucam-faas-python/ucam-faas
 License: MIT
 Author: University of Cambridge Information Services
 Author-email: devops-wilson@uis.cam.ac.uk
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: testing
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: cloudevents (>=1.10.1,<2.0.0)
+Requires-Dist: cloudevents[pydantic] (>=1.10.1,<2.0.0)
 Requires-Dist: flask (>=3.0.3,<4.0.0)
 Requires-Dist: functions-framework (>=3.5.0,<4.0.0)
 Requires-Dist: gunicorn (>=22.0.0,<23.0.0)
+Requires-Dist: polyfactory (>=2.16.0,<3.0.0) ; extra == "testing"
 Requires-Dist: pytest (>=8.1.1,<9.0.0) ; extra == "testing"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
+Requires-Dist: ucam-observe (>=0.1.1,<0.2.0)
 Project-URL: Repository, https://gitlab.developers.cam.ac.uk/uis/devops/ucam-faas-python/ucam-faas
 Description-Content-Type: text/markdown
 
 # UCam FaaS Library
 
 This project contains a support library and base Docker image to be used to
 create Function as a Service (FaaS) applications intended to be deployed to a
```

