# Comparing `tmp/codeflash-0.6.0.tar.gz` & `tmp/codeflash-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflash-0.6.0.tar", max compression
+gzip compressed data, was "codeflash-0.6.1.tar", max compression
```

## Comparing `codeflash-0.6.0.tar` & `codeflash-0.6.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0       11 2024-01-05 03:52:06.661399 codeflash-0.6.0/README.md
--rw-r--r--   0        0        0     4405 2024-05-09 02:46:13.702044 codeflash-0.6.0/codeflash/LICENSE
--rw-r--r--   0        0        0        0 2024-02-12 23:19:32.441827 codeflash-0.6.0/codeflash/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.664022 codeflash-0.6.0/codeflash/api/__init__.py
--rw-r--r--   0        0        0     9084 2024-05-10 22:08:41.323160 codeflash-0.6.0/codeflash/api/aiservice.py
--rw-r--r--   0        0        0     4699 2024-05-09 01:04:19.208503 codeflash-0.6.0/codeflash/api/cfapi.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:20.903968 codeflash-0.6.0/codeflash/cli_cmds/__init__.py
--rw-r--r--   0        0        0     8319 2024-05-13 20:50:08.613037 codeflash-0.6.0/codeflash/cli_cmds/cli.py
--rw-r--r--   0        0        0    22865 2024-04-26 00:11:25.877653 codeflash-0.6.0/codeflash/cli_cmds/cmd_init.py
--rw-r--r--   0        0        0      440 2024-04-13 01:39:38.777959 codeflash-0.6.0/codeflash/cli_cmds/logging_config.py
--rw-r--r--   0        0        0     1827 2024-03-22 23:15:30.441796 codeflash-0.6.0/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.665124 codeflash-0.6.0/codeflash/code_utils/__init__.py
--rw-r--r--   0        0        0     9536 2024-05-13 20:50:08.613395 codeflash-0.6.0/codeflash/code_utils/code_extractor.py
--rw-r--r--   0        0        0     8556 2024-05-13 20:50:08.613897 codeflash-0.6.0/codeflash/code_utils/code_replacer.py
--rw-r--r--   0        0        0     2956 2024-05-13 20:50:08.614171 codeflash-0.6.0/codeflash/code_utils/code_utils.py
--rw-r--r--   0        0        0      273 2024-03-09 01:29:18.207924 codeflash-0.6.0/codeflash/code_utils/compat.py
--rw-r--r--   0        0        0      224 2024-02-12 23:19:32.443100 codeflash-0.6.0/codeflash/code_utils/config_consts.py
--rw-r--r--   0        0        0     3908 2024-04-26 00:11:25.877810 codeflash-0.6.0/codeflash/code_utils/config_parser.py
--rw-r--r--   0        0        0     2880 2024-04-26 00:11:25.877913 codeflash-0.6.0/codeflash/code_utils/env_utils.py
--rw-r--r--   0        0        0     2056 2024-05-13 20:50:08.614476 codeflash-0.6.0/codeflash/code_utils/formatter.py
--rw-r--r--   0        0        0     3329 2024-05-13 20:50:08.614854 codeflash-0.6.0/codeflash/code_utils/git_utils.py
--rw-r--r--   0        0        0    23761 2024-05-13 20:50:08.615008 codeflash-0.6.0/codeflash/code_utils/instrument_existing_tests.py
--rw-r--r--   0        0        0      293 2024-05-09 02:00:12.294226 codeflash-0.6.0/codeflash/code_utils/main_calls_bubblesort.py
--rw-r--r--   0        0        0     3497 2024-04-26 00:11:25.878498 codeflash-0.6.0/codeflash/code_utils/shell_utils.py
--rw-r--r--   0        0        0     1007 2024-01-05 03:52:06.666361 codeflash-0.6.0/codeflash/code_utils/sqlalchemy_utils.py
--rw-r--r--   0        0        0     1898 2024-05-13 20:50:08.615426 codeflash-0.6.0/codeflash/code_utils/time_utils.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.666515 codeflash-0.6.0/codeflash/discovery/__init__.py
--rw-r--r--   0        0        0    18567 2024-05-13 20:50:08.615782 codeflash-0.6.0/codeflash/discovery/discover_unit_tests.py
--rw-r--r--   0        0        0    20447 2024-05-13 20:50:08.616245 codeflash-0.6.0/codeflash/discovery/functions_to_optimize.py
--rw-r--r--   0        0        0     1230 2024-04-26 00:11:25.879800 codeflash-0.6.0/codeflash/github/PrComment.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667045 codeflash-0.6.0/codeflash/github/__init__.py
--rw-r--r--   0        0        0      725 2024-04-15 21:39:54.603831 codeflash-0.6.0/codeflash/main.py
--rw-r--r--   0        0        0      133 2024-05-09 01:04:19.209290 codeflash-0.6.0/codeflash/models/ExperimentMetadata.py
--rw-r--r--   0        0        0        0 2024-05-09 01:04:19.209321 codeflash-0.6.0/codeflash/models/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667651 codeflash-0.6.0/codeflash/optimization/__init__.py
--rw-r--r--   0        0        0    11557 2024-05-06 23:55:18.537635 codeflash-0.6.0/codeflash/optimization/function_context.py
--rw-r--r--   0        0        0    53413 2024-05-13 20:50:08.616609 codeflash-0.6.0/codeflash/optimization/optimizer.py
--rw-r--r--   0        0        0    12288 2024-05-06 22:36:52.069428 codeflash-0.6.0/codeflash/output1.trace
--rw-r--r--   0        0        0        0 2024-01-29 22:42:06.720542 codeflash-0.6.0/codeflash/result/__init__.py
--rw-r--r--   0        0        0     4539 2024-05-13 20:50:08.617001 codeflash-0.6.0/codeflash/result/create_pr.py
--rw-r--r--   0        0        0     1992 2024-05-13 20:50:08.617647 codeflash-0.6.0/codeflash/result/explanation.py
--rw-r--r--   0        0        0        0 2024-03-19 03:48:11.207605 codeflash-0.6.0/codeflash/telemetry/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-26 00:11:25.880328 codeflash-0.6.0/codeflash/telemetry/posthog.py
--rw-r--r--   0        0        0      579 2024-03-19 03:48:11.207884 codeflash-0.6.0/codeflash/telemetry/sentry.py
--rw-r--r--   0        0        0    20467 2024-05-13 20:50:08.617770 codeflash-0.6.0/codeflash/tracer.py
--rw-r--r--   0        0        0        1 2024-05-13 20:50:08.617918 codeflash-0.6.0/codeflash/tracing/__init__.py
--rw-r--r--   0        0        0     2644 2024-05-13 20:50:08.618038 codeflash-0.6.0/codeflash/tracing/profile_stats.py
--rw-r--r--   0        0        0     5942 2024-05-13 20:50:08.618326 codeflash-0.6.0/codeflash/tracing/replay_test.py
--rw-r--r--   0        0        0      210 2024-04-26 00:11:25.881219 codeflash-0.6.0/codeflash/tracing/tracing_utils.py
--rw-r--r--   0        0        0     1905 2024-04-26 00:11:25.881455 codeflash-0.6.0/codeflash/update_license_version.py
--rw-r--r--   0        0        0        0 2024-01-19 22:35:16.406336 codeflash-0.6.0/codeflash/verification/__init__.py
--rw-r--r--   0        0        0     4977 2024-05-09 01:04:19.210115 codeflash-0.6.0/codeflash/verification/comparator.py
--rw-r--r--   0        0        0     1139 2024-04-05 00:50:30.445955 codeflash-0.6.0/codeflash/verification/equivalence.py
--rw-r--r--   0        0        0    14621 2024-05-13 20:50:08.618624 codeflash-0.6.0/codeflash/verification/parse_test_output.py
--rw-r--r--   0        0        0     6776 2024-05-13 20:50:08.619311 codeflash-0.6.0/codeflash/verification/test_results.py
--rw-r--r--   0        0        0     1852 2024-05-13 20:50:08.619642 codeflash-0.6.0/codeflash/verification/test_runner.py
--rw-r--r--   0        0        0     2338 2024-04-26 00:11:25.882465 codeflash-0.6.0/codeflash/verification/verification_utils.py
--rw-r--r--   0        0        0     4200 2024-05-10 22:08:41.328788 codeflash-0.6.0/codeflash/verification/verifier.py
--rw-r--r--   0        0        0      150 2024-05-13 21:06:20.912349 codeflash-0.6.0/codeflash/version.py
--rw-r--r--   0        0        0     2910 2024-05-13 21:06:20.911383 codeflash-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 codeflash-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-05 03:52:06.661399 codeflash-0.6.1/README.md
+-rw-r--r--   0        0        0     4405 2024-05-15 02:11:21.869131 codeflash-0.6.1/codeflash/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-12 23:19:32.441827 codeflash-0.6.1/codeflash/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.664022 codeflash-0.6.1/codeflash/api/__init__.py
+-rw-r--r--   0        0        0     9081 2024-05-15 00:58:25.797124 codeflash-0.6.1/codeflash/api/aiservice.py
+-rw-r--r--   0        0        0     4699 2024-05-09 01:04:19.208503 codeflash-0.6.1/codeflash/api/cfapi.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:20.903968 codeflash-0.6.1/codeflash/cli_cmds/__init__.py
+-rw-r--r--   0        0        0     8319 2024-05-15 00:42:51.836406 codeflash-0.6.1/codeflash/cli_cmds/cli.py
+-rw-r--r--   0        0        0    22865 2024-04-26 00:11:25.877653 codeflash-0.6.1/codeflash/cli_cmds/cmd_init.py
+-rw-r--r--   0        0        0      440 2024-04-13 01:39:38.777959 codeflash-0.6.1/codeflash/cli_cmds/logging_config.py
+-rw-r--r--   0        0        0     1827 2024-03-22 23:15:30.441796 codeflash-0.6.1/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.665124 codeflash-0.6.1/codeflash/code_utils/__init__.py
+-rw-r--r--   0        0        0     9536 2024-05-15 00:42:51.836902 codeflash-0.6.1/codeflash/code_utils/code_extractor.py
+-rw-r--r--   0        0        0     8556 2024-05-15 00:42:51.837279 codeflash-0.6.1/codeflash/code_utils/code_replacer.py
+-rw-r--r--   0        0        0     2956 2024-05-15 00:42:51.837580 codeflash-0.6.1/codeflash/code_utils/code_utils.py
+-rw-r--r--   0        0        0      273 2024-03-09 01:29:18.207924 codeflash-0.6.1/codeflash/code_utils/compat.py
+-rw-r--r--   0        0        0      224 2024-02-12 23:19:32.443100 codeflash-0.6.1/codeflash/code_utils/config_consts.py
+-rw-r--r--   0        0        0     3908 2024-04-26 00:11:25.877810 codeflash-0.6.1/codeflash/code_utils/config_parser.py
+-rw-r--r--   0        0        0     2880 2024-04-26 00:11:25.877913 codeflash-0.6.1/codeflash/code_utils/env_utils.py
+-rw-r--r--   0        0        0     2056 2024-05-15 00:42:51.837705 codeflash-0.6.1/codeflash/code_utils/formatter.py
+-rw-r--r--   0        0        0     3329 2024-05-15 00:42:51.838099 codeflash-0.6.1/codeflash/code_utils/git_utils.py
+-rw-r--r--   0        0        0    23761 2024-05-15 00:42:51.838253 codeflash-0.6.1/codeflash/code_utils/instrument_existing_tests.py
+-rw-r--r--   0        0        0      293 2024-05-09 02:00:12.294226 codeflash-0.6.1/codeflash/code_utils/main_calls_bubblesort.py
+-rw-r--r--   0        0        0     3497 2024-04-26 00:11:25.878498 codeflash-0.6.1/codeflash/code_utils/shell_utils.py
+-rw-r--r--   0        0        0     1007 2024-01-05 03:52:06.666361 codeflash-0.6.1/codeflash/code_utils/sqlalchemy_utils.py
+-rw-r--r--   0        0        0     1898 2024-05-15 00:42:51.838521 codeflash-0.6.1/codeflash/code_utils/time_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.666515 codeflash-0.6.1/codeflash/discovery/__init__.py
+-rw-r--r--   0        0        0    18567 2024-05-15 00:42:51.838792 codeflash-0.6.1/codeflash/discovery/discover_unit_tests.py
+-rw-r--r--   0        0        0    20032 2024-05-15 00:42:51.839180 codeflash-0.6.1/codeflash/discovery/functions_to_optimize.py
+-rw-r--r--   0        0        0     1230 2024-04-26 00:11:25.879800 codeflash-0.6.1/codeflash/github/PrComment.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667045 codeflash-0.6.1/codeflash/github/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-15 21:39:54.603831 codeflash-0.6.1/codeflash/main.py
+-rw-r--r--   0        0        0      133 2024-05-09 01:04:19.209290 codeflash-0.6.1/codeflash/models/ExperimentMetadata.py
+-rw-r--r--   0        0        0        0 2024-05-09 01:04:19.209321 codeflash-0.6.1/codeflash/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667651 codeflash-0.6.1/codeflash/optimization/__init__.py
+-rw-r--r--   0        0        0    11557 2024-05-06 23:55:18.537635 codeflash-0.6.1/codeflash/optimization/function_context.py
+-rw-r--r--   0        0        0    54500 2024-05-15 00:42:51.839552 codeflash-0.6.1/codeflash/optimization/optimizer.py
+-rw-r--r--   0        0        0    12288 2024-05-06 22:36:52.069428 codeflash-0.6.1/codeflash/output1.trace
+-rw-r--r--   0        0        0        0 2024-01-29 22:42:06.720542 codeflash-0.6.1/codeflash/result/__init__.py
+-rw-r--r--   0        0        0     4539 2024-05-15 00:42:51.839974 codeflash-0.6.1/codeflash/result/create_pr.py
+-rw-r--r--   0        0        0     1992 2024-05-15 00:42:51.840226 codeflash-0.6.1/codeflash/result/explanation.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:48:11.207605 codeflash-0.6.1/codeflash/telemetry/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-26 00:11:25.880328 codeflash-0.6.1/codeflash/telemetry/posthog.py
+-rw-r--r--   0        0        0      579 2024-03-19 03:48:11.207884 codeflash-0.6.1/codeflash/telemetry/sentry.py
+-rw-r--r--   0        0        0    20467 2024-05-15 00:42:51.840326 codeflash-0.6.1/codeflash/tracer.py
+-rw-r--r--   0        0        0        1 2024-05-15 00:42:51.840456 codeflash-0.6.1/codeflash/tracing/__init__.py
+-rw-r--r--   0        0        0     2644 2024-05-15 00:42:51.840553 codeflash-0.6.1/codeflash/tracing/profile_stats.py
+-rw-r--r--   0        0        0     5942 2024-05-15 00:42:51.840847 codeflash-0.6.1/codeflash/tracing/replay_test.py
+-rw-r--r--   0        0        0      210 2024-04-26 00:11:25.881219 codeflash-0.6.1/codeflash/tracing/tracing_utils.py
+-rw-r--r--   0        0        0     1905 2024-04-26 00:11:25.881455 codeflash-0.6.1/codeflash/update_license_version.py
+-rw-r--r--   0        0        0        0 2024-01-19 22:35:16.406336 codeflash-0.6.1/codeflash/verification/__init__.py
+-rw-r--r--   0        0        0     4977 2024-05-09 01:04:19.210115 codeflash-0.6.1/codeflash/verification/comparator.py
+-rw-r--r--   0        0        0     1241 2024-05-15 00:42:51.841223 codeflash-0.6.1/codeflash/verification/equivalence.py
+-rw-r--r--   0        0        0    14621 2024-05-15 00:42:51.841539 codeflash-0.6.1/codeflash/verification/parse_test_output.py
+-rw-r--r--   0        0        0     6776 2024-05-15 00:42:51.841964 codeflash-0.6.1/codeflash/verification/test_results.py
+-rw-r--r--   0        0        0     1852 2024-05-15 00:42:51.842356 codeflash-0.6.1/codeflash/verification/test_runner.py
+-rw-r--r--   0        0        0     2338 2024-04-26 00:11:25.882465 codeflash-0.6.1/codeflash/verification/verification_utils.py
+-rw-r--r--   0        0        0     4200 2024-05-10 22:08:41.328788 codeflash-0.6.1/codeflash/verification/verifier.py
+-rw-r--r--   0        0        0      150 2024-05-15 02:11:26.530525 codeflash-0.6.1/codeflash/version.py
+-rw-r--r--   0        0        0     2963 2024-05-15 02:11:26.528842 codeflash-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 codeflash-0.6.1/PKG-INFO
```

### Comparing `codeflash-0.6.0/codeflash/LICENSE` & `codeflash-0.6.1/codeflash/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Business Source License 1.1
 
 Parameters
 
 Licensor:             CodeFlash Inc.
