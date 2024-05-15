# Comparing `tmp/openai_priority_loadbalancer-1.0.0.tar.gz` & `tmp/openai_priority_loadbalancer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-1.0.0.tar", last modified: Tue May 14 20:12:10 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-1.0.1.tar", last modified: Wed May 15 10:41:08 2024, max compression
```

## Comparing `openai_priority_loadbalancer-1.0.0.tar` & `openai_priority_loadbalancer-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 20:12:10.893900 openai_priority_loadbalancer-1.0.0/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    11991 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.0/PACKAGE_README.md
--rw-rw-rw-   0        0        0    12630 2024-05-14 20:12:10.890250 openai_priority_loadbalancer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    12513 2024-05-14 04:17:29.000000 openai_priority_loadbalancer-1.0.0/README.md
--rw-rw-rw-   0        0        0      711 2024-05-14 20:10:44.000000 openai_priority_loadbalancer-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 20:12:10.897313 openai_priority_loadbalancer-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 20:12:10.720042 openai_priority_loadbalancer-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 20:12:10.800674 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer/
--rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer/__init__.py
--rw-rw-rw-   0        0        0    10592 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:12:10.886422 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    12630 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 10:41:08.557744 openai_priority_loadbalancer-1.0.1/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    12101 2024-05-15 10:38:20.000000 openai_priority_loadbalancer-1.0.1/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    12740 2024-05-15 10:41:08.552352 openai_priority_loadbalancer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12216 2024-05-15 09:57:38.000000 openai_priority_loadbalancer-1.0.1/README.md
+-rw-rw-rw-   0        0        0      711 2024-05-15 10:39:10.000000 openai_priority_loadbalancer-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 10:41:08.557744 openai_priority_loadbalancer-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 10:41:08.449846 openai_priority_loadbalancer-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 10:41:08.494955 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0     9649 2024-05-15 10:38:20.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:41:08.548589 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    12740 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-15 10:41:08.000000 openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-1.0.0/LICENSE` & `openai_priority_loadbalancer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.0/PACKAGE_README.md` & `openai_priority_loadbalancer-1.0.1/PACKAGE_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## Attribution
 
 This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
 
 ## Prerequisites
 
-It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
+It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) test harness for this package will look very familiar to you.
 It's also good to have some knowledge of authentication and identities.
 
 ## Getting Started
 
 ### Installing the Package
 
 1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
```

### Comparing `openai_priority_loadbalancer-1.0.0/PKG-INFO` & `openai_priority_loadbalancer-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,15 +40,15 @@
 
 ## Attribution
 
 This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
 
 ## Prerequisites
 
-It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
+It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) test harness for this package will look very familiar to you.
 It's also good to have some knowledge of authentication and identities.
 
 ## Getting Started
 
 ### Installing the Package
 
 1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
```

### Comparing `openai_priority_loadbalancer-1.0.0/README.md` & `openai_priority_loadbalancer-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,14 @@
 It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
 It's also good to have some knowledge of authentication and identities.
 
 ## Authentication
 
 Locally, you can log into Azure via the CLI and the steps below and use the `AzureDefaultCredential` (what I use in my example). When deploying this application in Azure, it's recommended to use a managed identity for authentication. It's best to avoid using the Azure OpenAI instances' keys as that could a) accidentally leave credentials in your source code, and b) the keys are different for each instance, which would probably require expanding upon the `Backends` class. Best to just avoid keys.
 
-## Single Requestor Model
-
-I started with a single-requestor model to experiment with the algorithm to select backends. This model is not typically used, as most workloads run multiple Python workers in parallel. Nevertheless, I left the files in the repo with the `single-requestor` suffix.
-
 ## Getting Started
 
 ### Cloning the repo & Preparing the python environment
 
 1. Clone the repo.
 1. Open the cloned repo folder in VS Code.
 1. Open a terminal session in VS Code.
```

### Comparing `openai_priority_loadbalancer-1.0.0/pyproject.toml` & `openai_priority_loadbalancer-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai_priority_loadbalancer"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Simon Kurtz", email="simonkurtz@gmail.com" },
 ]
 description = "A multi-backend, prioritization load balancer for OpenAI"
 readme = "PACKAGE_README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py` & `openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,14 +83,49 @@
                 soonest_retry_after = backend.retry_after
                 soonest_backend = backend.host
 
         delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1     # Add a 1 second buffer to ensure we don't retry too early
         self._log.info(f"Soonest Retry After: {soonest_backend} - {str(delay)} second(s)")
         return delay
 
