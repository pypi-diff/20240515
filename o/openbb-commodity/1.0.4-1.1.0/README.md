# Comparing `tmp/openbb_commodity-1.0.4.tar.gz` & `tmp/openbb_commodity-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_commodity-1.0.4.tar", max compression
+gzip compressed data, was "openbb_commodity-1.1.0.tar", max compression
```

## Comparing `openbb_commodity-1.0.4.tar` & `openbb_commodity-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      459 2024-04-17 12:33:20.497645 openbb_commodity-1.0.4/README.md
--rw-r--r--   0        0        0       34 2024-04-17 12:33:20.497645 openbb_commodity-1.0.4/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-17 12:33:20.497645 openbb_commodity-1.0.4/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0      470 2024-04-19 17:04:46.316050 openbb_commodity-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_commodity-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      332 2024-05-15 14:27:23.324681 openbb_commodity-1.1.0/README.md
+-rw-r--r--   0        0        0       34 2024-04-23 10:22:39.591940 openbb_commodity-1.1.0/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-23 10:22:39.592095 openbb_commodity-1.1.0/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0      496 2024-05-15 16:04:09.706991 openbb_commodity-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 openbb_commodity-1.1.0/PKG-INFO
```

### Comparing `openbb_commodity-1.0.4/openbb_commodity/commodity_router.py` & `openbb_commodity-1.1.0/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

