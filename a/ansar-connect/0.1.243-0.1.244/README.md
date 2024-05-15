# Comparing `tmp/ansar_connect-0.1.243.tar.gz` & `tmp/ansar_connect-0.1.244.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.243.tar", last modified: Tue May 14 16:40:54 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.244.tar", last modified: Tue May 14 16:45:29 2024, max compression
```

## Comparing `ansar_connect-0.1.243.tar` & `ansar_connect-0.1.244.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:40:54.179022 ansar_connect-0.1.243/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.243/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-14 16:40:54.179022 ansar_connect-0.1.243/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.243/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-14 16:40:37.000000 ansar_connect-0.1.243/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-14 16:40:54.179022 ansar_connect-0.1.243/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-14 16:40:30.000000 ansar_connect-0.1.243/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:40:54.175022 ansar_connect-0.1.243/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:40:54.175022 ansar_connect-0.1.243/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:40:54.179022 ansar_connect-0.1.243/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.243/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.243/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.243/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.243/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:40:54.179022 ansar_connect-0.1.243/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-14 16:40:51.000000 ansar_connect-0.1.243/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.243/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.243/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.243/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10461 2024-05-10 15:14:29.000000 ansar_connect-0.1.243/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.243/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.243/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.243/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.243/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.243/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.243/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.243/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33894 2024-05-13 17:10:04.000000 ansar_connect-0.1.243/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.243/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.243/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.243/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.243/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.243/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.243/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:40:54.179022 ansar_connect-0.1.243/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-14 16:40:54.000000 ansar_connect-0.1.243/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-14 16:40:54.000000 ansar_connect-0.1.243/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-14 16:40:54.000000 ansar_connect-0.1.243/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-14 16:40:54.000000 ansar_connect-0.1.243/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-14 16:40:54.000000 ansar_connect-0.1.243/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-14 16:40:54.000000 ansar_connect-0.1.243/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:45:29.296140 ansar_connect-0.1.244/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.244/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-14 16:45:29.296140 ansar_connect-0.1.244/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.244/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-14 16:45:18.000000 ansar_connect-0.1.244/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-14 16:45:29.296140 ansar_connect-0.1.244/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-14 16:45:11.000000 ansar_connect-0.1.244/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:45:29.292140 ansar_connect-0.1.244/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:45:29.292140 ansar_connect-0.1.244/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:45:29.292140 ansar_connect-0.1.244/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.244/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.244/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.244/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.244/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:45:29.296140 ansar_connect-0.1.244/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-14 16:45:26.000000 ansar_connect-0.1.244/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.244/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.244/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.244/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10461 2024-05-10 15:14:29.000000 ansar_connect-0.1.244/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.244/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.244/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.244/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.244/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.244/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.244/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.244/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33894 2024-05-13 17:10:04.000000 ansar_connect-0.1.244/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.244/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.244/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.244/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.244/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.244/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.244/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:45:29.296140 ansar_connect-0.1.244/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-14 16:45:29.000000 ansar_connect-0.1.244/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-14 16:45:29.000000 ansar_connect-0.1.244/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-14 16:45:29.000000 ansar_connect-0.1.244/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-14 16:45:29.000000 ansar_connect-0.1.244/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-14 16:45:29.000000 ansar_connect-0.1.244/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-14 16:45:29.000000 ansar_connect-0.1.244/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.243/LICENSE` & `ansar_connect-0.1.244/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/PKG-INFO` & `ansar_connect-0.1.244/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.243
+Version: 0.1.244
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.85
+Requires-Dist: ansar-create>=0.1.86
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
 messaging into the asynchronous model of execution. The result of this approach is that sending
```

### Comparing `ansar_connect-0.1.243/README.md` & `ansar_connect-0.1.244/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/pyproject.toml` & `ansar_connect-0.1.244/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries"
 ]
 dynamic = ["description", "version", "scripts"]
 dependencies = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.85"
+    "ansar-create>=0.1.86"
 ]
 
 [project.urls]
 Documentation = "https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html"
```

### Comparing `ansar_connect-0.1.243/setup.py` & `ansar_connect-0.1.244/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
     d = f.read()
 DOC_LINK = d[:-1]
 
 REQUIRES = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.85",
+    "ansar-create>=0.1.86",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
     author_email="scott.18.ansar@gmail.com.com",
```

### Comparing `ansar_connect-0.1.243/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.244/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.244/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.244/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.244/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/__init__.py` & `ansar_connect-0.1.244/src/ansar/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 62daa74c7823b81b3ac94ca4d570ba2ba9a56f9a
-Version: 0.1.242 (2024-05-15@04:40:51+NZST)
+Commit: 0d97f44f9329b251c11b15e313704619d5f067de
+Version: 0.1.243 (2024-05-15@04:45:26+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.243/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.244/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/directory.py` & `ansar_connect-0.1.244/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.244/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.244/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/group_if.py` & `ansar_connect-0.1.244/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/grouping.py` & `ansar_connect-0.1.244/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/moving.py` & `ansar_connect-0.1.244/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/networking.py` & `ansar_connect-0.1.244/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.244/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/node.py` & `ansar_connect-0.1.244/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.244/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/procedure.py` & `ansar_connect-0.1.244/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/product.py` & `ansar_connect-0.1.244/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/socketry.py` & `ansar_connect-0.1.244/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/standard.py` & `ansar_connect-0.1.244/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/transporting.py` & `ansar_connect-0.1.244/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.244/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar/connect/wan.py` & `ansar_connect-0.1.244/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.243/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.244/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.243
+Version: 0.1.244
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.85
+Requires-Dist: ansar-create>=0.1.86
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
 messaging into the asynchronous model of execution. The result of this approach is that sending
```

### Comparing `ansar_connect-0.1.243/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.244/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