-Licensed Work:        Codeflash Client version 0.5.x
+Licensed Work:        Codeflash Client version 0.6.x
                       The Licensed Work is (c) 2024 CodeFlash Inc.
 
 Additional Use Grant: None. Production use of the Licensed Work is only permitted
                       if you have entered into a separate written agreement
                       with CodeFlash Inc. for production use in connection
                       with a subscription to CodeFlash's Code Optimization
                       Platform. Please visit codeflash.ai for further
                       information.
 
-Change Date:          2028-04-11
+Change Date:          2028-05-13
 
 Change License:       MIT
 
 Notice
 
 The Business Source License (this document, or the “License”) is not an Open
 Source license. However, the Licensed Work will eventually be made available
```

### Comparing `codeflash-0.6.0/codeflash/api/aiservice.py` & `codeflash-0.6.1/codeflash/api/aiservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 class AiServiceClient:
     def __init__(self):
         self.base_url = self.get_aiservice_base_url()
         self.headers = {"Authorization": f"Bearer {get_codeflash_api_key()}"}
 
     def get_aiservice_base_url(self) -> str:
         if os.environ.get("CODEFLASH_AIS_SERVER", default="prod").lower() == "local":
-            logging.info("Using local AI Service at http://localhost:8000/")
-            return "http://localhost:8000/"
+            logging.info("Using local AI Service at http://localhost:8000")
+            return "http://localhost:8000"
         return "https://app.codeflash.ai"
 
     def make_ai_service_request(
         self,
         endpoint: str,
         method: str = "POST",
         payload: Optional[Dict[str, Any]] = None,
@@ -224,8 +224,8 @@
                     {"response_status_code": response.status_code, "error": response.text},
                 )
                 return None
 
 
 class LocalAiServiceClient(AiServiceClient):
     def get_aiservice_base_url(self) -> str:
