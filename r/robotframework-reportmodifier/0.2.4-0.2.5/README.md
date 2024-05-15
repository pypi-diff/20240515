# Comparing `tmp/robotframework_reportmodifier-0.2.4.tar.gz` & `tmp/robotframework_reportmodifier-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_reportmodifier-0.2.4.tar", max compression
+gzip compressed data, was "robotframework_reportmodifier-0.2.5.tar", max compression
```

## Comparing `robotframework_reportmodifier-0.2.4.tar` & `robotframework_reportmodifier-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35801 2024-02-12 08:28:04.348570 robotframework_reportmodifier-0.2.4/LICENSE
--rw-r--r--   0        0        0     1988 2024-04-04 08:41:05.991558 robotframework_reportmodifier-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4848 2024-04-03 11:11:32.367186 robotframework_reportmodifier-0.2.4/README.md
--rw-r--r--   0        0        0       44 2024-03-28 08:26:32.278869 robotframework_reportmodifier-0.2.4/src/reportmodifier/__init__.py
--rw-r--r--   0        0        0       23 2024-04-04 08:41:37.832176 robotframework_reportmodifier-0.2.4/src/reportmodifier/__version__.py
--rw-r--r--   0        0        0     1664 2024-04-03 11:11:32.397501 robotframework_reportmodifier-0.2.4/src/reportmodifier/_file_tools.py
--rw-r--r--   0        0        0     5981 2024-04-03 11:11:32.400497 robotframework_reportmodifier-0.2.4/src/reportmodifier/_report_configuration.py
--rw-r--r--   0        0        0     6945 2024-04-04 08:42:53.028946 robotframework_reportmodifier-0.2.4/src/reportmodifier/ReportModifier.py
--rw-r--r--   0        0        0    12069 2024-04-04 08:42:53.030952 robotframework_reportmodifier-0.2.4/src/reportmodifier/ReportModifierVisitor.py
--rw-r--r--   0        0        0       79 2024-04-03 11:11:32.384485 robotframework_reportmodifier-0.2.4/src/ReportModifierListener/__init__.py
--rw-r--r--   0        0        0      879 2024-04-03 11:11:32.380073 robotframework_reportmodifier-0.2.4/src/ReportModifierListener/ReportModifierListener.py
--rw-r--r--   0        0        0     5400 1970-01-01 00:00:00.000000 robotframework_reportmodifier-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35801 2024-02-12 08:28:04.348570 robotframework_reportmodifier-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1988 2024-05-14 12:27:24.265388 robotframework_reportmodifier-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4848 2024-04-03 11:11:32.367186 robotframework_reportmodifier-0.2.5/README.md
+-rw-r--r--   0        0        0       44 2024-03-28 08:26:32.278869 robotframework_reportmodifier-0.2.5/src/reportmodifier/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-15 06:52:24.460202 robotframework_reportmodifier-0.2.5/src/reportmodifier/__version__.py
+-rw-r--r--   0        0        0     1664 2024-04-03 11:11:32.397501 robotframework_reportmodifier-0.2.5/src/reportmodifier/_file_tools.py
+-rw-r--r--   0        0        0     5981 2024-04-03 11:11:32.400497 robotframework_reportmodifier-0.2.5/src/reportmodifier/_report_configuration.py
+-rw-r--r--   0        0        0     6945 2024-05-15 06:55:47.337400 robotframework_reportmodifier-0.2.5/src/reportmodifier/ReportModifier.py
+-rw-r--r--   0        0        0    12306 2024-05-15 06:55:47.339268 robotframework_reportmodifier-0.2.5/src/reportmodifier/ReportModifierVisitor.py
+-rw-r--r--   0        0        0       79 2024-04-03 11:11:32.384485 robotframework_reportmodifier-0.2.5/src/ReportModifierListener/__init__.py
+-rw-r--r--   0        0        0      879 2024-04-03 11:11:32.380073 robotframework_reportmodifier-0.2.5/src/ReportModifierListener/ReportModifierListener.py
+-rw-r--r--   0        0        0     5400 1970-01-01 00:00:00.000000 robotframework_reportmodifier-0.2.5/PKG-INFO
```

### Comparing `robotframework_reportmodifier-0.2.4/LICENSE` & `robotframework_reportmodifier-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.4/pyproject.toml` & `robotframework_reportmodifier-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2272 6f62 6f74 6672 616d  ame = "robotfram
 00000020: 6577 6f72 6b2d 7265 706f 7274 6d6f 6469  ework-reportmodi
 00000030: 6669 6572 220d 0a76 6572 7369 6f6e 203d  fier"..version =
