# Comparing `tmp/pyvisjs-1.0.0a1.tar.gz` & `tmp/pyvisjs-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-1.0.0a1.tar", last modified: Mon May 13 07:04:57 2024, max compression
+gzip compressed data, was "pyvisjs-1.0.0b1.tar", last modified: Wed May 15 12:34:06 2024, max compression
```

## Comparing `pyvisjs-1.0.0a1.tar` & `pyvisjs-1.0.0b1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.204625 pyvisjs-1.0.0a1/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2024-05-13 07:04:57.204625 pyvisjs-1.0.0a1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.198625 pyvisjs-1.0.0a1/examples/
--rw-rw-rw-   0 root         (0) root         (0)     8590 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/examples/bluor.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/examples/readme_usage.py
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.200625 pyvisjs-1.0.0a1/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     8467 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/node.py
--rw-rw-rw-   0 root         (0) root         (0)    13062 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.202625 pyvisjs-1.0.0a1/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/bs-container.html
--rw-rw-rw-   0 root         (0) root         (0)     3812 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/functions.js
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/select-edge-filter.html
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.204625 pyvisjs-1.0.0a1/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      775 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 07:04:57.204625 pyvisjs-1.0.0a1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.203625 pyvisjs-1.0.0a1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)    11730 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.089287 pyvisjs-1.0.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3321 2024-05-15 12:34:06.089287 pyvisjs-1.0.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.082287 pyvisjs-1.0.0b1/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     8663 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/examples/bluor.py
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/examples/readme.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.084287 pyvisjs-1.0.0b1/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     8831 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    13062 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.086287 pyvisjs-1.0.0b1/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/bs-container.html
+-rw-rw-rw-   0 root         (0) root         (0)     9063 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/functions.js
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/select-edge-filter.html
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/tom-select.html
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.088287 pyvisjs-1.0.0b1/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3321 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      803 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 12:34:06.089287 pyvisjs-1.0.0b1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.088287 pyvisjs-1.0.0b1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    12014 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_utils.py
```

### Comparing `pyvisjs-1.0.0a1/.gitignore` & `pyvisjs-1.0.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/.gitlab-ci.yml` & `pyvisjs-1.0.0b1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/CONTRIBUTING.md` & `pyvisjs-1.0.0b1/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 - Reporting bugs
 - Submitting feature requests
 - Writing code improvements
 - Providing documentation updates
 
 Please follow these steps when contributing:
 
-- **Create an Issue (Optional)**: Before making changes, consider creating an issue (Plan -> Issues -> New issue) to discuss and track the proposed changes. This step helps ensure that your contributions align with the project's goals and can provide helpful context for your merge request.
+- **Create an Issue (Optional)**: Before making changes, consider creating an issue (Plan -> Issues -> New issue) to discuss and track the proposed changes. This step helps ensure that your contributions align with the project's goals and can provide helpful context for your merge request. Simple requirements specification format could be:
+> As a [role],  
+> I want [feature/desire]  
+> so that [rationale/benefit].  
+> For example: [example]
 
 - **Clone the Repository**: Clone the repository to your local machine using the ```git clone``` command.
 
 - **Create a Branch**: Create a new branch for your changes using the ```git checkout -b feature-name``` command, replacing feature-name with a descriptive name for your branch.
 
 - **Create a virtual environment** ```py -m venv .venv```
```

### Comparing `pyvisjs-1.0.0a1/LICENSE` & `pyvisjs-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/PKG-INFO` & `pyvisjs-1.0.0b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0a1
+Version: 1.0.0b1
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,19 +39,21 @@
 Provides-Extra: all
 Requires-Dist: pyvisjs[test]; extra == "all"
 
 # pyvisjs: Python Wrapper for vis.js Network
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
-## Features
+## Workflow
 
-- **Integration**: Easily incorporate vis.js network visualizations into your Python projects.
-- **Flexibility**: Leverage the power of Python to manipulate network data and customize visualizations.
-- **Interactivity**: Enable users to interact with network visualizations directly from Python scripts.
+1. Create a network using python
+2. Apply standatd vis.js options such as colors, shapes or physics
+3. Apply pyvisjs specific options such as filtering or highlighting
+4. Show or generate html file
+5. Enjoy network interactions in your browser
 
 ## Installation
 
 You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
