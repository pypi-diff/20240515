# Comparing `tmp/article_to_podcast-0.1.tar.gz` & `tmp/article_to_podcast-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "article_to_podcast-0.1.tar", last modified: Tue May 14 19:27:36 2024, max compression
+gzip compressed data, was "article_to_podcast-0.1.6.tar", last modified: Wed May 15 06:08:28 2024, max compression
```

## Comparing `article_to_podcast-0.1.tar` & `article_to_podcast-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:36.686529 article_to_podcast-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 19:27:25.000000 article_to_podcast-0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-14 19:27:36.686529 article_to_podcast-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-14 19:27:25.000000 article_to_podcast-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:36.686529 article_to_podcast-0.1/article_to_podcast/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:25.000000 article_to_podcast-0.1/article_to_podcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 19:27:25.000000 article_to_podcast-0.1/article_to_podcast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-14 19:27:25.000000 article_to_podcast-0.1/article_to_podcast/article_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-14 19:27:25.000000 article_to_podcast-0.1/article_to_podcast/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-14 19:27:25.000000 article_to_podcast-0.1/article_to_podcast/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:36.686529 article_to_podcast-0.1/article_to_podcast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-14 19:27:36.000000 article_to_podcast-0.1/article_to_podcast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 19:27:36.000000 article_to_podcast-0.1/article_to_podcast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:27:36.000000 article_to_podcast-0.1/article_to_podcast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 19:27:36.000000 article_to_podcast-0.1/article_to_podcast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 19:27:36.000000 article_to_podcast-0.1/article_to_podcast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 19:27:36.000000 article_to_podcast-0.1/article_to_podcast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 19:27:25.000000 article_to_podcast-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:27:36.686529 article_to_podcast-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:36.686529 article_to_podcast-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-14 19:27:25.000000 article_to_podcast-0.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:28.261960 article_to_podcast-0.1.6/article_to_podcast/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/article_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/article_to_podcast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/tests/test_main.py
```

### Comparing `article_to_podcast-0.1/LICENSE.md` & `article_to_podcast-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `article_to_podcast-0.1/PKG-INFO` & `article_to_podcast-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article-to-podcast
-Version: 0.1
+Version: 0.1.6
 Summary: CLI tool for converting articles to podcasts
 Author: Ivan Kovnatsky
 License: MIT
 Project-URL: Homepage, https://github.com/ivankovnatsky/article-to-podcast
 Project-URL: Changelog, https://github.com/ivankovnatsky/article-to-podcast/releases
 Project-URL: Issues, https://github.com/ivankovnatsky/article-to-podcast/issues
 Project-URL: CI, https://github.com/ivankovnatsky/article-to-podcast/actions
@@ -22,33 +22,32 @@
 Requires-Dist: lxml[html_clean]
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: cogapp; extra == "test"
 
 # Article to Podcast
 
+[![PyPI](https://img.shields.io/pypi/v/ospeak.svg)](https://pypi.org/project/article-to-podcast/)
 [![Changelog](https://img.shields.io/github/release/ivankovnatsky/article-to-podcast.svg)](https://github.com/ivankovnatsky/article-to-podcast/releases)
-[![Tests](https://github.com/ivankovnatsky/article-to-podcast/actions/workflows/test.yml/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions)
+[![Tests](https://github.com/ivankovnatsky/article-to-podcast/workflows/Test/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/github/license/ivankovnatsky/article-to-podcast)](https://github.com/ivankovnatsky/article-to-podcast/blob/main/LICENSE.md)
 
 CLI tool for converting articles to podcasts using OpenAI's Text-to-Speech API.
 
-## Development
+## Usage
 
-If you're using Nix you can start running the tool by entering:
+Install article-to-podcast with:
 
 ```console
-nix develop
+pipx install article-to-podcast
 ```
 
-## Usage
-
 ```console
