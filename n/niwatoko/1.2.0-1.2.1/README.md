# Comparing `tmp/niwatoko-1.2.0.tar.gz` & `tmp/niwatoko-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.2.0.tar", last modified: Tue May 14 11:17:52 2024, max compression
+gzip compressed data, was "niwatoko-1.2.1.tar", last modified: Wed May 15 02:33:44 2024, max compression
```

## Comparing `niwatoko-1.2.0.tar` & `niwatoko-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.172196 niwatoko-1.2.0/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.2.0/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-14 11:17:52.172018 niwatoko-1.2.0/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-14 05:32:42.000000 niwatoko-1.2.0/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.163630 niwatoko-1.2.0/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.2.0/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16743 2024-05-14 10:37:30.000000 niwatoko-1.2.0/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.159933 niwatoko-1.2.0/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.159971 niwatoko-1.2.0/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.165028 niwatoko-1.2.0/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.2.0/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2266 2024-05-14 05:32:42.000000 niwatoko-1.2.0/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.165306 niwatoko-1.2.0/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.2.0/niwatoko/grammar/system.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-14 05:32:42.000000 niwatoko-1.2.0/niwatoko/temp.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.164573 niwatoko-1.2.0/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-14 11:17:52.000000 niwatoko-1.2.0/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-14 11:17:52.000000 niwatoko-1.2.0/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-14 11:17:52.000000 niwatoko-1.2.0/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-14 11:17:52.000000 niwatoko-1.2.0/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       56 2024-05-14 11:17:52.000000 niwatoko-1.2.0/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-14 11:17:52.000000 niwatoko-1.2.0/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-14 11:17:52.172234 niwatoko-1.2.0/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1741 2024-05-14 10:25:58.000000 niwatoko-1.2.0/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.167132 niwatoko-1.2.0/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.2.0/tests/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.2.0/tests/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.2.0/tests/test_compiler.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.2.0/tests/test_compiler.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.2.0/tests/test_compiler_v1_2.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-14 11:17:52.171565 niwatoko-1.2.0/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.2.0/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-14 05:32:42.000000 niwatoko-1.2.0/tests/test_docs/output copy.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-14 05:32:42.000000 niwatoko-1.2.0/tests/test_docs/output.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-14 05:32:42.000000 niwatoko-1.2.0/tests/test_docs/output.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-14 05:32:42.000000 niwatoko-1.2.0/tests/test_docs/output_.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.2.0/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.2.0/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.2.0/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.2.0/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.2.0/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.2.0/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.2.0/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.2.0/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-14 05:32:42.000000 niwatoko-1.2.0/tests/test_docs/test_import_function.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.2.0/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.2.0/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.845672 niwatoko-1.2.1/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.2.1/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-15 02:33:44.845385 niwatoko-1.2.1/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-14 05:32:42.000000 niwatoko-1.2.1/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.838283 niwatoko-1.2.1/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.2.1/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    22591 2024-05-14 20:12:57.000000 niwatoko-1.2.1/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.836688 niwatoko-1.2.1/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.836726 niwatoko-1.2.1/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.839754 niwatoko-1.2.1/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.2.1/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2266 2024-05-14 05:32:42.000000 niwatoko-1.2.1/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.839982 niwatoko-1.2.1/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.2.1/niwatoko/grammar/system.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-14 05:32:42.000000 niwatoko-1.2.1/niwatoko/temp.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.839166 niwatoko-1.2.1/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-15 02:33:44.000000 niwatoko-1.2.1/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-15 02:33:44.000000 niwatoko-1.2.1/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-15 02:33:44.000000 niwatoko-1.2.1/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-15 02:33:44.000000 niwatoko-1.2.1/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       80 2024-05-15 02:33:44.000000 niwatoko-1.2.1/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-15 02:33:44.000000 niwatoko-1.2.1/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-15 02:33:44.845706 niwatoko-1.2.1/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1775 2024-05-14 20:22:16.000000 niwatoko-1.2.1/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.841745 niwatoko-1.2.1/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.2.1/tests/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.2.1/tests/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.2.1/tests/test_compiler.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.2.1/tests/test_compiler.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.2.1/tests/test_compiler_v1_2.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 02:33:44.845041 niwatoko-1.2.1/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.2.1/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-14 05:32:42.000000 niwatoko-1.2.1/tests/test_docs/output copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-14 05:32:42.000000 niwatoko-1.2.1/tests/test_docs/output.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-14 05:32:42.000000 niwatoko-1.2.1/tests/test_docs/output.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-14 05:32:42.000000 niwatoko-1.2.1/tests/test_docs/output_.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.2.1/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.2.1/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.2.1/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.2.1/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.2.1/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.2.1/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.2.1/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.2.1/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-14 05:32:42.000000 niwatoko-1.2.1/tests/test_docs/test_import_function.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.2.1/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.2.1/tests/test_parser.py
```

### Comparing `niwatoko-1.2.0/LICENSE` & `niwatoko-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/PKG-INFO` & `niwatoko-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.2.0
+Version: 1.2.1
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.2.0/README.md` & `niwatoko-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/niwatoko/cli.py` & `niwatoko-1.2.1/niwatoko/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,43 +7,50 @@
 import niwatoko
 import re
 from tqdm import tqdm
 import itertools
 import threading
 import sys
 import time