-        return "http://localhost:8000/"
+        return "http://localhost:8000"
```

### Comparing `codeflash-0.6.0/codeflash/api/cfapi.py` & `codeflash-0.6.1/codeflash/api/cfapi.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/cli_cmds/cli.py` & `codeflash-0.6.1/codeflash/cli_cmds/cli.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/cli_cmds/cmd_init.py` & `codeflash-0.6.1/codeflash/cli_cmds/cmd_init.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/cli_cmds/workflows/codeflash-optimize.yaml` & `codeflash-0.6.1/codeflash/cli_cmds/workflows/codeflash-optimize.yaml`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/code_extractor.py` & `codeflash-0.6.1/codeflash/code_utils/code_extractor.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/code_replacer.py` & `codeflash-0.6.1/codeflash/code_utils/code_replacer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/code_utils.py` & `codeflash-0.6.1/codeflash/code_utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/config_parser.py` & `codeflash-0.6.1/codeflash/code_utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/env_utils.py` & `codeflash-0.6.1/codeflash/code_utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/formatter.py` & `codeflash-0.6.1/codeflash/code_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/git_utils.py` & `codeflash-0.6.1/codeflash/code_utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/instrument_existing_tests.py` & `codeflash-0.6.1/codeflash/code_utils/instrument_existing_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/shell_utils.py` & `codeflash-0.6.1/codeflash/code_utils/shell_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/sqlalchemy_utils.py` & `codeflash-0.6.1/codeflash/code_utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/code_utils/time_utils.py` & `codeflash-0.6.1/codeflash/code_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/discovery/discover_unit_tests.py` & `codeflash-0.6.1/codeflash/discovery/discover_unit_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/discovery/functions_to_optimize.py` & `codeflash-0.6.1/codeflash/discovery/functions_to_optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,33 +477,28 @@
     module_root: str,
 ) -> bool:
     """Optimized version of the filter_functions function above.
     Takes in file paths and returns the count of files that are to be optimized.
     """
     submodule_paths = None
     if file_path.startswith(tests_root + os.sep):
-        print(f"Ignoring file {file_path} because it is in the tests directory")
         return False
     if file_path in ignore_paths or any(
         file_path.startswith(ignore_path + os.sep) for ignore_path in ignore_paths
     ):
-        print(f"Ignoring file {file_path} because it is in the ignored paths")
         return False
     if path_belongs_to_site_packages(file_path):
-        print(f"Ignoring file {file_path} because it is in the site-packages directory")
         return False
     if not file_path.startswith(module_root + os.sep):
-        print(f"Ignoring file {file_path} because it is outside the module-root")
         return False
     if submodule_paths is None:
         submodule_paths = ignored_submodule_paths(module_root)
     if file_path in submodule_paths or any(
         file_path.startswith(submodule_path + os.sep) for submodule_path in submodule_paths
     ):
-        print(f"Ignoring file {file_path} because it is in the ignored submodules")
         return False
 
     return True
 
 
 def function_has_return_statement(function_node: Union[FunctionDef, AsyncFunctionDef]) -> bool:
     for node in ast.walk(function_node):
```