-00000040: 2022 302e 322e 3422 0d0a 6465 7363 7269   "0.2.4"..descri
+00000040: 2022 302e 322e 3522 0d0a 6465 7363 7269   "0.2.5"..descri
 00000050: 7074 696f 6e20 3d20 2246 696c 7465 7220  ption = "Filter 
 00000060: 7265 706f 7274 2063 6f6e 7465 6e74 2e22  report content."
 00000070: 0d0a 6175 7468 6f72 7320 3d20 5b22 4d61  ..authors = ["Ma
 00000080: 7474 6869 6173 2047 756e 7468 6572 203c  tthias Gunther <
 00000090: 6d61 7474 6869 6173 6775 6e74 6865 7240  matthiasgunther@
 000000a0: 676d 6169 6c2e 636f 6d3e 225d 0d0a 686f  gmail.com>"]..ho
 000000b0: 6d65 7061 6765 203d 2022 6874 7470 733a  mepage = "https:
```

### Comparing `robotframework_reportmodifier-0.2.4/README.md` & `robotframework_reportmodifier-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.4/src/reportmodifier/_file_tools.py` & `robotframework_reportmodifier-0.2.5/src/reportmodifier/_file_tools.py`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.4/src/reportmodifier/_report_configuration.py` & `robotframework_reportmodifier-0.2.5/src/reportmodifier/_report_configuration.py`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.4/src/reportmodifier/ReportModifier.py` & `robotframework_reportmodifier-0.2.5/src/reportmodifier/ReportModifier.py`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.4/src/reportmodifier/ReportModifierVisitor.py` & `robotframework_reportmodifier-0.2.5/src/reportmodifier/ReportModifierVisitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.report_configuration = ReportConfiguration(None)
         self.basic_configuration = ReportConfiguration(None)
         self.__report_name = None
         self.__keyword_calls = defaultdict(int)
         self._relevant_keyword_calls = []
         self._relevant_messages = defaultdict(list)
         self._keyword = None
-        self._keyword_path = ""
+        self._keyword_path = None
         self.__root = None
         self._tests = []
 
     @property
     def report_name(self):
         if self.__report_name is None:
             return "custom_log"
@@ -64,26 +64,25 @@
                     top_level_dir=test_dir,
                     condition_callback=lambda p: Path(p).stem.lower() == report_configuration  # noqa: B023
                     and Path(p).suffix == ".yaml",
                     recursive=True,
                 )
                 if not configuration_path:
                     logger.error(
-                        f'Could not find custon log configuration "{report_configuration}" of test  {test.name}',
+                        f'Could not find custom log configuration "{report_configuration}" of test  {test.name}',
                     )
                     return False
                 path = list(configuration_path.values())[0]
                 logger.info(f"Found log configuration of fest: {test.name}: {tag} {path}")
                 if report_configuration.lower() == "basic_config":
                     self.basic_configuration = ReportConfiguration(path)
                 else:
                     self.report_configuration = ReportConfiguration(path)
                     if self.__report_name is None:
                         self.__report_name = report_configuration
-                break
 
     def end_test(self, test: TestCase):
         if self.report_configuration or self.basic_configuration:
             test.body.clear()
             for keyword, messages in self._relevant_messages.items():
                 if keyword and messages:
                     keyword.libname = ""
@@ -103,16 +102,21 @@
             logger.debug(f"Checking {keyword.kwname} --> {keyword.libname} --> {keyword.parent.name}")
             self.__keyword_calls[keyword.kwname] += 1
             if _keyword_name_for_structure_is_relevant(
                 keyword.kwname,
                 [k.name for k in self.report_configuration.keyword_as_structure]
                 + [k.name for k in self.basic_configuration.keyword_as_structure],
             ):
-                self._keyword = keyword
-                self._keyword_path = _get_keyword_call_path(keyword)
+                if (
+                    self._keyword_path is None
+                    or self._keyword_path == _get_keyword_call_path(keyword)
+                    or self._keyword_path not in _get_keyword_call_path(keyword)
+                ):
+                    self._keyword = keyword
+                    self._keyword_path = _get_keyword_call_path(keyword)
             if _keyword_name_as_info_is_relevant(keyword, self.report_configuration, self.basic_configuration):
                 msg = f'<b><mark style="background:powderblue">{keyword.name.strip()}</mark></b>\n{keyword.doc.strip()}'
                 message = Message(msg, level="INFO", html=True, timestamp=keyword.starttime)
                 self._relevant_messages[self._keyword].append(message)
                 self._relevant_keyword_calls.append(_get_keyword_call_path(keyword))
             if _all_keyword_messages_are_relevant(
                 keyword,
```

### Comparing `robotframework_reportmodifier-0.2.4/src/ReportModifierListener/ReportModifierListener.py` & `robotframework_reportmodifier-0.2.5/src/ReportModifierListener/ReportModifierListener.py`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.4/PKG-INFO` & `robotframework_reportmodifier-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-reportmodifier
-Version: 0.2.4
+Version: 0.2.5
 Summary: Filter report content.
 Home-page: https://github.com/MarketSquare/robotframework-reportmodifier
 Author: Matthias Gunther
 Author-email: matthiasgunther@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

