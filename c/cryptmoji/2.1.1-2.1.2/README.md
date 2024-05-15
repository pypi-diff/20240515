# Comparing `tmp/cryptmoji-2.1.1.tar.gz` & `tmp/cryptmoji-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptmoji-2.1.1.tar", max compression
+gzip compressed data, was "cryptmoji-2.1.2.tar", max compression
```

## Comparing `cryptmoji-2.1.1.tar` & `cryptmoji-2.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      123 2024-05-13 16:15:31.984887 cryptmoji-2.1.1/cryptmoji/__init__.py
--rw-r--r--   0        0        0      816 2024-05-14 03:39:33.276065 cryptmoji-2.1.1/cryptmoji/cli.py
--rw-r--r--   0        0        0    13293 2022-09-15 07:14:58.000000 cryptmoji-2.1.1/cryptmoji/data.py
--rw-r--r--   0        0        0     1400 2024-05-13 07:18:19.674068 cryptmoji-2.1.1/cryptmoji/main.py
--rw-r--r--   0        0        0       25 2024-05-14 03:39:49.259709 cryptmoji-2.1.1/cryptmoji/version.py
--rw-r--r--   0        0        0     1094 2022-09-04 12:17:16.000000 cryptmoji-2.1.1/LICENSE
--rw-r--r--   0        0        0     1570 2024-05-14 03:40:12.020299 cryptmoji-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     1399 2024-05-13 17:22:55.307088 cryptmoji-2.1.1/README.md
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 cryptmoji-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-05-13 16:15:31.984887 cryptmoji-2.1.2/cryptmoji/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-15 16:17:53.140725 cryptmoji-2.1.2/cryptmoji/cli.py
+-rw-r--r--   0        0        0    13293 2022-09-15 07:14:58.000000 cryptmoji-2.1.2/cryptmoji/data.py
+-rw-r--r--   0        0        0     1421 2024-05-15 16:03:54.826995 cryptmoji-2.1.2/cryptmoji/main.py
+-rw-r--r--   0        0        0       25 2024-05-15 16:18:52.333099 cryptmoji-2.1.2/cryptmoji/version.py
+-rw-r--r--   0        0        0     1094 2022-09-04 12:17:16.000000 cryptmoji-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1570 2024-05-15 16:18:44.219895 cryptmoji-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1399 2024-05-13 17:22:55.307088 cryptmoji-2.1.2/README.md
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 cryptmoji-2.1.2/PKG-INFO
```

### Comparing `cryptmoji-2.1.1/cryptmoji/data.py` & `cryptmoji-2.1.2/cryptmoji/data.py`

 * *Files identical despite different names*

### Comparing `cryptmoji-2.1.1/cryptmoji/main.py` & `cryptmoji-2.1.2/cryptmoji/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,21 +16,21 @@
         The string to use for increasing complexity of encryption
 
     Returns
     -------
     encrypted: str
         The encrypted string
     """
-    iterator = range(len(text))
-    if key is None:
-        char_2_int = [ord(text[i]) for i in iterator]
-    else:  # key is not None
-        char_2_int = [ord(text[i]) + ord(key[i % len(key)]) for i in iterator]
-    char_arr = [EMOJIS[i % LENGTH] for i in char_2_int]
-    return "".join(char_arr)
+    if key:
+        key_len = len(key)
+        iterator = range(len(text))
+        char_2_int = map(lambda x: ord(text[x]) + ord(key[x % key_len]), iterator)
+    else:
+        char_2_int = map(ord, text)
+    return "".join(map(lambda x: EMOJIS[x % LENGTH], char_2_int))
 
 
 def decrypt(text: str, *, key: Union[str, None] = None) -> str:
     """
     Decrypts a string from emojis.
 
     Args
@@ -43,13 +43,16 @@
     Returns
     -------
     encrypted: str
         The decrypted string
     """
     emojis_2_int = [EMOJIS.index(i) for i in text]
     iterator = range(len(emojis_2_int))
-    if key is not None:
-        decrypted = [emojis_2_int[i] - ord(key[i % len(key)]) for i in iterator]
+    if key:
+        key_len = len(key)
+        decrypted = map(
+            lambda x: (emojis_2_int[x] - ord(key[x % key_len]) + LENGTH) % LENGTH,
+            iterator,
+        )
     else:
-        decrypted = [emojis_2_int[i] for i in iterator]
-    char_arr = [chr(i) for i in decrypted]
-    return "".join(char_arr)
+        decrypted = map(lambda x: emojis_2_int[x], iterator)
+    return "".join(map(chr, decrypted))
```

### Comparing `cryptmoji-2.1.1/LICENSE` & `cryptmoji-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptmoji-2.1.1/pyproject.toml` & `cryptmoji-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cryptmoji"
-version = "2.1.1"
+version = "2.1.2"
 description = "Encrypt Text using emojis!"
 authors = ["Siddhesh Agarwal <siddhesh.agarwal@gmail.com>"]
 license = "MIT"
 readme = "./README.md"
 repository = "https://github.com/Siddhesh-Agarwal/cryptmoji"
 documentation = "https://github.com/Siddhesh-Agarwal/cryptmoji/wiki"
 keywords = ["encryption", "emoji", "cipher", "cryptography", "cryptmoji"]
```

### Comparing `cryptmoji-2.1.1/README.md` & `cryptmoji-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cryptmoji-2.1.1/PKG-INFO` & `cryptmoji-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptmoji
-Version: 2.1.1
+Version: 2.1.2
 Summary: Encrypt Text using emojis!
 Home-page: https://github.com/Siddhesh-Agarwal/cryptmoji
 License: MIT
 Keywords: encryption,emoji,cipher,cryptography,cryptmoji
 Author: Siddhesh Agarwal
 Author-email: siddhesh.agarwal@gmail.com
 Requires-Python: >=3.7.0,<4.0
```