-python -m article_to_podcast --help                                                                                                                   
-Usage: python -m article_to_podcast [OPTIONS]
+article-to-podcast --help                                                                                                                   
+Usage: article-to-podcast [OPTIONS]
 
 Options:
   --url TEXT                      URL of the article to be fetched.
                                   [required]
   --directory DIRECTORY           Directory where the output audio file will
                                   be saved. The filename will be derived from
                                   the article title.  [required]
@@ -70,19 +69,28 @@
                                   tone and audience. The current voices are
                                   optimized for English.
   --help                          Show this message and exit.
 ```
 
 ```console
 export OPENAI_API_KEY="your-api-key"
-python \
-    -m article_to_podcast \
-    --directory . \
+article-to-podcast \
     --url 'https://blog.kubetools.io/kopylot-an-ai-powered-kubernetes-assistant-for-devops-developers'
+```
 
+## Development
+
+If you're using Nix you can start running the tool by entering:
+
+```console
+nix develop
+```
+
+```console
+export OPENAI_API_KEY="your-api-key"
 python \
     -m article_to_podcast \
     --model tts-1-hd \
     --voice nova \
     --directory . \
     --url 'https://blog.kubetools.io/kopylot-an-ai-powered-kubernetes-assistant-for-devops-developers'
 ```
```

### Comparing `article_to_podcast-0.1/README.md` & `article_to_podcast-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Article to Podcast
 