### Comparing `codeflash-0.6.0/codeflash/github/PrComment.py` & `codeflash-0.6.1/codeflash/github/PrComment.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/main.py` & `codeflash-0.6.1/codeflash/main.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/optimization/function_context.py` & `codeflash-0.6.1/codeflash/optimization/function_context.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/optimization/optimizer.py` & `codeflash-0.6.1/codeflash/optimization/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     get_constrained_function_context_and_dependent_functions,
 )
 from codeflash.result.create_pr import check_create_pr, existing_tests_source_for
 from codeflash.result.explanation import Explanation
 from codeflash.telemetry import posthog
 from codeflash.telemetry.posthog import ph
 from codeflash.telemetry.sentry import init_sentry
-from codeflash.verification.equivalence import compare_results
+from codeflash.verification.equivalence import compare_test_results
 from codeflash.verification.parse_test_output import parse_test_results
 from codeflash.verification.test_results import TestResults, TestType
 from codeflash.verification.test_runner import run_tests
 from codeflash.verification.verification_utils import TestConfig, get_test_file_path
 from codeflash.verification.verifier import generate_tests
 
 
@@ -286,17 +286,17 @@
         )
         if not is_successful(baseline_result):
             pathlib.Path(generated_tests_path).unlink(missing_ok=True)
             for instrumented_path in instrumented_unittests_created_for_function:
                 pathlib.Path(instrumented_path).unlink(missing_ok=True)
             return Failure(baseline_result.failure())
         original_code_baseline: OriginalCodeBaseline = baseline_result.unwrap()
