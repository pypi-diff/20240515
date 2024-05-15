# Comparing `tmp/openlit-1.2.0.tar.gz` & `tmp/openlit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-1.2.0.tar", max compression
+gzip compressed data, was "openlit-1.3.0.tar", max compression
```

## Comparing `openlit-1.2.0.tar` & `openlit-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
--rw-r--r--   0        0        0    11357 2024-05-09 06:25:35.217594 openlit-1.2.0/LICENSE
--rw-r--r--   0        0        0     9235 2024-05-09 06:25:35.217594 openlit-1.2.0/README.md
--rw-r--r--   0        0        0      966 2024-05-09 06:25:35.217594 openlit-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4651 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/__helpers.py
--rw-r--r--   0        0        0     9077 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    15993 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16035 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     1540 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0    22278 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/bedrock/bedrock.py
--rw-r--r--   0        0        0     3253 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10374 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20348 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     2531 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7609 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     3156 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21328 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21179 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0    16265 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8732 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     1478 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     6079 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/vertexai/__init__.py
--rw-r--r--   0        0        0    52372 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/vertexai/async_vertexai.py
--rw-r--r--   0        0        0    52125 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/vertexai/vertexai.py
--rw-r--r--   0        0        0     4291 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3612 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     5764 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0    10535 1970-01-01 00:00:00.000000 openlit-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 10:22:11.314715 openlit-1.3.0/LICENSE
+-rw-r--r--   0        0        0    10716 2024-05-15 10:22:11.314715 openlit-1.3.0/README.md
+-rw-r--r--   0        0        0      966 2024-05-15 10:22:11.314715 openlit-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4651 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/__helpers.py
+-rw-r--r--   0        0        0     9384 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    16026 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16068 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     1540 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0    22278 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/bedrock/bedrock.py
+-rw-r--r--   0        0        0     3253 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10407 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20381 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     1758 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/haystack/__init__.py
+-rw-r--r--   0        0        0     3891 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/haystack/haystack.py
+-rw-r--r--   0        0        0     2531 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7639 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     1973 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     4048 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/llamaindex/llamaindex.py
+-rw-r--r--   0        0        0     3156 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21361 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21212 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0    16265 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-05-15 10:22:11.314715 openlit-1.3.0/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8765 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     1478 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     6079 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/instrumentation/vertexai/__init__.py
+-rw-r--r--   0        0        0    52372 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/instrumentation/vertexai/async_vertexai.py
+-rw-r--r--   0        0        0    52125 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/instrumentation/vertexai/vertexai.py
+-rw-r--r--   0        0        0     4291 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3612 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     5849 2024-05-15 10:22:11.318715 openlit-1.3.0/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    12016 1970-01-01 00:00:00.000000 openlit-1.3.0/PKG-INFO
```

### Comparing `openlit-1.2.0/LICENSE` & `openlit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/README.md` & `openlit-1.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -20,38 +20,44 @@
 Whether you're directly using LLM Libraries like OpenAI, Anthropic or building complex RAG Agents using Langchain, OpenLIT seamlessly integrates observability into your applications, ensuring enhanced performance and reliability across diverse scenarios.
 
 This project adheres to the [Semantic Conventions](https://github.com/open-telemetry/semantic-conventions/tree/main/docs/gen-ai) proposed by the OpenTelemetry community. You can check out the current definitions [here](src/openlit/semcov/__init__.py).
 
 ## What can be Auto Instrumented?
 
 ### LLMs
-- ✅ OpenAI
-- ✅ Anthropic
-- ✅ Cohere
-- ✅ Mistral
-- ✅ Azure OpenAI
-- ✅ HuggingFace Transformers
+- [✅ OpenAI](https://docs.openlit.io/latest/integrations/openai)
+- [✅ Anthropic](https://docs.openlit.io/latest/integrations/anthropic)
+- [✅ Cohere](https://docs.openlit.io/latest/integrations/cohere)
+- [✅ Mistral](https://docs.openlit.io/latest/integrations/mistral)
+- [✅ Azure OpenAI](https://docs.openlit.io/latest/integrations/azure-openai)
+- [✅ HuggingFace Transformers](https://docs.openlit.io/latest/integrations/huggingface)
+- [✅ Amazon Bedrock](https://docs.openlit.io/latest/integrations/bedrock)
+- [✅ Vertex AI](https://docs.openlit.io/latest/integrations/vertexai)
 
 ### Vector DBs
-- ✅ ChromaDB
-- ✅ Pinecone
+- [✅ ChromaDB](https://docs.openlit.io/latest/integrations/chromadb)
+- [✅ Pinecone](https://docs.openlit.io/latest/integrations/pinecone)
 
 ### Frameworks
-- ✅ Langchain
-- ✅ LiteLLM
+- [✅ Langchain](https://docs.openlit.io/latest/integrations/langchain)
+- [✅ LiteLLM](https://docs.openlit.io/latest/integrations/litellm)
+- [✅ LlamaIndex](https://docs.openlit.io/latest/integrations/llama-index)
+- [✅ Haystack](https://docs.openlit.io/latest/integrations/haystack)
 
 ## Supported Destinations
-- ✅ OpenTelemetry Collector
-- ✅ Grafana Cloud
-- ✅ Grafana Tempo
-- ✅ DataDog
-- ✅ New Relic
-- ✅ SigNoz
-- ✅ Dynatrace
-- ✅ OpenObserve
+- [✅ OpenTelemetry Collector](https://docs.openlit.io/latest/connections/otelcol)
+- [✅ Prometheus + Tempo](https://docs.openlit.io/latest/connections/prometheus-tempo)
+- [✅ Prometheus + Jaeger](https://docs.openlit.io/latest/connections/prometheus-jaeger)
+- [✅ Grafana Cloud](https://docs.openlit.io/latest/connections/grafanacloud)
+- [✅ DataDog](https://docs.openlit.io/latest/connections/datadog)
+- [✅ New Relic](https://docs.openlit.io/latest/connections/new-relic)
+- [✅ SigNoz](https://docs.openlit.io/latest/connections/signoz)
+- [✅ Dynatrace](https://docs.openlit.io/latest/connections/dynatrace)
+- [✅ OpenObserve](https://docs.openlit.io/latest/connections/openobserve)
+- [✅ Highlight.io](https://docs.openlit.io/latest/connections/highlight)
 
 ## 💿 Installation
 
 ```bash
 pip install openlit
 ```
```

### Comparing `openlit-1.2.0/pyproject.toml` & `openlit-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlit"
-version = "1.2.0"
+version = "1.3.0"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
 repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
 homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
```

### Comparing `openlit-1.2.0/src/openlit/__helpers.py` & `openlit-1.3.0/src/openlit/__helpers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/__init__.py` & `openlit-1.3.0/src/openlit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from openlit.instrumentation.openai import OpenAIInstrumentor
 from openlit.instrumentation.anthropic import AnthropicInstrumentor
 from openlit.instrumentation.cohere import CohereInstrumentor
 from openlit.instrumentation.mistral import MistralInstrumentor
 from openlit.instrumentation.bedrock import BedrockInstrumentor
 from openlit.instrumentation.vertexai import VertexAIInstrumentor
 from openlit.instrumentation.langchain import LangChainInstrumentor
+from openlit.instrumentation.llamaindex import LlamaIndexInstrumentor
+from openlit.instrumentation.haystack import HaystackInstrumentor
 from openlit.instrumentation.chroma import ChromaInstrumentor
 from openlit.instrumentation.pinecone import PineconeInstrumentor
 from openlit.instrumentation.transformers import TransformersInstrumentor
 
 # Set up logging for error and information messages.
 logger = logging.getLogger(__name__)
 
@@ -146,14 +148,16 @@
         "openai": "openai",
         "anthropic": "anthropic",  
         "cohere": "cohere",  
         "mistral": "mistralai",
         "bedrock": "boto3",
         "vertexai": "vertexai",
         "langchain": "langchain",
+        "llama_index": "llama_index",
+        "haystack": "haystack",
         "chroma": "chromadb",
         "pinecone": "pinecone",
         "transformers": "transformers"
     }
 
     invalid_instrumentors = [name for name in disabled_instrumentors if name not in module_name_map]
     for invalid_name in invalid_instrumentors:
@@ -194,14 +198,16 @@
             "openai": OpenAIInstrumentor(),
             "anthropic": AnthropicInstrumentor(),
             "cohere": CohereInstrumentor(),
             "mistral": MistralInstrumentor(),
             "bedrock": BedrockInstrumentor(),
             "vertexai": VertexAIInstrumentor(),
             "langchain": LangChainInstrumentor(),
+            "llama_index": LlamaIndexInstrumentor(),
+            "haystack": HaystackInstrumentor(),
             "chroma": ChromaInstrumentor(),
             "pinecone": PineconeInstrumentor(),
             "transformers": TransformersInstrumentor()
         }
 
         # Initialize and instrument only the enabled instrumentors
         for name, instrumentor in instrumentor_instances.items():
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-1.3.0/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument
+# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument, possibly-used-before-assignment
 """
 Module for monitoring Anthropic API calls.
 """
 
 import logging
 from opentelemetry.trace import SpanKind, Status, StatusCode
 from opentelemetry.sdk.resources import TELEMETRY_SDK_NAME
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-1.3.0/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument
+# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument, possibly-used-before-assignment
 """
 Module for monitoring Anthropic API calls.
 """
 
 import logging
 from opentelemetry.trace import SpanKind, Status, StatusCode
 from opentelemetry.sdk.resources import TELEMETRY_SDK_NAME
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/bedrock/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/bedrock/bedrock.py` & `openlit-1.3.0/src/openlit/instrumentation/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/chroma/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/chroma/chroma.py` & `openlit-1.3.0/src/openlit/instrumentation/chroma/chroma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument
+# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument, possibly-used-before-assignment
 """
 Module for monitoring ChromaDB.
 """
 
 import logging
 from opentelemetry.trace import SpanKind, Status, StatusCode
 from opentelemetry.sdk.resources import TELEMETRY_SDK_NAME
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/cohere/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/cohere/cohere.py` & `openlit-1.3.0/src/openlit/instrumentation/cohere/cohere.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument
+# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument, possibly-used-before-assignment
 """
 Module for monitoring Cohere API calls.
 """
 
 import logging
 from opentelemetry.trace import SpanKind, Status, StatusCode
 from opentelemetry.sdk.resources import TELEMETRY_SDK_NAME
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/langchain/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/langchain/langchain.py` & `openlit-1.3.0/src/openlit/instrumentation/langchain/langchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         """
         with tracer.start_as_current_span(gen_ai_endpoint, kind= SpanKind.CLIENT) as span:
             response = wrapped(*args, **kwargs)
 
             try:
                 span.set_attribute(TELEMETRY_SDK_NAME, "openlit")
                 span.set_attribute(SemanticConvetion.GEN_AI_SYSTEM,
-                                    "langchain")
+                                    SemanticConvetion.GEN_AI_SYSTEM_LANGCHAIN)
                 span.set_attribute(SemanticConvetion.GEN_AI_ENDPOINT,
                                     gen_ai_endpoint)
                 span.set_attribute(SemanticConvetion.GEN_AI_ENVIRONMENT,
                                     environment)
                 span.set_attribute(SemanticConvetion.GEN_AI_TYPE,
                                     SemanticConvetion.GEN_AI_TYPE_FRAMEWORK)
                 span.set_attribute(SemanticConvetion.GEN_AI_APPLICATION_NAME,
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/mistral/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-1.3.0/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument
+# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument, possibly-used-before-assignment
 """
 Module for monitoring Mistral API calls.
 """
 
 import logging
 from opentelemetry.trace import SpanKind, Status, StatusCode
 from opentelemetry.sdk.resources import TELEMETRY_SDK_NAME
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/mistral/mistral.py` & `openlit-1.3.0/src/openlit/instrumentation/mistral/mistral.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument
+# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument, possibly-used-before-assignment
 """
 Module for monitoring Mistral API calls.
 """
 
 import logging
 from opentelemetry.trace import SpanKind, Status, StatusCode
 from opentelemetry.sdk.resources import TELEMETRY_SDK_NAME
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/openai/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-1.3.0/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/openai/async_openai.py` & `openlit-1.3.0/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-1.3.0/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/openai/openai.py` & `openlit-1.3.0/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-1.3.0/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument
+# pylint: disable=duplicate-code, broad-exception-caught, too-many-statements, unused-argument, possibly-used-before-assignment
 """
 Module for monitoring Pinecone.
 """
 
 import logging
 from opentelemetry.trace import SpanKind, Status, StatusCode
 from opentelemetry.sdk.resources import TELEMETRY_SDK_NAME
```

### Comparing `openlit-1.2.0/src/openlit/instrumentation/transformers/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/transformers/transformers.py` & `openlit-1.3.0/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/vertexai/__init__.py` & `openlit-1.3.0/src/openlit/instrumentation/vertexai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/vertexai/async_vertexai.py` & `openlit-1.3.0/src/openlit/instrumentation/vertexai/async_vertexai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/instrumentation/vertexai/vertexai.py` & `openlit-1.3.0/src/openlit/instrumentation/vertexai/vertexai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/otel/metrics.py` & `openlit-1.3.0/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/otel/tracing.py` & `openlit-1.3.0/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-1.2.0/src/openlit/semcov/__init__.py` & `openlit-1.3.0/src/openlit/semcov/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     GEN_AI_SYSTEM_AZURE_OPENAI = "azure_openai"
     GEN_AI_SYSTEM_ANTHROPIC = "anthropic"
     GEN_AI_SYSTEM_COHERE = "cohere"
     GEN_AI_SYSTEM_MISTRAL = "mistral"
     GEN_AI_SYSTEM_BEDROCK = "bedrock"
     GEN_AI_SYSTEM_VERTEXAI = "vertexai"
     GEN_AI_SYSTEM_LANGCHAIN = "langchain"
+    GEN_AI_SYSTEM_LLAMAINDEX = "llama_index"
+    GEN_AI_SYSTEM_HAYSTACK = "haystack"
 
     # Vector DB
     DB_REQUESTS = "db.total.requests"
     DB_SYSTEM = "db.system"
     DB_SYSTEM_CHROMA = "chroma"
     DB_SYSTEM_PINECONE = "pinecone"
     DB_COLLECTION_NAME = "db.collection.name"
```

### Comparing `openlit-1.2.0/PKG-INFO` & `openlit-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlit
-Version: 1.2.0
+Version: 1.3.0
 Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
 Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
 Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
 Author: OpenLIT
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -45,38 +45,44 @@
 Whether you're directly using LLM Libraries like OpenAI, Anthropic or building complex RAG Agents using Langchain, OpenLIT seamlessly integrates observability into your applications, ensuring enhanced performance and reliability across diverse scenarios.
 
 This project adheres to the [Semantic Conventions](https://github.com/open-telemetry/semantic-conventions/tree/main/docs/gen-ai) proposed by the OpenTelemetry community. You can check out the current definitions [here](src/openlit/semcov/__init__.py).
 
 ## What can be Auto Instrumented?
 
 ### LLMs
-- ✅ OpenAI
-- ✅ Anthropic
-- ✅ Cohere
-- ✅ Mistral
-- ✅ Azure OpenAI
-- ✅ HuggingFace Transformers
+- [✅ OpenAI](https://docs.openlit.io/latest/integrations/openai)
+- [✅ Anthropic](https://docs.openlit.io/latest/integrations/anthropic)
+- [✅ Cohere](https://docs.openlit.io/latest/integrations/cohere)
+- [✅ Mistral](https://docs.openlit.io/latest/integrations/mistral)
+- [✅ Azure OpenAI](https://docs.openlit.io/latest/integrations/azure-openai)
+- [✅ HuggingFace Transformers](https://docs.openlit.io/latest/integrations/huggingface)
+- [✅ Amazon Bedrock](https://docs.openlit.io/latest/integrations/bedrock)
+- [✅ Vertex AI](https://docs.openlit.io/latest/integrations/vertexai)
 
 ### Vector DBs
-- ✅ ChromaDB
-- ✅ Pinecone
+- [✅ ChromaDB](https://docs.openlit.io/latest/integrations/chromadb)
+- [✅ Pinecone](https://docs.openlit.io/latest/integrations/pinecone)
 
 ### Frameworks
-- ✅ Langchain
-- ✅ LiteLLM
+- [✅ Langchain](https://docs.openlit.io/latest/integrations/langchain)
+- [✅ LiteLLM](https://docs.openlit.io/latest/integrations/litellm)
+- [✅ LlamaIndex](https://docs.openlit.io/latest/integrations/llama-index)
+- [✅ Haystack](https://docs.openlit.io/latest/integrations/haystack)
 
 ## Supported Destinations
-- ✅ OpenTelemetry Collector
-- ✅ Grafana Cloud
-- ✅ Grafana Tempo
-- ✅ DataDog
-- ✅ New Relic
-- ✅ SigNoz
-- ✅ Dynatrace
-- ✅ OpenObserve
+- [✅ OpenTelemetry Collector](https://docs.openlit.io/latest/connections/otelcol)
+- [✅ Prometheus + Tempo](https://docs.openlit.io/latest/connections/prometheus-tempo)
+- [✅ Prometheus + Jaeger](https://docs.openlit.io/latest/connections/prometheus-jaeger)
+- [✅ Grafana Cloud](https://docs.openlit.io/latest/connections/grafanacloud)
+- [✅ DataDog](https://docs.openlit.io/latest/connections/datadog)
+- [✅ New Relic](https://docs.openlit.io/latest/connections/new-relic)
+- [✅ SigNoz](https://docs.openlit.io/latest/connections/signoz)
+- [✅ Dynatrace](https://docs.openlit.io/latest/connections/dynatrace)
+- [✅ OpenObserve](https://docs.openlit.io/latest/connections/openobserve)
+- [✅ Highlight.io](https://docs.openlit.io/latest/connections/highlight)
 
 ## 💿 Installation
 
 ```bash
 pip install openlit
 ```
```

