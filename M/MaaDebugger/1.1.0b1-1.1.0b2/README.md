# Comparing `tmp/maadebugger-1.1.0b1.tar.gz` & `tmp/maadebugger-1.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadebugger-1.1.0b1.tar", last modified: Wed May  8 07:09:02 2024, max compression
+gzip compressed data, was "maadebugger-1.1.0b2.tar", last modified: Wed May  8 08:05:47 2024, max compression
```

## Comparing `maadebugger-1.1.0b1.tar` & `maadebugger-1.1.0b2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-05-08 07:08:50.589925 maadebugger-1.1.0b1/LICENSE
--rw-r--r--   0        0        0      123 2024-05-08 07:08:50.589925 maadebugger-1.1.0b1/README.md
--rw-r--r--   0        0        0      478 2024-05-08 07:09:02.693932 maadebugger-1.1.0b1/pyproject.toml
--rw-r--r--   0        0        0       62 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/__main__.py
--rw-r--r--   0        0        0     4854 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/maafw/__init__.py
--rw-r--r--   0        0        0      254 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/main.py
--rw-r--r--   0        0        0      201 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/utils/__init__.py
--rw-r--r--   0        0        0      799 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/components/status_indicator.py
--rw-r--r--   0        0        0      240 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/__init__.py
--rw-r--r--   0        0        0     8775 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/master_control.py
--rw-r--r--   0        0        0     2788 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/runtime_control.py
--rw-r--r--   0        0        0      901 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/reco_page/__init__.py
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 maadebugger-1.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/LICENSE
+-rw-r--r--   0        0        0      123 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/README.md
+-rw-r--r--   0        0        0      479 2024-05-08 08:05:47.448804 maadebugger-1.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/__main__.py
+-rw-r--r--   0        0        0     4854 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/maafw/__init__.py
+-rw-r--r--   0        0        0      254 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/main.py
+-rw-r--r--   0        0        0      201 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/utils/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/components/status_indicator.py
+-rw-r--r--   0        0        0      240 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/__init__.py
+-rw-r--r--   0        0        0     8775 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/master_control.py
+-rw-r--r--   0        0        0     2788 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/runtime_control.py
+-rw-r--r--   0        0        0      901 2024-05-08 08:05:21.476698 maadebugger-1.1.0b2/src/MaaDebugger/webpage/reco_page/__init__.py
+-rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 maadebugger-1.1.0b2/PKG-INFO
```

### Comparing `maadebugger-1.1.0b1/LICENSE` & `maadebugger-1.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `maadebugger-1.1.0b1/src/MaaDebugger/maafw/__init__.py` & `maadebugger-1.1.0b2/src/MaaDebugger/maafw/__init__.py`

 * *Files identical despite different names*

### Comparing `maadebugger-1.1.0b1/src/MaaDebugger/webpage/components/status_indicator.py` & `maadebugger-1.1.0b2/src/MaaDebugger/webpage/components/status_indicator.py`

 * *Files identical despite different names*

### Comparing `maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/master_control.py` & `maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/master_control.py`

 * *Files identical despite different names*

### Comparing `maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/runtime_control.py` & `maadebugger-1.1.0b2/src/MaaDebugger/webpage/index_page/runtime_control.py`

 * *Files identical despite different names*

### Comparing `maadebugger-1.1.0b1/src/MaaDebugger/webpage/reco_page/__init__.py` & `maadebugger-1.1.0b2/src/MaaDebugger/webpage/reco_page/__init__.py`

 * *Files identical despite different names*

