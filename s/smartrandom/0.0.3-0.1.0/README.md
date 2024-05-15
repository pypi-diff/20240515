# Comparing `tmp/smartrandom-0.0.3.tar.gz` & `tmp/smartrandom-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartrandom-0.0.3.tar", last modified: Mon May 13 00:45:27 2024, max compression
+gzip compressed data, was "smartrandom-0.1.0.tar", last modified: Wed May 15 05:04:00 2024, max compression
```

## Comparing `smartrandom-0.0.3.tar` & `smartrandom-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 00:45:27.214796 smartrandom-0.0.3/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 03:52:29.000000 smartrandom-0.0.3/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)     3557 2024-05-13 00:45:27.214796 smartrandom-0.0.3/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     2632 2024-05-13 00:43:28.000000 smartrandom-0.0.3/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)     1108 2024-05-13 00:45:27.218129 smartrandom-0.0.3/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)       84 2024-05-08 03:52:29.000000 smartrandom-0.0.3/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 00:45:27.214796 smartrandom-0.0.3/smartrandom/
--rw-r--r--   0 smart     (1000) smart     (1000)      399 2024-05-13 00:44:17.000000 smartrandom-0.0.3/smartrandom/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     1987 2024-05-08 03:57:25.000000 smartrandom-0.0.3/smartrandom/random_master.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 00:45:27.214796 smartrandom-0.0.3/smartrandom.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     3557 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      263 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-13 00:45:27.000000 smartrandom-0.0.3/smartrandom.egg-info/top_level.txt
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:04:00.729252 smartrandom-0.1.0/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 03:52:29.000000 smartrandom-0.1.0/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)     3683 2024-05-15 05:04:00.729252 smartrandom-0.1.0/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     2679 2024-05-15 04:50:25.000000 smartrandom-0.1.0/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)     1191 2024-05-15 05:04:00.729252 smartrandom-0.1.0/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      442 2024-05-15 05:03:25.000000 smartrandom-0.1.0/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:04:00.725918 smartrandom-0.1.0/smartrandom/
+-rw-r--r--   0 smart     (1000) smart     (1000)      621 2024-05-15 04:46:27.000000 smartrandom-0.1.0/smartrandom/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     2503 2024-05-15 04:58:19.000000 smartrandom-0.1.0/smartrandom/random_master.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:04:00.729252 smartrandom-0.1.0/smartrandom.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     3683 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      263 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/top_level.txt
```

### Comparing `smartrandom-0.0.3/LICENSE` & `smartrandom-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartrandom-0.0.3/PKG-INFO` & `smartrandom-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.0.3
-Summary: Random Data Generators
+Version: 0.1.0
+Summary: Random Data Generators.
 Home-page: https://github.com/smartlegionlab/smartrandom/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
-Keywords: password generator,smartrandom,smartlegionlab
+Keywords: password generator,code generator,random generator,random code generator,random string generator,smartrandom,smartlegionlab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom <sup>v0.0.3</sup>
+# smartrandom <sup>v0.1.0</sup>
 ---
 
 ## Random Data Generators:
 
