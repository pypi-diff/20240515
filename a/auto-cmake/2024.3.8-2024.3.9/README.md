# Comparing `tmp/auto_cmake-2024.3.8.tar.gz` & `tmp/auto_cmake-2024.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_cmake-2024.3.8.tar", last modified: Mon Mar  4 08:39:39 2024, max compression
+gzip compressed data, was "auto_cmake-2024.3.9.tar", last modified: Mon Mar  4 09:53:19 2024, max compression
```

## Comparing `auto_cmake-2024.3.8.tar` & `auto_cmake-2024.3.9.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-04 08:39:39.381994 auto_cmake-2024.3.8/
--rw-r--r--   0 sentinel   (501) admin       (80)       17 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/MANIFEST.in
--rw-r--r--   0 sentinel   (501) admin       (80)     1798 2024-03-04 08:39:39.381899 auto_cmake-2024.3.8/PKG-INFO
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-04 08:39:39.381055 auto_cmake-2024.3.8/auto_cmake/
--rw-r--r--   0 sentinel   (501) admin       (80)      420 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/__init__.py
--rw-r--r--   0 sentinel   (501) admin       (80)     6292 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake.py
--rw-r--r--   0 sentinel   (501) admin       (80)     2994 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_android.py
--rw-r--r--   0 sentinel   (501) admin       (80)     2622 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_exe.py
--rw-r--r--   0 sentinel   (501) admin       (80)      865 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_indexer.py
--rw-r--r--   0 sentinel   (501) admin       (80)     6187 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_ios.py
--rw-r--r--   0 sentinel   (501) admin       (80)     3459 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_lib_shared_mac_intel.py
--rw-r--r--   0 sentinel   (501) admin       (80)     3455 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_lib_shared_mac_m1.py
--rw-r--r--   0 sentinel   (501) admin       (80)     3386 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_lib_shared_nux.py
--rw-r--r--   0 sentinel   (501) admin       (80)     3439 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_lib_shared_win.py
--rw-r--r--   0 sentinel   (501) admin       (80)     5459 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/auto_cmake/auto_cmake_stm32.py
-drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-04 08:39:39.381595 auto_cmake-2024.3.8/auto_cmake.egg-info/
--rw-r--r--   0 sentinel   (501) admin       (80)     1798 2024-03-04 08:39:39.000000 auto_cmake-2024.3.8/auto_cmake.egg-info/PKG-INFO
--rw-r--r--   0 sentinel   (501) admin       (80)      538 2024-03-04 08:39:39.000000 auto_cmake-2024.3.8/auto_cmake.egg-info/SOURCES.txt
--rw-r--r--   0 sentinel   (501) admin       (80)        1 2024-03-04 08:39:39.000000 auto_cmake-2024.3.8/auto_cmake.egg-info/dependency_links.txt
--rw-r--r--   0 sentinel   (501) admin       (80)       11 2024-03-04 08:39:39.000000 auto_cmake-2024.3.8/auto_cmake.egg-info/top_level.txt
--rw-r--r--   0 sentinel   (501) admin       (80)     1011 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/readme.md
--rw-r--r--   0 sentinel   (501) admin       (80)       38 2024-03-04 08:39:39.382135 auto_cmake-2024.3.8/setup.cfg
--rw-r--r--   0 sentinel   (501) admin       (80)      982 2024-03-04 08:38:01.000000 auto_cmake-2024.3.8/setup.py
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-04 09:53:19.314038 auto_cmake-2024.3.9/
+-rw-r--r--   0 sentinel   (501) admin       (80)       17 2024-03-04 08:38:01.000000 auto_cmake-2024.3.9/MANIFEST.in
+-rw-r--r--   0 sentinel   (501) admin       (80)     1799 2024-03-04 09:53:19.313862 auto_cmake-2024.3.9/PKG-INFO
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-04 09:53:19.311033 auto_cmake-2024.3.9/auto_cmake/
+-rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-04 09:08:04.000000 auto_cmake-2024.3.9/auto_cmake/__init__.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     7626 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     2969 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake_android.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     2438 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake_exe.py
+-rw-r--r--   0 sentinel   (501) admin       (80)      838 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake_indexer.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     6162 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake_ios.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     3606 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake_lib_shared_mac.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     3202 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake_lib_shared_nux.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     3255 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake_lib_shared_win.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     5275 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/auto_cmake/auto_cmake_stm32.py
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-04 09:53:19.312242 auto_cmake-2024.3.9/auto_cmake.egg-info/
+-rw-r--r--   0 sentinel   (501) admin       (80)     1799 2024-03-04 09:53:19.000000 auto_cmake-2024.3.9/auto_cmake.egg-info/PKG-INFO
+-rw-r--r--   0 sentinel   (501) admin       (80)      641 2024-03-04 09:53:19.000000 auto_cmake-2024.3.9/auto_cmake.egg-info/SOURCES.txt
+-rw-r--r--   0 sentinel   (501) admin       (80)        1 2024-03-04 09:53:19.000000 auto_cmake-2024.3.9/auto_cmake.egg-info/dependency_links.txt
+-rw-r--r--   0 sentinel   (501) admin       (80)       17 2024-03-04 09:53:19.000000 auto_cmake-2024.3.9/auto_cmake.egg-info/top_level.txt
+-rw-r--r--   0 sentinel   (501) admin       (80)     1012 2024-03-04 09:08:38.000000 auto_cmake-2024.3.9/readme.md
+-rw-r--r--   0 sentinel   (501) admin       (80)       38 2024-03-04 09:53:19.314074 auto_cmake-2024.3.9/setup.cfg
+-rw-r--r--   0 sentinel   (501) admin       (80)      982 2024-03-04 09:51:21.000000 auto_cmake-2024.3.9/setup.py
+drwxr-xr-x   0 sentinel   (501) admin       (80)        0 2024-03-04 09:53:19.313218 auto_cmake-2024.3.9/tests/
+-rw-r--r--   0 sentinel   (501) admin       (80)        0 2024-03-04 08:48:51.000000 auto_cmake-2024.3.9/tests/__init__.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1401 2024-03-04 09:42:54.000000 auto_cmake-2024.3.9/tests/test_auto_cmake.py
+-rw-r--r--   0 sentinel   (501) admin       (80)      882 2024-03-04 09:42:54.000000 auto_cmake-2024.3.9/tests/test_auto_cmake_exe.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1244 2024-03-04 09:48:56.000000 auto_cmake-2024.3.9/tests/test_auto_cmake_lib_shared_mac.py
+-rw-r--r--   0 sentinel   (501) admin       (80)     1015 2024-03-04 09:44:22.000000 auto_cmake-2024.3.9/tests/test_auto_cmake_lib_shared_win.py
```

### Comparing `auto_cmake-2024.3.8/PKG-INFO` & `auto_cmake-2024.3.9/auto_cmake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto_cmake
-Version: 2024.3.8
+Name: auto-cmake
+Version: 2024.3.9
 Summary: Automate setup of CMake projects
 Home-page: https://github.com/veda-s4dhak/auto-cmake.git
 Author: Veda Sadhak
 Author-email: vedasadhak@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -36,15 +36,15 @@
    2) Directories and paths to include and exclude
    3) Compiler flags
    4) Build directory
    
 ```
 import os
 
-from auto_cmake_exe import AutoCMakeExe
+from .auto_cmake_exe import AutoCMakeExe
 
 # Configuration
 cmake_config = dict()
 cmake_config['proj_name'] = 'proj_name'
 cmake_config['proj_dir'] = os.path.abspath(os.path.join(os.getcwd(), os.pardir))
 cmake_config['version'] = '0.01'
 cmake_config['cmake_version'] = '3.15'
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,36 +2,49 @@
 
 """
 Description: Core module.
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
 import pathlib
-from auto_cmake_indexer import AutoCMakeIndexer
+import shutil
+from .auto_cmake_indexer import AutoCMakeIndexer
 
 class AutoCMake(AutoCMakeIndexer):
 
     def __init__(self, **kwargs):
 
         AutoCMakeIndexer.__init__(self, kwargs['proj_dir'])
 
+        # Project Definition
         self.proj_name = kwargs['proj_name']
         self.version = kwargs['version']
-        self.acake_version = kwargs['cmake_version']
+
+        # CMake Definition
+        self.cmake_version = kwargs['cmake_version']
+
+        # Build & Export
+        self.build_dir = self.get_posix_path(kwargs['build_dir'])
+
+        # Include & Excludes
         self.include_dirs = kwargs['include_dirs']
         self.exclude_dirs = kwargs['exclude_dirs']
         self.exclude_paths = kwargs['exclude_paths']
 
+        # Internal excludes
+        self.exclude_paths.append(self.build_dir)
+
+        # Library cache
         self.library_paths = []
         self.library_names = []
 
+        # File cache
         self.sources = []
         self.headers = []
         self.includes = []
         self.startup = []
         self.linkers = []
 
     def clear(self):
@@ -185,8 +198,42 @@
                     for exclude_path in self.exclude_paths:
                         if self.get_posix_path(exclude_path) in self.get_posix_path(lib_path):
                             excluded = True
 
                 if not excluded:
                     self.add_libraries(os.path.join(path,dir))
 
-        self.add_library(path)
+        self.add_library(path)
+
+    def index(self):
+
+        for _dir in self.include_dirs:
+            self.add_libraries(os.path.join(self.proj_dir, _dir))
+            self.clear()
+
+    def create_build_dir(self):
+        if not os.path.exists(self.build_dir):
+            os.makedirs(self.build_dir)
+
+    def export(self):
+
+        # Create directories
+        include_dir = self.get_posix_path(os.path.join(self.build_dir, "include"))
+        src_dir = self.get_posix_path(os.path.join(self.build_dir, "src"))
+        if not os.path.exists(include_dir):
+            os.makedirs(include_dir)
+        if not os.path.exists(src_dir):
+            os.makedirs(src_dir)
+
+        # Copy over headers
+        for header in self.headers:
+            header_path, header_file = os.path.split(header)
+            shutil.copyfile(header, os.path.join(include_dir, header_file))
+
+        # Copy over sources
+        for source in self.sources:
+            source_path, source_file = os.path.split(source)
+            shutil.copyfile(source, os.path.join(src_dir, source_file))
+
+
+
+
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake_android.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake_android.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 """
 Description: Generates an executable target
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
 
-from auto_cmake import AutoCMake
+from .auto_cmake import AutoCMake
 
 class AutoCMakeAndroid():
 
     def __init__(self, **cmake_config):
 
         # Creating instance
         self.ac = AutoCMake(**cmake_config)
@@ -78,8 +77,8 @@
         self.ac.add(r"    ${log-lib}")
         self.ac.add(")\n")
 
         # Writing main CMakeLists.txt
         cmake_build_path = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, os.pardir, os.pardir))
         if not os.path.exists(cmake_build_path):
             os.makedirs(cmake_build_path)
-        self.ac.write(cmake_build_path)
+        self.ac.write(self.ac.build_dir)
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake_exe.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake_exe.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 """
 Description: Generates an executable target
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
 
-from auto_cmake import AutoCMake
+from .auto_cmake import AutoCMake
 
 class AutoCMakeExe():
 
     def __init__(self, **cmake_config):
 
         # Creating instance
         self.ac = AutoCMake(**cmake_config)
@@ -64,11 +63,9 @@
 
         # Adding include directories
         for path in self.ac.library_paths:
             self.ac.add('target_include_directories({} PUBLIC "{}")'.format(self.ac.proj_name, path))
         self.ac.add("")
 
         # Writing main CMakeLists.txt
-        cmake_build_path = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, "cmake-build-debug"))
-        if not os.path.exists(cmake_build_path):
-            os.makedirs(cmake_build_path)
-        self.ac.write(cmake_build_path)
+        self.ac.create_build_dir()
+        self.ac.write(self.ac.build_dir)
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake_indexer.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake_indexer.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 """
 Description: Builds a source index.
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
 
 class AutoCMakeIndexer():
 
     def __init__(self, proj_dir):
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake_ios.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake_ios.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 """
 Description: Generates a macosx shared library
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
 import shutil
 
-from auto_cmake import AutoCMake
+from .auto_cmake import AutoCMake
 
 class AutoCMakeIos():
 
     def __init__(self, **cmake_config):
 
         # Creating instance
         self.ac = AutoCMake(**cmake_config)
@@ -126,15 +125,15 @@
             self.ac.add('target_include_directories({} PUBLIC "{}")'.format(self.ac.proj_name, path))
         self.ac.add("")
 
         # Writing main CMakeLists.txt
         cmake_build_path = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, "build"))
         if not os.path.exists(cmake_build_path):
             os.makedirs(cmake_build_path)
-        self.ac.write(cmake_build_path)
+        self.ac.write(self.ac.build_dir)
 
         # Copy over headers
         xcode_file = f"{self.ac.proj_name}.framework"
         dst = os.path.join(cmake_build_path, "Debug", xcode_file, "Headers")
         if not os.path.exists(dst):
             os.makedirs(dst)
         for header in self.ac.headers:
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake_lib_shared_mac_intel.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake_lib_shared_mac.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 """
 Description: Generates a macosx shared library
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
 import shutil
 
-from auto_cmake import AutoCMake
+from .auto_cmake import AutoCMake
 
-class AutoCMakeLibSharedMacIntel():
+class AutoCMakeLibSharedMac():
 
     def __init__(self, **cmake_config):
 
         # Creating instance
         self.ac = AutoCMake(**cmake_config)
         self.libs = cmake_config["libs"]
 
@@ -25,27 +24,32 @@
         self.flags = cmake_config["flags"]
 
         if "jni_dir" in cmake_config.keys():
             self.jni_dir = cmake_config["jni_dir"]
         else:
             self.jni_dir = None
 
+        if "arch" in cmake_config.keys():
+            self.arch = cmake_config["arch"]
+        else:
+            raise ("cmake_config['arch'] must be specified")
+
     def run(self):
 
         # Recursively adding all source
         for _dir in self.ac.include_dirs:
             self.ac.add_libraries(os.path.join(self.ac.proj_dir, _dir))
             self.ac.clear()
 
         # Adding the compile config
         self.ac.add("cmake_minimum_required(VERSION {})".format(self.ac.cmake_version))
         self.ac.add("project({} VERSION {})".format(self.ac.proj_name, self.ac.version))
         self.ac.add("set(CMAKE_CXX_STANDARD 11)")
         self.ac.add('set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")')
-        self.ac.add('set(CMAKE_OSX_ARCHITECTURES "x86_64")\n')
+        self.ac.add('set(CMAKE_OSX_ARCHITECTURES "{}")\n'.format(self.arch))
 
         # Setting flags
         self.ac.add('SET_PROPERTY(GLOBAL PROPERTY TARGET_SUPPORTS_SHARED_LIBS TRUE)\n')
 
         # Set headers and sources
         self.ac.add("set(SOURCES".format(self.ac.proj_name))
         for source in self.ac.sources:
@@ -88,8 +92,8 @@
             self.ac.add('target_include_directories({} PUBLIC "{}")'.format(self.ac.proj_name, path))
         self.ac.add("")
 
         # Writing main CMakeLists.txt
         cmake_build_path = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, "build"))
         if not os.path.exists(cmake_build_path):
             os.makedirs(cmake_build_path)
-        self.ac.write(cmake_build_path)
+        self.ac.write(self.ac.build_dir)
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake_lib_shared_mac_m1.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake_lib_shared_nux.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python
 
 """
-Description: Generates a macosx shared library
+Description: Generates a nux shared library
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
-import shutil
 
-from auto_cmake import AutoCMake
+from .auto_cmake import AutoCMake
 
-class AutoCMakeLibSharedMacM1():
+class AutoCMakeLibSharedNux():
 
     def __init__(self, **cmake_config):
 
         # Creating instance
         self.ac = AutoCMake(**cmake_config)
         self.libs = cmake_config["libs"]
 
@@ -36,16 +34,15 @@
             self.ac.add_libraries(os.path.join(self.ac.proj_dir, _dir))
             self.ac.clear()
 
         # Adding the compile config
         self.ac.add("cmake_minimum_required(VERSION {})".format(self.ac.cmake_version))
         self.ac.add("project({} VERSION {})".format(self.ac.proj_name, self.ac.version))
         self.ac.add("set(CMAKE_CXX_STANDARD 11)")
-        self.ac.add('set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")')
-        self.ac.add('set(CMAKE_OSX_ARCHITECTURES "arm64")\n')
+        self.ac.add('set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")\n')
 
         # Setting flags
         self.ac.add('SET_PROPERTY(GLOBAL PROPERTY TARGET_SUPPORTS_SHARED_LIBS TRUE)\n')
 
         # Set headers and sources
         self.ac.add("set(SOURCES".format(self.ac.proj_name))
         for source in self.ac.sources:
@@ -63,16 +60,16 @@
             self.ac.add('    "{}"'.format(flag))
         self.ac.add(")\n")
 
         # Add JNI libs
         if self.jni_dir:
             self.ac.add('include_directories("{}/include")'.format(self.jni_dir))
             self.ac.add('link_directories("{}/include")'.format(self.jni_dir))
-            self.ac.add('include_directories("{}/include/darwin")'.format(self.jni_dir))
-            self.ac.add('link_directories("{}/include/darwin")\n'.format(self.jni_dir))
+            self.ac.add('include_directories("{}/include/linux")'.format(self.jni_dir))
+            self.ac.add('link_directories("{}/include/linux")\n'.format(self.jni_dir))
 
         # Setting shared lib properties
         self.ac.add('set_target_properties({} PROPERTIES COMPILE_FLAGS "-fPIC")\n'.format(self.ac.proj_name))
 
         # Link libraries
         for lib in self.libs:
             self.ac.add('target_link_libraries({} {})\n'.format(self.ac.proj_name, self.ac.get_posix_path(lib)))
@@ -85,11 +82,9 @@
 
         # Adding include directories
         for path in self.ac.library_paths:
             self.ac.add('target_include_directories({} PUBLIC "{}")'.format(self.ac.proj_name, path))
         self.ac.add("")
 
         # Writing main CMakeLists.txt
-        cmake_build_path = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, "build"))
-        if not os.path.exists(cmake_build_path):
-            os.makedirs(cmake_build_path)
-        self.ac.write(cmake_build_path)
+        self.ac.create_build_dir()
+        self.ac.write(self.ac.build_dir)
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake_lib_shared_nux.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake_lib_shared_win.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python
 
 """
-Description: Generates a nux shared library
+Description: Generates a windows shared library
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
 
-from auto_cmake import AutoCMake
+from .auto_cmake import AutoCMake
 
-class AutoCMakeLibSharedNux():
+class AutoCMakeLibSharedWin():
 
     def __init__(self, **cmake_config):
 
         # Creating instance
         self.ac = AutoCMake(**cmake_config)
         self.libs = cmake_config["libs"]
 
@@ -61,21 +60,21 @@
             self.ac.add('    "{}"'.format(flag))
         self.ac.add(")\n")
 
         # Add JNI libs
         if self.jni_dir:
             self.ac.add('include_directories("{}/include")'.format(self.jni_dir))
             self.ac.add('link_directories("{}/include")'.format(self.jni_dir))
-            self.ac.add('include_directories("{}/include/linux")'.format(self.jni_dir))
-            self.ac.add('link_directories("{}/include/linux")\n'.format(self.jni_dir))
+            self.ac.add('include_directories("{}/include/win32")'.format(self.jni_dir))
+            self.ac.add('link_directories("{}/include/win32")\n'.format(self.jni_dir))
 
         # Setting shared lib properties
         self.ac.add('set_target_properties({} PROPERTIES COMPILE_FLAGS "-fPIC")\n'.format(self.ac.proj_name))
 
-        # Link libraries
+        # Static linkage is required for successful Windows DLL creation.
         for lib in self.libs:
             self.ac.add('target_link_libraries({} {})\n'.format(self.ac.proj_name, self.ac.get_posix_path(lib)))
 
         # Adding include directories
         for include in self.ac.includes:
             if include not in self.ac.library_paths:
                 self.ac.add('target_include_directories({} PUBLIC "{}")'.format(self.ac.proj_name, include))
@@ -83,11 +82,9 @@
 
         # Adding include directories
         for path in self.ac.library_paths:
             self.ac.add('target_include_directories({} PUBLIC "{}")'.format(self.ac.proj_name, path))
         self.ac.add("")
 
         # Writing main CMakeLists.txt
-        cmake_build_path = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, "cmake-build-debug"))
-        if not os.path.exists(cmake_build_path):
-            os.makedirs(cmake_build_path)
-        self.ac.write(cmake_build_path)
+        self.ac.create_build_dir()
+        self.ac.write(self.ac.build_dir)
```

