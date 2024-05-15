# Comparing `tmp/langtrace_python_sdk-2.0.4.tar.gz` & `tmp/langtrace_python_sdk-2.0.5.tar.gz`

## Comparing `langtrace_python_sdk-2.0.4.tar` & `langtrace_python_sdk-2.0.5.tar`

### file list

```diff
@@ -1,130 +1,131 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    25572 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    36645 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/conftest.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/conftest.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_chat.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_embed.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_rerank.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_chat.yaml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
--rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_embed.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_rerank.yaml
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/LICENSE
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    37263 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/LICENSE
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/README.md
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     9582 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.5/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.0.4/src/run_example.py` & `langtrace_python_sdk-2.0.5/src/run_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-
 # Cohere
 # from examples.cohere_example.chat import chat_comp
 # from examples.cohere_example.chat_stream import chat_stream
 # from examples.cohere_example.tools import tool_calling
 # from examples.cohere_example.embed import embed
-from examples.cohere_example.rerank import rerank
+# from examples.cohere_example.rerank import rerank
 
 # OpenAI
 
 # from examples.openai_example.tool_calling import tool_calling
 # from examples.openai_example.chat_completion import chat_completion
 # from examples.openai_example.images_generate import images_generate
 # from examples.openai_example.embeddings_create import embeddings_create
@@ -21,15 +20,16 @@
 # import asyncio
 
 # Anthropic
 # from examples.anthropic_example.completion import messages_create
 
 # Rest
 # from examples.langchain_example.basic import basic, load_and_split, rag
-# from examples.pinecone_example.basic import basic
+from examples.pinecone_example.basic import basic
+
 # from examples.chroma_example.basic import basic
 # from examples.llamaindex_example.basic import basic
 # from examples.langchain_example.basic import basic
 # from examples.hiveagent_example.basic import basic
 # from examples.perplexity_example.basic import basic
 
 # OpenAI
@@ -45,12 +45,12 @@
 # messages_create()
 
 # Cohere
 # chat_comp()
 # chat_stream()
 # tool_calling()
 # embed()
-rerank()
+# rerank()
 
 # load_and_split()
 # rag()
-# basic()
+basic()
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.0.5/src/examples/anthropic_example/completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import anthropic
 from dotenv import find_dotenv, load_dotenv
 
 from langtrace_python_sdk import langtrace, with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 
 
 @with_langtrace_root_span("messages_create")
 def messages_create():
 
     client = anthropic.Anthropic()
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.0.5/src/examples/chroma_example/basic.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dotenv import find_dotenv, load_dotenv
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 
 
 @with_langtrace_root_span()
 def basic():
     chroma_client = chromadb.Client()
     embedder = embedding_functions.DefaultEmbeddingFunction()
     collection = chroma_client.create_collection(
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.0.5/src/examples/cohere_example/chat_stream.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import cohere
 from dotenv import find_dotenv, load_dotenv
 
 from langtrace_python_sdk import langtrace
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
+
 
 co = cohere.Client()
 
 
 # @with_langtrace_root_span("chat_stream")
 def chat_stream():
     result = []
-    for event in co.chat_stream(message="Tell me a short story in 2 lines", preamble="Respond like a pirate", max_tokens=100):
+    for event in co.chat_stream(
+        message="Tell me a short story in 2 lines",
+        preamble="Respond like a pirate",
+        max_tokens=100,
+    ):
         if event.event_type == "text-generation":
             result.append(event.text)
         elif event.event_type == "stream-end":
             break
     print("".join(result))
     return result
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.0.5/src/examples/cohere_example/embed.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from langtrace_python_sdk import langtrace
 
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
+
 
 co = cohere.Client()
 
 
 # @with_langtrace_root_span("embed_create")
 def embed():
     response = co.embed(
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.0.5/src/examples/cohere_example/rerank.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from langtrace_python_sdk import langtrace
 
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
+
 
 co = cohere.Client()
 
 
 # @with_langtrace_root_span("embed_create")
 def rerank():
     docs = [
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.0.5/src/examples/cohere_example/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,28 +3,44 @@
 import cohere
 from dotenv import find_dotenv, load_dotenv
 
 from langtrace_python_sdk import langtrace
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 
 co = cohere.Client()
 
 
 student_custom_functions = [
     {
         "name": "extract_student_info",
         "description": "Get the student information from the body of the input text",
         "parameter_definitions": {
-            "name": {"type": "string", "description": "Name of the person", "required": True},
-            "major": {"type": "string", "description": "Major subject.", "required": True},
-            "school": {"type": "string", "description": "The university name.", "required": True},
-            "grades": {"type": "integer", "description": "GPA of the student.", "required": True},
+            "name": {
+                "type": "string",
+                "description": "Name of the person",
+                "required": True,
+            },
+            "major": {
+                "type": "string",
+                "description": "Major subject.",
+                "required": True,
+            },
+            "school": {
+                "type": "string",
+                "description": "The university name.",
+                "required": True,
+            },
+            "grades": {
+                "type": "integer",
+                "description": "GPA of the student.",
+                "required": True,
+            },
             "club": {
                 "type": "string",
                 "description": "School club for extracurricular activities. ",
                 "required": False,
             },
         },
     }
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.0.5/src/examples/fastapi_example/basic_route.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from langchain_core.prompts.chat import ChatPromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from langchain_openai import ChatOpenAI, OpenAIEmbeddings
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 app = FastAPI()
 client = OpenAI()
 
 
 @app.get("/")
 def root():
     vectorstore = FAISS.from_texts(
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.0.5/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.0.5/src/examples/langchain_example/groq_example.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,13 +18,15 @@
     chat = ChatGroq(temperature=0, model_name="mixtral-8x7b-32768")
 
     system = "You are a helpful assistant."
     human = "{text}"
     prompt = ChatPromptTemplate.from_messages([("system", system), ("human", human)])
 
     chain = prompt | chat
-    result = chain.invoke({"text": "Explain the importance of low latency LLMs in 2 sentences or less."})
+    result = chain.invoke(
+        {"text": "Explain the importance of low latency LLMs in 2 sentences or less."}
+    )
     # print(result)
     return result
 
 
 groq_example()
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.0.5/src/examples/langchain_example/langgraph_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,37 +44,36 @@
     for tool_call in tool_calls:
         if tool_call.get("function").get("name") == "multiply":
             multiply_call = tool_call
 
     if multiply_call is None:
         raise Exception("No adder input found.")
 
-    res = multiply.invoke(
-        json.loads(multiply_call.get("function").get("arguments"))
-    )
+    res = multiply.invoke(json.loads(multiply_call.get("function").get("arguments")))
 
-    return ToolMessage(
-        tool_call_id=multiply_call.get("id"),
-        content=res
-    )
+    return ToolMessage(tool_call_id=multiply_call.get("id"), content=res)
 
 
-@with_langtrace_root_span('langgraph_example')
+@with_langtrace_root_span("langgraph_example")
 def basic():
 
     graph = MessageGraph()
 
     graph.add_node("oracle", invoke_model)
 
     graph.add_node("multiply", invoke_tool)
 
-    graph.add_conditional_edges("oracle", router, {
-        "multiply": "multiply",
-        "end": END,
-    })
+    graph.add_conditional_edges(
+        "oracle",
+        router,
+        {
+            "multiply": "multiply",
+            "end": END,
+        },
+    )
 
     graph.add_edge("multiply", END)
 
     graph.set_entry_point("oracle")
 
     runnable = graph.compile()
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.0.5/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openai.types.chat import ChatCompletionMessageToolCall
 from langtrace_python_sdk import langtrace
 
 import nest_asyncio
 
 nest_asyncio.apply()
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 
 
 def multiply(a: int, b: int) -> int:
     """Multiple two integers and returns the result integer"""
     return a * b
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 
 
 @with_langtrace_root_span()
 def basic():
     documents = SimpleDirectoryReader(
         "src/examples/llamaindex_example/data"
     ).load_data()
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.0.5/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.5/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,43 @@
 
 from langtrace_python_sdk import langtrace
 
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 
 client = AsyncOpenAI()
 
+
 # Example dummy function hard coded to return the same weather
 # In production, this could be your backend API or an external API
 def get_current_weather(location, unit="fahrenheit"):
     """Get the current weather in a given location"""
     if "tokyo" in location.lower():
         return json.dumps({"location": "Tokyo", "temperature": "10", "unit": unit})
     elif "san francisco" in location.lower():
-        return json.dumps({"location": "San Francisco", "temperature": "72", "unit": unit})
+        return json.dumps(
+            {"location": "San Francisco", "temperature": "72", "unit": unit}
+        )
     elif "paris" in location.lower():
         return json.dumps({"location": "Paris", "temperature": "22", "unit": unit})
     else:
         return json.dumps({"location": location, "temperature": "unknown"})
 
 
 async def run_conversation():
     # Step 1: send the conversation and available functions to the model
-    messages = [{"role": "user", "content": "What's the weather like in San Francisco, Tokyo, and Paris?"}]
+    messages = [
+        {
+            "role": "user",
+            "content": "What's the weather like in San Francisco, Tokyo, and Paris?",
+        }
+    ]
     tools = [
         {
             "type": "function",
             "function": {
                 "name": "get_current_weather",
                 "description": "Get the current weather in a given location",
                 "parameters": {
@@ -86,8 +94,7 @@
             )  # extend conversation with function response
         second_response = await client.chat.completions.create(
             model="gpt-3.5-turbo-0125",
             messages=messages,
         )  # get a new response from the model where it can see the function response
         # print(second_response)
         return second_response
-
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.0.5/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 
 from langtrace_python_sdk import langtrace
 
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 
 client = AsyncOpenAI()
 
 
 # Example dummy function hard coded to return the same weather
 # In production, this could be your backend API or an external API
 def get_current_weather(location, unit="fahrenheit"):
     """Get the current weather in a given location"""
     if "tokyo" in location.lower():
         return json.dumps({"location": "Tokyo", "temperature": "10", "unit": unit})
     elif "san francisco" in location.lower():
-        return json.dumps({"location": "San Francisco", "temperature": "72", "unit": unit})
+        return json.dumps(
+            {"location": "San Francisco", "temperature": "72", "unit": unit}
+        )
     elif "paris" in location.lower():
         return json.dumps({"location": "Paris", "temperature": "22", "unit": unit})
     else:
         return json.dumps({"location": location, "temperature": "unknown"})
 
 
 def get_current_time(location):
@@ -38,15 +40,20 @@
         return json.dumps({"location": "Paris", "time": "22"})
     else:
         return json.dumps({"location": location, "time": "unknown"})
 
 
 async def run_conversation():
     # Step 1: send the conversation and available functions to the model
-    messages = [{"role": "user", "content": "What's the weather like in San Francisco, Tokyo, and Paris?"}]
+    messages = [
+        {
+            "role": "user",
+            "content": "What's the weather like in San Francisco, Tokyo, and Paris?",
+        }
+    ]
     tools = [
         {
             "type": "function",
             "function": {
                 "name": "get_current_weather",
                 "description": "Get the current weather in a given location",
                 "parameters": {
@@ -74,15 +81,15 @@
                             "type": "string",
                             "description": "The city and state, e.g. San Francisco, CA",
                         },
                     },
                     "required": ["location"],
                 },
             },
-        }
+        },
     ]
     response = await client.chat.completions.create(
         model="gpt-4",
         messages=messages,
         tools=tools,
         tool_choice="auto",  # auto is default, but we'll be explicit
         stream=True,
@@ -91,37 +98,42 @@
     # For streaming, uncomment the following lines
     tool_call_dict = {}
     tool_calls = []
     id = ""
     name = ""
     arguments = ""
     async for chunk in response:
-        if chunk.choices[0].delta is not None and chunk.choices[0].delta.tool_calls is not None:
+        if (
+            chunk.choices[0].delta is not None
+            and chunk.choices[0].delta.tool_calls is not None
+        ):
             for choice in chunk.choices:
                 for tool_call in choice.delta.tool_calls:
                     if tool_call.id and id != tool_call.id:
                         id = tool_call.id if tool_call.id else ""
-                        name = tool_call.function.name if tool_call.function and tool_call.function.name else ""
+                        name = (
+                            tool_call.function.name
+                            if tool_call.function and tool_call.function.name
+                            else ""
+                        )
                         tool_call_dict[name] = {
                             "id": id,
-                            "function": {
-                                "name": name,
-                                "arguments": arguments
-                            },
-                            "type": "function"
+                            "function": {"name": name, "arguments": arguments},
+                            "type": "function",
                         }
-                    arguments += tool_call.function.arguments if tool_call.function and tool_call.function.arguments else ""
+                    arguments += (
+                        tool_call.function.arguments
+                        if tool_call.function and tool_call.function.arguments
+                        else ""
+                    )
                 if name != "":
                     tool_call_dict[name] = {
                         "id": id,
-                        "function": {
-                            "name": name,
-                            "arguments": arguments
-                        },
-                        "type": "function"
+                        "function": {"name": name, "arguments": arguments},
+                        "type": "function",
                     }
     for key, value in tool_call_dict.items():
         tool_calls.append(value)
 
     # Step 2: check if the model wanted to call a function
     if tool_calls:
         # Step 3: call the function
@@ -129,39 +141,39 @@
         available_functions = {
             "get_current_weather": get_current_weather,
             "get_current_time": get_current_time,
         }  # only one function in this example, but you can have multiple
         # messages.append(response_message)  # extend conversation with assistant's reply
         # Step 4: send the info for each function call and function response to the model
         for tool_call in tool_calls:
-            function_name = tool_call['function']['name']
+            function_name = tool_call["function"]["name"]
             function_to_call = available_functions[function_name]
-            function_args = json.loads(tool_call['function']['arguments'])
+            function_args = json.loads(tool_call["function"]["arguments"])
             function_response = function_to_call(
                 location=function_args.get("location"),
                 unit=function_args.get("unit"),
             )
             func_res = json.loads(function_response)
             content = f"Use the below information to answer the user's question: The current weather in {func_res['location']} is {func_res['temperature']} degrees {func_res['unit']}"
             messages.append(
-                {
-                    "role": "system",
-                    "content": content
-                }
+                {"role": "system", "content": content}
             )  # extend conversation with function response
         print(messages)
         second_response = await client.chat.completions.create(
             model="gpt-4",
             messages=messages,
             stream=True,
         )  # get a new response from the model where it can see the function response
         result = []
         async for chunk in second_response:
             if chunk.choices[0].delta.content is not None:
                 content = [
-                    choice.delta.content if choice.delta and
-                    choice.delta.content else ""
-                    for choice in chunk.choices]
-                result.append(
-                    content[0] if len(content) > 0 else "")
+                    (
+                        choice.delta.content
+                        if choice.delta and choice.delta.content
+                        else ""
+                    )
+                    for choice in chunk.choices
+                ]
+                result.append(content[0] if len(content) > 0 else "")
         print("".join(result))
-        # return second_response
+        # return second_response
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.0.5/src/examples/openai_example/chat_completion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from dotenv import find_dotenv, load_dotenv
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import (
-    with_additional_attributes, with_langtrace_root_span)
+    with_additional_attributes,
+    with_langtrace_root_span,
+)
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 client = OpenAI()
 
 
 # @with_additional_attributes({"user.id": "1234", "user.feedback.rating": 1})
 def api():
     response = client.chat.completions.create(
         model="gpt-4",
-        messages=[{"role": "system", "content": "Talk like a pirate"}, {"role": "user", "content": "Tell me a story in 3 sentences or less."}],
+        messages=[
+            {"role": "system", "content": "Talk like a pirate"},
+            {"role": "user", "content": "Tell me a story in 3 sentences or less."},
+        ],
         stream=True,
         # stream=False,
     )
     return response
 
 
 # @with_langtrace_root_span()
@@ -27,15 +32,14 @@
     response = api()
     # print(response)
     # Uncomment this for streaming
     result = []
     for chunk in response:
         if chunk.choices[0].delta.content is not None:
             content = [
-                choice.delta.content if choice.delta and
-                choice.delta.content else ""
-                for choice in chunk.choices]
-            result.append(
-                content[0] if len(content) > 0 else "")
+                choice.delta.content if choice.delta and choice.delta.content else ""
+                for choice in chunk.choices
+            ]
+            result.append(content[0] if len(content) > 0 else "")
 
     print("".join(result))
     return response
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.0.5/src/examples/openai_example/function_calling.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from dotenv import find_dotenv, load_dotenv
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
+
 
 client = OpenAI()
 
 
 student_custom_functions = [
     {
         "name": "extract_student_info",
@@ -47,18 +48,22 @@
     )
     # return response
 
     result = []
     for chunk in response:
         if chunk.choices[0].delta.function_call is not None:
             content = [
-                choice.delta.function_call.arguments if choice.delta.function_call and
-                choice.delta.function_call.arguments else ""
-                for choice in chunk.choices]
-            result.append(
-                content[0] if len(content) > 0 else "")
+                (
+                    choice.delta.function_call.arguments
+                    if choice.delta.function_call
+                    and choice.delta.function_call.arguments
+                    else ""
+                )
+                for choice in chunk.choices
+            ]
+            result.append(content[0] if len(content) > 0 else "")
 
     print("".join(result))
 
     # Loading the response as a JSON object
     # json_response = json.loads(response.choices[0].message.function_call.arguments)
     # print(json_response)
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dotenv import find_dotenv, load_dotenv
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 
 client = OpenAI()
 
 
 student_custom_functions = [
     {
         "type": "function",
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,36 +5,44 @@
 
 from langtrace_python_sdk import langtrace
 
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
+
 
 client = OpenAI()
 
 
 # Example dummy function hard coded to return the same weather
 # In production, this could be your backend API or an external API
 def get_current_weather(location, unit="fahrenheit"):
     """Get the current weather in a given location"""
     if "tokyo" in location.lower():
         return json.dumps({"location": "Tokyo", "temperature": "10", "unit": unit})
     elif "san francisco" in location.lower():
-        return json.dumps({"location": "San Francisco", "temperature": "72", "unit": unit})
+        return json.dumps(
+            {"location": "San Francisco", "temperature": "72", "unit": unit}
+        )
     elif "paris" in location.lower():
         return json.dumps({"location": "Paris", "temperature": "22", "unit": unit})
     else:
         return json.dumps({"location": location, "temperature": "unknown"})
 
 
 def run_conversation():
     # Step 1: send the conversation and available functions to the model
-    messages = [{"role": "user", "content": "What's the weather like in San Francisco, Tokyo, and Paris?"}]
+    messages = [
+        {
+            "role": "user",
+            "content": "What's the weather like in San Francisco, Tokyo, and Paris?",
+        }
+    ]
     tools = [
         {
             "type": "function",
             "function": {
                 "name": "get_current_weather",
                 "description": "Get the current weather in a given location",
                 "parameters": {
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.0.5/src/examples/openai_example/tool_calling_streaming.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 
 from langtrace_python_sdk import langtrace
 
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
+
 
 client = OpenAI()
 
 
 # Example dummy function hard coded to return the same weather
 # In production, this could be your backend API or an external API
 def get_current_weather(location, unit="fahrenheit"):
     """Get the current weather in a given location"""
     if "tokyo" in location.lower():
         return json.dumps({"location": "Tokyo", "temperature": "10", "unit": unit})
     elif "san francisco" in location.lower():
-        return json.dumps({"location": "San Francisco", "temperature": "72", "unit": unit})
+        return json.dumps(
+            {"location": "San Francisco", "temperature": "72", "unit": unit}
+        )
     elif "paris" in location.lower():
         return json.dumps({"location": "Paris", "temperature": "22", "unit": unit})
     else:
         return json.dumps({"location": location, "temperature": "unknown"})
 
 
 def get_current_time(location):
@@ -38,15 +41,20 @@
         return json.dumps({"location": "Paris", "time": "22"})
     else:
         return json.dumps({"location": location, "time": "unknown"})
 
 
 def run_conversation():
     # Step 1: send the conversation and available functions to the model
-    messages = [{"role": "user", "content": "What's the weather like in San Francisco, Tokyo, and Paris?"}]
+    messages = [
+        {
+            "role": "user",
+            "content": "What's the weather like in San Francisco, Tokyo, and Paris?",
+        }
+    ]
     tools = [
         {
             "type": "function",
             "function": {
                 "name": "get_current_weather",
                 "description": "Get the current weather in a given location",
                 "parameters": {
@@ -74,15 +82,15 @@
                             "type": "string",
                             "description": "The city and state, e.g. San Francisco, CA",
                         },
                     },
                     "required": ["location"],
                 },
             },
-        }
+        },
     ]
     response = client.chat.completions.create(
         model="gpt-4",
         messages=messages,
         tools=tools,
         tool_choice="auto",  # auto is default, but we'll be explicit
         stream=True,
@@ -91,37 +99,42 @@
     # For streaming, uncomment the following lines
     tool_call_dict = {}
     tool_calls = []
     id = ""
     name = ""
     arguments = ""
     for chunk in response:
-        if chunk.choices[0].delta is not None and chunk.choices[0].delta.tool_calls is not None:
+        if (
+            chunk.choices[0].delta is not None
+            and chunk.choices[0].delta.tool_calls is not None
+        ):
             for choice in chunk.choices:
                 for tool_call in choice.delta.tool_calls:
                     if tool_call.id and id != tool_call.id:
                         id = tool_call.id if tool_call.id else ""
-                        name = tool_call.function.name if tool_call.function and tool_call.function.name else ""
+                        name = (
+                            tool_call.function.name
+                            if tool_call.function and tool_call.function.name
+                            else ""
+                        )
                         tool_call_dict[name] = {
                             "id": id,
-                            "function": {
-                                "name": name,
-                                "arguments": arguments
-                            },
-                            "type": "function"
+                            "function": {"name": name, "arguments": arguments},
+                            "type": "function",
                         }
-                    arguments += tool_call.function.arguments if tool_call.function and tool_call.function.arguments else ""
+                    arguments += (
+                        tool_call.function.arguments
+                        if tool_call.function and tool_call.function.arguments
+                        else ""
+                    )
                 if name != "":
                     tool_call_dict[name] = {
                         "id": id,
-                        "function": {
-                            "name": name,
-                            "arguments": arguments
-                        },
-                        "type": "function"
+                        "function": {"name": name, "arguments": arguments},
+                        "type": "function",
                     }
     for key, value in tool_call_dict.items():
         tool_calls.append(value)
 
     # Step 2: check if the model wanted to call a function
     if tool_calls:
         # Step 3: call the function
@@ -129,39 +142,39 @@
         available_functions = {
             "get_current_weather": get_current_weather,
             "get_current_time": get_current_time,
         }  # only one function in this example, but you can have multiple
         # messages.append(response_message)  # extend conversation with assistant's reply
         # Step 4: send the info for each function call and function response to the model
         for tool_call in tool_calls:
-            function_name = tool_call['function']['name']
+            function_name = tool_call["function"]["name"]
             function_to_call = available_functions[function_name]
-            function_args = json.loads(tool_call['function']['arguments'])
+            function_args = json.loads(tool_call["function"]["arguments"])
             function_response = function_to_call(
                 location=function_args.get("location"),
                 unit=function_args.get("unit"),
             )
             func_res = json.loads(function_response)
             content = f"Use the below information to answer the user's question: The current weather in {func_res['location']} is {func_res['temperature']} degrees {func_res['unit']}"
             messages.append(
-                {
-                    "role": "system",
-                    "content": content
-                }
+                {"role": "system", "content": content}
             )  # extend conversation with function response
         print(messages)
         second_response = client.chat.completions.create(
             model="gpt-4",
             messages=messages,
             stream=True,
         )  # get a new response from the model where it can see the function response
         result = []
         for chunk in second_response:
             if chunk.choices[0].delta.content is not None:
                 content = [
-                    choice.delta.content if choice.delta and
-                    choice.delta.content else ""
-                    for choice in chunk.choices]
-                result.append(
-                    content[0] if len(content) > 0 else "")
+                    (
+                        choice.delta.content
+                        if choice.delta and choice.delta.content
+                        else ""
+                    )
+                    for choice in chunk.choices
+                ]
+                result.append(content[0] if len(content) > 0 else "")
         print("".join(result))
-        # return second_response
+        # return second_response
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.0.5/src/examples/perplexity_example/basic.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from langtrace_python_sdk.utils.with_root_span import (
     with_additional_attributes,
     with_langtrace_root_span,
 )
 
 # _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 client = OpenAI(base_url="https://api.perplexity.ai", api_key="PPLX_API_KEY")
 
 
 @with_additional_attributes({"user.id": "1234", "user.feedback.rating": 1})
 def basic():
     response = client.chat.completions.create(
         model="pplx-70b-online",
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.0.5/src/examples/pinecone_example/basic.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from pinecone import Pinecone
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(
+    write_spans_to_console=True,
+    disable_instrumentations={"all_except": ["pinecone", "openai"]},
+)
 
 client = OpenAI()
 pinecone = Pinecone()
 
 
 @with_langtrace_root_span()
 def basic():
```