-        logging.info("Optimizing code ...")
         # TODO: Postprocess the optimized function to include the original docstring and such
 
+        best_optimization = None
         for u, candidates in enumerate(
             [optimizations_set.control, optimizations_set.experiment],
         ):
             if candidates is None:
                 continue
 
             tests_in_file: list[TestsInFile] = function_to_tests.get(
@@ -383,14 +383,16 @@
                             function_to_optimize.file_path,
                             dependent_functions_by_module_abspath,
                         )
         # Delete all the generated tests to not cause any clutter.
         pathlib.Path(generated_tests_path).unlink(missing_ok=True)
         for test_paths in instrumented_unittests_created_for_function:
             pathlib.Path(test_paths).unlink(missing_ok=True)
+        if not best_optimization:
+            return Failure(f"No best optimizations found for function {function_to_optimize.qualified_name}")
         return Success(best_optimization)
 
     def determine_best_candidate(
         self,
         candidates: list[OptimizedCandidate],
         code_context: CodeOptimizationContext,
         dependent_functions_by_module_abspath: dict[str, set[str]],
@@ -403,29 +405,32 @@
         function_trace_id: str,
         only_run_this_test_function: list[TestsInFile] | None = None,
     ) -> BestOptimization | None:
         best_optimization: BestOptimization | None = None
         best_runtime_until_now = original_code_baseline.runtime  # The fastest code runtime until now
 
         speedup_ratios: dict[str, float | None] = {}
-        optimized_runtimes = {}
+        optimized_runtimes: dict[str, float | None] = {}
         is_correct = {}
 
