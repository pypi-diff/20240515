# Comparing `tmp/docugami_langchain-0.0.9rc6.tar.gz` & `tmp/docugami_langchain-0.0.9rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugami_langchain-0.0.9rc6.tar", max compression
+gzip compressed data, was "docugami_langchain-0.0.9rc7.tar", max compression
```

## Comparing `docugami_langchain-0.0.9rc6.tar` & `docugami_langchain-0.0.9rc7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1072 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/LICENSE
--rw-r--r--   0        0        0      361 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/README.md
--rw-r--r--   0        0        0      747 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/__init__.py
--rw-r--r--   0        0        0      487 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/agents/__init__.py
--rw-r--r--   0        0        0     8818 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/agents/base.py
--rw-r--r--   0        0        0     1805 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/agents/models.py
--rw-r--r--   0        0        0    11237 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/agents/re_act_agent.py
--rw-r--r--   0        0        0     9152 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/agents/tool_router_agent.py
--rw-r--r--   0        0        0    16628 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/base_runnable.py
--rw-r--r--   0        0        0     1506 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/__init__.py
--rw-r--r--   0        0        0     2210 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/answer_chain.py
--rw-r--r--   0        0        0     1415 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/base.py
--rw-r--r--   0        0        0      243 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/chunks/__init__.py
--rw-r--r--   0        0        0     3390 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
--rw-r--r--   0        0        0     3980 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/chunks/summarize_chunk_chain.py
--rw-r--r--   0        0        0      291 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/documents/__init__.py
--rw-r--r--   0        0        0     3838 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/documents/describe_document_set_chain.py
--rw-r--r--   0        0        0     3983 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/documents/summarize_document_chain.py
--rw-r--r--   0        0        0      647 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/__init__.py
--rw-r--r--   0        0        0     3398 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
--rw-r--r--   0        0        0      262 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/models.py
--rw-r--r--   0        0        0     3999 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/sql_fixup_chain.py
--rw-r--r--   0        0        0     4360 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/sql_query_explainer_chain.py
--rw-r--r--   0        0        0     8808 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/sql_result_chain.py
--rw-r--r--   0        0        0     3522 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/sql_result_explainer_chain.py
--rw-r--r--   0        0        0      722 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/__init__.py
--rw-r--r--   0        0        0      124 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/models.py
--rw-r--r--   0        0        0     4409 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/simple_rag_chain.py
--rw-r--r--   0        0        0     4006 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/standalone_question_chain.py
--rw-r--r--   0        0        0     4592 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/suggested_questions_chain.py
--rw-r--r--   0        0        0     4193 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/suggested_report_chain.py
--rw-r--r--   0        0        0     3600 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/tool_final_answer_chain.py
--rw-r--r--   0        0        0     4091 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/tool_output_grader_chain.py
--rw-r--r--   0        0        0      567 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/__init__.py
--rw-r--r--   0        0        0      999 2024-05-14 17:52:50.527223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/common.py
--rw-r--r--   0        0        0     3147 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/data_type_detection_chain.py
--rw-r--r--   0        0        0     3243 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/date_add_chain.py
--rw-r--r--   0        0        0     3102 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/date_parse_chain.py
--rw-r--r--   0        0        0     2464 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/timespan_parse_chain.py
--rw-r--r--   0        0        0     1604 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/config.py
--rw-r--r--   0        0        0      109 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0    13516 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0     2798 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/history.py
--rw-r--r--   0        0        0      797 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     4206 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/custom_react_json_single_input.py
--rw-r--r--   0        0        0     2091 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1075 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/key_finding.py
--rw-r--r--   0        0        0     1242 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/line_separated_list.py
--rw-r--r--   0        0        0     2816 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/sql_finding.py
--rw-r--r--   0        0        0      735 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/text_cleaning.py
--rw-r--r--   0        0        0     4502 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/timespan.py
--rw-r--r--   0        0        0      847 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/params.py
--rw-r--r--   0        0        0      122 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/py.typed
--rw-r--r--   0        0        0      165 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/retrievers/__init__.py
--rw-r--r--   0        0        0     7894 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/retrievers/fused_summary.py
--rw-r--r--   0        0        0     5890 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/retrievers/mappings.py
--rw-r--r--   0        0        0      194 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/tools/__init__.py
--rw-r--r--   0        0        0     3958 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/tools/common.py
--rw-r--r--   0        0        0     8697 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/tools/reports.py
--rw-r--r--   0        0        0     6830 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/tools/retrieval.py
--rw-r--r--   0        0        0      708 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/utils/documents.py
--rw-r--r--   0        0        0     8975 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/utils/sql.py
--rw-r--r--   0        0        0     3389 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/docugami_langchain/utils/string_cleanup.py
--rw-r--r--   0        0        0     2823 2024-05-14 17:52:50.531223 docugami_langchain-0.0.9rc6/pyproject.toml
--rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/LICENSE
+-rw-r--r--   0        0        0      361 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/README.md
+-rw-r--r--   0        0        0      747 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/agents/__init__.py
+-rw-r--r--   0        0        0     8818 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/agents/base.py
+-rw-r--r--   0        0        0     1805 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/agents/models.py
+-rw-r--r--   0        0        0    11237 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/agents/re_act_agent.py
+-rw-r--r--   0        0        0     9152 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/agents/tool_router_agent.py
+-rw-r--r--   0        0        0    16628 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/base_runnable.py
+-rw-r--r--   0        0        0     1506 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/__init__.py
+-rw-r--r--   0        0        0     2210 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/answer_chain.py
+-rw-r--r--   0        0        0     1415 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/base.py
+-rw-r--r--   0        0        0      243 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/chunks/__init__.py
+-rw-r--r--   0        0        0     3390 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
+-rw-r--r--   0        0        0     3980 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/chunks/summarize_chunk_chain.py
+-rw-r--r--   0        0        0      291 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/documents/__init__.py
+-rw-r--r--   0        0        0     3838 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/documents/describe_document_set_chain.py
+-rw-r--r--   0        0        0     3983 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/documents/summarize_document_chain.py
+-rw-r--r--   0        0        0      647 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/__init__.py
+-rw-r--r--   0        0        0     3398 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
+-rw-r--r--   0        0        0      262 2024-05-15 00:29:28.686305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/models.py
+-rw-r--r--   0        0        0     4112 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/sql_fixup_chain.py
+-rw-r--r--   0        0        0     4360 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/sql_query_explainer_chain.py
+-rw-r--r--   0        0        0     9004 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/sql_result_chain.py
+-rw-r--r--   0        0        0     3522 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/sql_result_explainer_chain.py
+-rw-r--r--   0        0        0      722 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/models.py
+-rw-r--r--   0        0        0     4409 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/simple_rag_chain.py
+-rw-r--r--   0        0        0     4006 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/standalone_question_chain.py
+-rw-r--r--   0        0        0     4592 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/suggested_questions_chain.py
+-rw-r--r--   0        0        0     4193 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/suggested_report_chain.py
+-rw-r--r--   0        0        0     3600 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/tool_final_answer_chain.py
+-rw-r--r--   0        0        0     4091 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/tool_output_grader_chain.py
+-rw-r--r--   0        0        0      567 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/common.py
+-rw-r--r--   0        0        0     3147 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/data_type_detection_chain.py
+-rw-r--r--   0        0        0     3243 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/date_add_chain.py
+-rw-r--r--   0        0        0     3102 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/date_parse_chain.py
+-rw-r--r--   0        0        0     2464 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/timespan_parse_chain.py
+-rw-r--r--   0        0        0     1604 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/config.py
+-rw-r--r--   0        0        0      109 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13516 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0     2798 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/history.py
+-rw-r--r--   0        0        0      797 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     4206 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/custom_react_json_single_input.py
+-rw-r--r--   0        0        0     2091 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1075 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/key_finding.py
+-rw-r--r--   0        0        0     1242 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/line_separated_list.py
+-rw-r--r--   0        0        0     2816 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/sql_finding.py
+-rw-r--r--   0        0        0      735 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/text_cleaning.py
+-rw-r--r--   0        0        0     4502 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/timespan.py
+-rw-r--r--   0        0        0      847 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/params.py
+-rw-r--r--   0        0        0      122 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/py.typed
+-rw-r--r--   0        0        0      165 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0     7894 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/retrievers/fused_summary.py
+-rw-r--r--   0        0        0     5890 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/retrievers/mappings.py
+-rw-r--r--   0        0        0      194 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/tools/__init__.py
+-rw-r--r--   0        0        0     3958 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/tools/common.py
+-rw-r--r--   0        0        0     8697 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/tools/reports.py
+-rw-r--r--   0        0        0     6830 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/tools/retrieval.py
+-rw-r--r--   0        0        0      708 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/utils/documents.py
+-rw-r--r--   0        0        0     8975 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/utils/sql.py
+-rw-r--r--   0        0        0     3389 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/docugami_langchain/utils/string_cleanup.py
+-rw-r--r--   0        0        0     2823 2024-05-15 00:29:28.690305 docugami_langchain-0.0.9rc7/pyproject.toml
+-rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc7/PKG-INFO
```

### Comparing `docugami_langchain-0.0.9rc6/LICENSE` & `docugami_langchain-0.0.9rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/__init__.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/agents/base.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/agents/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/agents/models.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/agents/models.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/agents/re_act_agent.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/agents/re_act_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/agents/tool_router_agent.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/agents/tool_router_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/base_runnable.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/base_runnable.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/__init__.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/answer_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/base.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/chunks/elaborate_chunk_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/chunks/elaborate_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/chunks/summarize_chunk_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/chunks/summarize_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/documents/describe_document_set_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/documents/describe_document_set_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/documents/summarize_document_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/documents/summarize_document_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/__init__.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/sql_fixup_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/sql_fixup_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import AsyncIterator, Optional
 
 from langchain_core.runnables import RunnableConfig
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
 from docugami_langchain.output_parsers.sql_finding import SQLFindingOutputParser
