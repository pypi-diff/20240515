# Comparing `tmp/latentscope-0.2.2.tar.gz` & `tmp/latentscope-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latentscope-0.2.2.tar", last modified: Mon May 13 13:33:24 2024, max compression
+gzip compressed data, was "latentscope-0.2.3.tar", last modified: Wed May 15 13:49:49 2024, max compression
```

## Comparing `latentscope-0.2.2.tar` & `latentscope-0.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.076438 latentscope-0.2.2/
--rw-r--r--   0 enjalot    (501) staff       (20)     1068 2024-02-16 15:11:38.000000 latentscope-0.2.2/LICENSE
--rw-r--r--   0 enjalot    (501) staff       (20)    18782 2024-05-13 13:33:24.076208 latentscope-0.2.2/PKG-INFO
--rw-r--r--   0 enjalot    (501) staff       (20)    12878 2024-05-13 13:19:12.000000 latentscope-0.2.2/README.md
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.068332 latentscope-0.2.2/latentscope/
--rw-r--r--   0 enjalot    (501) staff       (20)     2032 2024-04-25 14:11:19.000000 latentscope-0.2.2/latentscope/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)       22 2024-05-13 13:33:08.000000 latentscope-0.2.2/latentscope/__version__.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.069414 latentscope-0.2.2/latentscope/models/
--rw-r--r--   0 enjalot    (501) staff       (20)     2993 2024-03-19 19:02:11.000000 latentscope-0.2.2/latentscope/models/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1792 2024-03-19 18:27:46.000000 latentscope-0.2.2/latentscope/models/chat_models.json
--rw-r--r--   0 enjalot    (501) staff       (20)     6432 2024-03-18 16:42:28.000000 latentscope-0.2.2/latentscope/models/embedding_models.json
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.070438 latentscope-0.2.2/latentscope/models/providers/
--rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-12 13:46:58.000000 latentscope-0.2.2/latentscope/models/providers/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)      694 2024-01-25 14:33:56.000000 latentscope-0.2.2/latentscope/models/providers/base.py
--rw-r--r--   0 enjalot    (501) staff       (20)      705 2024-03-19 18:57:45.000000 latentscope-0.2.2/latentscope/models/providers/cohereai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1993 2024-03-19 18:58:41.000000 latentscope-0.2.2/latentscope/models/providers/mistralai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1147 2024-03-19 18:59:56.000000 latentscope-0.2.2/latentscope/models/providers/nltk.py
--rw-r--r--   0 enjalot    (501) staff       (20)     2053 2024-03-19 18:57:31.000000 latentscope-0.2.2/latentscope/models/providers/openai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1145 2024-03-19 19:00:13.000000 latentscope-0.2.2/latentscope/models/providers/togetherai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3726 2024-03-19 18:55:22.000000 latentscope-0.2.2/latentscope/models/providers/transformers.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1329 2024-03-19 19:00:29.000000 latentscope-0.2.2/latentscope/models/providers/voyageai.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.071406 latentscope-0.2.2/latentscope/scripts/
--rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-03 13:56:57.000000 latentscope-0.2.2/latentscope/scripts/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3893 2024-01-10 15:27:46.000000 latentscope-0.2.2/latentscope/scripts/cluster-1d.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7056 2024-03-19 19:11:37.000000 latentscope-0.2.2/latentscope/scripts/cluster.py
--rw-r--r--   0 enjalot    (501) staff       (20)    12774 2024-03-20 19:26:26.000000 latentscope-0.2.2/latentscope/scripts/embed.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6907 2024-04-25 14:11:19.000000 latentscope-0.2.2/latentscope/scripts/ingest.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7529 2024-03-19 19:14:07.000000 latentscope-0.2.2/latentscope/scripts/label_clusters.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6306 2024-05-02 18:45:04.000000 latentscope-0.2.2/latentscope/scripts/scope.py
--rw-r--r--   0 enjalot    (501) staff       (20)     2651 2024-01-20 15:57:31.000000 latentscope-0.2.2/latentscope/scripts/umapper-1d.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7489 2024-03-19 19:13:27.000000 latentscope-0.2.2/latentscope/scripts/umapper.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.072146 latentscope-0.2.2/latentscope/server/
--rw-r--r--   0 enjalot    (501) staff       (20)      827 2024-02-12 13:27:13.000000 latentscope-0.2.2/latentscope/server/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7964 2024-04-25 14:48:04.000000 latentscope-0.2.2/latentscope/server/app.py
--rw-r--r--   0 enjalot    (501) staff       (20)     5645 2024-05-02 18:44:22.000000 latentscope-0.2.2/latentscope/server/bulk.py
--rw-r--r--   0 enjalot    (501) staff       (20)    11284 2024-04-25 14:11:19.000000 latentscope-0.2.2/latentscope/server/datasets.py
--rw-r--r--   0 enjalot    (501) staff       (20)    13927 2024-05-02 18:50:28.000000 latentscope-0.2.2/latentscope/server/jobs.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6370 2024-03-01 17:16:49.000000 latentscope-0.2.2/latentscope/server/search.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7653 2024-04-25 14:11:19.000000 latentscope-0.2.2/latentscope/server/tags.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.072354 latentscope-0.2.2/latentscope/util/
--rw-r--r--   0 enjalot    (501) staff       (20)      173 2024-03-05 19:19:01.000000 latentscope-0.2.2/latentscope/util/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3360 2024-03-05 19:17:14.000000 latentscope-0.2.2/latentscope/util/configuration.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.069023 latentscope-0.2.2/latentscope.egg-info/
--rw-r--r--   0 enjalot    (501) staff       (20)    18782 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/PKG-INFO
--rw-r--r--   0 enjalot    (501) staff       (20)     1312 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/SOURCES.txt
--rw-r--r--   0 enjalot    (501) staff       (20)        1 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/dependency_links.txt
--rw-r--r--   0 enjalot    (501) staff       (20)      549 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/entry_points.txt
--rw-r--r--   0 enjalot    (501) staff       (20)     3006 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/requires.txt
--rw-r--r--   0 enjalot    (501) staff       (20)       12 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/top_level.txt
--rw-r--r--   0 enjalot    (501) staff       (20)       38 2024-05-13 13:33:24.076476 latentscope-0.2.2/setup.cfg
--rw-r--r--   0 enjalot    (501) staff       (20)     3865 2024-04-25 14:11:19.000000 latentscope-0.2.2/setup.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-15 13:49:49.591377 latentscope-0.2.3/
+-rw-r--r--   0 enjalot    (501) staff       (20)     1068 2024-02-16 15:11:38.000000 latentscope-0.2.3/LICENSE
+-rw-r--r--   0 enjalot    (501) staff       (20)    18782 2024-05-15 13:49:49.591081 latentscope-0.2.3/PKG-INFO
+-rw-r--r--   0 enjalot    (501) staff       (20)    12878 2024-05-13 13:19:12.000000 latentscope-0.2.3/README.md
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-15 13:49:49.581939 latentscope-0.2.3/latentscope/
+-rw-r--r--   0 enjalot    (501) staff       (20)     2032 2024-04-25 14:11:19.000000 latentscope-0.2.3/latentscope/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)       22 2024-05-15 13:48:54.000000 latentscope-0.2.3/latentscope/__version__.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-15 13:49:49.583310 latentscope-0.2.3/latentscope/models/
+-rw-r--r--   0 enjalot    (501) staff       (20)     2993 2024-03-19 19:02:11.000000 latentscope-0.2.3/latentscope/models/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1686 2024-05-15 13:40:08.000000 latentscope-0.2.3/latentscope/models/chat_models.json
+-rw-r--r--   0 enjalot    (501) staff       (20)     7511 2024-05-15 13:03:25.000000 latentscope-0.2.3/latentscope/models/embedding_models.json
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-15 13:49:49.584965 latentscope-0.2.3/latentscope/models/providers/
+-rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-12 13:46:58.000000 latentscope-0.2.3/latentscope/models/providers/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)      694 2024-01-25 14:33:56.000000 latentscope-0.2.3/latentscope/models/providers/base.py
+-rw-r--r--   0 enjalot    (501) staff       (20)      705 2024-03-19 18:57:45.000000 latentscope-0.2.3/latentscope/models/providers/cohereai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1993 2024-03-19 18:58:41.000000 latentscope-0.2.3/latentscope/models/providers/mistralai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1147 2024-03-19 18:59:56.000000 latentscope-0.2.3/latentscope/models/providers/nltk.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1842 2024-05-15 12:35:36.000000 latentscope-0.2.3/latentscope/models/providers/openai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1145 2024-03-19 19:00:13.000000 latentscope-0.2.3/latentscope/models/providers/togetherai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     4560 2024-05-15 13:33:15.000000 latentscope-0.2.3/latentscope/models/providers/transformers.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1329 2024-03-19 19:00:29.000000 latentscope-0.2.3/latentscope/models/providers/voyageai.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-15 13:49:49.586038 latentscope-0.2.3/latentscope/scripts/
+-rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-03 13:56:57.000000 latentscope-0.2.3/latentscope/scripts/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3893 2024-01-10 15:27:46.000000 latentscope-0.2.3/latentscope/scripts/cluster-1d.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7056 2024-03-19 19:11:37.000000 latentscope-0.2.3/latentscope/scripts/cluster.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    12774 2024-03-20 19:26:26.000000 latentscope-0.2.3/latentscope/scripts/embed.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6907 2024-04-25 14:11:19.000000 latentscope-0.2.3/latentscope/scripts/ingest.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7822 2024-05-15 13:44:21.000000 latentscope-0.2.3/latentscope/scripts/label_clusters.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6306 2024-05-02 18:45:04.000000 latentscope-0.2.3/latentscope/scripts/scope.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     2651 2024-01-20 15:57:31.000000 latentscope-0.2.3/latentscope/scripts/umapper-1d.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7489 2024-03-19 19:13:27.000000 latentscope-0.2.3/latentscope/scripts/umapper.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-15 13:49:49.587100 latentscope-0.2.3/latentscope/server/
+-rw-r--r--   0 enjalot    (501) staff       (20)      827 2024-02-12 13:27:13.000000 latentscope-0.2.3/latentscope/server/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7964 2024-04-25 14:48:04.000000 latentscope-0.2.3/latentscope/server/app.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     5645 2024-05-02 18:44:22.000000 latentscope-0.2.3/latentscope/server/bulk.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    11284 2024-04-25 14:11:19.000000 latentscope-0.2.3/latentscope/server/datasets.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    13927 2024-05-02 18:50:28.000000 latentscope-0.2.3/latentscope/server/jobs.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6370 2024-03-01 17:16:49.000000 latentscope-0.2.3/latentscope/server/search.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7653 2024-04-25 14:11:19.000000 latentscope-0.2.3/latentscope/server/tags.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-15 13:49:49.587319 latentscope-0.2.3/latentscope/util/
+-rw-r--r--   0 enjalot    (501) staff       (20)      173 2024-03-05 19:19:01.000000 latentscope-0.2.3/latentscope/util/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3360 2024-03-05 19:17:14.000000 latentscope-0.2.3/latentscope/util/configuration.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-15 13:49:49.582708 latentscope-0.2.3/latentscope.egg-info/
+-rw-r--r--   0 enjalot    (501) staff       (20)    18782 2024-05-15 13:49:49.000000 latentscope-0.2.3/latentscope.egg-info/PKG-INFO
+-rw-r--r--   0 enjalot    (501) staff       (20)     1312 2024-05-15 13:49:49.000000 latentscope-0.2.3/latentscope.egg-info/SOURCES.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)        1 2024-05-15 13:49:49.000000 latentscope-0.2.3/latentscope.egg-info/dependency_links.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)      549 2024-05-15 13:49:49.000000 latentscope-0.2.3/latentscope.egg-info/entry_points.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)     3006 2024-05-15 13:49:49.000000 latentscope-0.2.3/latentscope.egg-info/requires.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)       12 2024-05-15 13:49:49.000000 latentscope-0.2.3/latentscope.egg-info/top_level.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)       38 2024-05-15 13:49:49.591467 latentscope-0.2.3/setup.cfg
+-rw-r--r--   0 enjalot    (501) staff       (20)     3865 2024-04-25 14:11:19.000000 latentscope-0.2.3/setup.py
```

### Comparing `latentscope-0.2.2/LICENSE` & `latentscope-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/PKG-INFO` & `latentscope-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,185 +1,185 @@
 Metadata-Version: 2.1
 Name: latentscope
