# Comparing `tmp/langtrace_python_sdk-2.0.5.tar.gz` & `tmp/langtrace_python_sdk-2.0.6.tar.gz`

## Comparing `langtrace_python_sdk-2.0.5.tar` & `langtrace_python_sdk-2.0.6.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    37263 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/conftest.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/conftest.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_chat.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_embed.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_rerank.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_chat.yaml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
--rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_embed.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_rerank.yaml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/LICENSE
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     9582 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    37263 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/LICENSE
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/README.md
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9582 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.6/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.0.5/src/run_example.py` & `langtrace_python_sdk-2.0.6/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.0.6/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.0.6/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.0.6/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.0.6/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.0.6/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.0.6/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.0.6/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.0.6/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.0.6/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.0.6/src/examples/langchain_example/groq_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.0.6/src/examples/langchain_example/langgraph_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.0.6/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.0.6/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.0.6/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.0.6/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.6/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.0.6/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.0.6/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.0.6/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.0.6/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.6/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.0.6/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.0.6/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.0.6/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.0.6/src/examples/qdrant_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/langtrace.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 def init(
     api_key: str = None,
     batch: bool = True,
     write_spans_to_console: bool = False,
     custom_remote_exporter=None,
     api_host: Optional[str] = None,
-    disable_instrumentations: Optional[DisableInstrumentations] = {},
+    disable_instrumentations: Optional[DisableInstrumentations] = None,
 ):
     provider = TracerProvider()
 
     remote_write_exporter = (
         LangTraceExporter(api_key=api_key, api_host=api_host)
         if custom_remote_exporter is None
         else custom_remote_exporter
@@ -121,14 +121,18 @@
 
     init_instrumentations(disable_instrumentations, all_instrumentations)
 
 
 def init_instrumentations(
     disable_instrumentations: DisableInstrumentations, all_instrumentations: dict
 ):
+    if disable_instrumentations is None:
+        for _, v in all_instrumentations.items():
+            v.instrument()
+            return
     validate_instrumentations(disable_instrumentations)
 
     for key in disable_instrumentations:
         for vendor in disable_instrumentations[key]:
             if key == "only":
                 filtered_dict = {
                     k: v for k, v in all_instrumentations.items() if k != vendor.value
@@ -141,15 +145,14 @@
                 }
 
                 for _, v in filtered_dict.items():
                     v.instrument()
 
 
 def validate_instrumentations(disable_instrumentations):
-
     if disable_instrumentations is not None:
         for key, value in disable_instrumentations.items():
             if isinstance(value, str):
                 # Convert single string to list of enum values
                 disable_instrumentations[key] = [InstrumentationType.from_string(value)]
             elif isinstance(value, list):
                 # Convert list of strings to list of enum values
```

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/patch.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/instrumentation/qdrant/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/types/__init__.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.0.6/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/conftest.py` & `langtrace_python_sdk-2.0.6/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/utils.py` & `langtrace_python_sdk-2.0.6/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.0.6/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.0.6/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.0.6/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.6/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.6/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.0.6/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/cohere/conftest.py` & `langtrace_python_sdk-2.0.6/src/tests/cohere/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_chat.py` & `langtrace_python_sdk-2.0.6/src/tests/cohere/test_cohere_chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_embed.py` & `langtrace_python_sdk-2.0.6/src/tests/cohere/test_cohere_embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_rerank.py` & `langtrace_python_sdk-2.0.6/src/tests/cohere/test_cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_chat.yaml` & `langtrace_python_sdk-2.0.6/src/tests/cohere/cassettes/test_cohere_chat.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml` & `langtrace_python_sdk-2.0.6/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_embed.yaml` & `langtrace_python_sdk-2.0.6/src/tests/cohere/cassettes/test_cohere_embed.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_rerank.yaml` & `langtrace_python_sdk-2.0.6/src/tests/cohere/cassettes/test_cohere_rerank.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.0.6/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-2.0.6/src/tests/langchain/test_langchain_community.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.0.6/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.0.6/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.0.6/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.0.6/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.0.6/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.0.6/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/.gitignore` & `langtrace_python_sdk-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/LICENSE` & `langtrace_python_sdk-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/README.md` & `langtrace_python_sdk-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/pyproject.toml` & `langtrace_python_sdk-2.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.5/PKG-INFO` & `langtrace_python_sdk-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