+import base64
+import vertexai
+from vertexai.generative_models import GenerativeModel, Part, FinishReason
+import vertexai.preview.generative_models as generative_models
 
 @click.command()
 @click.argument('file_path', type=click.Path(exists=True), required=False)
-@click.option('-m', '--model', type=click.Choice(['openai', 'openai-gpt4o', 'claude', 'claude-sonnet', 'claude-opus', 'claude-haiku']), default='claude-haiku', help='使用するモデルを選択します。')
+@click.option('-m', '--model', type=click.Choice(['openai', 'openai-gpt4o', 'claude', 'claude-sonnet', 'claude-opus', 'claude-haiku', 'gemini-1.5-pro', 'gemini-1.5-flash']), default='claude-haiku', help='使用するモデルを選択します。')
+@click.option('-mii', '--model-input-image', type=click.Choice(['openai-gpt4o', 'gemini-1.5-pro', 'gemini-1.5-flash']), default='openai-gpt4o', help='使用する画像入力モデルを選択します。')
+# @click.option('-miv', '--model-input-video', type=click.Path(exists=True), help='動画ファイルのパスを指定します。')
 @click.option('-o', '--output', type=click.Path(), help='生成されたコードの出力先ファイルを指定します。')
 @click.option('-v', '--version',  is_flag=True, help='バージョン情報を表示します。')
 
-def main(file_path, model, output, version):
+def main(file_path, model, model_input_image, output, version):
     # print("file_path:", file_path)
     """
     自然言語のソースコードを読み込んで実行するコマンドラインインターフェース。
 
     Args:
         file_path (str): 自然言語のソースコードが書かれたファイルのパス。
         model (str): 使用するモデル（OpenAIまたはClaude）。
+        model_input_image (str): 使用する画像入力モデル。
         output (str): 生成されたコードの出力先ファイルのパス。
         version (bool): バージョン情報を表示するかどうか。
     """
     if version:
         try:
             print(f"niwatoko version: {niwatoko.__version__}")
         except AttributeError:
             print("バージョン情報がniwatokoモジュールに存在しません。")
         return
     if not file_path:
         print("ファイルパスが指定されていません。")
         return
 
-    processed_content = process_imports(file_path)
+    processed_content = process_imports(file_path, model_input_image)
 
     print("実行中... (Processing...)")
 
     # ぐるぐるアニメーションを表示するスレッドを開始
     done = False
     spinner = threading.Thread(target=spin, args=(lambda: done,))
     spinner.start()
@@ -57,14 +64,19 @@
         )
     elif model == 'openai-gpt4o':
         generated_code = gpt_generate_response_gpt4o(
             prompt=processed_content,
             max_tokens=2048,
             temperature=0.5,
         )
+    elif model in ['gemini-1.5-pro', 'gemini-1.5-flash']:
+        generated_code = generate_gemini_response(
+            model=model,
+            prompt=processed_content,
+        )
     else:
         if model == 'claude-sonnet':
             claude_model = 'claude-3-sonnet-20240229'
         elif model == 'claude-opus':
             claude_model = 'claude-3-opus-20240229'
         else:
             claude_model = 'claude-3-haiku-20240307'  # デフォルトはhaiku
