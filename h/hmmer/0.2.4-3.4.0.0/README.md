# Comparing `tmp/hmmer-0.2.4.tar.gz` & `tmp/hmmer-3.4.0.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer-0.2.4.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

