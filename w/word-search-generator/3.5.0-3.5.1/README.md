# Comparing `tmp/word-search-generator-3.5.0.tar.gz` & `tmp/word_search_generator-3.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "word-search-generator-3.5.0.tar", last modified: Fri Jul  7 18:40:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