-Allows you to generate random strings of a given length from letters, numbers, symbols.
-Helps to generate passwords, service codes (for example, for sending via SMS), hashes and much more.
+Allows you to generate random strings of a given length from letters, numbers, and symbols.
+Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
+
 ---
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartrandom?label=pypi%20downloads)](https://pypi.org/project/smartrandom/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartrandom)
 [![PyPI](https://img.shields.io/pypi/v/smartrandom)](https://pypi.org/project/smartrandom)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/blob/master/LICENSE)
 [![PyPI - Format](https://img.shields.io/pypi/format/smartrandom)](https://pypi.org/project/smartrandom)
 
+***
+
+Author and developer: ___A.A Suvorov.___
+
+***
 
 ## Help:
 
+`pip install smartrandom`
+
 ```python
-from smartrandom.random_master import RandomMaster
+from smartrandom.random_master import RandomStringMaster
 
-random_string = RandomMaster.string.create(length=10)
-random_number_string = RandomMaster.number.create(length=10)
-password = RandomMaster.password.create(length=10)
-random_hash = RandomMaster.hash.create(text='give me hash')
-random_number_code = RandomMaster.create_code(length=10, number_flag=True)
-random_string_code = RandomMaster.create_code(length=10, string_flag=True)
-random_symbol_code = RandomMaster.create_code(length=10, symbol_flag=True)
+random_string = RandomStringMaster.create_string(length=10)
+string_hash = RandomStringMaster.create_hash('text')
+number_code = RandomStringMaster.create_numeric_code(length=6)
+letter_code = RandomStringMaster.create_letters_code(length=6)
+symbol_code = RandomStringMaster.create_letters_code(length=6)
+code = RandomStringMaster.create_code(length=10, numeric_flag=True, letters_flag=True, symbols_flag=True)
 
 ```
 
 ***
 
 ## Disclaimer of liability:
```

### Comparing `smartrandom-0.0.3/README.md` & `smartrandom-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,43 @@
-# smartrandom <sup>v0.0.3</sup>
+# smartrandom <sup>v0.1.0</sup>
 ---
 
 ## Random Data Generators:
 
-Allows you to generate random strings of a given length from letters, numbers, symbols.
-Helps to generate passwords, service codes (for example, for sending via SMS), hashes and much more.
+Allows you to generate random strings of a given length from letters, numbers, and symbols.
+Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
+
 ---
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartrandom?label=pypi%20downloads)](https://pypi.org/project/smartrandom/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartrandom)
 [![PyPI](https://img.shields.io/pypi/v/smartrandom)](https://pypi.org/project/smartrandom)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/blob/master/LICENSE)
 [![PyPI - Format](https://img.shields.io/pypi/format/smartrandom)](https://pypi.org/project/smartrandom)
 
+***
+
+Author and developer: ___A.A Suvorov.___
+
+***
 
 ## Help:
 
+`pip install smartrandom`
+
 ```python
-from smartrandom.random_master import RandomMaster
+from smartrandom.random_master import RandomStringMaster
 
-random_string = RandomMaster.string.create(length=10)
-random_number_string = RandomMaster.number.create(length=10)
-password = RandomMaster.password.create(length=10)
-random_hash = RandomMaster.hash.create(text='give me hash')
-random_number_code = RandomMaster.create_code(length=10, number_flag=True)
-random_string_code = RandomMaster.create_code(length=10, string_flag=True)
-random_symbol_code = RandomMaster.create_code(length=10, symbol_flag=True)
+random_string = RandomStringMaster.create_string(length=10)
+string_hash = RandomStringMaster.create_hash('text')
+number_code = RandomStringMaster.create_numeric_code(length=6)
+letter_code = RandomStringMaster.create_letters_code(length=6)
+symbol_code = RandomStringMaster.create_letters_code(length=6)
+code = RandomStringMaster.create_code(length=10, numeric_flag=True, letters_flag=True, symbols_flag=True)
 
 ```
 
 ***
 
 ## Disclaimer of liability:
```

### Comparing `smartrandom-0.0.3/smartrandom/random_master.py` & `smartrandom-0.1.0/smartrandom/random_master.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,71 +2,85 @@
 # Licensed under the terms of the BSD 3-Clause License
 # (see LICENSE for details).
 # Copyright © 2018-2024, A.A Suvorov
 # All rights reserved.
 # --------------------------------------------------------
 # https://github.com/smartlegionlab
 # --------------------------------------------------------
+"""Random Data Generators."""
 import hashlib
 import random
 import string
 
 
-class RandomStringMaster:
+class RandomLettersMaster:
     letters = string.ascii_letters
 
     @classmethod
     def create(cls, length=10):
         return ''.join((random.choice(cls.letters) for _ in range(length)))
 
 
-class RandomNumberMaster:
+class RandomNumericMaster:
     numbers = string.digits
 
     @classmethod
     def create(cls, length=10):
         return ''.join((random.choice(cls.numbers) for _ in range(length)))
 
 
-class RandomSymbolMaster:
+class RandomSymbolsMaster:
     symbols = '@$!%*#?&-'
 
     @classmethod
     def create(cls, length=10):
         return ''.join((random.choice(cls.symbols) for _ in range(length)))
 
 
-class RandomPasswordMaster:
-    letters = string.ascii_letters
-    numbers = string.digits
-    symbols = '@$!%*#?&-'
+class HashMaster:
+    @classmethod
+    def create(cls, text: str):
+        text = str(text)
+        sha = hashlib.sha3_512(text.encode('utf-8'))
+        new_hash = sha.hexdigest()
+        return new_hash
+
+
+class RandomStringMaster:
+    letters_master = RandomLettersMaster()
+    numeric_master = RandomNumericMaster()
+    symbols_master = RandomSymbolsMaster()
+    hash_master = HashMaster()
 
     @classmethod
-    def create(cls, length=10):
-        return ''.join((random.choice(cls.letters + cls.numbers + cls.symbols) for _ in range(length)))
+    def create_string(cls, length=10):
+        random_string = cls.letters_master.letters + cls.numeric_master.numbers + cls.symbols_master.symbols
+        return ''.join((random.choice(random_string) for _ in range(length)))
 
+    @classmethod
+    def create_hash(cls, text):
+        return cls.hash_master.create(text)
 
-class RandomHashMaster:
     @classmethod
-    def create(cls, text):
-        sha = hashlib.sha3_512(text.encode('utf-8'))
-        new_hash = sha.hexdigest()
-        return new_hash
+    def create_numeric_code(cls, length):
+        return cls.numeric_master.create(length)
 
+    @classmethod
+    def create_letters_code(cls, length):
+        return cls.letters_master.create(length)
 
-class RandomMaster:
-    string = RandomStringMaster()
-    number = RandomNumberMaster()
-    symbol = RandomSymbolMaster()
-    password = RandomPasswordMaster()
-    hash = RandomHashMaster()
+    @classmethod
+    def create_symbols_code(cls, length):
+        return cls.symbols_master.create(length)
 
     @classmethod
-    def create_code(cls, length=10, number_flag=False, string_flag=False, symbol_flag=False):
+    def create_code(cls, length=10, numeric_flag=False, letters_flag=False, symbols_flag=False):
         data = ''
-        if string_flag:
-            data += cls.string.letters
-        if number_flag:
-            data += cls.number.numbers
-        if symbol_flag:
-            data += cls.symbol.symbols
-        return ''.join((random.choice(data) for _ in range(length)))
+        if letters_flag:
+            data += cls.letters_master.letters
+        if numeric_flag:
+            data += cls.numeric_master.numbers
+        if symbols_flag:
+            data += cls.symbols_master.symbols
+        if data:
+            return ''.join((random.choice(data) for _ in range(length)))
+        return None
```

### Comparing `smartrandom-0.0.3/smartrandom.egg-info/PKG-INFO` & `smartrandom-0.1.0/smartrandom.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.0.3
-Summary: Random Data Generators
+Version: 0.1.0
+Summary: Random Data Generators.
 Home-page: https://github.com/smartlegionlab/smartrandom/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
-Keywords: password generator,smartrandom,smartlegionlab
+Keywords: password generator,code generator,random generator,random code generator,random string generator,smartrandom,smartlegionlab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom <sup>v0.0.3</sup>
+# smartrandom <sup>v0.1.0</sup>
 ---
 
 ## Random Data Generators:
 
-Allows you to generate random strings of a given length from letters, numbers, symbols.
-Helps to generate passwords, service codes (for example, for sending via SMS), hashes and much more.
+Allows you to generate random strings of a given length from letters, numbers, and symbols.
+Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
+
 ---
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartrandom?label=pypi%20downloads)](https://pypi.org/project/smartrandom/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartrandom)
 [![PyPI](https://img.shields.io/pypi/v/smartrandom)](https://pypi.org/project/smartrandom)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/blob/master/LICENSE)
 [![PyPI - Format](https://img.shields.io/pypi/format/smartrandom)](https://pypi.org/project/smartrandom)
 
+***
+
+Author and developer: ___A.A Suvorov.___
+
+***
 
 ## Help:
 
+`pip install smartrandom`
+
 ```python
-from smartrandom.random_master import RandomMaster
+from smartrandom.random_master import RandomStringMaster
 
-random_string = RandomMaster.string.create(length=10)
-random_number_string = RandomMaster.number.create(length=10)
-password = RandomMaster.password.create(length=10)
-random_hash = RandomMaster.hash.create(text='give me hash')
-random_number_code = RandomMaster.create_code(length=10, number_flag=True)
-random_string_code = RandomMaster.create_code(length=10, string_flag=True)
-random_symbol_code = RandomMaster.create_code(length=10, symbol_flag=True)
+random_string = RandomStringMaster.create_string(length=10)
+string_hash = RandomStringMaster.create_hash('text')
+number_code = RandomStringMaster.create_numeric_code(length=6)
+letter_code = RandomStringMaster.create_letters_code(length=6)
+symbol_code = RandomStringMaster.create_letters_code(length=6)
+code = RandomStringMaster.create_code(length=10, numeric_flag=True, letters_flag=True, symbols_flag=True)
 
 ```
 
 ***
 
 ## Disclaimer of liability:
```

