# Comparing `tmp/agentuniverse-0.0.5.tar.gz` & `tmp/agentuniverse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentuniverse-0.0.5.tar", last modified: Wed May  8 15:59:53 2024, max compression
+gzip compressed data, was "agentuniverse-0.0.6.tar", max compression
```

## Comparing `agentuniverse-0.0.5.tar` & `agentuniverse-0.0.6.tar`

### file list

```diff
@@ -1,242 +1,184 @@
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.719728 agentuniverse-0.0.5/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2560 2024-05-08 14:09:08.000000 agentuniverse-0.0.5/CHANGELOG.md
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2183 2024-05-08 14:07:58.000000 agentuniverse-0.0.5/CHANGELOG_zh.md
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/LICENSE
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      304 2024-05-08 15:07:57.000000 agentuniverse-0.0.5/MANIFEST.in
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2633 2024-05-08 15:59:53.719138 agentuniverse-0.0.5/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3210 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/README.md
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2908 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/README_zh.md
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.718674 agentuniverse-0.0.5/agentUniverse.egg-info/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2633 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9373 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/SOURCES.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/dependency_links.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      324 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/requires.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       62 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/top_level.txt
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.662506 agentuniverse-0.0.5/agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentuniverse-0.0.5/agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.663708 agentuniverse-0.0.5/agentuniverse/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.663886 agentuniverse-0.0.5/agentuniverse/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.664363 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.664835 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      972 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4270 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/knowledge.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/knowledge_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.665150 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.666084 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1651 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1478 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/reader.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.666861 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5872 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/chroma_store.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2206 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/document.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/query.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3842 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/store.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.667475 agentuniverse-0.0.5/agentuniverse/agent/action/tool/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/tool/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/tool/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3868 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/action/tool/tool.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/tool/tool_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5469 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-26 03:44:12.000000 agentuniverse-0.0.5/agentuniverse/agent/agent_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/agent_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.667631 agentuniverse-0.0.5/agentuniverse/agent/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/default/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.668760 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1257 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1446 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3126 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/executing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      367 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/executing_agent.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.669575 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1499 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1866 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2030 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/expressing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      365 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/expressing_agent.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.670039 agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1289 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/peer_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      374 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/peer_agent.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.670805 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1343 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1623 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/planning_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      353 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/planning_agent.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.671564 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      769 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      884 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1333 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/rag_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/rag_agent.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.672317 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1222 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1412 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1954 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      359 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/reviewing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/input_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.674184 agentuniverse-0.0.5/agentuniverse/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3907 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/chat_memory.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.674696 agentuniverse-0.0.5/agentuniverse/agent/memory/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      174 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      845 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/default/default_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      321 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/default/default_memory.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7689 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3054 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/memory_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/message.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      754 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/summarizer_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/output_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.674862 agentuniverse-0.0.5/agentuniverse/agent/plan/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.675352 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.675837 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3670 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.676319 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3599 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.676832 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     8919 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6438 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planner_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.677311 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3599 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.677797 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3397 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.678271 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3603 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.679047 agentuniverse-0.0.5/agentuniverse/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/service_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/service_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.680191 agentuniverse-0.0.5/agentuniverse/agent_serve/web/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.680603 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.681033 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/entity/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/entity/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/entity/request_do.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5473 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/request_library.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5327 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/flask_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2351 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/gunicorn_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9311 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/request_task.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.681342 agentuniverse-0.0.5/agentuniverse/agent_serve/web/rpc/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/rpc/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1224 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/rpc/rpc_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/thread_with_result.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      822 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/web_booster.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2679 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/web_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.681647 agentuniverse-0.0.5/agentuniverse/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    11112 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/base/agentuniverse.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.681966 agentuniverse-0.0.5/agentuniverse/base/annotation/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/annotation/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/annotation/singleton.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.682919 agentuniverse-0.0.5/agentuniverse/base/component/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/component/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/component/application_component_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/component/component_base.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4380 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/component/component_configer_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/component/component_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/component/component_manager_base.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.683382 agentuniverse-0.0.5/agentuniverse/base/config/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.683926 agentuniverse-0.0.5/agentuniverse/base/config/application_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/application_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4173 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/config/application_configer/app_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/application_configer/application_config_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.684501 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2811 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/component_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.685816 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/agent_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/llm_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/memory_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/planner_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1889 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/prompt_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/tool_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/config_type_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4846 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/base/config/configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.686127 agentuniverse-0.0.5/agentuniverse/base/config/custom_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/custom_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-26 03:55:12.000000 agentuniverse-0.0.5/agentuniverse/base/config/custom_configer/custom_key_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.686580 agentuniverse-0.0.5/agentuniverse/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/context/framework_context.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/context/framework_context_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.687953 agentuniverse-0.0.5/agentuniverse/base/prompt/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      174 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      286 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/combine_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      318 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/combine_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      253 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/summary_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      272 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/summary_en_prompt.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.694604 agentuniverse-0.0.5/agentuniverse/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/env_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.700024 agentuniverse-0.0.5/agentuniverse/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-26 03:42:29.000000 agentuniverse-0.0.5/agentuniverse/base/util/logging/general_logger.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/logging/logging_config.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-26 03:42:21.000000 agentuniverse-0.0.5/agentuniverse/base/util/logging/logging_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-26 03:42:41.000000 agentuniverse-0.0.5/agentuniverse/base/util/memory_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6776 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/base/util/prompt_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/system_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.705713 agentuniverse-0.0.5/agentuniverse/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/llm/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.706733 agentuniverse-0.0.5/agentuniverse/llm/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/llm/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1352 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/llm/default/default_openai_llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/llm/default/default_openai_llm.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5625 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/llm/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5601 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/llm/llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/llm/llm_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      408 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/llm/llm_output.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     8063 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/llm/openai_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.713913 agentuniverse-0.0.5/agentuniverse/prompt/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/prompt/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      548 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/prompt/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2891 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/prompt/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      741 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/prompt/prompt_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1127 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/prompt/prompt_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.714276 agentuniverse-0.0.5/agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentuniverse-0.0.5/agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.717872 agentuniverse-0.0.5/agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentuniverse-0.0.5/agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.718360 agentuniverse-0.0.5/agentuniverse_extension/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse_extension/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse_extension/logger/sls_sink.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2162 2024-05-08 13:45:55.000000 agentuniverse-0.0.5/pyproject.toml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      323 2024-05-08 15:15:20.000000 agentuniverse-0.0.5/requirements.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-05-08 15:59:53.719851 agentuniverse-0.0.5/setup.cfg
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1230 2024-05-08 15:57:57.000000 agentuniverse-0.0.5/setup.py
+-rw-r--r--   0        0        0    11335 2024-04-02 12:08:01.834225 agentuniverse-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1527 2024-04-19 04:40:08.243214 agentuniverse-0.0.6/README_PYPI.md
+-rw-r--r--   0        0        0      164 2024-04-02 03:12:13.474920 agentuniverse-0.0.6/agentuniverse/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.835519 agentuniverse-0.0.6/agentuniverse/agent/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835723 agentuniverse-0.0.6/agentuniverse/agent/action/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835932 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.836127 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0        0        0      972 2024-04-26 07:36:14.016798 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/embedding.py
+-rw-r--r--   0        0        0     4270 2024-05-07 11:44:48.809512 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
+-rw-r--r--   0        0        0     3097 2024-04-26 03:46:54.112257 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/knowledge.py
+-rw-r--r--   0        0        0      655 2024-04-26 03:46:54.140111 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/knowledge_manager.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837041 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837386 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/__init__.py
+-rw-r--r--   0        0        0     1160 2024-04-26 03:46:54.147189 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
+-rw-r--r--   0        0        0     1651 2024-04-26 07:36:14.018108 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
+-rw-r--r--   0        0        0     1568 2024-04-26 03:46:54.126577 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
+-rw-r--r--   0        0        0     1460 2024-04-26 03:46:54.173810 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
+-rw-r--r--   0        0        0     1478 2024-04-26 07:36:14.018626 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
+-rw-r--r--   0        0        0      552 2024-04-26 03:46:54.132260 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/reader.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.838782 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/__init__.py
+-rw-r--r--   0        0        0     5872 2024-05-07 11:44:48.809653 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/chroma_store.py
+-rw-r--r--   0        0        0     2206 2024-05-07 11:44:48.809765 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/document.py
+-rw-r--r--   0        0        0      662 2024-04-02 12:08:01.839355 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/query.py
+-rw-r--r--   0        0        0     3842 2024-05-07 11:44:48.809881 agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/store.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.839707 agentuniverse-0.0.6/agentuniverse/agent/action/tool/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-02 12:08:01.839872 agentuniverse-0.0.6/agentuniverse/agent/action/tool/enum.py
+-rw-r--r--   0        0        0     3868 2024-04-26 07:36:14.019652 agentuniverse-0.0.6/agentuniverse/agent/action/tool/tool.py
+-rw-r--r--   0        0        0      626 2024-04-26 03:46:54.149120 agentuniverse-0.0.6/agentuniverse/agent/action/tool/tool_manager.py
+-rw-r--r--   0        0        0     5469 2024-05-09 06:23:55.005965 agentuniverse-0.0.6/agentuniverse/agent/agent.py
+-rw-r--r--   0        0        0      639 2024-04-26 03:44:12.686183 agentuniverse-0.0.6/agentuniverse/agent/agent_manager.py
+-rw-r--r--   0        0        0      526 2024-04-02 12:08:01.840672 agentuniverse-0.0.6/agentuniverse/agent/agent_model.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.840834 agentuniverse-0.0.6/agentuniverse/agent/default/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.006641 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/__init__.py
+-rw-r--r--   0        0        0     1257 2024-05-09 06:23:55.006784 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1446 2024-05-09 06:23:55.006896 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     3126 2024-05-09 06:23:55.006988 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/executing_agent.py
+-rw-r--r--   0        0        0      367 2024-05-09 06:23:55.007062 agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/executing_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.007720 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/__init__.py
+-rw-r--r--   0        0        0     1499 2024-05-09 06:23:55.007805 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1866 2024-05-09 06:23:55.007888 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     2030 2024-05-09 06:23:55.007964 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/expressing_agent.py
+-rw-r--r--   0        0        0      365 2024-05-09 06:23:55.008036 agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/expressing_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008209 agentuniverse-0.0.6/agentuniverse/agent/default/peer_agent/__init__.py
+-rw-r--r--   0        0        0     1289 2024-05-09 06:23:55.008282 agentuniverse-0.0.6/agentuniverse/agent/default/peer_agent/peer_agent.py
+-rw-r--r--   0        0        0      374 2024-05-09 06:23:55.008415 agentuniverse-0.0.6/agentuniverse/agent/default/peer_agent/peer_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008732 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-09 06:23:55.008817 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1613 2024-05-09 06:23:55.008890 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     1623 2024-05-09 06:23:55.008965 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/planning_agent.py
+-rw-r--r--   0        0        0      353 2024-05-09 06:23:55.009031 agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/planning_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009190 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-09 06:23:55.009270 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0      884 2024-05-09 06:23:55.009355 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     1333 2024-05-09 06:23:55.009442 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/rag_agent.py
+-rw-r--r--   0        0        0      276 2024-05-09 06:23:55.009511 agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/rag_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009871 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/__init__.py
+-rw-r--r--   0        0        0     1222 2024-05-09 06:23:55.009950 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1412 2024-05-09 06:23:55.010031 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     1954 2024-05-09 06:23:55.010184 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py
+-rw-r--r--   0        0        0      359 2024-05-09 06:23:55.010255 agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/reviewing_agent.yaml
+-rw-r--r--   0        0        0      657 2024-04-02 12:08:01.841347 agentuniverse-0.0.6/agentuniverse/agent/input_object.py
+-rw-r--r--   0        0        0      173 2024-04-09 07:08:39.103227 agentuniverse-0.0.6/agentuniverse/agent/memory/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-26 09:03:49.031293 agentuniverse-0.0.6/agentuniverse/agent/memory/chat_memory.py
+-rw-r--r--   0        0        0      174 2024-04-26 09:03:49.031587 agentuniverse-0.0.6/agentuniverse/agent/memory/default/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-26 09:03:49.032072 agentuniverse-0.0.6/agentuniverse/agent/memory/default/default_memory.py
+-rw-r--r--   0        0        0      321 2024-04-26 09:03:49.032468 agentuniverse-0.0.6/agentuniverse/agent/memory/default/default_memory.yaml
+-rw-r--r--   0        0        0      402 2024-04-01 06:19:56.174000 agentuniverse-0.0.6/agentuniverse/agent/memory/enum.py
+-rw-r--r--   0        0        0     7689 2024-04-26 09:03:49.032798 agentuniverse-0.0.6/agentuniverse/agent/memory/langchain_instance.py
+-rw-r--r--   0        0        0     3054 2024-04-26 07:36:14.022682 agentuniverse-0.0.6/agentuniverse/agent/memory/memory.py
+-rw-r--r--   0        0        0      635 2024-04-26 03:46:54.130633 agentuniverse-0.0.6/agentuniverse/agent/memory/memory_manager.py
+-rw-r--r--   0        0        0      508 2024-04-09 16:15:17.142565 agentuniverse-0.0.6/agentuniverse/agent/memory/message.py
+-rw-r--r--   0        0        0      754 2024-04-26 09:03:49.033037 agentuniverse-0.0.6/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
+-rw-r--r--   0        0        0      896 2024-04-26 09:03:49.033338 agentuniverse-0.0.6/agentuniverse/agent/memory/summarizer_en_prompt.yaml
+-rw-r--r--   0        0        0      572 2024-04-02 12:08:01.842690 agentuniverse-0.0.6/agentuniverse/agent/output_object.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842823 agentuniverse-0.0.6/agentuniverse/agent/plan/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842962 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.142958 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/executing_planner/__init__.py
+-rw-r--r--   0        0        0     3670 2024-05-09 06:23:55.010687 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
+-rw-r--r--   0        0        0      195 2024-04-26 03:46:54.158656 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.144134 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
+-rw-r--r--   0        0        0     3599 2024-05-09 06:23:55.010948 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
+-rw-r--r--   0        0        0      200 2024-04-26 03:46:54.188023 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
+-rw-r--r--   0        0        0      158 2024-04-09 16:15:17.145177 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/peer_planner/__init__.py
+-rw-r--r--   0        0        0     8919 2024-05-09 06:23:55.011260 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
+-rw-r--r--   0        0        0      170 2024-04-26 03:46:54.113707 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
+-rw-r--r--   0        0        0     6438 2024-05-09 06:23:55.011722 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planner.py
+-rw-r--r--   0        0        0      659 2024-04-26 03:46:54.185023 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planner_manager.py
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.145969 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planning_planner/__init__.py
+-rw-r--r--   0        0        0     3599 2024-05-09 06:23:55.012182 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
+-rw-r--r--   0        0        0      190 2024-04-26 03:46:54.166967 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-02 12:08:01.843408 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/rag_planner/__init__.py
+-rw-r--r--   0        0        0     3397 2024-05-09 06:23:55.012606 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
+-rw-r--r--   0        0        0      165 2024-04-26 03:46:54.135943 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.147020 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
+-rw-r--r--   0        0        0     3603 2024-05-09 06:23:55.012846 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
+-rw-r--r--   0        0        0      195 2024-04-26 03:46:54.178755 agentuniverse-0.0.6/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
+-rw-r--r--   0        0        0        0 2024-04-02 12:08:01.843939 agentuniverse-0.0.6/agentuniverse/agent_serve/__init__.py
+-rw-r--r--   0        0        0     1944 2024-04-02 12:08:01.844114 agentuniverse-0.0.6/agentuniverse/agent_serve/service.py
+-rw-r--r--   0        0        0     3152 2024-04-26 03:46:54.144088 agentuniverse-0.0.6/agentuniverse/agent_serve/service_configer.py
+-rw-r--r--   0        0        0     1161 2024-04-02 12:08:01.844424 agentuniverse-0.0.6/agentuniverse/agent_serve/service_instance.py
+-rw-r--r--   0        0        0      402 2024-04-02 12:08:01.844558 agentuniverse-0.0.6/agentuniverse/agent_serve/service_manager.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844690 agentuniverse-0.0.6/agentuniverse/agent_serve/web/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844823 agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.845006 agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/entity/__init__.py
+-rw-r--r--   0        0        0     1075 2024-04-02 12:08:01.845143 agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/entity/request_do.py
+-rw-r--r--   0        0        0     5473 2024-04-26 15:29:30.264684 agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/request_library.py
+-rw-r--r--   0        0        0     5019 2024-05-15 03:58:25.722266 agentuniverse-0.0.6/agentuniverse/agent_serve/web/flask_server.py
+-rw-r--r--   0        0        0     2351 2024-04-26 15:29:30.265783 agentuniverse-0.0.6/agentuniverse/agent_serve/web/gunicorn_server.py
+-rw-r--r--   0        0        0     9311 2024-04-26 09:03:49.038432 agentuniverse-0.0.6/agentuniverse/agent_serve/web/request_task.py
+-rw-r--r--   0        0        0      164 2024-04-26 09:03:49.038779 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-15 03:58:25.722567 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-15 03:58:25.722726 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto
+-rw-r--r--   0        0        0     2092 2024-05-15 03:58:25.722866 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py
+-rw-r--r--   0        0        0     5979 2024-05-15 03:58:25.723032 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5033 2024-05-15 03:58:25.723168 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py
+-rw-r--r--   0        0        0     3307 2024-05-15 03:58:25.723368 agentuniverse-0.0.6/agentuniverse/agent_serve/web/rpc/rpc_server.py
+-rw-r--r--   0        0        0     1146 2024-04-02 12:08:01.845635 agentuniverse-0.0.6/agentuniverse/agent_serve/web/thread_with_result.py
+-rw-r--r--   0        0        0      822 2024-04-26 15:29:30.266263 agentuniverse-0.0.6/agentuniverse/agent_serve/web/web_booster.py
+-rw-r--r--   0        0        0     2679 2024-04-26 15:29:30.266639 agentuniverse-0.0.6/agentuniverse/agent_serve/web/web_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846346 agentuniverse-0.0.6/agentuniverse/base/__init__.py
+-rw-r--r--   0        0        0    11557 2024-05-15 03:58:25.723582 agentuniverse-0.0.6/agentuniverse/base/agentuniverse.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846609 agentuniverse-0.0.6/agentuniverse/base/annotation/__init__.py
+-rw-r--r--   0        0        0      515 2024-04-02 12:08:01.846840 agentuniverse-0.0.6/agentuniverse/base/annotation/singleton.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.847286 agentuniverse-0.0.6/agentuniverse/base/component/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-26 03:46:54.108902 agentuniverse-0.0.6/agentuniverse/base/component/application_component_manager.py
+-rw-r--r--   0        0        0     1264 2024-04-26 03:46:54.107724 agentuniverse-0.0.6/agentuniverse/base/component/component_base.py
+-rw-r--r--   0        0        0     4380 2024-04-26 09:03:49.040235 agentuniverse-0.0.6/agentuniverse/base/component/component_configer_util.py
+-rw-r--r--   0        0        0      626 2024-04-26 09:03:49.040545 agentuniverse-0.0.6/agentuniverse/base/component/component_enum.py
+-rw-r--r--   0        0        0     2576 2024-04-26 03:46:54.137220 agentuniverse-0.0.6/agentuniverse/base/component/component_manager_base.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.848825 agentuniverse-0.0.6/agentuniverse/base/config/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.849235 agentuniverse-0.0.6/agentuniverse/base/config/application_configer/__init__.py
+-rw-r--r--   0        0        0     4173 2024-04-26 09:03:49.040952 agentuniverse-0.0.6/agentuniverse/base/config/application_configer/app_configer.py
+-rw-r--r--   0        0        0     1006 2024-04-26 03:46:54.105041 agentuniverse-0.0.6/agentuniverse/base/config/application_configer/application_config_manager.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850062 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/__init__.py
+-rw-r--r--   0        0        0     2811 2024-04-26 09:03:49.041321 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/component_configer.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850500 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/__init__.py
+-rw-r--r--   0        0        0     2599 2024-04-26 03:46:54.162861 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/agent_configer.py
+-rw-r--r--   0        0        0     2053 2024-04-26 03:46:54.189422 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
+-rw-r--r--   0        0        0     3272 2024-04-26 03:46:54.100009 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/llm_configer.py
+-rw-r--r--   0        0        0     2540 2024-04-26 03:46:54.198928 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/memory_configer.py
+-rw-r--r--   0        0        0     2392 2024-04-26 03:46:54.181023 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/planner_configer.py
+-rw-r--r--   0        0        0     1889 2024-04-26 09:03:49.041670 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/prompt_configer.py
+-rw-r--r--   0        0        0     2192 2024-04-26 03:46:54.165777 agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/tool_configer.py
+-rw-r--r--   0        0        0      423 2024-04-02 12:08:01.852070 agentuniverse-0.0.6/agentuniverse/base/config/config_type_enum.py
+-rw-r--r--   0        0        0     4846 2024-04-26 15:29:30.267459 agentuniverse-0.0.6/agentuniverse/base/config/configer.py
+-rw-r--r--   0        0        0      163 2024-04-02 12:08:01.852534 agentuniverse-0.0.6/agentuniverse/base/config/custom_configer/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-26 03:55:12.618569 agentuniverse-0.0.6/agentuniverse/base/config/custom_configer/custom_key_configer.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.852949 agentuniverse-0.0.6/agentuniverse/base/context/__init__.py
+-rw-r--r--   0        0        0     1447 2024-04-26 03:46:54.182246 agentuniverse-0.0.6/agentuniverse/base/context/framework_context.py
+-rw-r--r--   0        0        0     2768 2024-04-26 03:46:54.110018 agentuniverse-0.0.6/agentuniverse/base/context/framework_context_manager.py
+-rw-r--r--   0        0        0      174 2024-04-26 09:03:49.042097 agentuniverse-0.0.6/agentuniverse/base/prompt/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-26 09:03:49.042363 agentuniverse-0.0.6/agentuniverse/base/prompt/combine_cn_prompt.yaml
+-rw-r--r--   0        0        0      318 2024-04-26 09:03:49.042631 agentuniverse-0.0.6/agentuniverse/base/prompt/combine_en_prompt.yaml
+-rw-r--r--   0        0        0      253 2024-04-26 09:03:49.042893 agentuniverse-0.0.6/agentuniverse/base/prompt/summary_cn_prompt.yaml
+-rw-r--r--   0        0        0      272 2024-04-26 09:03:49.043156 agentuniverse-0.0.6/agentuniverse/base/prompt/summary_en_prompt.yaml
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.853924 agentuniverse-0.0.6/agentuniverse/base/util/__init__.py
+-rw-r--r--   0        0        0      307 2024-04-02 12:08:01.854131 agentuniverse-0.0.6/agentuniverse/base/util/env_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.854373 agentuniverse-0.0.6/agentuniverse/base/util/logging/__init__.py
+-rw-r--r--   0        0        0     6600 2024-04-26 03:42:29.579851 agentuniverse-0.0.6/agentuniverse/base/util/logging/general_logger.py
+-rw-r--r--   0        0        0     5132 2024-04-02 12:08:01.854819 agentuniverse-0.0.6/agentuniverse/base/util/logging/logging_config.py
+-rw-r--r--   0        0        0     6395 2024-04-26 03:42:21.826133 agentuniverse-0.0.6/agentuniverse/base/util/logging/logging_util.py
+-rw-r--r--   0        0        0      502 2024-04-26 03:42:41.042298 agentuniverse-0.0.6/agentuniverse/base/util/memory_util.py
+-rw-r--r--   0        0        0     6776 2024-05-09 06:23:55.013451 agentuniverse-0.0.6/agentuniverse/base/util/prompt_util.py
+-rw-r--r--   0        0        0      715 2024-04-02 12:08:01.855496 agentuniverse-0.0.6/agentuniverse/base/util/system_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.855704 agentuniverse-0.0.6/agentuniverse/llm/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.855856 agentuniverse-0.0.6/agentuniverse/llm/default/__init__.py
+-rw-r--r--   0        0        0     1352 2024-04-26 09:03:49.043837 agentuniverse-0.0.6/agentuniverse/llm/default/default_openai_llm.py
+-rw-r--r--   0        0        0      223 2024-04-26 09:03:49.044133 agentuniverse-0.0.6/agentuniverse/llm/default/default_openai_llm.yaml
+-rw-r--r--   0        0        0     5625 2024-05-09 06:23:55.013593 agentuniverse-0.0.6/agentuniverse/llm/langchain_instance.py
+-rw-r--r--   0        0        0     5601 2024-05-15 03:58:25.723788 agentuniverse-0.0.6/agentuniverse/llm/llm.py
+-rw-r--r--   0        0        0      619 2024-04-26 03:46:54.138842 agentuniverse-0.0.6/agentuniverse/llm/llm_manager.py
+-rw-r--r--   0        0        0      408 2024-04-26 09:03:49.045322 agentuniverse-0.0.6/agentuniverse/llm/llm_output.py
+-rw-r--r--   0        0        0     8294 2024-05-15 03:58:25.723994 agentuniverse-0.0.6/agentuniverse/llm/openai_llm.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.856945 agentuniverse-0.0.6/agentuniverse/prompt/__init__.py
+-rw-r--r--   0        0        0      548 2024-04-26 07:36:14.033265 agentuniverse-0.0.6/agentuniverse/prompt/enum.py
+-rw-r--r--   0        0        0     2891 2024-05-09 06:23:55.015272 agentuniverse-0.0.6/agentuniverse/prompt/prompt.py
+-rw-r--r--   0        0        0      741 2024-04-26 09:03:49.046141 agentuniverse-0.0.6/agentuniverse/prompt/prompt_manager.py
+-rw-r--r--   0        0        0     1120 2024-05-15 03:58:25.724188 agentuniverse-0.0.6/agentuniverse/prompt/prompt_model.py
+-rw-r--r--   0        0        0      164 2024-04-02 03:12:13.477398 agentuniverse-0.0.6/agentuniverse_connector/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 03:13:12.638584 agentuniverse-0.0.6/agentuniverse_extension/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.857428 agentuniverse-0.0.6/agentuniverse_extension/logger/__init__.py
+-rw-r--r--   0        0        0     7321 2024-04-02 12:08:01.857588 agentuniverse-0.0.6/agentuniverse_extension/logger/sls_sink.py
+-rw-r--r--   0        0        0     2581 2024-05-15 05:26:47.421174 agentuniverse-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 agentuniverse-0.0.6/PKG-INFO
```

### Comparing `agentuniverse-0.0.5/LICENSE` & `agentuniverse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/PKG-INFO` & `agentuniverse-0.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.5
+Version: 0.0.6
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
-Home-page: https://gitee.com/agentUniverse/agentUniverse
+Home-page: https://github.com/alipay/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
-Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: log-ext
+Requires-Dist: SQLAlchemy (==2.0.25)
+Requires-Dist: aliyun-log-python-sdk (==0.8.8) ; extra == "log-ext"
+Requires-Dist: cffi (>=1.15.1,<2.0.0)
+Requires-Dist: chromadb (==0.4.24)
+Requires-Dist: flask (==2.2)
+Requires-Dist: flask_cors (==4.0.0)
+Requires-Dist: googleapis-common-protos (>=1.63.0,<2.0.0)
+Requires-Dist: grpcio (==1.63.0)
+Requires-Dist: gunicorn (==21.2.0)
+Requires-Dist: langchain (==0.0.352)
+Requires-Dist: langchain-core (==0.1.3)
+Requires-Dist: loguru (==0.7.2)
+Requires-Dist: myst-parser (>=2.0.0,<3.0.0)
+Requires-Dist: openai (==1.13.3)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sphinx (>=7.2.6,<8.0.0)
+Requires-Dist: sphinx-rtd-theme (>=2.0.0,<3.0.0)
+Requires-Dist: tiktoken (==0.5.2)
+Requires-Dist: werkzeug (==2.2.2)
+Project-URL: Repository, https://github.com/alipay/agentUniverse
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: cffi>=1.15.1
-Requires-Dist: flask>=2.2
-Requires-Dist: werkzeug>=2.2.2
-Requires-Dist: langchain>=0.0.352
-Requires-Dist: langchain-core>=0.1.3
-Requires-Dist: openai>=1.13.3
-Requires-Dist: tiktoken>=0.5.2
-Requires-Dist: loguru>=0.7.2
-Requires-Dist: flask_cors>=4.0.0
-Requires-Dist: SQLAlchemy>=2.0.25
-Requires-Dist: pydantic>=2.6.4
-Requires-Dist: gunicorn>=21.2.0
-Requires-Dist: chromadb>=0.4.24
-Requires-Dist: aliyun-log-python-sdk>=0.8.8
-Requires-Dist: googleapis-common-protos>=1.63.0
-Requires-Dist: myst-parser>=2.0.0
-Requires-Dist: pdfminer.six
 
 # agentUniverse
 
 ## Overview
 agentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
 
 The framework will come with serveral pre-install multi-agent collaboration patterns which have been proven effective in real business scenarios, and will continue to be enriched in the future. Patterns that are currently about to be released include:
