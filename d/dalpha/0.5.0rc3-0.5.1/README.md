# Comparing `tmp/dalpha-0.5.0rc3.tar.gz` & `tmp/dalpha-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.0rc3.tar", max compression
+gzip compressed data, was "dalpha-0.5.1.tar", max compression
```

## Comparing `dalpha-0.5.0rc3.tar` & `dalpha-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.0rc3/README.md
--rw-r--r--   0        0        0     1966 2024-05-11 06:19:40.367843 dalpha-0.5.0rc3/dalpha/__init__.py
--rw-r--r--   0        0        0     8194 2024-05-13 09:40:01.895738 dalpha-0.5.0rc3/dalpha/agent.py
--rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.0rc3/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.0rc3/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.0rc3/dalpha/dto.py
--rw-r--r--   0        0        0      579 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/exception.py
--rw-r--r--   0        0        0     6022 2024-05-13 09:17:22.448483 dalpha-0.5.0rc3/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.0rc3/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.0rc3/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.0rc3/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.0rc3/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.0rc3/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/request.py
--rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/signal_handler.py
--rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/slack.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-05-13 09:40:01.895738 dalpha-0.5.0rc3/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.1/README.md
+-rw-r--r--   0        0        0     2028 2024-05-15 07:56:58.860556 dalpha-0.5.1/dalpha/__init__.py
+-rw-r--r--   0        0        0     8194 2024-05-13 09:40:01.895738 dalpha-0.5.1/dalpha/agent.py
+-rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.1/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.1/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.1/dalpha/dto.py
+-rw-r--r--   0        0        0      579 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/exception.py
+-rw-r--r--   0        0        0     6022 2024-05-13 09:17:22.448483 dalpha-0.5.1/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.1/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.1/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.1/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.1/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.1/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/slack.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/update_agent.py
+-rw-r--r--   0        0        0      946 2024-05-15 07:56:58.860556 dalpha-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 dalpha-0.5.1/PKG-INFO
```

### Comparing `dalpha-0.5.0rc3/README.md` & `dalpha-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/__init__.py` & `dalpha-0.5.1/dalpha/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     with open(file_path, 'r') as file:
         lines = file.readlines()
     
     for line in lines:
         line = line.strip()
         if line and not line.startswith("#"):
             key, value = line.split("=")
-            if os.environ.get(key) is None:
+            if bool(os.environ.get("DEV_SERVER", 'True') == 'True') or os.environ.get(key) is None:
                 os.environ[key] = value
 
 
 def check_package_version(package_name):
     installed_version = pkg_resources.get_distribution(package_name).version
     try:
         url = f"https://pypi.org/pypi/{package_name}/json"
@@ -47,8 +47,8 @@
 from dalpha.agent import Agent
 from dalpha.cobra_cls import Cobra
 from dalpha.data_update_cls import DalphaDataUpdater
 from dalpha.inference_cls import DalphaAI
 from dalpha.redis_cls import DalphaRedis
 from dalpha.openai_cls import DalphaOpenAI
 from dalpha.backend_cli import BackendCli, internal_call
-import dalpha.s3
+import dalpha.s3 as s3
```

### Comparing `dalpha-0.5.0rc3/dalpha/agent.py` & `dalpha-0.5.1/dalpha/agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/backend_cli.py` & `dalpha-0.5.1/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/cobra_cls.py` & `dalpha-0.5.1/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/context.py` & `dalpha-0.5.1/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/data_update_cls.py` & `dalpha-0.5.1/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/dto.py` & `dalpha-0.5.1/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/exception.py` & `dalpha-0.5.1/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/inference_cls.py` & `dalpha-0.5.1/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/logging/__init__.py` & `dalpha-0.5.1/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/logging/log_formatter.py` & `dalpha-0.5.1/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/logging/utils.py` & `dalpha-0.5.1/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/message_consumer.py` & `dalpha-0.5.1/dalpha/message_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/openai_cls.py` & `dalpha-0.5.1/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/redis_cli.py` & `dalpha-0.5.1/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/redis_cls.py` & `dalpha-0.5.1/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/request.py` & `dalpha-0.5.1/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/s3.py` & `dalpha-0.5.1/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/slack.py` & `dalpha-0.5.1/dalpha/slack.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/dalpha/update_agent.py` & `dalpha-0.5.1/dalpha/update_agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc3/pyproject.toml` & `dalpha-0.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.5.0rc3"
+version = "0.5.1"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,15 +17,15 @@
 pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.5.0rc3"
+version = "0.5.1"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
   { name="Gideok", email="gideok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `dalpha-0.5.0rc3/PKG-INFO` & `dalpha-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.0rc3
+Version: 0.5.1
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

