# Comparing `tmp/simpledali-0.8.0.tar.gz` & `tmp/simpledali-0.8.1.tar.gz`

## Comparing `simpledali-0.8.0.tar` & `simpledali-0.8.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 simpledali-0.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 simpledali-0.8.0/build-hints.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 simpledali-0.8.0/token
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/make.bat
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/.gitignore
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/conf.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/index.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/readme_link.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/requirements.txt
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/index.rst
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.abstractdali.rst
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.dali2jsonl.rst
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.dalipacket.rst
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.jsonencoder.rst
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.rst
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.socketdali.rst
--rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.util.rst
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.websocketdali.rst
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/.gitignore
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/README.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/dali2jsonl.toml
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/getid.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/readdali.py
--rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/ring.conf
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/sendBzJsonPacket.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/sendJsonPacket.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/sendMSeed3Packet.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/sendMSeedPacket.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/ring/.gitignore
--rw-r--r--   0        0        0  1048576 2020-02-02 00:00:00.000000 simpledali-0.8.0/example/ring/packetbuf
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 simpledali-0.8.0/src/simpledali/__init__.py
--rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 simpledali-0.8.0/src/simpledali/abstractdali.py
--rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 simpledali-0.8.0/src/simpledali/dali2jsonl.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 simpledali-0.8.0/src/simpledali/dalipacket.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 simpledali-0.8.0/src/simpledali/jsonencoder.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 simpledali-0.8.0/src/simpledali/socketdali.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 simpledali-0.8.0/src/simpledali/util.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 simpledali-0.8.0/src/simpledali/websocketdali.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 simpledali-0.8.0/tools/print_info.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 simpledali-0.8.0/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 simpledali-0.8.0/LICENSE
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 simpledali-0.8.0/README.md
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 simpledali-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 simpledali-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 simpledali-0.8.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 simpledali-0.8.1/build-hints.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 simpledali-0.8.1/token
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/make.bat
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/.gitignore
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/conf.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/index.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/readme_link.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/requirements.txt
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/index.rst
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.abstractdali.rst
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.dali2jsonl.rst
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.dalipacket.rst
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.jsonencoder.rst
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.rst
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.socketdali.rst
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.util.rst
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.websocketdali.rst
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/.gitignore
+-rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/README.md
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/TestSimpleDali.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/dali2jsonl.toml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/getid.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/readdali.py
+-rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/ring.conf
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/sendBzJsonPacket.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/sendJsonPacket.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/sendMSeed3Packet.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/sendMSeedPacket.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/ring/.gitignore
+-rw-r--r--   0        0        0  1048576 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/ring/packetbuf
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 simpledali-0.8.1/example/ring/streamidx
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 simpledali-0.8.1/src/simpledali/__init__.py
+-rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 simpledali-0.8.1/src/simpledali/abstractdali.py
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 simpledali-0.8.1/src/simpledali/dali2jsonl.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 simpledali-0.8.1/src/simpledali/dalipacket.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 simpledali-0.8.1/src/simpledali/jsonencoder.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 simpledali-0.8.1/src/simpledali/socketdali.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 simpledali-0.8.1/src/simpledali/util.py
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 simpledali-0.8.1/src/simpledali/websocketdali.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 simpledali-0.8.1/tools/print_info.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 simpledali-0.8.1/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 simpledali-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 simpledali-0.8.1/README.md
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 simpledali-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 simpledali-0.8.1/PKG-INFO
```

### Comparing `simpledali-0.8.0/.readthedocs.yaml` & `simpledali-0.8.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/build-hints.md` & `simpledali-0.8.1/build-hints.md`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/Makefile` & `simpledali-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/make.bat` & `simpledali-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/source/conf.py` & `simpledali-0.8.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'SimpleDali'
 copyright = '2024, Philip Crotwell'
 author = 'Philip Crotwell'
 release = '0.8'
-version = '0.8.0'
+version = '0.8.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
```

### Comparing `simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.abstractdali.rst` & `simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.abstractdali.rst`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.dali2jsonl.rst` & `simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.dali2jsonl.rst`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.dalipacket.rst` & `simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.dalipacket.rst`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.jsonencoder.rst` & `simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.jsonencoder.rst`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.rst` & `simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.rst`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
           :summary:
 
 API
 ~~~
 
 .. py:data:: __version__
    :canonical: simpledali.__version__
