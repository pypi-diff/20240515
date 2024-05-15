# Comparing `tmp/podgenai-0.1.2.tar.gz` & `tmp/podgenai-0.1.3.tar.gz`

## Comparing `podgenai-0.1.2.tar` & `podgenai-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 podgenai-0.1.2/.python-version
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.2/requirements-dev.lock
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.2/requirements.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/__init__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/__main__.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/config.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/exceptions.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/podgenai.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/work.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/content/audio.py
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/content/subtopics.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/content/topic.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/content/tts.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/content/voice.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/prompts/continuation_first.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/prompts/continuation_next.txt
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/prompts/generate_subtopic.txt
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/prompts/list_subtopics.txt
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/prompts/select_voice.txt
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/prompts/tts_disclaimer.txt
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/util/binascii.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/util/input.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/util/openai.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/util/semantic_text_splitter.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 podgenai-0.1.2/src/podgenai/util/sys.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 podgenai-0.1.2/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 podgenai-0.1.2/LICENSE
--rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 podgenai-0.1.2/README.md
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 podgenai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 podgenai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 podgenai-0.1.3/.python-version
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.3/requirements-dev.lock
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.3/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/__init__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/__main__.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/config.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/exceptions.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/podgenai.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/work.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/content/audio.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/content/subtopics.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/content/topic.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/content/tts.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/content/voice.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/prompts/continuation_first.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/prompts/continuation_next.txt
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/prompts/generate_subtopic.txt
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/prompts/list_subtopics.txt
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/prompts/select_voice.txt
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/prompts/tts_disclaimer.txt
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/util/binascii.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/util/input.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/util/openai.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/util/semantic_text_splitter.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 podgenai-0.1.3/src/podgenai/util/sys.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 podgenai-0.1.3/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 podgenai-0.1.3/LICENSE
+-rw-r--r--   0        0        0     9682 2020-02-02 00:00:00.000000 podgenai-0.1.3/README.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 podgenai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 podgenai-0.1.3/PKG-INFO
```

### Comparing `podgenai-0.1.2/requirements-dev.lock` & `podgenai-0.1.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/requirements.lock` & `podgenai-0.1.3/requirements.lock`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/__main__.py` & `podgenai-0.1.3/src/podgenai/__main__.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/config.py` & `podgenai-0.1.3/src/podgenai/config.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/podgenai.py` & `podgenai-0.1.3/src/podgenai/podgenai.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/work.py` & `podgenai-0.1.3/src/podgenai/work.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/content/audio.py` & `podgenai-0.1.3/src/podgenai/content/audio.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/content/subtopics.py` & `podgenai-0.1.3/src/podgenai/content/subtopics.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/content/topic.py` & `podgenai-0.1.3/src/podgenai/content/topic.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/content/tts.py` & `podgenai-0.1.3/src/podgenai/content/tts.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/content/voice.py` & `podgenai-0.1.3/src/podgenai/content/voice.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/prompts/generate_subtopic.txt` & `podgenai-0.1.3/src/podgenai/prompts/generate_subtopic.txt`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/prompts/list_subtopics.txt` & `podgenai-0.1.3/src/podgenai/prompts/list_subtopics.txt`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/util/input.py` & `podgenai-0.1.3/src/podgenai/util/input.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/src/podgenai/util/openai.py` & `podgenai-0.1.3/src/podgenai/util/openai.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/.gitignore` & `podgenai-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/LICENSE` & `podgenai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.2/README.md` & `podgenai-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,31 @@
 | Emotive | [Living a good life](https://mega.nz/file/NNMUFTJT#8ga2REaZaT79-zf83KqBT2tUW8Q8j5sT0WAuxQUEpQ8)                                               | Emotive voice selection                                           |
 | Default | [Artificial General Intelligence (AGI): Approaches and Algorithms](https://mega.nz/file/0JkWnDQQ#PSUA5aj0q_yU18T4XsazYZoSG9bqjUi7vCLmjVrY1IA) | Non-hierarchical flattened single-level subtopic list enforcement |
 | Female  | [Human circulatory system (unabridged)](https://mega.nz/file/UYt2WLDA#4q-UI8cWffzN0PG8ZGiQK_96dudklBJOfFmpE_3for4)                            | Implicit topic support for unabridged suffix                      |
 | Female  | [Buffy the Vampire Slayer](https://mega.nz/file/FddQWRJb#q_3XoTfgsQIvU6oZcJK7Y9or4Tjcx7BK2YLf_whjH4g)                                         | Female voice selection                                            |
 | Male    | [Bitcoin for nerds](https://mega.nz/file/QVNyWYrZ#RqKuAcG6LUwOZi20ZBkygRNin9f7rpLBm1xsoILoAFI)                                                | Male voice selection                                              |
 
 ## Setup
+* In the working directory, create a file named `.env`, with the intended environment variable `OPENAI_API_KEY=<your OpenAI API key>`, or set it in a different way.
+* Optionally set the environment variable `PODGENAI_OPENAI_MAX_WORKERS=32` for faster generation, with its default value being 16.
+* Ensure that `ffmpeg` is available.
+* Continue the setup via GitHub or PyPI as below.
+
+### Setup via GitHub
 * Ensure that [`rye`](https://rye-up.com/) is installed and available.
 * Clone or download this repo.
 * In the repo directory, run `rye sync` or more narrowly just `rye sync --no-lock` if on Linux.
-* In the repo directory, create a file named `.env`, with the intended environment variable `OPENAI_API_KEY=<your OpenAI API key>`, or set it in a different way.
-* Optionally set the environment variable `PODGENAI_OPENAI_MAX_WORKERS=32` for faster generation, with its default value being 16.
-* Ensure that `ffmpeg` is available.
 * If updating the repo, rerun the `rye sync` step.
 
+### Setup via PyPI
+* Create and activate a Python 3.12 virtual environment.
+* Install via PyPI: `pip install -U podgenai`.
+
 ## Usage
-Usage can be as a command-line application or as a Python library. By default, the generated mp3 file will be written to the repo directory. As of 2024, the estimated cost per generation is under $2 USD, more specifically under $0.10 USD per subtopic. The time taken is under three minutes.
+Usage can be as a command-line application or as a Python library. By default, the generated mp3 file will be written to the current working directory. As of 2024, the estimated cost per generation is under $2 USD, more specifically under $0.10 USD per subtopic. The time taken is under three minutes.
 
 ### Usage tips
 * If a requested topic fails to generate subtopics, try rewording it, perhaps to be broader or narrower or more factual. Up to two attempts are made, although the first attempt will use the disk cache if available.
 * For a potentially longer list of covered subtopics, consider appending the "(unabridged)" suffix to the requested topic, e.g. "PyTorch (unabridged)".
 * In case the topic fails to be spoken at the start of a podcast, delete `./work/<topic>/1.*.mp3` and regenerate the output.
 * To optionally generate a cover art image for your topic, [this custom GPT](https://chat.openai.com/g/g-SvmRhBwX1-podcast-episode-cover-art) can be used.
```

