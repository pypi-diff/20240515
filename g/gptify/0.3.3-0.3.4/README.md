# Comparing `tmp/gptify-0.3.3.tar.gz` & `tmp/gptify-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptify-0.3.3.tar", max compression
+gzip compressed data, was "gptify-0.3.4.tar", max compression
```

## Comparing `gptify-0.3.3.tar` & `gptify-0.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1234 2024-05-02 05:16:24.293395 gptify-0.3.3/README.md
--rw-r--r--   0        0        0      319 2024-05-02 05:16:24.293395 gptify-0.3.3/gptify/.gptignore
--rw-r--r--   0        0        0        0 2024-05-02 05:16:24.293395 gptify-0.3.3/gptify/__init__.py
--rw-r--r--   0        0        0      201 2024-05-02 05:16:24.293395 gptify-0.3.3/gptify/cli.py
--rw-r--r--   0        0        0     4665 2024-05-02 05:16:24.293395 gptify-0.3.3/gptify/gpt_repository_loader.py
--rw-r--r--   0        0        0      465 2024-05-02 05:16:24.293395 gptify-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 gptify-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1234 2024-05-15 05:42:52.225065 gptify-0.3.4/README.md
+-rw-r--r--   0        0        0      334 2024-05-15 05:42:52.225065 gptify-0.3.4/gptify/.gptignore
+-rw-r--r--   0        0        0        0 2024-05-15 05:42:52.225065 gptify-0.3.4/gptify/__init__.py
+-rw-r--r--   0        0        0      201 2024-05-15 05:42:52.225065 gptify-0.3.4/gptify/cli.py
+-rw-r--r--   0        0        0     4701 2024-05-15 05:42:52.225065 gptify-0.3.4/gptify/gpt_repository_loader.py
+-rw-r--r--   0        0        0      465 2024-05-15 05:42:52.225065 gptify-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 gptify-0.3.4/PKG-INFO
```

### Comparing `gptify-0.3.3/README.md` & `gptify-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `gptify-0.3.3/gptify/gpt_repository_loader.py` & `gptify-0.3.4/gptify/gpt_repository_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,37 +55,42 @@
     parser.add_argument(
         "--clipboard", help="copy the output to the clipboard", action="store_true"
     )
     parser.add_argument(
         "--openfile", help="open output file after creation", action="store_true"
     )
     parser.add_argument(
-        "--output", help="path to save output file", type=str, default="gptify_output.txt", nargs="?"
+        "--output",
+        help="path to save output file",
+        type=str,
+        default="gptify_output.txt",
+        nargs="?",
     )
     parser.add_argument(
         "--write-config",
         help="Write a default config file to the target directory.",
         type=str,
         nargs="?",
     )
     args = parser.parse_args()
 
     repo_path = args.repo_path or os.getcwd()
     ignore_file_path = os.path.join(repo_path, ".gptignore")
+
     if sys.platform == "win32":
         ignore_file_path = ignore_file_path.replace("/", "\\")
 
     if not os.path.exists(ignore_file_path):
         # try and use the .gptignore file in the current directory as a fallback.
         ignore_file_path = os.path.join(HERE, ".gptignore")
         assert os.path.exists(ignore_file_path)
         with open(ignore_file_path, "r") as ignore_file:
-           contents = ignore_file.read()
+            contents = ignore_file.read()
         with open(ignore_file_path, "w") as ignore_file:
-           ignore_file.write(contents)
+            ignore_file.write(contents)
 
     preamble_file = args.preamble
     if os.path.exists(ignore_file_path):
         ignore_list = get_ignore_list(ignore_file_path)
     else:
         ignore_list = []
     outfile = os.path.abspath(args.output)
```

### Comparing `gptify-0.3.3/PKG-INFO` & `gptify-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptify
-Version: 0.3.3
+Version: 0.3.4
 Summary: Convert code repos into an LLM prompt-friendly format. Forked from https://github.com/zackees/gptrepo
 Author: Wilder Lopes
 Author-email: wilder@ogre.run
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