### Comparing `langtrace_python_sdk-2.0.4/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.0.5/src/examples/qdrant_example/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 from qdrant_client.models import Batch, Distance, VectorParams
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init()
 
 
 @with_langtrace_root_span()
 def basic():
     client = QdrantClient(":memory:")
     cohere_client = cohere.Client()
 
-    client.create_collection(collection_name="MyCollection4", vectors_config=VectorParams(
-        size=1024,
-        distance=Distance.COSINE,
-    ))
+    client.create_collection(
+        collection_name="MyCollection4",
+        vectors_config=VectorParams(
+            size=1024,
+            distance=Distance.COSINE,
+        ),
+    )
 
     client.upsert(
         collection_name="MyCollection4",
         points=Batch(
             ids=[1],
             vectors=cohere_client.embed(
                 model="embed-english-v3.0",  # New Embed v3 model
@@ -36,15 +39,14 @@
     answer = client.search(
         collection_name="MyCollection4",
         query_vector=cohere_client.embed(
             model="embed-english-v3.0",  # New Embed v3 model
             input_type="search_query",  # Input type for search queries
             texts=["Which database is written in Rust?"],
         ).embeddings[0],
-
     )
     print(answer[0])
 
     return answer
 
 
 basic()
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,50 +21,45 @@
 
     - Provides a mechanism to export trace data from your application to a LangTrace collector.
     - Offers a convenient way to send spans with their attributes, events, and links.
 
     **Attributes:**
 
     * `api_key` (str): An API key to authenticate with the LangTrace collector (required).
-    * `write_to_remote_url` (bool): A flag indicating whether to send spans to the remote URL (defaults to False).
 
     **Methods:**
 
-    * `__init__(api_key: str = None, url: str = None, write_to_remote_url: bool = False) -> None`:
+    * `__init__(api_key: str = None, url: str = None) -> None`:
         - Initializes a `LangTraceExporter` instance.
         - Retrieves the API key and URL from environment variables if not provided explicitly.
-        - Raises a `ValueError` if the API key is missing or the URL is missing when `write_to_remote_url` is True.
+        - Raises a `ValueError` if the API key is missing.
     * `export(self, spans: typing.Sequence[ReadableSpan]) -> SpanExportResult`:
         - Exports a batch of `opentelemetry.trace.Span` objects to LangTrace.
         - Converts each span into a dictionary representation including trace ID, instrumentation library, events, dropped data counts, duration, and other span attributes.
-        - If `write_to_remote_url` is False, returns `SpanExportResult.SUCCESS` without sending data.
         - Otherwise, sends the data to the configured URL using a POST request with JSON data and the API key in the header.
         - Returns `SpanExportResult.SUCCESS` on successful export or `SpanExportResult.FAILURE` on errors.
     * `shutdown(self) -> None`:
         - (Optional) Performs any necessary cleanup tasks when the exporter is shut down. Currently does nothing.
 
     **Raises:**
 
-    * `ValueError`: If the API key is not provided or the URL is missing when `write_to_remote_url` is True.
+    * `ValueError`: If the API key is not provided.
     """
 
     api_key: str
-    write_to_remote_url: bool
 
     def __init__(
         self,
         api_key: str = None,
-        write_to_remote_url: bool = False,
         api_host: typing.Optional[str] = None,
     ) -> None:
         self.api_key = api_key or os.environ.get("LANGTRACE_API_KEY")
-        self.write_to_remote_url = write_to_remote_url
         self.api_host: str = api_host or LANGTRACE_REMOTE_URL
 
-        if self.write_to_remote_url and not self.api_key:
+        if not self.api_key:
             raise ValueError("No API key provided")
 
     def export(self, spans: typing.Sequence[ReadableSpan]) -> SpanExportResult:
         """
         Exports a batch of telemetry data.
 
         Args:
@@ -82,17 +77,14 @@
                 "droppedLinksCount": span.dropped_links,
                 "ended": span.status.is_ok,
                 **json.loads(span.to_json()),
             }
             for span in spans
         ]
 
-        if not self.write_to_remote_url:
-            return
-
         # Send data to remote URL
         try:
             requests.post(
                 url=f"{self.api_host}/api/trace",
                 data=json.dumps(data),
                 headers={"Content-Type": "application/json", "x-api-key": self.api_key},
             )
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 import logging
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.instrumentation.anthropic.patch import \
-    messages_create
+from langtrace_python_sdk.instrumentation.anthropic.patch import messages_create
 
 logging.basicConfig(level=logging.FATAL)
 
 
 class AnthropicInstrumentation(BaseInstrumentor):
     """
     The AnthropicInstrumentation class represents the Anthropic instrumentation
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from langtrace.trace_attributes import Event, LLMSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.anthropic import APIS
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
 def messages_create(original_method, version, tracer):
     """Wrap the `messages_create` method."""
 
     def traced_method(wrapped, instance, args, kwargs):
         base_url = (
@@ -54,15 +56,15 @@
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["MESSAGES_CREATE"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.prompts": prompts,
             "llm.stream": kwargs.get("stream"),
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         if kwargs.get("temperature") is not None:
             attributes.llm_temperature = kwargs.get("temperature")
         if kwargs.get("top_p") is not None:
@@ -81,15 +83,18 @@
             if value is not None:
                 span.set_attribute(field, value)
         try:
             # Attempt to call the original method
             result = wrapped(*args, **kwargs)
             if kwargs.get("stream") is False:
                 if hasattr(result, "content") and result.content is not None:
-                    span.set_attribute("llm.model", result.model if result.model else kwargs.get("model"))
+                    span.set_attribute(
+                        "llm.model",
+                        result.model if result.model else kwargs.get("model"),
+                    )
                     span.set_attribute(
                         "llm.responses",
                         json.dumps(
                             [
                                 {
                                     "role": result.role if result.role else "assistant",
                                     "content": result.content[0].text,
@@ -136,15 +141,20 @@
         """Process and yield streaming response chunks."""
         result_content = []
         span.add_event(Event.STREAM_START.value)
         input_tokens = 0
         output_tokens = 0
         try:
             for chunk in result:
-                if hasattr(chunk, "message") and chunk.message is not None and hasattr(chunk.message, "model") and chunk.message.model is not None:
+                if (
+                    hasattr(chunk, "message")
+                    and chunk.message is not None
+                    and hasattr(chunk.message, "model")
+                    and chunk.message.model is not None
+                ):
                     span.set_attribute("llm.model", chunk.message.model)
                 content = ""
                 if hasattr(chunk, "delta") and chunk.delta is not None:
                     content = chunk.delta.text if hasattr(chunk.delta, "text") else ""
                 # Assuming content needs to be aggregated before processing
                 result_content.append(content if len(content) > 0 else "")
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from langtrace.trace_attributes import DatabaseSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.chroma import APIS
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
 def collection_patch(method, version, tracer):
     """
     A generic patch method that wraps a function with a span
     """
 
@@ -38,15 +40,15 @@
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "db.system": "chromadb",
             "db.operation": api["OPERATION"],
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         if hasattr(instance, "name") and instance.name is not None:
             span_attributes["db.collection.name"] = instance.name
 
         attributes = DatabaseSpanAttributes(**span_attributes)
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,20 @@
 import importlib.metadata
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.instrumentation.cohere.patch import (chat_create,
-                                                               chat_stream,
-                                                               embed, rerank)
+from langtrace_python_sdk.instrumentation.cohere.patch import (
+    chat_create,
+    chat_stream,
+    embed,
+    rerank,
+)
 
 
 class CohereInstrumentation(BaseInstrumentor):
     """
     The CohereInstrumentation class represents the Anthropic instrumentation
     """
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.groq.patch import (
-    async_chat_completions_create, chat_completions_create)
+    async_chat_completions_create,
+    chat_completions_create,
+)
 
 logging.basicConfig(level=logging.FATAL)
 
 
 class GroqInstrumentation(BaseInstrumentor):
 
     def instrumentation_dependencies(self) -> Collection[str]:
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 
 from langtrace.trace_attributes import Event, LLMSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 from langtrace_python_sdk.constants.instrumentation.groq import APIS
-from langtrace_python_sdk.utils.llm import (calculate_prompt_tokens,
-                                            estimate_tokens)
+from langtrace_python_sdk.utils.llm import calculate_prompt_tokens, estimate_tokens
 
 
 def chat_completions_create(original_method, version, tracer):
     """Wrap the `create` method of the `ChatCompletion` class to trace it."""
 
     def traced_method(wrapped, instance, args, kwargs):
         base_url = (
@@ -132,15 +133,16 @@
                                     "content_filter_results": choice[
                                         "content_filter_results"
                                     ]
                                 }
                                 if "content_filter_results" in choice
                                 else {}
                             ),
-                        } for choice in result.choices
+                        }
+                        for choice in result.choices
                     ]
                     span.set_attribute("llm.responses", json.dumps(responses))
                 else:
                     responses = []
                     span.set_attribute("llm.responses", json.dumps(responses))
                 if (
                     hasattr(result, "system_fingerprint")
@@ -220,24 +222,30 @@
                                     choice.delta.function_call.arguments
                                 )
                                 completion_tokens += token_counts
                                 content = [choice.delta.function_call.arguments]
                     elif tool_calls:
                         for choice in chunk.choices:
                             tool_call = ""
-                            if (choice.delta and choice.delta.tool_calls is not None):
+                            if choice.delta and choice.delta.tool_calls is not None:
                                 toolcalls = choice.delta.tool_calls
                                 content = []
                                 for tool_call in toolcalls:
-                                    if tool_call and tool_call.function is not None and tool_call.function.arguments is not None:
+                                    if (
+                                        tool_call
+                                        and tool_call.function is not None
+                                        and tool_call.function.arguments is not None
+                                    ):
                                         token_counts = estimate_tokens(
                                             tool_call.function.arguments
                                         )
                                         completion_tokens += token_counts
-                                        content = content + [tool_call.function.arguments]
+                                        content = content + [
+                                            tool_call.function.arguments
+                                        ]
                                     else:
                                         content = content + []
                 else:
                     content = []
                 span.add_event(
                     Event.STREAM_OUTPUT.value,
                     {
@@ -385,15 +393,16 @@
                                     "content_filter_results": choice[
                                         "content_filter_results"
                                     ]
                                 }
                                 if "content_filter_results" in choice
                                 else {}
                             ),
-                        } for choice in result.choices
+                        }
+                        for choice in result.choices
                     ]
                     span.set_attribute("llm.responses", json.dumps(responses))
                 else:
                     responses = []
                     span.set_attribute("llm.responses", json.dumps(responses))
                 if (
                     hasattr(result, "system_fingerprint")
@@ -473,24 +482,30 @@
                                     choice.delta.function_call.arguments
                                 )
                                 completion_tokens += token_counts
                                 content = [choice.delta.function_call.arguments]
                     elif tool_calls:
                         for choice in chunk.choices:
                             tool_call = ""
-                            if (choice.delta and choice.delta.tool_calls is not None):
+                            if choice.delta and choice.delta.tool_calls is not None:
                                 toolcalls = choice.delta.tool_calls
                                 content = []
                                 for tool_call in toolcalls:
-                                    if tool_call and tool_call.function is not None and tool_call.function.arguments is not None:
+                                    if (
+                                        tool_call
+                                        and tool_call.function is not None
+                                        and tool_call.function.arguments is not None
+                                    ):
                                         token_counts = estimate_tokens(
                                             tool_call.function.arguments
                                         )
                                         completion_tokens += token_counts
-                                        content = content + [tool_call.function.arguments]
+                                        content = content + [
+                                            tool_call.function.arguments
+                                        ]
                                     else:
                                         content = content + []
                 else:
                     content = []
                 span.add_event(
                     Event.STREAM_OUTPUT.value,
                     {
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind, StatusCode
 from opentelemetry.trace.status import Status
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
 def generic_patch(
     method_name, task, tracer, version, trace_output=True, trace_input=True
 ):
     """
     patch method for generic methods.
@@ -39,15 +41,15 @@
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         if len(args) > 0 and trace_input:
             span_attributes["langchain.inputs"] = to_json_string(args)
 
         attributes = FrameworkSpanAttributes(**span_attributes)
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 import inspect
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.instrumentation.langchain_community.patch import \
-    generic_patch
+from langtrace_python_sdk.instrumentation.langchain_community.patch import generic_patch
 
 
 def patch_module_classes(
     module_name, tracer, version, task, trace_output=True, trace_input=True
 ):
     """
     Generic function to patch all public methods of all classes in a given module.
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-
 import json
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
 def generic_patch(
     method_name, task, tracer, version, trace_output=True, trace_input=True
 ):
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["LANGCHAIN_COMMUNITY"]
@@ -36,15 +37,15 @@
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         if trace_input and len(args) > 0:
             span_attributes["langchain.inputs"] = to_json_string(args)
 
         attributes = FrameworkSpanAttributes(**span_attributes)
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.langchain_core.patch import (
-    generic_patch, runnable_patch)
+    generic_patch,
+    runnable_patch,
+)
 
 
 # pylint: disable=dangerous-default-value
 def patch_module_classes(
     module_name,
     tracer,
     version,
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind, StatusCode
 from opentelemetry.trace.status import Status
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
 def generic_patch(
     method_name, task, tracer, version, trace_output=True, trace_input=True
 ):
     """
     Wrapper function to trace a generic method.
@@ -45,15 +47,15 @@
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         if len(args) > 0 and trace_input:
             inputs = {}
             for arg in args:
                 if isinstance(arg, dict):
                     for key, value in arg.items():
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 import inspect
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.instrumentation.langgraph.patch import \
-    patch_graph_methods
+from langtrace_python_sdk.instrumentation.langgraph.patch import patch_graph_methods
 
 
 class LanggraphInstrumentation(BaseInstrumentor):
     """
     Instrumentor for langgraph.
     """
 
@@ -37,29 +36,39 @@
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, "", tracer_provider)
         version = importlib.metadata.version("langgraph")
 
         # List of modules to patch, with their corresponding patch names
         modules_to_patch = [
-            ("langgraph.graph.graph", ["add_node", "add_edge", "set_entry_point", "set_finish_point", "add_conditional_edges"]),
+            (
+                "langgraph.graph.graph",
+                [
+                    "add_node",
+                    "add_edge",
+                    "set_entry_point",
+                    "set_finish_point",
+                    "add_conditional_edges",
+                ],
+            ),
         ]
 
         for module_name, methods in modules_to_patch:
             module = importlib.import_module(module_name)
             for name, obj in inspect.getmembers(
                 module,
-                lambda member: inspect.isclass(member) and member.__module__ == module.__name__,
+                lambda member: inspect.isclass(member)
+                and member.__module__ == module.__name__,
             ):
