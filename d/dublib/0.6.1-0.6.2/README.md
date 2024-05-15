# Comparing `tmp/dublib-0.6.1.tar.gz` & `tmp/dublib-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dublib-0.6.1.tar", last modified: Sun May  5 08:40:29 2024, max compression
+gzip compressed data, was "dublib-0.6.2.tar", last modified: Wed May 15 19:31:44 2024, max compression
```

## Comparing `dublib-0.6.1.tar` & `dublib-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.146376 dublib-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-05 08:40:20.000000 dublib-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-05 08:40:29.146376 dublib-0.6.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1742 2024-05-05 08:40:20.000000 dublib-0.6.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-05 08:40:20.000000 dublib-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:40:29.146376 dublib-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.138376 dublib-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.142376 dublib-0.6.1/src/dublib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.142376 dublib-0.6.1/src/dublib/Exceptions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/StyledPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      680 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/TelebotUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/WebRequestor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10447 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Polyglot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/StyledPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/TelebotUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30855 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/WebRequestor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.142376 dublib-0.6.1/src/dublib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:44.376910 dublib-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-15 19:31:36.000000 dublib-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-15 19:31:44.376910 dublib-0.6.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1742 2024-05-15 19:31:36.000000 dublib-0.6.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-15 19:31:36.000000 dublib-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:31:44.376910 dublib-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:44.368910 dublib-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:44.372910 dublib-0.6.2/src/dublib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:44.372910 dublib-0.6.2/src/dublib/Exceptions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/Exceptions/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      680 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/Exceptions/TelebotUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/Exceptions/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/Exceptions/WebRequestor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/Exceptions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10447 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/Methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/Polyglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15742 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/TelebotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30855 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/WebRequestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:36.000000 dublib-0.6.2/src/dublib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:44.372910 dublib-0.6.2/src/dublib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-15 19:31:44.000000 dublib-0.6.2/src/dublib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-15 19:31:44.000000 dublib-0.6.2/src/dublib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:31:44.000000 dublib-0.6.2/src/dublib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 19:31:44.000000 dublib-0.6.2/src/dublib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:31:44.000000 dublib-0.6.2/src/dublib.egg-info/top_level.txt
```

### Comparing `dublib-0.6.1/LICENSE` & `dublib-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/PKG-INFO` & `dublib-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.6.1
+Version: 0.6.2
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `dublib-0.6.1/README.md` & `dublib-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/pyproject.toml` & `dublib-0.6.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "cython"]
 
 [project]
 name = "dublib"
-version = "0.6.1"
+version = "0.6.2"
 description = "Коллекция модулей от DUB1401."
 authors = [
 	{name = "DUB1401", email = "vlad.milosta@outlook.com"}
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `dublib-0.6.1/src/dublib/Exceptions/StyledPrinter.py` & `dublib-0.6.2/src/dublib/Exceptions/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib/Exceptions/TelebotUtils.py` & `dublib-0.6.2/src/dublib/Exceptions/TelebotUtils.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib/Exceptions/Terminalyzer.py` & `dublib-0.6.2/src/dublib/Exceptions/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib/Exceptions/WebRequestor.py` & `dublib-0.6.2/src/dublib/Exceptions/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib/Methods.py` & `dublib-0.6.2/src/dublib/Methods.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib/Polyglot.py` & `dublib-0.6.2/src/dublib/Polyglot.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib/StyledPrinter.py` & `dublib-0.6.2/src/dublib/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib/TelebotUtils.py` & `dublib-0.6.2/src/dublib/TelebotUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,23 +125,24 @@
 				IsChanged = True
 
 		# Если список разрешений изменён, отсортировать его.
 		if IsChanged: self.__Data["permissions"] = sorted(self.__Data["permissions"])
 		# Сохранение данных.
 		self.__SaveData()
 
-	def create_property(self, key: str, value: any):
+	def create_property(self, key: str, value: any, force: bool = True):
 		"""
 		Создаёт свойство пользователя и задаёт ему значение, если такового ещё не существует.
 			key – ключ свойства;
-			value – значение.
+			value – значение;
+			force – указывает, необходимо ли перезаписывать значение уже существующего ключа.
 		"""
 		
 		# Если свойства не существует.
-		if key not in self.__Data["data"].keys():
+		if key not in self.__Data["data"].keys() or force:
 			# Создание свойства.
 			self.__Data["data"][key] = value
 			# Сохранение данных.
 			self.__SaveData()
 
 	def get_property(self, key: str) -> any:
 		"""
```

### Comparing `dublib-0.6.1/src/dublib/Terminalyzer.py` & `dublib-0.6.2/src/dublib/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib/WebRequestor.py` & `dublib-0.6.2/src/dublib/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.1/src/dublib.egg-info/PKG-INFO` & `dublib-0.6.2/src/dublib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.6.1
+Version: 0.6.2
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `dublib-0.6.1/src/dublib.egg-info/SOURCES.txt` & `dublib-0.6.2/src/dublib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