+    def _handle_200_399_response(self, request, response, backend_index):
+        # Successful requests
+        self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
+        self.backends[backend_index].successful_call_count += 1
+
+    def _handle_429_5xx_response(self, request, response, backend_index):
+        # If the server is throttling or there's a server error, retry with a different server
+        self._log.info(f"Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
+
+        retry_after = int(response.headers.get('Retry-After', '-1'))
+
+        if retry_after == -1:
+            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
+
+        if retry_after == -1:
+            retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
+
+        self._log.info(f"Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
+
+        backend = self.backends[backend_index]
+        backend.is_throttling = True
+        backend.retry_after = datetime.now(tzutc()) + timedelta(seconds = retry_after)
+        self._get_remaining_backends()
+
+    def _handle_4xx_response(self, request, response):
+        # Would likely be a 4xx error other than 429
+        self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
+
+    def modify_request(self, request, backend_index):
+        # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
+        # Update URL and host header as both must match the backend server.
+        request.url = request.url.copy_with(host = self.backends[backend_index].host)
+        request.headers = request.headers.copy()    # Create a mutable copy of the headers
+        request.headers['host'] = self.backends[backend_index].host
+
     def _return_429(self):
         self._log.warning("No backend available!")
         retry_after = str(self._get_soonest_retry_after())
         self._log.info(f"Returning HTTP 429 with Retry-After header value of {retry_after} second(s).")
         return Response(429, content = '', headers={'Retry-After': retry_after})
 
 class AsyncLoadBalancer(BaseLoadBalancer):
@@ -101,60 +136,40 @@
     # Public Methods
     async def handle_async_request(self, request):
         self._check_throttling()
         self._get_remaining_backends()
         response = None
 
         while True and self._remaining_backends > 0:
+            # 1) Determine the appropriate backend to use
             backend_index = self._get_backend_index()
 
             if backend_index == -1:
                 return self._return_429()
 
-            # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
-            # Update URL and host header as both must match the backend server.
-            request.url = request.url.copy_with(host = self.backends[backend_index].host)
-            request.headers = request.headers.copy()    # Create a mutable copy of the headers
-            request.headers['host'] = self.backends[backend_index].host
+            # 2) Modify the intercepted request
+            self.modify_request(request, backend_index)
 
-            # Send the request to the backend
+            # 3) Send the request to the selected backend (via async)
             try:
                 response = await self._transport.send(request)
             except Exception as e:
                 self._log.error(traceback.print_exc())
 
+            # 4) Evaluate the response from the backend
             if response is not None and (response.status_code == 429 or response.status_code >= 500):
-                # If the server is throttling or there's a server error, retry with a different server
-                self._log.info(f"Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
-
-                retry_after = int(response.headers.get('Retry-After', '-1'))
-
-                if retry_after == -1:
-                    retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
-
-                if retry_after == -1:
-                    retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
-
-                self._log.info(f"Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
-
-                backend = self.backends[backend_index]
-                backend.is_throttling = True
-                backend.retry_after = datetime.now(tzutc()) + timedelta(seconds = retry_after)
-                self._get_remaining_backends()
+                self._handle_429_5xx_response(request, response, backend_index)
                 continue
 
             elif response is not None and (response.status_code >= 200 and response.status_code <= 399):
-                # Successful requests
-                self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
-                self.backends[backend_index].successful_call_count += 1
+                self._handle_200_399_response(request, response, backend_index)
                 break
 
             else:
-                # Would likely be a 4xx error other than 429
-                self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
+                self._handle_4xx_response(request, response)
                 break
 
         if self._remaining_backends == 0:
             return self._return_429()
 
         return response
 
@@ -166,60 +181,39 @@
     # Public Methods
     def handle_request(self, request):
         self._check_throttling()
         self._get_remaining_backends()
         response = None
 
         while True and self._remaining_backends > 0:
+            # 1) Determine the appropriate backend to use
             backend_index = self._get_backend_index()
 
             if backend_index == -1:
                 return self._return_429()
 
-            # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
-            # Update URL and host header as both must match the backend server.
-            request.url = request.url.copy_with(host = self.backends[backend_index].host)
-            headers = request.headers.copy()    # Create a mutable copy of the headers
-            headers['host'] = self.backends[backend_index].host
-            request.headers = headers           # Assign the modified headers back to request.headers
+            # 2) Modify the intercepted request
+            self.modify_request(request, backend_index)
 
-            # Send the request to the backend
+            # 3) Send the request to the selected backend
             try:
                 response = self._transport.send(request)
             except Exception as e:
                 self._log.error(traceback.print_exc())
 
+            # 4) Evaluate the response from the backend
             if response is not None and (response.status_code == 429 or response.status_code >= 500):
-                # If the server is throttling or there's a server error, retry with a different server
-                self._log.warning(f"Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
-
-                retry_after = int(response.headers.get('Retry-After', '-1'))
-
-                if retry_after == -1:
-                    retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
-
-                if retry_after == -1:
-                    retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
-
-                self._log.info(f"Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
-
-                backend = self.backends[backend_index]
-                backend.is_throttling = True
-                backend.retry_after = datetime.now(tzutc()) + timedelta(seconds = retry_after)
-                self._get_remaining_backends()
+                self._handle_429_5xx_response(request, response, backend_index)
                 continue
 
             elif response is not None and (response.status_code >= 200 and response.status_code <= 399):
-                # Successful requests
-                self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
-                self.backends[backend_index].successful_call_count += 1
+                self._handle_200_399_response(request, response, backend_index)
                 break
 
             else:
-                # Would likely be a 4xx error other than 429
-                self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
+                self._handle_4xx_response(request, response)
                 break
 
         if self._remaining_backends == 0:
             return self._return_429()
 
         return response
```

### Comparing `openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-1.0.1/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,15 +40,15 @@
 
 ## Attribution
 
 This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
 
 ## Prerequisites
 
-It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
+It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) test harness for this package will look very familiar to you.
 It's also good to have some knowledge of authentication and identities.
 
 ## Getting Started
 
 ### Installing the Package
 
 1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
```

