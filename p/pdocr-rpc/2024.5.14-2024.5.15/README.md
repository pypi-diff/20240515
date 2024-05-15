# Comparing `tmp/pdocr_rpc-2024.5.14.tar.gz` & `tmp/pdocr_rpc-2024.5.15.tar.gz`

## Comparing `pdocr_rpc-2024.5.14.tar` & `pdocr_rpc-2024.5.15.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     9705 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pdocr_rpc/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pdocr_rpc/__version__.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pdocr_rpc/conf.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pdocr_rpc/server.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/LICENSE
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/NOTICE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/README.md
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pyproject.toml
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/PKG-INFO
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pdocr_rpc/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pdocr_rpc/__version__.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pdocr_rpc/conf.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pdocr_rpc/server.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/LICENSE
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/NOTICE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/README.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pyproject.toml
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/PKG-INFO
```

### Comparing `pdocr_rpc-2024.5.14/pdocr_rpc/__init__.py` & `pdocr_rpc-2024.5.15/pdocr_rpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 put_handle.close()
                 # 返回识别结果
                 pic_path =  cls.server().paddle_ocr(pic_dir, lang)
                 return pic_path
             except OSError:
                 continue
         raise EnvironmentError(
-            f"RPC服务器链接失败: {cls.server_url}"
+            f"RPC服务器链接失败: {cls.server_url()}"
         )
 
     @classmethod
     def _ocr(
             cls,
             *target_strings,
             picture_abspath=None,
```

### Comparing `pdocr_rpc-2024.5.14/pdocr_rpc/conf.py` & `pdocr_rpc-2024.5.15/pdocr_rpc/conf.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.14/pdocr_rpc/server.py` & `pdocr_rpc-2024.5.15/pdocr_rpc/server.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.14/LICENSE` & `pdocr_rpc-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.14/NOTICE` & `pdocr_rpc-2024.5.15/NOTICE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.14/README.md` & `pdocr_rpc-2024.5.15/README.md`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.14/pyproject.toml` & `pdocr_rpc-2024.5.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.14/PKG-INFO` & `pdocr_rpc-2024.5.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 2024.5.14
+Version: 2024.5.15
 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/linuxdeepin/pdocr-rpc
 Project-URL: Documentation, https://linuxdeepin.github.io/pdocr-rpc
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 License-File: NOTICE
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdocr-rpc Version: 2024.5.14 Summary: PaddleOCR-RPC
+Metadata-Version: 2.1 Name: pdocr-rpc Version: 2024.5.15 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/linuxdeepin/pdocr-rpc Project-URL:
 Documentation, https://linuxdeepin.github.io/pdocr-rpc Author-email: mikigo
 <1964191531@qq.com> License-File: LICENSE License-File: NOTICE Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.7 Requires-Dist: funnylog Requires-Dist: pillow; sys_platform ==
 'win32' Requires-Dist: pyscreenshot; sys_platform == 'linux' Provides-Extra:
```