```

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/embedding.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/knowledge.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/knowledge_manager.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/knowledge_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/file_reader.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/file_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/reader.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/reader/reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/chroma_store.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/chroma_store.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/document.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/document.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/query.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/query.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/store.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/knowledge/store/store.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/tool/tool.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/tool/tool.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/action/tool/tool_manager.py` & `agentuniverse-0.0.6/agentuniverse/agent/action/tool/tool_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/agent.py` & `agentuniverse-0.0.6/agentuniverse/agent/agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/agent_manager.py` & `agentuniverse-0.0.6/agentuniverse/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/agent_model.py` & `agentuniverse-0.0.6/agentuniverse/agent/agent_model.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/executing_agent.py` & `agentuniverse-0.0.6/agentuniverse/agent/default/executing_agent/executing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/expressing_agent.py` & `agentuniverse-0.0.6/agentuniverse/agent/default/expressing_agent/expressing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/peer_agent.py` & `agentuniverse-0.0.6/agentuniverse/agent/default/peer_agent/peer_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/planning_agent.py` & `agentuniverse-0.0.6/agentuniverse/agent/default/planning_agent/planning_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/rag_agent.py` & `agentuniverse-0.0.6/agentuniverse/agent/default/rag_agent/rag_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py` & `agentuniverse-0.0.6/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/input_object.py` & `agentuniverse-0.0.6/agentuniverse/agent/input_object.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/memory/chat_memory.py` & `agentuniverse-0.0.6/agentuniverse/agent/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/memory/default/default_memory.py` & `agentuniverse-0.0.6/agentuniverse/agent/memory/default/default_memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/memory/langchain_instance.py` & `agentuniverse-0.0.6/agentuniverse/agent/memory/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/memory/memory.py` & `agentuniverse-0.0.6/agentuniverse/agent/memory/memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/memory/memory_manager.py` & `agentuniverse-0.0.6/agentuniverse/agent/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/memory/summarizer_cn_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/memory/summarizer_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/memory/summarizer_en_prompt.yaml` & `agentuniverse-0.0.6/agentuniverse/agent/memory/summarizer_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/output_object.py` & `agentuniverse-0.0.6/agentuniverse/agent/output_object.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py` & `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py` & `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py` & `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planner.py` & `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planner_manager.py` & `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planner_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py` & `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py` & `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py` & `agentuniverse-0.0.6/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/service.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/service.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/service_configer.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/service_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/service_instance.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/service_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/entity/request_do.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/entity/request_do.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/request_library.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/web/dal/request_library.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/web/flask_server.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/web/flask_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,41 +26,39 @@
 
 @app.route("/service_run", methods=['POST'])
 @request_param
 def service_run(service_id: str, params: dict, saved: bool = False):
     """Synchronous invocation of an agent service.
 
     Request Args:
-        service_id(`str`): The id of the agent service. Format like
-            {appname}.service.{service_name}.
+        service_id(`str`): The id of the agent service.
         params(`dict`): Json style params passed to service.
         saved(`bool`): Save the request and result into database.
 
     Return:
         Returns a dict containing two keys: success and result.
         success: This key holds a boolean value indicating the task was
-        successfully or not.
+            successfully or not.
         result: This key points to a nested dictionary that includes the
-        result of the task.
+            result of the task.
     """
     params = {} if params is None else params
     request_task = RequestTask(ServiceInstance(service_id).run, saved, **params)
     result = request_task.run()
     return make_standard_response(success=True, result=result,
                                   request_id=request_task.request_id)
 
 
 @app.route("/service_run_stream", methods=['POST'])
 @request_param
 def service_run_stream(service_id: str, params: dict, saved: bool = False):
     """Synchronous invocation of an agent service, return in stream form.
 
     Request Args:
-        service_id(`str`): The id of the agent service. Format like
-            {appname}.service.{service_name}.
+        service_id(`str`): The id of the agent service.
         params(`dict`): Json style params passed to service.
         saved(`bool`): Save the request and result into database.
 
     Return:
         A SSE(Server-Sent Event) stream.
     """
     params = {} if params is None else params
@@ -74,30 +72,24 @@
 @app.route("/service_run_async", methods=['POST'])
 @request_param
 def service_run_async(service_id: str, params: dict, saved: bool = True):
     """Async invocation of an agent service, return the request id used to
     get result later.
 
     Request Args:
-        service_id(`str`): The id of the agent service. Format like
-            {appname}.service.{service_name}.
+        service_id(`str`): The id of the agent service.
         params(`dict`): Json style params passed to service.
         saved(`bool`): Save the request and result into database.
 
     Return:
         Returns a dict containing two keys: success and result.
         success: This key holds a boolean value indicating the task was
-        successfully or not.
-        result: This key points to a dictionary contains a key: request_id,
-        its value can be used in service_run_result api to get the result
-        of async task.
-
-    Example Response:
-        {"success": True, "data": {
-        "request_id":"05d0a28785cc455894ebb88bba14a67e"}}.
+            successfully or not.
+        request_id: Stand for a single request taski, can be used in
+            service_run_result api to get the result of async task.
     """
     params = {} if params is None else params
     params['service_id'] = service_id
     task = RequestTask(service_run_queue, saved, **params)
     task.async_run()
     return make_standard_response(success=True,
                                   request_id=task.request_id)
@@ -111,17 +103,17 @@
     Request Args:
         request_id(`str`): Request id returned by async run api.
 
     Return:
         Returns a dict containing two keys: success and result if request_id
         exists in database.
         success: This key holds a boolean value indicating the task was
-        successfully or not.
+            successfully or not.
         result: This key points to a nested dictionary that includes the
-        result of the task.
+            result of the task.
     """
     data = RequestTask.query_request_state(request_id)
     if data is None:
         return make_standard_response(
             success=False,
             message=f"request {request_id} not found"
         )
```

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/web/gunicorn_server.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/web/gunicorn_server.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/web/request_task.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/web/request_task.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/web/thread_with_result.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/web/thread_with_result.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/web/web_booster.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/web/web_booster.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/agent_serve/web/web_util.py` & `agentuniverse-0.0.6/agentuniverse/agent_serve/web/web_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/agentuniverse.py` & `agentuniverse-0.0.6/agentuniverse/base/agentuniverse.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # @Time    : 2024/4/2 15:27
 # @Author  : jerry.zzw 
 # @Email   : jerry.zzw@antgroup.com
 # @FileName: agentuniverse.py
 import importlib
 import sys