-Version: 0.2.2
+Version: 0.2.3
 Summary: Quickly embed, project, cluster and explore a dataset.
 Home-page: https://github.com/enjalot/latent-scope
 Project-URL: Source, https://github.com/enjalot/latent-scope
 Project-URL: Tracker, https://github.com/enjalot/latent-scope/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: accelerate==0.26.1
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: aiolimiter==1.1.0
-Requires-Dist: aiosignal==1.3.1
-Requires-Dist: annotated-types==0.6.0
-Requires-Dist: anyio==4.2.0
-Requires-Dist: appnope==0.1.3
-Requires-Dist: argon2-cffi==23.1.0
-Requires-Dist: argon2-cffi-bindings==21.2.0
-Requires-Dist: arrow==1.3.0
-Requires-Dist: asttokens==2.4.1
-Requires-Dist: async-lru==2.0.4
-Requires-Dist: attrs==23.2.0
-Requires-Dist: Babel==2.14.0
-Requires-Dist: backoff==2.2.1
-Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: bleach==6.1.0
-Requires-Dist: blinker==1.7.0
-Requires-Dist: certifi==2023.11.17
-Requires-Dist: cffi==1.16.0
-Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: click==8.1.7
-Requires-Dist: cohere==4.44
-Requires-Dist: comm==0.2.1
-Requires-Dist: contourpy==1.2.0
-Requires-Dist: cycler==0.12.1
-Requires-Dist: Cython==0.29.37
-Requires-Dist: debugpy==1.8.0
-Requires-Dist: decorator==5.1.1
-Requires-Dist: defusedxml==0.7.1
-Requires-Dist: distro==1.9.0
-Requires-Dist: einops==0.7.0
-Requires-Dist: executing==2.0.1
-Requires-Dist: fastavro==1.9.3
-Requires-Dist: fastjsonschema==2.19.1
-Requires-Dist: filelock==3.13.1
-Requires-Dist: Flask==3.0.0
-Requires-Dist: Flask-Cors==4.0.0
-Requires-Dist: fonttools==4.47.2
-Requires-Dist: fqdn==1.5.1
-Requires-Dist: frozenlist==1.4.1
-Requires-Dist: fsspec==2023.10.0
-Requires-Dist: h11==0.14.0
-Requires-Dist: h5py==3.10.0
-Requires-Dist: hdbscan==0.8.33
-Requires-Dist: httpcore==1.0.2
-Requires-Dist: httpx==0.25.2
-Requires-Dist: huggingface-hub==0.20.2
-Requires-Dist: idna==3.6
-Requires-Dist: importlib-metadata==6.11.0
-Requires-Dist: ipykernel==6.29.0
-Requires-Dist: ipython==8.20.0
-Requires-Dist: ipywidgets==8.1.1
-Requires-Dist: isoduration==20.11.0
-Requires-Dist: itsdangerous==2.1.2
-Requires-Dist: jedi==0.19.1
-Requires-Dist: Jinja2==3.1.3
-Requires-Dist: joblib==1.3.2
-Requires-Dist: json5==0.9.14
-Requires-Dist: jsonpointer==2.4
-Requires-Dist: jsonschema==4.21.1
-Requires-Dist: jsonschema-specifications==2023.12.1
-Requires-Dist: jupyter==1.0.0
-Requires-Dist: jupyter-console==6.6.3
-Requires-Dist: jupyter-events==0.9.0
-Requires-Dist: jupyter-lsp==2.2.2
-Requires-Dist: jupyter_client==8.6.0
-Requires-Dist: jupyter_core==5.7.1
-Requires-Dist: jupyter_server==2.12.5
-Requires-Dist: jupyter_server_terminals==0.5.2
-Requires-Dist: jupyterlab==4.0.12
-Requires-Dist: jupyterlab-widgets==3.0.9
-Requires-Dist: jupyterlab_pygments==0.3.0
-Requires-Dist: jupyterlab_server==2.25.2
-Requires-Dist: kiwisolver==1.4.5
-Requires-Dist: llvmlite==0.41.1
-Requires-Dist: MarkupSafe==2.1.3
-Requires-Dist: matplotlib==3.8.2
-Requires-Dist: matplotlib-inline==0.1.6
-Requires-Dist: mistralai==0.0.11
-Requires-Dist: mistune==3.0.2
-Requires-Dist: mpmath==1.3.0
-Requires-Dist: multidict==6.0.4
-Requires-Dist: nbclient==0.9.0
-Requires-Dist: nbconvert==7.14.2
-Requires-Dist: nbformat==5.9.2
-Requires-Dist: nest-asyncio==1.5.9
-Requires-Dist: networkx==3.2.1
-Requires-Dist: nltk==3.8.1
-Requires-Dist: notebook==7.0.7
-Requires-Dist: notebook_shim==0.2.3
-Requires-Dist: numba==0.58.1
-Requires-Dist: numpy==1.26.3
-Requires-Dist: openai==1.12.0
-Requires-Dist: opt-einsum==3.3.0
-Requires-Dist: orjson==3.9.12
-Requires-Dist: overrides==7.7.0
-Requires-Dist: packaging==23.2
-Requires-Dist: pandas==2.1.4
-Requires-Dist: pandocfilters==1.5.1
-Requires-Dist: parso==0.8.3
-Requires-Dist: pexpect==4.9.0
-Requires-Dist: pillow==10.2.0
-Requires-Dist: platformdirs==4.1.0
-Requires-Dist: prometheus-client==0.19.0
-Requires-Dist: prompt-toolkit==3.0.43
-Requires-Dist: psutil==5.9.7
-Requires-Dist: ptyprocess==0.7.0
-Requires-Dist: pure-eval==0.2.2
-Requires-Dist: pyarrow==14.0.2
-Requires-Dist: pycparser==2.21
-Requires-Dist: pydantic==2.5.3
-Requires-Dist: pydantic_core==2.14.6
-Requires-Dist: Pygments==2.17.2
-Requires-Dist: pynndescent==0.5.11
-Requires-Dist: pyparsing==3.1.1
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: python-json-logger==2.0.7
-Requires-Dist: pytz==2023.3.post1
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: pyzmq==25.1.2
-Requires-Dist: qtconsole==5.5.1
-Requires-Dist: QtPy==2.4.1
-Requires-Dist: referencing==0.33.0
-Requires-Dist: regex==2023.12.25
-Requires-Dist: requests==2.31.0
-Requires-Dist: rfc3339-validator==0.1.4
-Requires-Dist: rfc3986-validator==0.1.1
-Requires-Dist: rpds-py==0.17.1
-Requires-Dist: safetensors==0.4.1
-Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: scipy==1.11.4
-Requires-Dist: Send2Trash==1.8.2
-Requires-Dist: six==1.16.0
-Requires-Dist: sniffio==1.3.0
-Requires-Dist: soupsieve==2.5
-Requires-Dist: sseclient-py==1.8.0
-Requires-Dist: stack-data==0.6.3
-Requires-Dist: sympy==1.12
-Requires-Dist: tabulate==0.9.0
-Requires-Dist: tenacity==8.2.3
-Requires-Dist: terminado==0.18.0
-Requires-Dist: threadpoolctl==3.2.0
-Requires-Dist: tiktoken==0.5.2
-Requires-Dist: tinycss2==1.2.1
-Requires-Dist: together==0.2.10
-Requires-Dist: tokenizers==0.15.0
-Requires-Dist: torch==2.1.2
-Requires-Dist: tornado==6.4
-Requires-Dist: tqdm==4.66.1
-Requires-Dist: traitlets==5.14.1
-Requires-Dist: transformers==4.36.2
-Requires-Dist: typer==0.9.0
-Requires-Dist: types-python-dateutil==2.8.19.20240106
-Requires-Dist: typing_extensions==4.9.0
-Requires-Dist: tzdata==2023.4
-Requires-Dist: umap-learn==0.5.5
-Requires-Dist: uri-template==1.3.0
-Requires-Dist: urllib3==2.1.0
-Requires-Dist: voyageai==0.1.6
-Requires-Dist: wcwidth==0.2.13
-Requires-Dist: webcolors==1.13
-Requires-Dist: webencodings==0.5.1
-Requires-Dist: websocket-client==1.7.0
-Requires-Dist: Werkzeug==3.0.1
-Requires-Dist: widgetsnbextension==4.0.9
-Requires-Dist: yarl==1.9.4
-Requires-Dist: zipp==3.17.0
+Requires-Dist: accelerate~=0.26.1
+Requires-Dist: aiohttp~=3.9.1
+Requires-Dist: aiolimiter~=1.1.0
+Requires-Dist: aiosignal~=1.3.1
+Requires-Dist: annotated-types~=0.6.0
+Requires-Dist: anyio~=4.2.0
+Requires-Dist: appnope~=0.1.3
+Requires-Dist: argon2-cffi~=23.1.0
+Requires-Dist: argon2-cffi-bindings~=21.2.0
+Requires-Dist: arrow~=1.3.0
+Requires-Dist: asttokens~=2.4.1
+Requires-Dist: async-lru~=2.0.4
+Requires-Dist: attrs~=23.2.0
+Requires-Dist: Babel~=2.14.0
+Requires-Dist: backoff~=2.2.1
+Requires-Dist: beautifulsoup4~=4.12.3
+Requires-Dist: bleach~=6.1.0
+Requires-Dist: blinker~=1.7.0
+Requires-Dist: certifi~=2023.11.17
+Requires-Dist: cffi~=1.16.0
+Requires-Dist: charset-normalizer~=3.3.2
+Requires-Dist: click~=8.1.7
+Requires-Dist: cohere~=4.44
+Requires-Dist: comm~=0.2.1
+Requires-Dist: contourpy~=1.2.0
+Requires-Dist: cycler~=0.12.1
+Requires-Dist: Cython~=0.29.37
+Requires-Dist: debugpy~=1.8.0
+Requires-Dist: decorator~=5.1.1
+Requires-Dist: defusedxml~=0.7.1
+Requires-Dist: distro~=1.9.0
+Requires-Dist: einops~=0.7.0
+Requires-Dist: executing~=2.0.1
+Requires-Dist: fastavro~=1.9.3
+Requires-Dist: fastjsonschema~=2.19.1
+Requires-Dist: filelock~=3.13.1
+Requires-Dist: Flask~=3.0.0
+Requires-Dist: Flask-Cors~=4.0.0
+Requires-Dist: fonttools~=4.47.2
+Requires-Dist: fqdn~=1.5.1
+Requires-Dist: frozenlist~=1.4.1
+Requires-Dist: fsspec~=2023.10.0
+Requires-Dist: h11~=0.14.0
+Requires-Dist: h5py~=3.10.0
+Requires-Dist: hdbscan~=0.8.33
+Requires-Dist: httpcore~=1.0.2
+Requires-Dist: httpx~=0.25.2
+Requires-Dist: huggingface-hub~=0.20.2
+Requires-Dist: idna~=3.6
+Requires-Dist: importlib-metadata~=6.11.0
+Requires-Dist: ipykernel~=6.29.0
+Requires-Dist: ipython~=8.20.0
+Requires-Dist: ipywidgets~=8.1.1
+Requires-Dist: isoduration~=20.11.0
+Requires-Dist: itsdangerous~=2.1.2
+Requires-Dist: jedi~=0.19.1
+Requires-Dist: Jinja2~=3.1.3
+Requires-Dist: joblib~=1.3.2
+Requires-Dist: json5~=0.9.14
+Requires-Dist: jsonpointer~=2.4
+Requires-Dist: jsonschema~=4.21.1
+Requires-Dist: jsonschema-specifications~=2023.12.1
+Requires-Dist: jupyter~=1.0.0
+Requires-Dist: jupyter-console~=6.6.3
+Requires-Dist: jupyter-events~=0.9.0
+Requires-Dist: jupyter-lsp~=2.2.2
+Requires-Dist: jupyter_client~=8.6.0
+Requires-Dist: jupyter_core~=5.7.1
+Requires-Dist: jupyter_server~=2.12.5
+Requires-Dist: jupyter_server_terminals~=0.5.2
+Requires-Dist: jupyterlab~=4.0.12
+Requires-Dist: jupyterlab-widgets~=3.0.9
+Requires-Dist: jupyterlab_pygments~=0.3.0
+Requires-Dist: jupyterlab_server~=2.25.2
+Requires-Dist: kiwisolver~=1.4.5
+Requires-Dist: llvmlite~=0.41.1
+Requires-Dist: MarkupSafe~=2.1.3
+Requires-Dist: matplotlib~=3.8.2
+Requires-Dist: matplotlib-inline~=0.1.6
+Requires-Dist: mistralai~=0.0.11
+Requires-Dist: mistune~=3.0.2
+Requires-Dist: mpmath~=1.3.0
+Requires-Dist: multidict~=6.0.4
+Requires-Dist: nbclient~=0.9.0
+Requires-Dist: nbconvert~=7.14.2
+Requires-Dist: nbformat~=5.9.2
+Requires-Dist: nest-asyncio~=1.5.9
+Requires-Dist: networkx~=3.2.1
+Requires-Dist: nltk~=3.8.1
+Requires-Dist: notebook~=7.0.7
+Requires-Dist: notebook_shim~=0.2.3
+Requires-Dist: numba~=0.58.1
+Requires-Dist: numpy~=1.26.3
+Requires-Dist: openai~=1.12.0
+Requires-Dist: opt-einsum~=3.3.0
+Requires-Dist: orjson~=3.9.12
+Requires-Dist: overrides~=7.7.0
+Requires-Dist: packaging~=23.2
+Requires-Dist: pandas~=2.1.4
+Requires-Dist: pandocfilters~=1.5.1
+Requires-Dist: parso~=0.8.3
+Requires-Dist: pexpect~=4.9.0
+Requires-Dist: pillow~=10.2.0
+Requires-Dist: platformdirs~=4.1.0
+Requires-Dist: prometheus-client~=0.19.0
+Requires-Dist: prompt-toolkit~=3.0.43
+Requires-Dist: psutil~=5.9.7
+Requires-Dist: ptyprocess~=0.7.0
+Requires-Dist: pure-eval~=0.2.2
+Requires-Dist: pyarrow~=14.0.2
+Requires-Dist: pycparser~=2.21
+Requires-Dist: pydantic~=2.5.3
+Requires-Dist: pydantic_core~=2.14.6
+Requires-Dist: Pygments~=2.17.2
+Requires-Dist: pynndescent~=0.5.11
+Requires-Dist: pyparsing~=3.1.1
+Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: python-dotenv~=1.0.0
+Requires-Dist: python-json-logger~=2.0.7
+Requires-Dist: pytz~=2023.3.post1
+Requires-Dist: PyYAML~=6.0.1
+Requires-Dist: pyzmq~=25.1.2
+Requires-Dist: qtconsole~=5.5.1
+Requires-Dist: QtPy~=2.4.1
+Requires-Dist: referencing~=0.33.0
+Requires-Dist: regex~=2023.12.25
+Requires-Dist: requests~=2.31.0
+Requires-Dist: rfc3339-validator~=0.1.4
+Requires-Dist: rfc3986-validator~=0.1.1
+Requires-Dist: rpds-py~=0.17.1
+Requires-Dist: safetensors~=0.4.1
+Requires-Dist: scikit-learn~=1.3.2
+Requires-Dist: scipy~=1.11.4
+Requires-Dist: Send2Trash~=1.8.2
+Requires-Dist: six~=1.16.0
+Requires-Dist: sniffio~=1.3.0
+Requires-Dist: soupsieve~=2.5
+Requires-Dist: sseclient-py~=1.8.0
+Requires-Dist: stack-data~=0.6.3
+Requires-Dist: sympy~=1.12
+Requires-Dist: tabulate~=0.9.0
+Requires-Dist: tenacity~=8.2.3
+Requires-Dist: terminado~=0.18.0
+Requires-Dist: threadpoolctl~=3.2.0
+Requires-Dist: tiktoken~=0.7.0
+Requires-Dist: tinycss2~=1.2.1
+Requires-Dist: together~=0.2.10
+Requires-Dist: tokenizers~=0.15.0
+Requires-Dist: torch~=2.1.2
+Requires-Dist: tornado~=6.4
+Requires-Dist: tqdm~=4.66.1
+Requires-Dist: traitlets~=5.14.1
+Requires-Dist: transformers~=4.36.2
+Requires-Dist: typer~=0.9.0
+Requires-Dist: types-python-dateutil~=2.8.19.20240106
+Requires-Dist: typing_extensions~=4.9.0
+Requires-Dist: tzdata~=2023.4
+Requires-Dist: umap-learn~=0.5.5
+Requires-Dist: uri-template~=1.3.0
+Requires-Dist: urllib3~=2.1.0
+Requires-Dist: voyageai~=0.1.6
+Requires-Dist: wcwidth~=0.2.13
+Requires-Dist: webcolors~=1.13
+Requires-Dist: webencodings~=0.5.1
+Requires-Dist: websocket-client~=1.7.0
+Requires-Dist: Werkzeug~=3.0.1
+Requires-Dist: widgetsnbextension~=4.0.9
+Requires-Dist: yarl~=1.9.4
+Requires-Dist: zipp~=3.17.0
 
 # Latent Scope
 [![](https://dcbadge.vercel.app/api/server/x7NvpnM4pY?style=flat)](https://discord.gg/x7NvpnM4pY)
 [![PyPI version](https://img.shields.io/pypi/v/latentscope.svg)](https://pypi.org/project/latentscope/)
 
 Quickly embed, project, cluster and explore a dataset. This project is a new kind of workflow + tool for visualizing and exploring datasets through the lens of latent spaces.
```

### Comparing `latentscope-0.2.2/README.md` & `latentscope-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/__init__.py` & `latentscope-0.2.3/latentscope/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/models/__init__.py` & `latentscope-0.2.3/latentscope/models/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/models/embedding_models.json` & `latentscope-0.2.3/latentscope/models/embedding_models.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8737268518518518%*

 * *Differences: {'4': "{'params': {'rps': True}}",*

 * * '5': "{'params': {'rps': True}}",*

 * * 'insert': "[(6, OrderedDict([('provider', 'transformers'), ('name', "*

 * *           "'Snowflake/snowflake-arctic-embed-s'), ('sanitized_name', "*

 * *           "'Snowflake___snowflake-arctic-embed-s'), ('id', "*

 * *           "'transformers-Snowflake___snowflake-arctic-embed-s'), ('modality', 'text'), ('params', "*

 * *           "OrderedDict([('truncation', True), ('padding', True), ('pooling', 'cls')]))])), (7, "*

 * *           "OrderedDict([('provider',  […]*

```diff
@@ -51,14 +51,15 @@
         "id": "transformers-nomic-ai___nomic-embed-text-v1",
         "modality": "text",
         "name": "nomic-ai/nomic-embed-text-v1",
         "params": {
             "max_tokens": 8192,
             "padding": true,
             "pooling": "mean",
+            "rps": true,
             "truncation": true
         },
         "provider": "transformers",
         "sanitized_name": "nomic-ai___nomic-embed-text-v1"
     },
     {
         "id": "transformers-nomic-ai___nomic-embed-text-v1.5",
@@ -71,20 +72,47 @@
                 256,
                 128,
                 64
             ],
             "max_tokens": 8192,
             "padding": true,
             "pooling": "mean",
+            "rps": true,
             "truncation": true
         },
         "provider": "transformers",
         "sanitized_name": "nomic-ai___nomic-embed-text-v1.5"
     },
     {
+        "id": "transformers-Snowflake___snowflake-arctic-embed-s",
+        "modality": "text",
+        "name": "Snowflake/snowflake-arctic-embed-s",
+        "params": {
+            "padding": true,
+            "pooling": "cls",
+            "truncation": true
+        },
+        "provider": "transformers",
+        "sanitized_name": "Snowflake___snowflake-arctic-embed-s"
+    },
+    {
+        "id": "transformers-Snowflake___snowflake-arctic-embed-m-long",
+        "modality": "text",
+        "name": "Snowflake/snowflake-arctic-embed-m-long",
+        "params": {
+            "max_tokens": 8192,
+            "padding": true,
+            "pooling": "cls",
+            "rps": true,
+            "truncation": true
+        },
+        "provider": "transformers",
+        "sanitized_name": "Snowflake___snowflake-arctic-embed-m-long"
+    },
+    {
         "id": "transformers-intfloat___e5-large-v2",
         "modality": "text",
         "name": "intfloat/e5-large-v2",
         "params": {
             "padding": true,
             "pooling": "average",
             "truncation": true
@@ -101,14 +129,26 @@
             "pooling": "mean",
             "truncation": true
         },
         "provider": "transformers",
         "sanitized_name": "jinaai___jina-embeddings-v2-base-en"
     },
     {
+        "id": "transformers-BAAI___bge-m3",
+        "modality": "text",
+        "name": "BAAI/bge-m3",
+        "params": {
+            "padding": true,
+            "pooling": "cls",
+            "truncation": true
+        },
+        "provider": "transformers",
+        "sanitized_name": "BAAI___bge-m3"
+    },
+    {
         "id": "transformers-BAAI___bge-large-en-v1.5",
         "modality": "text",
         "name": "BAAI/bge-large-en-v1.5",
         "params": {
             "padding": true,
             "pooling": "cls",
             "truncation": true
```

### Comparing `latentscope-0.2.2/latentscope/models/providers/base.py` & `latentscope-0.2.3/latentscope/models/providers/base.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/models/providers/cohereai.py` & `latentscope-0.2.3/latentscope/models/providers/cohereai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/models/providers/mistralai.py` & `latentscope-0.2.3/latentscope/models/providers/mistralai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/models/providers/nltk.py` & `latentscope-0.2.3/latentscope/models/providers/nltk.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/models/providers/openai.py` & `latentscope-0.2.3/latentscope/models/providers/openai.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,15 @@
         from openai import OpenAI
         import tiktoken
         api_key = get_key("OPENAI_API_KEY")
         if api_key is None:
             print("ERROR: No API key found for OpenAI")
             print("Missing 'OPENAI_API_KEY' variable in:", f"{os.getcwd()}/.env")
         self.client = OpenAI(api_key=api_key)
-        # special case for the new embedding models
-        if self.name in ["text-embedding-3-small", "text-embedding-3-large"]:
-            self.encoder = tiktoken.get_encoding("cl100k_base")
-        else:
-            self.encoder = tiktoken.encoding_for_model(self.name)
+        self.encoder = tiktoken.encoding_for_model(self.name)
 
     def embed(self, inputs, dimensions=None):
         time.sleep(0.01) # TODO proper rate limiting
         enc = self.encoder
         max_tokens = self.params["max_tokens"]
         inputs = [b.replace("\n", " ") for b in inputs]
         inputs = [enc.decode(enc.encode(b)[:max_tokens]) if len(enc.encode(b)) > max_tokens else b for b in inputs]
@@ -42,13 +38,14 @@
 class OpenAIChatProvider(ChatModelProvider):
     def load_model(self):
         from openai import OpenAI
         import tiktoken
         self.client = OpenAI(api_key=get_key("OPENAI_API_KEY"))
         self.encoder = tiktoken.encoding_for_model(self.name)
 
+
     def chat(self, messages):
         response = self.client.chat.completions.create(
             model=self.name,
             messages=messages
         )
         return response.choices[0].message.content
```

### Comparing `latentscope-0.2.2/latentscope/models/providers/togetherai.py` & `latentscope-0.2.3/latentscope/models/providers/togetherai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/models/providers/voyageai.py` & `latentscope-0.2.3/latentscope/models/providers/voyageai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/scripts/cluster-1d.py` & `latentscope-0.2.3/latentscope/scripts/cluster-1d.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/scripts/cluster.py` & `latentscope-0.2.3/latentscope/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/scripts/embed.py` & `latentscope-0.2.3/latentscope/scripts/embed.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/scripts/ingest.py` & `latentscope-0.2.3/latentscope/scripts/ingest.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/scripts/label_clusters.py` & `latentscope-0.2.3/latentscope/scripts/label_clusters.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,18 +83,18 @@
         label_id = f"{cluster_id}-labels-{next_label_number:03d}"
     tqdm.write(f"RUNNING: {label_id}")
 
     model = get_chat_model(model_id)
     model.load_model()
     enc = model.encoder
 
-    system_prompt = {"role":"system", "content": f"""You're job is to summarize lists of items with a short label of no more than 4 words. 
+    system_prompt = {"role":"system", "content": f"""You're job is to summarize lists of items with a short label of no more than 4 words. The items are part of a cluster and the label will be used to distinguish this cluster from others, so pay attention to what makes this group of similar items distinct.
 {context}
 The user will submit a bulleted list of items and you should choose a label that best summarizes the theme of the list so that someone browsing the labels will have a good idea of what is in the list. 
-Do not use punctuation, just return a few words that summarize the list."""}
+Do not use punctuation, Do not explain yourself, respond with only a few words that summarize the list."""}
 
     # TODO: why the extra 10 for openai?
     max_tokens = model.params["max_tokens"] - len(enc.encode(system_prompt["content"])) - 10
 
     # Create the lists of items we will send for summarization
     # Current looks like:
     # 1. item 1
@@ -125,15 +125,15 @@
                 tqdm.write(f"skipping {i} already labeled {clusters.loc[i, 'label']}")
                 time.sleep(0.01)
                 continue
 
         try:
             time.sleep(0.01)
             messages=[
-                system_prompt, {"role":"user", "content": batch[0]} # TODO hardcoded batch size
+                system_prompt, {"role":"user", "content": "Here is a list of items, please summarize the list into a label using only a few words:\n" + batch[0]} # TODO hardcoded batch size
             ]
             label = model.chat(messages)
             labels.append(label)
             # tqdm.write("label:\n", label)
             # do some cleanup of the labels when the model doesn't follow instructions
             clean_label = label.replace("\n", " ")
             clean_label = clean_label.replace('"', '')
```

### Comparing `latentscope-0.2.2/latentscope/scripts/scope.py` & `latentscope-0.2.3/latentscope/scripts/scope.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/scripts/umapper-1d.py` & `latentscope-0.2.3/latentscope/scripts/umapper-1d.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/scripts/umapper.py` & `latentscope-0.2.3/latentscope/scripts/umapper.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/server/__init__.py` & `latentscope-0.2.3/latentscope/server/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/server/app.py` & `latentscope-0.2.3/latentscope/server/app.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/server/bulk.py` & `latentscope-0.2.3/latentscope/server/bulk.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/server/datasets.py` & `latentscope-0.2.3/latentscope/server/datasets.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/server/jobs.py` & `latentscope-0.2.3/latentscope/server/jobs.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/server/search.py` & `latentscope-0.2.3/latentscope/server/search.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/server/tags.py` & `latentscope-0.2.3/latentscope/server/tags.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope/util/configuration.py` & `latentscope-0.2.3/latentscope/util/configuration.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope.egg-info/PKG-INFO` & `latentscope-0.2.3/latentscope.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,185 +1,185 @@
 Metadata-Version: 2.1
 Name: latentscope
-Version: 0.2.2
+Version: 0.2.3
 Summary: Quickly embed, project, cluster and explore a dataset.
 Home-page: https://github.com/enjalot/latent-scope
 Project-URL: Source, https://github.com/enjalot/latent-scope
 Project-URL: Tracker, https://github.com/enjalot/latent-scope/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: accelerate==0.26.1
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: aiolimiter==1.1.0
-Requires-Dist: aiosignal==1.3.1
-Requires-Dist: annotated-types==0.6.0
-Requires-Dist: anyio==4.2.0
-Requires-Dist: appnope==0.1.3
-Requires-Dist: argon2-cffi==23.1.0
-Requires-Dist: argon2-cffi-bindings==21.2.0
-Requires-Dist: arrow==1.3.0
-Requires-Dist: asttokens==2.4.1
-Requires-Dist: async-lru==2.0.4
-Requires-Dist: attrs==23.2.0
-Requires-Dist: Babel==2.14.0
-Requires-Dist: backoff==2.2.1
-Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: bleach==6.1.0
-Requires-Dist: blinker==1.7.0
-Requires-Dist: certifi==2023.11.17
-Requires-Dist: cffi==1.16.0
-Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: click==8.1.7
-Requires-Dist: cohere==4.44
-Requires-Dist: comm==0.2.1
-Requires-Dist: contourpy==1.2.0
-Requires-Dist: cycler==0.12.1
-Requires-Dist: Cython==0.29.37
-Requires-Dist: debugpy==1.8.0
-Requires-Dist: decorator==5.1.1
-Requires-Dist: defusedxml==0.7.1
-Requires-Dist: distro==1.9.0
-Requires-Dist: einops==0.7.0
-Requires-Dist: executing==2.0.1
-Requires-Dist: fastavro==1.9.3
-Requires-Dist: fastjsonschema==2.19.1
-Requires-Dist: filelock==3.13.1
-Requires-Dist: Flask==3.0.0
-Requires-Dist: Flask-Cors==4.0.0
-Requires-Dist: fonttools==4.47.2
-Requires-Dist: fqdn==1.5.1
-Requires-Dist: frozenlist==1.4.1
-Requires-Dist: fsspec==2023.10.0
-Requires-Dist: h11==0.14.0
-Requires-Dist: h5py==3.10.0
-Requires-Dist: hdbscan==0.8.33
-Requires-Dist: httpcore==1.0.2
-Requires-Dist: httpx==0.25.2
-Requires-Dist: huggingface-hub==0.20.2
-Requires-Dist: idna==3.6
-Requires-Dist: importlib-metadata==6.11.0
-Requires-Dist: ipykernel==6.29.0
-Requires-Dist: ipython==8.20.0
-Requires-Dist: ipywidgets==8.1.1
-Requires-Dist: isoduration==20.11.0
-Requires-Dist: itsdangerous==2.1.2
-Requires-Dist: jedi==0.19.1
-Requires-Dist: Jinja2==3.1.3
-Requires-Dist: joblib==1.3.2
-Requires-Dist: json5==0.9.14
-Requires-Dist: jsonpointer==2.4
-Requires-Dist: jsonschema==4.21.1
-Requires-Dist: jsonschema-specifications==2023.12.1
-Requires-Dist: jupyter==1.0.0
-Requires-Dist: jupyter-console==6.6.3
-Requires-Dist: jupyter-events==0.9.0
-Requires-Dist: jupyter-lsp==2.2.2
-Requires-Dist: jupyter_client==8.6.0
-Requires-Dist: jupyter_core==5.7.1
-Requires-Dist: jupyter_server==2.12.5
-Requires-Dist: jupyter_server_terminals==0.5.2
-Requires-Dist: jupyterlab==4.0.12
-Requires-Dist: jupyterlab-widgets==3.0.9
-Requires-Dist: jupyterlab_pygments==0.3.0
-Requires-Dist: jupyterlab_server==2.25.2
-Requires-Dist: kiwisolver==1.4.5
-Requires-Dist: llvmlite==0.41.1
-Requires-Dist: MarkupSafe==2.1.3
-Requires-Dist: matplotlib==3.8.2
-Requires-Dist: matplotlib-inline==0.1.6
-Requires-Dist: mistralai==0.0.11
-Requires-Dist: mistune==3.0.2
-Requires-Dist: mpmath==1.3.0
-Requires-Dist: multidict==6.0.4
-Requires-Dist: nbclient==0.9.0
-Requires-Dist: nbconvert==7.14.2
-Requires-Dist: nbformat==5.9.2
-Requires-Dist: nest-asyncio==1.5.9
-Requires-Dist: networkx==3.2.1
-Requires-Dist: nltk==3.8.1
-Requires-Dist: notebook==7.0.7
-Requires-Dist: notebook_shim==0.2.3
-Requires-Dist: numba==0.58.1
-Requires-Dist: numpy==1.26.3
-Requires-Dist: openai==1.12.0
-Requires-Dist: opt-einsum==3.3.0
-Requires-Dist: orjson==3.9.12
-Requires-Dist: overrides==7.7.0
-Requires-Dist: packaging==23.2
-Requires-Dist: pandas==2.1.4
-Requires-Dist: pandocfilters==1.5.1
-Requires-Dist: parso==0.8.3
-Requires-Dist: pexpect==4.9.0
-Requires-Dist: pillow==10.2.0
-Requires-Dist: platformdirs==4.1.0
-Requires-Dist: prometheus-client==0.19.0
-Requires-Dist: prompt-toolkit==3.0.43
-Requires-Dist: psutil==5.9.7
-Requires-Dist: ptyprocess==0.7.0
-Requires-Dist: pure-eval==0.2.2
-Requires-Dist: pyarrow==14.0.2
-Requires-Dist: pycparser==2.21
-Requires-Dist: pydantic==2.5.3
-Requires-Dist: pydantic_core==2.14.6
-Requires-Dist: Pygments==2.17.2
-Requires-Dist: pynndescent==0.5.11
-Requires-Dist: pyparsing==3.1.1
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: python-json-logger==2.0.7
-Requires-Dist: pytz==2023.3.post1
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: pyzmq==25.1.2
-Requires-Dist: qtconsole==5.5.1
-Requires-Dist: QtPy==2.4.1
-Requires-Dist: referencing==0.33.0
-Requires-Dist: regex==2023.12.25
-Requires-Dist: requests==2.31.0
-Requires-Dist: rfc3339-validator==0.1.4
-Requires-Dist: rfc3986-validator==0.1.1
-Requires-Dist: rpds-py==0.17.1
-Requires-Dist: safetensors==0.4.1
-Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: scipy==1.11.4
-Requires-Dist: Send2Trash==1.8.2
-Requires-Dist: six==1.16.0
-Requires-Dist: sniffio==1.3.0
-Requires-Dist: soupsieve==2.5
-Requires-Dist: sseclient-py==1.8.0
-Requires-Dist: stack-data==0.6.3
-Requires-Dist: sympy==1.12
-Requires-Dist: tabulate==0.9.0
-Requires-Dist: tenacity==8.2.3
-Requires-Dist: terminado==0.18.0
-Requires-Dist: threadpoolctl==3.2.0
-Requires-Dist: tiktoken==0.5.2
-Requires-Dist: tinycss2==1.2.1
-Requires-Dist: together==0.2.10
-Requires-Dist: tokenizers==0.15.0
-Requires-Dist: torch==2.1.2
-Requires-Dist: tornado==6.4
-Requires-Dist: tqdm==4.66.1
-Requires-Dist: traitlets==5.14.1
-Requires-Dist: transformers==4.36.2
-Requires-Dist: typer==0.9.0
-Requires-Dist: types-python-dateutil==2.8.19.20240106
-Requires-Dist: typing_extensions==4.9.0
-Requires-Dist: tzdata==2023.4
-Requires-Dist: umap-learn==0.5.5
-Requires-Dist: uri-template==1.3.0
-Requires-Dist: urllib3==2.1.0
-Requires-Dist: voyageai==0.1.6
-Requires-Dist: wcwidth==0.2.13
-Requires-Dist: webcolors==1.13
-Requires-Dist: webencodings==0.5.1
-Requires-Dist: websocket-client==1.7.0
-Requires-Dist: Werkzeug==3.0.1
-Requires-Dist: widgetsnbextension==4.0.9
-Requires-Dist: yarl==1.9.4
-Requires-Dist: zipp==3.17.0
+Requires-Dist: accelerate~=0.26.1
+Requires-Dist: aiohttp~=3.9.1
+Requires-Dist: aiolimiter~=1.1.0
+Requires-Dist: aiosignal~=1.3.1
+Requires-Dist: annotated-types~=0.6.0
+Requires-Dist: anyio~=4.2.0
+Requires-Dist: appnope~=0.1.3
+Requires-Dist: argon2-cffi~=23.1.0
+Requires-Dist: argon2-cffi-bindings~=21.2.0
+Requires-Dist: arrow~=1.3.0
+Requires-Dist: asttokens~=2.4.1
+Requires-Dist: async-lru~=2.0.4
+Requires-Dist: attrs~=23.2.0
+Requires-Dist: Babel~=2.14.0
+Requires-Dist: backoff~=2.2.1
+Requires-Dist: beautifulsoup4~=4.12.3
+Requires-Dist: bleach~=6.1.0
+Requires-Dist: blinker~=1.7.0
+Requires-Dist: certifi~=2023.11.17
+Requires-Dist: cffi~=1.16.0
+Requires-Dist: charset-normalizer~=3.3.2
+Requires-Dist: click~=8.1.7
+Requires-Dist: cohere~=4.44
+Requires-Dist: comm~=0.2.1
+Requires-Dist: contourpy~=1.2.0
+Requires-Dist: cycler~=0.12.1
+Requires-Dist: Cython~=0.29.37
+Requires-Dist: debugpy~=1.8.0
+Requires-Dist: decorator~=5.1.1
+Requires-Dist: defusedxml~=0.7.1
+Requires-Dist: distro~=1.9.0
+Requires-Dist: einops~=0.7.0
+Requires-Dist: executing~=2.0.1
+Requires-Dist: fastavro~=1.9.3
+Requires-Dist: fastjsonschema~=2.19.1
+Requires-Dist: filelock~=3.13.1
+Requires-Dist: Flask~=3.0.0
+Requires-Dist: Flask-Cors~=4.0.0
+Requires-Dist: fonttools~=4.47.2
+Requires-Dist: fqdn~=1.5.1
+Requires-Dist: frozenlist~=1.4.1
+Requires-Dist: fsspec~=2023.10.0
+Requires-Dist: h11~=0.14.0
+Requires-Dist: h5py~=3.10.0
+Requires-Dist: hdbscan~=0.8.33
+Requires-Dist: httpcore~=1.0.2
+Requires-Dist: httpx~=0.25.2
+Requires-Dist: huggingface-hub~=0.20.2
+Requires-Dist: idna~=3.6
+Requires-Dist: importlib-metadata~=6.11.0
+Requires-Dist: ipykernel~=6.29.0
+Requires-Dist: ipython~=8.20.0
+Requires-Dist: ipywidgets~=8.1.1
+Requires-Dist: isoduration~=20.11.0
+Requires-Dist: itsdangerous~=2.1.2
+Requires-Dist: jedi~=0.19.1
+Requires-Dist: Jinja2~=3.1.3
+Requires-Dist: joblib~=1.3.2
+Requires-Dist: json5~=0.9.14
+Requires-Dist: jsonpointer~=2.4
+Requires-Dist: jsonschema~=4.21.1
+Requires-Dist: jsonschema-specifications~=2023.12.1
+Requires-Dist: jupyter~=1.0.0
+Requires-Dist: jupyter-console~=6.6.3
+Requires-Dist: jupyter-events~=0.9.0
+Requires-Dist: jupyter-lsp~=2.2.2
+Requires-Dist: jupyter_client~=8.6.0
+Requires-Dist: jupyter_core~=5.7.1
+Requires-Dist: jupyter_server~=2.12.5
+Requires-Dist: jupyter_server_terminals~=0.5.2
+Requires-Dist: jupyterlab~=4.0.12
+Requires-Dist: jupyterlab-widgets~=3.0.9
+Requires-Dist: jupyterlab_pygments~=0.3.0
+Requires-Dist: jupyterlab_server~=2.25.2
+Requires-Dist: kiwisolver~=1.4.5
+Requires-Dist: llvmlite~=0.41.1
+Requires-Dist: MarkupSafe~=2.1.3
+Requires-Dist: matplotlib~=3.8.2
+Requires-Dist: matplotlib-inline~=0.1.6
+Requires-Dist: mistralai~=0.0.11
+Requires-Dist: mistune~=3.0.2
+Requires-Dist: mpmath~=1.3.0
+Requires-Dist: multidict~=6.0.4
+Requires-Dist: nbclient~=0.9.0
+Requires-Dist: nbconvert~=7.14.2
+Requires-Dist: nbformat~=5.9.2
+Requires-Dist: nest-asyncio~=1.5.9
+Requires-Dist: networkx~=3.2.1
+Requires-Dist: nltk~=3.8.1
+Requires-Dist: notebook~=7.0.7
+Requires-Dist: notebook_shim~=0.2.3
+Requires-Dist: numba~=0.58.1
+Requires-Dist: numpy~=1.26.3
+Requires-Dist: openai~=1.12.0
+Requires-Dist: opt-einsum~=3.3.0
+Requires-Dist: orjson~=3.9.12
+Requires-Dist: overrides~=7.7.0
+Requires-Dist: packaging~=23.2
+Requires-Dist: pandas~=2.1.4
+Requires-Dist: pandocfilters~=1.5.1
+Requires-Dist: parso~=0.8.3
+Requires-Dist: pexpect~=4.9.0
+Requires-Dist: pillow~=10.2.0
+Requires-Dist: platformdirs~=4.1.0
+Requires-Dist: prometheus-client~=0.19.0
+Requires-Dist: prompt-toolkit~=3.0.43
+Requires-Dist: psutil~=5.9.7
+Requires-Dist: ptyprocess~=0.7.0
+Requires-Dist: pure-eval~=0.2.2
+Requires-Dist: pyarrow~=14.0.2
+Requires-Dist: pycparser~=2.21
+Requires-Dist: pydantic~=2.5.3
+Requires-Dist: pydantic_core~=2.14.6
+Requires-Dist: Pygments~=2.17.2
+Requires-Dist: pynndescent~=0.5.11
+Requires-Dist: pyparsing~=3.1.1
+Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: python-dotenv~=1.0.0
+Requires-Dist: python-json-logger~=2.0.7
+Requires-Dist: pytz~=2023.3.post1
+Requires-Dist: PyYAML~=6.0.1
+Requires-Dist: pyzmq~=25.1.2
+Requires-Dist: qtconsole~=5.5.1
+Requires-Dist: QtPy~=2.4.1
+Requires-Dist: referencing~=0.33.0
+Requires-Dist: regex~=2023.12.25
+Requires-Dist: requests~=2.31.0
+Requires-Dist: rfc3339-validator~=0.1.4
+Requires-Dist: rfc3986-validator~=0.1.1
+Requires-Dist: rpds-py~=0.17.1
+Requires-Dist: safetensors~=0.4.1
+Requires-Dist: scikit-learn~=1.3.2
+Requires-Dist: scipy~=1.11.4
+Requires-Dist: Send2Trash~=1.8.2
+Requires-Dist: six~=1.16.0
+Requires-Dist: sniffio~=1.3.0
+Requires-Dist: soupsieve~=2.5
+Requires-Dist: sseclient-py~=1.8.0
+Requires-Dist: stack-data~=0.6.3
+Requires-Dist: sympy~=1.12
+Requires-Dist: tabulate~=0.9.0
+Requires-Dist: tenacity~=8.2.3
+Requires-Dist: terminado~=0.18.0
+Requires-Dist: threadpoolctl~=3.2.0
+Requires-Dist: tiktoken~=0.7.0
+Requires-Dist: tinycss2~=1.2.1
+Requires-Dist: together~=0.2.10
+Requires-Dist: tokenizers~=0.15.0
+Requires-Dist: torch~=2.1.2
+Requires-Dist: tornado~=6.4
+Requires-Dist: tqdm~=4.66.1
+Requires-Dist: traitlets~=5.14.1
+Requires-Dist: transformers~=4.36.2
+Requires-Dist: typer~=0.9.0
+Requires-Dist: types-python-dateutil~=2.8.19.20240106
+Requires-Dist: typing_extensions~=4.9.0
+Requires-Dist: tzdata~=2023.4
+Requires-Dist: umap-learn~=0.5.5
+Requires-Dist: uri-template~=1.3.0
+Requires-Dist: urllib3~=2.1.0
+Requires-Dist: voyageai~=0.1.6
+Requires-Dist: wcwidth~=0.2.13
+Requires-Dist: webcolors~=1.13
+Requires-Dist: webencodings~=0.5.1
+Requires-Dist: websocket-client~=1.7.0
+Requires-Dist: Werkzeug~=3.0.1
+Requires-Dist: widgetsnbextension~=4.0.9
+Requires-Dist: yarl~=1.9.4
+Requires-Dist: zipp~=3.17.0
 
 # Latent Scope
 [![](https://dcbadge.vercel.app/api/server/x7NvpnM4pY?style=flat)](https://discord.gg/x7NvpnM4pY)
 [![PyPI version](https://img.shields.io/pypi/v/latentscope.svg)](https://pypi.org/project/latentscope/)
 
 Quickly embed, project, cluster and explore a dataset. This project is a new kind of workflow + tool for visualizing and exploring datasets through the lens of latent spaces.
```

### Comparing `latentscope-0.2.2/latentscope.egg-info/SOURCES.txt` & `latentscope-0.2.3/latentscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/latentscope.egg-info/entry_points.txt` & `latentscope-0.2.3/latentscope.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.2/setup.py` & `latentscope-0.2.3/setup.py`

 * *Files identical despite different names*