### Comparing `podgenai-0.1.2/pyproject.toml` & `podgenai-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "podgenai"
-version = "0.1.2"
+version = "0.1.3"
 description = "GPT-4 based informational audiobook/podcast mp3 generator"
 authors = [
     { name = "Ouroboros Chrysopoeia", email = "impredicative@users.noreply.github.com" }
 ]
 dependencies = [
     "fire>=0.6.0",
     "openai>=1.27.0",
@@ -43,14 +43,16 @@
 "check-fmt" = "rye fmt --check"
 fix = { chain = ["fix-lint", "fix-fmt" ] }
 "fix-lint" = "rye lint --fix"
 "fix-fmt" = "rye fmt"
 lockup = "rye lock --update-all"
 syncup = "rye sync --update-all"
 build = "rye build --clean --verbose"
+publish = "rye publish --verbose"
+release = { chain = ["build", "publish"]}
 
 [tool.hatch.build]
 exclude = [".env", "archive/", "scripts/", "work/"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

### Comparing `podgenai-0.1.2/PKG-INFO` & `podgenai-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: podgenai
-Version: 0.1.2
+Version: 0.1.3
 Summary: GPT-4 based informational audiobook/podcast mp3 generator
 Project-URL: Repository, https://github.com/impredicative/podgenai
 Author-email: Ouroboros Chrysopoeia <impredicative@users.noreply.github.com>
 License-File: LICENSE
 Keywords: GPT-4,aicast,audiobook,mp3,podcast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -48,24 +48,31 @@
 | Emotive | [Living a good life](https://mega.nz/file/NNMUFTJT#8ga2REaZaT79-zf83KqBT2tUW8Q8j5sT0WAuxQUEpQ8)                                               | Emotive voice selection                                           |
 | Default | [Artificial General Intelligence (AGI): Approaches and Algorithms](https://mega.nz/file/0JkWnDQQ#PSUA5aj0q_yU18T4XsazYZoSG9bqjUi7vCLmjVrY1IA) | Non-hierarchical flattened single-level subtopic list enforcement |
 | Female  | [Human circulatory system (unabridged)](https://mega.nz/file/UYt2WLDA#4q-UI8cWffzN0PG8ZGiQK_96dudklBJOfFmpE_3for4)                            | Implicit topic support for unabridged suffix                      |
 | Female  | [Buffy the Vampire Slayer](https://mega.nz/file/FddQWRJb#q_3XoTfgsQIvU6oZcJK7Y9or4Tjcx7BK2YLf_whjH4g)                                         | Female voice selection                                            |
 | Male    | [Bitcoin for nerds](https://mega.nz/file/QVNyWYrZ#RqKuAcG6LUwOZi20ZBkygRNin9f7rpLBm1xsoILoAFI)                                                | Male voice selection                                              |
 
 ## Setup
+* In the working directory, create a file named `.env`, with the intended environment variable `OPENAI_API_KEY=<your OpenAI API key>`, or set it in a different way.
+* Optionally set the environment variable `PODGENAI_OPENAI_MAX_WORKERS=32` for faster generation, with its default value being 16.
+* Ensure that `ffmpeg` is available.
+* Continue the setup via GitHub or PyPI as below.
+
+### Setup via GitHub
 * Ensure that [`rye`](https://rye-up.com/) is installed and available.
 * Clone or download this repo.
 * In the repo directory, run `rye sync` or more narrowly just `rye sync --no-lock` if on Linux.
-* In the repo directory, create a file named `.env`, with the intended environment variable `OPENAI_API_KEY=<your OpenAI API key>`, or set it in a different way.
-* Optionally set the environment variable `PODGENAI_OPENAI_MAX_WORKERS=32` for faster generation, with its default value being 16.
-* Ensure that `ffmpeg` is available.
 * If updating the repo, rerun the `rye sync` step.
 
+### Setup via PyPI
+* Create and activate a Python 3.12 virtual environment.
+* Install via PyPI: `pip install -U podgenai`.
+
 ## Usage
-Usage can be as a command-line application or as a Python library. By default, the generated mp3 file will be written to the repo directory. As of 2024, the estimated cost per generation is under $2 USD, more specifically under $0.10 USD per subtopic. The time taken is under three minutes.
+Usage can be as a command-line application or as a Python library. By default, the generated mp3 file will be written to the current working directory. As of 2024, the estimated cost per generation is under $2 USD, more specifically under $0.10 USD per subtopic. The time taken is under three minutes.
 
 ### Usage tips
 * If a requested topic fails to generate subtopics, try rewording it, perhaps to be broader or narrower or more factual. Up to two attempts are made, although the first attempt will use the disk cache if available.
 * For a potentially longer list of covered subtopics, consider appending the "(unabridged)" suffix to the requested topic, e.g. "PyTorch (unabridged)".
 * In case the topic fails to be spoken at the start of a podcast, delete `./work/<topic>/1.*.mp3` and regenerate the output.
 * To optionally generate a cover art image for your topic, [this custom GPT](https://chat.openai.com/g/g-SvmRhBwX1-podcast-episode-cover-art) can be used.
```

