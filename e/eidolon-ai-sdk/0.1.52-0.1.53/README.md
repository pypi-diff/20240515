# Comparing `tmp/eidolon_ai_sdk-0.1.52.tar.gz` & `tmp/eidolon_ai_sdk-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.52.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.53.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.52.tar` & `eidolon_ai_sdk-0.1.53.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0      701 2024-05-09 05:17:31.847805 eidolon_ai_sdk-0.1.52/README.md
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.847805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2429 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0     1311 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/audio_agent.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3025 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2710 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2817 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1434 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2329 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2864 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3717 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    13079 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1815 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4572 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12735 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     8381 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     9079 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     1823 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
--rw-r--r--   0        0        0     6440 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      601 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      614 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      597 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      595 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      586 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4638 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2562 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     9083 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     3718 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14325 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     4680 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0     9936 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11967 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     4518 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5753 2024-05-09 05:17:31.851805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9490 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3567 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3962 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     2421 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4477 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3793 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      974 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2159 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    23002 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14196 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4911 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3808 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6917 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      898 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/logging.conf
--rw-r--r--   0        0        0     2197 2024-05-09 05:17:31.855805 eidolon_ai_sdk-0.1.52/pyproject.toml
--rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.52/PKG-INFO
+-rw-r--r--   0        0        0      701 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0     1311 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/audio_agent.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3025 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2710 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-05-15 03:13:42.094929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1428 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2323 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2864 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3717 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    13073 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1809 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9545 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     8381 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     9073 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     1823 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
+-rw-r--r--   0        0        0     6440 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      601 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      614 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      597 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      595 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      586 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     3003 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     9083 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     5954 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/apu.py
+-rw-r--r--   0        0        0     3718 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14319 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     4680 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5753 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9490 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3567 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3962 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     2421 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4477 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      974 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-05-15 03:13:42.098929 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    23002 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14196 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4911 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6917 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/logging.conf
+-rw-r--r--   0        0        0     2214 2024-05-15 03:13:42.102928 eidolon_ai_sdk-0.1.53/pyproject.toml
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.53/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.52/README.md` & `eidolon_ai_sdk-0.1.53/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing
 from pydantic import BaseModel
 from typing import List, TypeVar, Generic
 
-from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.apu import APU
 from eidolon_ai_sdk.cpu.agents_logic_unit import (
     AgentsLogicUnit,
     AgentsLogicUnitSpec,
 )
 from eidolon_ai_sdk.system.fn_handler import FnHandler, register_handler
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/audio_agent.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/audio_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 from jinja2 import Environment, StrictUndefined
 from pydantic import Field
 from typing import List
 
 from eidolon_ai_sdk.agent.retriever_agent.question_transformer import QuestionTransformerSpec, QuestionTransformer