+import threading
 from pathlib import Path
 
 from agentuniverse.base.annotation.singleton import singleton
 from agentuniverse.base.component.application_component_manager import ApplicationComponentManager
 from agentuniverse.base.component.component_base import ComponentBase
 from agentuniverse.base.config.application_configer.app_configer import AppConfiger
 from agentuniverse.base.config.application_configer.application_config_manager import ApplicationConfigManager
@@ -19,14 +20,15 @@
 from agentuniverse.base.config.config_type_enum import ConfigTypeEnum
 from agentuniverse.base.config.configer import Configer
 from agentuniverse.base.config.custom_configer.custom_key_configer import CustomKeyConfiger
 from agentuniverse.base.component.component_enum import ComponentEnum
 from agentuniverse.base.util.system_util import get_project_root_path
 from agentuniverse.base.util.logging.logging_util import init_loggers
 from agentuniverse.agent_serve.web.request_task import RequestLibrary
+from agentuniverse.agent_serve.web.rpc.grpc.grpc_server_booster import start_grpc_server
 
 
 @singleton
 class AgentUniverse(object):
     """AgentUniverse framework object, responsible for the framework initialization,
        system variables management, etc."""
 
@@ -67,14 +69,23 @@
             configer.value.get('SUB_CONFIG_PATH', {}).get('log_config_path'),
             config_path)
         init_loggers(log_config_path)
 
         # init web request task database
         RequestLibrary(configer=configer)
 
