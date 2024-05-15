# Comparing `tmp/feature_clock-1.0.0.tar.gz` & `tmp/feature_clock-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_clock-1.0.0.tar", last modified: Wed May 15 15:55:55 2024, max compression
+gzip compressed data, was "feature_clock-1.0.1.tar", last modified: Wed May 15 16:07:48 2024, max compression
```

## Comparing `feature_clock-1.0.0.tar` & `feature_clock-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.950626 feature_clock-1.0.0/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    11356 2024-03-27 01:55:39.000000 feature_clock-1.0.0/LICENSE
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5623 2024-05-15 15:55:55.950407 feature_clock-1.0.0/PKG-INFO
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3019 2024-05-15 15:24:57.000000 feature_clock-1.0.0/README.md
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     2190 2024-05-15 15:55:44.000000 feature_clock-1.0.0/pyproject.toml
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       38 2024-05-15 15:55:55.950673 feature_clock-1.0.0/setup.cfg
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.944155 feature_clock-1.0.0/src/
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.945310 feature_clock-1.0.0/src/feature_clock/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        0 2024-02-16 15:04:27.000000 feature_clock-1.0.0/src/feature_clock/__init__.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1298 2024-05-15 15:33:23.000000 feature_clock-1.0.0/src/feature_clock/graph.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    51437 2024-05-15 15:33:17.000000 feature_clock-1.0.0/src/feature_clock/plot.py
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.950092 feature_clock-1.0.0/src/feature_clock.egg-info/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5623 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/PKG-INFO
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      513 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/SOURCES.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        1 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/dependency_links.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      799 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/requires.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       14 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/top_level.txt
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.949343 feature_clock-1.0.0/test/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    13015 2024-05-15 15:36:34.000000 feature_clock-1.0.0/test/test_cancer.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    15674 2024-05-15 15:33:01.000000 feature_clock-1.0.0/test/test_iris.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    15838 2024-05-15 15:33:30.000000 feature_clock-1.0.0/test/test_melody.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    28749 2024-05-15 15:34:13.000000 feature_clock-1.0.0/test/test_neftel.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    16859 2024-05-15 15:33:57.000000 feature_clock-1.0.0/test/test_pima.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    13372 2024-05-15 15:32:18.000000 feature_clock-1.0.0/test/test_pima_autoencoder.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8460 2024-05-15 15:32:41.000000 feature_clock-1.0.0/test/test_pima_nn.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8620 2024-05-15 15:32:43.000000 feature_clock-1.0.0/test/test_pima_nn_2out.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    48933 2024-05-15 15:33:49.000000 feature_clock-1.0.0/test/test_support.py
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 16:07:48.804398 feature_clock-1.0.1/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    11356 2024-03-27 01:55:39.000000 feature_clock-1.0.1/LICENSE
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5773 2024-05-15 16:07:48.804204 feature_clock-1.0.1/PKG-INFO
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3169 2024-05-15 16:06:24.000000 feature_clock-1.0.1/README.md
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     2190 2024-05-15 16:07:08.000000 feature_clock-1.0.1/pyproject.toml
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       38 2024-05-15 16:07:48.804448 feature_clock-1.0.1/setup.cfg
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 16:07:48.795345 feature_clock-1.0.1/src/
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 16:07:48.796548 feature_clock-1.0.1/src/feature_clock/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        0 2024-02-16 15:04:27.000000 feature_clock-1.0.1/src/feature_clock/__init__.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1298 2024-05-15 15:33:23.000000 feature_clock-1.0.1/src/feature_clock/graph.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    51437 2024-05-15 15:33:17.000000 feature_clock-1.0.1/src/feature_clock/plot.py
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 16:07:48.803877 feature_clock-1.0.1/src/feature_clock.egg-info/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5773 2024-05-15 16:07:48.000000 feature_clock-1.0.1/src/feature_clock.egg-info/PKG-INFO
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      513 2024-05-15 16:07:48.000000 feature_clock-1.0.1/src/feature_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        1 2024-05-15 16:07:48.000000 feature_clock-1.0.1/src/feature_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      799 2024-05-15 16:07:48.000000 feature_clock-1.0.1/src/feature_clock.egg-info/requires.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       14 2024-05-15 16:07:48.000000 feature_clock-1.0.1/src/feature_clock.egg-info/top_level.txt
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 16:07:48.803236 feature_clock-1.0.1/test/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    13015 2024-05-15 15:36:34.000000 feature_clock-1.0.1/test/test_cancer.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    15674 2024-05-15 15:33:01.000000 feature_clock-1.0.1/test/test_iris.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    15838 2024-05-15 15:33:30.000000 feature_clock-1.0.1/test/test_melody.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    28749 2024-05-15 15:34:13.000000 feature_clock-1.0.1/test/test_neftel.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    16859 2024-05-15 15:33:57.000000 feature_clock-1.0.1/test/test_pima.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    13372 2024-05-15 15:32:18.000000 feature_clock-1.0.1/test/test_pima_autoencoder.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8460 2024-05-15 15:32:41.000000 feature_clock-1.0.1/test/test_pima_nn.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8620 2024-05-15 15:32:43.000000 feature_clock-1.0.1/test/test_pima_nn_2out.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    48933 2024-05-15 15:33:49.000000 feature_clock-1.0.1/test/test_support.py
```

### Comparing `feature_clock-1.0.0/LICENSE` & `feature_clock-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/PKG-INFO` & `feature_clock-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_clock
-Version: 1.0.0
+Version: 1.0.1
 Summary: Feature Clock, provides visualizations that eliminate the need for multiple plots to inspect the influence of original variables in the latent space. Feature Clock enhances the explainability and compactness of visualizations of embedded data.
 Author-email: Olga Ovcharenko <ovcharenko.folga@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/feature-clock/
 Project-URL: Repository, https://github.com/OlgaOvcharenko/feature_clock_visualization
 Project-URL: Documentation, https://github.com/OlgaOvcharenko/feature_clock_visualization/blob/main/tutorials/docs.md
 Project-URL: Tutorial, https://github.com/OlgaOvcharenko/feature_clock_visualization/blob/main/tutorials/iris.md
 Project-URL: Issues, https://github.com/OlgaOvcharenko/feature_clock_visualization/issues
