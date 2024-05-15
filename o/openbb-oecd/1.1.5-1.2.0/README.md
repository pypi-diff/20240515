# Comparing `tmp/openbb_oecd-1.1.5.tar.gz` & `tmp/openbb_oecd-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_oecd-1.1.5.tar", max compression
+gzip compressed data, was "openbb_oecd-1.2.0.tar", max compression
```

## Comparing `openbb_oecd-1.1.5.tar` & `openbb_oecd-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/README.md
--rw-r--r--   0        0        0      981 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8810 2024-04-17 12:33:20.685645 openbb_oecd-1.1.5/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0      485 2024-04-19 16:42:30.271413 openbb_oecd-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 openbb_oecd-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      297 2024-05-15 14:29:02.754868 openbb_oecd-1.2.0/README.md
+-rw-r--r--   0        0        0     1145 2024-05-14 15:30:05.617681 openbb_oecd-1.2.0/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-04-08 12:02:16.665635 openbb_oecd-1.2.0/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-04-08 12:02:16.665758 openbb_oecd-1.2.0/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-04-08 12:02:16.665882 openbb_oecd-1.2.0/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-04-08 12:02:16.665998 openbb_oecd-1.2.0/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-04-08 12:02:16.666084 openbb_oecd-1.2.0/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-04-08 12:02:16.666136 openbb_oecd-1.2.0/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-04-08 12:02:16.666230 openbb_oecd-1.2.0/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-04-08 12:02:16.666349 openbb_oecd-1.2.0/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-04-23 10:22:39.676912 openbb_oecd-1.2.0/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0      511 2024-05-15 16:06:20.543758 openbb_oecd-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 openbb_oecd-1.2.0/PKG-INFO
```

### Comparing `openbb_oecd-1.1.5/openbb_oecd/models/composite_leading_indicator.py` & `openbb_oecd-1.2.0/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.5/openbb_oecd/models/gdp_forecast.py` & `openbb_oecd-1.2.0/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.5/openbb_oecd/models/gdp_nominal.py` & `openbb_oecd-1.2.0/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.5/openbb_oecd/models/gdp_real.py` & `openbb_oecd-1.2.0/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.5/openbb_oecd/models/long_term_interest_rate.py` & `openbb_oecd-1.2.0/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.5/openbb_oecd/models/short_term_interest_rate.py` & `openbb_oecd-1.2.0/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.5/openbb_oecd/models/unemployment.py` & `openbb_oecd-1.2.0/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.5/openbb_oecd/utils/constants.py` & `openbb_oecd-1.2.0/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.5/openbb_oecd/utils/helpers.py` & `openbb_oecd-1.2.0/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