```

### Comparing `pyvisjs-1.0.0a1/README.md` & `pyvisjs-1.0.0b1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # pyvisjs: Python Wrapper for vis.js Network
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
-## Features
+## Workflow
 
-- **Integration**: Easily incorporate vis.js network visualizations into your Python projects.
-- **Flexibility**: Leverage the power of Python to manipulate network data and customize visualizations.
-- **Interactivity**: Enable users to interact with network visualizations directly from Python scripts.
+1. Create a network using python
+2. Apply standatd vis.js options such as colors, shapes or physics
+3. Apply pyvisjs specific options such as filtering or highlighting
+4. Show or generate html file
+5. Enjoy network interactions in your browser
 
 ## Installation
 
 You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
```

### Comparing `pyvisjs-1.0.0a1/examples/bluor.py` & `pyvisjs-1.0.0b1/examples/bluor.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,12 +131,14 @@
         , partner2_name = row["Partner2Name"]
         , country = row["Countries"]
     )
 
 
 
 net.render_template(open_in_browser=True, 
-                    template_filename="bs-container.html", 
-                    #enable_highlighting=True, 
-                    edge_filtering=["country", "category"])
+                    template_filename="tom-select.html", 
+                    enable_highlighting=True, 
+                    edge_filtering=["country", "category"],
+                    node_filtering=["partner_name"]
+                    )
 
 #net.show("example2.html")
```

### Comparing `pyvisjs-1.0.0a1/folder_structure.txt` & `pyvisjs-1.0.0b1/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/pyproject.toml` & `pyvisjs-1.0.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/pyvisjs/base_dictable.py` & `pyvisjs-1.0.0b1/pyvisjs/base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/pyvisjs/edge.py` & `pyvisjs-1.0.0b1/pyvisjs/edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/pyvisjs/network.py` & `pyvisjs-1.0.0b1/pyvisjs/network.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     def to_dict(self):
         return super().to_dict()["_data"]
 
     def show(self, file_name, enable_highlighting=False, edge_filtering=None):
         self.render_template(open_in_browser=True, output_filename=file_name, enable_highlighting=enable_highlighting, edge_filtering=edge_filtering)
 
-    def render_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html", template_filename="basic.html", enable_highlighting=False, edge_filtering=None) -> str:
+    def render_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html", template_filename="basic.html", enable_highlighting=False, edge_filtering=None, node_filtering=None) -> str:
         """This method uses jinja to inject prepared data to a html file from the templates folder (for more info about the injected data see Notes section below).
         
         Parameters
         ----------
         open_in_browser: bool, default=False
             Resolved template will be saved as the `output_filename` and opened with `os.startfile`
 
@@ -147,47 +147,56 @@
 
         >>> .render(
         >>>     width=network_dict["options"].get("width", "100%"),
         >>>     height=network_dict["options"].get("height", "100%"),
         >>>     data=network_dict,
         >>>     pyvisjs={
         >>>         "enable_highlighting": enable_highlighting,
-        >>>         "edge_filtering_fields": edge_filtering_fields,
         >>>         "edge_filtering_lookup": edge_filtering_lookup,
         >>>     },
         >>> )
 
         """
         network_dict = self.to_dict()
         edge_filtering_lookup: Dict = None
-        edge_filtering_fields: List = None
+        node_filtering_lookup: Dict = None
 
+        # edges
         if not edge_filtering is None:
             if not isinstance(edge_filtering, list):
                 edge_filtering = [str(edge_filtering)]
 
             edge_filtering_lookup = {}
-            edge_filtering_fields = []
             for field_name in edge_filtering:
                 tp_field_name = Edge.convert_to_template_attribute(field_name)
                 unique_values = list(set([str(getattr(edge, field_name)) for edge in self.edges if hasattr(edge, field_name)]))
                 unique_values.sort()
                 edge_filtering_lookup[tp_field_name] = unique_values