+        # init grpc server
+        grpc_activate = configer.value.get('GRPC', {}).get('activate')
+        if grpc_activate and grpc_activate.lower() == 'true':
+            grpc_thread = threading.Thread(
+                target=start_grpc_server,
+                kwargs={"configer": configer}
+            )
+            grpc_thread.start()
+
         # init gunicorn web server on mac or unix platform
         if not sys.platform.lower().startswith("win"):
             gunicorn_config_path = self.__parse_sub_config_path(
                 configer.value.get('SUB_CONFIG_PATH', {})
                 .get('gunicorn_config_path'), config_path
             )
             from ..agent_serve.web.gunicorn_server import \
```

### Comparing `agentuniverse-0.0.5/agentuniverse/base/annotation/singleton.py` & `agentuniverse-0.0.6/agentuniverse/base/annotation/singleton.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/component/application_component_manager.py` & `agentuniverse-0.0.6/agentuniverse/base/component/application_component_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/component/component_base.py` & `agentuniverse-0.0.6/agentuniverse/base/component/component_base.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/component/component_configer_util.py` & `agentuniverse-0.0.6/agentuniverse/base/component/component_configer_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/component/component_enum.py` & `agentuniverse-0.0.6/agentuniverse/base/component/component_enum.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/component/component_manager_base.py` & `agentuniverse-0.0.6/agentuniverse/base/component/component_manager_base.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/application_configer/app_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/application_configer/app_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/application_configer/application_config_manager.py` & `agentuniverse-0.0.6/agentuniverse/base/config/application_configer/application_config_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/component_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/component_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/agent_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/agent_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/knowledge_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/knowledge_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/llm_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/llm_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/memory_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/memory_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/planner_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/planner_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/prompt_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/prompt_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/tool_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/component_configer/configers/tool_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/config/custom_configer/custom_key_configer.py` & `agentuniverse-0.0.6/agentuniverse/base/config/custom_configer/custom_key_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/context/framework_context.py` & `agentuniverse-0.0.6/agentuniverse/base/context/framework_context.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/context/framework_context_manager.py` & `agentuniverse-0.0.6/agentuniverse/base/context/framework_context_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/util/logging/general_logger.py` & `agentuniverse-0.0.6/agentuniverse/base/util/logging/general_logger.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/util/logging/logging_config.py` & `agentuniverse-0.0.6/agentuniverse/base/util/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/util/logging/logging_util.py` & `agentuniverse-0.0.6/agentuniverse/base/util/logging/logging_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/util/prompt_util.py` & `agentuniverse-0.0.6/agentuniverse/base/util/prompt_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/base/util/system_util.py` & `agentuniverse-0.0.6/agentuniverse/base/util/system_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/llm/default/default_openai_llm.py` & `agentuniverse-0.0.6/agentuniverse/llm/default/default_openai_llm.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/llm/langchain_instance.py` & `agentuniverse-0.0.6/agentuniverse/llm/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/llm/llm.py` & `agentuniverse-0.0.6/agentuniverse/llm/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     client: Any = None
     async_client: Any = None
     name: Optional[str] = None
     description: Optional[str] = None
     model_name: Optional[str] = None
     temperature: Optional[float] = 0.5
     request_timeout: Optional[int] = None
