# Comparing `tmp/xml_from_seq-0.3.2.tar.gz` & `tmp/xml_from_seq-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xml_from_seq-0.3.2.tar", last modified: Sun Feb 11 04:30:11 2024, max compression
+gzip compressed data, was "xml_from_seq-0.3.3.tar", last modified: Wed May 15 14:46:41 2024, max compression
```

## Comparing `xml_from_seq-0.3.2.tar` & `xml_from_seq-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nicwolff   (502) admin       (80)        0 2024-02-11 04:30:11.438279 xml_from_seq-0.3.2/
--rw-r--r--   0 nicwolff   (502) admin       (80)       33 2022-08-03 00:53:50.000000 xml_from_seq-0.3.2/MANIFEST.in
--rw-r--r--   0 nicwolff   (502) admin       (80)     2374 2024-02-11 04:30:11.438073 xml_from_seq-0.3.2/PKG-INFO
--rw-r--r--   0 nicwolff   (502) admin       (80)     1967 2024-02-11 04:29:04.000000 xml_from_seq-0.3.2/README.md
--rw-r--r--   0 nicwolff   (502) admin       (80)       38 2024-02-11 04:30:11.438318 xml_from_seq-0.3.2/setup.cfg
--rw-r--r--   0 nicwolff   (502) admin       (80)      615 2024-02-11 04:22:56.000000 xml_from_seq-0.3.2/setup.py
--rw-r--r--   0 nicwolff   (502) admin       (80)      888 2024-02-11 04:28:01.000000 xml_from_seq-0.3.2/test.py
-drwxr-xr-x   0 nicwolff   (502) admin       (80)        0 2024-02-11 04:30:11.437887 xml_from_seq-0.3.2/xml_from_seq.egg-info/
--rw-r--r--   0 nicwolff   (502) admin       (80)     2374 2024-02-11 04:30:11.000000 xml_from_seq-0.3.2/xml_from_seq.egg-info/PKG-INFO
--rw-r--r--   0 nicwolff   (502) admin       (80)      198 2024-02-11 04:30:11.000000 xml_from_seq-0.3.2/xml_from_seq.egg-info/SOURCES.txt
--rw-r--r--   0 nicwolff   (502) admin       (80)        1 2024-02-11 04:30:11.000000 xml_from_seq-0.3.2/xml_from_seq.egg-info/dependency_links.txt
--rw-r--r--   0 nicwolff   (502) admin       (80)       13 2024-02-11 04:30:11.000000 xml_from_seq-0.3.2/xml_from_seq.egg-info/top_level.txt
--rw-r--r--   0 nicwolff   (502) admin       (80)     2030 2024-02-11 04:29:30.000000 xml_from_seq-0.3.2/xml_from_seq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:46:41.326979 xml_from_seq-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-15 14:42:40.000000 xml_from_seq-0.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-05-15 14:46:41.326543 xml_from_seq-0.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1967 2024-05-15 14:42:40.000000 xml_from_seq-0.3.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 14:46:41.327126 xml_from_seq-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      622 2024-05-15 14:42:40.000000 xml_from_seq-0.3.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-05-15 14:42:40.000000 xml_from_seq-0.3.3/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:46:41.326091 xml_from_seq-0.3.3/xml_from_seq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-05-15 14:46:41.000000 xml_from_seq-0.3.3/xml_from_seq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      198 2024-05-15 14:46:41.000000 xml_from_seq-0.3.3/xml_from_seq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 14:46:41.000000 xml_from_seq-0.3.3/xml_from_seq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-15 14:46:41.000000 xml_from_seq-0.3.3/xml_from_seq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-05-15 14:42:40.000000 xml_from_seq-0.3.3/xml_from_seq.py
```

### Comparing `xml_from_seq-0.3.2/PKG-INFO` & `xml_from_seq-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xml_from_seq
-Version: 0.3.2
+Version: 0.3.3
 Summary: Generate XML from Python data structure
-Home-page: https://github.com/nicwolff/xml_from_seq
+Home-page: https://github.com/Media-Platforms/xml_from_seq
 Author: Nic Wolff
 Author-email: nwolff@hearst.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `xml_from_seq-0.3.2/README.md` & `xml_from_seq-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `xml_from_seq-0.3.2/setup.py` & `xml_from_seq-0.3.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from unittest import defaultTestLoader
 from setuptools import setup
 
 setup(
     name='xml_from_seq',
-    version='0.3.2',
+    version='0.3.3',
     description='Generate XML from Python data structure',
     author='Nic Wolff',
     author_email='nwolff@hearst.com',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    url='https://github.com/nicwolff/xml_from_seq',
+    url='https://github.com/Media-Platforms/xml_from_seq',
     py_modules=['xml_from_seq'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `xml_from_seq-0.3.2/test.py` & `xml_from_seq-0.3.3/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,10 +18,14 @@
     def test_end_tag(self):
         assert end_tag('foo') == '</foo>'
 
     def test_XMLdecl(self):
         x = XMLdecl(xmlns='http://example.com/foo.xml')
         assert x == '<?xml version="1.0" xmlns="http://example.com/foo.xml"?>\n'
 
+    def test_zero_value(self):
+        b = ['duration', INLINE, 0]
+        assert XML(b) == '<duration>0</duration>\n'
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xml_from_seq-0.3.2/xml_from_seq.egg-info/PKG-INFO` & `xml_from_seq-0.3.3/xml_from_seq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xml_from_seq
-Version: 0.3.2
+Version: 0.3.3
 Summary: Generate XML from Python data structure
-Home-page: https://github.com/nicwolff/xml_from_seq
+Home-page: https://github.com/Media-Platforms/xml_from_seq
 Author: Nic Wolff
 Author-email: nwolff@hearst.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `xml_from_seq-0.3.2/xml_from_seq.py` & `xml_from_seq-0.3.3/xml_from_seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def XML(*seq, indent=0, cr=True):
     e = partial(element_or_text, i=indent, cr=cr)
     return ''.join(filter(None, map(e, seq)))
 
 
 def element_or_text(x, i=0, cr=True):
-    if x in (False, None):
+    if x is False or x is None:
         return ''
     t = '\n' if cr else ''
     if is_seq(x):
         return element(*x, i=i) + t
     return ('\t' * i) + escape(str(x)) + t
```

