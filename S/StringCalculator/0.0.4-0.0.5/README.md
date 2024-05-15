# Comparing `tmp/StringCalculator-0.0.4.tar.gz` & `tmp/StringCalculator-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\StringCalculator-0.0.4.tar", last modified: Tue Jun  2 14:27:23 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

