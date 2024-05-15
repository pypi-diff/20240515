# Comparing `tmp/lap_data-4.0.46.tar.gz` & `tmp/lap_data-4.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lap_data-4.0.46.tar", last modified: Wed Feb 28 13:58:54 2024, max compression
+gzip compressed data, was "lap_data-4.0.47.tar", last modified: Wed May 15 12:19:14 2024, max compression
```

## Comparing `lap_data-4.0.46.tar` & `lap_data-4.0.47.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 13:58:54.018073 lap_data-4.0.46/
--rw-rw-rw-   0        0        0    35821 2022-10-20 13:06:49.000000 lap_data-4.0.46/LICENSE
--rw-rw-rw-   0        0        0      709 2024-02-28 13:58:54.018073 lap_data-4.0.46/PKG-INFO
--rw-rw-rw-   0        0        0      329 2022-10-20 13:06:49.000000 lap_data-4.0.46/README.md
--rw-rw-rw-   0        0        0       97 2022-10-20 13:06:49.000000 lap_data-4.0.46/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-02-28 13:58:54.018073 lap_data-4.0.46/setup.cfg
--rw-rw-rw-   0        0        0     1172 2024-02-28 13:22:32.000000 lap_data-4.0.46/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:58:53.949065 lap_data-4.0.46/src/
-drwxrwxrwx   0        0        0        0 2024-02-28 13:58:53.986795 lap_data-4.0.46/src/lap_data/
--rw-rw-rw-   0        0        0      197 2024-02-28 13:22:49.000000 lap_data-4.0.46/src/lap_data/__init__.py
--rw-rw-rw-   0        0        0    19286 2022-10-20 13:06:49.000000 lap_data-4.0.46/src/lap_data/lcmodel.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:58:54.018073 lap_data-4.0.46/src/lap_data.egg-info/
--rw-rw-rw-   0        0        0      709 2024-02-28 13:58:53.000000 lap_data-4.0.46/src/lap_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-02-28 13:58:53.000000 lap_data-4.0.46/src/lap_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 13:58:53.000000 lap_data-4.0.46/src/lap_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-02-28 13:58:53.000000 lap_data-4.0.46/src/lap_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-28 13:58:53.000000 lap_data-4.0.46/src/lap_data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 12:19:14.856734 lap_data-4.0.47/
+-rw-rw-rw-   0        0        0    35821 2022-10-20 13:06:49.000000 lap_data-4.0.47/LICENSE
+-rw-rw-rw-   0        0        0      709 2024-05-15 12:19:14.856734 lap_data-4.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2022-10-20 13:06:49.000000 lap_data-4.0.47/README.md
+-rw-rw-rw-   0        0        0       97 2022-10-20 13:06:49.000000 lap_data-4.0.47/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-15 12:19:14.860151 lap_data-4.0.47/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2024-05-04 22:11:23.000000 lap_data-4.0.47/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:19:14.794184 lap_data-4.0.47/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 12:19:14.828795 lap_data-4.0.47/src/lap_data/
+-rw-rw-rw-   0        0        0      197 2024-04-16 08:00:23.000000 lap_data-4.0.47/src/lap_data/__init__.py
+-rw-rw-rw-   0        0        0    19940 2024-04-16 08:00:15.000000 lap_data-4.0.47/src/lap_data/lcmodel.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:19:14.855754 lap_data-4.0.47/src/lap_data.egg-info/
+-rw-rw-rw-   0        0        0      709 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/top_level.txt
```

### Comparing `lap_data-4.0.46/LICENSE` & `lap_data-4.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `lap_data-4.0.46/PKG-INFO` & `lap_data-4.0.47/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lap_data
-Version: 4.0.46
+Version: 4.0.47
 Summary: Laser Aided Profiler Data Access Library
 Author: Peter Demján
 Author-email: peter.demjan@gmail.com
 Keywords: database,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Database
```

### Comparing `lap_data-4.0.46/setup.py` & `lap_data-4.0.47/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python
 #
 
 from setuptools import setup, find_packages
 