-    max_tokens: Optional[int] = None
+    max_tokens: Optional[int] = 1024
     max_retries: Optional[int] = 2
     streaming: Optional[bool] = False
     ext_info: Optional[dict] = None
 
     def __init__(self, **kwargs):
         """Initialize the llm."""
         super().__init__(component_type=ComponentEnum.LLM, **kwargs)
```

### Comparing `agentuniverse-0.0.5/agentuniverse/llm/llm_manager.py` & `agentuniverse-0.0.6/agentuniverse/llm/llm_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/llm/openai_llm.py` & `agentuniverse-0.0.6/agentuniverse/llm/openai_llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     "gpt-4-0314": 8192,
     "gpt-4": 8192,
     "gpt-4-32k": 32768,
     "gpt-4-32k-0613": 32768,
     "gpt-4-0613": 8192,
     "gpt-4-1106-preview": 128000,
     "gpt-4-turbo": 128000,
+    "gpt-4o": 128000,
+    "gpt-4o-2024-05-13": 128000,
 }
 
 
 class OpenAILLM(LLM):
     """The openai llm class.
 
     Attributes:
@@ -88,48 +90,50 @@
 
         Args:
             messages (list): The messages to send to the LLM.
             **kwargs: Arbitrary keyword arguments.
         """
         streaming = kwargs.pop("streaming") if "streaming" in kwargs else self.streaming
         self.client = self._new_client()
