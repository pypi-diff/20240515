# Comparing `tmp/chatgpt_md_converter-0.1.0.tar.gz` & `tmp/chatgpt_md_converter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_md_converter-0.1.0.tar", last modified: Wed May 15 08:58:49 2024, max compression
+gzip compressed data, was "chatgpt_md_converter-0.1.1.tar", last modified: Wed May 15 09:05:16 2024, max compression
```

## Comparing `chatgpt_md_converter-0.1.0.tar` & `chatgpt_md_converter-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:58:49.451458 chatgpt_md_converter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-15 08:58:49.451458 chatgpt_md_converter-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:58:49.451458 chatgpt_md_converter-0.1.0/chatgpt_md_converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter/extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter/telegram_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:58:49.451458 chatgpt_md_converter-0.1.0/chatgpt_md_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-15 08:58:49.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 08:58:49.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:58:49.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 08:58:49.000000 chatgpt_md_converter-0.1.0/chatgpt_md_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:58:49.451458 chatgpt_md_converter-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:58:49.451458 chatgpt_md_converter-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-15 08:58:46.000000 chatgpt_md_converter-0.1.0/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:05:16.486242 chatgpt_md_converter-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-15 09:05:16.486242 chatgpt_md_converter-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:05:16.482242 chatgpt_md_converter-0.1.1/chatgpt_md_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter/telegram_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:05:16.486242 chatgpt_md_converter-0.1.1/chatgpt_md_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-15 09:05:16.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 09:05:16.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:05:16.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 09:05:16.000000 chatgpt_md_converter-0.1.1/chatgpt_md_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 09:05:16.486242 chatgpt_md_converter-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:05:16.486242 chatgpt_md_converter-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-15 09:05:13.000000 chatgpt_md_converter-0.1.1/tests/test_parser.py
```

### Comparing `chatgpt_md_converter-0.1.0/LICENSE` & `chatgpt_md_converter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_md_converter-0.1.0/PKG-INFO` & `chatgpt_md_converter-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt_md_converter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for converting markdown to HTML for chat Telegram bots
 Home-page: https://github.com/Latand/formatter-chatgpt-telegram
 Author: Kostiantyn Kriuchkov
 Author-email: latand666@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,17 +38,27 @@
 
 3. **Markdown to HTML Conversion**: Applies various regex substitutions and custom logic to convert supported Markdown formatting to Telegram-compatible HTML tags.
 
 4. **Reinsert Code Blocks**: Reinserts the previously extracted and converted code blocks back into the main text, replacing placeholders with the appropriate HTML content.
 
 Simply call the `telegram_format(text: str) -> str` function with your Markdown-formatted text as input to receive the converted HTML output ready for use with the Telegram Bot API.
 
+## Installation
+
+You can install the package using pip:
+
+```sh
+pip install chatgpt-md-converter
+```
+
 ## Example
 
 ```python
+from chatgpt_md_converter import telegram_format
+
 formatted_text = telegram_format("Here is some **bold**, __underline__, and `inline code`.\n```python\nprint('Hello, world!')\n```")
 print(formatted_text)
 ```
 
 ## Requirements
 
 - Python 3.x
```

### Comparing `chatgpt_md_converter-0.1.0/chatgpt_md_converter/converters.py` & `chatgpt_md_converter-0.1.1/chatgpt_md_converter/converters.py`

 * *Files identical despite different names*

### Comparing `chatgpt_md_converter-0.1.0/chatgpt_md_converter/extractors.py` & `chatgpt_md_converter-0.1.1/chatgpt_md_converter/extractors.py`

 * *Files identical despite different names*

### Comparing `chatgpt_md_converter-0.1.0/chatgpt_md_converter/formatters.py` & `chatgpt_md_converter-0.1.1/chatgpt_md_converter/formatters.py`

 * *Files identical despite different names*

### Comparing `chatgpt_md_converter-0.1.0/chatgpt_md_converter/telegram_formatter.py` & `chatgpt_md_converter-0.1.1/chatgpt_md_converter/telegram_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_md_converter-0.1.0/chatgpt_md_converter.egg-info/PKG-INFO` & `chatgpt_md_converter-0.1.1/chatgpt_md_converter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt_md_converter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for converting markdown to HTML for chat Telegram bots
 Home-page: https://github.com/Latand/formatter-chatgpt-telegram
 Author: Kostiantyn Kriuchkov
 Author-email: latand666@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,17 +38,27 @@
 
 3. **Markdown to HTML Conversion**: Applies various regex substitutions and custom logic to convert supported Markdown formatting to Telegram-compatible HTML tags.
 
 4. **Reinsert Code Blocks**: Reinserts the previously extracted and converted code blocks back into the main text, replacing placeholders with the appropriate HTML content.
 
 Simply call the `telegram_format(text: str) -> str` function with your Markdown-formatted text as input to receive the converted HTML output ready for use with the Telegram Bot API.
 
+## Installation
+
+You can install the package using pip:
+
+```sh
+pip install chatgpt-md-converter
+```
+
 ## Example
 
 ```python
+from chatgpt_md_converter import telegram_format
+
 formatted_text = telegram_format("Here is some **bold**, __underline__, and `inline code`.\n```python\nprint('Hello, world!')\n```")
 print(formatted_text)
 ```
 
 ## Requirements
 
 - Python 3.x
```

### Comparing `chatgpt_md_converter-0.1.0/setup.py` & `chatgpt_md_converter-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="chatgpt_md_converter",
-    version="0.1.0",
+    version="0.1.1",
     author="Kostiantyn Kriuchkov",
     author_email="latand666@gmail.com",
     description="A package for converting markdown to HTML for chat Telegram bots",
     long_description=open("README.MD").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Latand/formatter-chatgpt-telegram",
     classifiers=[
```

### Comparing `chatgpt_md_converter-0.1.0/tests/test_parser.py` & `chatgpt_md_converter-0.1.1/tests/test_parser.py`

 * *Files identical despite different names*