@@ -60,27 +60,25 @@
 Requires-Dist: threadpoolctl==3.3.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: tzdata==2024.1
 Requires-Dist: umap-learn==0.5.5
 Requires-Dist: wrapt==1.16.0
 
 <picture align="center">
-  <source media="(prefers-color-scheme: dark)" srcset="examples/pima/pima_only_clock.png">
-  <img style="float: right;" alt="Feature Clock" src="examples/pima/pima_only_clock.png" width="200" 
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/OlgaOvcharenko/feature_clock_visualization/main/examples/pima/pima_only_clock.png">
+  <img style="float: right;" alt="Feature Clock" src="https://raw.githubusercontent.com/OlgaOvcharenko/feature_clock_visualization/main/examples/pima/pima_only_clock.png" width="200" 
      height="200">
 </picture>
 
 # Feature Clock: High-Dimensional Effects in Two-Dimensional Plots
 
-| | 
-| --- | 
-| [Package](https://pypi.org/project/feature-clock/) 
-| [Documentation](tutorials/docs.md) 
-| [Tutorial](tutorials/iris.md) 
-| [Examples](https://github.com/OlgaOvcharenko/feature_clock_visualization/tree/main/test) 
+- [Package](https://pypi.org/project/feature-clock/) 
+- [Documentation](tutorials/docs.md) 
+- [Tutorial](tutorials/iris.md) 
+- [Examples](https://github.com/OlgaOvcharenko/feature_clock_visualization/tree/main/test) 
 
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 
 ## What is it?
 
 It is difficult for humans to perceive high-dimensional data. Therefore, high-dimensional data is projected into lower dimensions to visualize it. 
 Many applications benefit from complex nonlinear dimensionality reduction techniques (e.g., UMAP, t-SNE, PHATE, and autoencoders), but the effects of individual high-dimensional features are hard to explain in the latent spaces.
```

### Comparing `feature_clock-1.0.0/README.md` & `feature_clock-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 <picture align="center">
-  <source media="(prefers-color-scheme: dark)" srcset="examples/pima/pima_only_clock.png">
-  <img style="float: right;" alt="Feature Clock" src="examples/pima/pima_only_clock.png" width="200" 
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/OlgaOvcharenko/feature_clock_visualization/main/examples/pima/pima_only_clock.png">
+  <img style="float: right;" alt="Feature Clock" src="https://raw.githubusercontent.com/OlgaOvcharenko/feature_clock_visualization/main/examples/pima/pima_only_clock.png" width="200" 
      height="200">
 </picture>
 
 # Feature Clock: High-Dimensional Effects in Two-Dimensional Plots
 
-| | 
-| --- | 
-| [Package](https://pypi.org/project/feature-clock/) 
-| [Documentation](tutorials/docs.md) 
-| [Tutorial](tutorials/iris.md) 
-| [Examples](https://github.com/OlgaOvcharenko/feature_clock_visualization/tree/main/test) 
+- [Package](https://pypi.org/project/feature-clock/) 
+- [Documentation](tutorials/docs.md) 
+- [Tutorial](tutorials/iris.md) 
+- [Examples](https://github.com/OlgaOvcharenko/feature_clock_visualization/tree/main/test) 
 
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 
 ## What is it?
 
 It is difficult for humans to perceive high-dimensional data. Therefore, high-dimensional data is projected into lower dimensions to visualize it. 
 Many applications benefit from complex nonlinear dimensionality reduction techniques (e.g., UMAP, t-SNE, PHATE, and autoencoders), but the effects of individual high-dimensional features are hard to explain in the latent spaces.
```

### Comparing `feature_clock-1.0.0/pyproject.toml` & `feature_clock-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "feature_clock"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Olga Ovcharenko", email="ovcharenko.folga@gmail.com" },
 ]
 description = "Feature Clock, provides visualizations that eliminate the need for multiple plots to inspect the influence of original variables in the latent space. Feature Clock enhances the explainability and compactness of visualizations of embedded data."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `feature_clock-1.0.0/src/feature_clock/graph.py` & `feature_clock-1.0.1/src/feature_clock/graph.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/src/feature_clock/plot.py` & `feature_clock-1.0.1/src/feature_clock/plot.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/src/feature_clock.egg-info/PKG-INFO` & `feature_clock-1.0.1/src/feature_clock.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_clock
-Version: 1.0.0
+Version: 1.0.1
 Summary: Feature Clock, provides visualizations that eliminate the need for multiple plots to inspect the influence of original variables in the latent space. Feature Clock enhances the explainability and compactness of visualizations of embedded data.
 Author-email: Olga Ovcharenko <ovcharenko.folga@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/feature-clock/
 Project-URL: Repository, https://github.com/OlgaOvcharenko/feature_clock_visualization
 Project-URL: Documentation, https://github.com/OlgaOvcharenko/feature_clock_visualization/blob/main/tutorials/docs.md
 Project-URL: Tutorial, https://github.com/OlgaOvcharenko/feature_clock_visualization/blob/main/tutorials/iris.md
 Project-URL: Issues, https://github.com/OlgaOvcharenko/feature_clock_visualization/issues
@@ -60,27 +60,25 @@
 Requires-Dist: threadpoolctl==3.3.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: tzdata==2024.1
 Requires-Dist: umap-learn==0.5.5
 Requires-Dist: wrapt==1.16.0
 
 <picture align="center">
-  <source media="(prefers-color-scheme: dark)" srcset="examples/pima/pima_only_clock.png">
-  <img style="float: right;" alt="Feature Clock" src="examples/pima/pima_only_clock.png" width="200" 
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/OlgaOvcharenko/feature_clock_visualization/main/examples/pima/pima_only_clock.png">
+  <img style="float: right;" alt="Feature Clock" src="https://raw.githubusercontent.com/OlgaOvcharenko/feature_clock_visualization/main/examples/pima/pima_only_clock.png" width="200" 
      height="200">
 </picture>
 
 # Feature Clock: High-Dimensional Effects in Two-Dimensional Plots
 
-| | 
-| --- | 
-| [Package](https://pypi.org/project/feature-clock/) 
-| [Documentation](tutorials/docs.md) 
-| [Tutorial](tutorials/iris.md) 
-| [Examples](https://github.com/OlgaOvcharenko/feature_clock_visualization/tree/main/test) 
+- [Package](https://pypi.org/project/feature-clock/) 
+- [Documentation](tutorials/docs.md) 
+- [Tutorial](tutorials/iris.md) 
+- [Examples](https://github.com/OlgaOvcharenko/feature_clock_visualization/tree/main/test) 
 
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 
 ## What is it?
 
 It is difficult for humans to perceive high-dimensional data. Therefore, high-dimensional data is projected into lower dimensions to visualize it. 
 Many applications benefit from complex nonlinear dimensionality reduction techniques (e.g., UMAP, t-SNE, PHATE, and autoencoders), but the effects of individual high-dimensional features are hard to explain in the latent spaces.
```

### Comparing `feature_clock-1.0.0/src/feature_clock.egg-info/SOURCES.txt` & `feature_clock-1.0.1/src/feature_clock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/src/feature_clock.egg-info/requires.txt` & `feature_clock-1.0.1/src/feature_clock.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_cancer.py` & `feature_clock-1.0.1/test/test_cancer.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_iris.py` & `feature_clock-1.0.1/test/test_iris.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_melody.py` & `feature_clock-1.0.1/test/test_melody.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_neftel.py` & `feature_clock-1.0.1/test/test_neftel.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_pima.py` & `feature_clock-1.0.1/test/test_pima.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_pima_autoencoder.py` & `feature_clock-1.0.1/test/test_pima_autoencoder.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_pima_nn.py` & `feature_clock-1.0.1/test/test_pima_nn.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_pima_nn_2out.py` & `feature_clock-1.0.1/test/test_pima_nn_2out.py`

 * *Files identical despite different names*

### Comparing `feature_clock-1.0.0/test/test_support.py` & `feature_clock-1.0.1/test/test_support.py`

 * *Files identical despite different names*