+        logging.info(
+            f"Determining best optimized candidate (out of {len(candidates)}) for {function_to_optimize.qualified_name} ...",
+        )
         for i, candidate in enumerate(candidates):
             j = i + 1
             if candidate.source_code is None:
                 continue
             # remove left overs from previous run
             pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.bin")).unlink(
                 missing_ok=True,
             )
             pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.sqlite")).unlink(
                 missing_ok=True,
             )
-            logging.info("Optimized candidate:")
+            logging.info(f"Optimized candidate {j}/{len(candidates)}:")
             logging.info(candidate.source_code)
             try:
                 replace_function_definitions_in_module(
                     function_names=[function_to_optimize.qualified_name],
                     optimized_code=candidate.source_code,
                     file_path_of_module_with_function_to_optimize=function_to_optimize.file_path,
                     module_abspath=function_to_optimize.file_path,
@@ -448,15 +453,15 @@
                     )
             except (
                 ValueError,
                 SyntaxError,
                 cst.ParserSyntaxError,
                 AttributeError,
             ) as e:
-                logging.exception(e)
+                logging.error(e)  # noqa: TRY400
                 self.write_code_and_dependents(
                     original_code,
                     original_dependent_code,
                     function_to_optimize.file_path,
                     dependent_functions_by_module_abspath,
                 )
                 continue
@@ -469,16 +474,16 @@
                         run_generated_tests = True
                         break
 
             run_results = self.run_optimized_candidate(
                 optimization_index=j,
                 instrumented_unittests_created_for_function=instrumented_unittests_created_for_function,
                 overall_original_test_results=original_code_baseline.overall_test_results,
-                existing_test_results=original_code_baseline.existing_test_results,
-                original_gen_results=original_code_baseline.generated_test_results,
+                original_existing_test_results=original_code_baseline.existing_test_results,
+                original_generated_test_results=original_code_baseline.generated_test_results,
                 generated_tests_path=generated_tests_path,
                 best_runtime_until_now=best_runtime_until_now,
                 tests_in_file=only_run_this_test_function,
                 run_generated_tests=run_generated_tests,
             )
             if not is_successful(run_results):
                 optimized_runtimes[candidate.optimization_id] = None
@@ -816,39 +821,43 @@
         )
 
     def establish_original_code_baseline(
         self,
         function_name: str,
         instrumented_unittests_created_for_function: set[str],
         generated_tests_path: str,
-        tests_in_file: List[TestsInFile],
+        tests_in_file: list[TestsInFile],
     ) -> Result[OriginalCodeBaseline, str]:
         original_runtime = None
         best_runtime = None
         original_gen_results = None
         overall_original_test_results = None
         times_run = 0
         success = True
         # Keep the runtime in some acceptable range
         generated_tests_elapsed_time = 0.0
 
         # For the original function - run the tests and get the runtime
+        logging.info(f"Establishing original code baseline runtime for {function_name}.")
         # TODO: Compare the function return values over the multiple runs and check if they are any different,
         #  if they are different, then we can't optimize this function because it is a non-deterministic function
         test_env = os.environ.copy()
         test_env["CODEFLASH_TEST_ITERATION"] = str(0)
         test_env["CODEFLASH_TRACER_DISABLE"] = "1"
         if "PYTHONPATH" not in test_env:
             test_env["PYTHONPATH"] = self.args.project_root
         else:
             test_env["PYTHONPATH"] += os.pathsep + self.args.project_root
         cumulative_test_runtime = 0
         cumulative_test_runs = 0
         first_run = True
         do_break = False
+        logging.info(
+            f"Running {len(instrumented_unittests_created_for_function)} tests for {function_name} ..."
+        )
         while (
             cumulative_test_runtime < MAX_CUMULATIVE_TEST_RUNTIME_NANOSECONDS
             and cumulative_test_runs < MAX_TEST_FUNCTION_RUNS
         ):
             for i in range(MAX_TEST_RUN_ITERATIONS):
                 if generated_tests_elapsed_time > MAX_FUNCTION_TEST_SECONDS:
                     do_break = True