-        chat_completion = self.client.chat.completions.create(
-            messages=messages,
-            model=kwargs.pop('model', self.model_name),
-            temperature=kwargs.pop('temperature', self.temperature),
-            stream=kwargs.pop('stream', streaming),
-            max_tokens=kwargs.pop('max_tokens', self.max_tokens),
-            **kwargs,
-        )
-        if not streaming:
-            text = chat_completion.choices[0].message.content
-            return LLMOutput(text=text, raw=chat_completion.model_dump())
-        return self.generate_stream_result(chat_completion)
+        with self.client as client:
+            chat_completion = client.chat.completions.create(
+                messages=messages,
+                model=kwargs.pop('model', self.model_name),
+                temperature=kwargs.pop('temperature', self.temperature),
+                stream=kwargs.pop('stream', streaming),
+                max_tokens=kwargs.pop('max_tokens', self.max_tokens),
+                **kwargs,
+            )
+            if not streaming:
+                text = chat_completion.choices[0].message.content
+                return LLMOutput(text=text, raw=chat_completion.model_dump())
+            return self.generate_stream_result(chat_completion)
 
     async def acall(self, messages: list, **kwargs: Any) -> Union[LLMOutput, AsyncIterator[LLMOutput]]:
         """Asynchronously run the OpenAI LLM.
 
         Args:
             messages (list): The messages to send to the LLM.
             **kwargs: Arbitrary keyword arguments.
         """
         streaming = kwargs.pop("streaming") if "streaming" in kwargs else self.streaming
         self.async_client = self._new_async_client()
