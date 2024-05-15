# Comparing `tmp/blacknoise-0.0.5.tar.gz` & `tmp/blacknoise-0.0.6.tar.gz`

## Comparing `blacknoise-0.0.5.tar` & `blacknoise-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 blacknoise-0.0.5/.editorconfig
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 blacknoise-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 blacknoise-0.0.5/src/blacknoise/__about__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 blacknoise-0.0.5/src/blacknoise/__init__.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 blacknoise-0.0.5/src/blacknoise/_impl.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 blacknoise-0.0.5/src/blacknoise/compress.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 blacknoise-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 blacknoise-0.0.5/tests/test_blacknoise.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 blacknoise-0.0.5/tests/static/hello.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 blacknoise-0.0.5/tests/static/hello.txt.gz
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 blacknoise-0.0.5/tests/static/hello2.txt.gz
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 blacknoise-0.0.5/tests/static/hello3.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blacknoise-0.0.5/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 blacknoise-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 blacknoise-0.0.5/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 blacknoise-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 blacknoise-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 blacknoise-0.0.6/.editorconfig
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 blacknoise-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 blacknoise-0.0.6/src/blacknoise/__about__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 blacknoise-0.0.6/src/blacknoise/__init__.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 blacknoise-0.0.6/src/blacknoise/_impl.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 blacknoise-0.0.6/src/blacknoise/compress.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/test_blacknoise.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/static/hello.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/static/hello.txt.gz
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/static/hello2.txt.gz
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 blacknoise-0.0.6/tests/static/hello3.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blacknoise-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 blacknoise-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 blacknoise-0.0.6/README.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 blacknoise-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 blacknoise-0.0.6/PKG-INFO
```

### Comparing `blacknoise-0.0.5/.pre-commit-config.yaml` & `blacknoise-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.5/src/blacknoise/_impl.py` & `blacknoise-0.0.6/src/blacknoise/_impl.py`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.5/src/blacknoise/compress.py` & `blacknoise-0.0.6/src/blacknoise/compress.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import argparse
+from concurrent.futures import ThreadPoolExecutor, wait
 import gzip
 import io
+from itertools import cycle
 import os
 from pathlib import Path
 
 try:
     import brotli
 except ModuleNotFoundError:  # no cov
     brotli = None
@@ -42,84 +44,79 @@
     ".mpeg",
     ".mpg",
     ".webm",
     ".wmv",
 )
 
 
-def _write_if_smaller(path, orig_bytes, compress_bytes, algorithm, suffix, stats):
+def _write_if_smaller(path, orig_bytes, compress_bytes, algorithm, suffix):
     orig_len = len(orig_bytes)
     compress_len = len(compress_bytes)
     if compress_len < orig_len * 0.9:
         print(
             f"{path!s} has been shrinked by {algorithm} by {orig_len - compress_len} bytes to {int(100 * len(compress_bytes) / len(orig_bytes))}%"
         )
         Path(str(path) + suffix).write_bytes(compress_bytes)
-        stats[0] += orig_len
-        stats[1] += compress_len
     else:
         print(f"{path!s} has been skipped because of missing gains")
 
 
-def try_gzip(path, orig_bytes, stats):
+def try_gzip(path, orig_bytes):
     with io.BytesIO() as f:
         with gzip.GzipFile(
             filename="", mode="wb", fileobj=f, compresslevel=9, mtime=0
         ) as compress_file:
             compress_file.write(orig_bytes)
         _write_if_smaller(
             path,
             orig_bytes,
             f.getvalue(),
             "Gzip",
             ".gz",
-            stats,
         )
 
 
-def try_brotli(path, orig_bytes, stats):
+def try_brotli(path, orig_bytes):
     if not brotli:  # no cov
         return
     _write_if_smaller(
         path,
         orig_bytes,
         brotli.compress(orig_bytes),
         "Brotli",
         ".br",
-        stats,
     )
 
 
-def print_stats(stats, algorithm):
-    if stats[0]:
-        print(
-            f"{algorithm} reduced assets of size {stats[0]} by {stats[1]}, an improvement of {int(100 * stats[1] / stats[0])}%"
-        )
-
-
 def compress(root):
-    brotli_stats = [0, 0]
-    gzip_stats = [0, 0]
+    workers = os.cpu_count()
+    paths = [[] for _ in range(workers)]
+    paths_ = cycle(paths)
+
     for dir_, _dirs, files in os.walk(root):
         dir = Path(dir_)
         for filename in files:
             path = dir / filename
-            if path.suffix in SKIP_COMPRESS_EXTENSIONS:
-                # print(f"Skipping {str(path)} because of extension")
-                continue
-
-            orig_bytes = path.read_bytes()
-            try_brotli(path, orig_bytes, brotli_stats)
-            try_gzip(path, orig_bytes, gzip_stats)
+            if path.suffix not in SKIP_COMPRESS_EXTENSIONS:
+                next(paths_).append(path)
+
+    with ThreadPoolExecutor(max_workers=workers) as executor:
+        futures = [executor.submit(_compress_paths, p) for p in paths]
+        wait(futures)
 
-    print_stats(brotli_stats, "Brotli")
-    print_stats(gzip_stats, "Gzip")
     return 0
 
 
+def _compress_paths(paths):
+    for path in paths:
+        orig_bytes = path.read_bytes()
+        try_brotli(path, orig_bytes)
+        try_gzip(path, orig_bytes)
+
+
 def parse_args(args=None):
     parser = argparse.ArgumentParser()
     parser.add_argument("root", help="Path containing static files to compress")
     return parser.parse_args(args)
 
 
 if __name__ == "__main__":
```

### Comparing `blacknoise-0.0.5/tests/test_blacknoise.py` & `blacknoise-0.0.6/tests/test_blacknoise.py`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.5/LICENSE.txt` & `blacknoise-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.5/README.md` & `blacknoise-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.5/pyproject.toml` & `blacknoise-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blacknoise-0.0.5/PKG-INFO` & `blacknoise-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: blacknoise
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Documentation, https://github.com/matthiask/blacknoise#readme
 Project-URL: Issues, https://github.com/matthiask/blacknoise/issues
 Project-URL: Source, https://github.com/matthiask/blacknoise
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