@@ -878,15 +887,15 @@
 
                     timing = unittest_results.total_passed_runtime()
                     original_test_results_iter.merge(unittest_results)
                     existing_test_results.merge(unittest_results)
                     instrumented_existing_test_timing.append(timing)
                 if i == 0 and first_run:
                     logging.info(
-                        f"original code, existing unit test results -> {original_test_results_iter.get_test_pass_fail_report()}",
+                        f"Existing unit test results for original code: {original_test_results_iter.get_test_pass_fail_report()}",
                     )
 
                 original_gen_results = self.run_and_parse_tests(
                     test_env,
                     generated_tests_path,
                     TestType.GENERATED_REGRESSION,
                     0,
@@ -904,15 +913,15 @@
                 # TODO: Doing a simple sum of test runtime, Improve it by looking at test by test runtime, or a better scheme
                 # TODO: If the runtime is None, that happens in the case where an exception is expected and is successfully
                 #  caught by the test framework. This makes the test pass, but we can't find runtime because the exception caused
                 #  the execution to not reach the runtime measurement part. We are currently ignoring such tests, because the performance
                 #  for such a execution that raises an exception should not matter.
                 if i == 0 and first_run:
                     logging.info(
-                        f"original generated tests results -> {original_gen_results.get_test_pass_fail_report()}",
+                        f"Generated tests results for original code: {original_gen_results.get_test_pass_fail_report()}",
                     )
 
                 if not original_gen_results:
                     original_total_runtime_iter = sum(instrumented_existing_test_timing)
                 else:
                     original_total_runtime_iter = original_gen_results.total_passed_runtime() + sum(
                         instrumented_existing_test_timing,
@@ -924,15 +933,15 @@
                     )
                     logging.warning(original_gen_results.test_results)
                     do_break = True
                     break
                 original_test_results_iter.merge(original_gen_results)
                 if i == 0 and first_run:
                     logging.info(
-                        f"Original overall test results = {TestResults.report_to_string(original_test_results_iter.get_test_pass_fail_report_by_type())}",
+                        f"Overall test results for original code: {TestResults.report_to_string(original_test_results_iter.get_test_pass_fail_report_by_type())}",
                     )
                 if original_runtime is None or original_total_runtime_iter < original_runtime:
                     original_runtime = best_runtime = original_total_runtime_iter
                     overall_original_test_results = original_test_results_iter
                 cumulative_test_runs += 1
                 cumulative_test_runtime += original_total_runtime_iter
                 times_run += 1
@@ -961,16 +970,16 @@
         )
 
     def run_optimized_candidate(
         self,
         optimization_index: int,
         instrumented_unittests_created_for_function: set[str],
         overall_original_test_results: TestResults,
-        existing_test_results: TestResults,
-        original_gen_results: TestResults,
+        original_existing_test_results: TestResults,
+        original_generated_test_results: TestResults,
         generated_tests_path: str,
         best_runtime_until_now: int,
         tests_in_file: Optional[List[TestsInFile]],
         run_generated_tests: bool,
     ) -> Result[OptimizedCandidateResult, str]:
         success = True
         best_test_runtime = None
@@ -1001,105 +1010,110 @@
                 pathlib.Path(
                     get_run_tmp_file(f"test_return_values_{optimization_index}.sqlite"),
                 ).unlink(missing_ok=True)
                 if generated_tests_elapsed_time > MAX_FUNCTION_TEST_SECONDS:
                     do_break = True
                     break
 
-                optimized_test_results_iter = TestResults()
+                candidate_existing_test_results = TestResults()
                 instrumented_test_timing = []
                 for instrumented_test_file in instrumented_unittests_created_for_function:
                     relevant_tests_in_file = [
                         test_in_file
                         for test_in_file in tests_in_file
                         if test_in_file.test_file == instrumented_test_file.replace("__perfinstrumented", "")
                     ]
                     is_replay_test = relevant_tests_in_file[0].test_type == TestType.REPLAY_TEST
                     if is_replay_test and len(relevant_tests_in_file) > 1:
                         logging.warning(
                             f"Multiple tests found for the replay test {instrumented_test_file}. Should not happen",
                         )
