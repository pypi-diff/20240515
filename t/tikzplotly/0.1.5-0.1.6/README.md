# Comparing `tmp/tikzplotly-0.1.5.tar.gz` & `tmp/tikzplotly-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikzplotly-0.1.5.tar", last modified: Mon May 13 08:33:36 2024, max compression
+gzip compressed data, was "tikzplotly-0.1.6.tar", last modified: Wed May 15 12:16:22 2024, max compression
```

## Comparing `tikzplotly-0.1.5.tar` & `tikzplotly-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:33:36.887591 tikzplotly-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-13 08:33:36.887591 tikzplotly-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:33:36.887591 tikzplotly-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:33:36.883591 tikzplotly-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:33:36.883591 tikzplotly-0.1.5/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tests/test_heatmaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    14231 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tests/test_line_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tests/test_markers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:33:36.883591 tikzplotly-0.1.5/src/tikzplotly/
--rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)    39173 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_dataContainer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4801 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_marker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3919 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_tex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-13 08:33:27.000000 tikzplotly-0.1.5/src/tikzplotly/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:33:36.887591 tikzplotly-0.1.5/src/tikzplotly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-13 08:33:36.000000 tikzplotly-0.1.5/src/tikzplotly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-13 08:33:36.000000 tikzplotly-0.1.5/src/tikzplotly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:33:36.000000 tikzplotly-0.1.5/src/tikzplotly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 08:33:36.000000 tikzplotly-0.1.5/src/tikzplotly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 08:33:36.000000 tikzplotly-0.1.5/src/tikzplotly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:16:22.136021 tikzplotly-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-15 12:16:22.136021 tikzplotly-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:16:22.136021 tikzplotly-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:16:22.132021 tikzplotly-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:16:22.132021 tikzplotly-0.1.6/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tests/test_heatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14231 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tests/test_line_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tests/test_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:16:22.132021 tikzplotly-0.1.6/src/tikzplotly/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39173 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_dataContainer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4811 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_marker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3979 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_tex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/src/tikzplotly/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:16:22.136021 tikzplotly-0.1.6/src/tikzplotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-15 12:16:22.000000 tikzplotly-0.1.6/src/tikzplotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-15 12:16:22.000000 tikzplotly-0.1.6/src/tikzplotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:16:22.000000 tikzplotly-0.1.6/src/tikzplotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 12:16:22.000000 tikzplotly-0.1.6/src/tikzplotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 12:16:22.000000 tikzplotly-0.1.6/src/tikzplotly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:16:22.136021 tikzplotly-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/tests/test_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/tests/test_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-15 12:16:17.000000 tikzplotly-0.1.6/tests/test_scatter.py
```

### Comparing `tikzplotly-0.1.5/LICENSE` & `tikzplotly-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/PKG-INFO` & `tikzplotly-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikzplotly
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convert plotly figures to LaTeX / tikz figures
 Author-email: Thomas Saigre <tikzplotly@outlook.fr>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 @thomas-saigre
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,14 @@
         SOFTWARE.
 Project-URL: Code, https://github.com/thomas-saigre/tikzplotly
 Project-URL: Issues, https://github.com/thomas-saigre/tikzplotly/issues
 Keywords: plotly,latex,tikz,figure,conversion,graphics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Scientific/Engineering :: Visualization
