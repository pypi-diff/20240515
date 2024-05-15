# Comparing `tmp/py4hw-2024.1.tar.gz` & `tmp/py4hw-2024.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4hw-2024.1.tar", last modified: Wed Apr  3 10:54:59 2024, max compression
+gzip compressed data, was "py4hw-2024.2.tar", last modified: Wed May 15 16:33:35 2024, max compression
```

## Comparing `py4hw-2024.1.tar` & `py4hw-2024.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.331527 py4hw-2024.1/
--rw-rw-rw-   0        0        0    35149 2021-06-17 16:52:58.000000 py4hw-2024.1/LICENSE
--rw-rw-rw-   0        0        0       21 2023-10-05 15:22:53.000000 py4hw-2024.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1226 2024-04-03 10:54:59.329526 py4hw-2024.1/PKG-INFO
--rw-rw-rw-   0        0        0      573 2022-01-30 16:19:40.000000 py4hw-2024.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.007711 py4hw-2024.1/py4hw/
--rw-rw-rw-   0        0        0      534 2023-05-10 09:47:00.000000 py4hw-2024.1/py4hw/__init__.py
--rw-rw-rw-   0        0        0    22222 2023-12-04 22:30:16.000000 py4hw-2024.1/py4hw/base.py
--rw-rw-rw-   0        0        0    27343 2023-04-07 08:22:39.000000 py4hw-2024.1/py4hw/code_generation.py
--rw-rw-rw-   0        0        0     5381 2022-11-20 10:25:09.000000 py4hw-2024.1/py4hw/debug.py
--rw-rw-rw-   0        0        0    11151 2024-02-16 15:11:29.000000 py4hw-2024.1/py4hw/gui.py
--rw-rw-rw-   0        0        0    25105 2023-12-04 22:30:16.000000 py4hw-2024.1/py4hw/helper.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.148632 py4hw-2024.1/py4hw/logic/
--rw-rw-rw-   0        0        0      294 2023-03-19 09:35:30.000000 py4hw-2024.1/py4hw/logic/__init__.py
--rw-rw-rw-   0        0        0    17588 2024-03-23 08:42:37.000000 py4hw-2024.1/py4hw/logic/arithmetic.py
--rw-rw-rw-   0        0        0    13229 2023-03-19 08:52:48.000000 py4hw-2024.1/py4hw/logic/arithmetic_fp.py
--rw-rw-rw-   0        0        0     2535 2023-03-19 19:29:08.000000 py4hw-2024.1/py4hw/logic/arithmetic_fxp.py
--rw-rw-rw-   0        0        0    25059 2024-03-24 11:59:06.000000 py4hw-2024.1/py4hw/logic/bitwise.py
--rw-rw-rw-   0        0        0     1616 2023-04-28 09:24:58.000000 py4hw-2024.1/py4hw/logic/clock.py
--rw-rw-rw-   0        0        0    12701 2023-04-28 08:59:53.000000 py4hw-2024.1/py4hw/logic/relational.py
--rw-rw-rw-   0        0        0    17573 2024-03-25 11:05:26.000000 py4hw-2024.1/py4hw/logic/simulation.py
--rw-rw-rw-   0        0        0     5188 2024-03-26 06:13:28.000000 py4hw-2024.1/py4hw/logic/storage.py
--rw-rw-rw-   0        0        0    29389 2024-03-25 16:08:37.000000 py4hw-2024.1/py4hw/rtl_generation.py
--rw-rw-rw-   0        0        0    63168 2024-02-12 17:48:36.000000 py4hw-2024.1/py4hw/schematic.py
--rw-rw-rw-   0        0        0    28055 2024-02-06 16:04:55.000000 py4hw-2024.1/py4hw/schematic_symbols.py
--rw-rw-rw-   0        0        0     6237 2023-05-25 08:24:27.000000 py4hw-2024.1/py4hw/simulation.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.316533 py4hw-2024.1/py4hw/transpilation/
--rw-rw-rw-   0        0        0      106 2023-04-02 13:11:02.000000 py4hw-2024.1/py4hw/transpilation/__init__.py
--rw-rw-rw-   0        0        0     2564 2023-04-03 11:16:36.000000 py4hw-2024.1/py4hw/transpilation/ast2xml.py
--rw-rw-rw-   0        0        0      402 2023-04-05 11:03:14.000000 py4hw-2024.1/py4hw/transpilation/astutils.py
--rw-rw-rw-   0        0        0    17990 2023-04-07 08:22:39.000000 py4hw-2024.1/py4hw/transpilation/python2cflexhdl_transpilation.py
--rw-rw-rw-   0        0        0     5474 2023-04-05 11:03:14.000000 py4hw-2024.1/py4hw/transpilation/python2structural.py
--rw-rw-rw-   0        0        0    28050 2024-03-19 17:05:40.000000 py4hw-2024.1/py4hw/transpilation/python2verilog_transpilation.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.320535 py4hw-2024.1/py4hw.egg-info/
--rw-rw-rw-   0        0        0     1226 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      880 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-06-10 10:55:08.000000 py4hw-2024.1/pyproject.toml
--rw-rw-rw-   0        0        0       83 2023-12-04 22:30:16.000000 py4hw-2024.1/requires.txt
--rw-rw-rw-   0        0        0      490 2024-04-03 10:54:59.342525 py4hw-2024.1/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-02-12 15:40:49.000000 py4hw-2024.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:33:35.857473 py4hw-2024.2/
+-rw-rw-rw-   0        0        0    35149 2021-06-17 16:52:58.000000 py4hw-2024.2/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-10-05 15:22:53.000000 py4hw-2024.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1237 2024-05-15 16:33:35.856748 py4hw-2024.2/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2022-01-30 16:19:40.000000 py4hw-2024.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 16:33:35.649753 py4hw-2024.2/py4hw/
+-rw-rw-rw-   0        0        0      534 2023-05-10 09:47:00.000000 py4hw-2024.2/py4hw/__init__.py
+-rw-rw-rw-   0        0        0    22222 2023-12-04 22:30:16.000000 py4hw-2024.2/py4hw/base.py
+-rw-rw-rw-   0        0        0    27343 2023-04-07 08:22:39.000000 py4hw-2024.2/py4hw/code_generation.py
+-rw-rw-rw-   0        0        0     5381 2022-11-20 10:25:09.000000 py4hw-2024.2/py4hw/debug.py
+-rw-rw-rw-   0        0        0    11398 2024-05-15 15:48:16.000000 py4hw-2024.2/py4hw/gui.py
+-rw-rw-rw-   0        0        0    25105 2023-12-04 22:30:16.000000 py4hw-2024.2/py4hw/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:33:35.794559 py4hw-2024.2/py4hw/logic/
+-rw-rw-rw-   0        0        0      294 2023-03-19 09:35:30.000000 py4hw-2024.2/py4hw/logic/__init__.py
+-rw-rw-rw-   0        0        0    17588 2024-03-23 08:42:37.000000 py4hw-2024.2/py4hw/logic/arithmetic.py
+-rw-rw-rw-   0        0        0    13229 2023-03-19 08:52:48.000000 py4hw-2024.2/py4hw/logic/arithmetic_fp.py
+-rw-rw-rw-   0        0        0     2535 2023-03-19 19:29:08.000000 py4hw-2024.2/py4hw/logic/arithmetic_fxp.py
+-rw-rw-rw-   0        0        0    25059 2024-03-24 11:59:06.000000 py4hw-2024.2/py4hw/logic/bitwise.py
+-rw-rw-rw-   0        0        0     1616 2023-04-28 09:24:58.000000 py4hw-2024.2/py4hw/logic/clock.py
+-rw-rw-rw-   0        0        0    12701 2023-04-28 08:59:53.000000 py4hw-2024.2/py4hw/logic/relational.py
+-rw-rw-rw-   0        0        0    17573 2024-03-25 11:05:26.000000 py4hw-2024.2/py4hw/logic/simulation.py
+-rw-rw-rw-   0        0        0     5188 2024-03-26 06:13:28.000000 py4hw-2024.2/py4hw/logic/storage.py
+-rw-rw-rw-   0        0        0    29389 2024-03-25 16:08:37.000000 py4hw-2024.2/py4hw/rtl_generation.py
+-rw-rw-rw-   0        0        0    63168 2024-02-12 17:48:36.000000 py4hw-2024.2/py4hw/schematic.py
+-rw-rw-rw-   0        0        0    28055 2024-02-06 16:04:55.000000 py4hw-2024.2/py4hw/schematic_symbols.py
+-rw-rw-rw-   0        0        0     6237 2023-05-25 08:24:27.000000 py4hw-2024.2/py4hw/simulation.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:33:35.853364 py4hw-2024.2/py4hw/transpilation/
+-rw-rw-rw-   0        0        0      106 2023-04-02 13:11:02.000000 py4hw-2024.2/py4hw/transpilation/__init__.py
+-rw-rw-rw-   0        0        0     2564 2023-04-03 11:16:36.000000 py4hw-2024.2/py4hw/transpilation/ast2xml.py
+-rw-rw-rw-   0        0        0      402 2023-04-05 11:03:14.000000 py4hw-2024.2/py4hw/transpilation/astutils.py
+-rw-rw-rw-   0        0        0    17990 2023-04-07 08:22:39.000000 py4hw-2024.2/py4hw/transpilation/python2cflexhdl_transpilation.py
+-rw-rw-rw-   0        0        0     5474 2023-04-05 11:03:14.000000 py4hw-2024.2/py4hw/transpilation/python2structural.py
+-rw-rw-rw-   0        0        0    28050 2024-03-19 17:05:40.000000 py4hw-2024.2/py4hw/transpilation/python2verilog_transpilation.py
+drwxrwxrwx   0        0        0        0 2024-05-15 16:33:35.853364 py4hw-2024.2/py4hw.egg-info/
+-rw-rw-rw-   0        0        0     1237 2024-05-15 16:33:35.000000 py4hw-2024.2/py4hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2024-05-15 16:33:35.000000 py4hw-2024.2/py4hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 16:33:35.000000 py4hw-2024.2/py4hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-15 16:33:35.000000 py4hw-2024.2/py4hw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 16:33:35.000000 py4hw-2024.2/py4hw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-06-10 10:55:08.000000 py4hw-2024.2/pyproject.toml
+-rw-rw-rw-   0        0        0       83 2023-12-04 22:30:16.000000 py4hw-2024.2/requires.txt
+-rw-rw-rw-   0        0        0      481 2024-05-15 16:33:35.868573 py4hw-2024.2/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-05-15 16:29:50.000000 py4hw-2024.2/setup.py
```

### Comparing `py4hw-2024.1/LICENSE` & `py4hw-2024.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/PKG-INFO` & `py4hw-2024.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py4hw
-Version: 2024.1
-Summary: py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural design style to build hardware and it is highly influenced by the ideas behind JHDL.
+Version: 2024.2
+Summary: py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural and behavioural design styles to build hardware and it is influenced by some ideas behind JHDL.
 Home-page: https://github.com/davidcastells/py4hw
 Author: David Castells-Rufas
 Author-email: david.castells@uab.cat
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nbwavedrom==0.2.0
 Requires-Dist: ipywidgets
