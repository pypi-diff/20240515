# Comparing `tmp/myccc-0.1.0.tar.gz` & `tmp/myccc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myccc-0.1.0.tar", max compression
+gzip compressed data, was "myccc-0.2.0.tar", max compression
```

## Comparing `myccc-0.1.0.tar` & `myccc-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-14 20:22:27.240956 myccc-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-14 20:22:27.240956 myccc-0.1.0/myccc/__init__.py
--rw-r--r--   0        0        0      280 2024-05-14 20:25:54.657951 myccc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 myccc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-14 20:27:28.426293 myccc-0.2.0/LICENSE
+-rw-r--r--   0        0        0       10 2024-05-14 20:27:28.410293 myccc-0.2.0/README.md
+-rw-r--r--   0        0        0       54 2024-05-14 21:54:24.488540 myccc-0.2.0/myccc/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-14 22:37:05.087439 myccc-0.2.0/myccc/media.py
+-rw-r--r--   0        0        0      105 2024-05-14 22:22:04.340535 myccc-0.2.0/myccc/schedule.py
+-rw-r--r--   0        0        0      301 2024-05-15 01:23:17.432024 myccc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 myccc-0.2.0/PKG-INFO
```

