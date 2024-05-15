# Comparing `tmp/transformers_cfg-0.2.0.tar.gz` & `tmp/transformers_cfg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_cfg-0.2.0.tar", last modified: Wed Mar 20 20:02:37 2024, max compression
+gzip compressed data, was "transformers_cfg-0.2.1.tar", last modified: Wed May 15 19:17:47 2024, max compression
```

## Comparing `transformers_cfg-0.2.0.tar` & `transformers_cfg-0.2.1.tar`

### file list

```diff
@@ -1,56 +1,66 @@
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.213244 transformers_cfg-0.2.0/
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     1085 2024-02-01 20:42:38.000000 transformers_cfg-0.2.0/LICENSE
--rw-r--r--   0 saibo     (1000) saibo     (1000)     9044 2024-03-20 20:02:37.213244 transformers_cfg-0.2.0/PKG-INFO
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     8297 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/README.md
--rw-rw-r--   0 saibo     (1000) saibo     (1000)       38 2024-03-20 20:02:37.213244 transformers_cfg-0.2.0/setup.cfg
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      917 2024-02-13 15:26:12.000000 transformers_cfg-0.2.0/setup.py
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.209243 transformers_cfg-0.2.0/tests/
--rw-rw-r--   0 saibo     (1000) saibo     (1000)       75 2024-02-13 13:23:38.000000 transformers_cfg-0.2.0/tests/__init__.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     6771 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/_tokenizer_common.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      269 2024-02-27 19:07:24.000000 transformers_cfg-0.2.0/tests/json_utils.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      906 2024-02-29 20:26:56.000000 transformers_cfg-0.2.0/tests/test_examples.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     5307 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_grammar_constrained_decoding.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)       65 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_mapping.py
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.209243 transformers_cfg-0.2.0/tests/test_parsing/
--rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_parsing/__init__.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)    16161 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_parsing/test_parsing.py
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.209243 transformers_cfg-0.2.0/tests/test_string_recognizer/
--rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_string_recognizer/__init__.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     2589 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_string_recognizer/test_decode_utf8.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     3242 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_string_recognizer/test_json.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     1117 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_string_recognizer/test_json_arr.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     1305 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_string_recognizer/test_unicode.py
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.209243 transformers_cfg-0.2.0/tests/test_token_sequence_recognizer/
--rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_token_sequence_recognizer/__init__.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     3151 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_token_sequence_recognizer/test_accept_unicode_bytes.py
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.209243 transformers_cfg-0.2.0/tests/test_tokenizers/
--rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-02-07 13:11:59.000000 transformers_cfg-0.2.0/tests/test_tokenizers/__init__.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      408 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_tokenizers/test_bloom.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      340 2024-02-29 20:26:56.000000 transformers_cfg-0.2.0/tests/test_tokenizers/test_codegen.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      345 2024-02-29 20:26:56.000000 transformers_cfg-0.2.0/tests/test_tokenizers/test_falcon.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      318 2024-02-13 13:23:39.000000 transformers_cfg-0.2.0/tests/test_tokenizers/test_gpt2.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      353 2024-02-29 20:26:56.000000 transformers_cfg-0.2.0/tests/test_tokenizers/test_gpt_neox.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      331 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_tokenizers/test_llama.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      389 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/tests/test_tokenizers/test_t5.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      375 2024-02-29 20:26:56.000000 transformers_cfg-0.2.0/tests/test_tokenizers/test_xglm.py
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.213244 transformers_cfg-0.2.0/transformers_cfg/
--rw-rw-r--   0 saibo     (1000) saibo     (1000)       82 2024-02-29 20:56:19.000000 transformers_cfg-0.2.0/transformers_cfg/__init__.py
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.213244 transformers_cfg-0.2.0/transformers_cfg/generation/
--rw-rw-r--   0 saibo     (1000) saibo     (1000)       62 2024-02-01 20:42:38.000000 transformers_cfg-0.2.0/transformers_cfg/generation/__init__.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     3975 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/transformers_cfg/generation/logits_process.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      544 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/transformers_cfg/grammar_utils.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      481 2024-02-13 13:23:39.000000 transformers_cfg-0.2.0/transformers_cfg/logging_config.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     8183 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/transformers_cfg/mapping.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)    19135 2024-02-13 12:53:14.000000 transformers_cfg-0.2.0/transformers_cfg/parser.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)    20878 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/transformers_cfg/recognizer.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)    13461 2024-03-20 19:58:24.000000 transformers_cfg-0.2.0/transformers_cfg/token_grammar_recognizer.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     7216 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/transformers_cfg/trie.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     6677 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/transformers_cfg/utf8_utils.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     3275 2024-02-29 20:41:32.000000 transformers_cfg-0.2.0/transformers_cfg/utils.py
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     3022 2024-02-16 15:41:09.000000 transformers_cfg-0.2.0/transformers_cfg/vocab_struct.py
-drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-03-20 20:02:37.213244 transformers_cfg-0.2.0/transformers_cfg.egg-info/
--rw-r--r--   0 saibo     (1000) saibo     (1000)     9044 2024-03-20 20:02:37.000000 transformers_cfg-0.2.0/transformers_cfg.egg-info/PKG-INFO
--rw-rw-r--   0 saibo     (1000) saibo     (1000)     1535 2024-03-20 20:02:37.000000 transformers_cfg-0.2.0/transformers_cfg.egg-info/SOURCES.txt
--rw-rw-r--   0 saibo     (1000) saibo     (1000)        1 2024-03-20 20:02:37.000000 transformers_cfg-0.2.0/transformers_cfg.egg-info/dependency_links.txt
--rw-rw-r--   0 saibo     (1000) saibo     (1000)      142 2024-03-20 20:02:37.000000 transformers_cfg-0.2.0/transformers_cfg.egg-info/requires.txt
--rw-rw-r--   0 saibo     (1000) saibo     (1000)       23 2024-03-20 20:02:37.000000 transformers_cfg-0.2.0/transformers_cfg.egg-info/top_level.txt
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     1085 2024-02-01 20:42:38.000000 transformers_cfg-0.2.1/LICENSE
+-rw-r--r--   0 saibo     (1000) saibo     (1000)     9879 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/PKG-INFO
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     9103 2024-05-15 19:15:12.000000 transformers_cfg-0.2.1/README.md
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)       38 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/setup.cfg
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      917 2024-02-13 15:26:12.000000 transformers_cfg-0.2.1/setup.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.285929 transformers_cfg-0.2.1/tests/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)       75 2024-02-13 13:23:38.000000 transformers_cfg-0.2.1/tests/__init__.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     6793 2024-04-13 18:54:30.000000 transformers_cfg-0.2.1/tests/_tokenizer_common.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      269 2024-02-27 19:07:24.000000 transformers_cfg-0.2.1/tests/json_utils.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      906 2024-02-29 20:26:56.000000 transformers_cfg-0.2.1/tests/test_examples.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     5307 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_grammar_constrained_decoding.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:14:37.000000 transformers_cfg-0.2.1/tests/test_mapping.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.285929 transformers_cfg-0.2.1/tests/test_parsing/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_parsing/__init__.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)    18154 2024-05-15 19:15:14.000000 transformers_cfg-0.2.1/tests/test_parsing/test_parsing.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.285929 transformers_cfg-0.2.1/tests/test_string_recognizer/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/__init__.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)    13763 2024-04-13 18:54:30.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_calflow.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     2589 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_decode_utf8.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     3625 2024-04-16 22:10:38.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_geo_query.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     3242 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_json.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     1117 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_json_arr.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     5951 2024-04-13 18:54:30.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_overnight.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     9022 2024-04-16 22:11:19.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_pddl.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     8945 2024-05-15 19:15:13.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_smiles.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     1305 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_string_recognizer/test_unicode.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.285929 transformers_cfg-0.2.1/tests/test_token_sequence_recognizer/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_token_sequence_recognizer/__init__.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     3151 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_token_sequence_recognizer/test_accept_unicode_bytes.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/tests/test_tokenizers/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-02-07 13:11:59.000000 transformers_cfg-0.2.1/tests/test_tokenizers/__init__.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      408 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_tokenizers/test_bloom.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      340 2024-02-29 20:26:56.000000 transformers_cfg-0.2.1/tests/test_tokenizers/test_codegen.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      345 2024-02-29 20:26:56.000000 transformers_cfg-0.2.1/tests/test_tokenizers/test_falcon.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      318 2024-02-13 13:23:39.000000 transformers_cfg-0.2.1/tests/test_tokenizers/test_gpt2.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      353 2024-02-29 20:26:56.000000 transformers_cfg-0.2.1/tests/test_tokenizers/test_gpt_neox.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      331 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_tokenizers/test_llama.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      389 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/tests/test_tokenizers/test_t5.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      375 2024-02-29 20:26:56.000000 transformers_cfg-0.2.1/tests/test_tokenizers/test_xglm.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/transformers_cfg/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)       82 2024-04-13 18:54:30.000000 transformers_cfg-0.2.1/transformers_cfg/__init__.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/transformers_cfg/generation/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)       62 2024-02-01 20:42:38.000000 transformers_cfg-0.2.1/transformers_cfg/generation/__init__.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     4120 2024-05-15 19:14:37.000000 transformers_cfg-0.2.1/transformers_cfg/generation/logits_process.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      544 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/transformers_cfg/grammar_utils.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      481 2024-02-13 13:23:39.000000 transformers_cfg-0.2.1/transformers_cfg/logging_config.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/transformers_cfg/metrics/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)       47 2024-04-24 11:25:27.000000 transformers_cfg-0.2.1/transformers_cfg/metrics/__init__.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)    12351 2024-04-24 11:25:27.000000 transformers_cfg-0.2.1/transformers_cfg/metrics/metrics.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)    19934 2024-05-15 19:14:37.000000 transformers_cfg-0.2.1/transformers_cfg/parser.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)    21500 2024-05-15 19:14:37.000000 transformers_cfg-0.2.1/transformers_cfg/recognizer.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)    13640 2024-05-15 19:14:37.000000 transformers_cfg-0.2.1/transformers_cfg/token_grammar_recognizer.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/transformers_cfg/tokenization/
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:14:37.000000 transformers_cfg-0.2.1/transformers_cfg/tokenization/__init__.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     8219 2024-05-15 19:14:37.000000 transformers_cfg-0.2.1/transformers_cfg/tokenization/mapping.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     7229 2024-05-15 19:14:37.000000 transformers_cfg-0.2.1/transformers_cfg/tokenization/trie.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     3134 2024-05-15 19:15:13.000000 transformers_cfg-0.2.1/transformers_cfg/tokenization/vocab_struct.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     6677 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/transformers_cfg/utf8_utils.py
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     3275 2024-02-29 20:41:32.000000 transformers_cfg-0.2.1/transformers_cfg/utils.py
+drwxrwxr-x   0 saibo     (1000) saibo     (1000)        0 2024-05-15 19:17:47.289929 transformers_cfg-0.2.1/transformers_cfg.egg-info/
+-rw-r--r--   0 saibo     (1000) saibo     (1000)     9879 2024-05-15 19:17:47.000000 transformers_cfg-0.2.1/transformers_cfg.egg-info/PKG-INFO
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)     1914 2024-05-15 19:17:47.000000 transformers_cfg-0.2.1/transformers_cfg.egg-info/SOURCES.txt
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)        1 2024-05-15 19:17:47.000000 transformers_cfg-0.2.1/transformers_cfg.egg-info/dependency_links.txt
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)      156 2024-05-15 19:17:47.000000 transformers_cfg-0.2.1/transformers_cfg.egg-info/requires.txt
+-rw-rw-r--   0 saibo     (1000) saibo     (1000)       23 2024-05-15 19:17:47.000000 transformers_cfg-0.2.1/transformers_cfg.egg-info/top_level.txt
```

### Comparing `transformers_cfg-0.2.0/LICENSE` & `transformers_cfg-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/PKG-INFO` & `transformers_cfg-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,72 @@
 Metadata-Version: 2.1
 Name: transformers_cfg
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extension of Transformers library for Context-Free Grammar Constrained Decoding with EBNF grammars
 Home-page: https://github.com/epfl-dlab/transformers-CFG
 Author: EPFL-dlab
 Author-email: saibo.geng@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch~=2.2.0