-                    unittest_results_optimized = self.run_and_parse_tests(
+                    candidate_existing_test_result = self.run_and_parse_tests(
                         test_env,
                         instrumented_test_file,
                         relevant_tests_in_file[0].test_type,
                         optimization_index,
                         relevant_tests_in_file[0].test_function if is_replay_test else None,
                     )
-                    timing = unittest_results_optimized.total_passed_runtime()
-                    optimized_test_results_iter.merge(unittest_results_optimized)
+                    timing = candidate_existing_test_result.total_passed_runtime()
+                    candidate_existing_test_results.merge(candidate_existing_test_result)
                     instrumented_test_timing.append(timing)
                 if first_run and test_index == 0:
                     equal_results = True
                     logging.info(
-                        f"optimized existing unit tests result -> {optimized_test_results_iter.get_test_pass_fail_report()}",
+                        f"Existing unit tests results for candidate: {candidate_existing_test_results.get_test_pass_fail_report()}",
                     )
-                    equal_return_values = compare_results(
-                        existing_test_results,
-                        optimized_test_results_iter,
+                    return_values_are_equal = compare_test_results(
+                        original_existing_test_results,
+                        candidate_existing_test_results,
                     )
-                    for test_invocation in optimized_test_results_iter:
+                    for test_invocation in candidate_existing_test_results:
                         if (
                             overall_original_test_results.get_by_id(test_invocation.id) is None
                             or test_invocation.did_pass
                             != overall_original_test_results.get_by_id(
                                 test_invocation.id,
                             ).did_pass
-                            or not equal_return_values
+                            or not return_values_are_equal
                         ):
-                            logging.info("Results did not match.")
+                            logging.info("Test results did not match the test results of the original code.")
                             logging.info(
-                                f"Test {test_invocation.id} failed on the optimized code. Skipping this optimization",
+                                f"Test {test_invocation.id} failed. Skipping this candidate.",
                             )
                             equal_results = False
                             do_break = True
                             break
                     if not equal_results:
                         do_break = True
                         break
 
-                test_results = None
+                candidate_generated_test_results = None
                 if run_generated_tests:
-                    test_results = self.run_and_parse_tests(
+                    candidate_generated_test_results = self.run_and_parse_tests(
                         test_env,
                         generated_tests_path,
                         TestType.GENERATED_REGRESSION,
                         optimization_index,
                     )
 
-                if test_results and first_run and test_index == 0:
+                if candidate_generated_test_results and first_run and test_index == 0:
                     logging.info(
-                        f"generated test_results optimized -> {test_results.get_test_pass_fail_report()}",
+                        f"Generated tests results for candidate: {candidate_generated_test_results.get_test_pass_fail_report()}",
                     )
-                    if compare_results(original_gen_results, test_results):
+                    if compare_test_results(
+                        original_generated_test_results,
+                        candidate_generated_test_results,
+                    ):
                         equal_results = True
-                        logging.info("Results matched!")
+                        logging.info("Test results matched!")
                     else:
-                        logging.info("Results did not match.")
+                        logging.info("Test results did not match the test results of the original code.")
                         equal_results = False
                 if not equal_results:
                     do_break = True
                     break
 
-                if not test_results:
+                if not candidate_generated_test_results:
                     test_runtime = sum(instrumented_test_timing)
                 else:
-                    test_runtime = test_results.total_passed_runtime() + sum(instrumented_test_timing)
+                    test_runtime = candidate_generated_test_results.total_passed_runtime() + sum(
+                        instrumented_test_timing,
+                    )
 
                 if test_runtime == 0:
                     logging.warning(
                         "The overall test runtime of the optimized function is 0, couldn't run tests.",
                     )
                     do_break = True
                     break
                 if best_test_runtime is None or test_runtime < best_test_runtime:
-                    if test_results:
-                        optimized_test_results_iter.merge(test_results)
+                    if candidate_generated_test_results:
+                        candidate_existing_test_results.merge(candidate_generated_test_results)
                     best_test_runtime = test_runtime
-                    best_test_results = optimized_test_results_iter
+                    best_test_results = candidate_existing_test_results
                 cumulative_test_runs += 1
                 cumulative_test_runtime += test_runtime
                 times_run += 1
             if first_run:
                 first_run = False
             if best_test_runtime is not None and (best_test_runtime > 3 * best_runtime_until_now):
                 # If after 5 runs, the optimized candidate is taking 3 times longer than the best code until now,
```

### Comparing `codeflash-0.6.0/codeflash/output1.trace` & `codeflash-0.6.1/codeflash/output1.trace`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/result/create_pr.py` & `codeflash-0.6.1/codeflash/result/create_pr.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/result/explanation.py` & `codeflash-0.6.1/codeflash/result/explanation.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/telemetry/posthog.py` & `codeflash-0.6.1/codeflash/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/telemetry/sentry.py` & `codeflash-0.6.1/codeflash/telemetry/sentry.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/tracer.py` & `codeflash-0.6.1/codeflash/tracer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/tracing/profile_stats.py` & `codeflash-0.6.1/codeflash/tracing/profile_stats.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/tracing/replay_test.py` & `codeflash-0.6.1/codeflash/tracing/replay_test.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/update_license_version.py` & `codeflash-0.6.1/codeflash/update_license_version.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/verification/comparator.py` & `codeflash-0.6.1/codeflash/verification/comparator.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/verification/parse_test_output.py` & `codeflash-0.6.1/codeflash/verification/parse_test_output.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/verification/test_results.py` & `codeflash-0.6.1/codeflash/verification/test_results.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/verification/test_runner.py` & `codeflash-0.6.1/codeflash/verification/test_runner.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/verification/verification_utils.py` & `codeflash-0.6.1/codeflash/verification/verification_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/codeflash/verification/verifier.py` & `codeflash-0.6.1/codeflash/verification/verifier.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.0/pyproject.toml` & `codeflash-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "codeflash"
-version = "0.6.0" # Determined by poetry-dynamic-versioning during `poetry build`
+version = "0.6.1" # Determined by poetry-dynamic-versioning during `poetry build`
 description = "Client for codeflash.ai - automatic code performance optimization, powered by AI"
 license = "BSL-1.1"
 authors = ["CodeFlash Inc. <contact@codeflash.ai>"]
 homepage = "https://codeflash.ai"
 readme = "README.md"
 packages = [
     { include = "codeflash" },
@@ -88,14 +88,17 @@
 
 [tool.ruff.lint.pep8-naming]
 classmethod-decorators = [
     # Allow Pydantic's `@validator` decorator to trigger class method treatment.
     "pydantic.validator",
 ]
 
+[tool.ruff.lint.per-file-ignores]
+"**/*" = ["D102"]
+
 [tool.ruff]
 line-length = 110
 
 [tool.ruff.format]
 docstring-code-format = true
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `codeflash-0.6.0/PKG-INFO` & `codeflash-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflash
-Version: 0.6.0
+Version: 0.6.1
 Summary: Client for codeflash.ai - automatic code performance optimization, powered by AI
 Home-page: https://codeflash.ai
 License: BSL-1.1
 Keywords: codeflash,performance,optimization,ai,code,machine learning,LLM
 Author: CodeFlash Inc.
 Author-email: contact@codeflash.ai
 Requires-Python: >=3.9,<4.0
```