+import ast
+import os
+
+def get_version():
+	with open(os.path.join(os.path.dirname(__file__), 'src', 'lap_data', '__init__.py')) as f:
+		tree = ast.parse(f.read())
+		for node in tree.body:
+			if isinstance(node, ast.Assign):
+				if node.targets[0].id == 'version_info':
+					return '.'.join(map(str, ast.literal_eval(node.value)))
+
 try:
 	from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
 	class bdist_wheel(_bdist_wheel):
 		def finalize_options(self):
 			_bdist_wheel.finalize_options(self)
 			self.root_is_pure = False
 except ImportError:
 	bdist_wheel = None
 
 description="Laser Aided Profiler Data Access Library"
 
 setup(
 	name="lap_data",
-	version="4.0.46",
+	version=get_version(),
 	description=description,
 	long_description=description,
 	long_description_content_type="text/markdown",
 	author="Peter Demján",
 	author_email="peter.demjan@gmail.com",
 	classifiers=[
 		"Development Status :: 5 - Production/Stable",
```

### Comparing `lap_data-4.0.46/src/lap_data/lcmodel.py` & `lap_data-4.0.47/src/lap_data/lcmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 				["Settings",				"Sample.Settings"],
 				["Date_Created",			"Sample.Date_Created"],
 				["Date_Modified",			"Sample.Date_Modified"],
 				["SW_Version",				"Sample.SW_Version"],
 				["Settings",				"Sample.Settings"],
 				["Detail_Geometry",			"Sample.Drawn.Detail.Geometry"],
 				["Detail_Filled",			"Sample.Drawn.Detail.Filled"],
+				["Detail_Dashed",			"Sample.Drawn.Detail.Dashed"],
+				["Detail_Fill_Color",		"Sample.Drawn.Detail.Fill_Color"],
+				["Detail_Line_Color",		"Sample.Drawn.Detail.Line_Color"],
 				["Break_Geometry",			"Sample.Drawn.Break.Geometry"],
 				["Inflection_Geometry",		"Sample.Drawn.Inflection.Geometry"],
 				["Inflection_Dashed",		"Sample.Drawn.Inflection.Dashed"],
 				["Arc_Geometry",			"Sample.Drawn.Arc.Geometry"],
 				["Photo_Image",				"Sample.Drawn.Photo.Image"],
 				["Photo_Mask",				"Sample.Drawn.Photo.Mask"],
 				["Photo_Position",			"Sample.Drawn.Photo.Position"],
@@ -200,14 +203,31 @@
 					classes.append(class2)
 				if (name, class2, descr) not in descriptors:
 					descriptors.append((name, class2, descr))
 				relations.add((class1, rel, class2))
 		
 		return classes, descriptors, relations
 	
+	def get_arc_structure(self):
+		
+		arc_cls, arc_descr, arc_rel = None, None, None
+		_, descriptors, relations = self.get_data_structure()
+		for name, cls, descr in descriptors:
+			if name == "Arc_Geometry":
+				arc_cls, arc_descr = cls, descr
+				break
+		for cls1, rel, cls2 in relations:
+			if cls1 == arc_cls:
+				arc_rel = self.reverse_relation(rel)
+				break
+			elif cls2 == arc_cls:
+				arc_rel = rel
+				break
+		return arc_cls, arc_descr, arc_rel
+	
 	def create_data_structure(self):
 		# returns descr_lookup, relations
 		#	descr_lookup = {name: (Class, Descriptor), ...}
 		#	relations = set((Class1, Relation, Class2), ...)
 		
 		classes, descriptors, relations = self.get_data_structure()
```

### Comparing `lap_data-4.0.46/src/lap_data.egg-info/PKG-INFO` & `lap_data-4.0.47/src/lap_data.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lap_data
-Version: 4.0.46
+Version: 4.0.47
 Summary: Laser Aided Profiler Data Access Library
 Author: Peter Demján
 Author-email: peter.demjan@gmail.com
 Keywords: database,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Database
```