-Requires-Dist: numpy~=1.24.2
-Requires-Dist: transformers~=4.37.2
-Requires-Dist: tokenizers~=0.15.2
-Requires-Dist: termcolor~=2.4.0
-Requires-Dist: sentencepiece~=0.1.99
-Requires-Dist: protobuf~=4.25.2
-Requires-Dist: setuptools~=69.0.3
+Requires-Dist: torch>=2.0.0
+Requires-Dist: numpy>=1.24.2
+Requires-Dist: transformers>=4.37.2
+Requires-Dist: tokenizers>=0.15.2
+Requires-Dist: termcolor>=2.4.0
+Requires-Dist: sentencepiece>=0.1.99
+Requires-Dist: protobuf>=4.25.2
+Requires-Dist: setuptools>=69.0.3
+Requires-Dist: line_profiler
 
 # 🤗 Transformers CFG
 
 ![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
-## Latest News
+## 💭Latest News
 
-**Support for Unicode(multilingual) grammars** (2024-02-29)
-**Integration with Text-Generation-WebUI** (2023-12-17)
+- **[Token masking optimization](#efficiency)(** (2024-04-25)
+
+- **Online [Demo with JSON Grammar](https://huggingface.co/spaces/saibo/transformers-CFG-JSON-demo) at HF space** (2024-04-10)
+
+- **Support for Unicode(multilingual) grammars** (2024-02-29)
+
+- **Integration with Text-Generation-WebUI** (2023-12-17)
 
 We are thrilled to announce that `transformers_cfg` has been used in the [Text-Generation-WebUI](https://github.com/oobabooga/text-generation-webui) project.
 This integration enables users to utilize our CFG capabilities within the popular, 30.5K-starred web interface for text generation.
 For more details, see [Relevent Pull Request](https://github.com/oobabooga/text-generation-webui/pull/4953)
 
 
-## Introduction
+## 🚀Introduction
 `transformers_cfg` is an extension library for the popular Transformers library by Hugging Face, tailored for working with context-free grammars (CFG).
 This package provides additional tools and functionalities to enhance your experience with natural language processing tasks involving CFGs.
 
 It was initially developed as a pull request to the [Hugging Face Transformers](https://github.com/huggingface/transformers) library.
 See relevant discussion [here](https://github.com/huggingface/transformers/pull/27557).
 
-## Installation
+## 💻 Installation
+
+- You can install the stable version of `transformers-cfg` using pip:
 
 ```bash
 pip install transformers-cfg
 ```
 
-## QuickStart: Force LLM to generate a valid json object
+- For the latest code and updates, you can install directly from the GitHub repository:
+
+```
+pip install git+https://github.com/epfl-dlab/transformers-CFG.git@main
+```
+This will install the package directly from the `main` branch of the repository.
+
+## 🔧QuickStart: Force LLM to generate a valid json object
 
 The below example can be found in `examples/generate_json.py`
 
 ```python
 import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from transformers_cfg.grammar_utils import IncrementalGrammarConstraint
@@ -98,22 +113,22 @@
     """
     'This is a valid json string for http request:{ "request": { "method": "GET", "headers": [], "content": "Content","type": "application" }}
     'This is a valid json string for shopping cart:{ "name": "MyCart", "price": 0, "value": 1 }
     """
 
 ```
 
-## Why should I use transformers-CFG?
+## 💡Why should I use transformers-CFG?
 
 - We support EBNF grammar description format
 - We offer the same grammar interface as llama-cpp project, allowing you to drop-in replace llama-cpp with transformers-CFG.
 - We allow you to use any of the models in the 🤗 Transformers library, including the ones that are not supported by llama-cpp.
 - We support multilingual grammars, you can use any character from any language in your grammar, e.g. 中文, 日本語, 한국어, हिन्दी, العربية, עברית, or emoji 🤗.
 
-## What is grammar ?
+## 🤔What is grammar ?
 
 TL;DR: Think of it as an enhanced version of regular expressions.
 
 Here is an example of a simplified JSON grammar:
 ```bnf
 # A JSON object is the root of the grammar
 root ::= object
@@ -175,14 +190,19 @@
 - ...
 
 See [supported_models.yaml](docs%2Fsupported_models.yaml) for the full list of supported models.
 
 As a rule of thumb, all models with the same tokenizer should naturally be supported.
 If you find any model that is not supported, please open an issue or submit a pull request.
 
+## Efficiency
+Our update in the `transformers_cfg` library has significantly improved the performance of grammar-constrained decoding (especially for complicated grammars).
+
+<img src="docs/assets/plots/benchmarking_results.png" style="width: 60%; height: auto;">
+
 ## Citation
 
 **Please consider citing our work, if you found the provided resources useful.**<br>
 ```
 @inproceedings{geng-etal-2023-grammar,
 	title        = {Grammar-Constrained Decoding for Structured {NLP} Tasks without Finetuning},
 	author       = {Geng, Saibo  and Josifoski, Martin  and Peyrard, Maxime  and West, Robert},
```

### Comparing `transformers_cfg-0.2.0/README.md` & `transformers_cfg-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 # 🤗 Transformers CFG
 
 ![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
-## Latest News
+## 💭Latest News
 
-**Support for Unicode(multilingual) grammars** (2024-02-29)
-**Integration with Text-Generation-WebUI** (2023-12-17)
+- **[Token masking optimization](#efficiency)(** (2024-04-25)
+
+- **Online [Demo with JSON Grammar](https://huggingface.co/spaces/saibo/transformers-CFG-JSON-demo) at HF space** (2024-04-10)
+
+- **Support for Unicode(multilingual) grammars** (2024-02-29)
+
+- **Integration with Text-Generation-WebUI** (2023-12-17)
 
 We are thrilled to announce that `transformers_cfg` has been used in the [Text-Generation-WebUI](https://github.com/oobabooga/text-generation-webui) project.
 This integration enables users to utilize our CFG capabilities within the popular, 30.5K-starred web interface for text generation.
 For more details, see [Relevent Pull Request](https://github.com/oobabooga/text-generation-webui/pull/4953)
 
 
-## Introduction
+## 🚀Introduction
 `transformers_cfg` is an extension library for the popular Transformers library by Hugging Face, tailored for working with context-free grammars (CFG).
 This package provides additional tools and functionalities to enhance your experience with natural language processing tasks involving CFGs.
 
 It was initially developed as a pull request to the [Hugging Face Transformers](https://github.com/huggingface/transformers) library.
 See relevant discussion [here](https://github.com/huggingface/transformers/pull/27557).
 
-## Installation
+## 💻 Installation
+
+- You can install the stable version of `transformers-cfg` using pip:
 
 ```bash
 pip install transformers-cfg
 ```
 
-## QuickStart: Force LLM to generate a valid json object
+- For the latest code and updates, you can install directly from the GitHub repository:
+
+```
+pip install git+https://github.com/epfl-dlab/transformers-CFG.git@main
+```
+This will install the package directly from the `main` branch of the repository.
+
+## 🔧QuickStart: Force LLM to generate a valid json object
 
 The below example can be found in `examples/generate_json.py`
 
 ```python
 import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from transformers_cfg.grammar_utils import IncrementalGrammarConstraint
@@ -77,22 +91,22 @@
     """
     'This is a valid json string for http request:{ "request": { "method": "GET", "headers": [], "content": "Content","type": "application" }}
     'This is a valid json string for shopping cart:{ "name": "MyCart", "price": 0, "value": 1 }
     """
 
 ```
 
-## Why should I use transformers-CFG?
+## 💡Why should I use transformers-CFG?
 
 - We support EBNF grammar description format
 - We offer the same grammar interface as llama-cpp project, allowing you to drop-in replace llama-cpp with transformers-CFG.
 - We allow you to use any of the models in the 🤗 Transformers library, including the ones that are not supported by llama-cpp.
 - We support multilingual grammars, you can use any character from any language in your grammar, e.g. 中文, 日本語, 한국어, हिन्दी, العربية, עברית, or emoji 🤗.
 
-## What is grammar ?
+## 🤔What is grammar ?
 
 TL;DR: Think of it as an enhanced version of regular expressions.
 
 Here is an example of a simplified JSON grammar:
 ```bnf
 # A JSON object is the root of the grammar
 root ::= object
@@ -154,14 +168,19 @@
 - ...
 
 See [supported_models.yaml](docs%2Fsupported_models.yaml) for the full list of supported models.
 
 As a rule of thumb, all models with the same tokenizer should naturally be supported.
 If you find any model that is not supported, please open an issue or submit a pull request.
 
+## Efficiency
+Our update in the `transformers_cfg` library has significantly improved the performance of grammar-constrained decoding (especially for complicated grammars).
+
+<img src="docs/assets/plots/benchmarking_results.png" style="width: 60%; height: auto;">
+
 ## Citation
 
 **Please consider citing our work, if you found the provided resources useful.**<br>
 ```
 @inproceedings{geng-etal-2023-grammar,
 	title        = {Grammar-Constrained Decoding for Structured {NLP} Tasks without Finetuning},
 	author       = {Geng, Saibo  and Josifoski, Martin  and Peyrard, Maxime  and West, Robert},
```

### Comparing `transformers_cfg-0.2.0/setup.py` & `transformers_cfg-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/tests/_tokenizer_common.py` & `transformers_cfg-0.2.1/tests/_tokenizer_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                     f"unk token found in input_token_ids: {token_ids}, skipping test"
                 )
                 return
 
         acc_state = JsontokenRecognizer._consume_token_ids(token_ids, as_string=False)
         # the json object is complete, so the stacks should be empty
         self.assertTrue(
-            acc_state.stacks == [] or acc_state.stacks == [[]],
+            acc_state.stacks == set() or acc_state.stacks == set(tuple()),
             f"stacks: {acc_state.stacks}, not empty",
         )
 
     def test_balanced_parentheses(self):
         # Test that we can recognize a balanced parentheses
         with open("examples/grammars/balanced_parentheses.ebnf", "r") as file:
             input_text = file.read()
@@ -84,15 +84,15 @@
                     f"unk token found in input_token_ids: {token_ids}, skipping test"
                 )
                 return
 
         accept_state = recognizer._consume_token_ids(token_ids, as_string=False)
         # the json object is complete, so the stacks should be empty
         self.assertTrue(
-            accept_state.stacks == [] or accept_state.stacks == [[]],
+            accept_state.stacks == set() or accept_state.stacks == set(tuple()),
             f"stacks: {accept_state.stacks}, not empty",
         )
 
         # inbalanced_parentheses = "((((((((()))))))))))))"
         # token_ids = self.tokenizer.encode(inbalanced_parentheses)
         # pprint_token_ids(self.tokenizer, token_ids)
         #
```

### Comparing `transformers_cfg-0.2.0/tests/test_examples.py` & `transformers_cfg-0.2.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/tests/test_grammar_constrained_decoding.py` & `transformers_cfg-0.2.1/tests/test_grammar_constrained_decoding.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/tests/test_parsing/test_parsing.py` & `transformers_cfg-0.2.1/tests/test_parsing/test_parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,14 +134,55 @@
         non_ascii_char_src = '"你"'
         outbuf = []
 
         remaining_src = _parse_rhs_literal_string(non_ascii_char_src, outbuf)
         self.assertEqual(3, len(outbuf), f"len(outbuf): {len(outbuf)} != 3")
         self.assertListEqual([2, ord("你"), ord("你")], outbuf)
 
+    def test__parse_escape(self):
+        escaped_char_src = '"\\n"'
+        outbuf = []
+
+        remaining_src = _parse_rhs_literal_string(escaped_char_src, outbuf)
+        self.assertEqual(3, len(outbuf), f"len(outbuf): {len(outbuf)} != 3")
+        self.assertListEqual([2, ord("\n"), ord("\n")], outbuf)
+
+        escaped_backslash_src = '"\\\\"'
+        outbuf = []
+
+        remaining_src = _parse_rhs_literal_string(escaped_backslash_src, outbuf)
+        self.assertEqual(3, len(outbuf), f"len(outbuf): {len(outbuf)} != 3")
+        self.assertListEqual([2, ord("\\"), ord("\\")], outbuf)
+        self.assertEqual("", remaining_src, f"remaining_src: {remaining_src} != ''")
+
+        escaped_backslash_src = '"\\x5C"'
+        outbuf = []
+
+        remaining_src = _parse_rhs_literal_string(escaped_backslash_src, outbuf)
+        self.assertEqual(3, len(outbuf), f"len(outbuf): {len(outbuf)} != 3")
+        self.assertListEqual([2, ord("\\"), ord("\\")], outbuf)
+        self.assertEqual("", remaining_src, f"remaining_src: {remaining_src} != ''")
+
+    def test__parse_escape_unicode(self):
+        # Test for 16-bit Unicode escape
+        escaped_unicode_16_src = '"\\u20AC"'  # Unicode for Euro symbol
+        outbuf = []
+        remaining_src = _parse_rhs_literal_string(escaped_unicode_16_src, outbuf)
+        self.assertEqual(3, len(outbuf), f"len(outbuf): {len(outbuf)} != 3")
+        self.assertListEqual([2, ord("€"), ord("€")], outbuf)
+        self.assertEqual("", remaining_src, f"remaining_src: {remaining_src} != ''")
+
+        # Test for 32-bit Unicode escape
+        escaped_unicode_32_src = '"\\U0001F600"'  # Unicode for grinning face emoji
+        outbuf = []
+        remaining_src = _parse_rhs_literal_string(escaped_unicode_32_src, outbuf)
+        self.assertEqual(3, len(outbuf), f"len(outbuf): {len(outbuf)} != 3")
+        self.assertListEqual([2, ord("😀"), ord("😀")], outbuf)
+        self.assertEqual("", remaining_src, f"remaining_src: {remaining_src} != ''")
+
     def test_null(self):
         src = "root ::= "
         rhs_src = ""
         state = ParseState()
         state.symbol_table["root"] = 9
         _ = parse_rhs(
             state=state, rhs=rhs_src, rule_name="root", rule_id=9, is_nested=False
```

### Comparing `transformers_cfg-0.2.0/tests/test_string_recognizer/test_decode_utf8.py` & `transformers_cfg-0.2.1/tests/test_string_recognizer/test_decode_utf8.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/tests/test_string_recognizer/test_json.py` & `transformers_cfg-0.2.1/tests/test_string_recognizer/test_json.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/tests/test_string_recognizer/test_json_arr.py` & `transformers_cfg-0.2.1/tests/test_string_recognizer/test_json_arr.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/tests/test_string_recognizer/test_unicode.py` & `transformers_cfg-0.2.1/tests/test_string_recognizer/test_unicode.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/tests/test_token_sequence_recognizer/test_accept_unicode_bytes.py` & `transformers_cfg-0.2.1/tests/test_token_sequence_recognizer/test_accept_unicode_bytes.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/transformers_cfg/generation/logits_process.py` & `transformers_cfg-0.2.1/transformers_cfg/generation/logits_process.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import math
 import os
 import pprint
 
 import torch
 import logging
+from line_profiler import profile
 from transformers.generation.logits_process import (
     LogitsProcessor,
     LOGITS_PROCESSOR_INPUTS_DOCSTRING,
 )
 from transformers.utils import add_start_docstrings
 
 logger = logging.getLogger(__name__)
@@ -18,14 +19,15 @@
     def __init__(self, grammar_constraint, parse_start_index=None):
         self.last_size = None
         self.grammar_constraint = grammar_constraint
         self.batch_accept_states = None
         self.parse_start_index = None
 
     def mask_logits(self, logits, device):
+        masked_logits = logits.clone()
         # resolve each stack to a tensor of True/False for each token
         # indicating acceptance
         # acceptance = self.grammar_acceptor.filter_vocab(self.stacks, device)
         acceptance = self.grammar_constraint.batch_filter_vocab(
             self.batch_accept_states, device
         )
         # acceptance is a tensor of shape (batch_size, vocab_size)
@@ -50,15 +52,16 @@
                     for token_id in token_ids
                 ]
                 for i, token_ids in accepted_token_indices.items()
             }
             logger.debug("Accepted tokens for the current batch:")
             logger.debug("\n" + pprint.pformat(accepted_tokens))
         # Logits to -inf where False
-        logits[~acceptance] = -math.inf
+        masked_logits[~acceptance] = -math.inf
+        return masked_logits
 
     # TODO: batching
     def process_logits(self, input_ids, scores):
         """
         :param input_ids:
         :param scores:
         :return:
@@ -83,20 +86,21 @@
             "num of stacks: \n"
             + pprint.pformat(
                 [len(acc_state.stacks) for acc_state in self.batch_accept_states]
             )
         )
         # logger.debug("stacks: \n" + pprint.pformat(self.batch_accept_states.stacks))
 
-        self.batch_accept_states = self.grammar_constraint.advance_token_ids(
+        self.batch_accept_states = self.grammar_constraint.consume_token_ids(
             input_ids, self.batch_accept_states, self.parse_start_index
         )
         logger.debug(f"input_ids: {input_ids}")
 
-        self.mask_logits(scores, scores.device)
-        return scores
+        masked_scores = self.mask_logits(scores, scores.device)
+        return masked_scores
 
     @add_start_docstrings(LOGITS_PROCESSOR_INPUTS_DOCSTRING)
+    @profile
     def __call__(
         self, input_ids: torch.LongTensor, scores: torch.FloatTensor
     ) -> torch.FloatTensor:
         return self.process_logits(input_ids, scores)
```

### Comparing `transformers_cfg-0.2.0/transformers_cfg/grammar_utils.py` & `transformers_cfg-0.2.1/transformers_cfg/grammar_utils.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/transformers_cfg/mapping.py` & `transformers_cfg-0.2.1/transformers_cfg/tokenization/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 
 class Mapping:
     def __init__(self, tokenizer):
         self.eos_token_id = tokenizer.eos_token_id
         self.bos_token_id = tokenizer.bos_token_id
         self.tokenizer = tokenizer
         self.special = tokenizer.all_special_ids
+        self._length = len(self.tokenizer.get_vocab())
 
     def __len__(self):
-        return len(self.tokenizer.get_vocab())
+        return self._length
 
     def _map(self, token_id: int) -> str:
         # This is the case for BOS,
         if token_id in self.special:
             return ""
         # if token_id is tensor, convert it to int
         if hasattr(token_id, "item"):
```

### Comparing `transformers_cfg-0.2.0/transformers_cfg/parser.py` & `transformers_cfg-0.2.1/transformers_cfg/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -123,24 +123,40 @@
     if src[0] == "\\":
         esc = src[1]
         if esc == "x":
             first = hex_to_int(src[2])
             if first > -1:
                 second = hex_to_int(src[3])
                 if second > -1:
-                    return (first << 4) + second, src[4:]
+                    return chr((first << 4) + second), src[4:]
             raise RuntimeError("expecting \\xNN at " + src)
+        elif esc == "u":
+            if len(src) >= 6:
+                hex_value = src[2:6]
+                if all(c in "0123456789ABCDEFabcdef" for c in hex_value):
+                    return chr(int(hex_value, 16)), src[6:]
+                raise RuntimeError("expecting \\uXXXX at " + src)
+            raise RuntimeError("incomplete \\uXXXX escape at " + src)
+        elif esc == "U":
+            if len(src) >= 10:
+                hex_value = src[2:10]
+                if all(c in "0123456789ABCDEFabcdef" for c in hex_value):
+                    return chr(int(hex_value, 16)), src[10:]
+                raise RuntimeError("expecting \\UXXXXXXXX at " + src)
+            raise RuntimeError("incomplete \\UXXXXXXXX escape at " + src)
         elif esc in ('"', "[", "]"):
             return esc, src[2:]
         elif esc == "r":
             return "\r", src[2:]
         elif esc == "n":
             return "\n", src[2:]
         elif esc == "t":
             return "\t", src[2:]
+        elif esc == "\\":
+            return "\\", src[2:]
         raise RuntimeError("unknown escape at " + src)
     elif src:
         return src[0], src[1:]
     raise RuntimeError("unexpected end of input")
 
 
 def _parse_rhs_literal_string(src: str, outbuf: List[int]) -> str:
```

### Comparing `transformers_cfg-0.2.0/transformers_cfg/recognizer.py` & `transformers_cfg-0.2.1/transformers_cfg/recognizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import logging
 from functools import lru_cache
-from typing import List, Tuple, Dict
+from typing import List, Tuple, Set, Optional
 
 from transformers_cfg.parser import (
     END_OF_RULE_MARKER,
     END_OF_ALTERNATE_MARKER,
     parse_ebnf,
     REF_RULE_MARKER,
 )
@@ -17,48 +17,48 @@
 class AcceptState:
     def __init__(self, stacks, partial_utf8):
         self.stacks = stacks
         self.partial_utf8 = partial_utf8
 
     @staticmethod
     def empty_state():
-        return AcceptState([], PartialUTF8())
+        return AcceptState(set(), PartialUTF8())
 
 
 class StringRecognizer:
     def __init__(
         self,
         grammar_encoding: List[int],
-        start_rule_id: int = None,
-        rule_offsets: List[int] = None,
-        stacks: List[List[int]] = None,
+        start_rule_id: int = -1,
+        rule_offsets: Optional[List[int]] = None,
+        stacks: Optional[Set[Tuple[int]]] = None,
     ):
         # strictly speaking, we don't need to copy grammar_encoding because we don't modify it
         # but we do it anyway to be safe
         # in case where the grammar is very large, we can consider not copying it
         self.grammar_encoding = grammar_encoding
         if rule_offsets is not None:
             self.rule_offsets = rule_offsets
         else:
-            if start_rule_id is None:
+            if start_rule_id == -1:
                 raise ValueError("start_rule_id cannot be None if rule_offsets is None")
             self.rule_offsets = self.init_rules(start_rule_id)
         # each stack is a list of indices into grammar_encoding
         # each index points to a rule's
         if stacks is not None:
             self.stacks = stacks
         else:
-            if start_rule_id is None:
+            if start_rule_id == -1:
                 raise ValueError("start_rule_id cannot be None if stacks is None")
-            self.stacks: List[List[int]] = self.init_stack(start_rule_id)
+            self.stacks = self.init_stack(start_rule_id)
         self.start_rule_id = start_rule_id
 
     def init_rules(self, start_rule_id: int) -> List[int]:
         _rule_offset = 0
-        rule_offsets = []
+        rule_offsets: List = []
         # Build `rules` as an array of rule IDs to their positions in `grammar_src`
         while self.grammar_encoding[_rule_offset] != 0xFFFF:
             rule_id = self.grammar_encoding[_rule_offset]
             # store the offset idx
             if len(rule_offsets) <= rule_id:
                 rule_offsets.extend([-1] * (rule_id - len(rule_offsets) + 1))
             rule_offsets[rule_id] = _rule_offset
@@ -78,213 +78,230 @@
             _rule_offset = simple_rhs_offset + 1
 
         retrieved_start_rule_id = self.grammar_encoding[rule_offsets[start_rule_id]]
         assert retrieved_start_rule_id == start_rule_id
 
         return rule_offsets
 
-    def init_stack(self, start_rule_id: int) -> List[List[int]]:
+    def init_stack(self, start_rule_id: int) -> Set[Tuple[int]]:
 
-        stacks = []
+        stacks = set()
         # Loop over alternates of start rule to build initial stacks
         sub_rhs_offset = self.rule_offsets[start_rule_id] + 1
         while self.grammar_encoding[sub_rhs_offset]:
             stack: List[int] = []
             # If alternate is nonempty, add to stack
             element_offset = sub_rhs_offset + 1
             if self.grammar_encoding[element_offset] != END_OF_ALTERNATE_MARKER:
                 stack.append(element_offset)
-            stacks.extend(self.advance_stack(tuple(stack)))
+            stacks.update(self.expand_stack_head(tuple(stack)))
             sub_rhs_offset += 1 + self.grammar_encoding[sub_rhs_offset]
         return stacks
 
     def get_initial_accept_state(self) -> AcceptState:
         return AcceptState(self.init_stack(self.start_rule_id), PartialUTF8())
 
     def get_termination_accept_state(self) -> AcceptState:
-        return AcceptState([], PartialUTF8())
+        return AcceptState(set(), PartialUTF8())
 
     @lru_cache(maxsize=32768)
-    def advance_stack(self, stack: Tuple[int]) -> List[List[int]]:
-        stack = list(stack)
+    def expand_stack_head(self, stack: Tuple[int]) -> Set[Tuple[int]]:
+        """
+        Stack is the internal state of the recognizer(Pushdown Automaton).
+        This method updates the stack by advancing it to the next element.
+        If the element is a non-terminal, it expands the stack by adding the elements of the referenced rule.
+        A new stack is created for each alternate of the referenced rule, so we could have multiple stacks as output.
+        :param stack:
+        :return:
+        """
         if len(stack) == 0:
-            return [stack]
+            return {stack}
 
         # we get the last element of the stack, which is the element we are currently processing
         cur_element_offset = stack[-1]
 
         # if the element is a terminal, we don't need to advance the stack
         if self.grammar_encoding[cur_element_offset] != REF_RULE_MARKER:
-            return [stack]
+            return {stack}
         # the remaining case is that the element is a non-terminal, i.e. a reference to another rule
         else:
             ref_rule_id = self.grammar_encoding[cur_element_offset + 1]
             # find the offset of the referenced rule
             ref_subrule_offset = self.rule_offsets[ref_rule_id] + 1
-            new_stacks: List[List[int]] = []
+            new_stacks: Set[Tuple[int]] = set()
             # Loop over alternates of referenced rule to build new stacks
             while self.grammar_encoding[ref_subrule_offset] != END_OF_RULE_MARKER:
                 # copy the original stack without the last element
-                new_stack = stack[:-1]
+                new_stack = list(stack[:-1])
                 # if the rule ref is followed by another element, we add it to the stack
                 next_element_offset = cur_element_offset + 2
                 if (
                     self.grammar_encoding[next_element_offset]
                     != END_OF_ALTERNATE_MARKER
                 ):
                     new_stack.append(next_element_offset)
 
                 # if the referenced rule is not empty, we add its element offset to the stack
                 ref_element_offset = ref_subrule_offset + 1
                 if self.grammar_encoding[ref_element_offset] != END_OF_ALTERNATE_MARKER:
                     new_stack.append(ref_element_offset)
 
-                new_stacks.extend(self.advance_stack(tuple(new_stack)))
+                new_stacks.update(self.expand_stack_head(tuple(new_stack)))
                 ref_subrule_offset += self.grammar_encoding[ref_subrule_offset] + 1
 
             return new_stacks
 
-    def _consume_byte(self, byte: int, accept_state: AcceptState):
+    def _consume_byte(self, byte: int, accept_state: AcceptState) -> AcceptState:
         # suppose we have code point 一, ord('一') = 19968, we need to match 3 bytes
         # we need to match 3 bytes, so we need to call _consume_byte_partial_match 3 times
-        self._consume_bytes(bytes([byte]), accept_state)
+        return self._consume_bytes(bytes([byte]), accept_state)
 
     # @lru_cache(maxsize=32768)
-    def _probe_bytes(
+    def _try_accept_bytes(
         self,
         byte_seq: bytes,
-        stacks: List[List[int]],
+        stacks: Set[Tuple[int]],
         partial_utf8: PartialUTF8,
         verbose=True,
     ):
+        """
+        The difference between accept_bytes and consume_bytes is that accept_bytes returns a boolean and
+        consume_bytes returns a new accept state
+        """
         if type(byte_seq) is list:
             byte_seq = bytes(byte_seq)
         code_points, new_partial_utf8 = decode_utf8(byte_seq, partial_utf8)
         if verbose:
             logging.debug(
                 f"code_points: {code_points}; new_partial_utf8: {new_partial_utf8}"
             )
-        new_stacks = self._consume_code_points(code_points, stacks)
+        new_stacks = self._consume_code_points_for_all_stacks(code_points, stacks)
 
         for stack in new_stacks:
 
             # stack is empty, meaning that the variables are all consumed
             if len(stack) == 0:
                 return True
             element_offset = stack[-1]
             if self.partial_utf8_accept_at_element(element_offset, new_partial_utf8):
                 return True
         return False
 
     def _consume_bytes(
         self,
         byte_seq: bytes,
-        accept_state: AcceptState = None,
+        accept_state: Optional[AcceptState] = None,
         verbose=True,
-    ):
+    ) -> AcceptState:
         if accept_state is None:
             accept_state = self.get_initial_accept_state()
         stacks = accept_state.stacks
         partial_utf8 = accept_state.partial_utf8
         if type(byte_seq) is list:
             byte_seq = bytes(byte_seq)
         code_points, new_partial_utf8 = decode_utf8(byte_seq, partial_utf8)
         if verbose:
             logging.debug(
                 f"code_points: {code_points}; new_partial_utf8: {new_partial_utf8}"
             )
-        new_stacks = self._consume_code_points(code_points, stacks)
+        new_stacks = self._consume_code_points_for_all_stacks(code_points, stacks)
 
-        new_new_stacks = []
+        new_new_stacks = set()
         for stack in new_stacks:
             if len(stack) == 0:
                 continue
             element_offset = stack[-1]
             if self.partial_utf8_accept_at_element(element_offset, new_partial_utf8):
-                new_new_stacks.append(stack)
+                new_new_stacks.add(stack)
         return AcceptState(new_new_stacks, new_partial_utf8)
 
     ##########################
     #
     # Code point recognition
     #
     ##########################
 
     @lru_cache(maxsize=30000)
-    def _consume_code_point(
+    def _consume_code_point_for_all_stacks(
         self, code_point: int, stacks: Tuple[Tuple[int]]
-    ) -> List[List[int]]:
+    ) -> Set[Tuple[int]]:
         """
         consume a character from the stack
         char_code_point: can be a Unicode code point, including ascii code points which are in the range [0, 127]
         """
-        new_stacks = []
+        new_stacks: Set[Tuple[int]] = set()
 
-        stacks: List[List[int]] = list([list(stack) for stack in stacks])
         if code_point == 0:
             return new_stacks
         for stack in stacks:
-            new_stacks.extend(
-                self._consume_code_point_per_stack(code_point, tuple(stack))
+            new_stacks.update(
+                self._consume_code_point_for_single_stack(code_point, stack)
             )
         return new_stacks
 
     @lru_cache(maxsize=30000)
-    def _consume_code_point_per_stack(
+    def _consume_code_point_for_single_stack(
         self, code_point: int, stack: Tuple[int]
-    ) -> List[List[int]]:
+    ) -> Set[Tuple[int]]:
         """
         consume a character from the stack
         char_code_point: can be a Unicode code point, including ascii code points which are in the range [0, 127]
         """
         # TODO, the below code will raise an error when the stack is empty, but why is this happening?
         # if len(stacks) == 0:
         #     raise ValueError("Stacks don't contain any stack, meaning that no character can be consumed")
         # code_point = 0 is a special case when the uf8 sequence is not complete, we return an empty stack
         # to indicate that the character is not accepted
-        stack = list(stack)
-        new_stacks = []
+
+        new_stacks: Set[Tuple[int]] = set()
         if code_point == 0:
             return new_stacks
         # stack is empty
         if len(stack) == 0:
             return new_stacks
 
         element_offset = stack[-1]
 
         found = self.accept_code_point_at_element(code_point, element_offset)
         if not found:
             return new_stacks
 
         size = self.grammar_encoding[element_offset]
         element_offset += size + 1
-        new_stack = stack[:-1]
+        new_stack = list(stack[:-1])
         if self.grammar_encoding[element_offset]:
             new_stack.append(element_offset)
-        return self.advance_stack(tuple(new_stack))
+        # # Explicitly convert list to tuple of int to make it hashable
+        new_tuple_stack: Tuple[int, ...] = tuple(new_stack)
+        return self.expand_stack_head(new_tuple_stack)
+
+    def _consume_code_points_for_all_stacks(
+        self, code_points: List[int], stacks: Set[Tuple[int]], verbose=False
+    ) -> Set[Tuple[int]]:
+        """
+        code points is a list of Unicode code points. For example, the code points for "hello" is [104, 101, 108, 108, 111]
+        For unicode string "こんにちは世界", the code points are [12371, 12435, 12395, 12385, 12399, 19990, 30028]
 
-    def _consume_code_points(
-        self, code_points: List[int], stacks: List[List[int]], verbose=False
-    ) -> List[List[int]]:
+        """
         for i, code_point in enumerate(code_points):
             # for lru_cache to work, we need to convert the list of stacks into a tuple of stacks
-            tuple_stacks: Tuple[Tuple[int]] = tuple([tuple(stack) for stack in stacks])
-            stacks = self._consume_code_point(code_point, tuple_stacks)
+            tuple_stacks: Tuple[Tuple[int], ...] = tuple(stacks)
+            stacks = self._consume_code_point_for_all_stacks(code_point, tuple_stacks)
             if len(stacks) > 0 and verbose:
                 accepted_code_point = code_points[: i + 1]
                 corresponding_char = chr(code_point)
                 logging.debug(
                     f"code point {accepted_code_point} corresponding to {corresponding_char} is accepted"
                 )
         return stacks
 
     def _accept_code_points(
-        self, code_points: List[int], stacks: List[List[int]], verbose=False
+        self, code_points: List[int], stacks: Set[Tuple[int]], verbose=False
     ) -> bool:
-        stacks = self._consume_code_points(code_points, stacks, verbose)
+        stacks = self._consume_code_points_for_all_stacks(code_points, stacks, verbose)
         return len(stacks) > 0
 
     @lru_cache(maxsize=30000)
     def accept_code_point_at_element(
         self, code_point: int, element_offset: int
     ) -> bool:
         size = self.grammar_encoding[element_offset]
@@ -295,20 +312,14 @@
                 self.grammar_encoding[element_offset + i]
                 <= code_point
                 <= self.grammar_encoding[element_offset + i + 1]
             ):
                 return True
         return False
 
-    # def _accept_code_point(self, code_point: int, stacks: List[List[int]]):
-    #     # for lru_cache to work, we need to convert the list of stacks into a tuple of stacks
-    #     tuple_stacks: Tuple[Tuple[int]] = tuple([tuple(stack) for stack in stacks])
-    #     new_stacks: List[List[int]] = self._consume_code_point(code_point, tuple_stacks)
-    #     return len(new_stacks) > 0
-
     #############################
     #
     # Partial UTF-8 recognition
     #
     #############################
 
     def partial_utf8_accept_at_element(
@@ -363,44 +374,46 @@
     # String recognition
     #
     #############################
 
     def _consume_string(self, string: str, accept_state: AcceptState):
         # _bytes = bytes(string, "utf-8")
         code_points = [ord(char) for char in string]
-        stacks = self._consume_code_points(code_points, accept_state.stacks)
+        stacks = self._consume_code_points_for_all_stacks(
+            code_points, accept_state.stacks
+        )
         return AcceptState(stacks, accept_state.partial_utf8)
 
-    def _accept_prefix(self, string: str, accept_state: AcceptState = None):
+    def _accept_prefix(self, string: str, accept_state: Optional[AcceptState] = None):
         if accept_state is None:
             accept_state = self.get_initial_accept_state()
         new_accept_state = self._consume_string(string, accept_state)
         return len(new_accept_state.stacks) > 0
 
-    def _accept_string(self, string: str, accept_state: AcceptState = None):
+    def _accept_string(self, string: str, accept_state: Optional[AcceptState] = None):
         if accept_state is None:
             accept_state = self.get_initial_accept_state()
         new_accept_state = self._consume_string(string, accept_state)
         at_least_one_stack_is_empty = any(
             len(stack) == 0 for stack in new_accept_state.stacks
         )
         return at_least_one_stack_is_empty
 
-    def _can_stop(self, stacks: List[List[int]]):
+    def _can_stop(self, stacks: Set[Tuple[int]]):
         # This happens in practice, but maybe it shouldn't? TODO
         if len(stacks) == 0:
             return True
         # if any of the stack is empty, we can stop
         for stack in stacks:
             if len(stack) == 0:
                 return True
         else:
             return False
 
-    def _must_stop(self, stacks: List[List[int]]):
+    def _must_stop(self, stacks: Set[Tuple[int]]):
         return len(stacks) == 0 or all(len(stack) == 0 for stack in stacks)
 
     #############################
     #
     # Not Used
     #
     #############################
@@ -427,37 +440,35 @@
             start = self.grammar_encoding[element_offset + i]
             end = self.grammar_encoding[element_offset + i + 1]
             for j in range(start, end + 1):
                 acceptance[j] = True
         logging.debug(acceptance)
         return acceptance
 
-    def _consume_code_points_new(
-        self, code_points: List[int], stacks: List[List[int]], verbose=False
-    ) -> List[List[int]]:
-        new_stacks: List[List[int]] = []
-        for stack in stacks:
-            new_stacks.extend(
-                self._consume_code_points_per_stack(
-                    tuple(code_points), tuple(stack), verbose
-                )
-            )
-        return new_stacks
-
-    @lru_cache(maxsize=30000)
-    def _consume_code_points_per_stack(
-        self, code_points: Tuple[int], stack: Tuple[int], verbose=False
-    ) -> List[List[int]]:
-        code_points = list(code_points)
-        stacks = (stack,)
-        for i, code_point in enumerate(code_points):
-            # for lru_cache to work, we need to convert the list of stacks into a tuple of stacks
-            stacks = self._consume_code_point(code_point, stacks)
-            stacks = tuple([tuple(stack) for stack in stacks])
-        return [list(stack) for stack in stacks]
+    # def _consume_code_points_new(
+    #     self, code_points: List[int], stacks: Set[Tuple[int]], verbose=False
+    # ) -> Set[Tuple[int]]:
+    #     new_stacks: Set[Tuple[int]] = set()
+    #     for stack in stacks:
+    #         new_stacks.update(
+    #             self._consume_code_points_per_stack(tuple(code_points), stack, verbose)
+    #         )
+    #     return new_stacks
+    #
+    # @lru_cache(maxsize=30000)
+    # def _consume_code_points_per_stack(
+    #     self, code_points: Tuple[int], stack: Tuple[int], verbose=False
+    # ) -> Set[Tuple[int]]:
+    #     stacks = {stack}
+    #
+    #     for code_point in code_points:
+    #         # Update the stacks variable by consuming each code point.
+    #         stacks = self._consume_code_point_for_all_stacks(code_point, (stack,))
+    #
+    #     return stacks
 
 
 if __name__ == "__main__":
     # set logging level
 
     with open("examples/grammars/japanese.ebnf", "r") as file:
         input_text = file.read()
@@ -493,17 +504,17 @@
 
     byte_tokens = [bytes_japanese[i] for i in range(len(bytes_japanese))]
     # cast into bytes
     byte_tokens = [bytes([byte]) for byte in byte_tokens]
 
     accept_state = AcceptState(recognizer.stacks, PartialUTF8())
     for i, byte in enumerate(byte_tokens):
-        new_accept_state = recognizer._consume_bytes(byte, accept_state)
-        logging.debug(f"new partial utf8: {new_accept_state.partial_utf8}")
-        if len(new_accept_state.stacks) > 0:
+        accept_state = recognizer._consume_bytes(byte, accept_state)
+        logging.debug(f"new partial utf8: {accept_state.partial_utf8}")
+        if len(accept_state.stacks) > 0:
             logging.debug(f"byte {byte} is accepted")
         else:
             logging.debug(f"byte {byte} is not accepted")
 
     # korean = "안녕하세요"
     # korean_bytes = bytes(korean, "utf-8")
     # head_bytes = korean_bytes[:8]
```

### Comparing `transformers_cfg-0.2.0/transformers_cfg/token_grammar_recognizer.py` & `transformers_cfg-0.2.1/transformers_cfg/token_grammar_recognizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import copy
 import logging
 from abc import ABC
 from functools import lru_cache
-from typing import List
+from typing import List, Optional
 
 import torch
 
 from transformers_cfg.recognizer import StringRecognizer, AcceptState
 from transformers_cfg.parser import parse_ebnf
-from transformers_cfg.trie import ByteTrie
-from transformers_cfg.utf8_utils import PartialUTF8
-from .vocab_struct import LEAF, TokenTrie
-from transformers_cfg.mapping import get_mapping
+from transformers_cfg.tokenization.trie import ByteTrie
+from transformers_cfg.tokenization.vocab_struct import LEAF, TokenTrie
+from transformers_cfg.tokenization.mapping import get_mapping
 
 logger = logging.getLogger(__name__)
 
 
 class AbsTokenRecognizer(ABC):
     def __init__(self, grammar_str, tokenizer, start_rule_name="root", unicode=False):
         parsed_grammar = parse_ebnf(grammar_str)
@@ -64,15 +62,15 @@
 
         bytes_or_codepoints = self.mapping.map(token_id)
         accept_state = self.string_recognizer._consume_bytes(
             bytes_or_codepoints, accept_state
         )
         return accept_state
 
-    def probe_token_id(self, token_id: int, accept_state: AcceptState) -> bool:
+    def try_accept_token_id(self, token_id: int, accept_state: AcceptState) -> bool:
         stacks = accept_state.stacks
         if self.string_recognizer._must_stop(stacks):
             if token_id == self.eos_token_id:
                 return True
             else:
                 return False
         if token_id == self.eos_token_id:
@@ -86,15 +84,15 @@
         #     stacks = self.grammar._consume_char_code_point(code_point, stacks)
         bytes_or_codepoints = self.mapping.map(token_id, verbose=False)
         new_acc_state = self.string_recognizer._consume_bytes(
             bytes_or_codepoints, accept_state, verbose=False
         )
         return len(new_acc_state.stacks) > 0
 
-    def advance_token_ids(self, *args, **kwargs):
+    def consume_token_ids(self, *args, **kwargs):
         """Process a list of tokens according to the grammar rules."""
         raise NotImplementedError
 
     def batch_filter_vocab(self, batch_accept_states, device) -> torch.Tensor:
         batch_acceptance = []
         for accept_state in batch_accept_states:
             batch_acceptance.append(self.filter_vocab(accept_state, device))
@@ -128,20 +126,19 @@
         acceptance = acceptance_matrix.reshape(len(accept_state.stacks), -1).any(dim=0)
         return acceptance
 
     @lru_cache(maxsize=32768)
     def get_token_acceptance_array_for_stack(self, stack, partial_utf8, device):
         # stack = list(stack)  # needs to come in as a tuple for lru_cache
         assert isinstance(stack, tuple)
-        stack = list(stack)
 
         if self.byte_encoding:
 
-            accept_f = lambda x: self.string_recognizer._probe_bytes(
-                x, [stack], partial_utf8=partial_utf8
+            accept_f = lambda x: self.string_recognizer._try_accept_bytes(
+                x, {stack}, partial_utf8=partial_utf8
             )
             token_acceptance = self.unicode_trie.get_token_acceptance(
                 accept=accept_f, accept_eos=False, eos_token_id=self.eos_token_id
             )
         else:
             accepts = [False] * len(self.mapping)
             token_acceptance = check_token_acceptance_in_trie(
@@ -169,21 +166,23 @@
     def __init__(self, grammar_str, start_rule_name, tokenizer, unicode=False):
         super().__init__(grammar_str, tokenizer, start_rule_name, unicode)
         self.last_size = None
 
         # if self.last_size is not set (which would be the case when processing the first token).
         # In this case, do nothing.
 
-    def advance_token_ids(self, input_ids, batch_accept_states, parse_start_index=None):
+    def consume_token_ids(self, input_ids, batch_accept_states, parse_start_index=None):
 
         if self.last_size is None:
             prefix_to_parse = [
-                single_input_ids[parse_start_index:]
-                if parse_start_index is not None
-                else []
+                (
+                    single_input_ids[parse_start_index:]
+                    if parse_start_index is not None
+                    else []
+                )
                 for single_input_ids in input_ids
             ]
 
             # self.grammar_acceptor.accept_token_ids(prefix_to_parse, self.stacks)
             batch_accept_states = [
                 self._consume_token_ids(prefix, accept_state)
                 for prefix, accept_state in zip(prefix_to_parse, batch_accept_states)
@@ -216,15 +215,18 @@
                 "GrammarConstrainedLogitsProcessor."
             )
         self.last_size = len(input_ids[0])
 
         return batch_accept_states
 
     def _consume_token_ids(
-        self, token_ids: List[int], accept_state: AcceptState = None, as_string=True
+        self,
+        token_ids: List[int],
+        accept_state: Optional[AcceptState] = None,
+        as_string=True,
     ):
         if accept_state is None:
             accept_state = self.string_recognizer.get_initial_accept_state()
         if as_string:
             string = self.tokenizer.decode(token_ids)
             accept_state = self.string_recognizer._consume_string(string, accept_state)
         else:
@@ -245,33 +247,33 @@
             token_id = next_trie
             if token_id != eos_token_id:
                 # if the stacks is not empty, it means we can still continue to parse
                 # so we should accept the token
                 accepts[token_id] = bool(stacks)
             continue
 
-        new_stacks = []
+        new_stacks = set()
         for stk in stacks:
             if not stk:
                 continue
 
             next_element_offset = stk[-1]
             num_chars = grammar.grammar_encoding[next_element_offset]
 
             if not grammar.char_acceptance_at_element(next_element_offset).get(
                 byte, False
             ):
                 # if the current byte is not accepted by the current rule, we need to try next rule
                 continue
 
             next_element_offset += num_chars + 1
-            new_stack = stk[:-1]
+            new_stack = list(stk[:-1])
             if grammar.grammar_encoding[next_element_offset]:
                 new_stack.append(next_element_offset)
-            new_stacks.extend(grammar.advance_stack(tuple(new_stack)))
+            new_stacks.update(grammar.expand_stack_head(tuple(new_stack)))
 
         if new_stacks:
             check_token_acceptance_in_trie(
                 next_trie, new_stacks, grammar, eos_token_id, accepts
             )
 
     return accepts
@@ -284,35 +286,40 @@
         input_text = file.read()
     parsed_grammar = parse_ebnf(input_text)
     parsed_grammar.print()
 
     tokenizer = AutoTokenizer.from_pretrained("gpt2")
 
     tokenRecognizer = IncrementalTokenRecognizer(
-        grammar_str=input_text, start_rule_name="root", tokenizer=tokenizer
+        grammar_str=input_text,
+        start_rule_name="root",
+        tokenizer=tokenizer,
+        unicode=True,
     )
 
     japanese = "トリーム"  # "こんにちは"
     token_ids = tokenizer.encode(japanese)
     # 13298, 12675, 12045, 254
-    stacks = tokenRecognizer._consume_token_ids(
-        token_ids, tokenRecognizer.string_recognizer.stacks, as_string=False
-    )
+    init_state = None
+    state = tokenRecognizer._consume_token_ids(token_ids, init_state, as_string=False)
 
-    if stacks:
+    if state.stacks:
         print("The Japanese input is accepted")
     else:
         print("The Japanese input is not accepted")
 
     korean = "안녕하세요"
     token_ids = tokenizer.encode(korean)
+    init_state = tokenRecognizer.string_recognizer.get_initial_accept_state()
 
     try:
-        stacks = tokenRecognizer._consume_token_ids(
-            token_ids, tokenRecognizer.string_recognizer.stacks, as_string=False
+        state = tokenRecognizer._consume_token_ids(
+            token_ids,
+            init_state,
+            as_string=False,
         )
-        if stacks:
+        if state.stacks:
             print("The Korean input is accepted")
         else:
             print("The Korean input is not accepted")
     except ValueError as e:
         print("The Korean input is not accepted")
```

### Comparing `transformers_cfg-0.2.0/transformers_cfg/trie.py` & `transformers_cfg-0.2.1/transformers_cfg/tokenization/trie.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from functools import lru_cache
 from typing import Dict, List, Tuple
 from collections import deque
 
-from transformers_cfg.mapping import get_mapping
+from transformers_cfg.tokenization.mapping import get_mapping
 
 # from transformers_cfg.parser import parse_ebnf
 # from transformers_cfg.recognizer import GrammarRecognizer
 # from transformers_cfg.token_grammar_recognizer import IncrementalTokenGrammarRecognizer
 
 logger = logging.getLogger(__name__)
```

### Comparing `transformers_cfg-0.2.0/transformers_cfg/utf8_utils.py` & `transformers_cfg-0.2.1/transformers_cfg/utf8_utils.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/transformers_cfg/utils.py` & `transformers_cfg-0.2.1/transformers_cfg/utils.py`

 * *Files identical despite different names*

### Comparing `transformers_cfg-0.2.0/transformers_cfg/vocab_struct.py` & `transformers_cfg-0.2.1/transformers_cfg/tokenization/vocab_struct.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,18 @@
         return len(self.tokens)
 
     def load_tokens(self, tokenizer):
         def replace_hex(match):
             hex_value = match.group(1)
             return chr(int(hex_value, 16))
 
-        if "gpt2" in tokenizer.__class__.__name__.lower():
+        if (
+            "gpt2" in tokenizer.__class__.__name__.lower()
+            or "pretrained" in tokenizer.__class__.__name__.lower()
+        ):  # llama3 tokenizer
             special = tokenizer.additional_special_tokens_ids
 
             # Here, the decoder does a string replace on a bunch of sequences
             # like ' .' for '.'. This interferes with our assumptions, where a
             # token should always have exactly one representation.
             # Fortunately(?) text-generation-inference doesn't seem to run this
             # cleanup, so we get extraneous spaces. So, in order to generate
```

### Comparing `transformers_cfg-0.2.0/transformers_cfg.egg-info/PKG-INFO` & `transformers_cfg-0.2.1/transformers_cfg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,72 @@
 Metadata-Version: 2.1
 Name: transformers_cfg
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extension of Transformers library for Context-Free Grammar Constrained Decoding with EBNF grammars
 Home-page: https://github.com/epfl-dlab/transformers-CFG
 Author: EPFL-dlab
 Author-email: saibo.geng@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch~=2.2.0
-Requires-Dist: numpy~=1.24.2
-Requires-Dist: transformers~=4.37.2
-Requires-Dist: tokenizers~=0.15.2
-Requires-Dist: termcolor~=2.4.0
-Requires-Dist: sentencepiece~=0.1.99
-Requires-Dist: protobuf~=4.25.2
-Requires-Dist: setuptools~=69.0.3
+Requires-Dist: torch>=2.0.0
+Requires-Dist: numpy>=1.24.2
+Requires-Dist: transformers>=4.37.2
+Requires-Dist: tokenizers>=0.15.2
+Requires-Dist: termcolor>=2.4.0
+Requires-Dist: sentencepiece>=0.1.99
+Requires-Dist: protobuf>=4.25.2
+Requires-Dist: setuptools>=69.0.3
+Requires-Dist: line_profiler
 
 # 🤗 Transformers CFG
 
 ![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
-## Latest News
+## 💭Latest News
 
-**Support for Unicode(multilingual) grammars** (2024-02-29)
-**Integration with Text-Generation-WebUI** (2023-12-17)
+- **[Token masking optimization](#efficiency)(** (2024-04-25)
+
+- **Online [Demo with JSON Grammar](https://huggingface.co/spaces/saibo/transformers-CFG-JSON-demo) at HF space** (2024-04-10)
+
+- **Support for Unicode(multilingual) grammars** (2024-02-29)
+
+- **Integration with Text-Generation-WebUI** (2023-12-17)
 
 We are thrilled to announce that `transformers_cfg` has been used in the [Text-Generation-WebUI](https://github.com/oobabooga/text-generation-webui) project.
 This integration enables users to utilize our CFG capabilities within the popular, 30.5K-starred web interface for text generation.
 For more details, see [Relevent Pull Request](https://github.com/oobabooga/text-generation-webui/pull/4953)
 
 
-## Introduction
+## 🚀Introduction
 `transformers_cfg` is an extension library for the popular Transformers library by Hugging Face, tailored for working with context-free grammars (CFG).
 This package provides additional tools and functionalities to enhance your experience with natural language processing tasks involving CFGs.
 
 It was initially developed as a pull request to the [Hugging Face Transformers](https://github.com/huggingface/transformers) library.
 See relevant discussion [here](https://github.com/huggingface/transformers/pull/27557).
 
-## Installation
+## 💻 Installation
+
+- You can install the stable version of `transformers-cfg` using pip:
 
 ```bash
 pip install transformers-cfg
 ```
 
-## QuickStart: Force LLM to generate a valid json object
+- For the latest code and updates, you can install directly from the GitHub repository:
+
+```
+pip install git+https://github.com/epfl-dlab/transformers-CFG.git@main
+```
+This will install the package directly from the `main` branch of the repository.
+
+## 🔧QuickStart: Force LLM to generate a valid json object
 
 The below example can be found in `examples/generate_json.py`
 
 ```python
 import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from transformers_cfg.grammar_utils import IncrementalGrammarConstraint
@@ -98,22 +113,22 @@
     """
     'This is a valid json string for http request:{ "request": { "method": "GET", "headers": [], "content": "Content","type": "application" }}
     'This is a valid json string for shopping cart:{ "name": "MyCart", "price": 0, "value": 1 }
     """
 
 ```
 
-## Why should I use transformers-CFG?
+## 💡Why should I use transformers-CFG?
 
 - We support EBNF grammar description format
 - We offer the same grammar interface as llama-cpp project, allowing you to drop-in replace llama-cpp with transformers-CFG.
 - We allow you to use any of the models in the 🤗 Transformers library, including the ones that are not supported by llama-cpp.
 - We support multilingual grammars, you can use any character from any language in your grammar, e.g. 中文, 日本語, 한국어, हिन्दी, العربية, עברית, or emoji 🤗.
 
-## What is grammar ?
+## 🤔What is grammar ?
 
 TL;DR: Think of it as an enhanced version of regular expressions.
 
 Here is an example of a simplified JSON grammar:
 ```bnf
 # A JSON object is the root of the grammar
 root ::= object
@@ -175,14 +190,19 @@
 - ...
 
 See [supported_models.yaml](docs%2Fsupported_models.yaml) for the full list of supported models.
 
 As a rule of thumb, all models with the same tokenizer should naturally be supported.
 If you find any model that is not supported, please open an issue or submit a pull request.
 
+## Efficiency
+Our update in the `transformers_cfg` library has significantly improved the performance of grammar-constrained decoding (especially for complicated grammars).
+
+<img src="docs/assets/plots/benchmarking_results.png" style="width: 60%; height: auto;">
+
 ## Citation
 
 **Please consider citing our work, if you found the provided resources useful.**<br>
 ```
 @inproceedings{geng-etal-2023-grammar,
 	title        = {Grammar-Constrained Decoding for Structured {NLP} Tasks without Finetuning},
 	author       = {Geng, Saibo  and Josifoski, Martin  and Peyrard, Maxime  and West, Robert},
```

### Comparing `transformers_cfg-0.2.0/transformers_cfg.egg-info/SOURCES.txt` & `transformers_cfg-0.2.1/transformers_cfg.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,22 @@
 tests/json_utils.py
 tests/test_examples.py
 tests/test_grammar_constrained_decoding.py
 tests/test_mapping.py
 tests/test_parsing/__init__.py
 tests/test_parsing/test_parsing.py
 tests/test_string_recognizer/__init__.py
+tests/test_string_recognizer/test_calflow.py
 tests/test_string_recognizer/test_decode_utf8.py
+tests/test_string_recognizer/test_geo_query.py
 tests/test_string_recognizer/test_json.py
 tests/test_string_recognizer/test_json_arr.py
+tests/test_string_recognizer/test_overnight.py
+tests/test_string_recognizer/test_pddl.py
+tests/test_string_recognizer/test_smiles.py
 tests/test_string_recognizer/test_unicode.py
 tests/test_token_sequence_recognizer/__init__.py
 tests/test_token_sequence_recognizer/test_accept_unicode_bytes.py
 tests/test_tokenizers/__init__.py
 tests/test_tokenizers/test_bloom.py
 tests/test_tokenizers/test_codegen.py
 tests/test_tokenizers/test_falcon.py
@@ -24,22 +29,25 @@
 tests/test_tokenizers/test_gpt_neox.py
 tests/test_tokenizers/test_llama.py
 tests/test_tokenizers/test_t5.py
 tests/test_tokenizers/test_xglm.py
 transformers_cfg/__init__.py
 transformers_cfg/grammar_utils.py
 transformers_cfg/logging_config.py
-transformers_cfg/mapping.py
 transformers_cfg/parser.py
 transformers_cfg/recognizer.py
 transformers_cfg/token_grammar_recognizer.py
-transformers_cfg/trie.py
 transformers_cfg/utf8_utils.py
 transformers_cfg/utils.py
-transformers_cfg/vocab_struct.py
 transformers_cfg.egg-info/PKG-INFO
 transformers_cfg.egg-info/SOURCES.txt
 transformers_cfg.egg-info/dependency_links.txt
 transformers_cfg.egg-info/requires.txt
 transformers_cfg.egg-info/top_level.txt
 transformers_cfg/generation/__init__.py
-transformers_cfg/generation/logits_process.py
+transformers_cfg/generation/logits_process.py
+transformers_cfg/metrics/__init__.py
+transformers_cfg/metrics/metrics.py
+transformers_cfg/tokenization/__init__.py
+transformers_cfg/tokenization/mapping.py
+transformers_cfg/tokenization/trie.py
+transformers_cfg/tokenization/vocab_struct.py
```