### Comparing `auto_cmake-2024.3.8/auto_cmake/auto_cmake_stm32.py` & `auto_cmake-2024.3.9/auto_cmake/auto_cmake_stm32.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 """
 Description: Generates an executable target
 """
 
 __author__ = "Veda Sadhak"
 __license__ = "MIT"
-__version__ = "2024.03.08"
 
 import os
 import shutil
 
-from auto_cmake import AutoCMake
+from .auto_cmake import AutoCMake
 
 class AutoCMakeSTM32():
 
     def __init__(self, **cmake_config):
 
         # Creating instance
         self.ac = AutoCMake(**cmake_config)
@@ -116,16 +115,14 @@
         self.ac.add(r'                   COMMAND ${OBJCOPY} -Oihex ${PROJECT_NAME}.elf ${HEX_FILE}')
         self.ac.add(r'                   COMMAND ${OBJCOPY} -Obinary ${PROJECT_NAME}.elf ${BIN_FILE}')
         self.ac.add(r'                   COMMENT "Building ${HEX_FILE} \nBuilding ${BIN_FILE}"')
         self.ac.add(r'                   COMMAND arm-none-eabi-size ${PROJECT_NAME}.elf)')
         self.ac.add("")
 
         # Writing main CMakeLists.txt
-        cmake_build_path = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, "cmake-build-debug"))
-        if not os.path.exists(cmake_build_path):
-            os.makedirs(cmake_build_path)
-        self.ac.write(cmake_build_path)
+        self.ac.create_build_dir()
+        self.ac.write(self.ac.build_dir)
 
         # Copy toolchain file
         src_file = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, "Scripts", "cmake", "auto_cmake", "resources", "arm-none-eabi-gcc.toolchain.cmake"))
         dst_file = self.ac.get_posix_path(os.path.join(self.ac.proj_dir, "cmake-build-debug", "arm-none-eabi-gcc.toolchain.cmake"))
         shutil.copyfile(src_file, dst_file)
```

### Comparing `auto_cmake-2024.3.8/auto_cmake.egg-info/PKG-INFO` & `auto_cmake-2024.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto-cmake
-Version: 2024.3.8
+Name: auto_cmake
+Version: 2024.3.9
 Summary: Automate setup of CMake projects
 Home-page: https://github.com/veda-s4dhak/auto-cmake.git
 Author: Veda Sadhak
 Author-email: vedasadhak@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -36,15 +36,15 @@
    2) Directories and paths to include and exclude
    3) Compiler flags
    4) Build directory
    
 ```
 import os
 
-from auto_cmake_exe import AutoCMakeExe
+from .auto_cmake_exe import AutoCMakeExe
 
 # Configuration
 cmake_config = dict()
 cmake_config['proj_name'] = 'proj_name'
 cmake_config['proj_dir'] = os.path.abspath(os.path.join(os.getcwd(), os.pardir))
 cmake_config['version'] = '0.01'
 cmake_config['cmake_version'] = '3.15'
```

### Comparing `auto_cmake-2024.3.8/auto_cmake.egg-info/SOURCES.txt` & `auto_cmake-2024.3.9/auto_cmake.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 setup.py
 auto_cmake/__init__.py
 auto_cmake/auto_cmake.py
 auto_cmake/auto_cmake_android.py
 auto_cmake/auto_cmake_exe.py
 auto_cmake/auto_cmake_indexer.py
 auto_cmake/auto_cmake_ios.py
-auto_cmake/auto_cmake_lib_shared_mac_intel.py
-auto_cmake/auto_cmake_lib_shared_mac_m1.py
+auto_cmake/auto_cmake_lib_shared_mac.py
 auto_cmake/auto_cmake_lib_shared_nux.py
 auto_cmake/auto_cmake_lib_shared_win.py
 auto_cmake/auto_cmake_stm32.py
 auto_cmake.egg-info/PKG-INFO
 auto_cmake.egg-info/SOURCES.txt
 auto_cmake.egg-info/dependency_links.txt
-auto_cmake.egg-info/top_level.txt
+auto_cmake.egg-info/top_level.txt
+tests/__init__.py
+tests/test_auto_cmake.py
+tests/test_auto_cmake_exe.py
+tests/test_auto_cmake_lib_shared_mac.py
+tests/test_auto_cmake_lib_shared_win.py
```

### Comparing `auto_cmake-2024.3.8/readme.md` & `auto_cmake-2024.3.9/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
    2) Directories and paths to include and exclude
    3) Compiler flags
    4) Build directory
    
 ```
 import os
 
-from auto_cmake_exe import AutoCMakeExe
+from .auto_cmake_exe import AutoCMakeExe
 
 # Configuration
 cmake_config = dict()
 cmake_config['proj_name'] = 'proj_name'
 cmake_config['proj_dir'] = os.path.abspath(os.path.join(os.getcwd(), os.pardir))
 cmake_config['version'] = '0.01'
 cmake_config['cmake_version'] = '3.15'
```

### Comparing `auto_cmake-2024.3.8/setup.py` & `auto_cmake-2024.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto_cmake',
-    version='2024.03.08',
+    version='2024.03.09',
     author='Veda Sadhak',
     author_email='vedasadhak@gmail.com',
     description='Automate setup of CMake projects',
     long_description=open('readme.md').read(),
     include_package_data=True,
     long_description_content_type='text/markdown',
     url='https://github.com/veda-s4dhak/auto-cmake.git',
```