```

### Comparing `py4hw-2024.1/README.md` & `py4hw-2024.2/README.md`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/__init__.py` & `py4hw-2024.2/py4hw/__init__.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/base.py` & `py4hw-2024.2/py4hw/base.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/code_generation.py` & `py4hw-2024.2/py4hw/code_generation.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/debug.py` & `py4hw-2024.2/py4hw/debug.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/gui.py` & `py4hw-2024.2/py4hw/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import os
 from .base import Logic
 from .schematic import Schematic
     
 class Workbench():
     
     def getIcon(self, path):
-        script_directory = os.path.dirname(os.path.abspath(__file__))
-        icon_path = os.path.join(script_directory, path)
+        #script_directory = os.path.dirname(os.path.abspath(__file__))
+        #icon_path = os.path.join(script_directory, path)
         
-        icon = Image.open(icon_path)
+        icon = Image.open(path)
         icon = ImageTk.PhotoImage(icon)
         return icon
         
     def __init__(self, sys:Logic):
     
         self.sys = sys
         self.detailObj = None
@@ -62,16 +62,22 @@
         self.schematicAreaPane = PanedWindow(self.rightPane,  orient=VERTICAL, relief = SUNKEN, width=100, heigh=20)
         self.schematicToolbarPane = Frame(self.schematicAreaPane) #,  orient=HORIZONTAL, relief = SUNKEN, width=100, heigh=20)
                 
         self.rightPane.add(self.interfacePane)
         self.rightPane.add(self.schematicAreaPane)
         self.schematicAreaPane.add(self.schematicToolbarPane) 
         
-        icon_zo = self.getIcon('zoomout24.png')
-        icon_zi = self.getIcon('zoomin24.png')
+        import importlib
+        package_path = importlib.resources.files('py4hw')
+        # Construct the full path to the image file
+        zoomout_path = package_path / 'zoomout24.png'
+        zoomin_path = package_path / 'zoomin24.png'
+        
+        icon_zo = self.getIcon(zoomout_path)
+        icon_zi = self.getIcon(zoomin_path)
         
         btnZoomIn = ttk.Button(self.schematicToolbarPane,  image=icon_zi, text="Zoom in", command=self.guiZoomIn)
         btnZoomOut = ttk.Button(self.schematicToolbarPane, image=icon_zo, text="Zoom out", command=self.guiZoomOut)
         
         btnZoomIn.pack(side=tkinter.LEFT)
         btnZoomOut.pack(side=tkinter.LEFT)
```

