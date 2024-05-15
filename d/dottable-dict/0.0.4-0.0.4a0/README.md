# Comparing `tmp/dottable_dict-0.0.4.tar.gz` & `tmp/dottable_dict-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dottable_dict-0.0.4.tar", last modified: Tue May 14 21:01:25 2024, max compression
+gzip compressed data, was "dottable_dict-0.0.4a0.tar", last modified: Wed May 15 20:29:44 2024, max compression
```

## Comparing `dottable_dict-0.0.4.tar` & `dottable_dict-0.0.4a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 21:01:25.546659 dottable_dict-0.0.4/
--rw-rw-rw-   0        0        0     1083 2024-05-11 22:16:47.000000 dottable_dict-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2717 2024-05-14 21:01:25.544654 dottable_dict-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2140 2024-05-12 00:26:48.000000 dottable_dict-0.0.4/README.md
--rw-rw-rw-   0        0        0      652 2024-05-14 21:01:04.000000 dottable_dict-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 21:01:25.547655 dottable_dict-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 21:01:25.513197 dottable_dict-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 21:01:25.526605 dottable_dict-0.0.4/src/dottable_dict/
--rw-rw-rw-   0        0        0       28 2024-05-11 23:10:12.000000 dottable_dict-0.0.4/src/dottable_dict/__init__.py
--rw-rw-rw-   0        0        0     7514 2024-05-14 20:44:16.000000 dottable_dict-0.0.4/src/dottable_dict/dottable_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:01:25.541596 dottable_dict-0.0.4/src/dottable_dict.egg-info/
--rw-rw-rw-   0        0        0     2717 2024-05-14 21:01:25.000000 dottable_dict-0.0.4/src/dottable_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-05-14 21:01:25.000000 dottable_dict-0.0.4/src/dottable_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 21:01:25.000000 dottable_dict-0.0.4/src/dottable_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 21:01:25.000000 dottable_dict-0.0.4/src/dottable_dict.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.670955 dottable_dict-0.0.4a0/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 22:16:47.000000 dottable_dict-0.0.4a0/LICENSE
+-rw-rw-rw-   0        0        0     2719 2024-05-15 20:29:44.667464 dottable_dict-0.0.4a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2140 2024-05-12 00:26:48.000000 dottable_dict-0.0.4a0/README.md
+-rw-rw-rw-   0        0        0      653 2024-05-15 20:28:32.000000 dottable_dict-0.0.4a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:29:44.671469 dottable_dict-0.0.4a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.636841 dottable_dict-0.0.4a0/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.650084 dottable_dict-0.0.4a0/src/dottable_dict/
+-rw-rw-rw-   0        0        0       28 2024-05-11 23:10:12.000000 dottable_dict-0.0.4a0/src/dottable_dict/__init__.py
+-rw-rw-rw-   0        0        0     7617 2024-05-15 20:27:54.000000 dottable_dict-0.0.4a0/src/dottable_dict/dottable_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:29:44.665470 dottable_dict-0.0.4a0/src/dottable_dict.egg-info/
+-rw-rw-rw-   0        0        0     2719 2024-05-15 20:29:44.000000 dottable_dict-0.0.4a0/src/dottable_dict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-15 20:29:44.000000 dottable_dict-0.0.4a0/src/dottable_dict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:29:44.000000 dottable_dict-0.0.4a0/src/dottable_dict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 20:29:44.000000 dottable_dict-0.0.4a0/src/dottable_dict.egg-info/top_level.txt
```

### Comparing `dottable_dict-0.0.4/LICENSE` & `dottable_dict-0.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dottable_dict-0.0.4/PKG-INFO` & `dottable_dict-0.0.4a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dottable_dict
-Version: 0.0.4
+Version: 0.0.4a0
 Summary: Your everyday dictionary, with the special ability to be accessed using dot-notation
 Author-email: Yuval Dotan <ydotan.tech@gmail.com>
 Project-URL: Homepage, https://github.com/yuvdo/dottable_dict
 Project-URL: Issues, https://github.com/yuvdo/dottable_dict/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dottable_dict-0.0.4/README.md` & `dottable_dict-0.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `dottable_dict-0.0.4/pyproject.toml` & `dottable_dict-0.0.4a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dottable_dict"
-version = "0.0.4"
+version = "0.0.4a"
 authors = [{ name = "Yuval Dotan", email = "ydotan.tech@gmail.com" }]
 description = "Your everyday dictionary, with the special ability to be accessed using dot-notation"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dottable_dict-0.0.4/src/dottable_dict/dottable_dict.py` & `dottable_dict-0.0.4a0/src/dottable_dict/dottable_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,47 +8,50 @@
     class _MergedValues(list):
         pass
 
     __data__: dict
     __autoconvert__: bool
 
     @staticmethod
-    def __convert_sequence__(it: Sequence):
+    def __convert_sequence__(seq: Sequence):
+        seq_type: type = type(seq)
         converted = []
-        for i in it:
+        if "join" in dir(seq):
+            return seq
+        for i in seq:
             if isinstance(i, Sequence):
                 converted.append(DottableDict.__convert_sequence__(i))
             else:
                 try:
                     converted.append(DottableDict(i))
                 except:
                     converted.append(i)
-        return converted
+        return seq_type(converted)
 
     def __init__(self, data: Any = None, autoconvert_dicts: bool = True):
         self.__autoconvert__ = autoconvert_dicts
         data = {} if data is None else data
         if isinstance(data, DottableDict):
             self.__data__ = data.__data__.copy()
         else:
             try:
                 data = dict(data)
             except Exception as e:
                 e.args = (f"cannot convert input to dict: {data}",)
                 raise (e)
             self.__data__ = {}
             for k, v in data.items():
-                val = v
                 if self.__autoconvert__:
-                    if isinstance(v, dict):
-                        val = DottableDict(v)
-                    elif isinstance(v, Sequence):
+                    if isinstance(v, Sequence):
                         val = DottableDict.__convert_sequence__(v)
                     else:
-                        val = v
+                        try:
+                            val = DottableDict(v)
+                        except:
+                            val = v
                 self.__data__[k] = val
 
     def __getattr__(self, key: str) -> Any:
         if not (key in self.__data__ or key in dir(self)):
             return self.__data__.__getattribute__(key)
         if key.isidentifier():
             return self.__data__[key]
```

### Comparing `dottable_dict-0.0.4/src/dottable_dict.egg-info/PKG-INFO` & `dottable_dict-0.0.4a0/src/dottable_dict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dottable_dict
-Version: 0.0.4
+Version: 0.0.4a0
 Summary: Your everyday dictionary, with the special ability to be accessed using dot-notation
 Author-email: Yuval Dotan <ydotan.tech@gmail.com>
 Project-URL: Homepage, https://github.com/yuvdo/dottable_dict
 Project-URL: Issues, https://github.com/yuvdo/dottable_dict/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

