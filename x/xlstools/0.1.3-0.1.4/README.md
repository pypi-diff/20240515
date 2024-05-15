# Comparing `tmp/xlstools-0.1.3.tar.gz` & `tmp/xlstools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlstools-0.1.3.tar", last modified: Tue Feb 21 09:12:30 2023, max compression
+gzip compressed data, was "xlstools-0.1.4.tar", last modified: Wed May 15 21:45:49 2024, max compression
```

## Comparing `xlstools-0.1.3.tar` & `xlstools-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-02-21 09:12:30.815425 xlstools-0.1.3/
--rw-r--r--   0 b          (500) b          (506)     1553 2022-04-08 17:49:25.000000 xlstools-0.1.3/LICENSE
--rw-r--r--   0 b          (500) b          (506)     2215 2023-02-21 09:12:30.815425 xlstools-0.1.3/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     1961 2022-04-08 18:08:16.000000 xlstools-0.1.3/README.md
--rw-r--r--   0 b          (500) b          (506)       38 2023-02-21 09:12:30.815425 xlstools-0.1.3/setup.cfg
--rw-r--r--   0 b          (500) b          (506)      933 2023-02-21 09:12:20.000000 xlstools-0.1.3/setup.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-02-21 09:12:30.815425 xlstools-0.1.3/xlstools/
--rw-r--r--   0 b          (500) b          (506)     1324 2022-04-08 17:59:31.000000 xlstools-0.1.3/xlstools/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2689 2022-05-03 19:29:57.000000 xlstools-0.1.3/xlstools/csv_reader.py
--rw-r--r--   0 b          (500) b          (506)    12933 2023-02-09 00:49:06.000000 xlstools-0.1.3/xlstools/google_sheet_reader.py
--rw-r--r--   0 b          (500) b          (506)      722 2022-05-03 19:29:57.000000 xlstools-0.1.3/xlstools/open_xl.py
--rw-r--r--   0 b          (500) b          (506)     3317 2022-01-26 09:04:58.000000 xlstools-0.1.3/xlstools/openpyxlrd.py
--rw-r--r--   0 b          (500) b          (506)     1373 2022-05-03 19:36:14.000000 xlstools-0.1.3/xlstools/pd_emulator.py
--rw-r--r--   0 b          (500) b          (506)      826 2022-01-11 21:26:45.000000 xlstools-0.1.3/xlstools/util.py
--rw-r--r--   0 b          (500) b          (506)     3072 2022-01-26 08:26:58.000000 xlstools-0.1.3/xlstools/xl_reader.py
--rw-r--r--   0 b          (500) b          (506)    14564 2022-05-04 20:20:00.000000 xlstools-0.1.3/xlstools/xl_sheet.py
--rw-r--r--   0 b          (500) b          (506)     4588 2023-02-21 08:14:57.000000 xlstools-0.1.3/xlstools/xlrd_like.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-02-21 09:12:30.815425 xlstools-0.1.3/xlstools.egg-info/
--rw-r--r--   0 b          (500) b          (506)     2215 2023-02-21 09:12:30.000000 xlstools-0.1.3/xlstools.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)      410 2023-02-21 09:12:30.000000 xlstools-0.1.3/xlstools.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2023-02-21 09:12:30.000000 xlstools-0.1.3/xlstools.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)       90 2023-02-21 09:12:30.000000 xlstools-0.1.3/xlstools.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)        9 2023-02-21 09:12:30.000000 xlstools-0.1.3/xlstools.egg-info/top_level.txt
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 21:45:49.615706 xlstools-0.1.4/
+-rw-r--r--   0 b          (500) b          (506)     1553 2022-04-08 17:49:25.000000 xlstools-0.1.4/LICENSE
+-rw-r--r--   0 b          (500) b          (506)     2393 2024-05-15 21:45:49.612373 xlstools-0.1.4/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     1961 2022-04-08 18:08:16.000000 xlstools-0.1.4/README.md
+-rw-r--r--   0 b          (500) b          (506)       38 2024-05-15 21:45:49.615706 xlstools-0.1.4/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     1009 2024-05-15 21:36:32.000000 xlstools-0.1.4/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 21:45:49.612373 xlstools-0.1.4/xlstools/
+-rw-r--r--   0 b          (500) b          (506)     1324 2022-04-08 17:59:31.000000 xlstools-0.1.4/xlstools/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2689 2022-05-03 19:29:57.000000 xlstools-0.1.4/xlstools/csv_reader.py
+-rw-r--r--   0 b          (500) b          (506)    13053 2024-05-14 19:11:45.000000 xlstools-0.1.4/xlstools/google_sheet_reader.py
+-rw-r--r--   0 b          (500) b          (506)      722 2022-05-03 19:29:57.000000 xlstools-0.1.4/xlstools/open_xl.py
+-rw-r--r--   0 b          (500) b          (506)     3321 2023-07-10 07:19:39.000000 xlstools-0.1.4/xlstools/openpyxlrd.py
+-rw-r--r--   0 b          (500) b          (506)     1373 2022-05-03 19:36:14.000000 xlstools-0.1.4/xlstools/pd_emulator.py
+-rw-r--r--   0 b          (500) b          (506)      826 2022-01-11 21:26:45.000000 xlstools-0.1.4/xlstools/util.py
+-rw-r--r--   0 b          (500) b          (506)     3072 2022-01-26 08:26:58.000000 xlstools-0.1.4/xlstools/xl_reader.py
+-rw-r--r--   0 b          (500) b          (506)    14564 2022-05-04 20:20:00.000000 xlstools-0.1.4/xlstools/xl_sheet.py
+-rw-r--r--   0 b          (500) b          (506)     4588 2023-02-21 08:14:57.000000 xlstools-0.1.4/xlstools/xlrd_like.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 21:45:49.612373 xlstools-0.1.4/xlstools.egg-info/
+-rw-r--r--   0 b          (500) b          (506)     2393 2024-05-15 21:45:49.000000 xlstools-0.1.4/xlstools.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)      410 2024-05-15 21:45:49.000000 xlstools-0.1.4/xlstools.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2024-05-15 21:45:49.000000 xlstools-0.1.4/xlstools.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)       90 2024-05-15 21:45:49.000000 xlstools-0.1.4/xlstools.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)        9 2024-05-15 21:45:49.000000 xlstools-0.1.4/xlstools.egg-info/top_level.txt
```

### Comparing `xlstools-0.1.3/LICENSE` & `xlstools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/PKG-INFO` & `xlstools-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: xlstools
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/scope3/xls-tools
 Author: Brandon Kuczenski
 Author-email: brandon@scope3consulting.com
 Description-Content-Type: text/markdown