-                edge_filtering_fields.append(tp_field_name)
+
+        # nodes
+        if not node_filtering is None:
+            if not isinstance(node_filtering, list):
+                node_filtering = [str(node_filtering)]
+
+            node_filtering_lookup = {}
+            for field_name in node_filtering:
+                unique_values = list(set([str(getattr(node, field_name)) for node in self.nodes if hasattr(node, field_name)]))
+                unique_values.sort()
+                node_filtering_lookup[field_name] = unique_values             
         
         html_output = self.env \
             .get_template(template_filename) \
             .render(
                 width=network_dict["options"].get("width", "100%"),
                 height=network_dict["options"].get("height", "100%"),
                 data=network_dict,
                 pyvisjs={
                     "enable_highlighting": enable_highlighting,
-                    "edge_filtering_fields": edge_filtering_fields,
                     "edge_filtering_lookup": edge_filtering_lookup,
+                    "node_filtering_lookup": node_filtering_lookup,
                 },
             )
 
         if save_to_output or open_in_browser:
             file_path = save_file(output_filename, html_output)
 
         if open_in_browser:
```

### Comparing `pyvisjs-1.0.0a1/pyvisjs/node.py` & `pyvisjs-1.0.0b1/pyvisjs/node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/pyvisjs/options.py` & `pyvisjs-1.0.0b1/pyvisjs/options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/pyvisjs/templates/base.html` & `pyvisjs-1.0.0b1/pyvisjs/templates/base.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 <html>
   <head>
-  {%- block head %}
+    {% block head -%}
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>{% block title %}{% endblock %}</title>
+    {% block head_scripts -%}
     <script type="text/javascript" src="https://unpkg.com/vis-network/standalone/umd/vis-network.min.js"></script>
-
+    {%- endblock %}
     <style type="text/css">
-        #visjsnet {
-            width: {{width}};
-            height: {{height}};
-            border: 1px solid lightgray;
-        }
+      {% block head_style -%}
+      #visjsnet {
+          width: {{width}};
+          height: {{height}};
+          border: 1px solid lightgray;
+      }
+      {%- endblock %}
     </style>
-    <title>{% block title %}{% endblock %}</title>
-  {% endblock -%}
+  {%- endblock %}
   </head>
   <body>
-    {% block content -%}{% endblock %}
+    {% block content -%}{%- endblock %}
     <script type="text/javascript">
     {% block javascript %}
 {% include "functions.js" %}
     {% endblock -%}
     </script>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,3 +1,5 @@
-{%- block head %}
-{% endblock -%}
-{% block content -%}{% endblock %}
+{% block head -%}
+{% block head_scripts -%}
+{%- endblock %}
+{%- endblock %}
+{% block content -%}{%- endblock %}
```

### Comparing `pyvisjs-1.0.0a1/pyvisjs/utils.py` & `pyvisjs-1.0.0b1/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-1.0.0b1/pyvisjs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0a1
+Version: 1.0.0b1
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,19 +39,21 @@
 Provides-Extra: all
 Requires-Dist: pyvisjs[test]; extra == "all"
 
 # pyvisjs: Python Wrapper for vis.js Network
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
-## Features
+## Workflow
 
-- **Integration**: Easily incorporate vis.js network visualizations into your Python projects.
-- **Flexibility**: Leverage the power of Python to manipulate network data and customize visualizations.
-- **Interactivity**: Enable users to interact with network visualizations directly from Python scripts.
+1. Create a network using python
+2. Apply standatd vis.js options such as colors, shapes or physics
+3. Apply pyvisjs specific options such as filtering or highlighting
+4. Show or generate html file
+5. Enjoy network interactions in your browser
 
 ## Installation
 
 You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
```

### Comparing `pyvisjs-1.0.0a1/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-1.0.0b1/pyvisjs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 CONTRIBUTING.md
 LICENSE
 README.md
 folder_structure.txt
 pyproject.toml
 requirements.txt
 examples/bluor.py
-examples/readme_usage.py
+examples/readme.py
 pyvisjs/__init__.py
 pyvisjs/_version.py
 pyvisjs/base_dictable.py
 pyvisjs/edge.py
 pyvisjs/network.py
 pyvisjs/node.py
 pyvisjs/options.py
@@ -22,14 +22,15 @@
 pyvisjs.egg-info/requires.txt
 pyvisjs.egg-info/top_level.txt
 pyvisjs/templates/base.html
 pyvisjs/templates/basic.html
 pyvisjs/templates/bs-container.html
 pyvisjs/templates/functions.js
 pyvisjs/templates/select-edge-filter.html
+pyvisjs/templates/tom-select.html
 tests/__init__.py
 tests/test_base_dictable.py
 tests/test_edge.py
 tests/test_network.py
 tests/test_node.py
 tests/test_options.py
 tests/test_utils.py
