# Comparing `tmp/pytups-0.87.3.tar.gz` & `tmp/pytups-0.88.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytups-0.87.3.tar", last modified: Fri Apr 12 16:47:04 2024, max compression
+gzip compressed data, was "pytups-0.88.1.tar", last modified: Wed May 15 15:31:03 2024, max compression
```

## Comparing `pytups-0.87.3.tar` & `pytups-0.88.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:47:04.810806 pytups-0.87.3/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 16:47:00.000000 pytups-0.87.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-12 16:47:00.000000 pytups-0.87.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-12 16:47:04.810806 pytups-0.87.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-12 16:47:00.000000 pytups-0.87.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:47:04.810806 pytups-0.87.3/pytups/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 16:47:00.000000 pytups-0.87.3/pytups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 16:47:00.000000 pytups-0.87.3/pytups/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-12 16:47:00.000000 pytups-0.87.3/pytups/orderedSet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-04-12 16:47:00.000000 pytups-0.87.3/pytups/superdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 16:47:00.000000 pytups-0.87.3/pytups/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-04-12 16:47:00.000000 pytups-0.87.3/pytups/tuplist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:47:04.810806 pytups-0.87.3/pytups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-12 16:47:04.000000 pytups-0.87.3/pytups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-12 16:47:04.000000 pytups-0.87.3/pytups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:47:04.000000 pytups-0.87.3/pytups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 16:47:04.000000 pytups-0.87.3/pytups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:47:04.810806 pytups-0.87.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 16:47:00.000000 pytups-0.87.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:47:04.810806 pytups-0.87.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-12 16:47:00.000000 pytups-0.87.3/tests/test_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-12 16:47:00.000000 pytups-0.87.3/tests/test_ordSet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-04-12 16:47:00.000000 pytups-0.87.3/tests/test_tuplists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:31:03.625001 pytups-0.88.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 15:30:59.000000 pytups-0.88.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-15 15:30:59.000000 pytups-0.88.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-15 15:31:03.625001 pytups-0.88.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-15 15:30:59.000000 pytups-0.88.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:31:03.621001 pytups-0.88.1/pytups/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 15:30:59.000000 pytups-0.88.1/pytups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 15:30:59.000000 pytups-0.88.1/pytups/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-15 15:30:59.000000 pytups-0.88.1/pytups/orderedSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-05-15 15:30:59.000000 pytups-0.88.1/pytups/superdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 15:30:59.000000 pytups-0.88.1/pytups/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-15 15:30:59.000000 pytups-0.88.1/pytups/tuplist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:31:03.625001 pytups-0.88.1/pytups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-15 15:31:03.000000 pytups-0.88.1/pytups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 15:31:03.000000 pytups-0.88.1/pytups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:31:03.000000 pytups-0.88.1/pytups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:31:03.000000 pytups-0.88.1/pytups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:31:03.625001 pytups-0.88.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-15 15:30:59.000000 pytups-0.88.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:31:03.625001 pytups-0.88.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18895 2024-05-15 15:30:59.000000 pytups-0.88.1/tests/test_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-15 15:30:59.000000 pytups-0.88.1/tests/test_ordSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-05-15 15:30:59.000000 pytups-0.88.1/tests/test_tuplists.py
```

### Comparing `pytups-0.87.3/LICENSE.txt` & `pytups-0.88.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytups-0.87.3/PKG-INFO` & `pytups-0.88.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytups
-Version: 0.87.3
+Version: 0.88.1
 Summary: data wrangling for lists of tuples and dictionaries
 Home-page: https://github.com/pchtsp/pytups
 Download-URL: https://github.com/pchtsp/pytups/archive/master.zip
 Author: Franco Peschiera
 Author-email: pchtsp@gmail.com
 Maintainer: Franco Peschiera
 Maintainer-email: pchtsp@gmail.com
