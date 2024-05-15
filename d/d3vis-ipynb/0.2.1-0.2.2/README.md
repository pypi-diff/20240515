# Comparing `tmp/d3vis_ipynb-0.2.1.tar.gz` & `tmp/d3vis_ipynb-0.2.2.tar.gz`

## Comparing `d3vis_ipynb-0.2.1.tar` & `d3vis_ipynb-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/D3vis_ipynb.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/MANIFEST.in
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/RELEASE.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/install.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/setup.cfg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/setup.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/_version.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/custom.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/embedding.py
--rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/widgets.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/package.json
--rw-r--r--   0        0        0    27903 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/363.d2d286fd78e0907ef3c1.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js
--rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/remoteEntry.065ac4641043ad457b9a.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/style.js
--rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    93725 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/d3vis_ipynb/nbextension/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/amd-public-path.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/package.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/webpack.config.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/webpack.exports.config.js
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/css/widget.css
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/extension.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/index.js
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/labplugin.js
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/web-dev.js
--rw-r--r--   0        0        0    13007 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/widgets.js
--rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/graphs/barplot.js
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/graphs/histogramplot.js
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/graphs/linearhistplot.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/graphs/rangeslider.js
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/graphs/scatterplot.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/tools/lasso.js
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/js/lib/wrappers/embedding.wrapper.js
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/README.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/D3vis_ipynb.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/MANIFEST.in
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/RELEASE.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/install.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/setup.cfg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/setup.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/_version.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/custom.py
+-rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/embedding.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/widgets.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/package.json
+-rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/112.a36093df8a8075509d10.js
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/493.9def85d738cd0e72c5f5.js
+-rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/remoteEntry.6f9edec5dc6ff6501b02.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/style.js
+-rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    98223 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/d3vis_ipynb/nbextension/index.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/amd-public-path.js
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/package.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/webpack.config.js
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/webpack.exports.config.js
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/css/widget.css
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/extension.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/index.js
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/labplugin.js
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/web-dev.js
+-rw-r--r--   0        0        0    15340 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/widgets.js
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/barplot.js
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/histogramplot.js
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/linearhistplot.js
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/linearplot.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/rangeslider.js
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/graphs/scatterplot.js
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/tools/group_data.js
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/js/lib/tools/lasso.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/README.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.2.2/PKG-INFO
```

### Comparing `d3vis_ipynb-0.2.1/RELEASE.md` & `d3vis_ipynb-0.2.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/setup.cfg` & `d3vis_ipynb-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/__init__.py` & `d3vis_ipynb-0.2.2/d3vis_ipynb/__init__.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/custom.py` & `d3vis_ipynb-0.2.2/d3vis_ipynb/custom.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/widgets.py` & `d3vis_ipynb-0.2.2/d3vis_ipynb/widgets.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,53 +12,33 @@
     _view_name = Unicode("LinearHistPlotView").tag(sync=True)
     _model_name = Unicode("LinearHistPlotModel").tag(sync=True)
     _view_module = Unicode("d3vis_ipynb").tag(sync=True)
     _model_module = Unicode("d3vis_ipynb").tag(sync=True)
     _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
     _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
 
-    _name = "linearhistplot"
-    _observing = []
-
     linearData_x = List([]).tag(sync=True)
     linearData_y = List([]).tag(sync=True)
     histogramData = List([]).tag(sync=True)
     elementId = Unicode().tag(sync=True)
     clickedValue = Unicode().tag(sync=True)
 
-    def name(self):
-        return self._name
-
-    def export_data(self):
-        data = {
-            "linearData_x": self.linearData_x,
-            "linearData_y": self.linearData_y,
-            "histogramData": self.histogramData,
-            "elementId": self.elementId,
-            "observing": self._observing,
-        }
-
-        return {self._name: data}
-
     def on_click_value(self, callback):
         self.observe(callback, names=["clickedValue"])
 
 
 @widgets.register
 class ScatterPlot(widgets.DOMWidget):
     _view_name = Unicode("ScatterPlotView").tag(sync=True)
     _model_name = Unicode("ScatterPlotModel").tag(sync=True)
     _view_module = Unicode("d3vis_ipynb").tag(sync=True)
     _model_module = Unicode("d3vis_ipynb").tag(sync=True)
     _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
     _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
 
-    _name = "scatterplot"
-    _observing = []
-
     dataRecords = List([]).tag(sync=True)
     x = Unicode().tag(sync=True)
     y = Unicode().tag(sync=True)
     hue = Unicode().tag(sync=True)
     elementId = Unicode().tag(sync=True)
     clickedValue = Unicode().tag(sync=True)
     selectedValuesRecords = List([]).tag(sync=True)
@@ -80,48 +60,73 @@
     def selectedValues(self):
         return pd.DataFrame.from_records(self.selectedValuesRecords)
 
     @selectedValues.setter
     def selectedValues(self, val):
         self.selectedValuesRecords = val.to_dict(orient="records")
 
-    def name(self):
-        return self._name
+    def on_select_values(self, callback):
+        self.observe(callback, names=["selectedValuesRecords"])
+
+    def on_click_value(self, callback):
+        self.observe(callback, names=["clickedValue"])
+
+@widgets.register
+class LinearPlot(widgets.DOMWidget):
+    _view_name = Unicode("LinearPlotView").tag(sync=True)
+    _model_name = Unicode("LinearPlotModel").tag(sync=True)
+    _view_module = Unicode("d3vis_ipynb").tag(sync=True)
+    _model_module = Unicode("d3vis_ipynb").tag(sync=True)
+    _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
+    _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
+
+    dataRecords = List([]).tag(sync=True)
+    x = Unicode().tag(sync=True)
+    y = Unicode().tag(sync=True)
+    hue = Unicode().tag(sync=True)
+    elementId = Unicode().tag(sync=True)
+    clickedValue = Unicode().tag(sync=True)
+    selectedValuesRecords = List([]).tag(sync=True)
+
+    def __init__(self, data, **kwargs):
+        self.data = data
+        self.selectedValues = pd.DataFrame()
+        super().__init__(**kwargs)
+
+    @property
+    def data(self):
+        return pd.DataFrame.from_records(self.dataRecords)
+
+    @data.setter
+    def data(self, val):
+        self.dataRecords = val.to_dict(orient="records")
 
-    def export_data(self):
-        data = {
-            "data": self.data,
-            "x": self.x,
-            "y": self.y,
-            "hue": self.hue,
-            "elementId": self.elementId,
-            "observing": self._observing,
-        }
+    @property
+    def selectedValues(self):
+        return pd.DataFrame.from_records(self.selectedValuesRecords)
 
-        return {self._name: data}
+    @selectedValues.setter
+    def selectedValues(self, val):
+        self.selectedValuesRecords = val.to_dict(orient="records")
 
     def on_select_values(self, callback):
         self.observe(callback, names=["selectedValuesRecords"])
 
     def on_click_value(self, callback):
         self.observe(callback, names=["clickedValue"])
 
-
 @widgets.register
 class BarPlot(widgets.DOMWidget):
     _view_name = Unicode("BarPlotView").tag(sync=True)
     _model_name = Unicode("BarPlotModel").tag(sync=True)
     _view_module = Unicode("d3vis_ipynb").tag(sync=True)
     _model_module = Unicode("d3vis_ipynb").tag(sync=True)
     _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
     _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
 
-    _name = "barplot"
-    _observing = []
-
     dataRecords = List([]).tag(sync=True)
     x = Unicode().tag(sync=True)
     y = Unicode().tag(sync=True)
     hue = Unicode().tag(sync=True)
     elementId = Unicode().tag(sync=True)
 
     def __init__(self, data, **kwargs):
@@ -132,42 +137,24 @@
     def data(self):
         return pd.DataFrame.from_records(self.dataRecords)
 
     @data.setter
     def data(self, val):
         self.dataRecords = val.to_dict(orient="records")
 
-    def name(self):
-        return self._name
-
-    def export_data(self):
-        data = {
-            "data": self.data,
-            "x": self.x,
-            "y": self.y,
-            "hue": self.hue,
-            "elementId": self.elementId,
-            "observing": self._observing,
-        }
-
-        return {self._name: data}
-
 
 @widgets.register
 class HistogramPlot(widgets.DOMWidget):
     _view_name = Unicode("HistogramPlotView").tag(sync=True)
     _model_name = Unicode("HistogramPlotModel").tag(sync=True)
     _view_module = Unicode("d3vis_ipynb").tag(sync=True)
     _model_module = Unicode("d3vis_ipynb").tag(sync=True)
     _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
     _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
 
-    _name = "histogramplot"
-    _observing = []
-
     dataRecords = List([]).tag(sync=True)
     x = Unicode().tag(sync=True)
     start = Float().tag(sync=True)
     end = Float().tag(sync=True)
     elementId = Unicode().tag(sync=True)
 
     def __init__(self, data, **kwargs):
@@ -178,42 +165,24 @@
     def data(self):
         return pd.DataFrame.from_records(self.dataRecords)
 
     @data.setter
     def data(self, val):
         self.dataRecords = val.to_dict(orient="records")
 
-    def name(self):
-        return self._name
-
-    def export_data(self):
-        data = {
-            "data": self.data,
-            "x": self.x,
-            "start": self.start,
-            "end": self.end,
-            "elementId": self.elementId,
-            "observing": self._observing,
-        }
-
-        return {self._name: data}
-
 
 @widgets.register
 class RangeSlider(widgets.DOMWidget):
     _view_name = Unicode("RangeSliderView").tag(sync=True)
     _model_name = Unicode("RangeSliderModel").tag(sync=True)
     _view_module = Unicode("d3vis_ipynb").tag(sync=True)
     _model_module = Unicode("d3vis_ipynb").tag(sync=True)
     _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
     _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
 
-    _name = "rangeslider"
-    _observing = []
-
     dataRecords = List([]).tag(sync=True)
     variable = Unicode().tag(sync=True)
     step = Float().tag(sync=True)
     description = Unicode().tag(sync=True)
     minValue = Float().tag(sync=True)
     maxValue = Float().tag(sync=True)
     elementId = Unicode().tag(sync=True)
@@ -226,24 +195,9 @@
     def data(self):
         return pd.DataFrame.from_records(self.dataRecords)
 
     @data.setter
     def data(self, val):
         self.dataRecords = val.to_dict(orient="records")
 
-    def name(self):
-        return self._name
-
-    def export_data(self):
-        data = {
-            "data": self.data,
-            "variable": self.variable,
-            "step": self.step,
-            "description": self.description,
-            "elementId": self.elementId,
-            "observing": self._observing,
-        }
-
-        return {self._name: data}
-
     def on_drag(self, callback):
         self.observe(callback, names=["minValue", "maxValue"])
