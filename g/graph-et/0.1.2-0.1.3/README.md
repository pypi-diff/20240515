# Comparing `tmp/graph-et-0.1.2.tar.gz` & `tmp/graph_et-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-et-0.1.2.tar", last modified: Thu Feb 15 22:50:18 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `graph-et-0.1.2.tar` & `graph_et-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-02-15 22:50:18.424455 graph-et-0.1.2/
--rw-r--r--   0 hayk      (1000) hayk      (1000)     1492 2024-02-15 20:16:47.000000 graph-et-0.1.2/LICENSE
--rw-r--r--   0 hayk      (1000) hayk      (1000)       56 2024-02-15 20:16:47.000000 graph-et-0.1.2/MANIFEST.in
--rw-r--r--   0 hayk      (1000) hayk      (1000)     2610 2024-02-15 22:50:18.424455 graph-et-0.1.2/PKG-INFO
--rw-r--r--   0 hayk      (1000) hayk      (1000)     1958 2024-02-15 22:49:37.000000 graph-et-0.1.2/README.md
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-02-15 22:50:18.424455 graph-et-0.1.2/graph_et.egg-info/
--rw-r--r--   0 hayk      (1000) hayk      (1000)     2610 2024-02-15 22:50:18.000000 graph-et-0.1.2/graph_et.egg-info/PKG-INFO
--rw-r--r--   0 hayk      (1000) hayk      (1000)      386 2024-02-15 22:50:18.000000 graph-et-0.1.2/graph_et.egg-info/SOURCES.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)        1 2024-02-15 22:50:18.000000 graph-et-0.1.2/graph_et.egg-info/dependency_links.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)      118 2024-02-15 22:50:18.000000 graph-et-0.1.2/graph_et.egg-info/requires.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)        8 2024-02-15 22:50:18.000000 graph-et-0.1.2/graph_et.egg-info/top_level.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)        1 2024-02-15 22:50:18.000000 graph-et-0.1.2/graph_et.egg-info/zip-safe
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-02-15 22:50:18.424455 graph-et-0.1.2/graphet/
--rw-r--r--   0 hayk      (1000) hayk      (1000)       66 2024-02-15 22:49:51.000000 graph-et-0.1.2/graphet/__init__.py
--rw-r--r--   0 hayk      (1000) hayk      (1000)     5005 2024-02-15 22:44:52.000000 graph-et-0.1.2/graphet/data.py
--rw-r--r--   0 hayk      (1000) hayk      (1000)    12584 2024-02-15 22:42:10.000000 graph-et-0.1.2/graphet/plugin.py
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-02-15 22:50:18.424455 graph-et-0.1.2/graphet/plugins/
--rw-r--r--   0 hayk      (1000) hayk      (1000)       33 2024-02-15 20:16:47.000000 graph-et-0.1.2/graphet/plugins/__init__.py
--rw-r--r--   0 hayk      (1000) hayk      (1000)     6997 2024-02-15 22:07:50.000000 graph-et-0.1.2/graphet/plugins/tristanv2.py
--rw-r--r--   0 hayk      (1000) hayk      (1000)     3242 2024-02-15 22:03:09.000000 graph-et-0.1.2/graphet/test_tristanv2.py
--rw-r--r--   0 hayk      (1000) hayk      (1000)       85 2024-02-15 20:16:47.000000 graph-et-0.1.2/pyproject.toml
--rw-r--r--   0 hayk      (1000) hayk      (1000)      724 2024-02-15 22:50:18.424455 graph-et-0.1.2/setup.cfg
--rw-r--r--   0 hayk      (1000) hayk      (1000)      256 2024-02-15 20:16:47.000000 graph-et-0.1.2/setup.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 graph_et-0.1.3/MANIFEST.in
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 graph_et-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 graph_et-0.1.3/.github/workflows/pytest_publish.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/__init__.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/data.py
+-rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/plugin.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/test_tristanv2.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/plugins/__init__.py
+-rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/plugins/tristanv2.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/fakedata.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/input.cfg
+-rw-r--r--   0        0        0   724096 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/flds/flds.tot.00000
+-rw-r--r--   0        0        0   724096 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/flds/flds.tot.00001
+-rw-r--r--   0        0        0   724096 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/flds/flds.tot.00002
+-rw-r--r--   0        0        0   724096 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/flds/flds.tot.00003
+-rw-r--r--   0        0        0   724096 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/flds/flds.tot.00004
+-rw-r--r--   0        0        0    22248 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/prtl/prtl.tot.00000
+-rw-r--r--   0        0        0    21816 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/prtl/prtl.tot.00001
+-rw-r--r--   0        0        0    21312 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/prtl/prtl.tot.00002
+-rw-r--r--   0        0        0    20784 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/prtl/prtl.tot.00003
+-rw-r--r--   0        0        0    20232 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/prtl/prtl.tot.00004
+-rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/spec/spec.tot.00000
+-rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/spec/spec.tot.00001
+-rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/spec/spec.tot.00002
+-rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/spec/spec.tot.00003
+-rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 graph_et-0.1.3/graphet/tests/data/tristanv2/spec/spec.tot.00004
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 graph_et-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 graph_et-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 graph_et-0.1.3/README.md
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 graph_et-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 graph_et-0.1.3/PKG-INFO
```

### Comparing `graph-et-0.1.2/LICENSE` & `graph_et-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graph-et-0.1.2/README.md` & `graph_et-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 # load the metadata using the TristanV2 plugin
 d = Data(
     TristanV2,              # plugin
     steps=range(150),       # steps to load metadata for
     path=f"output/",        # path to the data
     cfg_fname=f"input.cfg", # configuration file
+    params=True,            # read configuration file
     coord_transform={       # time/coordinate transformation
         "t": lambda t, prm: t * prm["output:interval"] * prm["algorithm:c"] / prm["grid:my0"],
         "x": lambda x, prm: (x - x.mean()) / prm["grid:my0"],
         "z": lambda z, prm: (z - z.mean()) / prm["grid:my0"],
         "y": lambda y, prm: (y - y.mean()) / prm["grid:my0"],
     },
     swapaxes=[(0, 1), (2, 1)],  # axes swapping "zyx" -> "yxz"
@@ -47,8 +48,8 @@
 ```
 
 ### Todo
 
 - [ ] Add support for `TristanV1` plugin
 - [x] Coordinate transformations for particles
 - [x] Support for coordinate swapping in field names
-- [ ] Support for custom defined fields
+- [ ] Support for custom defined fields
```

### Comparing `graph-et-0.1.2/graphet/data.py` & `graph_et-0.1.3/graphet/data.py`

 * *Files identical despite different names*

### Comparing `graph-et-0.1.2/graphet/plugin.py` & `graph_et-0.1.3/graphet/plugin.py`

 * *Files identical despite different names*

### Comparing `graph-et-0.1.2/graphet/plugins/tristanv2.py` & `graph_et-0.1.3/graphet/plugins/tristanv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,18 @@
             "coord_transform",
             "origaxes",
             "swapaxes",
         ]
         super().__init__(**{k: v for k, v in kwargs.items() if k in parent_kwargs})
         self.path = path
         self.cfg_fname = cfg_fname
