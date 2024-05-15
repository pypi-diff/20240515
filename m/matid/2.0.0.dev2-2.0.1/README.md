# Comparing `tmp/matid-2.0.0.dev2.tar.gz` & `tmp/matid-2.0.1-cp311-cp311-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matid-2.0.0.dev2.tar", last modified: Wed Jan 17 08:52:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