```

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/package.json` & `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9533435314685316%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.6f9edec5dc6ff6501b02.js'}}",*

 * * "'scripts'": "{delete: ['start:export', 'export']}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -16,15 +16,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.065ac4641043ad457b9a.js"
+            "load": "static/remoteEntry.6f9edec5dc6ff6501b02.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -47,16 +47,14 @@
     },
     "scripts": {
         "build": "webpack --mode=development && yarn run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension",
-        "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
-        "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/363.d2d286fd78e0907ef3c1.js` & `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/112.a36093df8a8075509d10.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,323 +1,478 @@
 "use strict";
 (self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || []).push([
-    [363], {
-        363: (e, t, n) => {
+    [112], {
+        112: (e, t, n) => {
             n.r(t), n.d(t, {
-                BarPlotModel: () => S,
-                BarPlotView: () => V,
-                EmbeddingModel: () => C,
-                EmbeddingView: () => O,
-                HistogramPlotModel: () => D,
-                HistogramPlotView: () => j,
-                LinearHistPlotModel: () => M,
-                LinearHistPlotView: () => E,
-                RangeSliderModel: () => I,
-                RangeSliderView: () => R,
-                ScatterPlotModel: () => L,
+                BarPlotModel: () => j,
+                BarPlotView: () => C,
+                EmbeddingModel: () => B,
+                EmbeddingView: () => W,
+                HistogramPlotModel: () => R,
+                HistogramPlotView: () => I,
+                LinearHistPlotModel: () => E,
+                LinearHistPlotView: () => S,
+                LinearPlotModel: () => D,
+                LinearPlotView: () => O,
+                RangeSliderModel: () => P,
+                RangeSliderView: () => H,
+                ScatterPlotModel: () => V,
                 ScatterPlotView: () => A,
-                author: () => B.author,
-                dependencies: () => B.dependencies,
-                description: () => B.description,
-                devDependencies: () => B.devDependencies,
-                files: () => B.files,
-                jupyterlab: () => B.jupyterlab,
-                keywords: () => B.keywords,
-                license: () => B.license,
-                main: () => B.main,
-                name: () => B.name,
-                repository: () => B.repository,
-                scripts: () => B.scripts,
-                version: () => B.version
+                author: () => T.author,
+                dependencies: () => T.dependencies,
+                description: () => T.description,
+                devDependencies: () => T.devDependencies,
+                files: () => T.files,
+                jupyterlab: () => T.jupyterlab,
+                keywords: () => T.keywords,
+                license: () => T.license,
+                main: () => T.main,
+                name: () => T.name,
+                repository: () => T.repository,
+                scripts: () => T.scripts,
+                version: () => T.version
             });
             var a = n(801),
                 i = n(72),
                 o = n.n(i),
                 s = n(825),
                 r = n.n(s),
                 l = n(659),
                 d = n.n(l),
                 c = n(56),
                 m = n.n(c),
                 u = n(540),
                 p = n.n(u),
                 h = n(113),
                 g = n.n(h),
-                v = n(930),
-                f = {};
-            f.styleTagTransform = g(), f.setAttributes = m(), f.insert = d().bind(null, "head"), f.domAPI = r(), f.insertStyleElement = p(), o()(v.A, f), v.A && v.A.locals && v.A.locals;
+                f = n(930),
+                v = {};
+            v.styleTagTransform = g(), v.setAttributes = m(), v.insert = d().bind(null, "head"), v.domAPI = r(), v.insertStyleElement = p(), o()(f.A, v), f.A && f.A.locals && f.A.locals;
             var _ = n(840);
 
             function x(e) {
                 const t = e.reduce(((e, t) => e + t), 0) / e.length,
                     n = 1.96 * function(e, t) {
                         let n = 0;
                         return e.forEach((e => n += (e - t) ** 2)), n = Math.sqrt(n) / e.length, n
                     }(e, t);
                 return [t - n, t + n]
             }
-            const b = n(330),
-                y = 400,
-                w = {
+
+            function y(e, t, n, a, i, o, s, r, l, d) {
+                let c = [];
+                const m = _.line(),
+                    u = _.select(e).selectAll(".dot"),
+                    p = _.drag().on("start", (function() {
+                        c = [], r(), _.select(e).select("svg").append("path").attr("id", "lasso" + d)
+                    })).on("drag", (function(e) {
+                        let t = e.sourceEvent.offsetX,
+                            n = e.sourceEvent.offsetY;
+                        c.push([t, n]), _.select("#lasso" + d).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", m(c))
+                    })).on("end", (function() {
+                        let e = [];
+                        u.each(((r, l) => {
+                            (function(e, t) {
+                                for (var n = e[0], a = e[1], i = !1, o = 0, s = t.length - 1; o < t.length; s = o++) {
+                                    var r = t[o][0],
+                                        l = t[o][1],
+                                        d = t[s][0],
+                                        c = t[s][1];
+                                    l > a != c > a && n < (d - r) * (a - l) / (c - l) + r && (i = !i)
+                                }
+                                return i
+                            })([t(r[a]) + o, n(r[i]) + s], c) && (_.select("#dot-" + d + r.id).style("fill", "red").attr("r", 6), e.push(r))
+                        })), _.select("#lasso" + d).remove(), l(e)
+                    }));
+                _.select(e).call(p)
+            }
+
+            function b(e, t) {
+                return e.reduce((function(e, n) {
+                    return {
+                        ...e,
+                        [n[t]]: [...e[n[t]] ?? [], n]
+                    }
+                }), {})
+            }
+            const w = n(330),
+                k = 400,
+                M = {
                     top: 20,
                     right: 20,
                     bottom: 30,
                     left: 40
                 };
 
-            function k(e) {
+            function L(e) {
                 e.timeout && clearTimeout(e.timeout), e.timeout = setTimeout((() => {
                     e.plot()
                 }), 100)
             }
-            class M extends a.DOMWidgetModel {
+            class E extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: M.model_name,
-                        _view_name: M.view_name,
-                        _model_module: M.model_module,
-                        _view_module: M.view_module,
-                        _model_module_version: M.model_module_version,
-                        _view_module_version: M.view_module_version,
+                        _model_name: E.model_name,
+                        _view_name: E.view_name,
+                        _model_module: E.model_module,
+                        _view_module: E.view_module,
+                        _model_module_version: E.model_module_version,
+                        _view_module_version: E.view_module_version,
                         linearData_x: [],
                         linearData_y: [],
                         histogramData: [],
                         elementId: String,
                         clickedValue: String
                     }
                 }
                 static model_name = "LinearHistPlotModel";
-                static model_module = b.name;
-                static model_module_version = b.version;
+                static model_module = w.name;
+                static model_module_version = w.version;
                 static view_name = "LinearHistPlotView";
-                static view_module = b.name;
-                static view_module_version = b.version
+                static view_module = w.name;
+                static view_module_version = w.version
             }
-            class E extends a.DOMWidgetView {
+            class S extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:linearData_x", (() => k(this)), this), this.model.on("change:linearData_y", (() => k(this)), this), this.model.on("change:histogramData", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    L(this), this.model.on("change:linearData_x", (() => L(this)), this), this.model.on("change:linearData_y", (() => L(this)), this), this.model.on("change:histogramData", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("linearData_x"),
                         t = this.model.get("linearData_y"),
                         n = this.model.get("histogramData"),
                         a = this.model.get("elementId");
-                    let i = y,
+                    let i = k,
                         o = this.el;
                     a && (o = document.getElementById(a), i = o.clientHeight);
                     let s = o.clientWidth;
-                    const r = w;
+                    const r = M;
                     ! function(e, t, n, a, i, o, s, r) {
                         const l = o - r.left - r.right,
                             d = s - r.top - r.bottom,
                             c = d / 4;
                         _.select(a).selectAll("*").remove();
                         const m = Math.min(_.min(e), _.min(n)),
                             u = Math.max(_.max(e), _.max(n)),
                             p = _.scaleLinear().range([0, l]),
                             h = _.scaleLinear().range([d, 0]),
                             g = _.scaleLinear().range([c, 0]),
-                            v = _.axisBottom(p),
-                            f = _.axisLeft(h),
+                            f = _.axisBottom(p),
+                            v = _.axisLeft(h),
                             x = _.bin().thresholds(20).value((e => Math.round(10 * e) / 10))(n),
-                            b = _.select(a).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
+                            y = _.select(a).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
                         p.domain([m, u]), h.domain(_.extent(t)), g.domain([0, _.max(x, (e => e.length))]);
-                        const y = b.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
-                            w = b.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
-                        b.append("g").attr("transform", "translate(0," + d + ")").call(v).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), b.append("g").call(f).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end");
+                        const b = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                            w = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
+                        y.append("g").attr("transform", "translate(0," + d + ")").call(f).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), y.append("g").call(v).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end");
                         const k = [];
                         k.x0 = x[0].x0 - 2.5, k.x1 = x[0].x1 - 2.5, x.unshift(k);
                         const M = [];
-                        M.x0 = x[x.length - 1].x0 + 2.5, M.x1 = x[x.length - 1].x1 + 2.5, b.append("path").datum(x).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", _.line().x((e => p((e.x1 + e.x0) / 2))).y((e => g(e.length) + d - c)).curve(_.curveCatmullRom));
-                        const E = e.map(((e, n) => [e, t[n]])).map((([e, t]) => ({
+                        M.x0 = x[x.length - 1].x0 + 2.5, M.x1 = x[x.length - 1].x1 + 2.5, y.append("path").datum(x).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", _.line().x((e => p((e.x1 + e.x0) / 2))).y((e => g(e.length) + d - c)).curve(_.curveCatmullRom));
+                        const L = e.map(((e, n) => [e, t[n]])).map((([e, t]) => ({
                             x: e,
                             y: t
                         })));
-                        b.append("path").datum(E).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", _.line().x((e => p(e.x))).y((e => h(e.y)))), b.selectAll("myCircles").data(E).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => p(e.x))).attr("cy", (e => h(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
-                            y.style("opacity", 1), w.style("opacity", 1), y.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                        y.append("path").datum(L).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", _.line().x((e => p(e.x))).y((e => h(e.y)))), y.selectAll("myCircles").data(L).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => p(e.x))).attr("cy", (e => h(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
+                            b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
                         })).on("mouseout", (function() {
-                            y.style("opacity", 0), w.style("opacity", 0)
+                            b.style("opacity", 0), w.style("opacity", 0)
                         })).on("click", (function(e, t) {
                             const n = "x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10;
                             void 0 !== i && i(n)
                         }))
                     }(e, t, n, o, this.setValue.bind(this), s, i, r)
                 }
                 setValue(e) {
                     this.model.set({
                         clickedValue: e
                     }), this.model.save_changes()
                 }
             }
-            class L extends a.DOMWidgetModel {
+            class V extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: L.model_name,
-                        _view_name: L.view_name,
-                        _model_module: L.model_module,
-                        _view_module: L.view_module,
-                        _model_module_version: L.model_module_version,
-                        _view_module_version: L.view_module_version,
+                        _model_name: V.model_name,
+                        _view_name: V.view_name,
+                        _model_module: V.model_module,
+                        _view_module: V.view_module,
+                        _model_module_version: V.model_module_version,
+                        _view_module_version: V.view_module_version,
                         dataRecords: [],
                         x: String,
                         y: String,
                         hue: String,
                         elementId: String,
                         clickedValue: String,
                         selectedValuesRecords: []
                     }
                 }
-                static model_name = "ScatterplotModel";
-                static model_module = b.name;
-                static model_module_version = b.version;
-                static view_name = "ScatterplotView";
-                static view_module = b.name;
-                static view_module_version = b.version
+                static model_name = "ScatterPlotModel";
+                static model_module = w.name;
+                static model_module_version = w.version;
+                static view_name = "ScatterPlotView";
+                static view_module = w.name;
+                static view_module_version = w.version
             }
             class A extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:dataRecords", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:y", (() => k(this)), this), this.model.on("change:hue", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:x", (() => L(this)), this), this.model.on("change:y", (() => L(this)), this), this.model.on("change:hue", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
                         a = this.model.get("hue"),
                         i = this.model.get("elementId");
-                    let o = y,
+                    let o = k,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight);
                     let r = s.clientWidth;
-                    const l = w;
+                    const l = M;
                     ! function(e, t, n, a, i, o, s, r, l, d) {
                         const c = r - d.left - d.right,
                             m = l - d.top - d.bottom;
                         for (let t = 0; t < e.length; t++) e[t].id = t;
                         const u = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
                         _.select(i).selectAll("*").remove();
                         const p = _.scaleLinear().range([0, c]),
                             h = _.scaleLinear().range([m, 0]),
                             g = _.scaleOrdinal(_.schemeCategory10),
-                            v = _.axisBottom(p),
-                            f = _.axisLeft(h),
+                            f = _.axisBottom(p),
+                            v = _.axisLeft(h),
                             x = _.select(i).append("svg").attr("width", r).attr("height", l).append("g").attr("transform", "translate(" + d.left + "," + d.top + ")");
-                        p.domain(_.extent(e, (function(e) {
+                        if (p.domain(_.extent(e, (function(e) {
                                 return e[t]
                             }))).nice(), h.domain(_.extent(e, (function(e) {
                                 return e[n]
-                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + m + ")").call(v).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(f).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
+                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + m + ")").call(f).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
                                 return "dot-" + u + e.id
                             })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
                                 return p(e[t])
                             })).attr("cy", (function(e) {
                                 return h(e[n])
                             })).style("fill", (function(e) {
                                 return g(e[a])
                             })).on("mouseover", (function(e, a) {
-                                y.style("opacity", 1), w.style("opacity", 1), y.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                                b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
                             })).on("mouseout", (function() {
-                                y.style("opacity", 0), w.style("opacity", 0)
+                                b.style("opacity", 0), w.style("opacity", 0)
                             })).on("click", (function(e, a) {
                                 const i = "x:" + Math.round(10 * a[t]) / 10 + "    y:" + Math.round(10 * a[n]) / 10;
                                 void 0 !== o && o(i)
-                            })),
-                            function(e, t, n, a, i, o, s, r, l, d) {
-                                let c = [];
-                                const m = _.line(),
-                                    u = _.select(e).selectAll(".dot"),
-                                    p = _.drag().on("start", (function() {
-                                        c = [], r(), _.select(e).select("svg").append("path").attr("id", "lasso" + d)
-                                    })).on("drag", (function(e) {
-                                        let t = e.sourceEvent.offsetX,
-                                            n = e.sourceEvent.offsetY;
-                                        c.push([t, n]), _.select("#lasso" + d).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", m(c))
-                                    })).on("end", (function() {
-                                        let e = [];
-                                        u.each(((r, l) => {
-                                            (function(e, t) {
-                                                for (var n = e[0], a = e[1], i = !1, o = 0, s = t.length - 1; o < t.length; s = o++) {
-                                                    var r = t[o][0],
-                                                        l = t[o][1],
-                                                        d = t[s][0],
-                                                        c = t[s][1];
-                                                    l > a != c > a && n < (d - r) * (a - l) / (c - l) + r && (i = !i)
-                                                }
-                                                return i
-                                            })([t(r[a]) + o, n(r[i]) + s], c) && (_.select("#dot-" + d + r.id).style("fill", "red").attr("r", 6), e.push(r))
-                                        })), _.select("#lasso" + d).remove(), l(e)
-                                    }));
-                                _.select(e).call(p)
-                            }(i, p, h, t, n, d.left, d.top, (function() {
+                            })), y(i, p, h, t, n, d.left, d.top, (function() {
                                 x.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
                                     return g(e[a])
                                 }))
                             }), (function(e) {
                                 void 0 !== s && s(e)
-                            }), u);
-                        const b = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
-                            return "translate(0," + 20 * t + ")"
-                        }));
-                        b.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", g), b.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
-                            return e
-                        }));
-                        const y = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                            }), u), a) {
+                            const e = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                                return "translate(0," + 20 * t + ")"
+                            }));
+                            e.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", g), e.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                                return e
+                            }))
+                        }
+                        const b = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
                             w = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
                     }(e, t, n, a, s, this.setValue.bind(this), this.setSelectedValues.bind(this), r, o, l)
                 }
                 setValue(e) {
                     this.model.set({
                         clickedValue: e
                     }), this.model.save_changes()
                 }
                 setSelectedValues(e) {
                     this.model.set({
                         selectedValuesRecords: e
                     }), this.model.save_changes()
                 }
             }
-            class S extends a.DOMWidgetModel {
+            class D extends a.DOMWidgetModel {
+                defaults() {
+                    return {
+                        ...super.defaults(),
+                        _model_name: D.model_name,
+                        _view_name: D.view_name,
+                        _model_module: D.model_module,
+                        _view_module: D.view_module,
+                        _model_module_version: D.model_module_version,
+                        _view_module_version: D.view_module_version,
+                        dataRecords: [],
+                        x: String,
+                        y: String,
+                        hue: String,
+                        elementId: String,
+                        clickedValue: String,
+                        selectedValuesRecords: []
+                    }
+                }
+                static model_name = "LinearPlotModel";
+                static model_module = w.name;
+                static model_module_version = w.version;
+                static view_name = "LinearPlotView";
+                static view_module = w.name;
+                static view_module_version = w.version
+            }
+            class O extends a.DOMWidgetView {
+                timeout;
+                render() {
+                    L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:x", (() => L(this)), this), this.model.on("change:y", (() => L(this)), this), this.model.on("change:hue", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
+                }
+                plot() {
+                    const e = this.model.get("dataRecords"),
+                        t = this.model.get("x"),
+                        n = this.model.get("y"),
+                        a = this.model.get("hue"),
+                        i = this.model.get("elementId");
+                    let o = k,
+                        s = this.el;
+                    i && (s = document.getElementById(i), o = s.clientHeight);
+                    let r = s.clientWidth;
+                    const l = M;
+                    ! function(e, t, n, a, i, o, s, r, l, d) {
+                        const c = r - d.left - d.right,
+                            m = l - d.top - d.bottom;
+                        e = function(e, t, n, a) {
+                            function i(e) {
+                                const i = e.reduce((function(e, i) {
+                                        if (!e[i[t]]) {
+                                            const o = {};
+                                            return o[t] = i[t], o[n] = i[n], a && (o[a] = i[a]), o.count = 1, e[i[t]] = o, e
+                                        }
+                                        return e[i[t]][n] += i[n], e[i[t]].count += 1, e
+                                    }), {}),
+                                    o = Object.keys(i).map((function(e) {
+                                        const t = i[e],
+                                            a = {};
+                                        return a[n] = t[n] / t.count, {
+                                            ...t,
+                                            ...a
+                                        }
+                                    }));
+                                return o.sort((r = 1, "-" === (s = t)[0] && (r = -1, s = s.substr(1)), function(e, t) {
+                                    return (e[s] < t[s] ? -1 : e[s] > t[s] ? 1 : 0) * r
+                                })), o;
+                                var s, r
+                            }
+                            if (!a) return i(e);
+                            let o = b(e, a),
+                                s = [];
+                            return Object.values(o).forEach((function(e, t) {
+                                const n = i(e);
+                                s = s.concat(n)
+                            })), s
+                        }(e, t, [n], a);
+                        for (let t = 0; t < e.length; t++) e[t].id = t;
+                        const u = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                        _.select(i).selectAll("*").remove();
+                        const p = _.scaleLinear().range([0, c]),
+                            h = _.scaleLinear().range([m, 0]),
+                            g = _.scaleOrdinal(_.schemeCategory10),
+                            f = _.axisBottom(p),
+                            v = _.axisLeft(h),
+                            x = _.select(i).append("svg").attr("width", r).attr("height", l).append("g").attr("transform", "translate(" + d.left + "," + d.top + ")");
+
+                        function w(e, a) {
+                            x.append("path").datum(e).attr("fill", "none").attr("stroke", g(a)).attr("stroke-width", 2).attr("d", _.line().x((e => p(e[t]))).y((e => h(e[n]))))
+                        }
+                        if (p.domain(_.extent(e, (function(e) {
+                                return e[t]
+                            }))).nice(), h.domain(_.extent(e, (function(e) {
+                                return e[n]
+                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + m + ")").call(f).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), a) {
+                            const t = b(e, a);
+                            Object.keys(t).forEach((function(e, n) {
+                                w(t[e], e)
+                            }))
+                        } else w(e);
+                        if (x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
+                                return "dot-" + u + e.id
+                            })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
+                                return p(e[t])
+                            })).attr("cy", (function(e) {
+                                return h(e[n])
+                            })).style("fill", (function(e) {
+                                return g(e[a])
+                            })).on("mouseover", (function(e, a) {
+                                k.style("opacity", 1), M.style("opacity", 1), k.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), M.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                            })).on("mouseout", (function() {
+                                k.style("opacity", 0), M.style("opacity", 0)
+                            })).on("click", (function(e, a) {
+                                const i = "x:" + Math.round(10 * a[t]) / 10 + "    y:" + Math.round(10 * a[n]) / 10;
+                                void 0 !== o && o(i)
+                            })), y(i, p, h, t, n, d.left, d.top, (function() {
+                                x.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
+                                    return g(e[a])
+                                }))
+                            }), (function(e) {
+                                void 0 !== s && s(e)
+                            }), u), a) {
+                            const e = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                                return "translate(0," + 20 * t + ")"
+                            }));
+                            e.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", g), e.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                                return e
+                            }))
+                        }
+                        const k = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                            M = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
+                    }(e, t, n, a, s, this.setValue.bind(this), this.setSelectedValues.bind(this), r, o, l)
+                }
+                setValue(e) {
+                    this.model.set({
+                        clickedValue: e
+                    }), this.model.save_changes()
+                }
+                setSelectedValues(e) {
+                    this.model.set({
+                        selectedValuesRecords: e
+                    }), this.model.save_changes()
+                }
+            }
+            class j extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: S.model_name,
-                        _view_name: S.view_name,
-                        _model_module: S.model_module,
-                        _view_module: S.view_module,
-                        _model_module_version: S.model_module_version,
-                        _view_module_version: S.view_module_version,
+                        _model_name: j.model_name,
+                        _view_name: j.view_name,
+                        _model_module: j.model_module,
+                        _view_module: j.view_module,
+                        _model_module_version: j.model_module_version,
+                        _view_module_version: j.view_module_version,
                         dataRecords: [],
                         x: String,
                         y: String,
                         hue: String,
                         elementId: String
                     }
                 }
                 static model_name = "BarplotModel";
-                static model_module = b.name;
-                static model_module_version = b.version;
+                static model_module = w.name;
+                static model_module_version = w.version;
                 static view_name = "BarplotView";
-                static view_module = b.name;
-                static view_module_version = b.version
+                static view_module = w.name;
+                static view_module_version = w.version
             }
-            class V extends a.DOMWidgetView {
+            class C extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:dataRecords", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:y", (() => k(this)), this), this.model.on("change:hue", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:x", (() => L(this)), this), this.model.on("change:y", (() => L(this)), this), this.model.on("change:hue", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
                         a = this.model.get("hue"),
                         i = this.model.get("elementId");
-                    let o = y,
+                    let o = k,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight),
                         function(e, t, n, a, i, o, s, r) {
                             const l = o - r.left - r.right,
                                 d = s - r.top - r.bottom;
                             _.select(i).selectAll("*").remove();
                             const c = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
@@ -416,147 +571,147 @@
                                 Object.keys(u).map((e => {
                                     m.forEach((t => r.push(u[e][t])))
                                 }));
                                 const h = [];
                                 h.push(_.min(r, (e => e.min))), h.push(_.max(r, (e => e.max))), h[0] > 0 && h[1] > 0 ? h[0] = 0 : h[0] < 0 && h[1] < 0 && (h[1] = 0);
                                 const g = _.scaleLinear().domain(h).range([d, 0]);
                                 c.append("g").call(_.axisLeft(g));
-                                const v = _.scaleBand().domain(s).range([0, l]).padding([.2]),
-                                    f = _.scaleBand().domain(o).range([0, v.bandwidth()]).padding([.05]);
+                                const f = _.scaleBand().domain(s).range([0, l]).padding([.2]),
+                                    v = _.scaleBand().domain(o).range([0, f.bandwidth()]).padding([.05]);
                                 c.append("g").selectAll("g").data(i).enter().append("g").attr("transform", (function(e) {
-                                    return "translate(" + v(e[t]) + ",0)"
+                                    return "translate(" + f(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
                                     return o.map((function(t) {
                                         return {
                                             key: t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
-                                    return f(e.key)
+                                    return v(e.key)
                                 })).attr("y", (function(e) {
                                     return g(e.value) < g(0) ? g(e.value) : g(0)
-                                })).attr("width", f.bandwidth()).attr("height", (function(e) {
+                                })).attr("width", v.bandwidth()).attr("height", (function(e) {
                                     return Math.abs(g(0) - g(e.value))
                                 })).data(m).attr("fill", (function(e) {
                                     return p(e)
                                 }));
-                                const b = Object.keys(u).map((e => {
+                                const y = Object.keys(u).map((e => {
                                     let n = {};
                                     return n[t] = e, n = {
                                         ...n,
                                         ...u[e]
                                     }, n
                                 }));
-                                c.append("g").selectAll("g").data(b).enter().append("g").attr("transform", (function(e) {
-                                    return "translate(" + v(e[t]) + ",0)"
+                                c.append("g").selectAll("g").data(y).enter().append("g").attr("transform", (function(e) {
+                                    return "translate(" + f(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
                                     return m.map((function(t) {
                                         return {
                                             key: n + "-" + t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
-                                    return f(e.key) + f.bandwidth() / 2 - 1
+                                    return v(e.key) + v.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
                                     return e.value.max ? g(e.value.max) : 0
                                 })).attr("width", 2).attr("height", (function(e) {
                                     return e.value.min && e.value.max ? g(e.value.min) - g(e.value.max) : 0
                                 }));
-                                const y = c.selectAll(".legend").data(p.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                                const b = c.selectAll(".legend").data(p.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
                                     return "translate(0," + 20 * t + ")"
                                 }));
-                                y.append("rect").attr("x", l - 18).attr("width", 18).attr("height", 18).style("fill", p), y.append("text").attr("x", l - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                                b.append("rect").attr("x", l - 18).attr("width", 18).attr("height", 18).style("fill", p), b.append("text").attr("x", l - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
                                     return e
-                                })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + g(0) + ")").call(_.axisBottom(v).tickSize(0))
+                                })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + g(0) + ")").call(_.axisBottom(f).tickSize(0))
                             }()
-                        }(e, t, n, a, s, s.clientWidth, o, w)
+                        }(e, t, n, a, s, s.clientWidth, o, M)
                 }
             }
-            class D extends a.DOMWidgetModel {
+            class R extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: D.model_name,
-                        _view_name: D.view_name,
-                        _model_module: D.model_module,
-                        _view_module: D.view_module,
-                        _model_module_version: D.model_module_version,
-                        _view_module_version: D.view_module_version,
+                        _model_name: R.model_name,
+                        _view_name: R.view_name,
+                        _model_module: R.model_module,
+                        _view_module: R.view_module,
+                        _model_module_version: R.model_module_version,
+                        _view_module_version: R.view_module_version,
                         dataRecords: [],
                         x: String,
                         start: Number,
                         end: Number,
                         elementId: String
                     }
                 }
                 static model_name = "HistogramplotModel";
-                static model_module = b.name;
-                static model_module_version = b.version;
+                static model_module = w.name;
+                static model_module_version = w.version;
                 static view_name = "HistogramplotView";
-                static view_module = b.name;
-                static view_module_version = b.version
+                static view_module = w.name;
+                static view_module_version = w.version
             }
-            class j extends a.DOMWidgetView {
+            class I extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:dataRecords", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:start", (() => k(this)), this), this.model.on("change:end", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:x", (() => L(this)), this), this.model.on("change:start", (() => L(this)), this), this.model.on("change:end", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("x"),
                         n = this.model.get("start"),
                         a = this.model.get("end"),
                         i = this.model.get("elementId");
-                    let o = y,
+                    let o = k,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight),
                         function(e, t, n, a, i, o, s, r) {
                             const l = o - r.left - r.right,
                                 d = s - r.top - r.bottom;
                             _.select(i).selectAll("*").remove();
                             let c = n;
                             n || (c = _.min(e, (e => e[t])));
                             let m = a;
                             a || (m = _.max(e, (e => e[t])));
                             const u = _.scaleLinear().range([0, l]),
                                 p = _.scaleLinear().range([d, 0]),
                                 h = _.axisBottom(u),
                                 g = _.axisLeft(p),
-                                v = _.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
-                                f = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
-                            u.domain([c, m]), p.domain([0, _.max(v, (e => e.length))]), f.append("g").attr("transform", "translate(0," + d + ")").call(h).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), f.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), f.append("g").attr("fill", "steelblue").selectAll().data(v).join("rect").attr("x", (e => u(e.x0) + 1)).attr("width", (e => u(e.x1) - u(e.x0) - 1)).attr("y", (e => p(e.length))).attr("height", (e => p(0) - p(e.length)))
-                        }(e, t, n, a, s, s.clientWidth, o, w)
+                                f = _.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
+                                v = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
+                            u.domain([c, m]), p.domain([0, _.max(f, (e => e.length))]), v.append("g").attr("transform", "translate(0," + d + ")").call(h).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), v.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), v.append("g").attr("fill", "steelblue").selectAll().data(f).join("rect").attr("x", (e => u(e.x0) + 1)).attr("width", (e => u(e.x1) - u(e.x0) - 1)).attr("y", (e => p(e.length))).attr("height", (e => p(0) - p(e.length)))
+                        }(e, t, n, a, s, s.clientWidth, o, M)
                 }
             }
-            class C extends a.DOMWidgetModel {
+            class B extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: C.model_name,
-                        _view_name: C.view_name,
-                        _model_module: C.model_module,
-                        _view_module: C.view_module,
-                        _model_module_version: C.model_module_version,
-                        _view_module_version: C.view_module_version,
+                        _model_name: B.model_name,
+                        _view_name: B.view_name,
+                        _model_module: B.model_module,
+                        _view_module: B.view_module,
+                        _model_module_version: B.model_module_version,
+                        _view_module_version: B.view_module_version,
                         matrix: [],
                         grid_areas: [],
                         grid_template_areas: String,
                         style: String
                     }
                 }
                 static model_name = "EmbeddingModel";
-                static model_module = b.name;
-                static model_module_version = b.version;
+                static model_module = w.name;
+                static model_module_version = w.version;
                 static view_name = "EmbeddingView";
-                static view_module = b.name;
-                static view_module_version = b.version
+                static view_module = w.name;
+                static view_module_version = w.version
             }
-            class O extends a.DOMWidgetView {
+            class W extends a.DOMWidgetView {
                 render() {
                     this.value_changed()
                 }
                 value_changed() {
                     const e = this.model.get("matrix"),
                         t = this.model.get("grid_areas"),
                         n = this.model.get("grid_template_areas");
@@ -565,55 +720,55 @@
                     const i = document.createElement("div");
                     i.classList.add(a), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + e.length + ", 180px)", i.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", i.style.width = "100%", t.forEach((e => {
                         const t = document.createElement("div");
                         t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), i.appendChild(t)
                     })), this.el.appendChild(i)
                 }
             }
-            class I extends a.DOMWidgetModel {
+            class P extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: I.model_name,
-                        _view_name: I.view_name,
-                        _model_module: I.model_module,
-                        _view_module: I.view_module,
-                        _model_module_version: I.model_module_version,
-                        _view_module_version: I.view_module_version,
+                        _model_name: P.model_name,
+                        _view_name: P.view_name,
+                        _model_module: P.model_module,
+                        _view_module: P.view_module,
+                        _model_module_version: P.model_module_version,
+                        _view_module_version: P.view_module_version,
                         dataRecords: [],
                         variable: String,
                         step: Number,
                         description: String,
                         minValue: Number,
                         maxValue: Number,
                         elementId: String
                     }
                 }
                 static model_name = "RangeSliderModel";
-                static model_module = b.name;
-                static model_module_version = b.version;
+                static model_module = w.name;
+                static model_module_version = w.version;
                 static view_name = "RangeSliderView";
-                static view_module = b.name;
-                static view_module_version = b.version
+                static view_module = w.name;
+                static view_module_version = w.version
             }
-            class R extends a.DOMWidgetView {
+            class H extends a.DOMWidgetView {
                 render() {
-                    k(this), this.model.on("change:dataRecords", (() => k(this)), this), this.model.on("change:variable", (() => k(this)), this), this.model.on("change:step", (() => k(this)), this), this.model.on("change:description", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                    L(this), this.model.on("change:dataRecords", (() => L(this)), this), this.model.on("change:variable", (() => L(this)), this), this.model.on("change:step", (() => L(this)), this), this.model.on("change:description", (() => L(this)), this), window.addEventListener("resize", (() => L(this)))
                 }
                 plot() {
                     const e = this.model.get("dataRecords"),
                         t = this.model.get("variable"),
                         n = this.model.get("step"),
                         a = this.model.get("description"),
                         i = this.model.get("elementId"),
                         o = this.model.get("minValue"),
                         s = this.model.get("maxValue");
                     let r = this.el;
                     i && (r = document.getElementById(i));
-                    const l = w;
+                    const l = M;
                     ! function(e, t, n, a, i, o, s, r, l) {
                         const d = document.createElement("div");
                         d.classList.add("range_outside_container"), d.style.margin = l.top + "px " + l.right + "px " + l.bottom + "px " + l.left + "px";
                         const c = document.createElement("span");
                         c.classList.add("range_description"), c.textContent = a, d.appendChild(c);
                         const m = document.createElement("div");
                         m.classList.add("range_inside_container"), d.appendChild(m);
@@ -621,28 +776,28 @@
                         u.classList.add("range_value"), d.appendChild(u);
                         const p = document.createElement("div");
                         p.classList.add("sliders_control"), m.appendChild(p);
                         const h = document.createElement("input");
                         h.classList.add("top_slider"), h.setAttribute("step", n), h.setAttribute("type", "range"), p.appendChild(h);
                         const g = document.createElement("input");
 
-                        function v(e, t) {
+                        function f(e, t) {
                             u.textContent = e + " - " + t, s(e, t)
                         }
                         g.setAttribute("step", n), g.setAttribute("type", "range"), p.appendChild(g);
-                        const f = _.min(e, (e => e[t])),
+                        const v = _.min(e, (e => e[t])),
                             x = _.max(e, (e => e[t]));
-                        h.setAttribute("min", f), h.setAttribute("max", x), g.setAttribute("min", f), g.setAttribute("max", x), i && o ? (h.value = i, g.value = o) : (h.value = f, g.value = x), v(parseFloat(h.value), parseFloat(g.value)), h.addEventListener("input", (() => {
+                        h.setAttribute("min", v), h.setAttribute("max", x), g.setAttribute("min", v), g.setAttribute("max", x), i && o ? (h.value = i, g.value = o) : (h.value = v, g.value = x), f(parseFloat(h.value), parseFloat(g.value)), h.addEventListener("input", (() => {
                             const e = parseFloat(h.value),
                                 t = parseFloat(g.value);
-                            e > t && (h.value = g.value), v(e, t)
+                            e > t && (h.value = g.value), f(e, t)
                         })), g.addEventListener("input", (() => {
                             const e = parseFloat(h.value),
                                 t = parseFloat(g.value);
-                            t < e && (g.value = h.value), v(e, t)
+                            t < e && (g.value = h.value), f(e, t)
                         })), h.addEventListener("click", (() => {
                             h.classList.add("top_slider"), g.classList.remove("top_slider")
                         })), g.addEventListener("click", (() => {
                             g.classList.add("top_slider"), h.classList.remove("top_slider")
                         })), r.innerHTML = "", r.appendChild(d)
                     }(e, t, n, a, o, s, this.setValues.bind(this), r, l)
                 }
@@ -650,15 +805,15 @@
                     this.model.set({
                         minValue: e
                     }), this.model.set({
                         maxValue: t
                     }), this.model.save_changes()
                 }
             }
-            var B = n(330)
+            var T = n(330)
         },
         930: (e, t, n) => {
             n.d(t, {
                 A: () => r
             });
             var a = n(601),
                 i = n.n(a),
@@ -828,11 +983,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.1","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js` & `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/493.9def85d738cd0e72c5f5.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,39 +1,41 @@
 "use strict";
 (self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || []).push([
     [493], {
         493: (e, i, t) => {
             t.r(i), t.d(i, {
-                default: () => r,
-                helloWidgetPlugin: () => d
+                default: () => d,
+                helloWidgetPlugin: () => r
             });
             var l = t(801),
-                o = t(363);
-            const d = {
+                o = t(112);
+            const r = {
                     id: "d3vis_ipynb:plugin",
                     requires: [l.IJupyterWidgetRegistry],
                     activate: function(e, i) {
                         i.registerWidget({
                             name: "d3vis_ipynb",
                             version: o.version,
                             exports: {
                                 LinearHistPlotModel: o.LinearHistPlotModel,
                                 LinearHistPlotView: o.LinearHistPlotView,
                                 ScatterPlotModel: o.ScatterPlotModel,
                                 ScatterPlotView: o.ScatterPlotView,
+                                LinearPlotModel: o.LinearPlotModel,
+                                LinearPlotView: o.LinearPlotView,
                                 BarPlotModel: o.BarPlotModel,
                                 BarPlotView: o.BarPlotView,
                                 HistogramPlotModel: o.HistogramPlotModel,
                                 HistogramPlotView: o.HistogramPlotView,
                                 EmbeddingModel: o.EmbeddingModel,
                                 EmbeddingView: o.EmbeddingView,
                                 RangeSliderModel: o.RangeSliderModel,
                                 RangeSliderView: o.RangeSliderView
                             }
                         })
                     },
                     autoStart: !0
                 },
-                r = d
+                d = r
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js` & `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/remoteEntry.065ac4641043ad457b9a.js` & `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/remoteEntry.6f9edec5dc6ff6501b02.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, d, s, l, f, p, c, h, v, b, g, m, y, w = {
+    var e, r, t, n, o, a, i, u, s, l, d, f, p, c, h, v, g, b, m, y, w = {
             772: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(363).then((() => () => t(363))),
-                        "./extension": () => Promise.all([t.e(363), t.e(493)]).then((() => () => t(493)))
+                        "./index": () => t.e(112).then((() => () => t(112))),
+                        "./extension": () => Promise.all([t.e(112), t.e(493)]).then((() => () => t(493)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    i = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
                                 o = t.S[n];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => i
+                    init: () => a
                 })
             }
         },
         S = {};
 
     function E(e) {
         var r = S[e];
@@ -42,51 +42,51 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        363: "d2d286fd78e0907ef3c1",
-        493: "053b071a46f0bcccaab9",
+        112: "a36093df8a8075509d10",
+        493: "9def85d738cd0e72c5f5",
         693: "c8409ce8329f6703470f"
     } [e] + ".js?v=" + {
-        363: "d2d286fd78e0907ef3c1",
-        493: "053b071a46f0bcccaab9",
+        112: "a36093df8a8075509d10",
+        493: "9def85d738cd0e72c5f5",
         693: "c8409ce8329f6703470f"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, i) => {
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, u;
+            var i, u;
             if (void 0 !== o)
-                for (var d = document.getElementsByTagName("script"), s = 0; s < d.length; s++) {
-                    var l = d[s];
-                    if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + o) {
-                        a = l;
+                for (var s = document.getElementsByTagName("script"), l = 0; l < s.length; l++) {
+                    var d = s[l];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
-            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
-                    target: a
+                    target: i
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), u && document.head.appendChild(a)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -96,27 +96,27 @@
             r = {};
         E.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
-                var i = E.S[t],
-                    a = "d3vis_ipynb",
+                var a = E.S[t],
+                    i = "d3vis_ipynb",
                     u = (e, r, t, n) => {
-                        var o = i[e] = i[e] || {},
+                        var o = a[e] = a[e] || {},
                             u = o[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
-                            from: a,
+                            from: i,
                             eager: !!n
                         })
                     },
-                    d = [];
-                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.2.1", (() => E.e(363).then((() => () => E(363)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                    s = [];
+                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.2.2", (() => E.e(112).then((() => () => E(112)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -132,125 +132,125 @@
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
-                i = (typeof o)[0];
-            if (n >= r.length) return "u" == i;
-            var a = r[n],
-                u = (typeof a)[0];
-            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
-            if ("o" != i && "u" != i && o != a) return o < a;
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
+            var i = r[n],
+                u = (typeof i)[0];
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
-        var a = [];
-        for (i = 1; i < e.length; i++) {
-            var u = e[i];
-            a.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
+        var i = [];
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + s() + ")" : 1 === u ? "(" + s() + " || " + s() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return d();
+        return s();
 
-        function d() {
-            return a.pop().replace(/^\((.+)\)$/, "$1")
+        function s() {
+            return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, i = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, u = 1, d = !0;; u++, a++) {
-                var s, l, f = u < e.length ? (typeof e[u])[0] : "";
-                if (a >= r.length || "o" == (l = (typeof(s = r[a]))[0])) return !d || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == l) {
-                    if (!d || "u" != f) return !1
-                } else if (d)
-                    if (f == l)
+            for (var i = 0, u = 1, s = !0;; u++, i++) {
+                var l, d, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(l = r[i]))[0])) return !s || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == d) {
+                    if (!s || "u" != f) return !1
+                } else if (s)
+                    if (f == d)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (d = !1)
+                            if (o ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (s = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
-                    d = !1, u--
+                    s = !1, u--
                 } else {
-                    if (u <= n || l < f != o) return !1;
-                    d = !1
-                } else "s" != f && "n" != f && (d = !1, u--)
+                    if (u <= n || d < f != o) return !1;
+                    s = !1
+                } else "s" != f && "n" != f && (s = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
-        for (a = 1; a < e.length; a++) {
-            var h = e[a];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+        for (i = 1; i < e.length; i++) {
+            var h = e[i];
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
-    }, a = (e, r) => {
+    }, i = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return i(n, o) || f(d(e, t, o, n)), p(e[t][o])
-    }, l = (e, r, t) => {
+        return a(n, o) || f(s(e, t, o, n)), p(e[t][o])
+    }, d = (e, r, t) => {
         var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
-        var i = E.I(r);
-        return i && i.then ? i.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
-        var i = r && E.o(r, t) && l(r, t, n);
-        return i ? p(i) : o()
-    })), b = {}, g = {
+        var a = E.I(r);
+        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
+        var a = r && E.o(r, t) && d(r, t, n);
+        return a ? p(a) : o()
+    })), g = {}, b = {
         801: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
         840: () => v("default", "d3", [1, 7, 9, 0], (() => E.e(693).then((() => () => E(693)))))
     }, m = {
-        363: [801, 840]
+        112: [801, 840]
     }, y = {}, E.f.consumes = (e, r) => {
         E.o(m, e) && m[e].forEach((e => {
-            if (E.o(b, e)) return r.push(b[e]);
+            if (E.o(g, e)) return r.push(g[e]);
             if (!y[e]) {
                 var t = r => {
-                    b[e] = 0, E.m[e] = t => {
+                    g[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
                 var n = r => {
-                    delete b[e], E.m[e] = t => {
+                    delete g[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
                 try {
-                    var o = g[e]();
-                    o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                    var o = b[e]();
+                    o.then ? r.push(g[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
@@ -259,33 +259,33 @@
         E.f.j = (r, t) => {
             var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var i = E.p + E.u(r),
-                        a = new Error;
-                    E.l(i, (t => {
+                    var a = E.p + E.u(r),
+                        i = new Error;
+                    E.l(a, (t => {
                         if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
-                                i = t && t.target && t.target.src;
-                            a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [i, a, u] = t,
-                    d = 0;
-                if (i.some((r => 0 !== e[r]))) {
-                    for (n in a) E.o(a, n) && (E.m[n] = a[n]);
+                var n, o, [a, i, u] = t,
+                    s = 0;
+                if (a.some((r => 0 !== e[r]))) {
+                    for (n in i) E.o(i, n) && (E.m[n] = i[n]);
                     u && u(E)
                 }
-                for (r && r(t); d < i.length; d++) o = i[d], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); s < a.length; s++) o = a[s], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var P = E(772);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).d3vis_ipynb = P
 })();
```

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/labextension/static/third-party-licenses.json` & `d3vis_ipynb-0.2.2/d3vis_ipynb/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/d3vis_ipynb/nbextension/index.js` & `d3vis_ipynb-0.2.2/d3vis_ipynb/nbextension/index.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -57,25 +57,25 @@
                 function r(t, r) {
                     for (var o = {}, a = [], s = 0; s < t.length; s++) {
                         var l = t[s],
                             u = r.base ? l[0] + r.base : l[0],
                             c = o[u] || 0,
                             h = "".concat(u, " ").concat(c);
                         o[u] = c + 1;
-                        var f = n(h),
-                            d = {
+                        var d = n(h),
+                            f = {
                                 css: l[1],
                                 media: l[2],
                                 sourceMap: l[3],
                                 supports: l[4],
                                 layer: l[5]
                             };
-                        if (-1 !== f) e[f].references++, e[f].updater(d);
+                        if (-1 !== d) e[d].references++, e[d].updater(f);
                         else {
-                            var p = i(d, r);
+                            var p = i(f, r);
                             r.byIndex = s, e.splice(s, 0, {
                                 identifier: h,
                                 updater: p,
                                 references: 1
                             })
                         }
                         a.push(h)
@@ -179,15 +179,15 @@
             55: t => {
                 t.exports = e
             },
             308: e => {
                 e.exports = t
             },
             330: t => {
-                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.1","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.2.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
@@ -217,67 +217,69 @@
     var o = {};
     return (() => {
         var t = i(308);
         const e = new URL(t.uri, document.location);
         e.pathname = e.pathname.slice(0, e.pathname.lastIndexOf("/") + 1), i.p = `${e.origin}${e.pathname}`
     })(), (() => {
         i.r(o), i.d(o, {
-            BarPlotModel: () => Vi,
-            BarPlotView: () => Li,
-            EmbeddingModel: () => Ri,
-            EmbeddingView: () => qi,
-            HistogramPlotModel: () => Di,
-            HistogramPlotView: () => Ii,
-            LinearHistPlotModel: () => Ti,
-            LinearHistPlotView: () => ji,
-            RangeSliderModel: () => Hi,
-            RangeSliderView: () => zi,
-            ScatterPlotModel: () => Oi,
-            ScatterPlotView: () => Pi,
-            author: () => Xi.author,
-            dependencies: () => Xi.dependencies,
-            description: () => Xi.description,
-            devDependencies: () => Xi.devDependencies,
-            files: () => Xi.files,
-            jupyterlab: () => Xi.jupyterlab,
-            keywords: () => Xi.keywords,
-            license: () => Xi.license,
-            main: () => Xi.main,
-            name: () => Xi.name,
-            repository: () => Xi.repository,
-            scripts: () => Xi.scripts,
-            version: () => Xi.version
+            BarPlotModel: () => Ri,
+            BarPlotView: () => Ii,
+            EmbeddingModel: () => zi,
+            EmbeddingView: () => Xi,
+            HistogramPlotModel: () => qi,
+            HistogramPlotView: () => Hi,
+            LinearHistPlotModel: () => Ci,
+            LinearHistPlotView: () => Ti,
+            LinearPlotModel: () => Li,
+            LinearPlotView: () => Di,
+            RangeSliderModel: () => Yi,
+            RangeSliderView: () => Bi,
+            ScatterPlotModel: () => Pi,
+            ScatterPlotView: () => Oi,
+            author: () => Fi.author,
+            dependencies: () => Fi.dependencies,
+            description: () => Fi.description,
+            devDependencies: () => Fi.devDependencies,
+            files: () => Fi.files,
+            jupyterlab: () => Fi.jupyterlab,
+            keywords: () => Fi.keywords,
+            license: () => Fi.license,
+            main: () => Fi.main,
+            name: () => Fi.name,
+            repository: () => Fi.repository,
+            scripts: () => Fi.scripts,
+            version: () => Fi.version
         });
         var t = i(55),
             e = i(72),
             n = i.n(e),
             r = i(825),
             a = i.n(r),
             s = i(659),
             l = i.n(s),
             u = i(56),
             c = i.n(u),
             h = i(540),
-            f = i.n(h),
-            d = i(113),
-            p = i.n(d),
+            d = i.n(h),
+            f = i(113),
+            p = i.n(f),
             m = i(930),
             _ = {};
 
         function g(t, e) {
             let n, r;
             if (void 0 === e)
                 for (const e of t) null != e && (void 0 === n ? e >= e && (n = r = e) : (n > e && (n = e), r < e && (r = e)));
             else {
                 let i = -1;
                 for (let o of t) null != (o = e(o, ++i, t)) && (void 0 === n ? o >= o && (n = r = o) : (n > o && (n = o), r < o && (r = o)))
             }
             return [n, r]
         }
-        _.styleTagTransform = p(), _.setAttributes = c(), _.insert = l().bind(null, "head"), _.domAPI = a(), _.insertStyleElement = f(), n()(m.A, _), m.A && m.A.locals && m.A.locals;
+        _.styleTagTransform = p(), _.setAttributes = c(), _.insert = l().bind(null, "head"), _.domAPI = a(), _.insertStyleElement = d(), n()(m.A, _), m.A && m.A.locals && m.A.locals;
         var v = Array.prototype,
             y = v.slice;
 
         function w(t, e) {
             return null == t || null == e ? NaN : t < e ? -1 : t > e ? 1 : t >= e ? 0 : NaN
         }
 
@@ -323,39 +325,39 @@
         v.map;
         const k = b(w),
             A = k.right,
             E = (k.left, b((function(t) {
                 return null === t ? NaN : +t
             })).center, A);
 
-        function N(t) {
+        function S(t) {
             return () => t
         }
 
-        function S(t) {
+        function N(t) {
             return t
         }
         const $ = Math.sqrt(50),
-            C = Math.sqrt(10),
-            T = Math.sqrt(2);
+            V = Math.sqrt(10),
+            j = Math.sqrt(2);
 
-        function j(t, e, n) {
+        function C(t, e, n) {
             const r = (e - t) / Math.max(0, n),
                 i = Math.floor(Math.log10(r)),
                 o = r / Math.pow(10, i),
-                a = o >= $ ? 10 : o >= C ? 5 : o >= T ? 2 : 1;
+                a = o >= $ ? 10 : o >= V ? 5 : o >= j ? 2 : 1;
             let s, l, u;
-            return i < 0 ? (u = Math.pow(10, -i) / a, s = Math.round(t * u), l = Math.round(e * u), s / u < t && ++s, l / u > e && --l, u = -u) : (u = Math.pow(10, i) * a, s = Math.round(t / u), l = Math.round(e / u), s * u < t && ++s, l * u > e && --l), l < s && .5 <= n && n < 2 ? j(t, e, 2 * n) : [s, l, u]
+            return i < 0 ? (u = Math.pow(10, -i) / a, s = Math.round(t * u), l = Math.round(e * u), s / u < t && ++s, l / u > e && --l, u = -u) : (u = Math.pow(10, i) * a, s = Math.round(t / u), l = Math.round(e / u), s * u < t && ++s, l * u > e && --l), l < s && .5 <= n && n < 2 ? C(t, e, 2 * n) : [s, l, u]
         }
 
-        function O(t, e, n) {
+        function T(t, e, n) {
             if (!((n = +n) > 0)) return [];
             if ((t = +t) == (e = +e)) return [t];
             const r = e < t,
-                [i, o, a] = r ? j(e, t, n) : j(t, e, n);
+                [i, o, a] = r ? C(e, t, n) : C(t, e, n);
             if (!(o >= i)) return [];
             const s = o - i + 1,
                 l = new Array(s);
             if (r)
                 if (a < 0)
                     for (let t = 0; t < s; ++t) l[t] = (o - t) / -a;
                 else
@@ -364,105 +366,105 @@
                 for (let t = 0; t < s; ++t) l[t] = (i + t) / -a;
             else
                 for (let t = 0; t < s; ++t) l[t] = (i + t) * a;
             return l
         }
 
         function P(t, e, n) {
-            return j(t = +t, e = +e, n = +n)[2]
+            return C(t = +t, e = +e, n = +n)[2]
         }
 
-        function V(t) {
+        function O(t) {
             return Math.max(1, Math.ceil(Math.log(function(t, e) {
                 let n = 0;
                 for (let e of t) null != e && (e = +e) >= e && ++n;
                 return n
             }(t)) / Math.LN2) + 1)
         }
 
         function L() {
-            var t = S,
+            var t = N,
                 e = g,
-                n = V;
+                n = O;
 
             function r(r) {
                 Array.isArray(r) || (r = Array.from(r));
                 var i, o, a, s = r.length,
                     l = new Array(s);
                 for (i = 0; i < s; ++i) l[i] = t(r[i], i, r);
                 var u = e(l),
                     c = u[0],
                     h = u[1],
-                    f = n(l, c, h);
-                if (!Array.isArray(f)) {
+                    d = n(l, c, h);
+                if (!Array.isArray(d)) {
                     const t = h,
-                        n = +f;
+                        n = +d;
                     if (e === g && ([c, h] = function(t, e, n) {
                             let r;
                             for (;;) {
                                 const i = P(t, e, n);
                                 if (i === r || 0 === i || !isFinite(i)) return [t, e];
                                 i > 0 ? (t = Math.floor(t / i) * i, e = Math.ceil(e / i) * i) : i < 0 && (t = Math.ceil(t * i) / i, e = Math.floor(e * i) / i), r = i
                             }
-                        }(c, h, n)), (f = O(c, h, n))[0] <= c && (a = P(c, h, n)), f[f.length - 1] >= h)
+                        }(c, h, n)), (d = T(c, h, n))[0] <= c && (a = P(c, h, n)), d[d.length - 1] >= h)
                         if (t >= h && e === g) {
                             const t = P(c, h, n);
                             isFinite(t) && (t > 0 ? h = (Math.floor(h / t) + 1) * t : t < 0 && (h = (Math.ceil(h * -t) + 1) / -t))
-                        } else f.pop()
+                        } else d.pop()
                 }
-                for (var d = f.length, p = 0, m = d; f[p] <= c;) ++p;
-                for (; f[m - 1] > h;) --m;
-                (p || m < d) && (f = f.slice(p, m), d = m - p);
-                var _, v = new Array(d + 1);
-                for (i = 0; i <= d; ++i)(_ = v[i] = []).x0 = i > 0 ? f[i - 1] : c, _.x1 = i < d ? f[i] : h;
+                for (var f = d.length, p = 0, m = f; d[p] <= c;) ++p;
+                for (; d[m - 1] > h;) --m;
+                (p || m < f) && (d = d.slice(p, m), f = m - p);
+                var _, v = new Array(f + 1);
+                for (i = 0; i <= f; ++i)(_ = v[i] = []).x0 = i > 0 ? d[i - 1] : c, _.x1 = i < f ? d[i] : h;
                 if (isFinite(a)) {
                     if (a > 0)
-                        for (i = 0; i < s; ++i) null != (o = l[i]) && c <= o && o <= h && v[Math.min(d, Math.floor((o - c) / a))].push(r[i]);
+                        for (i = 0; i < s; ++i) null != (o = l[i]) && c <= o && o <= h && v[Math.min(f, Math.floor((o - c) / a))].push(r[i]);
                     else if (a < 0)
                         for (i = 0; i < s; ++i)
                             if (null != (o = l[i]) && c <= o && o <= h) {
                                 const t = Math.floor((c - o) * a);
-                                v[Math.min(d, t + (f[t] <= o))].push(r[i])
+                                v[Math.min(f, t + (d[t] <= o))].push(r[i])
                             }
                 } else
-                    for (i = 0; i < s; ++i) null != (o = l[i]) && c <= o && o <= h && v[E(f, o, 0, d)].push(r[i]);
+                    for (i = 0; i < s; ++i) null != (o = l[i]) && c <= o && o <= h && v[E(d, o, 0, f)].push(r[i]);
                 return v
             }
             return r.value = function(e) {
-                return arguments.length ? (t = "function" == typeof e ? e : N(e), r) : t
+                return arguments.length ? (t = "function" == typeof e ? e : S(e), r) : t
             }, r.domain = function(t) {
-                return arguments.length ? (e = "function" == typeof t ? t : N([t[0], t[1]]), r) : e
+                return arguments.length ? (e = "function" == typeof t ? t : S([t[0], t[1]]), r) : e
             }, r.thresholds = function(t) {
-                return arguments.length ? (n = "function" == typeof t ? t : N(Array.isArray(t) ? y.call(t) : t), r) : n
+                return arguments.length ? (n = "function" == typeof t ? t : S(Array.isArray(t) ? y.call(t) : t), r) : n
             }, r
         }
 
         function D(t, e) {
             let n;
             if (void 0 === e)
                 for (const e of t) null != e && (n < e || void 0 === n && e >= e) && (n = e);
             else {
                 let r = -1;
                 for (let i of t) null != (i = e(i, ++r, t)) && (n < i || void 0 === n && i >= i) && (n = i)
             }
             return n
         }
 
-        function I(t, e) {
+        function R(t, e) {
             let n;
             if (void 0 === e)
                 for (const e of t) null != e && (n > e || void 0 === n && e >= e) && (n = e);
             else {
                 let r = -1;
                 for (let i of t) null != (i = e(i, ++r, t)) && (n > i || void 0 === n && i >= i) && (n = i)
             }
             return n
         }
 
-        function R(t) {
+        function I(t) {
             return t
         }
         var q = 1,
             H = 2,
             z = 3,
             X = 4,
             Y = 1e-6;
@@ -495,61 +497,61 @@
                 a = 6,
                 s = 3,
                 l = "undefined" != typeof window && window.devicePixelRatio > 1 ? 0 : .5,
                 u = t === q || t === X ? -1 : 1,
                 c = t === X || t === H ? "x" : "y",
                 h = t === q || t === z ? B : F;
 
-            function f(f) {
-                var d = null == r ? e.ticks ? e.ticks.apply(e, n) : e.domain() : r,
-                    p = null == i ? e.tickFormat ? e.tickFormat.apply(e, n) : R : i,
+            function d(d) {
+                var f = null == r ? e.ticks ? e.ticks.apply(e, n) : e.domain() : r,
+                    p = null == i ? e.tickFormat ? e.tickFormat.apply(e, n) : I : i,
                     m = Math.max(o, 0) + s,
                     _ = e.range(),
                     g = +_[0] + l,
                     v = +_[_.length - 1] + l,
                     y = (e.bandwidth ? U : W)(e.copy(), l),
-                    w = f.selection ? f.selection() : f,
+                    w = d.selection ? d.selection() : d,
                     x = w.selectAll(".domain").data([null]),
-                    b = w.selectAll(".tick").data(d, e).order(),
+                    b = w.selectAll(".tick").data(f, e).order(),
                     M = b.exit(),
                     k = b.enter().append("g").attr("class", "tick"),
                     A = b.select("line"),
                     E = b.select("text");
-                x = x.merge(x.enter().insert("path", ".tick").attr("class", "domain").attr("stroke", "currentColor")), b = b.merge(k), A = A.merge(k.append("line").attr("stroke", "currentColor").attr(c + "2", u * o)), E = E.merge(k.append("text").attr("fill", "currentColor").attr(c, u * m).attr("dy", t === q ? "0em" : t === z ? "0.71em" : "0.32em")), f !== w && (x = x.transition(f), b = b.transition(f), A = A.transition(f), E = E.transition(f), M = M.transition(f).attr("opacity", Y).attr("transform", (function(t) {
+                x = x.merge(x.enter().insert("path", ".tick").attr("class", "domain").attr("stroke", "currentColor")), b = b.merge(k), A = A.merge(k.append("line").attr("stroke", "currentColor").attr(c + "2", u * o)), E = E.merge(k.append("text").attr("fill", "currentColor").attr(c, u * m).attr("dy", t === q ? "0em" : t === z ? "0.71em" : "0.32em")), d !== w && (x = x.transition(d), b = b.transition(d), A = A.transition(d), E = E.transition(d), M = M.transition(d).attr("opacity", Y).attr("transform", (function(t) {
                     return isFinite(t = y(t)) ? h(t + l) : this.getAttribute("transform")
                 })), k.attr("opacity", Y).attr("transform", (function(t) {
                     var e = this.parentNode.__axis;
                     return h((e && isFinite(e = e(t)) ? e : y(t)) + l)
                 }))), M.remove(), x.attr("d", t === X || t === H ? a ? "M" + u * a + "," + g + "H" + l + "V" + v + "H" + u * a : "M" + l + "," + g + "V" + v : a ? "M" + g + "," + u * a + "V" + l + "H" + v + "V" + u * a : "M" + g + "," + l + "H" + v), b.attr("opacity", 1).attr("transform", (function(t) {
                     return h(y(t) + l)
                 })), A.attr(c + "2", u * o), E.attr(c, u * m).text(p), w.filter(G).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", t === H ? "start" : t === X ? "end" : "middle"), w.each((function() {
                     this.__axis = y
                 }))
             }
-            return f.scale = function(t) {
-                return arguments.length ? (e = t, f) : e
-            }, f.ticks = function() {
-                return n = Array.from(arguments), f
-            }, f.tickArguments = function(t) {
-                return arguments.length ? (n = null == t ? [] : Array.from(t), f) : n.slice()
-            }, f.tickValues = function(t) {
-                return arguments.length ? (r = null == t ? null : Array.from(t), f) : r && r.slice()
-            }, f.tickFormat = function(t) {
-                return arguments.length ? (i = t, f) : i
-            }, f.tickSize = function(t) {
-                return arguments.length ? (o = a = +t, f) : o
-            }, f.tickSizeInner = function(t) {
-                return arguments.length ? (o = +t, f) : o
-            }, f.tickSizeOuter = function(t) {
-                return arguments.length ? (a = +t, f) : a
-            }, f.tickPadding = function(t) {
-                return arguments.length ? (s = +t, f) : s
-            }, f.offset = function(t) {
-                return arguments.length ? (l = +t, f) : l
-            }, f
+            return d.scale = function(t) {
+                return arguments.length ? (e = t, d) : e
+            }, d.ticks = function() {
+                return n = Array.from(arguments), d
+            }, d.tickArguments = function(t) {
+                return arguments.length ? (n = null == t ? [] : Array.from(t), d) : n.slice()
+            }, d.tickValues = function(t) {
+                return arguments.length ? (r = null == t ? null : Array.from(t), d) : r && r.slice()
+            }, d.tickFormat = function(t) {
+                return arguments.length ? (i = t, d) : i
+            }, d.tickSize = function(t) {
+                return arguments.length ? (o = a = +t, d) : o
+            }, d.tickSizeInner = function(t) {
+                return arguments.length ? (o = +t, d) : o
+            }, d.tickSizeOuter = function(t) {
+                return arguments.length ? (a = +t, d) : a
+            }, d.tickPadding = function(t) {
+                return arguments.length ? (s = +t, d) : s
+            }, d.offset = function(t) {
+                return arguments.length ? (l = +t, d) : l
+            }, d
         }
 
         function Z(t) {
             return J(z, t)
         }
 
         function K(t) {
@@ -605,25 +607,25 @@
         }
 
         function ht(t, e, n, r, i, o) {
             for (var a, s = 0, l = e.length, u = o.length; s < u; ++s)(a = e[s]) ? (a.__data__ = o[s], r[s] = a) : n[s] = new ct(t, o[s]);
             for (; s < l; ++s)(a = e[s]) && (i[s] = a)
         }
 
-        function ft(t, e, n, r, i, o, a) {
+        function dt(t, e, n, r, i, o, a) {
             var s, l, u, c = new Map,
                 h = e.length,
-                f = o.length,
-                d = new Array(h);
-            for (s = 0; s < h; ++s)(l = e[s]) && (d[s] = u = a.call(l, l.__data__, s, e) + "", c.has(u) ? i[s] = l : c.set(u, l));
-            for (s = 0; s < f; ++s) u = a.call(t, o[s], s, o) + "", (l = c.get(u)) ? (r[s] = l, l.__data__ = o[s], c.delete(u)) : n[s] = new ct(t, o[s]);
-            for (s = 0; s < h; ++s)(l = e[s]) && c.get(d[s]) === l && (i[s] = l)
+                d = o.length,
+                f = new Array(h);
+            for (s = 0; s < h; ++s)(l = e[s]) && (f[s] = u = a.call(l, l.__data__, s, e) + "", c.has(u) ? i[s] = l : c.set(u, l));
+            for (s = 0; s < d; ++s) u = a.call(t, o[s], s, o) + "", (l = c.get(u)) ? (r[s] = l, l.__data__ = o[s], c.delete(u)) : n[s] = new ct(t, o[s]);
+            for (s = 0; s < h; ++s)(l = e[s]) && c.get(f[s]) === l && (i[s] = l)
         }
 
-        function dt(t) {
+        function ft(t) {
             return t.__data__
         }
 
         function pt(t) {
             return "object" == typeof t && "length" in t ? t : Array.from(t)
         }
 
@@ -707,77 +709,77 @@
 
         function Et(t) {
             return function() {
                 this.style.removeProperty(t)
             }
         }
 
-        function Nt(t, e, n) {
+        function St(t, e, n) {
             return function() {
                 this.style.setProperty(t, e, n)
             }
         }
 
-        function St(t, e, n) {
+        function Nt(t, e, n) {
             return function() {
                 var r = e.apply(this, arguments);
                 null == r ? this.style.removeProperty(t) : this.style.setProperty(t, r, n)
             }
         }
 
         function $t(t, e) {
             return t.style.getPropertyValue(e) || At(t).getComputedStyle(t, null).getPropertyValue(e)
         }
 
-        function Ct(t) {
+        function Vt(t) {
             return function() {
                 delete this[t]
             }
         }
 
-        function Tt(t, e) {
+        function jt(t, e) {
             return function() {
                 this[t] = e
             }
         }
 
-        function jt(t, e) {
+        function Ct(t, e) {
             return function() {
                 var n = e.apply(this, arguments);
                 null == n ? delete this[t] : this[t] = n
             }
         }
 
-        function Ot(t) {
+        function Tt(t) {
             return t.trim().split(/^|\s+/)
         }
 
         function Pt(t) {
-            return t.classList || new Vt(t)
+            return t.classList || new Ot(t)
         }
 
-        function Vt(t) {
-            this._node = t, this._names = Ot(t.getAttribute("class") || "")
+        function Ot(t) {
+            this._node = t, this._names = Tt(t.getAttribute("class") || "")
         }
 
         function Lt(t, e) {
             for (var n = Pt(t), r = -1, i = e.length; ++r < i;) n.add(e[r])
         }
 
         function Dt(t, e) {
             for (var n = Pt(t), r = -1, i = e.length; ++r < i;) n.remove(e[r])
         }
 
-        function It(t) {
+        function Rt(t) {
             return function() {
                 Lt(this, t)
             }
         }
 
-        function Rt(t) {
+        function It(t) {
             return function() {
                 Dt(this, t)
             }
         }
 
         function qt(t, e) {
             return function() {
@@ -911,15 +913,15 @@
         }
 
         function ae(t, e) {
             return function() {
                 return ie(this, t, e.apply(this, arguments))
             }
         }
-        Vt.prototype = {
+        Ot.prototype = {
             add: function(t) {
                 this._names.indexOf(t) < 0 && (this._names.push(t), this._node.setAttribute("class", this._names.join(" ")))
             },
             remove: function(t) {
                 var e = this._names.indexOf(t);
                 e >= 0 && (this._names.splice(e, 1), this._node.setAttribute("class", this._names.join(" ")))
             },
@@ -974,30 +976,30 @@
             filter: function(t) {
                 "function" != typeof t && (t = rt(t));
                 for (var e = this._groups, n = e.length, r = new Array(n), i = 0; i < n; ++i)
                     for (var o, a = e[i], s = a.length, l = r[i] = [], u = 0; u < s; ++u)(o = a[u]) && t.call(o, o.__data__, u, a) && l.push(o);
                 return new le(r, this._parents)
             },
             data: function(t, e) {
-                if (!arguments.length) return Array.from(this, dt);
-                var n, r = e ? ft : ht,
+                if (!arguments.length) return Array.from(this, ft);
+                var n, r = e ? dt : ht,
                     i = this._parents,
                     o = this._groups;
                 "function" != typeof t && (n = t, t = function() {
                     return n
                 });
                 for (var a = o.length, s = new Array(a), l = new Array(a), u = new Array(a), c = 0; c < a; ++c) {
                     var h = i[c],
-                        f = o[c],
-                        d = f.length,
+                        d = o[c],
+                        f = d.length,
                         p = pt(t.call(h, h && h.__data__, c, i)),
                         m = p.length,
                         _ = l[c] = new Array(m),
                         g = s[c] = new Array(m);
-                    r(h, f, _, g, u[c] = new Array(d), p, e);
+                    r(h, d, _, g, u[c] = new Array(f), p, e);
                     for (var v, y, w = 0, x = 0; w < m; ++w)
                         if (v = _[w]) {
                             for (w >= x && (x = w + 1); !(y = g[x]) && ++x < m;);
                             v._next = y || null
                         }
                 }
                 return (s = new le(s, i))._enter = l, s._exit = u, s
@@ -1012,15 +1014,15 @@
                 var r = this.enter(),
                     i = this,
                     o = this.exit();
                 return "function" == typeof t ? (r = t(r)) && (r = r.selection()) : r = r.append(t + ""), null != e && (i = e(i)) && (i = i.selection()), null == n ? o.remove() : n(o), r && i ? r.merge(i).order() : i
             },
             merge: function(t) {
                 for (var e = t.selection ? t.selection() : t, n = this._groups, r = e._groups, i = n.length, o = r.length, a = Math.min(i, o), s = new Array(i), l = 0; l < a; ++l)
-                    for (var u, c = n[l], h = r[l], f = c.length, d = s[l] = new Array(f), p = 0; p < f; ++p)(u = c[p] || h[p]) && (d[p] = u);
+                    for (var u, c = n[l], h = r[l], d = c.length, f = s[l] = new Array(d), p = 0; p < d; ++p)(u = c[p] || h[p]) && (f[p] = u);
                 for (; l < i; ++l) s[l] = n[l];
                 return new le(s, this._parents)
             },
             selection: function() {
                 return this
             },
             order: function() {
@@ -1072,27 +1074,27 @@
                 if (arguments.length < 2) {
                     var r = this.node();
                     return n.local ? r.getAttributeNS(n.space, n.local) : r.getAttribute(n)
                 }
                 return this.each((null == e ? n.local ? wt : yt : "function" == typeof e ? n.local ? kt : Mt : n.local ? bt : xt)(n, e))
             },
             style: function(t, e, n) {
-                return arguments.length > 1 ? this.each((null == e ? Et : "function" == typeof e ? St : Nt)(t, e, null == n ? "" : n)) : $t(this.node(), t)
+                return arguments.length > 1 ? this.each((null == e ? Et : "function" == typeof e ? Nt : St)(t, e, null == n ? "" : n)) : $t(this.node(), t)
             },
             property: function(t, e) {
-                return arguments.length > 1 ? this.each((null == e ? Ct : "function" == typeof e ? jt : Tt)(t, e)) : this.node()[t]
+                return arguments.length > 1 ? this.each((null == e ? Vt : "function" == typeof e ? Ct : jt)(t, e)) : this.node()[t]
             },
             classed: function(t, e) {
-                var n = Ot(t + "");
+                var n = Tt(t + "");
                 if (arguments.length < 2) {
                     for (var r = Pt(this.node()), i = -1, o = n.length; ++i < o;)
                         if (!r.contains(n[i])) return !1;
                     return !0
                 }
-                return this.each(("function" == typeof e ? qt : e ? It : Rt)(n, e))
+                return this.each(("function" == typeof e ? qt : e ? Rt : It)(n, e))
             },
             text: function(t) {
                 return arguments.length ? this.each(null == t ? Ht : ("function" == typeof t ? Xt : zt)(t)) : this.node().textContent
             },
             html: function(t) {
                 return arguments.length ? this.each(null == t ? Yt : ("function" == typeof t ? Ft : Bt)(t)) : this.node().innerHTML
             },
@@ -1155,23 +1157,23 @@
             }
         };
         const ce = ue;
         var he = {
             value: () => {}
         };
 
-        function fe() {
+        function de() {
             for (var t, e = 0, n = arguments.length, r = {}; e < n; ++e) {
                 if (!(t = arguments[e] + "") || t in r || /[\s.]/.test(t)) throw new Error("illegal type: " + t);
                 r[t] = []
             }
-            return new de(r)
+            return new fe(r)
         }
 
-        function de(t) {
+        function fe(t) {
             this._ = t
         }
 
         function pe(t, e) {
             for (var n, r = 0, i = t.length; r < i; ++r)
                 if ((n = t[r]).name === e) return n.value
         }
@@ -1182,16 +1184,16 @@
                     t[r] = he, t = t.slice(0, r).concat(t.slice(r + 1));
                     break
                 } return null != n && t.push({
                 name: e,
                 value: n
             }), t
         }
-        de.prototype = fe.prototype = {
-            constructor: de,
+        fe.prototype = de.prototype = {
+            constructor: fe,
             on: function(t, e) {
                 var n, r, i = this._,
                     o = (r = i, (t + "").trim().split(/^|\s+/).map((function(t) {
                         var e = "",
                             n = t.indexOf(".");
                         if (n >= 0 && (e = t.slice(n + 1), t = t.slice(0, n)), t && !r.hasOwnProperty(t)) throw new Error("unknown type: " + t);
                         return {
@@ -1212,164 +1214,164 @@
                 for (; ++a < s;)
                     if ((n = (t = o[a]).type) && (n = pe(i[n], t.name))) return n
             },
             copy: function() {
                 var t = {},
                     e = this._;
                 for (var n in e) t[n] = e[n].slice();
-                return new de(t)
+                return new fe(t)
             },
             call: function(t, e) {
                 if ((n = arguments.length - 2) > 0)
                     for (var n, r, i = new Array(n), o = 0; o < n; ++o) i[o] = arguments[o + 2];
                 if (!this._.hasOwnProperty(t)) throw new Error("unknown type: " + t);
                 for (o = 0, n = (r = this._[t]).length; o < n; ++o) r[o].value.apply(e, i)
             },
             apply: function(t, e, n) {
                 if (!this._.hasOwnProperty(t)) throw new Error("unknown type: " + t);
                 for (var r = this._[t], i = 0, o = r.length; i < o; ++i) r[i].value.apply(e, n)
             }
         };
-        const _e = fe;
+        const _e = de;
         var ge, ve, ye = 0,
             we = 0,
             xe = 0,
             be = 1e3,
             Me = 0,
             ke = 0,
             Ae = 0,
             Ee = "object" == typeof performance && performance.now ? performance : Date,
-            Ne = "object" == typeof window && window.requestAnimationFrame ? window.requestAnimationFrame.bind(window) : function(t) {
+            Se = "object" == typeof window && window.requestAnimationFrame ? window.requestAnimationFrame.bind(window) : function(t) {
                 setTimeout(t, 17)
             };
 
-        function Se() {
-            return ke || (Ne($e), ke = Ee.now() + Ae)
+        function Ne() {
+            return ke || (Se($e), ke = Ee.now() + Ae)
         }
 
         function $e() {
             ke = 0
         }
 
-        function Ce() {
+        function Ve() {
             this._call = this._time = this._next = null
         }
 
-        function Te(t, e, n) {
-            var r = new Ce;
+        function je(t, e, n) {
+            var r = new Ve;
             return r.restart(t, e, n), r
         }
 
-        function je() {
+        function Ce() {
             ke = (Me = Ee.now()) + Ae, ye = we = 0;
             try {
                 ! function() {
-                    Se(), ++ye;
+                    Ne(), ++ye;
                     for (var t, e = ge; e;)(t = ke - e._time) >= 0 && e._call.call(void 0, t), e = e._next;
                     --ye
                 }()
             } finally {
                 ye = 0,
                     function() {
                         for (var t, e, n = ge, r = 1 / 0; n;) n._call ? (r > n._time && (r = n._time), t = n, n = n._next) : (e = n._next, n._next = null, n = t ? t._next = e : ge = e);
                         ve = t, Pe(r)
                     }(), ke = 0
             }
         }
 
-        function Oe() {
+        function Te() {
             var t = Ee.now(),
                 e = t - Me;
             e > be && (Ae -= e, Me = t)
         }
 
         function Pe(t) {
-            ye || (we && (we = clearTimeout(we)), t - ke > 24 ? (t < 1 / 0 && (we = setTimeout(je, t - Ee.now() - Ae)), xe && (xe = clearInterval(xe))) : (xe || (Me = Ee.now(), xe = setInterval(Oe, be)), ye = 1, Ne(je)))
+            ye || (we && (we = clearTimeout(we)), t - ke > 24 ? (t < 1 / 0 && (we = setTimeout(Ce, t - Ee.now() - Ae)), xe && (xe = clearInterval(xe))) : (xe || (Me = Ee.now(), xe = setInterval(Te, be)), ye = 1, Se(Ce)))
         }
 
-        function Ve(t, e, n) {
-            var r = new Ce;
+        function Oe(t, e, n) {
+            var r = new Ve;
             return e = null == e ? 0 : +e, r.restart((n => {
                 r.stop(), t(n + e)
             }), e, n), r
         }
-        Ce.prototype = Te.prototype = {
-            constructor: Ce,
+        Ve.prototype = je.prototype = {
+            constructor: Ve,
             restart: function(t, e, n) {
                 if ("function" != typeof t) throw new TypeError("callback is not a function");
-                n = (null == n ? Se() : +n) + (null == e ? 0 : +e), this._next || ve === this || (ve ? ve._next = this : ge = this, ve = this), this._call = t, this._time = n, Pe()
+                n = (null == n ? Ne() : +n) + (null == e ? 0 : +e), this._next || ve === this || (ve ? ve._next = this : ge = this, ve = this), this._call = t, this._time = n, Pe()
             },
             stop: function() {
                 this._call && (this._call = null, this._time = 1 / 0, Pe())
             }
         };
         var Le = _e("start", "end", "cancel", "interrupt"),
             De = [],
-            Ie = 0,
-            Re = 3;
+            Re = 0,
+            Ie = 3;
 
         function qe(t, e, n, r, i, o) {
             var a = t.__transition;
             if (a) {
                 if (n in a) return
             } else t.__transition = {};
             ! function(t, e, n) {
                 var r, i = t.__transition;
 
                 function o(l) {
-                    var u, c, h, f;
+                    var u, c, h, d;
                     if (1 !== n.state) return s();
                     for (u in i)
-                        if ((f = i[u]).name === n.name) {
-                            if (f.state === Re) return Ve(o);
-                            4 === f.state ? (f.state = 6, f.timer.stop(), f.on.call("interrupt", t, t.__data__, f.index, f.group), delete i[u]) : +u < e && (f.state = 6, f.timer.stop(), f.on.call("cancel", t, t.__data__, f.index, f.group), delete i[u])
-                        } if (Ve((function() {
-                            n.state === Re && (n.state = 4, n.timer.restart(a, n.delay, n.time), a(l))
+                        if ((d = i[u]).name === n.name) {
+                            if (d.state === Ie) return Oe(o);
+                            4 === d.state ? (d.state = 6, d.timer.stop(), d.on.call("interrupt", t, t.__data__, d.index, d.group), delete i[u]) : +u < e && (d.state = 6, d.timer.stop(), d.on.call("cancel", t, t.__data__, d.index, d.group), delete i[u])
+                        } if (Oe((function() {
+                            n.state === Ie && (n.state = 4, n.timer.restart(a, n.delay, n.time), a(l))
                         })), n.state = 2, n.on.call("start", t, t.__data__, n.index, n.group), 2 === n.state) {
-                        for (n.state = Re, r = new Array(h = n.tween.length), u = 0, c = -1; u < h; ++u)(f = n.tween[u].value.call(t, t.__data__, n.index, n.group)) && (r[++c] = f);
+                        for (n.state = Ie, r = new Array(h = n.tween.length), u = 0, c = -1; u < h; ++u)(d = n.tween[u].value.call(t, t.__data__, n.index, n.group)) && (r[++c] = d);
                         r.length = c + 1
                     }
                 }
 
                 function a(e) {
                     for (var i = e < n.duration ? n.ease.call(null, e / n.duration) : (n.timer.restart(s), n.state = 5, 1), o = -1, a = r.length; ++o < a;) r[o].call(t, i);
                     5 === n.state && (n.on.call("end", t, t.__data__, n.index, n.group), s())
                 }
 
                 function s() {
                     for (var r in n.state = 6, n.timer.stop(), delete i[e], i) return;
                     delete t.__transition
                 }
-                i[e] = n, n.timer = Te((function(t) {
+                i[e] = n, n.timer = je((function(t) {
                     n.state = 1, n.timer.restart(o, n.delay, n.time), n.delay <= t && o(t - n.delay)
                 }), 0, n.time)
             }(t, n, {
                 name: e,
                 index: r,
                 group: i,
                 on: Le,
                 tween: De,
                 time: o.time,
                 delay: o.delay,
                 duration: o.duration,
                 ease: o.ease,
                 timer: null,
-                state: Ie
+                state: Re
             })
         }
 
         function He(t, e) {
             var n = Xe(t, e);
-            if (n.state > Ie) throw new Error("too late; already scheduled");
+            if (n.state > Re) throw new Error("too late; already scheduled");
             return n
         }
 
         function ze(t, e) {
             var n = Xe(t, e);
-            if (n.state > Re) throw new Error("too late; already running");
+            if (n.state > Ie) throw new Error("too late; already running");
             return n
         }
 
         function Xe(t, e) {
             var n = t.__transition;
             if (!n || !(n = n[e])) throw new Error("transition not found");
             return n
@@ -1521,16 +1523,16 @@
         var on = .7,
             an = 1 / on,
             sn = "\\s*([+-]?\\d+)\\s*",
             ln = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)\\s*",
             un = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)%\\s*",
             cn = /^#([0-9a-f]{3,8})$/,
             hn = new RegExp(`^rgb\\(${sn},${sn},${sn}\\)$`),
-            fn = new RegExp(`^rgb\\(${un},${un},${un}\\)$`),
-            dn = new RegExp(`^rgba\\(${sn},${sn},${sn},${ln}\\)$`),
+            dn = new RegExp(`^rgb\\(${un},${un},${un}\\)$`),
+            fn = new RegExp(`^rgba\\(${sn},${sn},${sn},${ln}\\)$`),
             pn = new RegExp(`^rgba\\(${un},${un},${un},${ln}\\)$`),
             mn = new RegExp(`^hsl\\(${ln},${un},${un}\\)$`),
             _n = new RegExp(`^hsla\\(${ln},${un},${un},${ln}\\)$`),
             gn = {
                 aliceblue: 15792383,
                 antiquewhite: 16444375,
                 aqua: 65535,
@@ -1687,15 +1689,15 @@
 
         function yn() {
             return this.rgb().formatRgb()
         }
 
         function wn(t) {
             var e, n;
-            return t = (t + "").trim().toLowerCase(), (e = cn.exec(t)) ? (n = e[1].length, e = parseInt(e[1], 16), 6 === n ? xn(e) : 3 === n ? new kn(e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, (15 & e) << 4 | 15 & e, 1) : 8 === n ? bn(e >> 24 & 255, e >> 16 & 255, e >> 8 & 255, (255 & e) / 255) : 4 === n ? bn(e >> 12 & 15 | e >> 8 & 240, e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, ((15 & e) << 4 | 15 & e) / 255) : null) : (e = hn.exec(t)) ? new kn(e[1], e[2], e[3], 1) : (e = fn.exec(t)) ? new kn(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, 1) : (e = dn.exec(t)) ? bn(e[1], e[2], e[3], e[4]) : (e = pn.exec(t)) ? bn(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, e[4]) : (e = mn.exec(t)) ? Cn(e[1], e[2] / 100, e[3] / 100, 1) : (e = _n.exec(t)) ? Cn(e[1], e[2] / 100, e[3] / 100, e[4]) : gn.hasOwnProperty(t) ? xn(gn[t]) : "transparent" === t ? new kn(NaN, NaN, NaN, 0) : null
+            return t = (t + "").trim().toLowerCase(), (e = cn.exec(t)) ? (n = e[1].length, e = parseInt(e[1], 16), 6 === n ? xn(e) : 3 === n ? new kn(e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, (15 & e) << 4 | 15 & e, 1) : 8 === n ? bn(e >> 24 & 255, e >> 16 & 255, e >> 8 & 255, (255 & e) / 255) : 4 === n ? bn(e >> 12 & 15 | e >> 8 & 240, e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, ((15 & e) << 4 | 15 & e) / 255) : null) : (e = hn.exec(t)) ? new kn(e[1], e[2], e[3], 1) : (e = dn.exec(t)) ? new kn(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, 1) : (e = fn.exec(t)) ? bn(e[1], e[2], e[3], e[4]) : (e = pn.exec(t)) ? bn(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, e[4]) : (e = mn.exec(t)) ? Vn(e[1], e[2] / 100, e[3] / 100, 1) : (e = _n.exec(t)) ? Vn(e[1], e[2] / 100, e[3] / 100, e[4]) : gn.hasOwnProperty(t) ? xn(gn[t]) : "transparent" === t ? new kn(NaN, NaN, NaN, 0) : null
         }
 
         function xn(t) {
             return new kn(t >> 16 & 255, t >> 8 & 255, 255 & t, 1)
         }
 
         function bn(t, e, n, r) {
@@ -1712,62 +1714,62 @@
         }
 
         function An() {
             return `#${$n(this.r)}${$n(this.g)}${$n(this.b)}`
         }
 
         function En() {
-            const t = Nn(this.opacity);
-            return `${1===t?"rgb(":"rgba("}${Sn(this.r)}, ${Sn(this.g)}, ${Sn(this.b)}${1===t?")":`, ${t})`}`
+            const t = Sn(this.opacity);
+            return `${1===t?"rgb(":"rgba("}${Nn(this.r)}, ${Nn(this.g)}, ${Nn(this.b)}${1===t?")":`, ${t})`}`
         }
 
-        function Nn(t) {
+        function Sn(t) {
             return isNaN(t) ? 1 : Math.max(0, Math.min(1, t))
         }
 
-        function Sn(t) {
+        function Nn(t) {
             return Math.max(0, Math.min(255, Math.round(t) || 0))
         }
 
         function $n(t) {
-            return ((t = Sn(t)) < 16 ? "0" : "") + t.toString(16)
+            return ((t = Nn(t)) < 16 ? "0" : "") + t.toString(16)
         }
 
-        function Cn(t, e, n, r) {
-            return r <= 0 ? t = e = n = NaN : n <= 0 || n >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new jn(t, e, n, r)
+        function Vn(t, e, n, r) {
+            return r <= 0 ? t = e = n = NaN : n <= 0 || n >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new Cn(t, e, n, r)
         }
 
-        function Tn(t) {
-            if (t instanceof jn) return new jn(t.h, t.s, t.l, t.opacity);
-            if (t instanceof rn || (t = wn(t)), !t) return new jn;
-            if (t instanceof jn) return t;
+        function jn(t) {
+            if (t instanceof Cn) return new Cn(t.h, t.s, t.l, t.opacity);
+            if (t instanceof rn || (t = wn(t)), !t) return new Cn;
+            if (t instanceof Cn) return t;
             var e = (t = t.rgb()).r / 255,
                 n = t.g / 255,
                 r = t.b / 255,
                 i = Math.min(e, n, r),
                 o = Math.max(e, n, r),
                 a = NaN,
                 s = o - i,
                 l = (o + i) / 2;
-            return s ? (a = e === o ? (n - r) / s + 6 * (n < r) : n === o ? (r - e) / s + 2 : (e - n) / s + 4, s /= l < .5 ? o + i : 2 - o - i, a *= 60) : s = l > 0 && l < 1 ? 0 : a, new jn(a, s, l, t.opacity)
+            return s ? (a = e === o ? (n - r) / s + 6 * (n < r) : n === o ? (r - e) / s + 2 : (e - n) / s + 4, s /= l < .5 ? o + i : 2 - o - i, a *= 60) : s = l > 0 && l < 1 ? 0 : a, new Cn(a, s, l, t.opacity)
         }
 
-        function jn(t, e, n, r) {
+        function Cn(t, e, n, r) {
             this.h = +t, this.s = +e, this.l = +n, this.opacity = +r
         }
 
-        function On(t) {
+        function Tn(t) {
             return (t = (t || 0) % 360) < 0 ? t + 360 : t
         }
 
         function Pn(t) {
             return Math.max(0, Math.min(1, t || 0))
         }
 
-        function Vn(t, e, n) {
+        function On(t, e, n) {
             return 255 * (t < 60 ? e + (n - e) * t / 60 : t < 180 ? n : t < 240 ? e + (n - e) * (240 - t) / 60 : e)
         }
 
         function Ln(t, e, n, r, i) {
             var o = t * t,
                 a = o * t;
             return ((1 - 3 * t + 3 * o - a) * e + (4 - 6 * o + 3 * a) * n + (1 + 3 * t + 3 * o - 3 * a) * r + a * i) / 6
@@ -1781,96 +1783,96 @@
             },
             hex: vn,
             formatHex: vn,
             formatHex8: function() {
                 return this.rgb().formatHex8()
             },
             formatHsl: function() {
-                return Tn(this).formatHsl()
+                return jn(this).formatHsl()
             },
             formatRgb: yn,
             toString: yn
         }), en(kn, Mn, nn(rn, {
             brighter(t) {
                 return t = null == t ? an : Math.pow(an, t), new kn(this.r * t, this.g * t, this.b * t, this.opacity)
             },
             darker(t) {
                 return t = null == t ? on : Math.pow(on, t), new kn(this.r * t, this.g * t, this.b * t, this.opacity)
             },
             rgb() {
                 return this
             },
             clamp() {
-                return new kn(Sn(this.r), Sn(this.g), Sn(this.b), Nn(this.opacity))
+                return new kn(Nn(this.r), Nn(this.g), Nn(this.b), Sn(this.opacity))
             },
             displayable() {
                 return -.5 <= this.r && this.r < 255.5 && -.5 <= this.g && this.g < 255.5 && -.5 <= this.b && this.b < 255.5 && 0 <= this.opacity && this.opacity <= 1
             },
             hex: An,
             formatHex: An,
             formatHex8: function() {
                 return `#${$n(this.r)}${$n(this.g)}${$n(this.b)}${$n(255*(isNaN(this.opacity)?1:this.opacity))}`
             },
             formatRgb: En,
             toString: En
-        })), en(jn, (function(t, e, n, r) {
-            return 1 === arguments.length ? Tn(t) : new jn(t, e, n, null == r ? 1 : r)
+        })), en(Cn, (function(t, e, n, r) {
+            return 1 === arguments.length ? jn(t) : new Cn(t, e, n, null == r ? 1 : r)
         }), nn(rn, {
             brighter(t) {
-                return t = null == t ? an : Math.pow(an, t), new jn(this.h, this.s, this.l * t, this.opacity)
+                return t = null == t ? an : Math.pow(an, t), new Cn(this.h, this.s, this.l * t, this.opacity)
             },
             darker(t) {
-                return t = null == t ? on : Math.pow(on, t), new jn(this.h, this.s, this.l * t, this.opacity)
+                return t = null == t ? on : Math.pow(on, t), new Cn(this.h, this.s, this.l * t, this.opacity)
             },
             rgb() {
                 var t = this.h % 360 + 360 * (this.h < 0),
                     e = isNaN(t) || isNaN(this.s) ? 0 : this.s,
                     n = this.l,
                     r = n + (n < .5 ? n : 1 - n) * e,
                     i = 2 * n - r;
-                return new kn(Vn(t >= 240 ? t - 240 : t + 120, i, r), Vn(t, i, r), Vn(t < 120 ? t + 240 : t - 120, i, r), this.opacity)
+                return new kn(On(t >= 240 ? t - 240 : t + 120, i, r), On(t, i, r), On(t < 120 ? t + 240 : t - 120, i, r), this.opacity)
             },
             clamp() {
-                return new jn(On(this.h), Pn(this.s), Pn(this.l), Nn(this.opacity))
+                return new Cn(Tn(this.h), Pn(this.s), Pn(this.l), Sn(this.opacity))
             },
             displayable() {
                 return (0 <= this.s && this.s <= 1 || isNaN(this.s)) && 0 <= this.l && this.l <= 1 && 0 <= this.opacity && this.opacity <= 1
             },
             formatHsl() {
-                const t = Nn(this.opacity);
-                return `${1===t?"hsl(":"hsla("}${On(this.h)}, ${100*Pn(this.s)}%, ${100*Pn(this.l)}%${1===t?")":`, ${t})`}`
+                const t = Sn(this.opacity);
+                return `${1===t?"hsl(":"hsla("}${Tn(this.h)}, ${100*Pn(this.s)}%, ${100*Pn(this.l)}%${1===t?")":`, ${t})`}`
             }
         }));
         const Dn = t => () => t;
 
-        function In(t, e) {
+        function Rn(t, e) {
             var n = e - t;
             return n ? function(t, e) {
                 return function(n) {
                     return t + n * e
                 }
             }(t, n) : Dn(isNaN(t) ? e : t)
         }
-        const Rn = function t(e) {
+        const In = function t(e) {
             var n = function(t) {
-                return 1 == (t = +t) ? In : function(e, n) {
+                return 1 == (t = +t) ? Rn : function(e, n) {
                     return n - e ? function(t, e, n) {
                         return t = Math.pow(t, n), e = Math.pow(e, n) - t, n = 1 / n,
                             function(r) {
                                 return Math.pow(t + r * e, n)
                             }
                     }(e, n, t) : Dn(isNaN(e) ? n : e)
                 }
             }(e);
 
             function r(t, e) {
                 var r = n((t = Mn(t)).r, (e = Mn(e)).r),
                     i = n(t.g, e.g),
                     o = n(t.b, e.b),
-                    a = In(t.opacity, e.opacity);
+                    a = Rn(t.opacity, e.opacity);
                 return function(e) {
                     return t.r = r(e), t.g = i(e), t.b = o(e), t.opacity = a(e), t + ""
                 }
             }
             return r.gamma = t, r
         }(1);
 
@@ -1933,15 +1935,15 @@
                 for (var n, r = 0; r < e; ++r) s[(n = l[r]).i] = n.x(t);
                 return s.join("")
             })
         }
 
         function Yn(t, e) {
             var n;
-            return ("number" == typeof e ? Ye : e instanceof wn ? Rn : (n = wn(e)) ? (e = n, Rn) : Xn)(t, e)
+            return ("number" == typeof e ? Ye : e instanceof wn ? In : (n = wn(e)) ? (e = n, In) : Xn)(t, e)
         }
 
         function Bn(t) {
             return function() {
                 this.removeAttribute(t)
             }
         }
@@ -2061,40 +2063,40 @@
         }.prototype = {
             constructor: ar,
             select: function(t) {
                 var e = this._name,
                     n = this._id;
                 "function" != typeof t && (t = tt(t));
                 for (var r = this._groups, i = r.length, o = new Array(i), a = 0; a < i; ++a)
-                    for (var s, l, u = r[a], c = u.length, h = o[a] = new Array(c), f = 0; f < c; ++f)(s = u[f]) && (l = t.call(s, s.__data__, f, u)) && ("__data__" in s && (l.__data__ = s.__data__), h[f] = l, qe(h[f], e, n, f, h, Xe(s, n)));
+                    for (var s, l, u = r[a], c = u.length, h = o[a] = new Array(c), d = 0; d < c; ++d)(s = u[d]) && (l = t.call(s, s.__data__, d, u)) && ("__data__" in s && (l.__data__ = s.__data__), h[d] = l, qe(h[d], e, n, d, h, Xe(s, n)));
                 return new ar(o, this._parents, e, n)
             },
             selectAll: function(t) {
                 var e = this._name,
                     n = this._id;
                 "function" != typeof t && (t = nt(t));
                 for (var r = this._groups, i = r.length, o = [], a = [], s = 0; s < i; ++s)
                     for (var l, u = r[s], c = u.length, h = 0; h < c; ++h)
                         if (l = u[h]) {
-                            for (var f, d = t.call(l, l.__data__, h, u), p = Xe(l, n), m = 0, _ = d.length; m < _; ++m)(f = d[m]) && qe(f, e, n, m, d, p);
-                            o.push(d), a.push(l)
+                            for (var d, f = t.call(l, l.__data__, h, u), p = Xe(l, n), m = 0, _ = f.length; m < _; ++m)(d = f[m]) && qe(d, e, n, m, f, p);
+                            o.push(f), a.push(l)
                         } return new ar(o, a, e, n)
             },
             selectChild: lr.selectChild,
             selectChildren: lr.selectChildren,
             filter: function(t) {
                 "function" != typeof t && (t = rt(t));
                 for (var e = this._groups, n = e.length, r = new Array(n), i = 0; i < n; ++i)
                     for (var o, a = e[i], s = a.length, l = r[i] = [], u = 0; u < s; ++u)(o = a[u]) && t.call(o, o.__data__, u, a) && l.push(o);
                 return new ar(r, this._parents, this._name, this._id)
             },
             merge: function(t) {
                 if (t._id !== this._id) throw new Error;
                 for (var e = this._groups, n = t._groups, r = e.length, i = n.length, o = Math.min(r, i), a = new Array(r), s = 0; s < o; ++s)
-                    for (var l, u = e[s], c = n[s], h = u.length, f = a[s] = new Array(h), d = 0; d < h; ++d)(l = u[d] || c[d]) && (f[d] = l);
+                    for (var l, u = e[s], c = n[s], h = u.length, d = a[s] = new Array(h), f = 0; f < h; ++f)(l = u[f] || c[f]) && (d[f] = l);
                 for (; s < r; ++s) a[s] = e[s];
                 return new ar(a, this._parents, this._name, this._id)
             },
             selection: function() {
                 return new rr(this._groups, this._parents)
             },
             transition: function() {
@@ -2320,23 +2322,23 @@
                         for (i in e = null == e ? null : e + "", o)(n = o[i]).name === e ? (r = n.state > 2 && n.state < 5, n.state = 6, n.timer.stop(), n.on.call(r ? "interrupt" : "cancel", t, t.__data__, n.index, n.group), delete o[i]) : a = !1;
                         a && delete t.__transition
                     }
                 }(this, t)
             }))
         }, ce.prototype.transition = function(t) {
             var e, n;
-            t instanceof ar ? (e = t._id, t = t._name) : (e = sr(), (n = ur).time = Se(), t = null == t ? null : t + "");
+            t instanceof ar ? (e = t._id, t = t._name) : (e = sr(), (n = ur).time = Ne(), t = null == t ? null : t + "");
             for (var r = this._groups, i = r.length, o = 0; o < i; ++o)
                 for (var a, s = r[o], l = s.length, u = 0; u < l; ++u)(a = s[u]) && qe(a, t, e, u, s, n || cr(a, e));
             return new ar(r, this._parents, t, e)
         };
         const {
             abs: hr,
-            max: fr,
-            min: dr
+            max: dr,
+            min: fr
         } = Math;
 
         function pr(t) {
             return {
                 type: t
             }
         }
@@ -2468,15 +2470,15 @@
             } : e
         }
 
         function Er() {
             return navigator.maxTouchPoints || "ontouchstart" in this
         }
 
-        function Nr(t, e) {
+        function Sr(t, e) {
             switch (arguments.length) {
                 case 0:
                     break;
                 case 1:
                     this.range(t);
                     break;
                 default:
@@ -2484,16 +2486,16 @@
             }
             return this
         }
         br.prototype.on = function() {
             var t = this._.on.apply(this._, arguments);
             return t === this._ ? this : t
         };
-        class Sr extends Map {
-            constructor(t, e = Cr) {
+        class Nr extends Map {
+            constructor(t, e = Vr) {
                 if (super(), Object.defineProperties(this, {
                         _intern: {
                             value: new Map
                         },
                         _key: {
                             value: e
                         }
@@ -2530,71 +2532,71 @@
             _intern: t,
             _key: e
         }, n) {
             const r = e(n);
             return t.has(r) ? t.get(r) : n
         }
 
-        function Cr(t) {
+        function Vr(t) {
             return null !== t && "object" == typeof t ? t.valueOf() : t
         }
         Set;
-        const Tr = Symbol("implicit");
+        const jr = Symbol("implicit");
 
-        function jr() {
-            var t = new Sr,
+        function Cr() {
+            var t = new Nr,
                 e = [],
                 n = [],
-                r = Tr;
+                r = jr;
 
             function i(i) {
                 let o = t.get(i);
                 if (void 0 === o) {
-                    if (r !== Tr) return r;
+                    if (r !== jr) return r;
                     t.set(i, o = e.push(i) - 1)
                 }
                 return n[o % n.length]
             }
             return i.domain = function(n) {
                 if (!arguments.length) return e.slice();
-                e = [], t = new Sr;
+                e = [], t = new Nr;
                 for (const r of n) t.has(r) || t.set(r, e.push(r) - 1);
                 return i
             }, i.range = function(t) {
                 return arguments.length ? (n = Array.from(t), i) : n.slice()
             }, i.unknown = function(t) {
                 return arguments.length ? (r = t, i) : r
             }, i.copy = function() {
-                return jr(e, n).unknown(r)
-            }, Nr.apply(i, arguments), i
+                return Cr(e, n).unknown(r)
+            }, Sr.apply(i, arguments), i
         }
 
-        function Or() {
-            var t, e, n = jr().unknown(void 0),
+        function Tr() {
+            var t, e, n = Cr().unknown(void 0),
                 r = n.domain,
                 i = n.range,
                 o = 0,
                 a = 1,
                 s = !1,
                 l = 0,
                 u = 0,
                 c = .5;
 
             function h() {
                 var n = r().length,
                     h = a < o,
-                    f = h ? a : o,
-                    d = h ? o : a;
-                t = (d - f) / Math.max(1, n - l + 2 * u), s && (t = Math.floor(t)), f += (d - f - t * (n - l)) * c, e = t * (1 - l), s && (f = Math.round(f), e = Math.round(e));
+                    d = h ? a : o,
+                    f = h ? o : a;
+                t = (f - d) / Math.max(1, n - l + 2 * u), s && (t = Math.floor(t)), d += (f - d - t * (n - l)) * c, e = t * (1 - l), s && (d = Math.round(d), e = Math.round(e));
                 var p = function(t, e, n) {
                     t = +t, e = +e, n = (i = arguments.length) < 2 ? (e = t, t = 0, 1) : i < 3 ? 1 : +n;
                     for (var r = -1, i = 0 | Math.max(0, Math.ceil((e - t) / n)), o = new Array(i); ++r < i;) o[r] = t + r * n;
                     return o
                 }(n).map((function(e) {
-                    return f + t * e
+                    return d + t * e
                 }));
                 return i(h ? p.reverse() : p)
             }
             return delete n.unknown, n.domain = function(t) {
                 return arguments.length ? (r(t), h()) : r()
             }, n.range = function(t) {
                 return arguments.length ? ([o, a] = t, o = +o, a = +a, h()) : [o, a]
@@ -2611,43 +2613,43 @@
             }, n.paddingInner = function(t) {
                 return arguments.length ? (l = Math.min(1, t), h()) : l
             }, n.paddingOuter = function(t) {
                 return arguments.length ? (u = +t, h()) : u
             }, n.align = function(t) {
                 return arguments.length ? (c = Math.max(0, Math.min(1, t)), h()) : c
             }, n.copy = function() {
-                return Or(r(), [o, a]).round(s).paddingInner(l).paddingOuter(u).align(c)
-            }, Nr.apply(h(), arguments)
+                return Tr(r(), [o, a]).round(s).paddingInner(l).paddingOuter(u).align(c)
+            }, Sr.apply(h(), arguments)
         }
 
         function Pr(t, e) {
             var n, r = e ? e.length : 0,
                 i = t ? Math.min(r, t.length) : 0,
                 o = new Array(i),
                 a = new Array(r);
-            for (n = 0; n < i; ++n) o[n] = Ir(t[n], e[n]);
+            for (n = 0; n < i; ++n) o[n] = Rr(t[n], e[n]);
             for (; n < r; ++n) a[n] = e[n];
             return function(t) {
                 for (n = 0; n < i; ++n) a[n] = o[n](t);
                 return a
             }
         }
 
-        function Vr(t, e) {
+        function Or(t, e) {
             var n = new Date;
             return t = +t, e = +e,
                 function(r) {
                     return n.setTime(t * (1 - r) + e * r), n
                 }
         }
 
         function Lr(t, e) {
             var n, r = {},
                 i = {};
-            for (n in null !== t && "object" == typeof t || (t = {}), null !== e && "object" == typeof e || (e = {}), e) n in t ? r[n] = Ir(t[n], e[n]) : i[n] = e[n];
+            for (n in null !== t && "object" == typeof t || (t = {}), null !== e && "object" == typeof e || (e = {}), e) n in t ? r[n] = Rr(t[n], e[n]) : i[n] = e[n];
             return function(t) {
                 for (n in r) i[n] = r[n](t);
                 return i
             }
         }
 
         function Dr(t, e) {
@@ -2656,20 +2658,20 @@
                 i = e.slice();
             return function(o) {
                 for (n = 0; n < r; ++n) i[n] = t[n] * (1 - o) + e[n] * o;
                 return i
             }
         }
 
-        function Ir(t, e) {
+        function Rr(t, e) {
             var n, r, i = typeof e;
-            return null == e || "boolean" === i ? Dn(e) : ("number" === i ? Ye : "string" === i ? (n = wn(e)) ? (e = n, Rn) : Xn : e instanceof wn ? Rn : e instanceof Date ? Vr : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? Pr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? Lr : Ye : Dr))(t, e)
+            return null == e || "boolean" === i ? Dn(e) : ("number" === i ? Ye : "string" === i ? (n = wn(e)) ? (e = n, In) : Xn : e instanceof wn ? In : e instanceof Date ? Or : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? Pr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? Lr : Ye : Dr))(t, e)
         }
 
-        function Rr(t, e) {
+        function Ir(t, e) {
             return t = +t, e = +e,
                 function(n) {
                     return Math.round(t * (1 - n) + e * n)
                 }
         }
 
         function qr(t) {
@@ -2787,15 +2789,15 @@
         var ei, ni, ri, ii = Array.prototype.map,
             oi = ["y", "z", "a", "f", "p", "n", "µ", "m", "", "k", "M", "G", "T", "P", "E", "Z", "Y"];
 
         function ai() {
             var t = function() {
                 var t, e, n, r, i, o, a = Hr,
                     s = Hr,
-                    l = Ir,
+                    l = Rr,
                     u = zr;
 
                 function c() {
                     var t, e, n, l = Math.min(a.length, s.length);
                     return u !== zr && (t = a[0], e = a[l - 1], t > e && (n = t, t = e, e = n), u = function(n) {
                         return Math.max(t, Math.min(e, n))
                     }), r = l > 2 ? Br : Yr, i = o = null, h
@@ -2807,35 +2809,35 @@
                 return h.invert = function(n) {
                         return u(e((o || (o = r(s, a.map(t), Ye)))(n)))
                     }, h.domain = function(t) {
                         return arguments.length ? (a = Array.from(t, qr), c()) : a.slice()
                     }, h.range = function(t) {
                         return arguments.length ? (s = Array.from(t), c()) : s.slice()
                     }, h.rangeRound = function(t) {
-                        return s = Array.from(t), l = Rr, c()
+                        return s = Array.from(t), l = Ir, c()
                     }, h.clamp = function(t) {
                         return arguments.length ? (u = !!t || zr, c()) : u !== zr
                     }, h.interpolate = function(t) {
                         return arguments.length ? (l = t, c()) : l
                     }, h.unknown = function(t) {
                         return arguments.length ? (n = t, h) : n
                     },
                     function(n, r) {
                         return t = n, e = r, c()
                     }
             }()(zr, zr);
             return t.copy = function() {
                     return e = t, ai().domain(e.domain()).range(e.range()).interpolate(e.interpolate()).clamp(e.clamp()).unknown(e.unknown());
                     var e
-                }, Nr.apply(t, arguments),
+                }, Sr.apply(t, arguments),
                 function(t) {
                     var e = t.domain;
                     return t.ticks = function(t) {
                         var n = e();
-                        return O(n[0], n[n.length - 1], null == t ? 10 : t)
+                        return T(n[0], n[n.length - 1], null == t ? 10 : t)
                     }, t.tickFormat = function(t, n) {
                         var r = e();
                         return function(t, e, n, r) {
                             var i, o = function(t, e, n) {
                                 n = +n;
                                 const r = (e = +e) < (t = +t),
                                     i = r ? P(e, t, n) : P(t, e, n);
@@ -2904,29 +2906,29 @@
                 u = void 0 === t.minus ? "−" : t.minus + "",
                 c = void 0 === t.nan ? "NaN" : t.nan + "";
 
             function h(t) {
                 var e = (t = Ur(t)).fill,
                     n = t.align,
                     h = t.sign,
-                    f = t.symbol,
-                    d = t.zero,
+                    d = t.symbol,
+                    f = t.zero,
                     p = t.width,
                     m = t.comma,
                     _ = t.precision,
                     g = t.trim,
                     v = t.type;
-                "n" === v ? (m = !0, v = "g") : Qr[v] || (void 0 === _ && (_ = 12), g = !0, v = "g"), (d || "0" === e && "=" === n) && (d = !0, e = "0", n = "=");
-                var y = "$" === f ? i : "#" === f && /[boxX]/.test(v) ? "0" + v.toLowerCase() : "",
-                    w = "$" === f ? o : /[%p]/.test(v) ? l : "",
+                "n" === v ? (m = !0, v = "g") : Qr[v] || (void 0 === _ && (_ = 12), g = !0, v = "g"), (f || "0" === e && "=" === n) && (f = !0, e = "0", n = "=");
+                var y = "$" === d ? i : "#" === d && /[boxX]/.test(v) ? "0" + v.toLowerCase() : "",
+                    w = "$" === d ? o : /[%p]/.test(v) ? l : "",
                     x = Qr[v],
                     b = /[defgprs%]/.test(v);
 
                 function M(t) {
-                    var i, o, l, f = y,
+                    var i, o, l, d = y,
                         M = w;
                     if ("c" === v) M = x(t) + M, t = "";
                     else {
                         var k = (t = +t) < 0 || 1 / t < 0;
                         if (t = isNaN(t) ? c : x(Math.abs(t), _), g && (t = function(t) {
                                 t: for (var e, n = t.length, r = 1, i = -1; r < n; ++r) switch (t[r]) {
                                     case ".":
@@ -2936,36 +2938,36 @@
                                         0 === i && (i = r), e = r;
                                         break;
                                     default:
                                         if (!+t[r]) break t;
                                         i > 0 && (i = 0)
                                 }
                                 return i > 0 ? t.slice(0, i) + t.slice(e + 1) : t
-                            }(t)), k && 0 == +t && "+" !== h && (k = !1), f = (k ? "(" === h ? h : u : "-" === h || "(" === h ? "" : h) + f, M = ("s" === v ? oi[8 + Fr / 3] : "") + M + (k && "(" === h ? ")" : ""), b)
+                            }(t)), k && 0 == +t && "+" !== h && (k = !1), d = (k ? "(" === h ? h : u : "-" === h || "(" === h ? "" : h) + d, M = ("s" === v ? oi[8 + Fr / 3] : "") + M + (k && "(" === h ? ")" : ""), b)
                             for (i = -1, o = t.length; ++i < o;)
                                 if (48 > (l = t.charCodeAt(i)) || l > 57) {
                                     M = (46 === l ? a + t.slice(i + 1) : t.slice(i)) + M, t = t.slice(0, i);
                                     break
                                 }
                     }
-                    m && !d && (t = r(t, 1 / 0));
-                    var A = f.length + t.length + M.length,
+                    m && !f && (t = r(t, 1 / 0));
+                    var A = d.length + t.length + M.length,
                         E = A < p ? new Array(p - A + 1).join(e) : "";
-                    switch (m && d && (t = r(E + t, E.length ? p - M.length : 1 / 0), E = ""), n) {
+                    switch (m && f && (t = r(E + t, E.length ? p - M.length : 1 / 0), E = ""), n) {
                         case "<":
-                            t = f + t + M + E;
+                            t = d + t + M + E;
                             break;
                         case "=":
-                            t = f + E + t + M;
+                            t = d + E + t + M;
                             break;
                         case "^":
-                            t = E.slice(0, A = E.length >> 1) + f + t + M + E.slice(A);
+                            t = E.slice(0, A = E.length >> 1) + d + t + M + E.slice(A);
                             break;
                         default:
-                            t = E + f + t + M
+                            t = E + d + t + M
                     }
                     return s(t)
                 }
                 return _ = void 0 === _ ? 6 : /[gprs]/.test(v) ? Math.max(1, Math.min(21, _)) : Math.max(0, Math.min(20, _)), M.toString = function() {
                     return t + ""
                 }, M
             }
@@ -3026,17 +3028,17 @@
                         this._point = 2;
                     default:
                         this._context.lineTo(t, e)
                 }
             }
         };
         const hi = Math.PI,
-            fi = 2 * hi,
-            di = 1e-6,
-            pi = fi - di;
+            di = 2 * hi,
+            fi = 1e-6,
+            pi = di - fi;
 
         function mi(t) {
             this._ += t[0];
             for (let e = 1, n = t.length; e < n; ++e) this._ += arguments[e] + t[e]
         }
         class _i {
             constructor(t) {
@@ -3072,37 +3074,37 @@
                     a = this._y1,
                     s = n - t,
                     l = r - e,
                     u = o - t,
                     c = a - e,
                     h = u * u + c * c;
                 if (null === this._x1) this._append`M${this._x1=t},${this._y1=e}`;
-                else if (h > di)
-                    if (Math.abs(c * s - l * u) > di && i) {
-                        let f = n - o,
-                            d = r - a,
+                else if (h > fi)
+                    if (Math.abs(c * s - l * u) > fi && i) {
+                        let d = n - o,
+                            f = r - a,
                             p = s * s + l * l,
-                            m = f * f + d * d,
+                            m = d * d + f * f,
                             _ = Math.sqrt(p),
                             g = Math.sqrt(h),
                             v = i * Math.tan((hi - Math.acos((p + h - m) / (2 * _ * g))) / 2),
                             y = v / g,
                             w = v / _;
-                        Math.abs(y - 1) > di && this._append`L${t+y*u},${e+y*c}`, this._append`A${i},${i},0,0,${+(c*f>u*d)},${this._x1=t+w*s},${this._y1=e+w*l}`
+                        Math.abs(y - 1) > fi && this._append`L${t+y*u},${e+y*c}`, this._append`A${i},${i},0,0,${+(c*d>u*f)},${this._x1=t+w*s},${this._y1=e+w*l}`
                     } else this._append`L${this._x1=t},${this._y1=e}`
             }
             arc(t, e, n, r, i, o) {
                 if (t = +t, e = +e, o = !!o, (n = +n) < 0) throw new Error(`negative radius: ${n}`);
                 let a = n * Math.cos(r),
                     s = n * Math.sin(r),
                     l = t + a,
                     u = e + s,
                     c = 1 ^ o,
                     h = o ? r - i : i - r;
-                null === this._x1 ? this._append`M${l},${u}` : (Math.abs(this._x1 - l) > di || Math.abs(this._y1 - u) > di) && this._append`L${l},${u}`, n && (h < 0 && (h = h % fi + fi), h > pi ? this._append`A${n},${n},0,1,${c},${t-a},${e-s}A${n},${n},0,1,${c},${this._x1=l},${this._y1=u}` : h > di && this._append`A${n},${n},0,${+(h>=hi)},${c},${this._x1=t+n*Math.cos(i)},${this._y1=e+n*Math.sin(i)}`)
+                null === this._x1 ? this._append`M${l},${u}` : (Math.abs(this._x1 - l) > fi || Math.abs(this._y1 - u) > fi) && this._append`L${l},${u}`, n && (h < 0 && (h = h % di + di), h > pi ? this._append`A${n},${n},0,1,${c},${t-a},${e-s}A${n},${n},0,1,${c},${this._x1=l},${this._y1=u}` : h > fi && this._append`A${n},${n},0,${+(h>=hi)},${c},${this._x1=t+n*Math.cos(i)},${this._y1=e+n*Math.sin(i)}`)
             }
             rect(t, e, n, r) {
                 this._append`M${this._x0=this._x1=+t},${this._y0=this._y1=+e}h${n=+n}v${+r}h${-n}Z`
             }
             toString() {
                 return this._
             }
@@ -3135,16 +3137,16 @@
                     }, () => new _i(e)
                 }(s);
 
             function s(s) {
                 var l, u, c, h = (s = function(t) {
                         return "object" == typeof t && "length" in t ? t : Array.from(t)
                     }(s)).length,
-                    f = !1;
-                for (null == r && (o = i(c = a())), l = 0; l <= h; ++l) !(l < h && n(u = s[l], l, s)) === f && ((f = !f) ? o.lineStart() : o.lineEnd()), f && o.point(+t(u, l, s), +e(u, l, s));
+                    d = !1;
+                for (null == r && (o = i(c = a())), l = 0; l <= h; ++l) !(l < h && n(u = s[l], l, s)) === d && ((d = !d) ? o.lineStart() : o.lineEnd()), d && o.point(+t(u, l, s), +e(u, l, s));
                 if (c) return o = null, c + "" || null
             }
             return t = "function" == typeof t ? t : void 0 === t ? gi : li(t), e = "function" == typeof e ? e : void 0 === e ? vi : li(e), s.x = function(e) {
                 return arguments.length ? (t = "function" == typeof e ? e : li(+e), s) : t
             }, s.y = function(t) {
                 return arguments.length ? (e = "function" == typeof t ? t : li(+t), s) : e
             }, s.defined = function(t) {
@@ -3286,30 +3288,30 @@
                 }(t, e);
             return [e - n, e + n]
         }
 
         function Ei(t, e, n, r, i, o, a, s, l, u) {
             let c = [];
             const h = yi(),
-                f = mr(t).selectAll(".dot"),
-                d = function() {
+                d = mr(t).selectAll(".dot"),
+                f = function() {
                     var t, e, n, r, i = Mr,
                         o = kr,
                         a = Ar,
                         s = Er,
                         l = {},
                         u = _e("start", "drag", "end"),
                         c = 0,
                         h = 0;
 
-                    function f(t) {
-                        t.on("mousedown.drag", d).filter(s).on("touchstart.drag", _).on("touchmove.drag", g, gr).on("touchend.drag touchcancel.drag", v).style("touch-action", "none").style("-webkit-tap-highlight-color", "rgba(0,0,0,0)")
+                    function d(t) {
+                        t.on("mousedown.drag", f).filter(s).on("touchstart.drag", _).on("touchmove.drag", g, gr).on("touchend.drag touchcancel.drag", v).style("touch-action", "none").style("-webkit-tap-highlight-color", "rgba(0,0,0,0)")
                     }
 
-                    function d(a, s) {
+                    function f(a, s) {
                         if (!r && i.call(this, a, s)) {
                             var l = y(this, o.call(this, a, s), a, s, "mouse");
                             l && (mr(a.view).on("mousemove.drag", p, vr).on("mouseup.drag", m, vr), function(t) {
                                 var e = t.document.documentElement,
                                     n = mr(t).on("dragstart.drag", wr, vr);
                                 "onselectstart" in e ? n.on("selectstart.drag", wr, vr) : (e.__noselect = e.style.MozUserSelect, e.style.MozUserSelect = "none")
                             }(a.view), yr(a), n = !1, t = a.clientX, e = a.clientY, l("start", a))
@@ -3356,88 +3358,97 @@
                             o = i.length;
                         for (r && clearTimeout(r), r = setTimeout((function() {
                                 r = null
                             }), 500), e = 0; e < o; ++e)(n = l[i[e].identifier]) && (yr(t), n("end", t, i[e]))
                     }
 
                     function y(t, e, n, r, i, o) {
-                        var s, h, d, p = u.copy(),
+                        var s, h, f, p = u.copy(),
                             m = _r(o || n, e);
-                        if (null != (d = a.call(t, new br("beforestart", {
+                        if (null != (f = a.call(t, new br("beforestart", {
                                 sourceEvent: n,
-                                target: f,
+                                target: d,
                                 identifier: i,
                                 active: c,
                                 x: m[0],
                                 y: m[1],
                                 dx: 0,
                                 dy: 0,
                                 dispatch: p
-                            }), r))) return s = d.x - m[0] || 0, h = d.y - m[1] || 0,
+                            }), r))) return s = f.x - m[0] || 0, h = f.y - m[1] || 0,
                             function n(o, a, u) {
                                 var _, g = m;
                                 switch (o) {
                                     case "start":
                                         l[i] = n, _ = c++;
                                         break;
                                     case "end":
                                         delete l[i], --c;
                                     case "drag":
                                         m = _r(u || a, e), _ = c
                                 }
                                 p.call(o, t, new br(o, {
                                     sourceEvent: a,
-                                    subject: d,
-                                    target: f,
+                                    subject: f,
+                                    target: d,
                                     identifier: i,
                                     active: _,
                                     x: m[0] + s,
                                     y: m[1] + h,
                                     dx: m[0] - g[0],
                                     dy: m[1] - g[1],
                                     dispatch: p
                                 }), r)
                             }
                     }
-                    return f.filter = function(t) {
-                        return arguments.length ? (i = "function" == typeof t ? t : xr(!!t), f) : i
-                    }, f.container = function(t) {
-                        return arguments.length ? (o = "function" == typeof t ? t : xr(t), f) : o
-                    }, f.subject = function(t) {
-                        return arguments.length ? (a = "function" == typeof t ? t : xr(t), f) : a
-                    }, f.touchable = function(t) {
-                        return arguments.length ? (s = "function" == typeof t ? t : xr(!!t), f) : s
-                    }, f.on = function() {
+                    return d.filter = function(t) {
+                        return arguments.length ? (i = "function" == typeof t ? t : xr(!!t), d) : i
+                    }, d.container = function(t) {
+                        return arguments.length ? (o = "function" == typeof t ? t : xr(t), d) : o
+                    }, d.subject = function(t) {
+                        return arguments.length ? (a = "function" == typeof t ? t : xr(t), d) : a
+                    }, d.touchable = function(t) {
+                        return arguments.length ? (s = "function" == typeof t ? t : xr(!!t), d) : s
+                    }, d.on = function() {
                         var t = u.on.apply(u, arguments);
-                        return t === u ? f : t
-                    }, f.clickDistance = function(t) {
-                        return arguments.length ? (h = (t = +t) * t, f) : Math.sqrt(h)
-                    }, f
+                        return t === u ? d : t
+                    }, d.clickDistance = function(t) {
+                        return arguments.length ? (h = (t = +t) * t, d) : Math.sqrt(h)
+                    }, d
                 }().on("start", (function() {
                     c = [], s(), mr(t).select("svg").append("path").attr("id", "lasso" + u)
                 })).on("drag", (function(t) {
                     let e = t.sourceEvent.offsetX,
                         n = t.sourceEvent.offsetY;
                     c.push([e, n]), mr("#lasso" + u).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", h(c))
                 })).on("end", (function() {
                     let t = [];
-                    f.each(((s, l) => {
+                    d.each(((s, l) => {
                         (function(t, e) {
                             for (var n = t[0], r = t[1], i = !1, o = 0, a = e.length - 1; o < e.length; a = o++) {
                                 var s = e[o][0],
                                     l = e[o][1],
                                     u = e[a][0],
                                     c = e[a][1];
                                 l > r != c > r && n < (u - s) * (r - l) / (c - l) + s && (i = !i)
                             }
                             return i
                         })([e(s[r]) + o, n(s[i]) + a], c) && (mr("#dot-" + u + s.id).style("fill", "red").attr("r", 6), t.push(s))
                     })), mr("#lasso" + u).remove(), l(t)
                 }));
-            mr(t).call(d)
+            mr(t).call(f)
+        }
+
+        function Si(t, e) {
+            return t.reduce((function(t, n) {
+                return {
+                    ...t,
+                    [n[e]]: [...t[n[e]] ?? [], n]
+                }
+            }), {})
         }
         ki.prototype = {
             constructor: ki,
             scale: function(t) {
                 return 1 === t ? this : new ki(this.k * t, this.x, this.y)
             },
             translate: function(t, e) {
@@ -3468,93 +3479,93 @@
                 return t.copy().domain(t.range().map(this.invertY, this).map(t.invert, t))
             },
             toString: function() {
                 return "translate(" + this.x + "," + this.y + ") scale(" + this.k + ")"
             }
         }, new ki(1, 0, 0), ki.prototype;
         const Ni = i(330),
-            Si = 400,
-            $i = {
+            $i = 400,
+            Vi = {
                 top: 20,
                 right: 20,
                 bottom: 30,
                 left: 40
             };
 
-        function Ci(t) {
+        function ji(t) {
             t.timeout && clearTimeout(t.timeout), t.timeout = setTimeout((() => {
                 t.plot()
             }), 100)
         }
-        class Ti extends t.DOMWidgetModel {
+        class Ci extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Ti.model_name,
-                    _view_name: Ti.view_name,
-                    _model_module: Ti.model_module,
-                    _view_module: Ti.view_module,
-                    _model_module_version: Ti.model_module_version,
-                    _view_module_version: Ti.view_module_version,
+                    _model_name: Ci.model_name,
+                    _view_name: Ci.view_name,
+                    _model_module: Ci.model_module,
+                    _view_module: Ci.view_module,
+                    _model_module_version: Ci.model_module_version,
+                    _view_module_version: Ci.view_module_version,
                     linearData_x: [],
                     linearData_y: [],
                     histogramData: [],
                     elementId: String,
                     clickedValue: String
                 }
             }
             static model_name = "LinearHistPlotModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "LinearHistPlotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class ji extends t.DOMWidgetView {
+        class Ti extends t.DOMWidgetView {
             timeout;
             render() {
-                Ci(this), this.model.on("change:linearData_x", (() => Ci(this)), this), this.model.on("change:linearData_y", (() => Ci(this)), this), this.model.on("change:histogramData", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                ji(this), this.model.on("change:linearData_x", (() => ji(this)), this), this.model.on("change:linearData_y", (() => ji(this)), this), this.model.on("change:histogramData", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
             }
             plot() {
                 const t = this.model.get("linearData_x"),
                     e = this.model.get("linearData_y"),
                     n = this.model.get("histogramData"),
                     r = this.model.get("elementId");
-                let i = Si,
+                let i = $i,
                     o = this.el;
                 r && (o = document.getElementById(r), i = o.clientHeight);
                 let a = o.clientWidth;
-                const s = $i;
+                const s = Vi;
                 ! function(t, e, n, r, i, o, a, s) {
                     const l = o - s.left - s.right,
                         u = a - s.top - s.bottom,
                         c = u / 4;
                     mr(r).selectAll("*").remove();
-                    const h = Math.min(I(t), I(n)),
-                        f = Math.max(D(t), D(n)),
-                        d = ai().range([0, l]),
+                    const h = Math.min(R(t), R(n)),
+                        d = Math.max(D(t), D(n)),
+                        f = ai().range([0, l]),
                         p = ai().range([u, 0]),
                         m = ai().range([c, 0]),
-                        _ = Z(d),
+                        _ = Z(f),
                         v = K(p),
                         y = L().thresholds(20).value((t => Math.round(10 * t) / 10))(n),
                         w = mr(r).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
-                    d.domain([h, f]), p.domain(g(e)), m.domain([0, D(y, (t => t.length))]);
+                    f.domain([h, d]), p.domain(g(e)), m.domain([0, D(y, (t => t.length))]);
                     const x = w.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
                         b = w.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
                     w.append("g").attr("transform", "translate(0," + u + ")").call(_).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), w.append("g").call(v).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end");
                     const M = [];
                     M.x0 = y[0].x0 - 2.5, M.x1 = y[0].x1 - 2.5, y.unshift(M);
                     const k = [];
-                    k.x0 = y[y.length - 1].x0 + 2.5, k.x1 = y[y.length - 1].x1 + 2.5, w.append("path").datum(y).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", yi().x((t => d((t.x1 + t.x0) / 2))).y((t => m(t.length) + u - c)).curve(Mi));
+                    k.x0 = y[y.length - 1].x0 + 2.5, k.x1 = y[y.length - 1].x1 + 2.5, w.append("path").datum(y).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", yi().x((t => f((t.x1 + t.x0) / 2))).y((t => m(t.length) + u - c)).curve(Mi));
                     const A = t.map(((t, n) => [t, e[n]])).map((([t, e]) => ({
                         x: t,
                         y: e
                     })));
-                    w.append("path").datum(A).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", yi().x((t => d(t.x))).y((t => p(t.y)))), w.selectAll("myCircles").data(A).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (t => d(t.x))).attr("cy", (t => p(t.y))).attr("r", 3).on("mouseover", (function(t, e) {
+                    w.append("path").datum(A).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", yi().x((t => f(t.x))).y((t => p(t.y)))), w.selectAll("myCircles").data(A).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (t => f(t.x))).attr("cy", (t => p(t.y))).attr("r", 3).on("mouseover", (function(t, e) {
                         x.style("opacity", 1), b.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), b.html("x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
                     })).on("mouseout", (function() {
                         x.style("opacity", 0), b.style("opacity", 0)
                     })).on("click", (function(t, e) {
                         const n = "x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10;
                         void 0 !== i && i(n)
                     }))
@@ -3562,100 +3573,243 @@
             }
             setValue(t) {
                 this.model.set({
                     clickedValue: t
                 }), this.model.save_changes()
             }
         }
-        class Oi extends t.DOMWidgetModel {
+        class Pi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Oi.model_name,
-                    _view_name: Oi.view_name,
-                    _model_module: Oi.model_module,
-                    _view_module: Oi.view_module,
-                    _model_module_version: Oi.model_module_version,
-                    _view_module_version: Oi.view_module_version,
+                    _model_name: Pi.model_name,
+                    _view_name: Pi.view_name,
+                    _model_module: Pi.model_module,
+                    _view_module: Pi.view_module,
+                    _model_module_version: Pi.model_module_version,
+                    _view_module_version: Pi.view_module_version,
                     dataRecords: [],
                     x: String,
                     y: String,
                     hue: String,
                     elementId: String,
                     clickedValue: String,
                     selectedValuesRecords: []
                 }
             }
-            static model_name = "ScatterplotModel";
+            static model_name = "ScatterPlotModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
-            static view_name = "ScatterplotView";
+            static view_name = "ScatterPlotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class Pi extends t.DOMWidgetView {
+        class Oi extends t.DOMWidgetView {
             timeout;
             render() {
-                Ci(this), this.model.on("change:dataRecords", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:y", (() => Ci(this)), this), this.model.on("change:hue", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:x", (() => ji(this)), this), this.model.on("change:y", (() => ji(this)), this), this.model.on("change:hue", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
                     r = this.model.get("hue"),
                     i = this.model.get("elementId");
-                let o = Si,
+                let o = $i,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight);
                 let s = a.clientWidth;
-                const l = $i;
+                const l = Vi;
                 ! function(t, e, n, r, i, o, a, s, l, u) {
                     const c = s - u.left - u.right,
                         h = l - u.top - u.bottom;
                     for (let e = 0; e < t.length; e++) t[e].id = e;
-                    const f = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                    const d = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
                     mr(i).selectAll("*").remove();
-                    const d = ai().range([0, c]),
+                    const f = ai().range([0, c]),
                         p = ai().range([h, 0]),
-                        m = jr(si),
-                        _ = Z(d),
+                        m = Cr(si),
+                        _ = Z(f),
                         v = K(p),
                         y = mr(i).append("svg").attr("width", s).attr("height", l).append("g").attr("transform", "translate(" + u.left + "," + u.top + ")");
-                    d.domain(g(t, (function(t) {
-                        return t[e]
-                    }))).nice(), p.domain(g(t, (function(t) {
-                        return t[n]
-                    }))).nice(), y.append("g").attr("class", "x axis").attr("transform", "translate(0," + h + ")").call(_).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), y.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.selectAll(".dot").data(t).enter().append("circle").attr("id", (function(t, e) {
-                        return "dot-" + f + t.id
-                    })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(t) {
-                        return d(t[e])
-                    })).attr("cy", (function(t) {
-                        return p(t[n])
-                    })).style("fill", (function(t) {
-                        return m(t[r])
-                    })).on("mouseover", (function(t, r) {
-                        x.style("opacity", 1), b.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), b.html("x: " + Math.round(10 * r[e]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * r[n]) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
-                    })).on("mouseout", (function() {
-                        x.style("opacity", 0), b.style("opacity", 0)
-                    })).on("click", (function(t, r) {
-                        const i = "x:" + Math.round(10 * r[e]) / 10 + "    y:" + Math.round(10 * r[n]) / 10;
-                        void 0 !== o && o(i)
-                    })), Ei(i, d, p, e, n, u.left, u.top, (function() {
-                        y.selectAll(".dot").data(t).attr("r", 3.5).style("fill", (function(t) {
+                    if (f.domain(g(t, (function(t) {
+                            return t[e]
+                        }))).nice(), p.domain(g(t, (function(t) {
+                            return t[n]
+                        }))).nice(), y.append("g").attr("class", "x axis").attr("transform", "translate(0," + h + ")").call(_).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), y.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.selectAll(".dot").data(t).enter().append("circle").attr("id", (function(t, e) {
+                            return "dot-" + d + t.id
+                        })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(t) {
+                            return f(t[e])
+                        })).attr("cy", (function(t) {
+                            return p(t[n])
+                        })).style("fill", (function(t) {
                             return m(t[r])
+                        })).on("mouseover", (function(t, r) {
+                            w.style("opacity", 1), x.style("opacity", 1), w.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), x.html("x: " + Math.round(10 * r[e]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * r[n]) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
+                        })).on("mouseout", (function() {
+                            w.style("opacity", 0), x.style("opacity", 0)
+                        })).on("click", (function(t, r) {
+                            const i = "x:" + Math.round(10 * r[e]) / 10 + "    y:" + Math.round(10 * r[n]) / 10;
+                            void 0 !== o && o(i)
+                        })), Ei(i, f, p, e, n, u.left, u.top, (function() {
+                            y.selectAll(".dot").data(t).attr("r", 3.5).style("fill", (function(t) {
+                                return m(t[r])
+                            }))
+                        }), (function(t) {
+                            void 0 !== a && a(t)
+                        }), d), r) {
+                        const t = y.selectAll(".legend").data(m.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
+                            return "translate(0," + 20 * e + ")"
+                        }));
+                        t.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", m), t.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
+                            return t
                         }))
-                    }), (function(t) {
-                        void 0 !== a && a(t)
-                    }), f);
-                    const w = y.selectAll(".legend").data(m.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
-                        return "translate(0," + 20 * e + ")"
-                    }));
-                    w.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", m), w.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
-                        return t
-                    }));
+                    }
+                    const w = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                        x = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
+                }(t, e, n, r, a, this.setValue.bind(this), this.setSelectedValues.bind(this), s, o, l)
+            }
+            setValue(t) {
+                this.model.set({
+                    clickedValue: t
+                }), this.model.save_changes()
+            }
+            setSelectedValues(t) {
+                this.model.set({
+                    selectedValuesRecords: t
+                }), this.model.save_changes()
+            }
+        }
+        class Li extends t.DOMWidgetModel {
+            defaults() {
+                return {
+                    ...super.defaults(),
+                    _model_name: Li.model_name,
+                    _view_name: Li.view_name,
+                    _model_module: Li.model_module,
+                    _view_module: Li.view_module,
+                    _model_module_version: Li.model_module_version,
+                    _view_module_version: Li.view_module_version,
+                    dataRecords: [],
+                    x: String,
+                    y: String,
+                    hue: String,
+                    elementId: String,
+                    clickedValue: String,
+                    selectedValuesRecords: []
+                }
+            }
+            static model_name = "LinearPlotModel";
+            static model_module = Ni.name;
+            static model_module_version = Ni.version;
+            static view_name = "LinearPlotView";
+            static view_module = Ni.name;
+            static view_module_version = Ni.version
+        }
+        class Di extends t.DOMWidgetView {
+            timeout;
+            render() {
+                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:x", (() => ji(this)), this), this.model.on("change:y", (() => ji(this)), this), this.model.on("change:hue", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
+            }
+            plot() {
+                const t = this.model.get("dataRecords"),
+                    e = this.model.get("x"),
+                    n = this.model.get("y"),
+                    r = this.model.get("hue"),
+                    i = this.model.get("elementId");
+                let o = $i,
+                    a = this.el;
+                i && (a = document.getElementById(i), o = a.clientHeight);
+                let s = a.clientWidth;
+                const l = Vi;
+                ! function(t, e, n, r, i, o, a, s, l, u) {
+                    const c = s - u.left - u.right,
+                        h = l - u.top - u.bottom;
+                    t = function(t, e, n, r) {
+                        function i(t) {
+                            const i = t.reduce((function(t, i) {
+                                    if (!t[i[e]]) {
+                                        const o = {};
+                                        return o[e] = i[e], o[n] = i[n], r && (o[r] = i[r]), o.count = 1, t[i[e]] = o, t
+                                    }
+                                    return t[i[e]][n] += i[n], t[i[e]].count += 1, t
+                                }), {}),
+                                o = Object.keys(i).map((function(t) {
+                                    const e = i[t],
+                                        r = {};
+                                    return r[n] = e[n] / e.count, {
+                                        ...e,
+                                        ...r
+                                    }
+                                }));
+                            return o.sort((s = 1, "-" === (a = e)[0] && (s = -1, a = a.substr(1)), function(t, e) {
+                                return (t[a] < e[a] ? -1 : t[a] > e[a] ? 1 : 0) * s
+                            })), o;
+                            var a, s
+                        }
+                        if (!r) return i(t);
+                        let o = Si(t, r),
+                            a = [];
+                        return Object.values(o).forEach((function(t, e) {
+                            const n = i(t);
+                            a = a.concat(n)
+                        })), a
+                    }(t, e, [n], r);
+                    for (let e = 0; e < t.length; e++) t[e].id = e;
+                    const d = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                    mr(i).selectAll("*").remove();
+                    const f = ai().range([0, c]),
+                        p = ai().range([h, 0]),
+                        m = Cr(si),
+                        _ = Z(f),
+                        v = K(p),
+                        y = mr(i).append("svg").attr("width", s).attr("height", l).append("g").attr("transform", "translate(" + u.left + "," + u.top + ")");
+
+                    function w(t, r) {
+                        y.append("path").datum(t).attr("fill", "none").attr("stroke", m(r)).attr("stroke-width", 2).attr("d", yi().x((t => f(t[e]))).y((t => p(t[n]))))
+                    }
+                    if (f.domain(g(t, (function(t) {
+                            return t[e]
+                        }))).nice(), p.domain(g(t, (function(t) {
+                            return t[n]
+                        }))).nice(), y.append("g").attr("class", "x axis").attr("transform", "translate(0," + h + ")").call(_).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), y.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), r) {
+                        const e = Si(t, r);
+                        Object.keys(e).forEach((function(t, n) {
+                            w(e[t], t)
+                        }))
+                    } else w(t);
+                    if (y.selectAll(".dot").data(t).enter().append("circle").attr("id", (function(t, e) {
+                            return "dot-" + d + t.id
+                        })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(t) {
+                            return f(t[e])
+                        })).attr("cy", (function(t) {
+                            return p(t[n])
+                        })).style("fill", (function(t) {
+                            return m(t[r])
+                        })).on("mouseover", (function(t, r) {
+                            x.style("opacity", 1), b.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), b.html("x: " + Math.round(10 * r[e]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * r[n]) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
+                        })).on("mouseout", (function() {
+                            x.style("opacity", 0), b.style("opacity", 0)
+                        })).on("click", (function(t, r) {
+                            const i = "x:" + Math.round(10 * r[e]) / 10 + "    y:" + Math.round(10 * r[n]) / 10;
+                            void 0 !== o && o(i)
+                        })), Ei(i, f, p, e, n, u.left, u.top, (function() {
+                            y.selectAll(".dot").data(t).attr("r", 3.5).style("fill", (function(t) {
+                                return m(t[r])
+                            }))
+                        }), (function(t) {
+                            void 0 !== a && a(t)
+                        }), d), r) {
+                        const t = y.selectAll(".legend").data(m.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
+                            return "translate(0," + 20 * e + ")"
+                        }));
+                        t.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", m), t.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
+                            return t
+                        }))
+                    }
                     const x = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
                         b = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
                 }(t, e, n, r, a, this.setValue.bind(this), this.setSelectedValues.bind(this), s, o, l)
             }
             setValue(t) {
                 this.model.set({
                     clickedValue: t
@@ -3663,158 +3817,158 @@
             }
             setSelectedValues(t) {
                 this.model.set({
                     selectedValuesRecords: t
                 }), this.model.save_changes()
             }
         }
-        class Vi extends t.DOMWidgetModel {
+        class Ri extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Vi.model_name,
-                    _view_name: Vi.view_name,
-                    _model_module: Vi.model_module,
-                    _view_module: Vi.view_module,
-                    _model_module_version: Vi.model_module_version,
-                    _view_module_version: Vi.view_module_version,
+                    _model_name: Ri.model_name,
+                    _view_name: Ri.view_name,
+                    _model_module: Ri.model_module,
+                    _view_module: Ri.view_module,
+                    _model_module_version: Ri.model_module_version,
+                    _view_module_version: Ri.view_module_version,
                     dataRecords: [],
                     x: String,
                     y: String,
                     hue: String,
                     elementId: String
                 }
             }
             static model_name = "BarplotModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "BarplotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class Li extends t.DOMWidgetView {
+        class Ii extends t.DOMWidgetView {
             timeout;
             render() {
-                Ci(this), this.model.on("change:dataRecords", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:y", (() => Ci(this)), this), this.model.on("change:hue", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:x", (() => ji(this)), this), this.model.on("change:y", (() => ji(this)), this), this.model.on("change:hue", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
                     r = this.model.get("hue"),
                     i = this.model.get("elementId");
-                let o = Si,
+                let o = $i,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
                     function(t, e, n, r, i, o, a, s) {
                         const l = o - s.left - s.right,
                             u = a - s.top - s.bottom;
                         mr(i).selectAll("*").remove();
                         const c = mr(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
                         r || (r = e);
                         const h = t.reduce(((t, e) => (t && -1 === t.indexOf(e[r]) && t.push(e[r]), t)), []),
-                            f = {},
-                            d = jr(si);
+                            d = {},
+                            f = Cr(si);
                         r == e ? function() {
                             let r = t.reduce(((t, r) => {
                                 const i = r[e],
                                     o = r[n];
-                                if (i in t) t[i] += o, f[i].qt += 1, f[i][n].push(o);
+                                if (i in t) t[i] += o, d[i].qt += 1, d[i][n].push(o);
                                 else {
                                     const e = {
                                         qt: 1
                                     };
-                                    e[n] = [], e[n].push(o), f[i] = e, t[i] = o
+                                    e[n] = [], e[n].push(o), d[i] = e, t[i] = o
                                 }
                                 return t
                             }), {});
                             r = Object.keys(r).map((t => {
                                 const i = {};
-                                return i[e] = t, i[n] = r[t], 0 != f[t].qt && (i[n] = i[n] / f[t].qt), i
-                            })), Object.keys(f).forEach((t => {
-                                const e = f[t][n],
+                                return i[e] = t, i[n] = r[t], 0 != d[t].qt && (i[n] = i[n] / d[t].qt), i
+                            })), Object.keys(d).forEach((t => {
+                                const e = d[t][n],
                                     [r, i] = Ai(e);
-                                f[t].min = r, f[t].max = i
+                                d[t].min = r, d[t].max = i
                             }));
                             const i = r.map((t => t[e])),
                                 o = [],
-                                a = Object.keys(f).map((t => f[t]));
-                            o.push(I(a, (t => t.min))), o.push(D(a, (t => t.max))), o[0] > 0 && o[1] > 0 ? o[0] = 0 : o[0] < 0 && o[1] < 0 && (o[1] = 0);
+                                a = Object.keys(d).map((t => d[t]));
+                            o.push(R(a, (t => t.min))), o.push(D(a, (t => t.max))), o[0] > 0 && o[1] > 0 ? o[0] = 0 : o[0] < 0 && o[1] < 0 && (o[1] = 0);
                             const s = ai().domain(o).range([u, 0]);
                             c.append("g").call(K(s));
-                            const p = Or().domain(i).range([0, l]).padding([.2]);
+                            const p = Tr().domain(i).range([0, l]).padding([.2]);
                             c.append("g").selectAll("g").data(r).enter().append("rect").attr("x", (function(t) {
                                 return p(t[e])
                             })).attr("y", (function(t) {
                                 return s(t[n]) < s(0) ? s(t[n]) : s(0)
                             })).attr("width", p.bandwidth()).attr("height", (function(t) {
                                 return Math.abs(s(0) - s(t[n]))
                             })).data(h).attr("fill", (function(t) {
-                                return d(t)
+                                return f(t)
                             }));
-                            const m = Object.keys(f).map((t => {
+                            const m = Object.keys(d).map((t => {
                                 const n = {};
-                                return n[e] = t, n.min = f[t].min, n.max = f[t].max, n
+                                return n[e] = t, n.min = d[t].min, n.max = d[t].max, n
                             }));
                             c.append("g").selectAll("g").data(m).enter().append("rect").attr("x", (function(t) {
                                 return p(t[e]) + p.bandwidth() / 2 - 1
                             })).attr("y", (function(t) {
                                 return s(t.max)
                             })).attr("width", 2).attr("height", (function(t) {
                                 return s(t.min) - s(t.max)
                             })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + s(0) + ")").call(Z(p).tickSize(0))
                         }() : function() {
                             let i = t.reduce(((t, i) => {
                                 const o = i[e],
                                     a = i[n],
                                     s = i[r];
                                 if (o in t) {
-                                    f[o].qt[n + "-" + s] += 1, f[o][s][n].push(a);
+                                    d[o].qt[n + "-" + s] += 1, d[o][s][n].push(a);
                                     for (const e of h) s == e && (t[o][n + "-" + e] += a)
                                 } else {
                                     const e = {};
                                     h.forEach((t => {
                                         e[t] = {}, e[t][n] = []
                                     }));
                                     const r = {};
                                     for (const t of h) r[n + "-" + t] = 0;
-                                    r[n + "-" + s] = 1, e.qt = r, e[s][n].push(a), f[o] = e;
+                                    r[n + "-" + s] = 1, e.qt = r, e[s][n].push(a), d[o] = e;
                                     const i = {};
                                     for (const t of h) i[n + "-" + t] = s == t ? a : 0;
                                     t[o] = i
                                 }
                                 return t
                             }), {});
                             i = Object.keys(i).map((t => {
                                 let n = {};
                                 n[e] = t;
-                                for (const e of Object.keys(i[t])) 0 != f[t].qt[e] && (i[t][e] = i[t][e] / f[t].qt[e]);
+                                for (const e of Object.keys(i[t])) 0 != d[t].qt[e] && (i[t][e] = i[t][e] / d[t].qt[e]);
                                 return n = {
                                     ...n,
                                     ...i[t]
                                 }, n
-                            })), Object.keys(f).forEach((t => {
+                            })), Object.keys(d).forEach((t => {
                                 h.forEach((e => {
-                                    const r = f[t][e][n],
+                                    const r = d[t][e][n],
                                         [i, o] = Ai(r);
-                                    f[t][e].min = i, f[t][e].max = o
+                                    d[t][e].min = i, d[t][e].max = o
                                 }))
                             }));
                             const o = h.map((t => n + "-" + t)),
                                 a = i.map((t => t[e])),
                                 s = [];
-                            Object.keys(f).map((t => {
-                                h.forEach((e => s.push(f[t][e])))
+                            Object.keys(d).map((t => {
+                                h.forEach((e => s.push(d[t][e])))
                             }));
                             const p = [];
-                            p.push(I(s, (t => t.min))), p.push(D(s, (t => t.max))), p[0] > 0 && p[1] > 0 ? p[0] = 0 : p[0] < 0 && p[1] < 0 && (p[1] = 0);
+                            p.push(R(s, (t => t.min))), p.push(D(s, (t => t.max))), p[0] > 0 && p[1] > 0 ? p[0] = 0 : p[0] < 0 && p[1] < 0 && (p[1] = 0);
                             const m = ai().domain(p).range([u, 0]);
                             c.append("g").call(K(m));
-                            const _ = Or().domain(a).range([0, l]).padding([.2]),
-                                g = Or().domain(o).range([0, _.bandwidth()]).padding([.05]);
+                            const _ = Tr().domain(a).range([0, l]).padding([.2]),
+                                g = Tr().domain(o).range([0, _.bandwidth()]).padding([.05]);
                             c.append("g").selectAll("g").data(i).enter().append("g").attr("transform", (function(t) {
                                 return "translate(" + _(t[e]) + ",0)"
                             })).selectAll("rect").data((function(t) {
                                 return o.map((function(e) {
                                     return {
                                         key: e,
                                         value: t[e]
@@ -3823,21 +3977,21 @@
                             })).enter().append("rect").attr("x", (function(t) {
                                 return g(t.key)
                             })).attr("y", (function(t) {
                                 return m(t.value) < m(0) ? m(t.value) : m(0)
                             })).attr("width", g.bandwidth()).attr("height", (function(t) {
                                 return Math.abs(m(0) - m(t.value))
                             })).data(h).attr("fill", (function(t) {
-                                return d(t)
+                                return f(t)
                             }));
-                            const v = Object.keys(f).map((t => {
+                            const v = Object.keys(d).map((t => {
                                 let n = {};
                                 return n[e] = t, n = {
                                     ...n,
-                                    ...f[t]
+                                    ...d[t]
                                 }, n
                             }));
                             c.append("g").selectAll("g").data(v).enter().append("g").attr("transform", (function(t) {
                                 return "translate(" + _(t[e]) + ",0)"
                             })).selectAll("rect").data((function(t) {
                                 return h.map((function(e) {
                                     return {
@@ -3848,104 +4002,104 @@
                             })).enter().append("rect").attr("x", (function(t) {
                                 return g(t.key) + g.bandwidth() / 2 - 1
                             })).attr("y", (function(t) {
                                 return t.value.max ? m(t.value.max) : 0
                             })).attr("width", 2).attr("height", (function(t) {
                                 return t.value.min && t.value.max ? m(t.value.min) - m(t.value.max) : 0
                             }));
-                            const y = c.selectAll(".legend").data(d.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
+                            const y = c.selectAll(".legend").data(f.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
                                 return "translate(0," + 20 * e + ")"
                             }));
-                            y.append("rect").attr("x", l - 18).attr("width", 18).attr("height", 18).style("fill", d), y.append("text").attr("x", l - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
+                            y.append("rect").attr("x", l - 18).attr("width", 18).attr("height", 18).style("fill", f), y.append("text").attr("x", l - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
                                 return t
                             })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + m(0) + ")").call(Z(_).tickSize(0))
                         }()
-                    }(t, e, n, r, a, a.clientWidth, o, $i)
+                    }(t, e, n, r, a, a.clientWidth, o, Vi)
             }
         }
-        class Di extends t.DOMWidgetModel {
+        class qi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Di.model_name,
-                    _view_name: Di.view_name,
-                    _model_module: Di.model_module,
-                    _view_module: Di.view_module,
-                    _model_module_version: Di.model_module_version,
-                    _view_module_version: Di.view_module_version,
+                    _model_name: qi.model_name,
+                    _view_name: qi.view_name,
+                    _model_module: qi.model_module,
+                    _view_module: qi.view_module,
+                    _model_module_version: qi.model_module_version,
+                    _view_module_version: qi.view_module_version,
                     dataRecords: [],
                     x: String,
                     start: Number,
                     end: Number,
                     elementId: String
                 }
             }
             static model_name = "HistogramplotModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "HistogramplotView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class Ii extends t.DOMWidgetView {
+        class Hi extends t.DOMWidgetView {
             timeout;
             render() {
-                Ci(this), this.model.on("change:dataRecords", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:start", (() => Ci(this)), this), this.model.on("change:end", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:x", (() => ji(this)), this), this.model.on("change:start", (() => ji(this)), this), this.model.on("change:end", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("x"),
                     n = this.model.get("start"),
                     r = this.model.get("end"),
                     i = this.model.get("elementId");
-                let o = Si,
+                let o = $i,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
                     function(t, e, n, r, i, o, a, s) {
                         const l = o - s.left - s.right,
                             u = a - s.top - s.bottom;
                         mr(i).selectAll("*").remove();
                         let c = n;
-                        n || (c = I(t, (t => t[e])));
+                        n || (c = R(t, (t => t[e])));
                         let h = r;
                         r || (h = D(t, (t => t[e])));
-                        const f = ai().range([0, l]),
-                            d = ai().range([u, 0]),
-                            p = Z(f),
-                            m = K(d),
+                        const d = ai().range([0, l]),
+                            f = ai().range([u, 0]),
+                            p = Z(d),
+                            m = K(f),
                             _ = L().thresholds(40).value((t => Math.round(10 * t[e]) / 10))(t),
                             g = mr(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
-                        f.domain([c, h]), d.domain([0, D(_, (t => t.length))]), g.append("g").attr("transform", "translate(0," + u + ")").call(p).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), g.append("g").call(m).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), g.append("g").attr("fill", "steelblue").selectAll().data(_).join("rect").attr("x", (t => f(t.x0) + 1)).attr("width", (t => f(t.x1) - f(t.x0) - 1)).attr("y", (t => d(t.length))).attr("height", (t => d(0) - d(t.length)))
-                    }(t, e, n, r, a, a.clientWidth, o, $i)
+                        d.domain([c, h]), f.domain([0, D(_, (t => t.length))]), g.append("g").attr("transform", "translate(0," + u + ")").call(p).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), g.append("g").call(m).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), g.append("g").attr("fill", "steelblue").selectAll().data(_).join("rect").attr("x", (t => d(t.x0) + 1)).attr("width", (t => d(t.x1) - d(t.x0) - 1)).attr("y", (t => f(t.length))).attr("height", (t => f(0) - f(t.length)))
+                    }(t, e, n, r, a, a.clientWidth, o, Vi)
             }
         }
-        class Ri extends t.DOMWidgetModel {
+        class zi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Ri.model_name,
-                    _view_name: Ri.view_name,
-                    _model_module: Ri.model_module,
-                    _view_module: Ri.view_module,
-                    _model_module_version: Ri.model_module_version,
-                    _view_module_version: Ri.view_module_version,
+                    _model_name: zi.model_name,
+                    _view_name: zi.view_name,
+                    _model_module: zi.model_module,
+                    _view_module: zi.view_module,
+                    _model_module_version: zi.model_module_version,
+                    _view_module_version: zi.view_module_version,
                     matrix: [],
                     grid_areas: [],
                     grid_template_areas: String,
                     style: String
                 }
             }
             static model_name = "EmbeddingModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "EmbeddingView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class qi extends t.DOMWidgetView {
+        class Xi extends t.DOMWidgetView {
             render() {
                 this.value_changed()
             }
             value_changed() {
                 const t = this.model.get("matrix"),
                     e = this.model.get("grid_areas"),
                     n = this.model.get("grid_template_areas");
@@ -3954,24 +4108,24 @@
                 const i = document.createElement("div");
                 i.classList.add(r), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + t.length + ", 180px)", i.style.gridTemplateColumns = "repeat(" + t[0].length + ", 1fr)", i.style.width = "100%", e.forEach((t => {
                     const e = document.createElement("div");
                     e.setAttribute("id", t), e.style.gridArea = t, e.classList.add("dashboard-div"), i.appendChild(e)
                 })), this.el.appendChild(i)
             }
         }
-        class Hi extends t.DOMWidgetModel {
+        class Yi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Hi.model_name,
-                    _view_name: Hi.view_name,
-                    _model_module: Hi.model_module,
-                    _view_module: Hi.view_module,
-                    _model_module_version: Hi.model_module_version,
-                    _view_module_version: Hi.view_module_version,
+                    _model_name: Yi.model_name,
+                    _view_name: Yi.view_name,
+                    _model_module: Yi.model_module,
+                    _view_module: Yi.view_module,
+                    _model_module_version: Yi.model_module_version,
+                    _view_module_version: Yi.view_module_version,
                     dataRecords: [],
                     variable: String,
                     step: Number,
                     description: String,
                     minValue: Number,
                     maxValue: Number,
                     elementId: String
@@ -3980,49 +4134,49 @@
             static model_name = "RangeSliderModel";
             static model_module = Ni.name;
             static model_module_version = Ni.version;
             static view_name = "RangeSliderView";
             static view_module = Ni.name;
             static view_module_version = Ni.version
         }
-        class zi extends t.DOMWidgetView {
+        class Bi extends t.DOMWidgetView {
             render() {
-                Ci(this), this.model.on("change:dataRecords", (() => Ci(this)), this), this.model.on("change:variable", (() => Ci(this)), this), this.model.on("change:step", (() => Ci(this)), this), this.model.on("change:description", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+                ji(this), this.model.on("change:dataRecords", (() => ji(this)), this), this.model.on("change:variable", (() => ji(this)), this), this.model.on("change:step", (() => ji(this)), this), this.model.on("change:description", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this)))
             }
             plot() {
                 const t = this.model.get("dataRecords"),
                     e = this.model.get("variable"),
                     n = this.model.get("step"),
                     r = this.model.get("description"),
                     i = this.model.get("elementId"),
                     o = this.model.get("minValue"),
                     a = this.model.get("maxValue");
                 let s = this.el;
                 i && (s = document.getElementById(i));
-                const l = $i;
+                const l = Vi;
                 ! function(t, e, n, r, i, o, a, s, l) {
                     const u = document.createElement("div");
                     u.classList.add("range_outside_container"), u.style.margin = l.top + "px " + l.right + "px " + l.bottom + "px " + l.left + "px";
                     const c = document.createElement("span");
                     c.classList.add("range_description"), c.textContent = r, u.appendChild(c);
                     const h = document.createElement("div");
                     h.classList.add("range_inside_container"), u.appendChild(h);
-                    const f = document.createElement("span");
-                    f.classList.add("range_value"), u.appendChild(f);
-                    const d = document.createElement("div");
-                    d.classList.add("sliders_control"), h.appendChild(d);
+                    const d = document.createElement("span");
+                    d.classList.add("range_value"), u.appendChild(d);
+                    const f = document.createElement("div");
+                    f.classList.add("sliders_control"), h.appendChild(f);
                     const p = document.createElement("input");
-                    p.classList.add("top_slider"), p.setAttribute("step", n), p.setAttribute("type", "range"), d.appendChild(p);
+                    p.classList.add("top_slider"), p.setAttribute("step", n), p.setAttribute("type", "range"), f.appendChild(p);
                     const m = document.createElement("input");
 
                     function _(t, e) {
-                        f.textContent = t + " - " + e, a(t, e)
+                        d.textContent = t + " - " + e, a(t, e)
                     }
-                    m.setAttribute("step", n), m.setAttribute("type", "range"), d.appendChild(m);
-                    const g = I(t, (t => t[e])),
+                    m.setAttribute("step", n), m.setAttribute("type", "range"), f.appendChild(m);
+                    const g = R(t, (t => t[e])),
                         v = D(t, (t => t[e]));
                     p.setAttribute("min", g), p.setAttribute("max", v), m.setAttribute("min", g), m.setAttribute("max", v), i && o ? (p.value = i, m.value = o) : (p.value = g, m.value = v), _(parseFloat(p.value), parseFloat(m.value)), p.addEventListener("input", (() => {
                         const t = parseFloat(p.value),
                             e = parseFloat(m.value);
                         t > e && (p.value = m.value), _(t, e)
                     })), m.addEventListener("input", (() => {
                         const t = parseFloat(p.value),
@@ -4039,10 +4193,10 @@
                 this.model.set({
                     minValue: t
                 }), this.model.set({
                     maxValue: e
                 }), this.model.save_changes()
             }
         }
-        var Xi = i(330)
+        var Fi = i(330)
     })(), o
 })()));
```

### Comparing `d3vis_ipynb-0.2.1/js/amd-public-path.js` & `d3vis_ipynb-0.2.2/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/js/package.json` & `d3vis_ipynb-0.2.2/js/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'scripts'": "{delete: ['start:export', 'export']}", "'version'": "'0.2.2'"}*

```diff
@@ -43,16 +43,14 @@
     },
     "scripts": {
         "build": "webpack --mode=development && yarn run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension",
-        "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
-        "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `d3vis_ipynb-0.2.1/js/webpack.config.js` & `d3vis_ipynb-0.2.2/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/js/webpack.exports.config.js` & `d3vis_ipynb-0.2.2/js/webpack.exports.config.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,12 @@
 const path = require("path");
 const HtmlWebpackPlugin = require("html-webpack-plugin");
 
 module.exports = (env) => {
-    let entry = "./lib/web-dev.js"
-    if (env.export) {
-        entry = "./lib/wrappers/embedding.wrapper.js"
-    }
+    let entry = "./lib/web-dev.js";
 
     return {
         mode: "development",
         entry: entry,
         devtool: "inline-source-map",
         devServer: {
             static: "./web-dev",
```

### Comparing `d3vis_ipynb-0.2.1/js/css/widget.css` & `d3vis_ipynb-0.2.2/js/css/widget.css`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/js/lib/labplugin.js` & `d3vis_ipynb-0.2.2/js/lib/labplugin.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -10,14 +10,16 @@
     HistogramPlotView,
     LinearHistPlotModel,
     LinearHistPlotView,
     RangeSliderModel,
     RangeSliderView,
     ScatterPlotModel,
     ScatterPlotView,
+    LinearPlotModel,
+    LinearPlotView,
     version,
 } from "./index";
 
 export const helloWidgetPlugin = {
     id: "d3vis_ipynb:plugin",
     requires: [IJupyterWidgetRegistry],
     activate: function(app, widgets) {
@@ -25,14 +27,16 @@
             name: "d3vis_ipynb",
             version: version,
             exports: {
                 LinearHistPlotModel,
                 LinearHistPlotView,
                 ScatterPlotModel,
                 ScatterPlotView,
+                LinearPlotModel,
+                LinearPlotView,
                 BarPlotModel,
                 BarPlotView,
                 HistogramPlotModel,
                 HistogramPlotView,
                 EmbeddingModel,
                 EmbeddingView,
                 RangeSliderModel,
```

### Comparing `d3vis_ipynb-0.2.1/js/lib/web-dev.js` & `d3vis_ipynb-0.2.2/js/lib/web-dev.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/js/lib/widgets.js` & `d3vis_ipynb-0.2.2/js/lib/widgets.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -9,14 +9,17 @@
 import {
     histogramplot
 } from "./graphs/histogramplot";
 import {
     linearhistplot
 } from "./graphs/linearhistplot";
 import {
+    linearplot
+} from "./graphs/linearplot";
+import {
     rangeslider
 } from "./graphs/rangeslider";
 import {
     scatterplot
 } from "./graphs/scatterplot";
 const packageData = require("../package.json");
 
@@ -129,18 +132,18 @@
             hue: String,
             elementId: String,
             clickedValue: String,
             selectedValuesRecords: [],
         };
     }
 
-    static model_name = "ScatterplotModel";
+    static model_name = "ScatterPlotModel";
     static model_module = packageData.name;
     static model_module_version = packageData.version;
-    static view_name = "ScatterplotView"; // Set to null if no view
+    static view_name = "ScatterPlotView"; // Set to null if no view
     static view_module = packageData.name; // Set to null if no view
     static view_module_version = packageData.version;
 }
 
 export class ScatterPlotView extends DOMWidgetView {
     timeout;
 
@@ -174,14 +177,101 @@
             data,
             x,
             y,
             hue,
             element,
             this.setValue.bind(this),
             this.setSelectedValues.bind(this),
+            width,
+            height,
+            margin
+        );
+    }
+
+    setValue(text) {
+        this.model.set({
+            clickedValue: text
+        });
+        this.model.save_changes();
+    }
+
+    setSelectedValues(values) {
+        this.model.set({
+            selectedValuesRecords: values
+        });
+        this.model.save_changes();
+    }
+}
+
+export class LinearPlotModel extends DOMWidgetModel {
+    defaults() {
+        return {
+            ...super.defaults(),
+            _model_name: LinearPlotModel.model_name,
+            _view_name: LinearPlotModel.view_name,
+            _model_module: LinearPlotModel.model_module,
+            _view_module: LinearPlotModel.view_module,
+            _model_module_version: LinearPlotModel.model_module_version,
+            _view_module_version: LinearPlotModel.view_module_version,
+
+            dataRecords: [],
+            x: String,
+            y: String,
+            hue: String,
+            elementId: String,
+            clickedValue: String,
+            selectedValuesRecords: [],
+        };
+    }
+
+    static model_name = "LinearPlotModel";
+    static model_module = packageData.name;
+    static model_module_version = packageData.version;
+    static view_name = "LinearPlotView"; // Set to null if no view
+    static view_module = packageData.name; // Set to null if no view
+    static view_module_version = packageData.version;
+}
+
+export class LinearPlotView extends DOMWidgetView {
+    timeout;
+
+    render() {
+        plotAfterInterval(this);
+
+        this.model.on("change:dataRecords", () => plotAfterInterval(this), this);
+        this.model.on("change:x", () => plotAfterInterval(this), this);
+        this.model.on("change:y", () => plotAfterInterval(this), this);
+        this.model.on("change:hue", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this));
+    }
+
+    plot() {
+        const data = this.model.get("dataRecords");
+        const x = this.model.get("x");
+        const y = this.model.get("y");
+        const hue = this.model.get("hue");
+        const elementId = this.model.get("elementId");
+
+        let height = WIDGET_HEIGHT;
+        let element = this.el;
+        if (elementId) {
+            element = document.getElementById(elementId);
+            height = element.clientHeight;
+        }
+        let width = element.clientWidth;
+        const margin = WIDGET_MARGIN;
+
+        linearplot(
+            data,
+            x,
+            y,
+            hue,
+            element,
+            this.setValue.bind(this),
+            this.setSelectedValues.bind(this),
             width,
             height,
             margin
         );
     }
 
     setValue(text) {
```

### Comparing `d3vis_ipynb-0.2.1/js/lib/graphs/barplot.js` & `d3vis_ipynb-0.2.2/js/lib/graphs/barplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/js/lib/graphs/histogramplot.js` & `d3vis_ipynb-0.2.2/js/lib/graphs/histogramplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/js/lib/graphs/linearhistplot.js` & `d3vis_ipynb-0.2.2/js/lib/graphs/linearhistplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/js/lib/graphs/rangeslider.js` & `d3vis_ipynb-0.2.2/js/lib/graphs/rangeslider.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/js/lib/graphs/scatterplot.js` & `d3vis_ipynb-0.2.2/js/lib/graphs/scatterplot.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,14 @@
     height,
     margin
 ) {
     const innerWidth = width - margin.left - margin.right;
     const innerHeight = height - margin.top - margin.bottom;
 
     for (let i = 0; i < data.length; i++) {
-        ("");
         data[i]["id"] = i;
     }
 
     const randomString = Math.floor(Math.random() * Date.now() * 10000).toString(
         36
     );
 
@@ -161,40 +160,42 @@
         margin.left,
         margin.top,
         resetColor,
         setLassoValues,
         randomString
     );
 
-    const legend = svg
-        .selectAll(".legend")
-        .data(color.domain())
-        .enter()
-        .append("g")
-        .attr("class", "legend")
-        .attr("transform", function(d, i) {
-            return "translate(0," + i * 20 + ")";
-        });
-
-    legend
-        .append("rect")
-        .attr("x", innerWidth - 18)
-        .attr("width", 18)
-        .attr("height", 18)
-        .style("fill", color);
+    if (hue) {
+        const legend = svg
+            .selectAll(".legend")
+            .data(color.domain())
+            .enter()
+            .append("g")
+            .attr("class", "legend")
+            .attr("transform", function(d, i) {
+                return "translate(0," + i * 20 + ")";
+            });
 
-    legend
-        .append("text")
-        .attr("x", innerWidth - 24)
-        .attr("y", 9)
-        .attr("dy", ".35em")
-        .style("text-anchor", "end")
-        .text(function(d) {
-            return d;
-        });
+        legend
+            .append("rect")
+            .attr("x", innerWidth - 18)
+            .attr("width", 18)
+            .attr("height", 18)
+            .style("fill", color);
+
+        legend
+            .append("text")
+            .attr("x", innerWidth - 24)
+            .attr("y", 9)
+            .attr("dy", ".35em")
+            .style("text-anchor", "end")
+            .text(function(d) {
+                return d;
+            });
+    }
 
     const focus = svg
         .append("g")
         .append("rect")
         .style("fill", "none")
         .attr("width", 160)
         .attr("height", 40)
```

### Comparing `d3vis_ipynb-0.2.1/js/lib/tools/lasso.js` & `d3vis_ipynb-0.2.2/js/lib/tools/lasso.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/LICENSE.txt` & `d3vis_ipynb-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/README.md` & `d3vis_ipynb-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.2.1/pyproject.toml` & `d3vis_ipynb-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "ipywidgets==7.7.1",
     "simplejson >=3.19.0",
     "anywidget >= 0.9.6"
 ]
-version = "0.2.1"
+version = "0.2.2"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
```

### Comparing `d3vis_ipynb-0.2.1/PKG-INFO` & `d3vis_ipynb-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: d3vis_ipynb
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Custom Jupyter Widget Library with visualizations created with D3.js.
 Project-URL: Homepage, https://github.com/H-IAAC/d3vis_ipynb
 Author-email: Daniel Adam Miranda <daniel.miranda@eldorado.org.br>
 License: Copyright (c) 2024 Daniel Adam Miranda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

