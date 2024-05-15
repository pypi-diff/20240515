# Comparing `tmp/ASCA-1.1.tar.gz` & `tmp/ASCA-1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCA-1.1.tar", last modified: Wed May 15 15:52:40 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