@@ -72,14 +84,16 @@
         print("model:", claude_model)
         generated_code = generate_response(
             model=claude_model,
             prompt=processed_content,
             max_tokens=4000,
             temperature=0.2,
         )
+    
+
     # ぐるぐるアニメーションを停止
     done = True
     spinner.join()
 
     if output:
         with open(output, 'w', encoding = "utf-8") as file:
             file.write(generated_code)
@@ -97,15 +111,15 @@
             break
         sys.stdout.write(f'\r{c}')
         sys.stdout.flush()
         time.sleep(0.1)
     sys.stdout.write('\rDone!     \n')
 
 import os
-def process_imports(file_path):
+def process_imports(file_path, model_input_image):
     with open(file_path, 'r', encoding='utf-8') as file:
         lines = file.readlines()
     
     output = []
     for line in lines:
         output.extend(process_variable_imports(line))
         if line.startswith('- '):
@@ -139,19 +153,19 @@
                     # ブラケットで囲まれたパスを抽出
                     path_within_brackets = import_path[1:-1]
                     # print("ブラケット内のパス:", path_within_brackets)  # デバッグ用print
                     # 拡張子を取得
                     extension = path_within_brackets.split('.')[-1]
                     # print("拡張子:", extension)  # デバッグ用print
                     if extension in ['png', 'jpg', 'jpeg', 'gif']:
-                        print("画像ファイルとして処理")  # デバッグ用print
-                        output.extend(process_image_import(import_path, line))
+                        output.extend(process_image_import(import_path, model_input_image, line))
+
                     elif extension in ['mp4', 'mov', 'avi']:
                         print("動画ファイルとして処理")  # デバッグ用print
-                        output.extend(process_video_import(import_path, line))
+                        output.extend(process_video_import(import_path, model_input_image, line))
                     # 拡張子が指定されていない場合、新しい関数を使用して処理
                     else:
                         # print("拡張子が指定されていないため、process_no_extension_importを使用")  # デバッグ用print
                         output.extend(process_no_extension_import(import_path, line))
             else:
                 output.append(line)
         else:
@@ -254,42 +268,53 @@
         list: 処理後の出力行のリスト
     """
     extension = import_path.split('[')[0].strip()  # 文字列の一番左から [ の一文字前までを拡張子として取得
     import_path = import_path.split('[')[1].split(']')[0].strip() + '.' + extension  # [ と ] の間にあるパスに拡張子を追加
     import_content = get_file_content(import_path)
     return [line, f'```{extension}\n', import_content, '```\n']
 
-def process_image_import(import_path, line):
+def process_image_import(import_path, model_input_image, line):
     """
     画像ファイルのインポートを処理する関数
 
     Args:
         import_path (str): インポートするファイルのパス
         line (str): インポート文の行
 
     Returns:
         list: 処理後の出力行のリスト
     """
     import_path = import_path[1:-1]
-    recognized_text = recognize_image_text(import_path)
+    if model_input_image == 'openai-gpt4o':
+        recognized_text = recognize_image_text_gpt4o(import_path)
+    elif model_input_image in ['gemini-1.5-pro', 'gemini-1.5-flash']:
+        recognized_text = recognize_image_text_gemini(model_input_image, import_path)
+    else:
+        recognized_text = "指定された画像入力モデルがサポートされていません。"
     return [line, '```\n', recognized_text, '```\n']
 
-def process_video_import(import_path, line):
+def process_video_import(import_path, model_input_image, line):
     """
     動画ファイルのインポートを処理する関数
 
     Args:
         import_path (str): インポートするファイルのパス
         line (str): インポート文の行
 
     Returns:
         list: 処理後の出力行のリスト
     """
+
     import_path = import_path[1:-1]
-    recognized_text = recognize_video_text(import_path)
+    if model_input_image == 'openai-gpt4o':
+        recognized_text = recognize_video_text_gpt4o(import_path)
+    elif model_input_image in ['gemini-1.5-pro', 'gemini-1.5-flash']:
+        recognized_text = recognize_video_text_gemini(model_input_image, import_path)
+    else:
+        recognized_text = "指定された動画入力モデルがサポートされていません。"
     return [line, '```\n', recognized_text, '```\n']
 
 def get_file_content(file_path):
     # print(file_path)
     if os.path.isfile(file_path):
         with open(file_path, 'rb') as file:
             return file.read().decode('utf-8')
@@ -298,29 +323,37 @@
         # print(error_message)
         raise FileNotFoundError(error_message)
 
 import base64
 import requests
 
 # OpenAI API Key
-api_key = os.getenv("OPENAI_API_KEY", "YOUR_OPENAI_API_KEY")
+from dotenv import load_dotenv
+
+# .envファイルから環境変数を読み込む
+load_dotenv()
+
+# OpenAI APIキーを環境変数から取得
+api_key = os.getenv("OPENAI_API_KEY")
+if not api_key:
+    raise ValueError("OpenAI APIキーが設定されていません。")
 def encode_image(image_path):
     """
     画像ファイルをBase64エンコードする関数
 
     Args:
         image_path (str): 画像ファイルのパス
 
     Returns:
         str: Base64エンコードされた画像データ
     """
     with open(image_path, "rb") as image_file:
         return base64.b64encode(image_file.read()).decode('utf-8')
 
-def recognize_image_text(image_path):
+def recognize_image_text_gpt4o(image_path):
     """
     画像ファイルからテキストを認識する関数
 
     Args:
         image_path (str): 画像ファイルのパス
 
     Returns:
@@ -358,22 +391,20 @@
     response = requests.post("https://api.openai.com/v1/chat/completions", headers=headers, json=payload)
     content = response.json().get('choices', [{}])[0].get('message', {}).get('content', '')
     print(content)
     print('')
 
     return content
 
-
-
 import cv2
 from moviepy.editor import VideoFileClip
 import time
 import base64
 
-def recognize_video_text(video_path, seconds_per_frame=1):
+def recognize_video_text_gpt4o(video_path, seconds_per_frame=1):
     """
     動画ファイルからフレームを抽出し、テキストのサマリーを生成する関数
 
     Args:
         video_path (str): 動画ファイルのパス
         seconds_per_frame (int): フレームを抽出する間隔（秒）
 
@@ -446,7 +477,147 @@
         pbar.update(1)
     response = requests.post("https://api.openai.com/v1/chat/completions", headers=headers, json=payload)
     summary = response.json().get('choices', [{}])[0].get('message', {}).get('content', '')
     print(summary)
     print('')
 
     return summary
+
+
+
+
+
+def initialize_gemini_model(model):
+    """
+    Geminiモデルを初期化する共通関数
+
+    Args:
+        model (str): 使用するGeminiモデルの名前
+
+    Returns:
+        GenerativeModel: 初期化されたGeminiモデル
+    """
+    # model名に -review-0514 を追加
+    model = f"{model}-preview-0514"
+    
+    # 環境変数からプロジェクトとロケーションを取得
+    from dotenv import load_dotenv
+    load_dotenv()
+
+    project = os.getenv("GEMINI_PROJECT")
+    location = os.getenv("GEMINI_LOCATION")
+    
+    # Vertex AIの初期化
+    vertexai.init(project=project, location=location)
+    return GenerativeModel(model)
+
+def recognize_image_text_gemini(model, image_path):
+    """
+    Geminiモデルを使用して画像認識を行う関数
+
+    Args:
+        model (str): 使用するGeminiモデルの名前
+        image_path (str): 画像ファイルのパス
+
+    Returns:
+        str: 生成されたテキスト
+    """
+    model = initialize_gemini_model(model)
+
+    # 画像ファイルをBase64エンコード
+    with open(image_path, "rb") as image_file:
+        base64_image = base64.b64encode(image_file.read()).decode('utf-8')
+
+    # 画像データをPartオブジェクトとして作成
+    image1 = Part.from_data(
+        mime_type="image/jpeg",
+        data=base64.b64decode(base64_image)
+    )
+
+    # コンテンツ生成リクエストを送信
+    responses = model.generate_content(
+        [image1, """この画像について説明してください lang ja"""],
+        generation_config=generation_config,
+        safety_settings=safety_settings,
+        stream=True,
+    )
+
+    # 生成されたテキストを結合
+    generated_text = ""
+    for response in responses:
+        generated_text += response.text
+
+    return generated_text
+
+def recognize_video_text_gemini(model, video_path):
+    """
+    Geminiモデルを使用して動画認識を行う関数
+
+    Args:
+        model (str): 使用するGeminiモデルの名前
+        video_path (str): 動画ファイルのパス
+
+    Returns:
+        str: 生成されたテキスト
+    """
+    model = initialize_gemini_model(model)
+
+    # 動画ファイルをBase64エンコード
+    with open(video_path, "rb") as video_file:
+        base64_video = base64.b64encode(video_file.read()).decode('utf-8')
+
+    # 動画データをPartオブジェクトとして作成
+    video1 = Part.from_data(
+        mime_type="video/mp4",
+        data=base64.b64decode(base64_video)
+    )
+
+    # コンテンツ生成リクエストを送信
+    responses = model.generate_content(
+        [video1, """この動画について説明してください lang ja"""],
+        generation_config=generation_config,
+        safety_settings=safety_settings,
+        stream=True,
+    )
+
+    # 生成されたテキストを結合
+    generated_text = ""
+    for response in responses:
+        generated_text += response.text
+
+    return generated_text
+
+def generate_gemini_response(model, prompt):
+    """
+    Geminiモデルを使用してテキストを生成する関数
+
+    Returns:
+        str: 生成されたテキスト
+    """
+    model = initialize_gemini_model(model)
+
+    responses = model.generate_content(
+        [prompt],
+        generation_config=generation_config,
+        safety_settings=safety_settings,
+        stream=True,
+    )
+
+    generated_text = ""
+    for response in responses:
+        generated_text += response.text
+
+    return generated_text
+
+# 共通設定
+generation_config = {
+    "max_output_tokens": 8192,
+    "temperature": 1,
+    "top_p": 0.95,
+}
+
+safety_settings = {
+    generative_models.HarmCategory.HARM_CATEGORY_HATE_SPEECH: generative_models.HarmBlockThreshold.BLOCK_MEDIUM_AND_ABOVE,
+    generative_models.HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: generative_models.HarmBlockThreshold.BLOCK_MEDIUM_AND_ABOVE,
+    generative_models.HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: generative_models.HarmBlockThreshold.BLOCK_MEDIUM_AND_ABOVE,
+    generative_models.HarmCategory.HARM_CATEGORY_HARASSMENT: generative_models.HarmBlockThreshold.BLOCK_MEDIUM_AND_ABOVE,
+}
```

### Comparing `niwatoko-1.2.0/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.2.1/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.2.1/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/niwatoko/grammar/system.md` & `niwatoko-1.2.1/niwatoko/grammar/system.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.2.1/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.2.0
+Version: 1.2.1
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.2.0/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.2.1/niwatoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/setup.py` & `niwatoko-1.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.2.0',
+    version='1.2.1',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
@@ -17,14 +17,15 @@
     install_requires=[
         'streamlit',
         'gradio',
         'openai',
         'anthropic',
         'opencv-python',
         'moviepy',
+        'google-cloud-aiplatform'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: Japanese',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

### Comparing `niwatoko-1.2.0/tests/README.md` & `niwatoko-1.2.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/__init__.py` & `niwatoko-1.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_compiler.md` & `niwatoko-1.2.1/tests/test_compiler.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_compiler.py` & `niwatoko-1.2.1/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_compiler_v1_2.py` & `niwatoko-1.2.1/tests/test_compiler_v1_2.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/__init__.py` & `niwatoko-1.2.1/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/output copy.md` & `niwatoko-1.2.1/tests/test_docs/output copy.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/output.md` & `niwatoko-1.2.1/tests/test_docs/output.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/output.py` & `niwatoko-1.2.1/tests/test_docs/output.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/output_.md` & `niwatoko-1.2.1/tests/test_docs/output_.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_doc1.md` & `niwatoko-1.2.1/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_doc2.md` & `niwatoko-1.2.1/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_doc3.md` & `niwatoko-1.2.1/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.2.1/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.2.1/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.2.1/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.2.1/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.2.1/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_docs/test_import_function.md` & `niwatoko-1.2.1/tests/test_docs/test_import_function.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_interpreter.py` & `niwatoko-1.2.1/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.0/tests/test_parser.py` & `niwatoko-1.2.1/tests/test_parser.py`

 * *Files identical despite different names*

