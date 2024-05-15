# Comparing `tmp/annobee-0.5.6.tar.gz` & `tmp/annobee-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annobee-0.5.6.tar", last modified: Wed May 15 11:02:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

