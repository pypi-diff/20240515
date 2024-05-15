# Comparing `tmp/nuitka_winsvc-2.2.1.tar.gz` & `tmp/Nuitka_winsvc-2.2.2-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuitka_winsvc-2.2.1.tar", last modified: Mon May  6 03:09:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

