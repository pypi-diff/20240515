# Comparing `tmp/openai_priority_loadbalancer-0.0.6.tar.gz` & `tmp/openai_priority_loadbalancer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-0.0.6.tar", last modified: Tue May 14 18:57:29 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-1.0.0.tar", last modified: Tue May 14 20:12:10 2024, max compression
```

## Comparing `openai_priority_loadbalancer-0.0.6.tar` & `openai_priority_loadbalancer-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:57:29.233017 openai_priority_loadbalancer-0.0.6/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    11693 2024-05-14 18:56:49.000000 openai_priority_loadbalancer-0.0.6/PACKAGE_README.md
--rw-rw-rw-   0        0        0    12528 2024-05-14 18:57:29.228920 openai_priority_loadbalancer-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    12513 2024-05-14 04:17:29.000000 openai_priority_loadbalancer-0.0.6/README.md
--rw-rw-rw-   0        0        0      711 2024-05-14 18:57:02.000000 openai_priority_loadbalancer-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 18:57:29.233813 openai_priority_loadbalancer-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 18:57:29.064963 openai_priority_loadbalancer-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:57:29.130833 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer/
--rw-rw-rw-   0        0        0       44 2024-05-14 04:07:11.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer/__init__.py
--rw-rw-rw-   0        0        0    10367 2024-05-14 18:54:50.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:57:29.217677 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    12528 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 20:12:10.893900 openai_priority_loadbalancer-1.0.0/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    11991 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.0/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    12630 2024-05-14 20:12:10.890250 openai_priority_loadbalancer-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12513 2024-05-14 04:17:29.000000 openai_priority_loadbalancer-1.0.0/README.md
+-rw-rw-rw-   0        0        0      711 2024-05-14 20:10:44.000000 openai_priority_loadbalancer-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 20:12:10.897313 openai_priority_loadbalancer-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 20:12:10.720042 openai_priority_loadbalancer-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 20:12:10.800674 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0    10592 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:12:10.886422 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    12630 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-14 20:12:10.000000 openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-0.0.6/LICENSE` & `openai_priority_loadbalancer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-0.0.6/PACKAGE_README.md` & `openai_priority_loadbalancer-1.0.0/PACKAGE_README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,196 +1,198 @@
-# OpenAI Priority Load Balancer
-
-Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
-
-- Distribution of requests over multiple consumption instances to mitigate throttling.
-- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
-- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
-
-While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
-
-And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
-
-Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
-
-## Disclaimer
-
-**This is a pseudo load-balancer.**
-
-When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
-immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
-
-Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
-
-## Attribution
-
-This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
-
-## Prerequisites
-
-It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
-It's also good to have some knowledge of authentication and identities.
-
-## Getting Started
-
-### Installing the Package
-
-1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
-
-    ```text
-    openai_priority_loadbalancer
-    ```
-
-1. Run `pip install -r </path/to/requirements.txt>`.
-
-### Importing Classes
-
-Either import the synchronous load balancer:
-
-```python
-from openai_priority_loadbalancer import LoadBalancer, Backend
-```
-
-Or import the asynchronous load balancer:
-
-```python
-from openai_priority_loadbalancer import AsyncLoadBalancer, Backend
-```
-
-### Configuring the Backends and Load Balancer
-
-1. Define a list of backends according to the *Load Balancer Configuration* section below.
-
-    ```python
-    backends: List[Backend] = [
-        Backend("oai-eastus.openai.azure.com", 1),
-        Backend("oai-southcentralus.openai.azure.com", 1)
-    ]
-    ```
-
-1. Instantiate the load balancer and inject a new httpx client with the load balancer as the new transport.
-
-    ```python
-    lb = LoadBalancer(backends)
-
-    client = AzureOpenAI(
-        azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
-        azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
-        api_version = "2024-04-01-preview",
-        http_client = DefaultHttpxClient(transport = lb)        # Inject the load balancer as the transport in a new default httpx client
-    )
-    ```
-
-### Using the Load Balancer
-
-As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
-
-### Logging
-
-OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
-
-## Distribution of Requests
-
-### Across Different Priorities
-
-Requests are made to the highest priority backend that is available. For example:
-
-- Priority 1, when available, will always supersede priority 2.
-- Priority 2, when available, will always supersede an unavailable priority 1.
-- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
-
-### Across Multiple Backends of Same Priority
-
-In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
-
-There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
-
-## Backoff & Retries
-
-When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
-You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
-
-In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
-The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
-
-```text
-2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
-2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
-2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
-2024-05-11 00:56:32.452883:   No backends available. Exiting.
-2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
-2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
-2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
-```
-
-## Load Balancer Configuration
-
-At its core, the Load Balancer configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
-
-I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
-The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
-While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
-
-### One Backend
-
-This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Two Backends with Same Priority
-
-Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Same Priority
-
-Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Two Different Priorities
-
-The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
-]
-```
-
-### Three Backends with Three Different Priorities
-
-An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
-]
-```
+# OpenAI Priority Load Balancer
+
+Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
+
+- Distribution of requests over multiple consumption instances to mitigate throttling.
+- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
+- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
+
+While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
+
+And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
+
+Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
+
+**Please refer to the GitHub repo for detailed test harnesses for the use cases described below.**
+
+## Disclaimer
+
+**This is a pseudo load-balancer.**
+
+When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
+immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
+
+Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
+
+## Attribution
+
+This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
+
+## Prerequisites
+
+It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
+It's also good to have some knowledge of authentication and identities.
+
+## Getting Started
+
+### Installing the Package
+
+1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
+
+    ```text
+    openai_priority_loadbalancer
+    ```
+
+1. Run `pip install -r </path/to/requirements.txt>`.
+
+### Importing Classes
+
+Either import the synchronous load balancer:
+
+```python
+from openai_priority_loadbalancer import LoadBalancer, Backend
+```
+
+Or import the asynchronous load balancer:
+
+```python
+from openai_priority_loadbalancer import AsyncLoadBalancer, Backend
+```
+
+### Configuring the Backends and Load Balancer
+
+1. Define a list of backends according to the *Load Balancer Configuration* section below.
+
+    ```python
+    backends: List[Backend] = [
+        Backend("oai-eastus.openai.azure.com", 1),
+        Backend("oai-southcentralus.openai.azure.com", 1)
+    ]
+    ```
+
+1. Instantiate the load balancer and inject a new httpx client with the load balancer as the new transport.
+
+    ```python
+    lb = LoadBalancer(backends)
+
+    client = AzureOpenAI(
+        azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
+        azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
+        api_version = "2024-04-01-preview",
+        http_client = DefaultHttpxClient(transport = lb)        # Inject the load balancer as the transport in a new default httpx client
+    )
+    ```
+
+### Using the Load Balancer
+
+As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
+
+### Logging
+
+OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
+
+## Distribution of Requests
+
+### Across Different Priorities
+
+Requests are made to the highest priority backend that is available. For example:
+
+- Priority 1, when available, will always supersede priority 2.
+- Priority 2, when available, will always supersede an unavailable priority 1.
+- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
+
+### Across Multiple Backends of Same Priority
+
+In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
+
+There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
+
+## Backoff & Retries
+
+When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
+You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
+
+In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
+The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+
+```text
+2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
+2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
+2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
+2024-05-11 00:56:32.452883:   No backends available. Exiting.
+2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
+2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
+2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
+```
+
+## Load Balancer Configuration
+
+At its core, the Load Balancer configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
+
+I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
+The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
+While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
+
+### One Backend
+
+This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Two Backends with Same Priority
+
+Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Same Priority
+
+Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Two Different Priorities
+
+The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
+]
+```
+
+### Three Backends with Three Different Priorities
+
+An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
+]
+```
```

### Comparing `openai_priority_loadbalancer-0.0.6/PKG-INFO` & `openai_priority_loadbalancer-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 0.0.6
+Version: 1.0.0
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,16 @@
 
 While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
 
 And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
 
 Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
 