-from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.apu import APU
 from eidolon_ai_sdk.cpu.agent_io import UserTextAPUMessage
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 
 
 class HydeQuestionTransformerSpec(QuestionTransformerSpec):
     cpu: AnnotatedReference[APU]
     prompt: str = Field(
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 from jinja2 import Environment, StrictUndefined
 from pydantic import Field, BaseModel
 from typing import List
 
 from eidolon_ai_sdk.agent.retriever_agent.question_transformer import QuestionTransformerSpec, QuestionTransformer
-from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.apu import APU
 from eidolon_ai_sdk.cpu.agent_io import UserTextAPUMessage
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 
 
 class MultiQuestionTransformerSpec(QuestionTransformerSpec):
     cpu: AnnotatedReference[APU]
     keep_original: bool = Field(default=True, description="Whether to keep the original question in the output")
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pydantic_core import to_jsonable_python
 
 from eidolon_ai_client.events import AgentStateEvent, StreamEvent, StringOutputEvent, UserInputEvent, FileHandle
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_client.util.request_context import RequestContext
 from eidolon_ai_sdk.agent.agent import register_action
 from eidolon_ai_sdk.agent.doc_manager.document_processor import DocumentProcessor
-from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.apu import APU
 from eidolon_ai_sdk.cpu.agent_io import SystemAPUMessage, UserTextAPUMessage, AttachedFileMessage
 from eidolon_ai_sdk.cpu.agents_logic_unit import AgentsLogicUnitSpec, AgentsLogicUnit
 from eidolon_ai_sdk.system.processes import ProcessDoc
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 from eidolon_ai_sdk.util.schema_to_model import schema_to_model
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from jinja2 import StrictUndefined, Environment
 from pydantic import Field, BaseModel
 
-from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.apu import APU
 from eidolon_ai_sdk.cpu.agent_io import UserTextAPUMessage
 from eidolon_ai_sdk.agent.tot_agent.prompts import CHECKER_PROMPT
 from eidolon_ai_sdk.agent.tot_agent.thought import ThoughtValidity
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
 class TotCheckerConfig(BaseModel):
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 import yaml
 from click import Choice, BadParameter
 from pydantic import BaseModel
 from pydantic_core import PydanticUndefinedType
 from rich import print as richprint
 from rich.syntax import Syntax
 
+from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.system.reference_model import Reference
-from eidolon_ai_sdk.system.resources import agent_resources, AgentResource
+from eidolon_ai_sdk.system.resources.agent_resource import AgentResource
 from eidolon_ai_sdk.util.class_utils import for_name, fqn
 
 echo = lambda text, **kwargs: typer.echo(pad(text), **kwargs)  # noqa
 confirm = lambda text, **kwargs: typer.confirm(pad(text), **kwargs)  # noqa
 
 
 def prompt(text, default=None, choices: list[str] = None, case_sensitive=False, **kwargs):
@@ -85,14 +86,15 @@
         else:
             classes = (n for n, v in inspect.getmembers(sys.modules[package_name], inspect.isclass))
             options = [package_name + "." + c for c in classes if c.startswith(substring)]
     return options[state] if state < len(options) else None
 
 
 def create_agent():
+    agent_resources = AgentOS.get_resources(AgentResource)
     agents = [a for a in agent_resources.keys() if a != "Agent"] + ["Custom"]
 
     name = prompt("What is the name of the agent?", default="NewAgent")
     kind = prompt(f"What type of agent is {name}?", default="GenericAgent", choices=agents)
     args = dict(apiVersion="eidolon/v1")
     args["kind"] = kind if kind != "Custom" else "Agent"
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from eidolon_ai_sdk.agent.simple_agent import SimpleAgent
 from eidolon_ai_sdk.agent.tot_agent.checker import ToTChecker
 from eidolon_ai_sdk.agent.tot_agent.thought_generators import ThoughtGenerationStrategy, ProposePromptStrategy
 from eidolon_ai_sdk.agent.tot_agent.tot_agent import TreeOfThoughtsAgent
 from eidolon_ai_sdk.builtins.components.opentelemetry import OpenTelemetryManager, CustomSampler, NoopSpanExporter
 from eidolon_ai_sdk.builtins.components.usage import UsageMiddleware
 from eidolon_ai_sdk.builtins.logic_units.web_search import WebSearch, Browser, Search
-from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.apu import APU
 from eidolon_ai_sdk.cpu.agent_io import IOUnit
 from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.cpu.conversation_memory_unit import RawMemoryUnit
 from eidolon_ai_sdk.cpu.conversational_apu import ConversationalAPU
 from eidolon_ai_sdk.agent_os_interfaces import FileMemory, SymbolicMemory, SimilarityMemory, SecurityManager
 from eidolon_ai_sdk.cpu.llm.anthropic_llm_unit import AnthropicLLMUnit
 from eidolon_ai_sdk.cpu.llm.mistral_llm_unit import MistralGPT
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/mistral_large.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/mistral_small.yaml` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/apu.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import json
 from abc import abstractmethod, ABC
-from pydantic import BaseModel, Field, TypeAdapter
 from typing import Any, List, Dict, Literal, Union, TypeVar, Type, cast, AsyncIterator
 
+from pydantic import BaseModel, Field, TypeAdapter
+
+from eidolon_ai_client.events import StreamEvent, convert_output_object, ObjectOutputEvent, ErrorEvent, StringOutputEvent
 from eidolon_ai_sdk.cpu.agent_io import CPUMessageTypes
 from eidolon_ai_sdk.cpu.call_context import CallContext
-from eidolon_ai_client.events import StreamEvent, convert_output_object, ObjectOutputEvent, ErrorEvent, StringOutputEvent
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
 class APUCapabilities(BaseModel):
     input_context_limit: int
     output_context_limit: int
     supports_tools: bool
@@ -26,35 +27,56 @@
     max_num_function_calls: int = Field(
         10,
         description="The maximum number of function calls to make in a single request.",
     )
 
 
 class APU(Specable[APUSpec], ABC):
+    """
+    The APU is the main interface for the Agent to interact with the LLM.
+    The APU provides a set of capabilities that encapsulate LLM functionality and creates a clear separation between business logic and the underlying LLM implementation.
+    """
     title: str
 
     def __init__(self, spec: T, **kwargs: object):
         super().__init__(spec, **kwargs)
         self.title = "default"
 
     @abstractmethod
     def get_capabilities(self) -> APUCapabilities:
+        """
+        Returns the capabilities of the APU including the context limits, whether it supports tools, image input, audio input, file search, image generation, and audio generation.
+        """
         pass
 
     @abstractmethod
     async def set_boot_messages(self, call_context: CallContext, boot_messages: List[CPUMessageTypes]):
+        """
+        Sets the boot messages for the APU storing them in the call context using the registered memory unit.
+
+        :param call_context: The current call context including process id and thread id.
+        :param boot_messages: The boot message
+        """
         pass
 
     @abstractmethod
     async def schedule_request(
-        self,
-        call_context: CallContext,
-        prompts: List[CPUMessageTypes],
-        output_format: Union[Literal["str"], Dict[str, Any]],
+            self,
+            call_context: CallContext,
+            prompts: List[CPUMessageTypes],
+            output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[StreamEvent]:
+        """
+        Schedules the given prompts with the APU. The default implementation saves the new prompts into memory, executes the prompts, including intermediate tool calls, and returns the output in the specified format.
+
+        :param call_context: The current call context including process id and thread id.
+        :param prompts: The new prompts to schedule.
+        :param output_format: The output format to return the response in.
+        :return: Yields a stream of events including the output response.
+        """
         yield None
 
     def _to_json(self, obj):
         if obj is None:
             return ""
         elif isinstance(obj, BaseModel):
             return obj.model_dump_json()
@@ -82,30 +104,30 @@
     _cpu: APU
 
     def __init__(self, call_context: CallContext, cpu: APU):
         self._call_context = call_context
         self._cpu = cpu
 
     async def set_boot_messages(
-        self,
-        prompts: List[CPUMessageTypes],
+            self,
+            prompts: List[CPUMessageTypes],
     ):
         return await self._cpu.set_boot_messages(self._call_context, list(prompts))
 
     async def run_request(
-        self,
-        prompts: List[CPUMessageTypes],
-        output_format: Union[Literal["str"], Dict[str, Any], Type[T]] = "str",
+            self,
+            prompts: List[CPUMessageTypes],
+            output_format: Union[Literal["str"], Dict[str, Any], Type[T]] = "str",
     ) -> T:
         stream = self.stream_request(prompts, output_format)
         result = None
         error = None
 
         is_string_call = not isinstance(output_format, type) and (
-            output_format == "str" or output_format["type"] == "string"
+                output_format == "str" or output_format["type"] == "string"
         )
         string_output = ""
         async for event in stream:
             if event.is_root_and_type(ObjectOutputEvent):
                 result = event.content
             elif event.is_root_and_type(StringOutputEvent):
                 string_output += event.content
@@ -120,15 +142,15 @@
                 raise error
             else:
                 raise Exception(error)
 
         return result
 
     def stream_request(
-        self, prompts: List[CPUMessageTypes], output_format: Union[Literal["str"], Dict[str, Any], Type[T]] = "str"
+            self, prompts: List[CPUMessageTypes], output_format: Union[Literal["str"], Dict[str, Any], Type[T]] = "str"
     ) -> AsyncIterator[StreamEvent]:
         if isinstance(output_format, type):
             model = TypeAdapter(output_format)
             schema = model.json_schema()
             s = convert_output_object(
                 self._cpu.schedule_request(self._call_context, prompts, schema), cast(Type[T], output_format)
             )
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_client.util.stream_collector import merge_streams
 from eidolon_ai_sdk.agent.doc_manager.document_processor import DocumentProcessor
 from eidolon_ai_sdk.agent.doc_manager.loaders.base_loader import FileInfo
 from eidolon_ai_sdk.agent.doc_manager.parsers.base_parser import DataBlob
 from eidolon_ai_sdk.agent_os import AgentOS
-from eidolon_ai_sdk.cpu.agent_cpu import APU, APUSpec, Thread, APUException, APUCapabilities
+from eidolon_ai_sdk.cpu.apu import APU, APUSpec, Thread, APUException, APUCapabilities
 from eidolon_ai_sdk.cpu.agent_io import IOUnit, CPUMessageTypes
 from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.image_unit import ImageUnit
 from eidolon_ai_sdk.cpu.llm_message import (
     AssistantMessage,
     ToolResponseMessage,
```

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/agent_machine.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/process_file_system.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.53/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/logging.conf` & `eidolon_ai_sdk-0.1.53/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.52/pyproject.toml` & `eidolon_ai_sdk-0.1.53/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.52"
+version = "0.1.53"
 description = "An open source sgent service SDK"
 authors = [ "Luke Lalor <lukehlalor@gmail.com>",]
 readme = "README.md"
 include = [ "logging.conf",]
 
 [tool.ruff]
 line-length = 121
 
 [tool.eidolon]
 update-tag = "sdk"
-last-update-hash = "873244c738f72497e575912bc5e4c5823e37720f"
+last-update-hash = "d8a126252e6bb70019540a51e86d844e83ad6f37"
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
 Website = "https://www.eidolonai.com/"
 
 [tool.poetry.scripts]
 eidolon-server = "eidolon_ai_sdk.bin.agent_http_server:main"
@@ -80,14 +80,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pylint = "^3.0.3"
 ruff = "^0.1.7"
 pytest-recording = "^0.13.1"
 pytest-asyncio = "^0.23.4"
+pdoc = "^14.4.0"
 
 [tool.poetry.group.dev.dependencies.eidolon-ai-client]
 path = "../client/python"
 develop = true
 
 [tool.poetry.group.dev.dependencies.eidolon-ai-usage-client]
 path = "../usage-service/usage-client"
```

### Comparing `eidolon_ai_sdk-0.1.52/PKG-INFO` & `eidolon_ai_sdk-0.1.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.52
+Version: 0.1.53
 Summary: An open source sgent service SDK
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
```

