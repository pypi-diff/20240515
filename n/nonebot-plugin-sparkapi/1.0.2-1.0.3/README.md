# Comparing `tmp/nonebot_plugin_sparkapi-1.0.2.tar.gz` & `tmp/nonebot_plugin_sparkapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sparkapi-1.0.2.tar", last modified: Wed May 15 13:19:33 2024, max compression
+gzip compressed data, was "nonebot_plugin_sparkapi-1.0.3.tar", last modified: Wed May 15 13:21:47 2024, max compression
```

## Comparing `nonebot_plugin_sparkapi-1.0.2.tar` & `nonebot_plugin_sparkapi-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 13:19:33.095052 nonebot_plugin_sparkapi-1.0.2/
--rw-rw-rw-   0        0        0     1084 2024-05-15 03:42:49.000000 nonebot_plugin_sparkapi-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     6492 2024-05-15 13:19:33.094038 nonebot_plugin_sparkapi-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4744 2024-05-15 12:25:00.000000 nonebot_plugin_sparkapi-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 13:19:33.088037 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/
--rw-rw-rw-   0        0        0     4397 2024-05-15 02:01:14.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/SparkApi.py
--rw-rw-rw-   0        0        0     7224 2024-05-15 11:52:10.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/__init__.py
--rw-rw-rw-   0        0        0     1193 2024-05-15 10:08:12.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/config.py
--rw-rw-rw-   0        0        0     1987 2024-05-15 11:56:48.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/data.py
--rw-rw-rw-   0        0        0     1731 2024-05-15 02:00:58.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/funcs.py
-drwxrwxrwx   0        0        0        0 2024-05-15 13:19:33.093037 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi.egg-info/
--rw-rw-rw-   0        0        0     6492 2024-05-15 13:19:33.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-05-15 13:19:33.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 13:19:33.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-05-15 13:19:33.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-15 13:19:33.000000 nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      649 2024-05-15 13:19:28.000000 nonebot_plugin_sparkapi-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 13:19:33.095052 nonebot_plugin_sparkapi-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 13:21:47.520990 nonebot_plugin_sparkapi-1.0.3/
+-rw-rw-rw-   0        0        0     1084 2024-05-15 03:42:49.000000 nonebot_plugin_sparkapi-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6495 2024-05-15 13:21:47.519989 nonebot_plugin_sparkapi-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4744 2024-05-15 12:25:00.000000 nonebot_plugin_sparkapi-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 13:21:47.514073 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/
+-rw-rw-rw-   0        0        0     4397 2024-05-15 02:01:14.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/SparkApi.py
+-rw-rw-rw-   0        0        0     7224 2024-05-15 11:52:10.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/__init__.py
+-rw-rw-rw-   0        0        0     1193 2024-05-15 10:08:12.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/config.py
+-rw-rw-rw-   0        0        0     1987 2024-05-15 11:56:48.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/data.py
+-rw-rw-rw-   0        0        0     1731 2024-05-15 02:00:58.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/funcs.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:21:47.518994 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi.egg-info/
+-rw-rw-rw-   0        0        0     6495 2024-05-15 13:21:47.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-05-15 13:21:47.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 13:21:47.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-15 13:21:47.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-15 13:21:47.000000 nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2024-05-15 13:21:42.000000 nonebot_plugin_sparkapi-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 13:21:47.520990 nonebot_plugin_sparkapi-1.0.3/setup.cfg
```

### Comparing `nonebot_plugin_sparkapi-1.0.2/LICENSE` & `nonebot_plugin_sparkapi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.2/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.0.2
-Summary: Nonebot2 ChatBot that calls the official API of the KDDI Spark LLM for all model versions, defaulting to the current latest (v3.5)
+Version: 1.0.3
+Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.2 Summary:
-Nonebot2 ChatBot that calls the official API of the KDDI Spark LLM for all
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.3 Summary:
+Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `nonebot_plugin_sparkapi-1.0.2/README.md` & `nonebot_plugin_sparkapi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/SparkApi.py` & `nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/SparkApi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/__init__.py` & `nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/config.py` & `nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/data.py` & `nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi/funcs.py` & `nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi/funcs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.2/nonebot_plugin_sparkapi.egg-info/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.3/nonebot_plugin_sparkapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.0.2
-Summary: Nonebot2 ChatBot that calls the official API of the KDDI Spark LLM for all model versions, defaulting to the current latest (v3.5)
+Version: 1.0.3
+Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.2 Summary:
-Nonebot2 ChatBot that calls the official API of the KDDI Spark LLM for all
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.3 Summary:
+Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `nonebot_plugin_sparkapi-1.0.2/pyproject.toml` & `nonebot_plugin_sparkapi-1.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "nonebot_plugin_sparkapi"
-version = "1.0.2"
-description = "Nonebot2 ChatBot that calls the official API of the KDDI Spark LLM for all model versions, defaulting to the current latest (v3.5)"
+version = "1.0.3"
+description = "Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)"
 authors = [
     { name = "CCLMSY", email = "2502408581@qq.com" }
 ]
 dependencies = [
     "nonebot2 >=2.0.0rc3, <3.0.0",
     "nonebot-adapter-onebot >=2.2.1, <3.0.0",
     "websocket-client >=1.6.1, <2.0.0"
```