-        if self.params and cfg_fname is None:
-            raise ValueError("`cfg_fname` must be specified if `params` is True")
+        if not self.cfg_fname is None:
+            self.params = True
+        else:
+            self.params = False
         self.fname_templates = {
             "flds": "flds/flds.tot.%05d",
             "prtl": "prtl/prtl.tot.%05d",
             "spec": "spec/spec.tot.%05d",
         }
         self.kwargs = {k: v for k, v in kwargs.items() if k not in parent_kwargs}
         self.files = {
```

### Comparing `graph-et-0.1.2/graphet/test_tristanv2.py` & `graph_et-0.1.3/graphet/test_tristanv2.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,21 @@
     fdir = os.path.dirname(os.path.abspath(__file__))
     d = Data(
         TristanV2,
         steps=range(5),
         path=f"{fdir}/tests/data/tristanv2/",
         first_step=0,
         swapaxes=[(0, 1), (2, 1)],
+        cfg_fname=f"{fdir}/tests/data/tristanv2/input.cfg",
     )
+    assert d.params is not None
+    assert d.params["blockA:paramA1"] == 1.23
+    assert d.params["blockA:paramA2"] == 2
+    assert d.params["blockB:paramB1"] == 345
+    assert d.params["blockB:paramB2"] == 4.56
     # "zyx" -> "yxz"
     # test fields
     assert sorted(list(d.fields.variables.keys())) == sorted(
         [
             "t",
             "z",
             "y",
```

