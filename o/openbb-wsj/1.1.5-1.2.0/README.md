# Comparing `tmp/openbb_wsj-1.1.5.tar.gz` & `tmp/openbb_wsj-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_wsj-1.1.5.tar", max compression
+gzip compressed data, was "openbb_wsj-1.2.0.tar", max compression
```

## Comparing `openbb_wsj-1.1.5.tar` & `openbb_wsj-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      427 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/README.md
--rw-r--r--   0        0        0     1044 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-04-17 12:33:20.849645 openbb_wsj-1.1.5/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0      433 2024-04-19 16:42:48.787460 openbb_wsj-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 openbb_wsj-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-05-15 14:24:28.442108 openbb_wsj-1.2.0/README.md
+-rw-r--r--   0        0        0     1071 2024-05-14 15:30:05.621595 openbb_wsj-1.2.0/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-02-29 11:03:36.977934 openbb_wsj-1.2.0/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-04-08 12:02:16.764578 openbb_wsj-1.2.0/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-04-08 12:02:16.764674 openbb_wsj-1.2.0/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0      459 2024-05-15 16:05:29.883147 openbb_wsj-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 openbb_wsj-1.2.0/PKG-INFO
```

### Comparing `openbb_wsj-1.1.5/openbb_wsj/__init__.py` & `openbb_wsj-1.2.0/openbb_wsj/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 from openbb_core.provider.abstract.provider import Provider
 from openbb_wsj.models.active import WSJActiveFetcher
 from openbb_wsj.models.gainers import WSJGainersFetcher
 from openbb_wsj.models.losers import WSJLosersFetcher
 
 wsj_provider = Provider(
     name="wsj",
-    website="www.wsj.com",
+    website="https://www.wsj.com",
     description="""WSJ (Wall Street Journal) is a business-focused, English-language
-    international daily newspaper based in New York City. The Journal is published six
-    days a week by Dow Jones & Company, a division of News Corp, along with its Asian
-    and European editions. The newspaper is published in the broadsheet format and
-    online. The Journal has been printed continuously since its inception on
-    July 8, 1889, by Charles Dow, Edward Jones, and Charles Bergstresser.
-    The WSJ is the largest newspaper in the United States, by circulation.
+international daily newspaper based in New York City. The Journal is published six
+days a week by Dow Jones & Company, a division of News Corp, along with its Asian
+and European editions. The newspaper is published in the broadsheet format and
+online. The Journal has been printed continuously since its inception on
+July 8, 1889, by Charles Dow, Edward Jones, and Charles Bergstresser.
+The WSJ is the largest newspaper in the United States, by circulation.
     """,
     fetcher_dict={
         "ETFGainers": WSJGainersFetcher,
         "ETFLosers": WSJLosersFetcher,
         "ETFActive": WSJActiveFetcher,
     },
+    repr_name="Wall Street Journal (WSJ)",
 )
```

### Comparing `openbb_wsj-1.1.5/openbb_wsj/models/active.py` & `openbb_wsj-1.2.0/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.1.5/openbb_wsj/models/gainers.py` & `openbb_wsj-1.2.0/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.1.5/openbb_wsj/models/losers.py` & `openbb_wsj-1.2.0/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.1.5/PKG-INFO` & `openbb_wsj-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-wsj
-Version: 1.1.5
+Version: 1.2.0
 Summary: wsj extension for OpenBB
+License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Wall St Journal Provider
 
 This extension integrates the [WSJ](https://wsj.com/) data provider into the OpenBB Platform.
 
 ## Installation
 
 To install the extension:
 
 ```bash
 pip install openbb-wsj
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