### Comparing `py4hw-2024.1/py4hw/helper.py` & `py4hw-2024.2/py4hw/helper.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/logic/arithmetic.py` & `py4hw-2024.2/py4hw/logic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/logic/arithmetic_fp.py` & `py4hw-2024.2/py4hw/logic/arithmetic_fp.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/logic/arithmetic_fxp.py` & `py4hw-2024.2/py4hw/logic/arithmetic_fxp.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/logic/bitwise.py` & `py4hw-2024.2/py4hw/logic/bitwise.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/logic/clock.py` & `py4hw-2024.2/py4hw/logic/clock.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/logic/relational.py` & `py4hw-2024.2/py4hw/logic/relational.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/logic/simulation.py` & `py4hw-2024.2/py4hw/logic/simulation.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/logic/storage.py` & `py4hw-2024.2/py4hw/logic/storage.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/rtl_generation.py` & `py4hw-2024.2/py4hw/rtl_generation.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/schematic.py` & `py4hw-2024.2/py4hw/schematic.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/schematic_symbols.py` & `py4hw-2024.2/py4hw/schematic_symbols.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/simulation.py` & `py4hw-2024.2/py4hw/simulation.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/transpilation/ast2xml.py` & `py4hw-2024.2/py4hw/transpilation/ast2xml.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/transpilation/python2cflexhdl_transpilation.py` & `py4hw-2024.2/py4hw/transpilation/python2cflexhdl_transpilation.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/transpilation/python2structural.py` & `py4hw-2024.2/py4hw/transpilation/python2structural.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw/transpilation/python2verilog_transpilation.py` & `py4hw-2024.2/py4hw/transpilation/python2verilog_transpilation.py`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/py4hw.egg-info/PKG-INFO` & `py4hw-2024.2/py4hw.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py4hw
-Version: 2024.1
-Summary: py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural design style to build hardware and it is highly influenced by the ideas behind JHDL.
+Version: 2024.2
+Summary: py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural and behavioural design styles to build hardware and it is influenced by some ideas behind JHDL.
 Home-page: https://github.com/davidcastells/py4hw
 Author: David Castells-Rufas
 Author-email: david.castells@uab.cat
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nbwavedrom==0.2.0
 Requires-Dist: ipywidgets
```

### Comparing `py4hw-2024.1/py4hw.egg-info/SOURCES.txt` & `py4hw-2024.2/py4hw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4hw-2024.1/setup.py` & `py4hw-2024.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
                          
 setup(
     name='py4hw',
-    version='2024.1',
+    version='2024.2',
     author='David Castells-Rufas',
     author_email='david.castells@uab.cat',
-    description='py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural design style to build hardware and it is highly influenced by the ideas behind JHDL.',
+    description='py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural and behavioural design styles to build hardware and it is influenced by some ideas behind JHDL.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/davidcastells/py4hw',
     install_requires=open('requires.txt').readlines(),
     tests_require=open('requires.txt').readlines(),
-    packages=find_packages(exclude=['riscv'])
+    packages=find_packages() 
 )
```