+**Please refer to the GitHub repo for detailed test harnesses for the use cases described below.**
+
 ## Disclaimer
 
 **This is a pseudo load-balancer.**
 
 When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
 immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
```

### Comparing `openai_priority_loadbalancer-0.0.6/README.md` & `openai_priority_loadbalancer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-0.0.6/pyproject.toml` & `openai_priority_loadbalancer-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai_priority_loadbalancer"
-version = "0.0.6"
+version = "1.0.0"
 authors = [
   { name="Simon Kurtz", email="simonkurtz@gmail.com" },
 ]
 description = "A multi-backend, prioritization load balancer for OpenAI"
 readme = "PACKAGE_README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py` & `openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-from datetime import datetime, MINYEAR, MAXYEAR, timedelta, timezone
-from dateutil.tz import tzutc
-from httpx import Client, Response, BaseTransport, AsyncBaseTransport, AsyncClient
-from typing import List
-import logging
-import random
-import traceback
-
-class Backend:
-    # Constructor
-    def __init__(self, host: str, priority: int):
-        self.host = host
-        self.priority = priority
-        self.is_throttling = False
-        self.retry_after = datetime.min
-        self.successful_call_count = 0
-
-# Reference design at https://github.com/encode/httpx/blob/master/httpx/_transports/base.py
-# BaseLoadBalancer providing functionality to both synchronous and asynchronous load balancers
-class BaseLoadBalancer():
-    # Constructor
-    def __init__(self, transport, backends: List[Backend]):
-        self._transport = transport
-        self.backends = backends
-        self._backend_index = -1
-        self._remaining_backends = 1
-        self._log = logging.getLogger("openai-priority-loadbalancer")     # https://www.loggly.com/ultimate-guide/python-logging-basics/
-
-    # "Protected" Methods
-    def _check_throttling(self):
-        min_datetime = datetime(MINYEAR, 1, 1, tzinfo = tzutc())
-
-        for backend in self.backends:
-            if backend.is_throttling and datetime.now(tzutc()) >= backend.retry_after:
-                backend.is_throttling = False
-                backend.retry_after = min_datetime
-                self._log.info(f"Backend {backend.host} is no longer throttling.")
-
-    def _get_backend_index(self):
-        # This is the main logic to pick the backend to be used
-        selected_priority = float('inf')
-        available_backends = []
-
-        for i in range(len(self.backends)):
-            backend = self.backends[i]
-
-            if not backend.is_throttling:
-                backendPriority = backend.priority
-
-                if backendPriority < selected_priority:
-                    selected_priority = backendPriority
-                    available_backends.clear()
-                    available_backends.append(i)
-                elif backendPriority == selected_priority:
-                    available_backends.append(i)
-
-        if len(available_backends) == 1:
-            return available_backends[0]
-
-        if len(available_backends) > 0:
-            # Since this code is very likely being called from multiple python instances with multiple workers in parallel executions, there's no way to distribute requests uniformly across all Azure OpenAI instances.
-            # Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
-            # immediately inhibit the performance benefits of the load balancer. This is why this is more of a pseudo load-balancer. Therefore, we'll just randomize across the available backends.
-            return random.choice(available_backends)
-        else:
-            # If there are no available Backend, -1 will be returned to indicate that nothing is available (and that we should bail).
-            return -1
-
-    def _get_remaining_backends(self):
-        self._remaining_backends = 0
-
-        for backend in self.backends:
-            if not backend.is_throttling:
-                self._remaining_backends += 1
-
-        return self._remaining_backends
-
-    def _get_soonest_retry_after(self):
-        soonest_retry_after = datetime(MAXYEAR, 1, 1, tzinfo = tzutc())
-
-        for backend in self.backends:
-            if backend.is_throttling and backend.retry_after < soonest_retry_after:
-                soonest_retry_after = backend.retry_after
-                soonest_backend = backend.host
-
-        delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1     # Add a 1 second buffer to ensure we don't retry too early
-        self._log.info(f"Soonest Retry After: {soonest_backend} - {str(delay)} second(s)")
-        return delay
-
-    def _return_429(self):
-        self._log.warning("No backend available!")
-        retry_after = str(self._get_soonest_retry_after())
-        self._log.info(f"Returning HTTP 429 with Retry-After header value of {retry_after} second(s).")
-        return Response(429, content = '', headers={'Retry-After': retry_after})
-
-class AsyncLoadBalancer(BaseLoadBalancer):
-    # Constructor
-    def __init__(self, backends: List[Backend]):
-        super().__init__(AsyncClient(), backends)
-
-    # Public Methods
-    async def handle_async_request(self, request):
-        self._check_throttling()
-        self._get_remaining_backends()
-        response = None
-
-        while True and self._remaining_backends > 0:
-            backend_index = self._get_backend_index()
-
-            if backend_index == -1:
-                return self._return_429()
-
-            # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
-            # Update URL and host header as both must match the backend server.
-            request.url = request.url.copy_with(host = self.backends[backend_index].host)
-            request.headers = request.headers.copy()    # Create a mutable copy of the headers
-            request.headers['host'] = self.backends[backend_index].host
-
-            # Send the request to the backend
-            try:
-                response = await self._transport.send(request)
-            except Exception as e:
-                self._log.error(traceback.print_exc())
-
-            if response is not None and (response.status_code == 429 or response.status_code >= 500):
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
-                continue
-
-            elif response is not None and (response.status_code >= 200 and response.status_code <= 399):
-                # Successful requests
-                self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
-                self.backends[backend_index].successful_call_count += 1
-                break
-
-            else:
-                # Would likely be a 4xx error other than 429
-                self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
-                break
-
-        if self._remaining_backends == 0:
-            return self._return_429()
-
-        return response
-
-class LoadBalancer(BaseLoadBalancer):
-    # Constructor
-    def __init__(self, backends: List[Backend]):
-        super().__init__(Client(), backends)
-
-    # Public Methods
-    def handle_request(self, request):
-        self._check_throttling()
-        self._get_remaining_backends()
-        response = None
-
-        while True and self._remaining_backends > 0:
-            backend_index = self._get_backend_index()
-
-            if backend_index == -1:
-                return self._return_429()
-
-            # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
-            # Update URL and host header as both must match the backend server.
-            request.url = request.url.copy_with(host = self.backends[backend_index].host)
-            headers = request.headers.copy()    # Create a mutable copy of the headers
-            headers['host'] = self.backends[backend_index].host
-            request.headers = headers           # Assign the modified headers back to request.headers
-
-            # Send the request to the backend
-            try:
-                response = self._transport.send(request)
-            except Exception as e:
-                self._log.error(traceback.print_exc())
-
-            if response is not None and (response.status_code == 429 or response.status_code >= 500):
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
-                continue
-
-            elif response is not None and (response.status_code >= 200 and response.status_code <= 399):
-                # Successful requests
-                self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
-                self.backends[backend_index].successful_call_count += 1
-                break
-
-            else:
-                # Would likely be a 4xx error other than 429
-                self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
-                break
-
-        if self._remaining_backends == 0:
-            return self._return_429()
-
-        return response
+from datetime import datetime, MINYEAR, MAXYEAR, timedelta, timezone
+from dateutil.tz import tzutc
+from httpx import Client, Response, BaseTransport, AsyncBaseTransport, AsyncClient
+from typing import List
+import logging
+import random
+import traceback
+
+class Backend:
+    # Constructor
+    def __init__(self, host: str, priority: int):
+        self.host = host
+        self.priority = priority
+        self.is_throttling = False
+        self.retry_after = datetime.min
+        self.successful_call_count = 0
+
+# Reference design at https://github.com/encode/httpx/blob/master/httpx/_transports/base.py
+# BaseLoadBalancer providing functionality to both synchronous and asynchronous load balancers
+class BaseLoadBalancer():
+    # Constructor
+    def __init__(self, transport, backends: List[Backend]):
+        self._transport = transport
+        self.backends = backends
+        self._backend_index = -1
+        self._remaining_backends = 1
+        self._log = logging.getLogger("openai-priority-loadbalancer")     # https://www.loggly.com/ultimate-guide/python-logging-basics/
+
+    # "Protected" Methods
+    def _check_throttling(self):
+        min_datetime = datetime(MINYEAR, 1, 1, tzinfo = tzutc())
+
+        for backend in self.backends:
+            if backend.is_throttling and datetime.now(tzutc()) >= backend.retry_after:
+                backend.is_throttling = False
+                backend.retry_after = min_datetime
+                self._log.info(f"Backend {backend.host} is no longer throttling.")
+
+    def _get_backend_index(self):
+        # This is the main logic to pick the backend to be used
+        selected_priority = float('inf')
+        available_backends = []
+
+        for i in range(len(self.backends)):
+            backend = self.backends[i]
+
+            if not backend.is_throttling:
+                backendPriority = backend.priority
+
+                if backendPriority < selected_priority:
+                    selected_priority = backendPriority
+                    available_backends.clear()
+                    available_backends.append(i)
+                elif backendPriority == selected_priority:
+                    available_backends.append(i)
+
+        if len(available_backends) == 1:
+            return available_backends[0]
+
+        if len(available_backends) > 0:
+            # Since this code is very likely being called from multiple python instances with multiple workers in parallel executions, there's no way to distribute requests uniformly across all Azure OpenAI instances.
+            # Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
+            # immediately inhibit the performance benefits of the load balancer. This is why this is more of a pseudo load-balancer. Therefore, we'll just randomize across the available backends.
+            return random.choice(available_backends)
+        else:
+            # If there are no available Backend, -1 will be returned to indicate that nothing is available (and that we should bail).
+            return -1
+
+    def _get_remaining_backends(self):
+        self._remaining_backends = 0
+
+        for backend in self.backends:
+            if not backend.is_throttling:
+                self._remaining_backends += 1
+
+        return self._remaining_backends
+
+    def _get_soonest_retry_after(self):
+        soonest_retry_after = datetime(MAXYEAR, 1, 1, tzinfo = tzutc())
+
+        for backend in self.backends:
+            if backend.is_throttling and backend.retry_after < soonest_retry_after:
+                soonest_retry_after = backend.retry_after
+                soonest_backend = backend.host
+
+        delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1     # Add a 1 second buffer to ensure we don't retry too early
+        self._log.info(f"Soonest Retry After: {soonest_backend} - {str(delay)} second(s)")
+        return delay
+
+    def _return_429(self):
+        self._log.warning("No backend available!")
+        retry_after = str(self._get_soonest_retry_after())
+        self._log.info(f"Returning HTTP 429 with Retry-After header value of {retry_after} second(s).")
+        return Response(429, content = '', headers={'Retry-After': retry_after})
+
+class AsyncLoadBalancer(BaseLoadBalancer):
+    # Constructor
+    def __init__(self, backends: List[Backend]):
+        super().__init__(AsyncClient(), backends)
+
+    # Public Methods
+    async def handle_async_request(self, request):
+        self._check_throttling()
+        self._get_remaining_backends()
+        response = None
+
+        while True and self._remaining_backends > 0:
+            backend_index = self._get_backend_index()
+
+            if backend_index == -1:
+                return self._return_429()
+
+            # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
+            # Update URL and host header as both must match the backend server.
+            request.url = request.url.copy_with(host = self.backends[backend_index].host)
+            request.headers = request.headers.copy()    # Create a mutable copy of the headers
+            request.headers['host'] = self.backends[backend_index].host
+
+            # Send the request to the backend
+            try:
+                response = await self._transport.send(request)
+            except Exception as e:
+                self._log.error(traceback.print_exc())
+
+            if response is not None and (response.status_code == 429 or response.status_code >= 500):
+                # If the server is throttling or there's a server error, retry with a different server
+                self._log.info(f"Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
+
+                retry_after = int(response.headers.get('Retry-After', '-1'))
+
+                if retry_after == -1:
+                    retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
+
+                if retry_after == -1:
+                    retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
+
+                self._log.info(f"Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
+
+                backend = self.backends[backend_index]
+                backend.is_throttling = True
+                backend.retry_after = datetime.now(tzutc()) + timedelta(seconds = retry_after)
+                self._get_remaining_backends()
+                continue
+
+            elif response is not None and (response.status_code >= 200 and response.status_code <= 399):
+                # Successful requests
+                self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
+                self.backends[backend_index].successful_call_count += 1
+                break
+
+            else:
+                # Would likely be a 4xx error other than 429
+                self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
+                break
+
+        if self._remaining_backends == 0:
+            return self._return_429()
+
+        return response
+
+class LoadBalancer(BaseLoadBalancer):
+    # Constructor
+    def __init__(self, backends: List[Backend]):
+        super().__init__(Client(), backends)
+
+    # Public Methods
+    def handle_request(self, request):
+        self._check_throttling()
+        self._get_remaining_backends()
+        response = None
+
+        while True and self._remaining_backends > 0:
+            backend_index = self._get_backend_index()
+
+            if backend_index == -1:
+                return self._return_429()
+
+            # Modify the request. Note that only the URL and Host header are being modified on the original request object. We make the smallest incision possible to avoid side effects.
+            # Update URL and host header as both must match the backend server.
+            request.url = request.url.copy_with(host = self.backends[backend_index].host)
+            headers = request.headers.copy()    # Create a mutable copy of the headers
+            headers['host'] = self.backends[backend_index].host
+            request.headers = headers           # Assign the modified headers back to request.headers
+
+            # Send the request to the backend
+            try:
+                response = self._transport.send(request)
+            except Exception as e:
+                self._log.error(traceback.print_exc())
+
+            if response is not None and (response.status_code == 429 or response.status_code >= 500):
+                # If the server is throttling or there's a server error, retry with a different server
+                self._log.warning(f"Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
+
+                retry_after = int(response.headers.get('Retry-After', '-1'))
+
+                if retry_after == -1:
+                    retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
+
+                if retry_after == -1:
+                    retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
+
+                self._log.info(f"Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
+
+                backend = self.backends[backend_index]
+                backend.is_throttling = True
+                backend.retry_after = datetime.now(tzutc()) + timedelta(seconds = retry_after)
+                self._get_remaining_backends()
+                continue
+
+            elif response is not None and (response.status_code >= 200 and response.status_code <= 399):
+                # Successful requests
+                self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
+                self.backends[backend_index].successful_call_count += 1
+                break
+
+            else:
+                # Would likely be a 4xx error other than 429
+                self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
+                break
+
+        if self._remaining_backends == 0:
+            return self._return_429()
+
+        return response
```

### Comparing `openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-1.0.0/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 0.0.6
+Version: 1.0.0
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,16 @@
 
 While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
 
 And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
 
 Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
 
+**Please refer to the GitHub repo for detailed test harnesses for the use cases described below.**
+
 ## Disclaimer
 
 **This is a pseudo load-balancer.**
 
 When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
 immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
```