@@ -48,14 +47,17 @@
 
 ![logo-tikzplotly](https://raw.githubusercontent.com/thomas-saigre/tikzplotly/main/doc/img/logo.svg "Tikzplotly")
 
 [![PyPi Version](https://img.shields.io/pypi/v/tikzplotly.svg?style=flat-square)](https://pypi.org/project/tikzplotly)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tikzplotly.svg?style=flat-square)](https://pypi.org/pypi/tikzplotly/)
 
 [![Issue](https://img.shields.io/github/issues-raw/thomas-saigre/tikzplotly?style=flat-square)](https://github.com/thomas-saigre/tikzplotly/issues)
+[![codecov](https://img.shields.io/codecov/c/github/thomas-saigre/tikzplotly.svg?style=flat-square)](https://codecov.io/gh/thomas-saigre/tikzplotly)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/thomas-saigre/tikzplotly/ci.yml?style=flat-square)
+
 
 # Tikzplotly
 
 Convert [plotly](https://plotly.com/python/) figures to tikz code for inclusion into [PGFPlots](https://www.ctan.org/pkg/pgfplots) ([PGF/TikZ](https://www.ctan.org/pkg/pgf)) figures.
 
 This results in a ti*k*z code, that can be easily included into your LaTeX document.
 This also allows to easily edit the content of the figure.
```

### Comparing `tikzplotly-0.1.5/README.md` & `tikzplotly-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ![logo-tikzplotly](https://raw.githubusercontent.com/thomas-saigre/tikzplotly/main/doc/img/logo.svg "Tikzplotly")
 
 [![PyPi Version](https://img.shields.io/pypi/v/tikzplotly.svg?style=flat-square)](https://pypi.org/project/tikzplotly)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tikzplotly.svg?style=flat-square)](https://pypi.org/pypi/tikzplotly/)
 
 [![Issue](https://img.shields.io/github/issues-raw/thomas-saigre/tikzplotly?style=flat-square)](https://github.com/thomas-saigre/tikzplotly/issues)
+[![codecov](https://img.shields.io/codecov/c/github/thomas-saigre/tikzplotly.svg?style=flat-square)](https://codecov.io/gh/thomas-saigre/tikzplotly)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/thomas-saigre/tikzplotly/ci.yml?style=flat-square)
+
 
 # Tikzplotly
 
 Convert [plotly](https://plotly.com/python/) figures to tikz code for inclusion into [PGFPlots](https://www.ctan.org/pkg/pgfplots) ([PGF/TikZ](https://www.ctan.org/pkg/pgf)) figures.
 
 This results in a ti*k*z code, that can be easily included into your LaTeX document.
 This also allows to easily edit the content of the figure.
```

### Comparing `tikzplotly-0.1.5/pyproject.toml` & `tikzplotly-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tikzplotly"
-version = "0.1.5"
+version = "0.1.6"
 description = "Convert plotly figures to LaTeX / tikz figures"
 readme = "README.md"
 authors = [{name = "Thomas Saigre", email = "tikzplotly@outlook.fr"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Multimedia :: Graphics :: Graphics Conversion",
     "Topic :: Scientific/Engineering :: Visualization",
```

### Comparing `tikzplotly-0.1.5/src/tests/test_heatmaps.py` & `tikzplotly-0.1.6/src/tests/test_heatmaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 import os
 import tikzplotly
 
 from tikzplotly._tex import tex_create_document, tex_begin_environment, tex_end_environment, tex_end_all_environment
 
 import plotly
 import plotly.express as px
-import pandas as pd
 import plotly.graph_objects as go
 import numpy as np
 import datetime
-import numpy as np
 np.random.seed(1)
 
 def fig1():
     fig = px.imshow([[1, 20, 30],
                     [20, 1, 60],
                     [30, 60, 1]])
     # fig.show()
@@ -164,37 +162,35 @@
     print("Tikzploty : ", tikzplotly.__version__)
     print("Plotly : ", plotly.__version__)
     print("Test line charts")
 
     file_directory = os.path.dirname(os.path.abspath(__file__))
 
     functions = [
-        ("1", fig1),
-        ("2", fig2),
-        # ("3", fig3),          # texttemplate not supported
-        ("4", fig4),
-        ("5", fig5),
-        ("6", fig6),
+        # ("1", fig1),
+        # ("2", fig2),
+        # # ("3", fig3),          # texttemplate not supported
+        # ("4", fig4),
+        # ("5", fig5),
+        # ("6", fig6),
         ("7", fig7),
-        # ("8", fig8),          # Not supported
-        ("9", fig9),
-        ("11", fig11)
-
+        # # ("8", fig8),          # Not supported
+        # ("9", fig9),
+        # ("11", fig11)
     ]
 
     main_tex_content = tex_create_document(options="twocolumn", compatibility="newest")
     main_tex_content += "\\usepackage[left=1cm, right=1cm, top=1cm, bottom=1cm]{geometry}\n"
     main_tex_content += "\n"
     stack_env = []
     main_tex_content += tex_begin_environment("document", stack_env) + '\n'
 
     for i, f in functions:
         print(f"Figure {i}")
         fig, title = f()
-        data = fig.data
         save_path = os.path.join(file_directory, "outputs", "test_heatmap", "fig{}.tex".format(i))
         tikzplotly.save(save_path, fig, img_name=os.path.join(file_directory, "outputs", "test_heatmap", "fig{}.png".format(i)))
         main_tex_content += tex_begin_environment("figure", stack_env)
         main_tex_content += "  \\input{fig" + str(i) + ".tex}\n"
         main_tex_content += "  \\caption{" + title + "}\n"
         main_tex_content += tex_end_environment(stack_env) + '\n'
```

### Comparing `tikzplotly-0.1.5/src/tests/test_line_charts.py` & `tikzplotly-0.1.6/src/tests/test_line_charts.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tests/test_markers.py` & `tikzplotly-0.1.6/src/tests/test_markers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # From https://plotly.com/python/marker-style/
 import plotly
 import plotly.express as px
-import pandas as pd
 import plotly.graph_objects as go
 import numpy as np
 import tikzplotly
 import os
 import plotly.graph_objects as go
 from plotly.validators.scatter.marker import SymbolValidator
 from warnings import warn
```

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_annotations.py` & `tikzplotly-0.1.6/src/tikzplotly/_annotations.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_axis.py` & `tikzplotly-0.1.6/src/tikzplotly/_axis.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_color.py` & `tikzplotly-0.1.6/src/tikzplotly/_color.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_data.py` & `tikzplotly-0.1.6/src/tikzplotly/_data.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_dataContainer.py` & `tikzplotly-0.1.6/src/tikzplotly/_dataContainer.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_heatmap.py` & `tikzplotly-0.1.6/src/tikzplotly/_heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,16 @@
     elif (colorscale := fig.layout.coloraxis.colorscale) is not None:
         axis.add_option("colormap", get_tikz_colorscale(colorscale))
     elif data.showscale is not False:
         warn("No colorscale found, using default")
         axis.add_option("colormap", get_tikz_colorscale(DEFAULT_COLORSCALE))
 
     tmp = np.where(figure_data == None, np.nan, figure_data)
-    axis.add_option("point meta max", tmp.max())
-    axis.add_option("point meta min", tmp.min())
+    axis.add_option("point meta max", np.nanmax(tmp))
+    axis.add_option("point meta min", np.nanmin(tmp))
     axis.add_option("xmin", xmin)
     axis.add_option("xmax", xmax)
     axis.add_option("ymin", ymax)
     axis.add_option("ymax", ymin)
     axis.add_option("tick align", "outside")
     axis.add_option("tick pos", "left")
```

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_marker.py` & `tikzplotly-0.1.6/src/tikzplotly/_marker.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_save.py` & `tikzplotly-0.1.6/src/tikzplotly/_save.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,21 +74,24 @@
 
     code = """"""
     stack_env = []
 
     if include_disclamer:
         code += tex_comment(f"This file was created with tikzplotly version {__version__}.")
 
-    code += data_container.exportData()
-    code += "\n"
+    if len(data_container.data) > 0:
+        code += data_container.exportData()
+        code += "\n"
 
     code += tex_begin_environment("tikzpicture", stack_env, options=tikz_options)
 
     code += "\n"
-    for color in colors_set:
+    color_list = list(colors_set)
+    color_list.sort()
+    for color in color_list:
         code += tex_add_color(color[0], color[1], color[2])
     code += "\n"
 
     code += axis.open_environment(stack_env)
 
     if figure_layout.legend.title.text is not None and figure_layout.showlegend:
         code += "\\addlegendimage{empty legend}\n"
@@ -103,15 +106,15 @@
         code = re.sub(r"\\addlegendentry{.+}\n", "", code)
 
     code += tex_end_all_environment(stack_env)
 
     return code
 
 
-def save(filepath: str | Path, *args, encoding: str | None = None, **kwargs):
+def save(filepath, *args, **kwargs):
     """Save a figure to a file or a stream.
 
     Parameters
     ----------
     filepath : str or Path
         A string containing a path to a filename, or a Path object.
     *args, **kwargs
```

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_scatter.py` & `tikzplotly-0.1.6/src/tikzplotly/_scatter.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_tex.py` & `tikzplotly-0.1.6/src/tikzplotly/_tex.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly/_utils.py` & `tikzplotly-0.1.6/src/tikzplotly/_utils.py`

 * *Files identical despite different names*

### Comparing `tikzplotly-0.1.5/src/tikzplotly.egg-info/PKG-INFO` & `tikzplotly-0.1.6/src/tikzplotly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikzplotly
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convert plotly figures to LaTeX / tikz figures
 Author-email: Thomas Saigre <tikzplotly@outlook.fr>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 @thomas-saigre
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,14 @@
         SOFTWARE.
 Project-URL: Code, https://github.com/thomas-saigre/tikzplotly
 Project-URL: Issues, https://github.com/thomas-saigre/tikzplotly/issues
 Keywords: plotly,latex,tikz,figure,conversion,graphics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Scientific/Engineering :: Visualization
@@ -48,14 +47,17 @@
 
 ![logo-tikzplotly](https://raw.githubusercontent.com/thomas-saigre/tikzplotly/main/doc/img/logo.svg "Tikzplotly")
 
 [![PyPi Version](https://img.shields.io/pypi/v/tikzplotly.svg?style=flat-square)](https://pypi.org/project/tikzplotly)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tikzplotly.svg?style=flat-square)](https://pypi.org/pypi/tikzplotly/)
 
 [![Issue](https://img.shields.io/github/issues-raw/thomas-saigre/tikzplotly?style=flat-square)](https://github.com/thomas-saigre/tikzplotly/issues)
+[![codecov](https://img.shields.io/codecov/c/github/thomas-saigre/tikzplotly.svg?style=flat-square)](https://codecov.io/gh/thomas-saigre/tikzplotly)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/thomas-saigre/tikzplotly/ci.yml?style=flat-square)
+
 
 # Tikzplotly
 
 Convert [plotly](https://plotly.com/python/) figures to tikz code for inclusion into [PGFPlots](https://www.ctan.org/pkg/pgfplots) ([PGF/TikZ](https://www.ctan.org/pkg/pgf)) figures.
 
 This results in a ti*k*z code, that can be easily included into your LaTeX document.
 This also allows to easily edit the content of the figure.
```