-        chat_completion = await self.async_client.chat.completions.create(
-            messages=messages,
-            model=kwargs.pop('model', self.model_name),
-            temperature=kwargs.pop('temperature', self.temperature),
-            stream=kwargs.pop('stream', streaming),
-            max_tokens=kwargs.pop('max_tokens', self.max_tokens),
-            **kwargs,
-        )
-        if not streaming:
-            text = chat_completion.choices[0].message.content
-            return LLMOutput(text=text, raw=chat_completion.model_dump())
-        return self.agenerate_stream_result(chat_completion)
+        async with self.async_client as async_client:
+            chat_completion = await async_client.chat.completions.create(
+                messages=messages,
+                model=kwargs.pop('model', self.model_name),
+                temperature=kwargs.pop('temperature', self.temperature),
+                stream=kwargs.pop('stream', streaming),
+                max_tokens=kwargs.pop('max_tokens', self.max_tokens),
+                **kwargs,
+            )
+            if not streaming:
+                text = chat_completion.choices[0].message.content
+                return LLMOutput(text=text, raw=chat_completion.model_dump())
+            return self.agenerate_stream_result(chat_completion)
 
     def as_langchain(self) -> BaseLanguageModel:
         """Convert the AgentUniverse(AU) openai llm class to the langchain openai llm class."""
         return LangchainOpenAI(self)
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the OpenAILLM model in the agent configuration."""
```

### Comparing `agentuniverse-0.0.5/agentuniverse/prompt/enum.py` & `agentuniverse-0.0.6/agentuniverse/prompt/enum.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/prompt/prompt.py` & `agentuniverse-0.0.6/agentuniverse/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/prompt/prompt_manager.py` & `agentuniverse-0.0.6/agentuniverse/prompt/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/agentuniverse/prompt/prompt_model.py` & `agentuniverse-0.0.6/agentuniverse/prompt/prompt_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
     def __bool__(self):
         """ Check whether the object is empty.
 
         Return True if one of the introduction, target and instruction attribute is not empty.
         Return False otherwise.
         """
-        return bool(self.introduction or self.introduction or self.introduction)
+        return bool(self.introduction or self.target or self.instruction)
```

### Comparing `agentuniverse-0.0.5/agentuniverse_extension/logger/sls_sink.py` & `agentuniverse-0.0.6/agentuniverse_extension/logger/sls_sink.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.5/pyproject.toml` & `agentuniverse-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 [tool.poetry]
 name = "agentUniverse"
-version = "0.0.5"
+version = "0.0.6"
 description = "agentUniverse is a framework for developing applications powered by multi-agent base on large language model."
-authors = ["AntGroup <AntGroup>"]
-readme = "README.md"
+
+authors = ["AntGroup <jerry.zzw@antgroup.com>"]
+repository = "https://github.com/alipay/agentUniverse"
+readme = "README_PYPI.md"
+
+packages = [
+    { include = "agentuniverse" },
+    { include = "agentuniverse_connector" },
+    { include = "agentuniverse_extension" },
+]
+include = ["*.yaml"]
+classifiers = [
+    "Programming Language :: Python :: 3.10",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 cffi = "^1.15.1"
 flask = "2.2"
 werkzeug = "2.2.2"
@@ -16,14 +30,15 @@
 openai = '1.13.3'
 tiktoken = '0.5.2'
 loguru = '0.7.2'
 flask_cors = '4.0.0'
 SQLAlchemy = '2.0.25'
 pydantic = "^2.6.4"
 gunicorn = "21.2.0"
+grpcio = "1.63.0"
 chromadb = "0.4.24"
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 aliyun-log-python-sdk = { version = "0.8.8", optional = true}
 googleapis-common-protos = "^1.63.0"
 myst-parser = "^2.0.0"
```