```

### Comparing `pyvisjs-1.0.0a1/tests/test_base_dictable.py` & `pyvisjs-1.0.0b1/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/tests/test_edge.py` & `pyvisjs-1.0.0b1/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/tests/test_network.py` & `pyvisjs-1.0.0b1/tests/test_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,16 +161,16 @@
 def test_network_render_template_passing_render_default_params(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     PYVISJS={
         "enable_highlighting": False,
-        "edge_filtering_fields": None,
         "edge_filtering_lookup": None,
+        "node_filtering_lookup": None,
     }
     
     # mock
     mock_render = mock_Environment.return_value.get_template.return_value.render
 
     # call
     network = Network("Test Network")
@@ -183,28 +183,33 @@
 def test_network_render_template_passing_render_params(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     TEMPLATE_FILENAME="another_template.html"
     ENABLE_HIGHLIGHTING=True
-    EDGE_FILTERING="node_field" # str(!) not list
+    EDGE_FILTERING="edge_field" # str(!) not list
+    NODE_FILTERING=["field1", "field2"] # list
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
-        "edge_filtering_fields": [EDGE_FILTERING],
-        "edge_filtering_lookup": {"node_field": []},
+        "edge_filtering_lookup": {"edge_field": []},
+        "node_filtering_lookup": {"field1": [], "field2": []},
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
     network = Network("Test Network")
-    html_output = network.render_template(template_filename=TEMPLATE_FILENAME, enable_highlighting=ENABLE_HIGHLIGHTING, edge_filtering=EDGE_FILTERING) # <--------------------
+    html_output = network.render_template( # <--------------------
+        template_filename=TEMPLATE_FILENAME, 
+        enable_highlighting=ENABLE_HIGHLIGHTING, 
+        edge_filtering=EDGE_FILTERING, 
+        node_filtering=NODE_FILTERING)
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_edge_filtering_list(mock_Environment):
@@ -221,63 +226,67 @@
             {'to': '3', 'field1': 'AM', 'from': '1'}, 
             {'to': '3', 'field1': 'JL', 'from': '2'}], 
         'options': {}
     }
     TEMPLATE_FILENAME="another_template.html"
     ENABLE_HIGHLIGHTING=True
     EDGE_FILTERING=["field1", "field2"]
+    NODE_FILTERING=["label", "shape"]
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
-        "edge_filtering_fields": EDGE_FILTERING,
         "edge_filtering_lookup": {"field1": ["AM", "JL"], "field2": []},
+        "node_filtering_lookup": {"label": ["1", "2", "3"], "shape": ["dot"]},
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
     net = Network("Network1")
     net.add_edge(1, 2, field1="AM")
     net.add_edge(1, 3, field1="AM")
     net.add_edge(2, 3, field1="JL")
-    html_output = net.render_template(# <--------------------
+    html_output = net.render_template( # <--------------------
         template_filename=TEMPLATE_FILENAME, 
         enable_highlighting=ENABLE_HIGHLIGHTING, 
-        edge_filtering=EDGE_FILTERING) 
+        edge_filtering=EDGE_FILTERING,
+        node_filtering=NODE_FILTERING) 
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_edge_filtering_int(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     TEMPLATE_FILENAME="another_template.html"
     ENABLE_HIGHLIGHTING=True
     EDGE_FILTERING=34
+    NODE_FILTERING=22
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
-        "edge_filtering_fields": [str(EDGE_FILTERING)],
         "edge_filtering_lookup": {"34": []},
+        "node_filtering_lookup": {"22": []},
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
     net = Network("Network1")
     html_output = net.render_template(# <--------------------
         template_filename=TEMPLATE_FILENAME, 
         enable_highlighting=ENABLE_HIGHLIGHTING, 
-        edge_filtering=EDGE_FILTERING) 
+        edge_filtering=EDGE_FILTERING,
+        node_filtering=NODE_FILTERING) 
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
```

### Comparing `pyvisjs-1.0.0a1/tests/test_node.py` & `pyvisjs-1.0.0b1/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/tests/test_options.py` & `pyvisjs-1.0.0b1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0a1/tests/test_utils.py` & `pyvisjs-1.0.0b1/tests/test_utils.py`

 * *Files identical despite different names*