-Provides-Extra: gsheet
 License-File: LICENSE
+Requires-Dist: xlrd>=2.0.0
+Requires-Dist: openpyxl>=3.0.7
+Provides-Extra: gsheet
+Requires-Dist: google-api-python-client>=2.2.0; extra == "gsheet"
+Requires-Dist: oauth2client>=4.1.3; extra == "gsheet"
 
 # xls-tools
 Excel and Excel-like tools
 
 # xlrd_like
 
 A minimal interface for accessing excel-type files using the `xlrd` API:
```

### Comparing `xlstools-0.1.3/README.md` & `xlstools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/setup.py` & `xlstools-0.1.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 
 0.1.1 - 1 August 2022 - add CSV reader (with pandas emulation!)
         change package name to xlstools
         
 0.1.2 - 19 February 2023 - finish csv; add write class
 
 0.1.3 - 21 February 2023 - dumb abc error. we should think about writing some tests :P
+
+0.1.4 - 15 May 2024 - bugfixes: Openpyxl workbook name; gsheet empty-sheet
 """
 
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 
 setup(
     name="xlstools",
     version=VERSION,
     author="Brandon Kuczenski",
     author_email="brandon@scope3consulting.com",
     install_requires=requires,
```

### Comparing `xlstools-0.1.3/xlstools/__init__.py` & `xlstools-0.1.4/xlstools/__init__.py`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/xlstools/csv_reader.py` & `xlstools-0.1.4/xlstools/csv_reader.py`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/xlstools/google_sheet_reader.py` & `xlstools-0.1.4/xlstools/google_sheet_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class GSheetEmulator(XlrdSheetLike):
     def __init__(self, value_data):
         """
 
         :param value_data: must follow the google sheets v4 API .spreadsheets().values().get(... range=sheetname)
         """
-        if len(value_data['values']) == 0:
+        if len(value_data.get('values', [])) == 0:
             _nr = _nc = 0
             data = [[]]
         else:
             if value_data['majorDimension'] == 'ROWS':
                 data = value_data['values']
             elif value_data['majorDimension'] == 'COLUMNS':
                 raise NotImplementedError
@@ -147,15 +147,19 @@
         """
         quoted_sheetname = "'%s'" % sheetname  # without quotes it may be interpreted as a named range
         req = self._res.spreadsheets().values().get(spreadsheetId=self._sheet_id, range=quoted_sheetname)
         try:
             d = req.execute()
         except HttpError:
             raise KeyError('Unable to open sheet %s' % sheetname)
-        return GSheetEmulator(d)
+        try:
+            return GSheetEmulator(d)
+        except KeyError:
+            print('failed GSheet instantiation')
+            return d
 
     def sheet_by_index(self, index):
         return self.sheet_by_name(self._sheetnames[index])
 
     def sheets(self):
         """
         No sheet caching!
```

### Comparing `xlstools-0.1.3/xlstools/open_xl.py` & `xlstools-0.1.4/xlstools/open_xl.py`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/xlstools/openpyxlrd.py` & `xlstools-0.1.4/xlstools/openpyxlrd.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,8 +117,8 @@
         return self._sheets[index]
 
     def sheets(self):
         return self._sheets
 
     @property
     def filename(self):
-        return self._book.file
+        return 'openpyxl-workbook'
```

### Comparing `xlstools-0.1.3/xlstools/pd_emulator.py` & `xlstools-0.1.4/xlstools/pd_emulator.py`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/xlstools/util.py` & `xlstools-0.1.4/xlstools/util.py`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/xlstools/xl_reader.py` & `xlstools-0.1.4/xlstools/xl_reader.py`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/xlstools/xl_sheet.py` & `xlstools-0.1.4/xlstools/xl_sheet.py`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/xlstools/xlrd_like.py` & `xlstools-0.1.4/xlstools/xlrd_like.py`

 * *Files identical despite different names*

### Comparing `xlstools-0.1.3/xlstools.egg-info/PKG-INFO` & `xlstools-0.1.4/xlstools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: xlstools
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/scope3/xls-tools
 Author: Brandon Kuczenski
 Author-email: brandon@scope3consulting.com
 Description-Content-Type: text/markdown
-Provides-Extra: gsheet
 License-File: LICENSE
+Requires-Dist: xlrd>=2.0.0
+Requires-Dist: openpyxl>=3.0.7
+Provides-Extra: gsheet
+Requires-Dist: google-api-python-client>=2.2.0; extra == "gsheet"
+Requires-Dist: oauth2client>=4.1.3; extra == "gsheet"
 
 # xls-tools
 Excel and Excel-like tools
 
 # xlrd_like
 
 A minimal interface for accessing excel-type files using the `xlrd` API:
```

