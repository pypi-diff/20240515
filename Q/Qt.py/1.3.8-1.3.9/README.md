# Comparing `tmp/Qt.py-1.3.8.tar.gz` & `tmp/Qt.py-1.3.9-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Qt.py-1.3.8.tar", last modified: Mon Feb 13 07:28:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