+from docugami_langchain.output_parsers.text_cleaning import TextCleaningOutputParser
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
 
 
 class SQLFixupChain(BaseDocugamiChain[str]):
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
@@ -41,15 +42,15 @@
                 "- Quote all column names and strings appropriately per SQLite syntax",
                 "- Make sure all column names in SELECT statements actually exist in the table (update column names if you find a near match)",
                 "- Don't select more than 10 columns to avoid making the query so long that it gets truncated",
                 "",
                 "If you see any of the above mistakes, or any other mistakes, rewrite the query to fix them. If there are no mistakes, just reproduce the original query.",
             ],
             stop_sequences=["\n", ";", "<|eot_id|>"],
-            additional_runnables=[SQLFindingOutputParser()],
+            additional_runnables=[TextCleaningOutputParser(), SQLFindingOutputParser()],
         )
 
     def run(  # type: ignore[override]
         self,
         table_info: str,
         sql_query: str,
         exception: str = "",
```

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/sql_query_explainer_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/sql_query_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/sql_result_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/sql_result_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from sqlglot import ParseError
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
 from docugami_langchain.chains.querying.models import ExplainedSQLResult
 from docugami_langchain.chains.querying.sql_fixup_chain import SQLFixupChain
 from docugami_langchain.output_parsers.sql_finding import SQLFindingOutputParser
+from docugami_langchain.output_parsers.text_cleaning import TextCleaningOutputParser
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
 from docugami_langchain.utils.sql import (
     check_and_format_query,
     create_example_selector,
     get_table_info_as_create_table,
 )
 
@@ -54,15 +55,17 @@
             question = inputs.get("question")
             return get_table_info_as_create_table(
                 self.db,
                 question=question,
                 example_selector=self._example_row_selector,
             )
 
-        def run_sql_query(inputs: dict, config: Optional[RunnableConfig]) -> ExplainedSQLResult:
+        def run_sql_query(
+            inputs: dict, config: Optional[RunnableConfig]
+        ) -> ExplainedSQLResult:
             """
             Runs the given SQL query against the database connection for this chain, and returns the result.
             """
 
             question = inputs.get("question")
             sql_query = inputs.get("sql_query")
             table_info = table_info_func({"question": question})
@@ -149,14 +152,15 @@
                 "- Pay attention to use the date('now') function to get the current date, if the question involves \"today\".",
                 """- When matching strings in WHERE clauses, always use LIKE with LOWER rather than exact string match with "=" since users may not fully specify complete input with the right """
                 + """casing, for example generate SELECT * from "athletes" WHERE LOWER("last name") LIKE '%jones%' instead of SELECT * from "athletes" WHERE "last name" = 'Jones'""",
                 "- Never provide any additional explanation or discussion, only output the SQLite query requested, which answers the question against the given table description.",
                 "- If example rows are given, pay special attention to them to improve your query e.g. to account for abbreviations or formatting of values.",
             ],
             stop_sequences=["\n", ";", "<|eot_id|>"],
+            additional_runnables=[TextCleaningOutputParser(), SQLFindingOutputParser()],
         )
 
     def run(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
     ) -> TracedResponse[ExplainedSQLResult]:
```

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/querying/sql_result_explainer_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/querying/sql_result_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/__init__.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/simple_rag_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/simple_rag_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/standalone_question_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/standalone_question_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/suggested_questions_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/suggested_questions_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/suggested_report_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/suggested_report_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/tool_final_answer_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/tool_final_answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/rag/tool_output_grader_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/rag/tool_output_grader_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/__init__.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/common.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/data_type_detection_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/data_type_detection_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/date_add_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/date_add_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/date_parse_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/date_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/chains/types/timespan_parse_chain.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/chains/types/timespan_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/config.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/config.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/document_loaders/docugami.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/history.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/history.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/__init__.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/custom_react_json_single_input.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/custom_react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/datetime.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/key_finding.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/key_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/line_separated_list.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/line_separated_list.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/sql_finding.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/sql_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/text_cleaning.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/text_cleaning.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/output_parsers/timespan.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/output_parsers/timespan.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/params.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/params.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/retrievers/fused_summary.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/retrievers/fused_summary.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/retrievers/mappings.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/retrievers/mappings.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/tools/common.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/tools/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/tools/reports.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/tools/reports.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/tools/retrieval.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/utils/documents.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/utils/documents.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/utils/sql.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/utils/sql.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/docugami_langchain/utils/string_cleanup.py` & `docugami_langchain-0.0.9rc7/docugami_langchain/utils/string_cleanup.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc6/pyproject.toml` & `docugami_langchain-0.0.9rc7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docugami-langchain"
-version = "0.0.9rc6"
+version = "0.0.9rc7"
 description = "An integration package connecting Docugami and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/docugami/docugami-langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `docugami_langchain-0.0.9rc6/PKG-INFO` & `docugami_langchain-0.0.9rc7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugami-langchain
-Version: 0.0.9rc6
+Version: 0.0.9rc7
 Summary: An integration package connecting Docugami and LangChain
 Home-page: https://github.com/docugami/docugami-langchain
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

