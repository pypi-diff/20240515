# Comparing `tmp/webscout-2.5.tar.gz` & `tmp/webscout-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-2.5.tar", last modified: Tue May 14 08:39:48 2024, max compression
+gzip compressed data, was "webscout-2.6.tar", last modified: Wed May 15 14:23:29 2024, max compression
```

## Comparing `webscout-2.5.tar` & `webscout-2.6.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.909575 webscout-2.5/
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.697906 webscout-2.5/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.705908 webscout-2.5/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.719944 webscout-2.5/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.726969 webscout-2.5/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.5/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.5/LICENSE.md
--rw-rw-rw-   0        0        0    46638 2024-05-14 08:39:48.905178 webscout-2.5/PKG-INFO
--rw-rw-rw-   0        0        0    44186 2024-05-14 08:07:30.000000 webscout-2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 08:39:48.910590 webscout-2.5/setup.cfg
--rw-rw-rw-   0        0        0     2723 2024-05-14 08:39:26.000000 webscout-2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.791739 webscout-2.5/webscout/
--rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.5/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.5/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.5/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.5/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.5/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.841233 webscout-2.5/webscout/Local/
--rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-2.5/webscout/Local/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-13 10:17:01.000000 webscout-2.5/webscout/Local/_version.py
--rw-rw-rw-   0        0        0    17153 2024-05-13 10:22:12.000000 webscout-2.5/webscout/Local/formats.py
--rw-rw-rw-   0        0        0    27611 2024-05-13 10:21:04.000000 webscout-2.5/webscout/Local/model.py
--rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.5/webscout/Local/samplers.py
--rw-rw-rw-   0        0        0    26786 2024-05-14 05:00:48.000000 webscout-2.5/webscout/Local/thread.py
--rw-rw-rw-   0        0        0     6108 2024-05-14 05:14:09.000000 webscout-2.5/webscout/Local/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.898175 webscout-2.5/webscout/Provider/
--rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.5/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.5/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.5/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.5/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.5/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.5/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.5/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.5/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.5/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.5/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.5/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.5/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.5/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.5/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.5/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.5/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.5/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.5/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1318 2024-05-13 09:09:36.000000 webscout-2.5/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     2214 2024-05-14 03:52:34.000000 webscout-2.5/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.5/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.5/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.5/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.5/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.5/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.5/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.5/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.5/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.5/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.5/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.5/webscout/voice.py
--rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.5/webscout/webai.py
--rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.5/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.5/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:39:48.901179 webscout-2.5/webscout.egg-info/
--rw-rw-rw-   0        0        0    46638 2024-05-14 08:39:48.000000 webscout-2.5/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1772 2024-05-14 08:39:48.000000 webscout-2.5/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:39:48.000000 webscout-2.5/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-14 08:39:48.000000 webscout-2.5/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      379 2024-05-14 08:39:48.000000 webscout-2.5/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-14 08:39:48.000000 webscout-2.5/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:29.309273 webscout-2.6/
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:27.529805 webscout-2.6/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:27.580652 webscout-2.6/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:27.660368 webscout-2.6/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:27.682370 webscout-2.6/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.6/LICENSE.md
+-rw-rw-rw-   0        0        0    47429 2024-05-15 14:23:29.279272 webscout-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    44977 2024-05-14 14:17:49.000000 webscout-2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:23:29.309273 webscout-2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2723 2024-05-15 14:22:40.000000 webscout-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:28.112112 webscout-2.6/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.6/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.6/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33256 2024-05-14 14:10:47.000000 webscout-2.6/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.6/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.6/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:28.352353 webscout-2.6/webscout/Local/
+-rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-2.6/webscout/Local/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-14 08:49:56.000000 webscout-2.6/webscout/Local/_version.py
+-rw-rw-rw-   0        0        0    16644 2024-05-15 04:24:04.000000 webscout-2.6/webscout/Local/formats.py
+-rw-rw-rw-   0        0        0    27611 2024-05-13 10:21:04.000000 webscout-2.6/webscout/Local/model.py
+-rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.6/webscout/Local/samplers.py
+-rw-rw-rw-   0        0        0    26788 2024-05-14 08:49:17.000000 webscout-2.6/webscout/Local/thread.py
+-rw-rw-rw-   0        0        0     6108 2024-05-14 05:14:09.000000 webscout-2.6/webscout/Local/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:29.248271 webscout-2.6/webscout/Provider/
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.6/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.6/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.6/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.6/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.6/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.6/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.6/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.6/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.6/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.6/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.6/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.6/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.6/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     7303 2024-05-14 14:08:46.000000 webscout-2.6/webscout/Provider/Poe.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.6/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.6/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.6/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.6/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.6/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1348 2024-05-14 14:09:14.000000 webscout-2.6/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     1836 2024-05-14 14:10:37.000000 webscout-2.6/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.6/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.6/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.6/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.6/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.6/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.6/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.6/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.6/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.6/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.6/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.6/webscout/voice.py
+-rw-rw-rw-   0        0        0    85324 2024-05-14 14:12:32.000000 webscout-2.6/webscout/webai.py
+-rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.6/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.6/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:29.261275 webscout-2.6/webscout.egg-info/
+-rw-rw-rw-   0        0        0    47429 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1797 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      379 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/top_level.txt
```

### Comparing `webscout-2.5/DeepWEBS/documents/query_results_extractor.py` & `webscout-2.6/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-2.6/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/DeepWEBS/networks/filepath_converter.py` & `webscout-2.6/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/DeepWEBS/networks/google_searcher.py` & `webscout-2.6/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/DeepWEBS/networks/network_configs.py` & `webscout-2.6/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/DeepWEBS/networks/webpage_fetcher.py` & `webscout-2.6/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/DeepWEBS/utilsdw/enver.py` & `webscout-2.6/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/DeepWEBS/utilsdw/logger.py` & `webscout-2.6/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/LICENSE.md` & `webscout-2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-2.5/PKG-INFO` & `webscout-2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.5
+Version: 2.6
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -131,14 +131,15 @@
     - [9. `KOBOLDAI` -](#9-koboldai--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
     - [`LLM`](#llm)
+    - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -1221,14 +1222,34 @@
 
     # Use the mistral_chat method to get the response
     response = llm.chat(messages)
 
     # Print the response
     print("AI: ", response)
 ```
+### `Local-LLM` webscout can now run GGUF models
+```python
+from webscout.Local.utils import download_model
+from webscout.Local.model import Model
+from webscout.Local.thread import Thread
+from webscout.Local import formats
+# 1. Download the model
+repo_id = "microsoft/Phi-3-mini-4k-instruct-gguf"  # Replace with the desired Hugging Face repo
+filename = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+model_path = download_model(repo_id, filename)
+
+# 2. Load the model 
+model = Model(model_path, n_gpu_layers=4)  
+
+# 3. Create a Thread for conversation
+thread = Thread(model, formats.phi3)
+
+# 4. Start interacting with the model
+thread.interact()
+```
 ### `LLM` with internet
 ```python
 from __future__ import annotations
 from typing import List, Optional
 
 from webscout.LLM import LLM
 from webscout import WEBS
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.5 Summary: Search for anything
+Metadata-Version: 2.1 Name: webscout Version: 2.6 Summary: Search for anything
 using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
 videos, temporary email and phone number generation, has TTS support, webai
 (terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -70,71 +70,72 @@
   With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
 Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
  - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-
  koboldai--) - [10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11.
   `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) - [12. `Xjai` -
  chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13. `ThinkAny` -
  AI search engine](#13-thinkany---ai-search-engine) - [14. `chatgptuk` - Chat
-with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) - [`LLM`
-with internet](#llm-with-internet) - [LLM with deepwebs](#llm-with-deepwebs) -
-  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
-   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
-version ```python3 python -m webscout --help ``` | Command | Description | |---
-----------------------------------------|--------------------------------------
- -----------------------------------------------------------------| | python -
- m webscout answers -k Text | CLI function to perform an answers search using
- Webscout. | | python -m webscout images -k Text | CLI function to perform an
-    images search using Webscout. | | python -m webscout maps -k Text | CLI
-function to perform a maps search using Webscout. | | python -m webscout news -
-  k Text | CLI function to perform a news search using Webscout. | | python -
- m webscout suggestions -k Text | CLI function to perform a suggestions search
-using Webscout. | | python -m webscout text -k Text | CLI function to perform a
-  text search using Webscout. | | python -m webscout translate -k Text | CLI
-function to perform translate using Webscout. | | python -m webscout version |
-  A command-line interface command that prints and returns the version of the
-  program. | | python -m webscout videos -k Text | CLI function to perform a
-videos search using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar
-for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de
-for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-
-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es
-for Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
- Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
-### Temp number ```python from rich.console import Console from webscout import
- tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
-try: # Get a temporary phone number for a specific country (or random) number =
-   phone.get_number(country="Finland") console.print(f"Your temporary phone
- number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
-   with your actual logic) # import time module import time time.sleep(30) #
-  Adjust the waiting time as needed # Retrieve and print messages messages =
-  phone.get_messages(number) if messages: # Access individual messages using
-     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
-    [0].content}") # (Add more lines if you expect multiple messages) else:
-console.print("No messages received.") except Exception as e: console.print(f"
- [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
-    Tempmail ```python import asyncio from rich.console import Console from
-rich.table import Table from rich.text import Text from webscout import tempid
-  async def main() -> None: console = Console() client = tempid.Client() try:
-   domains = await client.get_domains() if not domains: console.print("[bold
-   red]No domains available. Please try again later.") return email = await
-  client.create_email(domain=domains[0].name) console.print(f"Your temporary
-    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
-    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+   with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) -
+[`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-
+gguf-models) - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs]
+(#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---
+    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
+   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
+ ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
+au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
+(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
+ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
+Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
+  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
+Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
+ (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
+ for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
+for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
+en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
+for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
+ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
+za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
+ (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
+th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
+us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
+  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
+number ### Temp number ```python from rich.console import Console from webscout
+             import tempid def main(): console = Console() phone =
+    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
+   specific country (or random) number = phone.get_number(country="Finland")
+console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
+# Pause execution briefly (replace with your actual logic) # import time module
+ import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
+  print messages messages = phone.get_messages(number) if messages: # Access
+   individual messages using indexing: console.print(f"[bold green]{messages
+ [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
+ messages) else: console.print("No messages received.") except Exception as e:
+ console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
+   main() ``` ### Tempmail ```python import asyncio from rich.console import
+ Console from rich.table import Table from rich.text import Text from webscout
+     import tempid async def main() -> None: console = Console() client =
+   tempid.Client() try: domains = await client.get_domains() if not domains:
+console.print("[bold red]No domains available. Please try again later.") return
+email = await client.create_email(domain=domains[0].name) console.print(f"Your
+ temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
+  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
   messages = await client.get_messages(email.email) if messages is not None:
 break if messages: table = Table(show_header=True, header_style="bold magenta")
     table.add_column("From", style="bold cyan") table.add_column("Subject",
  style="bold yellow") table.add_column("Body", style="bold green") for message
  in messages: body_preview = Text(message.body_text if message.body_text else
  "No body") table.add_row(message.email_from or "Unknown", message.subject or
    "No Subject", body_preview) console.print(table) else: console.print("No
@@ -414,17 +415,26 @@
       system message from the file with open('system.txt', 'r') as file:
 system_message = file.read() # Initialize the LLM class with the model name and
          system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
  system_message=system_message) while True: # Get the user input user_input =
 input("User: ") # Define the messages to be sent messages = [ {"role": "user",
   "content": user_input} ] # Use the mistral_chat method to get the response
 response = llm.chat(messages) # Print the response print("AI: ", response) ```
-   ### `LLM` with internet ```python from __future__ import annotations from
-typing import List, Optional from webscout.LLM import LLM from webscout import
- WEBS import warnings system_message: str = ( "As an AI assistant, I have been
+        ### `Local-LLM` webscout can now run GGUF models ```python from
+  webscout.Local.utils import download_model from webscout.Local.model import
+   Model from webscout.Local.thread import Thread from webscout.Local import
+ formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-instruct-
+ gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-mini-4k-
+      instruct-q4.gguf" # Replace with the correct filename model_path =
+download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
+ n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
+ formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
+ `LLM` with internet ```python from __future__ import annotations from typing
+ import List, Optional from webscout.LLM import LLM from webscout import WEBS
+   import warnings system_message: str = ( "As an AI assistant, I have been
    designed with advanced capabilities, including real-time access to online
   resources. This enables me to enrich our conversations and provide you with
 informed and accurate responses, drawing from a vast array of information. With
  each interaction, my goal is to create a seamless and meaningful connection,
  offering insights and sharing relevant content." "My directives emphasize the
  importance of respect, impartiality, and intellectual integrity. I am here to
 provide unbiased responses, ensuring an ethical and respectful exchange. I will
```

### Comparing `webscout-2.5/README.md` & `webscout-2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     - [9. `KOBOLDAI` -](#9-koboldai--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
     - [`LLM`](#llm)
+    - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -1159,14 +1160,34 @@
 
     # Use the mistral_chat method to get the response
     response = llm.chat(messages)
 
     # Print the response
     print("AI: ", response)
 ```
+### `Local-LLM` webscout can now run GGUF models
+```python
+from webscout.Local.utils import download_model
+from webscout.Local.model import Model
+from webscout.Local.thread import Thread
+from webscout.Local import formats
+# 1. Download the model
+repo_id = "microsoft/Phi-3-mini-4k-instruct-gguf"  # Replace with the desired Hugging Face repo
+filename = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+model_path = download_model(repo_id, filename)
+
+# 2. Load the model 
+model = Model(model_path, n_gpu_layers=4)  
+
+# 3. Create a Thread for conversation
+thread = Thread(model, formats.phi3)
+
+# 4. Start interacting with the model
+thread.interact()
+```
 ### `LLM` with internet
 ```python
 from __future__ import annotations
 from typing import List, Optional
 
 from webscout.LLM import LLM
 from webscout import WEBS
```

#### html2text {}

```diff
@@ -38,71 +38,72 @@
   With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
 Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
  - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-
  koboldai--) - [10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11.
   `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) - [12. `Xjai` -
  chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13. `ThinkAny` -
  AI search engine](#13-thinkany---ai-search-engine) - [14. `chatgptuk` - Chat
-with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) - [`LLM`
-with internet](#llm-with-internet) - [LLM with deepwebs](#llm-with-deepwebs) -
-  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
-   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
-version ```python3 python -m webscout --help ``` | Command | Description | |---
-----------------------------------------|--------------------------------------
- -----------------------------------------------------------------| | python -
- m webscout answers -k Text | CLI function to perform an answers search using
- Webscout. | | python -m webscout images -k Text | CLI function to perform an
-    images search using Webscout. | | python -m webscout maps -k Text | CLI
-function to perform a maps search using Webscout. | | python -m webscout news -
-  k Text | CLI function to perform a news search using Webscout. | | python -
- m webscout suggestions -k Text | CLI function to perform a suggestions search
-using Webscout. | | python -m webscout text -k Text | CLI function to perform a
-  text search using Webscout. | | python -m webscout translate -k Text | CLI
-function to perform translate using Webscout. | | python -m webscout version |
-  A command-line interface command that prints and returns the version of the
-  program. | | python -m webscout videos -k Text | CLI function to perform a
-videos search using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar
-for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de
-for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-
-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es
-for Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
- Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
-### Temp number ```python from rich.console import Console from webscout import
- tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
-try: # Get a temporary phone number for a specific country (or random) number =
-   phone.get_number(country="Finland") console.print(f"Your temporary phone
- number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
-   with your actual logic) # import time module import time time.sleep(30) #
-  Adjust the waiting time as needed # Retrieve and print messages messages =
-  phone.get_messages(number) if messages: # Access individual messages using
-     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
-    [0].content}") # (Add more lines if you expect multiple messages) else:
-console.print("No messages received.") except Exception as e: console.print(f"
- [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
-    Tempmail ```python import asyncio from rich.console import Console from
-rich.table import Table from rich.text import Text from webscout import tempid
-  async def main() -> None: console = Console() client = tempid.Client() try:
-   domains = await client.get_domains() if not domains: console.print("[bold
-   red]No domains available. Please try again later.") return email = await
-  client.create_email(domain=domains[0].name) console.print(f"Your temporary
-    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
-    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+   with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) -
+[`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-
+gguf-models) - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs]
+(#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---
+    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
+   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
+ ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
+au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
+(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
+ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
+Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
+  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
+Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
+ (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
+ for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
+for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
+en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
+for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
+ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
+za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
+ (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
+th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
+us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
+  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
+number ### Temp number ```python from rich.console import Console from webscout
+             import tempid def main(): console = Console() phone =
+    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
+   specific country (or random) number = phone.get_number(country="Finland")
+console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
+# Pause execution briefly (replace with your actual logic) # import time module
+ import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
+  print messages messages = phone.get_messages(number) if messages: # Access
+   individual messages using indexing: console.print(f"[bold green]{messages
+ [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
+ messages) else: console.print("No messages received.") except Exception as e:
+ console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
+   main() ``` ### Tempmail ```python import asyncio from rich.console import
+ Console from rich.table import Table from rich.text import Text from webscout
+     import tempid async def main() -> None: console = Console() client =
+   tempid.Client() try: domains = await client.get_domains() if not domains:
+console.print("[bold red]No domains available. Please try again later.") return
+email = await client.create_email(domain=domains[0].name) console.print(f"Your
+ temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
+  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
   messages = await client.get_messages(email.email) if messages is not None:
 break if messages: table = Table(show_header=True, header_style="bold magenta")
     table.add_column("From", style="bold cyan") table.add_column("Subject",
  style="bold yellow") table.add_column("Body", style="bold green") for message
  in messages: body_preview = Text(message.body_text if message.body_text else
  "No body") table.add_row(message.email_from or "Unknown", message.subject or
    "No Subject", body_preview) console.print(table) else: console.print("No
@@ -382,17 +383,26 @@
       system message from the file with open('system.txt', 'r') as file:
 system_message = file.read() # Initialize the LLM class with the model name and
          system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
  system_message=system_message) while True: # Get the user input user_input =
 input("User: ") # Define the messages to be sent messages = [ {"role": "user",
   "content": user_input} ] # Use the mistral_chat method to get the response
 response = llm.chat(messages) # Print the response print("AI: ", response) ```
-   ### `LLM` with internet ```python from __future__ import annotations from
-typing import List, Optional from webscout.LLM import LLM from webscout import
- WEBS import warnings system_message: str = ( "As an AI assistant, I have been
+        ### `Local-LLM` webscout can now run GGUF models ```python from
+  webscout.Local.utils import download_model from webscout.Local.model import
+   Model from webscout.Local.thread import Thread from webscout.Local import
+ formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-instruct-
+ gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-mini-4k-
+      instruct-q4.gguf" # Replace with the correct filename model_path =
+download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
+ n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
+ formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
+ `LLM` with internet ```python from __future__ import annotations from typing
+ import List, Optional from webscout.LLM import LLM from webscout import WEBS
+   import warnings system_message: str = ( "As an AI assistant, I have been
    designed with advanced capabilities, including real-time access to online
   resources. This enables me to enrich our conversations and provide you with
 informed and accurate responses, drawing from a vast array of information. With
  each interaction, my goal is to create a seamless and meaningful connection,
  offering insights and sharing relevant content." "My directives emphasize the
  importance of respect, impartiality, and intellectual integrity. I am here to
 provide unbiased responses, ensuring an ethical and respectful exchange. I will
```

### Comparing `webscout-2.5/setup.py` & `webscout-2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="2.5",
+    version="2.6",
     description="Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-2.5/webscout/AIauto.py` & `webscout-2.6/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/AIbase.py` & `webscout-2.6/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/AIutel.py` & `webscout-2.6/webscout/AIutel.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,35 +22,35 @@
 appdir = appdirs.AppDirs("AIWEBS", "vortex")
 
 default_path = appdir.user_cache_dir
 
 if not os.path.exists(default_path):
     os.makedirs(default_path)
 webai = [
-    "leo",
-    "openai",
-    "opengpt",
-    "koboldai",
-    "gemini",
-    "phind",
-    "blackboxai",
-    "g4fauto",
-    "perplexity",
-    "groq",
-    "reka",
-    "cohere",
-    "yepchat",
-    "you",
-    "xjai",
-    "thinkany",
-    "berlin4h",
-    "chatgptuk",
-    "auto",
+   "leo",
+   "openai",
+   "opengpt",
+   "koboldai",
+   "gemini",
+   "phind",
+   "blackboxai",
+   "g4fauto",
+   "perplexity",
+   "groq",
+   "reka",
+   "cohere",
+   "yepchat",
+   "you",
+   "xjai",
+   "thinkany",
+   "berlin4h",
+   "chatgptuk",
+   "auto",
+   "poe",
 ]
-
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
 def sanitize_stream(
     chunk: str, intro_value: str = "data:", to_json: bool = True
```

### Comparing `webscout-2.5/webscout/DWEBS.py` & `webscout-2.6/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/LLM.py` & `webscout-2.6/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Local/formats.py` & `webscout-2.6/webscout/Local/formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,27 +41,14 @@
     "user_content": "",
     "user_postfix": "\n\n",
     "bot_prefix": "### Response:\n",
     "bot_content": "",
     "bot_postfix": "\n\n",
     "stops": ['###', 'Instruction:', '\n\n\n']
 }
-
-# https://docs.mistral.ai/models/
-# As a reference, here is the format used to tokenize instructions during fine-tuning:
-# ```
-# [START_SYMBOL_ID] + 
-# tok("[INST]") + tok(USER_MESSAGE_1) + tok("[/INST]") +
-# tok(BOT_MESSAGE_1) + [END_SYMBOL_ID] +
-# …
-# tok("[INST]") + tok(USER_MESSAGE_N) + tok("[/INST]") +
-# tok(BOT_MESSAGE_N) + [END_SYMBOL_ID]
-# ```
-# In the pseudo-code above, note that the tokenize method should not add a BOS or EOS token automatically, but should add a prefix space.
-
 mistral_instruct: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
     "system_postfix": "",
     "user_prefix": " [INST] ",
     "user_content": "",
     "user_postfix": " [/INST]",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `webscout-2.5/webscout/Local/model.py` & `webscout-2.6/webscout/Local/model.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Local/samplers.py` & `webscout-2.6/webscout/Local/samplers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Local/thread.py` & `webscout-2.6/webscout/Local/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
             SPECIAL_STYLE = ''
         
         if header is not None:
             print(f"{SPECIAL_STYLE}{header}{RESET_ALL}\n")
         
         while True:
 
-            prompt = f"{RESET_ALL}  > {USER_STYLE}"
+            prompt = f"{RESET_ALL}  >>> {USER_STYLE}"
             
             try:
                 user_prompt, next_message_start = self._interactive_input(
                     prompt,
                     DIM_STYLE,
                     USER_STYLE,
                     BOT_STYLE
```

### Comparing `webscout-2.5/webscout/Local/utils.py` & `webscout-2.6/webscout/Local/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Berlin4h.py` & `webscout-2.6/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Blackboxai.py` & `webscout-2.6/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/ChatGPTUK.py` & `webscout-2.6/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Cohere.py` & `webscout-2.6/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Gemini.py` & `webscout-2.6/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Groq.py` & `webscout-2.6/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Koboldai.py` & `webscout-2.6/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Leo.py` & `webscout-2.6/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Llama2.py` & `webscout-2.6/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/OpenGPT.py` & `webscout-2.6/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Openai.py` & `webscout-2.6/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Perplexity.py` & `webscout-2.6/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Phind.py` & `webscout-2.6/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Reka.py` & `webscout-2.6/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/ThinkAnyAI.py` & `webscout-2.6/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Xjai.py` & `webscout-2.6/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Yepchat.py` & `webscout-2.6/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/Youchat.py` & `webscout-2.6/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/Provider/__init__.py` & `webscout-2.6/webscout/Provider/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .Phind import AsyncPhindSearch
 from .Yepchat import YEPCHAT
 from .Yepchat import AsyncYEPCHAT
 from .Youchat import YouChat
 from .Gemini import GEMINI
 from .Berlin4h import Berlin4h
 from .ChatGPTUK import ChatGPTUK
-
+from .Poe import POE
 __all__ = [
     'ThinkAnyAI',
     'Xjai',
     'LLAMA2', 
     'AsyncLLAMA2',
     'Cohere',
     'REKA',
@@ -52,8 +52,9 @@
     'AsyncPhindSearch',
     'YEPCHAT',
     'AsyncYEPCHAT',
     'YouChat',
     'GEMINI',
     'Berlin4h',
     'ChatGPTUK',
+    'POE'
 ]
```

### Comparing `webscout-2.5/webscout/__init__.py` & `webscout-2.6/webscout/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,15 @@
 from .transcriber import transcriber
 from .voice import play_audio
 from .tempid import Client as TempMailClient, TemporaryPhoneNumber
 from .LLM import LLM
 # from .Local import *
 import g4f
 # Import provider classes for direct access
-from .Provider import (
-   ThinkAnyAI,
-   Xjai,
-   LLAMA2, 
-   AsyncLLAMA2,
-   Cohere,
-   REKA,
-   GROQ,
-   AsyncGROQ,
-   OPENAI,
-   AsyncOPENAI,
-   LEO,
-   AsyncLEO,
-   KOBOLDAI,
-   AsyncKOBOLDAI,
-   OPENGPT,
-   AsyncOPENGPT,
-   PERPLEXITY,
-   BLACKBOXAI,
-   AsyncBLACKBOXAI,
-   PhindSearch,
-   AsyncPhindSearch,
-   YEPCHAT,
-   AsyncYEPCHAT,
-   YouChat,
-   GEMINI,
-   Berlin4h,
-   ChatGPTUK,
-)
+from .Provider import *
 
 __repo__ = "https://github.com/OE-LUCIFER/Webscout"
 
 webai = [
    "leo",
    "openai",
    "opengpt",
@@ -57,14 +29,15 @@
    "yepchat",
    "you",
    "xjai",
    "thinkany",
    "berlin4h",
    "chatgptuk",
    "auto",
+   "poe",
 ]
 
 gpt4free_providers = [
    provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
@@ -109,11 +82,12 @@
    "AsyncPhindSearch",
    "YEPCHAT",
    "AsyncYEPCHAT",
    "YouChat",
    "GEMINI",
    "Berlin4h",
    "ChatGPTUK",
+   "POE"
 ]
 
 import logging
 logging.getLogger("webscout").addHandler(logging.NullHandler())
```

### Comparing `webscout-2.5/webscout/async_providers.py` & `webscout-2.6/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/cli.py` & `webscout-2.6/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/g4f.py` & `webscout-2.6/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/models.py` & `webscout-2.6/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/tempid.py` & `webscout-2.6/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/transcriber.py` & `webscout-2.6/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/utils.py` & `webscout-2.6/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/voice.py` & `webscout-2.6/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/webai.py` & `webscout-2.6/webscout/webai.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,15 +409,31 @@
                         act=awesome_prompt,
                     )
                 else:
                     raise Exception(
                         "No working g4f provider found. "
                         "Consider running 'webscout gpt4free test -y' first"
                     )
+            elif provider == "poe":
+                assert auth, (
+                    "Path to poe.com.cookies.json file or 'p-b' cookie-value is required. "
+                    "Use the flag `--key` or `-k`"
+                )
+                from webscout import POE
 
+                self.bot = POE(
+                    cookie=auth,
+                    model=getOr(model, "Assistant"),
+                    proxy=bool(proxies),
+                    timeout=timeout,
+                    filepath=filepath,
+                    update_file=update_file,
+                    intro=intro,
+                    act=awesome_prompt,
+                )
             elif provider == "leo":
                 from webscout import LEO
 
                 self.bot = LEO(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
```

### Comparing `webscout-2.5/webscout/webscout_search.py` & `webscout-2.6/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout/webscout_search_async.py` & `webscout-2.6/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-2.5/webscout.egg-info/PKG-INFO` & `webscout-2.6/webscout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.5
+Version: 2.6
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -131,14 +131,15 @@
     - [9. `KOBOLDAI` -](#9-koboldai--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
     - [`LLM`](#llm)
+    - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -1221,14 +1222,34 @@
 
     # Use the mistral_chat method to get the response
     response = llm.chat(messages)
 
     # Print the response
     print("AI: ", response)
 ```
+### `Local-LLM` webscout can now run GGUF models
+```python
+from webscout.Local.utils import download_model
+from webscout.Local.model import Model
+from webscout.Local.thread import Thread
+from webscout.Local import formats
+# 1. Download the model
+repo_id = "microsoft/Phi-3-mini-4k-instruct-gguf"  # Replace with the desired Hugging Face repo
+filename = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+model_path = download_model(repo_id, filename)
+
+# 2. Load the model 
+model = Model(model_path, n_gpu_layers=4)  
+
+# 3. Create a Thread for conversation
+thread = Thread(model, formats.phi3)
+
+# 4. Start interacting with the model
+thread.interact()
+```
 ### `LLM` with internet
 ```python
 from __future__ import annotations
 from typing import List, Optional
 
 from webscout.LLM import LLM
 from webscout import WEBS
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.5 Summary: Search for anything
+Metadata-Version: 2.1 Name: webscout Version: 2.6 Summary: Search for anything
 using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
 videos, temporary email and phone number generation, has TTS support, webai
 (terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -70,71 +70,72 @@
   With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
 Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
  - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-
  koboldai--) - [10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11.
   `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) - [12. `Xjai` -
  chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13. `ThinkAny` -
  AI search engine](#13-thinkany---ai-search-engine) - [14. `chatgptuk` - Chat
-with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) - [`LLM`
-with internet](#llm-with-internet) - [LLM with deepwebs](#llm-with-deepwebs) -
-  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
-   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
-version ```python3 python -m webscout --help ``` | Command | Description | |---
-----------------------------------------|--------------------------------------
- -----------------------------------------------------------------| | python -
- m webscout answers -k Text | CLI function to perform an answers search using
- Webscout. | | python -m webscout images -k Text | CLI function to perform an
-    images search using Webscout. | | python -m webscout maps -k Text | CLI
-function to perform a maps search using Webscout. | | python -m webscout news -
-  k Text | CLI function to perform a news search using Webscout. | | python -
- m webscout suggestions -k Text | CLI function to perform a suggestions search
-using Webscout. | | python -m webscout text -k Text | CLI function to perform a
-  text search using Webscout. | | python -m webscout translate -k Text | CLI
-function to perform translate using Webscout. | | python -m webscout version |
-  A command-line interface command that prints and returns the version of the
-  program. | | python -m webscout videos -k Text | CLI function to perform a
-videos search using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar
-for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de
-for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-
-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es
-for Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
- Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
-### Temp number ```python from rich.console import Console from webscout import
- tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
-try: # Get a temporary phone number for a specific country (or random) number =
-   phone.get_number(country="Finland") console.print(f"Your temporary phone
- number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
-   with your actual logic) # import time module import time time.sleep(30) #
-  Adjust the waiting time as needed # Retrieve and print messages messages =
-  phone.get_messages(number) if messages: # Access individual messages using
-     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
-    [0].content}") # (Add more lines if you expect multiple messages) else:
-console.print("No messages received.") except Exception as e: console.print(f"
- [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
-    Tempmail ```python import asyncio from rich.console import Console from
-rich.table import Table from rich.text import Text from webscout import tempid
-  async def main() -> None: console = Console() client = tempid.Client() try:
-   domains = await client.get_domains() if not domains: console.print("[bold
-   red]No domains available. Please try again later.") return email = await
-  client.create_email(domain=domains[0].name) console.print(f"Your temporary
-    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
-    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+   with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) -
+[`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-
+gguf-models) - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs]
+(#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---
+    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
+   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
+ ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
+au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
+(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
+ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
+Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
+  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
+Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
+ (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
+ for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
+for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
+en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
+for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
+ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
+za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
+ (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
+th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
+us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
+  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
+number ### Temp number ```python from rich.console import Console from webscout
+             import tempid def main(): console = Console() phone =
+    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
+   specific country (or random) number = phone.get_number(country="Finland")
+console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
+# Pause execution briefly (replace with your actual logic) # import time module
+ import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
+  print messages messages = phone.get_messages(number) if messages: # Access
+   individual messages using indexing: console.print(f"[bold green]{messages
+ [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
+ messages) else: console.print("No messages received.") except Exception as e:
+ console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
+   main() ``` ### Tempmail ```python import asyncio from rich.console import
+ Console from rich.table import Table from rich.text import Text from webscout
+     import tempid async def main() -> None: console = Console() client =
+   tempid.Client() try: domains = await client.get_domains() if not domains:
+console.print("[bold red]No domains available. Please try again later.") return
+email = await client.create_email(domain=domains[0].name) console.print(f"Your
+ temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
+  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
   messages = await client.get_messages(email.email) if messages is not None:
 break if messages: table = Table(show_header=True, header_style="bold magenta")
     table.add_column("From", style="bold cyan") table.add_column("Subject",
  style="bold yellow") table.add_column("Body", style="bold green") for message
  in messages: body_preview = Text(message.body_text if message.body_text else
  "No body") table.add_row(message.email_from or "Unknown", message.subject or
    "No Subject", body_preview) console.print(table) else: console.print("No
@@ -414,17 +415,26 @@
       system message from the file with open('system.txt', 'r') as file:
 system_message = file.read() # Initialize the LLM class with the model name and
          system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
  system_message=system_message) while True: # Get the user input user_input =
 input("User: ") # Define the messages to be sent messages = [ {"role": "user",
   "content": user_input} ] # Use the mistral_chat method to get the response
 response = llm.chat(messages) # Print the response print("AI: ", response) ```
-   ### `LLM` with internet ```python from __future__ import annotations from
-typing import List, Optional from webscout.LLM import LLM from webscout import
- WEBS import warnings system_message: str = ( "As an AI assistant, I have been
+        ### `Local-LLM` webscout can now run GGUF models ```python from
+  webscout.Local.utils import download_model from webscout.Local.model import
+   Model from webscout.Local.thread import Thread from webscout.Local import
+ formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-instruct-
+ gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-mini-4k-
+      instruct-q4.gguf" # Replace with the correct filename model_path =
+download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
+ n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
+ formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
+ `LLM` with internet ```python from __future__ import annotations from typing
+ import List, Optional from webscout.LLM import LLM from webscout import WEBS
+   import warnings system_message: str = ( "As an AI assistant, I have been
    designed with advanced capabilities, including real-time access to online
   resources. This enables me to enrich our conversations and provide you with
 informed and accurate responses, drawing from a vast array of information. With
  each interaction, my goal is to create a seamless and meaningful connection,
  offering insights and sharing relevant content." "My directives emphasize the
  importance of respect, impartiality, and intellectual integrity. I am here to
 provide unbiased responses, ensuring an ethical and respectful exchange. I will
```

### Comparing `webscout-2.5/webscout.egg-info/SOURCES.txt` & `webscout-2.6/webscout.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,13 +55,14 @@
 webscout/Provider/Koboldai.py
 webscout/Provider/Leo.py
 webscout/Provider/Llama2.py
 webscout/Provider/OpenGPT.py
 webscout/Provider/Openai.py
 webscout/Provider/Perplexity.py
 webscout/Provider/Phind.py
+webscout/Provider/Poe.py
 webscout/Provider/Reka.py
 webscout/Provider/ThinkAnyAI.py
 webscout/Provider/Xjai.py
 webscout/Provider/Yepchat.py
 webscout/Provider/Youchat.py
 webscout/Provider/__init__.py
```