@@ -43,15 +43,15 @@
 They're made to always return a new object, so no "in-place" editing, hopefully.
 
 Right now there are three classes to use: dictionaries, tuple lists and ordered sets.
 
 Python versions
 ================
 
-Python 3.6 and up.
+Python 3.8 and up.
 
 
 Quick example
 ================
 
 We index a tuple list according to some index positions.::
```

### Comparing `pytups-0.87.3/README.rst` & `pytups-0.88.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 They're made to always return a new object, so no "in-place" editing, hopefully.
 
 Right now there are three classes to use: dictionaries, tuple lists and ordered sets.
 
 Python versions
 ================
 
-Python 3.6 and up.
+Python 3.8 and up.
 
 
 Quick example
 ================
 
 We index a tuple list according to some index positions.::
```

### Comparing `pytups-0.87.3/pytups/orderedSet.py` & `pytups-0.88.1/pytups/orderedSet.py`

 * *Files identical despite different names*

### Comparing `pytups-0.87.3/pytups/superdict.py` & `pytups-0.88.1/pytups/superdict.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,33 +34,66 @@
 
     def __getitem__(self, key: K) -> V:
         return dict.__getitem__(self, key)
 
     def __iter__(self) -> Iterator[K]:
         return dict.__iter__(self)
 
-    def __add__(self, other):
+    def __add__(self, other: Union[dict, int, float, str]) -> "SuperDict":
+        """
+        Applies the adding operator to the values in the SuperDict and another object.
+        This operation might raise a TypeError based on the types of the values of the SuperDict and the other object.
+        """
         return self.sapply(op.__add__, other)
 
     # def __radd__(self, other):
     #     return self.sapply(op.__add__, other)
 
-    def __sub__(self, other):
+    def __sub__(self, other: Union[dict, int, float, str]) -> "SuperDict":
+        """
+        Applies the substract operator to the values in the SuperDict and another object.
+        This operation might raise a TypeError based on the types of the values of the SuperDict and the other object.
+        """
         return self.sapply(op.__sub__, other)
 
     # def __rsub__(self, other):
     #     return other.sapply(op.__sub__, self)
 
-    def __mul__(self, other):
+    def __mul__(self, other: Union[dict, int, float, str]) -> "SuperDict":
+        """
+        Applies the multiply operator to the values in the SuperDict and another object.
+        This operation might raise a TypeError based on the types of the values of the SuperDict and the other object.
+        """
         return self.sapply(op.__mul__, other)
 
     # def __rmul__(self, other):
     #     return self.sapply(op.__mul__, other)
 