-   :value: '0.8.0'
+   :value: '0.8.1'
 
    .. autodoc2-docstring:: simpledali.__version__
 
 .. py:data:: __all__
    :canonical: simpledali.__all__
    :value: ['DataLink', 'DaliResponse', 'DaliPacket', 'DaliException', 'nslcToStreamId', 'fdsnSourceIdToStreamI...
```

### Comparing `simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.socketdali.rst` & `simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.socketdali.rst`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.util.rst` & `simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.util.rst`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/docs/source/apidocs/simpledali/simpledali.websocketdali.rst` & `simpledali-0.8.1/docs/source/apidocs/simpledali/simpledali.websocketdali.rst`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/README.md` & `simpledali-0.8.1/example/README.md`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/dali2jsonl.toml` & `simpledali-0.8.1/example/dali2jsonl.toml`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/getid.py` & `simpledali-0.8.1/example/getid.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/readdali.py` & `simpledali-0.8.1/example/readdali.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/ring.conf` & `simpledali-0.8.1/example/ring.conf`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/sendBzJsonPacket.py` & `simpledali-0.8.1/example/sendBzJsonPacket.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/sendJsonPacket.py` & `simpledali-0.8.1/example/sendJsonPacket.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/sendMSeed3Packet.py` & `simpledali-0.8.1/example/sendMSeed3Packet.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/example/sendMSeedPacket.py` & `simpledali-0.8.1/example/sendMSeedPacket.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/src/simpledali/__init__.py` & `simpledali-0.8.1/src/simpledali/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 from .abstractdali import DataLink
 from .dalipacket import (
     DaliPacket,
     DaliResponse,
     DaliException,
     nslcToStreamId,
```

### Comparing `simpledali-0.8.0/src/simpledali/abstractdali.py` & `simpledali-0.8.1/src/simpledali/abstractdali.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/src/simpledali/dali2jsonl.py` & `simpledali-0.8.1/src/simpledali/dali2jsonl.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/src/simpledali/dalipacket.py` & `simpledali-0.8.1/src/simpledali/dalipacket.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/src/simpledali/socketdali.py` & `simpledali-0.8.1/src/simpledali/socketdali.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/src/simpledali/util.py` & `simpledali-0.8.1/src/simpledali/util.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/src/simpledali/websocketdali.py` & `simpledali-0.8.1/src/simpledali/websocketdali.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/tools/print_info.py` & `simpledali-0.8.1/tools/print_info.py`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/.gitignore` & `simpledali-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/LICENSE` & `simpledali-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpledali-0.8.0/README.md` & `simpledali-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,8 +80,8 @@
 write='/data/scsn/www/jsonl/%n/%s/%Y/%j/%n.%s.%l.%c.%Y.%j.%H.jsonl'
 
 ```
 
 # Example
 
 There are examples of sending and receiving Datalink packets in the
-[example directory](https://github.com/crotwell/simplemseed/tree/main/examples).
+[example directory](https://github.com/crotwell/simplemdali/tree/main/examples).
```

### Comparing `simpledali-0.8.0/pyproject.toml` & `simpledali-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "simplemseed >= 0.3.0",
+    "simplemseed >= 0.3.1",
     "defusedxml",
     "pyjwt",
     "websockets",
     'tomli >= 1.1.0 ; python_version < "3.11"',
     'importlib-metadata; python_version<"3.10"',
 ]
```

### Comparing `simpledali-0.8.0/PKG-INFO` & `simpledali-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: simpledali
-Version: 0.8.0
+Version: 0.8.1
 Summary: Datalink protocol in python
 Project-URL: Homepage, https://github.com/crotwell/simpledali
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/crotwell/simpledali
 Project-URL: Issues, https://github.com/crotwell/simpledali/issues
 Author-email: Philip Crotwell <crotwell@seis.sc.edu>
 License-File: LICENSE
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: defusedxml
 Requires-Dist: importlib-metadata; python_version < '3.10'
 Requires-Dist: pyjwt
-Requires-Dist: simplemseed>=0.3.0
+Requires-Dist: simplemseed>=0.3.1
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Requires-Dist: websockets
 Description-Content-Type: text/markdown
 
 # simpledali
 
 [![PyPI](https://img.shields.io/pypi/v/simpledali)](https://pypi.org/project/simpledali/)
@@ -103,8 +103,8 @@
 write='/data/scsn/www/jsonl/%n/%s/%Y/%j/%n.%s.%l.%c.%Y.%j.%H.jsonl'
 
 ```
 
 # Example
 
 There are examples of sending and receiving Datalink packets in the
-[example directory](https://github.com/crotwell/simplemseed/tree/main/examples).
+[example directory](https://github.com/crotwell/simplemdali/tree/main/examples).
```