-                for method_name, _ in inspect.getmembers(obj, predicate=inspect.isfunction):
+                for method_name, _ in inspect.getmembers(
+                    obj, predicate=inspect.isfunction
+                ):
                     if method_name in methods:
                         module = f"{name}.{method_name}"
                         wrap_function_wrapper(
                             module_name,
                             module,
-                            patch_graph_methods(
-                                module, tracer, version
-                            ),
+                            patch_graph_methods(module, tracer, version),
                         )
 
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
-def patch_graph_methods(
-    method_name, tracer, version
-):
+def patch_graph_methods(method_name, tracer, version):
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["LANGGRAPH"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attr = get_atrribute_key_value(method_name, args)
         if attr is not None:
             span_attributes.update(attr)
 
         attributes = FrameworkSpanAttributes(**span_attributes)
@@ -71,43 +71,64 @@
 
 def get_atrribute_key_value(method_name, args):
     if args is None or len(args) == 0:
         return None
 
     if "add_node" in method_name:
         return {
-            'langgraph.node': json.dumps({
-                'name': args[0],
-                'action': args[1].json() if hasattr(args[1], 'json') else args[1].__name__ if hasattr(args[1], '__name__') else str(args[1]),
-            }),
-            'langgraph.task.name': 'add_node',
+            "langgraph.node": json.dumps(
+                {
+                    "name": args[0],
+                    "action": (
+                        args[1].json()
+                        if hasattr(args[1], "json")
+                        else (
+                            args[1].__name__
+                            if hasattr(args[1], "__name__")
+                            else str(args[1])
+                        )
+                    ),
+                }
+            ),
+            "langgraph.task.name": "add_node",
         }
     elif "add_edge" in method_name:
         return {
-            'langgraph.edge': json.dumps({
-                'source': args[0],
-                'destination': args[1],
-            }),
-            'langgraph.task.name': 'add_edge',
+            "langgraph.edge": json.dumps(
+                {
+                    "source": args[0],
+                    "destination": args[1],
+                }
+            ),
+            "langgraph.task.name": "add_edge",
         }
     elif "add_conditional_edges" in method_name:
         return {
-            'langgraph.edge': json.dumps({
-                'source': args[0],
-                'path': args[1].json() if hasattr(args[1], 'json') else args[1].__name__ if hasattr(args[1], '__name__') else str(args[1]),
-                'path_map': args[2],
-            }),
-            'langgraph.task.name': 'add_conditional_edges',
+            "langgraph.edge": json.dumps(
+                {
+                    "source": args[0],
+                    "path": (
+                        args[1].json()
+                        if hasattr(args[1], "json")
+                        else (
+                            args[1].__name__
+                            if hasattr(args[1], "__name__")
+                            else str(args[1])
+                        )
+                    ),
+                    "path_map": args[2],
+                }
+            ),
+            "langgraph.task.name": "add_conditional_edges",
         }
     elif "set_entry_point" in method_name:
         return {
-            'langgraph.entrypoint': args[0],
-            'langgraph.task.name': 'set_entry_point',
+            "langgraph.entrypoint": args[0],
+            "langgraph.task.name": "set_entry_point",
         }
     elif "set_finish_point" in method_name:
         return {
-            'langgraph.finishpoint': args[0],
-            'langgraph.task.name': 'set_finish_point',
+            "langgraph.finishpoint": args[0],
+            "langgraph.task.name": "set_finish_point",
         }
     else:
         return None
-
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
 def generic_patch(method, task, tracer, version):
     """
     A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,21 @@
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.openai.patch import (
-    async_chat_completions_create, async_embeddings_create,
-    async_images_generate, chat_completions_create, embeddings_create,
-    images_generate)
+    async_chat_completions_create,
+    async_embeddings_create,
+    async_images_generate,
+    chat_completions_create,
+    embeddings_create,
+    images_generate,
+)
 
 logging.basicConfig(level=logging.FATAL)
 
 
 class OpenAIInstrumentation(BaseInstrumentor):
 
     def instrumentation_dependencies(self) -> Collection[str]:
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 
 from langtrace.trace_attributes import Event, LLMSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
-from langtrace_python_sdk.utils.llm import (calculate_prompt_tokens,
-                                            estimate_tokens)
+from langtrace_python_sdk.utils.llm import calculate_prompt_tokens, estimate_tokens
 
 
 def images_generate(original_method, version, tracer):
     """
     Wrap the `generate` method of the `Images` class to trace it.
     """
 
@@ -48,15 +49,17 @@
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["IMAGES_GENERATION"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.stream": kwargs.get("stream"),
-            "llm.prompts": json.dumps([{"role": "user", "content": kwargs.get("prompt", [])}]),
+            "llm.prompts": json.dumps(
+                [{"role": "user", "content": kwargs.get("prompt", [])}]
+            ),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(
             APIS["IMAGES_GENERATION"]["METHOD"], kind=SpanKind.CLIENT
@@ -79,15 +82,15 @@
                             "content": {
                                 "url": data.url if hasattr(data, "url") else "",
                                 "revised_prompt": (
                                     data.revised_prompt
                                     if hasattr(data, "revised_prompt")
                                     else ""
                                 ),
-                            }
+                            },
                         }
                     ]
                     span.set_attribute("llm.responses", json.dumps(response))
 
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
@@ -123,15 +126,17 @@
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["IMAGES_GENERATION"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.stream": kwargs.get("stream"),
-            "llm.prompts": json.dumps([{"role": "user", "content": kwargs.get("prompt", [])}]),
+            "llm.prompts": json.dumps(
+                [{"role": "user", "content": kwargs.get("prompt", [])}]
+            ),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(
             APIS["IMAGES_GENERATION"]["METHOD"], kind=SpanKind.CLIENT
@@ -155,15 +160,15 @@
                             "content": {
                                 "url": data.url if hasattr(data, "url") else "",
                                 "revised_prompt": (
                                     data.revised_prompt
                                     if hasattr(data, "revised_prompt")
                                     else ""
                                 ),
-                            }
+                            },
                         }
                     ]
                     span.set_attribute("llm.responses", json.dumps(response))
 
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
@@ -283,15 +288,16 @@
                                     "content_filter_results": choice[
                                         "content_filter_results"
                                     ]
                                 }
                                 if "content_filter_results" in choice
                                 else {}
                             ),
-                        } for choice in result.choices
+                        }
+                        for choice in result.choices
                     ]
                     span.set_attribute("llm.responses", json.dumps(responses))
                 else:
                     responses = []
                     span.set_attribute("llm.responses", json.dumps(responses))
                 if (
                     hasattr(result, "system_fingerprint")
@@ -371,24 +377,30 @@
                                     choice.delta.function_call.arguments
                                 )
                                 completion_tokens += token_counts
                                 content = [choice.delta.function_call.arguments]
                     elif tool_calls:
                         for choice in chunk.choices:
                             tool_call = ""
-                            if (choice.delta and choice.delta.tool_calls is not None):
+                            if choice.delta and choice.delta.tool_calls is not None:
                                 toolcalls = choice.delta.tool_calls
                                 content = []
                                 for tool_call in toolcalls:
-                                    if tool_call and tool_call.function is not None and tool_call.function.arguments is not None:
+                                    if (
+                                        tool_call
+                                        and tool_call.function is not None
+                                        and tool_call.function.arguments is not None
+                                    ):
                                         token_counts = estimate_tokens(
                                             tool_call.function.arguments
                                         )
                                         completion_tokens += token_counts
-                                        content = content + [tool_call.function.arguments]
+                                        content = content + [
+                                            tool_call.function.arguments
+                                        ]
                                     else:
                                         content = content + []
                 else:
                     content = []
                 span.add_event(
                     Event.STREAM_OUTPUT.value,
                     {
@@ -536,15 +548,16 @@
                                     "content_filter_results": choice[
                                         "content_filter_results"
                                     ]
                                 }
                                 if "content_filter_results" in choice
                                 else {}
                             ),
-                        } for choice in result.choices
+                        }
+                        for choice in result.choices
                     ]
                     span.set_attribute("llm.responses", json.dumps(responses))
                 else:
                     responses = []
                     span.set_attribute("llm.responses", json.dumps(responses))
                 if (
                     hasattr(result, "system_fingerprint")
@@ -624,24 +637,30 @@
                                     choice.delta.function_call.arguments
                                 )
                                 completion_tokens += token_counts
                                 content = [choice.delta.function_call.arguments]
                     elif tool_calls:
                         for choice in chunk.choices:
                             tool_call = ""
-                            if (choice.delta and choice.delta.tool_calls is not None):
+                            if choice.delta and choice.delta.tool_calls is not None:
                                 toolcalls = choice.delta.tool_calls
                                 content = []
                                 for tool_call in toolcalls:
-                                    if tool_call and tool_call.function is not None and tool_call.function.arguments is not None:
+                                    if (
+                                        tool_call
+                                        and tool_call.function is not None
+                                        and tool_call.function.arguments is not None
+                                    ):
                                         token_counts = estimate_tokens(
                                             tool_call.function.arguments
                                         )
                                         completion_tokens += token_counts
-                                        content = content + [tool_call.function.arguments]
+                                        content = content + [
+                                            tool_call.function.arguments
+                                        ]
                                     else:
                                         content = content + []
                 else:
                     content = []
                 span.add_event(
                     Event.STREAM_OUTPUT.value,
                     {
@@ -711,15 +730,17 @@
             "llm.model": kwargs.get("model"),
             "llm.prompts": "",
             "llm.embedding_inputs": json.dumps([kwargs.get("input", "")]),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         if kwargs.get("encoding_format") is not None:
-            span_attributes["llm.encoding.formats"] = json.dumps([kwargs.get("encoding_format")])
+            span_attributes["llm.encoding.formats"] = json.dumps(
+                [kwargs.get("encoding_format")]
+            )
 
         attributes = LLMSpanAttributes(**span_attributes)
         kwargs.get("encoding_format")
 
         if kwargs.get("dimensions") is not None:
             attributes["llm.dimensions"] = kwargs.get("dimensions")
         if kwargs.get("user") is not None:
@@ -770,15 +791,17 @@
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["EMBEDDINGS_CREATE"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
-            "llm.prompts": json.dumps([{"role": "user", "content": kwargs.get("input", "")}]),
+            "llm.prompts": json.dumps(
+                [{"role": "user", "content": kwargs.get("input", "")}]
+            ),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
         kwargs.get("encoding_format")
 
         if kwargs.get("encoding_format") is not None:
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,47 +16,53 @@
 
 from langtrace.trace_attributes import DatabaseSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
-from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
+from langtrace_python_sdk.constants.instrumentation.qdrant import APIS
 
 
-def generic_patch(original_method, method, version, tracer):
+def collection_patch(method, version, tracer):
+    """
+    A generic patch method that wraps a function with a span
     """
-    A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
         api = APIS[method]
-        service_provider = SERVICE_PROVIDERS["PINECONE"]
+        service_provider = SERVICE_PROVIDERS["QDRANT"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "db.system": "pinecone",
+            "db.system": "qdrant",
             "db.operation": api["OPERATION"],
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
+        if hasattr(instance, "name") and instance.name is not None:
+            span_attributes["db.collection.name"] = instance.name
+
         attributes = DatabaseSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(api["METHOD"], kind=SpanKind.CLIENT) as span:
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
-                result = original_method(instance, *args, **kwargs)
+                result = wrapped(*args, **kwargs)
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
                 # Record the exception in the span
                 span.record_exception(err)
 
                 # Set the span status to indicate an error
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/patch.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,51 +16,49 @@
 
 from langtrace.trace_attributes import DatabaseSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
-from langtrace_python_sdk.constants.instrumentation.qdrant import APIS
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
+from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
 
 
-def collection_patch(method, version, tracer):
-    """
-    A generic patch method that wraps a function with a span
+def generic_patch(original_method, method, version, tracer):
     """
+    A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
         api = APIS[method]
-        service_provider = SERVICE_PROVIDERS["QDRANT"]
+        service_provider = SERVICE_PROVIDERS["PINECONE"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "db.system": "qdrant",
+            "db.system": "pinecone",
             "db.operation": api["OPERATION"],
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
-        if hasattr(instance, "name") and instance.name is not None:
-            span_attributes["db.collection.name"] = instance.name
-
         attributes = DatabaseSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(api["METHOD"], kind=SpanKind.CLIENT) as span:
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
-                result = wrapped(*args, **kwargs)
+                result = original_method(instance, *args, **kwargs)
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
                 # Record the exception in the span
                 span.record_exception(err)
 
                 # Set the span status to indicate an error
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from tiktoken import get_encoding
 
-from langtrace_python_sdk.constants.instrumentation.common import \
-    TIKTOKEN_MODEL_MAPPING
-from langtrace_python_sdk.constants.instrumentation.openai import \
-    OPENAI_COST_TABLE
+from langtrace_python_sdk.constants.instrumentation.common import TIKTOKEN_MODEL_MAPPING
+from langtrace_python_sdk.constants.instrumentation.openai import OPENAI_COST_TABLE
 
 
 def estimate_tokens(prompt):
     """
     Estimate the number of tokens in a prompt."""
     if prompt and len(prompt) > 0:
         # Simplified token estimation: count the words.
```

### Comparing `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.0.5/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-
 import asyncio
 from functools import wraps
 
 from opentelemetry import baggage, context, trace
 from opentelemetry.trace import SpanKind
 
-from langtrace_python_sdk.constants.instrumentation.common import \
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY
+from langtrace_python_sdk.constants.instrumentation.common import (
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+)
 
 
 def with_langtrace_root_span(
     name="LangtraceRootSpan",
     kind=SpanKind.INTERNAL,
 ):
```

### Comparing `langtrace_python_sdk-2.0.4/src/tests/conftest.py` & `langtrace_python_sdk-2.0.5/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/utils.py` & `langtrace_python_sdk-2.0.5/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.0.5/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.0.5/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.5/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.0.5/src/tests/chroma/test_chroma.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from unittest.mock import MagicMock, patch, call
-from langtrace_python_sdk.constants.instrumentation.common import \
-    SERVICE_PROVIDERS
+from langtrace_python_sdk.constants.instrumentation.common import SERVICE_PROVIDERS
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
-from opentelemetry.trace.status import StatusCode,Status
+from opentelemetry.trace.status import StatusCode, Status
 from langtrace_python_sdk.instrumentation.chroma.patch import collection_patch
 from opentelemetry.trace import SpanKind
 from tests.utils import common_setup
 import unittest
 import json
 
 
 class TestChromaPatch(unittest.TestCase):
     data = {
         "status": "success",
     }
+
     def setUp(self):
-            self.chroma_mock, self.tracer, self.span = common_setup(self.data, 'chromadb.Collection.add')
-            self.wrapped_method = MagicMock(return_value="mocked method result")
-            self.instance = MagicMock()
-            self.instance.name = "aa" 
+        self.chroma_mock, self.tracer, self.span = common_setup(
+            self.data, "chromadb.Collection.add"
+        )
+        self.wrapped_method = MagicMock(return_value="mocked method result")
+        self.instance = MagicMock()
+        self.instance.name = "aa"
 
     def tearDown(self):
         self.chroma_mock.stop()
 
     def test_collection_patch_success(self):
         # Arrange
         traced_method = collection_patch("ADD", "1.2.3", self.tracer)
@@ -31,34 +33,38 @@
         result = traced_method(self.wrapped_method, self.instance, (), {})
 
         # Assert
         # Assert the result of the original method is returned
         self.assertEqual(result, "mocked method result")
 
         # Assert the span is started with the correct parameters
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with("chromadb.Collection.add", kind=SpanKind.CLIENT))
+        self.assertTrue(
+            self.tracer.start_as_current_span.called_once_with(
+                "chromadb.Collection.add", kind=SpanKind.CLIENT
+            )
+        )
 
         # Verify span attributes are set as expected
         expected_attributes = {
-            'langtrace.sdk.name': 'langtrace-python-sdk',
-            'langtrace.service.name': 'Chroma',
-            'langtrace.service.type': 'vectordb',
-            'langtrace.service.version': '1.2.3',
-            'langtrace.version': '1.0.0',
-            'db.system': 'chromadb',
-            'db.operation': 'add',
-            'db.collection.name': 'aa',
+            "langtrace.sdk.name": "langtrace-python-sdk",
+            "langtrace.service.name": "Chroma",
+            "langtrace.service.type": "vectordb",
+            "langtrace.service.version": "1.2.3",
+            "langtrace.version": "1.0.0",
+            "db.system": "chromadb",
+            "db.operation": "add",
+            "db.collection.name": "aa",
         }
         for key, value in expected_attributes.items():
             self.span.set_attribute.assert_has_calls([call(key, value)], any_order=True)
 
         actual_calls = self.span.set_attribute.call_args_list
 
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
-        
+
         # Assert the span status is set to OK
         self.span.set_status.assert_called_with(StatusCode.OK)
-        
 
-if __name__ == '__main__':
-    unittest.main()
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `langtrace_python_sdk-2.0.4/src/tests/cohere/conftest.py` & `langtrace_python_sdk-2.0.5/src/tests/cohere/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_chat.py` & `langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_embed.py` & `langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_rerank.py` & `langtrace_python_sdk-2.0.5/src/tests/cohere/test_cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_chat.yaml` & `langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_chat.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml` & `langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_embed.yaml` & `langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_embed.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_rerank.yaml` & `langtrace_python_sdk-2.0.5/src/tests/cohere/cassettes/test_cohere_rerank.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,82 @@
-
 import unittest
 from unittest.mock import MagicMock, call
 from langtrace_python_sdk.instrumentation.langchain.patch import generic_patch
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace import get_tracer
 import importlib.metadata
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
 from opentelemetry.trace.status import Status, StatusCode
 from tests.utils import common_setup
 import json
 
+
 class TestGenericPatch(unittest.TestCase):
     data = {"key": "value"}
+
     def setUp(self):
         self.langchain_mock, self.tracer, self.span = common_setup(self.data, None)
 
     def tearDown(self):
         # Clean up after each test case
         pass
-      
+
     def test_generic_patch(self):
         # Arrange
         method_name = "example_method"
         trace_output = False
         trace_input = False  # Change as per your requirement
         args = (1, 2, 3)
         task = "split_text"
-        kwargs = {'key': 'value'}
-        version = importlib.metadata.version('langchain')
+        kwargs = {"key": "value"}
+        version = importlib.metadata.version("langchain")
 
         # Act
-        wrapped_function = generic_patch("langchain.text_splitter", task, self.tracer, version, trace_output, trace_input)
+        wrapped_function = generic_patch(
+            "langchain.text_splitter",
+            task,
+            self.tracer,
+            version,
+            trace_output,
+            trace_input,
+        )
         result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
 
         # Assert
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with(method_name, kind=SpanKind.CLIENT))
-        
+        self.assertTrue(
+            self.tracer.start_as_current_span.called_once_with(
+                method_name, kind=SpanKind.CLIENT
+            )
+        )
+
         service_provider = "Langchain"
         expected_attributes = {
-            'langtrace.sdk.name': 'langtrace-python-sdk',
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
         }
-        
-        
+
         self.assertTrue(
             self.span.set_attribute.has_calls(
-                [call(key, value) for key, value in expected_attributes.items()], any_order=True
+                [call(key, value) for key, value in expected_attributes.items()],
+                any_order=True,
             )
         )
-                
+
         actual_calls = self.span.set_attribute.call_args_list
 
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
-        
+
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
-        expected_result_data = {"key": "value"  }   
+        expected_result_data = {"key": "value"}
 
         self.assertEqual(result.key, expected_result_data["key"])
 
-if __name__ == '__main__':
-    unittest.main()
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain_community.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,82 @@
-
 import unittest
 from unittest.mock import MagicMock, Mock, patch, call
 from langtrace_python_sdk.instrumentation.langchain_community.patch import generic_patch
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace import get_tracer
 import importlib.metadata
 import openai
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
 from opentelemetry.trace.status import Status, StatusCode
 import json
 from tests.utils import common_setup
+
+
 class TestGenericPatch(unittest.TestCase):
     data = {"key": "value"}
+
     def setUp(self):
         self.langchain_mock, self.tracer, self.span = common_setup(self.data, None)
 
     def tearDown(self):
         # Clean up after each test case
         pass
 
     def test_generic_patch(self):
         # Arrange
         method_name = "example_method"
         trace_output = False
-        trace_input = False 
+        trace_input = False
         args = (1, 2, 3)
         task = "vector_store"
-        kwargs = {'key': 'value'}
+        kwargs = {"key": "value"}
         version = importlib.metadata.version("langchain-community")
 
         # Act
-        wrapped_function = generic_patch("langchain_community.vectorstores.faiss", task, self.tracer, version, trace_output, trace_input)
+        wrapped_function = generic_patch(
+            "langchain_community.vectorstores.faiss",
+            task,
+            self.tracer,
+            version,
+            trace_output,
+            trace_input,
+        )
         result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
 
         # Assert
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with(method_name, kind=SpanKind.CLIENT))
-        
+        self.assertTrue(
+            self.tracer.start_as_current_span.called_once_with(
+                method_name, kind=SpanKind.CLIENT
+            )
+        )
+
         service_provider = "Langchain Community"
         expected_attributes = {
-            'langtrace.sdk.name': 'langtrace-python-sdk',
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
         }
-        
-        
+
         self.assertTrue(
             self.span.set_attribute.has_calls(
-                [call(key, value) for key, value in expected_attributes.items()], any_order=True
+                [call(key, value) for key, value in expected_attributes.items()],
+                any_order=True,
             )
         )
-                
+
         actual_calls = self.span.set_attribute.call_args_list
 
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
-        
+
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
-        expected_result_data = {"key": "value"  }   
+        expected_result_data = {"key": "value"}
         self.assertEqual(result.key, expected_result_data["key"])
 
 
-if __name__ == '__main__':
-    unittest.main()
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.0.5/src/tests/langchain/test_langchain_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,115 +1,141 @@
-
 import unittest
 from unittest.mock import MagicMock, Mock, patch, call
-from langtrace_python_sdk.instrumentation.langchain_core.patch import generic_patch, runnable_patch
+from langtrace_python_sdk.instrumentation.langchain_core.patch import (
+    generic_patch,
+    runnable_patch,
+)
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace import get_tracer
 import importlib.metadata
 import openai
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
 from opentelemetry.trace.status import Status, StatusCode
 import json
 from tests.utils import common_setup
+
+
 class TestGenericPatch(unittest.TestCase):
     data = {"items": "value"}
+
     def setUp(self):
         self.langchain_mock, self.tracer, self.span = common_setup(self.data, None)
 
     def tearDown(self):
         # Clean up after each test case
         pass
 
     def test_generic_patch(self):
         # Arrange
         method_name = "example_method"
         trace_output = False
-        trace_input = True 
+        trace_input = True
         task = "retriever"
         args = (1, 2, 3)
-        kwargs = {'key': 'value'}
+        kwargs = {"key": "value"}
         version = importlib.metadata.version("langchain-core")
 
         # Act
-        wrapped_function = generic_patch("langchain_core.retrievers", task , self.tracer, version, trace_output, trace_input)
+        wrapped_function = generic_patch(
+            "langchain_core.retrievers",
+            task,
+            self.tracer,
+            version,
+            trace_output,
+            trace_input,
+        )
         result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
 
         # Assert
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with(method_name, kind=SpanKind.CLIENT))
-        
+        self.assertTrue(
+            self.tracer.start_as_current_span.called_once_with(
+                method_name, kind=SpanKind.CLIENT
+            )
+        )
+
         service_provider = "Langchain Core"
         expected_attributes = {
-            'langtrace.sdk.name': 'langtrace-python-sdk',
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
         }
-        
+
         self.assertTrue(
             self.span.set_attribute.has_calls(
-                [call(key, value) for key, value in expected_attributes.items()], any_order=True
+                [call(key, value) for key, value in expected_attributes.items()],
+                any_order=True,
             )
         )
-             
+
         actual_calls = self.span.set_attribute.call_args_list
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
 
-        
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
-        expected_result_data = {"items": "value"  }   
+        expected_result_data = {"items": "value"}
         self.assertEqual(result.items, expected_result_data["items"])
 
     def test_runnable_patch(self):
         # Arrange
         method_name = "example_method"
         trace_output = False
-        trace_input = True 
+        trace_input = True
         args = (1, 2, 3)
-        kwargs = {'key': 'value'}
+        kwargs = {"key": "value"}
         version = importlib.metadata.version("langchain-core")
 
         # Act
-        wrapped_function = runnable_patch("langchain_core.runnables.passthrough",
-                "runnablepassthrough", self.tracer, version, trace_output, trace_input)
+        wrapped_function = runnable_patch(
+            "langchain_core.runnables.passthrough",
+            "runnablepassthrough",
+            self.tracer,
+            version,
+            trace_output,
+            trace_input,
+        )
 
         result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
 
         # Assert
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with(method_name, kind=SpanKind.CLIENT))
-        
+        self.assertTrue(
+            self.tracer.start_as_current_span.called_once_with(
+                method_name, kind=SpanKind.CLIENT
+            )
+        )
+
         service_provider = "Langchain Core"
         expected_attributes = {
-            'langtrace.sdk.name': 'langtrace-python-sdk',
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": "runnablepassthrough",
         }
 
         self.assertTrue(
             self.span.set_attribute.has_calls(
-                [call(key, value) for key, value in expected_attributes.items()], any_order=True
+                [call(key, value) for key, value in expected_attributes.items()],
+                any_order=True,
             )
         )
-        
+
         actual_calls = self.span.set_attribute.call_args_list
 
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
 
-       
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
-        expected_result_data = {"items": "value"  }   
+        expected_result_data = {"items": "value"}
 
         self.assertEqual(result.items, expected_result_data["items"])
 
 
-if __name__ == '__main__':
-    unittest.main()
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `langtrace_python_sdk-2.0.4/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.0.5/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.0.5/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.0.5/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.0.5/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.0.5/src/tests/pinecone/test_pinecone.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,63 +10,72 @@
 import unittest
 import json
 from tests.utils import common_setup
 
 
 class TestPinecone(unittest.TestCase):
     data = {
-    "status": "success",
-    "message": "Data upserted successfully",
-    "upserted_ids": [1, 2, 3]
+        "status": "success",
+        "message": "Data upserted successfully",
+        "upserted_ids": [1, 2, 3],
     }
-    
-    def setUp(self):
-        self.pinecone_mock, self.tracer, self.span = common_setup(self.data, 'pinecone.Index.upsert')
 
+    def setUp(self):
+        self.pinecone_mock, self.tracer, self.span = common_setup(
+            self.data, "pinecone.Index.upsert"
+        )
 
     def tearDown(self):
         self.pinecone_mock.stop()
 
     def test_pinecone(self):
-    
-       # Arrange
-        version = importlib.metadata.version('pinecone-client')
+
+        # Arrange
+        version = importlib.metadata.version("pinecone-client")
         method = "UPSERT"
         vectors = [[1, 2, 3], [4, 5, 6]]
 
         # Act
-        wrapped_function = generic_patch(pinecone.Index.upsert, method, version, self.tracer)
+        wrapped_function = generic_patch(
+            pinecone.Index.upsert, method, version, self.tracer
+        )
         result = wrapped_function(MagicMock(), MagicMock(), (vectors,), {})
 
         # Assert
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with("pinecone.data.index", kind=SpanKind.CLIENT))
+        self.assertTrue(
+            self.tracer.start_as_current_span.called_once_with(
+                "pinecone.data.index", kind=SpanKind.CLIENT
+            )
+        )
         api = APIS[method]
         service_provider = SERVICE_PROVIDERS["PINECONE"]
         expected_attributes = {
-            'langtrace.sdk.name': 'langtrace-python-sdk',
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "db.system": "pinecone",
             "db.operation": api["OPERATION"],
         }
         self.assertTrue(
             self.span.set_attribute.has_calls(
-                [call(key, value) for key, value in expected_attributes.items()], any_order=True
+                [call(key, value) for key, value in expected_attributes.items()],
+                any_order=True,
             )
-        )      
+        )
 
         actual_calls = self.span.set_attribute.call_args_list
 
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
-            
+
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
-        expected_result = ['status', 'message', 'upserted_ids']
+        expected_result = ["status", "message", "upserted_ids"]
         result_keys = json.loads(result).keys()
         self.assertSetEqual(set(expected_result), set(result_keys), "Keys mismatch")
 
-if __name__ == '__main__':
-    unittest.main()
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `langtrace_python_sdk-2.0.4/.gitignore` & `langtrace_python_sdk-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/LICENSE` & `langtrace_python_sdk-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/README.md` & `langtrace_python_sdk-2.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 ``` python
 pip install langtrace-python-sdk
 ```
 
 ``` python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 ```
 
 ## Langtrace self hosted custom exporter
 
 Get started by adding simply three lines to your code and see traces being exported to your remote location!
 
 ``` python
```

### Comparing `langtrace_python_sdk-2.0.4/pyproject.toml` & `langtrace_python_sdk-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.4/PKG-INFO` & `langtrace_python_sdk-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -145,15 +145,15 @@
 
 ``` python
 pip install langtrace-python-sdk
 ```
 
 ``` python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
-langtrace.init(write_to_langtrace_cloud=False)
+langtrace.init(write_spans_to_console=True)
 ```
 
 ## Langtrace self hosted custom exporter
 
 Get started by adding simply three lines to your code and see traces being exported to your remote location!
 
 ``` python
```