-    def head(self):
+    def __truediv__(self, other: Union[dict, int, float, str]) -> "SuperDict":
+        """
+        Applies the true division (float division) operator to the values in the SuperDict and another object.
+        This operation might raise a TypeError based on the types of the values of the SuperDict and the other object.
+        """
+        return self.sapply(op.__truediv__, other)
+
+    def __floordiv__(self, other: Union[dict, int, float, str]) -> "SuperDict":
+        """
+        Applies the floor division (integer division) operator to the values in the SuperDict and another object.
+        This operation might raise a TypeError based on the types of the values of the SuperDict and the other object.
+        """
+        return self.sapply(op.__floordiv__, other)
+
+    def head(self) -> str:
+        """
+        Returns a string representation with the first pair of key values in the SuperDict, the last pair of key value
+        and the number of elements on the SuperDict.
+
+        :return: the head string representation of the SuperDict
+        :rtype: str
+        """
         if len(self) <= 2:
             return dict.__repr__(self)
         _keys = self.keys_l()
         first, last = (_keys[n] for n in [0, -1])
         first_v, last_v = (self[n] for n in [first, last])
         return '"{{{}: {}\n,..., \n{}: {}}}"\n{} elements'.format(
             first.__repr__(),
@@ -450,27 +483,31 @@
         Same as apply but only on keys
 
         :param callable func: function to apply.
         :return: new :py:class:`SuperDict`
         """
         return SuperDict({k: func(k, *args, **kwargs) for k in self})
 
-    def sapply(self, func: Callable, other: dict, *args, **kwargs) -> "SuperDict":
+    def sapply(
+        self, func: Callable, other: Union[dict, int, float, str], *args, **kwargs
+    ) -> "SuperDict":
         """
         Applies function to both dictionaries.
         Using keys of the self.
         It's like applying a function over the left join.
 
         :param callable func: function to apply.
-        :param dict other: dictionary to apply function to
+        :param Union[dict, int, float,s tr] other: either an int, a float, a string or another dictionary to
+          perform the operation over
         :return: new :py:class:`SuperDict`
         """
-        return SuperDict(
-            {k: func(v, other[k], *args, **kwargs) for k, v in self.items()}
-        )
+        if isinstance(other, (int, float, str)):
+            return self.vapply(lambda v: func(v, other, *args, **kwargs))
+
+        return self.kvapply(lambda k, v: func(v, other[k], *args, **kwargs))
 
     def get_m(self, *args, default=None) -> Any:
         """
         Safe way to search for something in a nested dictionary
 
         :param args: keys in nested dictionary
         :return: content after traversing the nested dictionary. None if doesn't exit
```

### Comparing `pytups-0.87.3/pytups/tools.py` & `pytups-0.88.1/pytups/tools.py`

 * *Files identical despite different names*

### Comparing `pytups-0.87.3/pytups/tuplist.py` & `pytups-0.88.1/pytups/tuplist.py`

 * *Files identical despite different names*

### Comparing `pytups-0.87.3/pytups.egg-info/PKG-INFO` & `pytups-0.88.1/pytups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytups
-Version: 0.87.3
+Version: 0.88.1
 Summary: data wrangling for lists of tuples and dictionaries
 Home-page: https://github.com/pchtsp/pytups
 Download-URL: https://github.com/pchtsp/pytups/archive/master.zip
 Author: Franco Peschiera
 Author-email: pchtsp@gmail.com
 Maintainer: Franco Peschiera
 Maintainer-email: pchtsp@gmail.com
@@ -43,15 +43,15 @@
 They're made to always return a new object, so no "in-place" editing, hopefully.
 
 Right now there are three classes to use: dictionaries, tuple lists and ordered sets.
 
 Python versions
 ================
 
-Python 3.6 and up.
+Python 3.8 and up.
 
 
 Quick example
 ================
 
 We index a tuple list according to some index positions.::
```

### Comparing `pytups-0.87.3/setup.py` & `pytups-0.88.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytups-0.87.3/tests/test_dicts.py` & `pytups-0.88.1/tests/test_dicts.py`

 * *Files 14% similar despite different names*

```diff
@@ -458,14 +458,131 @@
         a = self.dict_class()
         try:
             a.set_m("y", "x", value=1)
         except AttributeError as e:
             self.fail(e)
         self.assertEqual(a, {"y": {"x": 1}})
 
+    def test_add_dicts(self):
+        a = self.dict_class({"a": 1})
+        b = self.dict_class({"a": 2, "b": 1})
+        c = a + b
+        self.assertEqual(c, {"a": 3})
+
+    def test_add_int(self):
+        a = self.dict_class({"a": 1, "b": 5})
+        c = a + 2
+        self.assertEqual(c, {"a": 3, "b": 7})
+
+    def test_add_float(self):
+        a = self.dict_class({"a": 1, "b": 5})
+        c = a + 2.5
+        self.assertEqual(c, {"a": 3.5, "b": 7.5})
+
+    def test_subtract_dict(self):
+        a = self.dict_class({"a": 1})
+        b = self.dict_class({"a": 2})
+        c = a - b
+        self.assertEqual(c, {"a": -1})
+
+    def test_subtract_int(self):
+        a = self.dict_class({"a": 1, "b": 1})
+        c = a - 1
+        self.assertEqual(c, {"a": 0, "b": 0})
+
+    def test_subtract_float(self):
+        a = self.dict_class({"a": 1, "b": 1})
+        c = a - 1.5
+        self.assertEqual(c, {"a": -0.5, "b": -0.5})
+
+    def test_multiply_dicts(self):
+        a = self.dict_class({"a": 1})
+        b = self.dict_class({"a": 2})
+        c = a * b
+        self.assertEqual(c, {"a": 2})
+
+    def test_multiply_int(self):
+        a = self.dict_class({"a": 1, "b": -1})
+        c = a * 2
+        self.assertEqual(c, {"a": 2, "b": -2})
+
+    def test_multiply_float(self):
+        a = self.dict_class({"a": 1, "b": 5})
+        c = a * 2.5
+        self.assertEqual(c, {"a": 2.5, "b": 12.5})
+
+    def test_divide_dicts(self):
+        a = self.dict_class({"a": 4})
+        b = self.dict_class({"a": 2})
+        c = a / b
+        self.assertEqual(c, {"a": 2})
+
+    def test_divide_int(self):
+        a = self.dict_class({"a": 4, "b": 4})
+        c = a / 3
+        self.assertEqual(c, {"a": 4 / 3, "b": 4 / 3})
+
+    def test_divide_float(self):
+        a = self.dict_class({"a": 4, "b": 6})
+        c = a / 3.0
+        self.assertEqual(c, {"a": 4 / 3.0, "b": 6 / 3.0})
+
+    def test_integer_div_dicts(self):
+        a = self.dict_class({"a": 4})
+        b = self.dict_class({"a": 3, "b": 1})
+        c = a // b
+        self.assertEqual(c, {"a": 1})
+
+    def test_integer_div_int(self):
+        a = self.dict_class({"a": 4, "b": 6})
+        c = a // 3
+        self.assertEqual(c, {"a": 1, "b": 2})
+
+    def test_integer_div_float(self):
+        a = self.dict_class({"a": 4, "b": 7})
+        c = a // 3.5
+        self.assertEqual(c, {"a": 1, "b": 2})
+
+    def test_add_strings(self):
+        a = self.dict_class({"a": "a"})
+        b = self.dict_class({"a": "b"})
+        c = a + b
+        self.assertEqual(c, {"a": "ab"})
+
+    def test_add_lists(self):
+        a = self.dict_class({"a": [1]})
+        b = self.dict_class({"a": [2]})
+        c = a + b
+        self.assertEqual(c, {"a": [1, 2]})
+
+    def test_add_int_to_list(self):
+        a = self.dict_class({"a": [1]})
+        lambda_add = lambda a: a + 2
+        self.assertRaises(TypeError, lambda_add, a)
+
+    def test_add_int_to_string(self):
+        a = self.dict_class({"a": "a"})
+        lambda_add = lambda a: a + 2
+        self.assertRaises(TypeError, lambda_add, a)
+
+    def test_add_str_to_int(self):
+        a = self.dict_class({"a": 2})
+        lambda_add = lambda a: a + "2"
+        self.assertRaises(TypeError, lambda_add, a)
+
+    def test_multiply_string_into_int(self):
+        a = self.dict_class({"a": "a"})
+        c = a * 2
+        self.assertEqual(c, {"a": "aa"})
+
+    def test_multiply_int_to_string(self):
+        a = self.dict_class({"a": 2})
+        c = a * "2"
+        self.assertEqual(c, {"a": "22"})
+
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
```

### Comparing `pytups-0.87.3/tests/test_ordSet.py` & `pytups-0.88.1/tests/test_ordSet.py`

 * *Files identical despite different names*

### Comparing `pytups-0.87.3/tests/test_tuplists.py` & `pytups-0.88.1/tests/test_tuplists.py`

 * *Files identical despite different names*

