# Comparing `tmp/flashlight_text-0.0.8.dev308.tar.gz` & `tmp/flashlight_text-0.0.8.dev309-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashlight_text-0.0.8.dev308.tar", last modified: Tue May  7 11:19:21 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