+[![PyPI](https://img.shields.io/pypi/v/ospeak.svg)](https://pypi.org/project/article-to-podcast/)
 [![Changelog](https://img.shields.io/github/release/ivankovnatsky/article-to-podcast.svg)](https://github.com/ivankovnatsky/article-to-podcast/releases)
-[![Tests](https://github.com/ivankovnatsky/article-to-podcast/actions/workflows/test.yml/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions)
+[![Tests](https://github.com/ivankovnatsky/article-to-podcast/workflows/Test/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/github/license/ivankovnatsky/article-to-podcast)](https://github.com/ivankovnatsky/article-to-podcast/blob/main/LICENSE.md)
 
 CLI tool for converting articles to podcasts using OpenAI's Text-to-Speech API.
 
-## Development
+## Usage
 
-If you're using Nix you can start running the tool by entering:
+Install article-to-podcast with:
 
 ```console
-nix develop
+pipx install article-to-podcast
 ```
 
-## Usage
-
 ```console
-python -m article_to_podcast --help                                                                                                                   
-Usage: python -m article_to_podcast [OPTIONS]
+article-to-podcast --help                                                                                                                   
+Usage: article-to-podcast [OPTIONS]
 
 Options:
   --url TEXT                      URL of the article to be fetched.
                                   [required]
   --directory DIRECTORY           Directory where the output audio file will
                                   be saved. The filename will be derived from
                                   the article title.  [required]
@@ -44,19 +43,28 @@
                                   tone and audience. The current voices are
                                   optimized for English.
   --help                          Show this message and exit.
 ```
 
 ```console
 export OPENAI_API_KEY="your-api-key"
-python \
-    -m article_to_podcast \
-    --directory . \
+article-to-podcast \
     --url 'https://blog.kubetools.io/kopylot-an-ai-powered-kubernetes-assistant-for-devops-developers'
+```
 
+## Development
+
+If you're using Nix you can start running the tool by entering:
+
+```console
+nix develop
+```
+
+```console
+export OPENAI_API_KEY="your-api-key"
 python \
     -m article_to_podcast \
     --model tts-1-hd \
     --voice nova \
     --directory . \
     --url 'https://blog.kubetools.io/kopylot-an-ai-powered-kubernetes-assistant-for-devops-developers'
 ```
```

### Comparing `article_to_podcast-0.1/article_to_podcast/cli.py` & `article_to_podcast-0.1.6/article_to_podcast/cli.py`

 * *Files identical despite different names*

### Comparing `article_to_podcast-0.1/article_to_podcast/main.py` & `article_to_podcast-0.1.6/article_to_podcast/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,10 +50,10 @@
                 success = False
                 break
 
     if success and not combined_audio.empty():
         combined_audio.export(output_path, format=output_format)
         print(f"Combined audio saved to {output_path}")
     else:
-        print("No audio generated due to errors or quota exceeded.")
+        print("No audio generated due to errors.")
         if output_path.exists():
             output_path.unlink()  # Ensure no partial files are left
```

### Comparing `article_to_podcast-0.1/article_to_podcast.egg-info/PKG-INFO` & `article_to_podcast-0.1.6/article_to_podcast.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article-to-podcast
-Version: 0.1
+Version: 0.1.6
 Summary: CLI tool for converting articles to podcasts
 Author: Ivan Kovnatsky
 License: MIT
 Project-URL: Homepage, https://github.com/ivankovnatsky/article-to-podcast
 Project-URL: Changelog, https://github.com/ivankovnatsky/article-to-podcast/releases
 Project-URL: Issues, https://github.com/ivankovnatsky/article-to-podcast/issues
 Project-URL: CI, https://github.com/ivankovnatsky/article-to-podcast/actions
@@ -22,33 +22,32 @@
 Requires-Dist: lxml[html_clean]
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: cogapp; extra == "test"
 
 # Article to Podcast
 
+[![PyPI](https://img.shields.io/pypi/v/ospeak.svg)](https://pypi.org/project/article-to-podcast/)
 [![Changelog](https://img.shields.io/github/release/ivankovnatsky/article-to-podcast.svg)](https://github.com/ivankovnatsky/article-to-podcast/releases)
-[![Tests](https://github.com/ivankovnatsky/article-to-podcast/actions/workflows/test.yml/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions)
+[![Tests](https://github.com/ivankovnatsky/article-to-podcast/workflows/Test/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/github/license/ivankovnatsky/article-to-podcast)](https://github.com/ivankovnatsky/article-to-podcast/blob/main/LICENSE.md)
 
 CLI tool for converting articles to podcasts using OpenAI's Text-to-Speech API.
 
-## Development
+## Usage
 
-If you're using Nix you can start running the tool by entering:
+Install article-to-podcast with:
 
 ```console
-nix develop
+pipx install article-to-podcast
 ```
 
-## Usage
-
 ```console
-python -m article_to_podcast --help                                                                                                                   
-Usage: python -m article_to_podcast [OPTIONS]
+article-to-podcast --help                                                                                                                   
+Usage: article-to-podcast [OPTIONS]
 
 Options:
   --url TEXT                      URL of the article to be fetched.
                                   [required]
   --directory DIRECTORY           Directory where the output audio file will
                                   be saved. The filename will be derived from
                                   the article title.  [required]
@@ -70,19 +69,28 @@
                                   tone and audience. The current voices are
                                   optimized for English.
   --help                          Show this message and exit.
 ```
 
 ```console
 export OPENAI_API_KEY="your-api-key"
-python \
-    -m article_to_podcast \
-    --directory . \
+article-to-podcast \
     --url 'https://blog.kubetools.io/kopylot-an-ai-powered-kubernetes-assistant-for-devops-developers'
+```
 
+## Development
+
+If you're using Nix you can start running the tool by entering:
+
+```console
+nix develop
+```
+
+```console
+export OPENAI_API_KEY="your-api-key"
 python \
     -m article_to_podcast \
     --model tts-1-hd \
     --voice nova \
     --directory . \
     --url 'https://blog.kubetools.io/kopylot-an-ai-powered-kubernetes-assistant-for-devops-developers'
 ```
```

### Comparing `article_to_podcast-0.1/pyproject.toml` & `article_to_podcast-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "article-to-podcast"
-version = "0.1"
+version = "0.1.6"
 description = "CLI tool for converting articles to podcasts"
 readme = "README.md"
 authors = [{name = "Ivan Kovnatsky"}]
 license = {text = "MIT"}
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: MIT License"
```

### Comparing `article_to_podcast-0.1/tests/test_main.py` & `article_to_podcast-0.1.6/tests/test_main.py`

 * *Files identical despite different names*

