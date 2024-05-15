# Comparing `tmp/onion_clustering-0.2.1.tar.gz` & `tmp/onion_clustering-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_clustering-0.2.1.tar", last modified: Mon May 13 10:01:18 2024, max compression
+gzip compressed data, was "onion_clustering-0.2.2.tar", last modified: Tue May 14 14:16:00 2024, max compression
```

## Comparing `onion_clustering-0.2.1.tar` & `onion_clustering-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.882819 onion_clustering-0.2.1/
--rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-10 14:58:09.000000 onion_clustering-0.2.1/.coverage
--rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/.gitignore
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.1/LICENSE
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-13 10:01:18.881807 onion_clustering-0.2.1/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/README.md
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.860596 onion_clustering-0.2.1/examples/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3663 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/examples/example_script.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/examples/example_script_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/justfile
--rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-10 14:21:08.000000 onion_clustering-0.2.1/pyproject.toml
--rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.1/pytest.ini
--rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-13 10:01:18.883017 onion_clustering-0.2.1/setup.cfg
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.854860 onion_clustering-0.2.1/src/
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.868907 onion_clustering-0.2.1/src/onion_clustering/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/src/onion_clustering/__init__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-10 14:39:49.000000 onion_clustering-0.2.1/src/onion_clustering/classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    19700 2024-05-10 14:05:21.000000 onion_clustering-0.2.1/src/onion_clustering/first_classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23955 2024-05-10 14:53:43.000000 onion_clustering-0.2.1/src/onion_clustering/functions.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    25883 2024-05-10 14:03:06.000000 onion_clustering-0.2.1/src/onion_clustering/main.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23334 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/src/onion_clustering/main_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/src/onion_clustering/utilities.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.880540 onion_clustering-0.2.1/src/onion_clustering.egg-info/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/requires.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-13 10:01:18.000000 onion_clustering-0.2.1/src/onion_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.874029 onion_clustering-0.2.1/test/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.1/test/__init__.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.876595 onion_clustering-0.2.1/test/output_multi/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/test/output_multi/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/test/output_multi/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/test/output_multi/number_of_states.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-13 10:01:18.879266 onion_clustering-0.2.1/test/output_uni/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1759 2024-05-10 14:20:03.000000 onion_clustering-0.2.1/test/output_uni/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-10 14:19:53.000000 onion_clustering-0.2.1/test/output_uni/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-10 14:19:46.000000 onion_clustering-0.2.1/test/output_uni/number_of_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3375 2024-05-08 09:25:50.000000 onion_clustering-0.2.1/test/test_multi.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     2941 2024-05-10 14:20:36.000000 onion_clustering-0.2.1/test/test_uni.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-14 14:16:00.325472 onion_clustering-0.2.2/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/.gitignore
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.2/LICENSE
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-14 14:16:00.324682 onion_clustering-0.2.2/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/README.md
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-14 14:16:00.310029 onion_clustering-0.2.2/examples/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3663 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/examples/example_script.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/examples/example_script_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/justfile
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-14 14:15:24.000000 onion_clustering-0.2.2/pyproject.toml
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.2/pytest.ini
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-14 14:16:00.325647 onion_clustering-0.2.2/setup.cfg
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-14 14:16:00.305259 onion_clustering-0.2.2/src/
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-14 14:16:00.314272 onion_clustering-0.2.2/src/onion_clustering/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/src/onion_clustering/__init__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-10 14:39:49.000000 onion_clustering-0.2.2/src/onion_clustering/classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    19700 2024-05-10 14:05:21.000000 onion_clustering-0.2.2/src/onion_clustering/first_classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    27610 2024-05-14 13:39:51.000000 onion_clustering-0.2.2/src/onion_clustering/functions.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    26241 2024-05-14 13:42:19.000000 onion_clustering-0.2.2/src/onion_clustering/main.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    23334 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/src/onion_clustering/main_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/src/onion_clustering/utilities.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-14 14:16:00.323742 onion_clustering-0.2.2/src/onion_clustering.egg-info/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-14 14:16:00.000000 onion_clustering-0.2.2/src/onion_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      832 2024-05-14 14:16:00.000000 onion_clustering-0.2.2/src/onion_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-14 14:16:00.000000 onion_clustering-0.2.2/src/onion_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-14 14:16:00.000000 onion_clustering-0.2.2/src/onion_clustering.egg-info/requires.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-14 14:16:00.000000 onion_clustering-0.2.2/src/onion_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-14 14:16:00.318738 onion_clustering-0.2.2/test/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.2/test/__init__.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-14 14:16:00.321014 onion_clustering-0.2.2/test/output_multi/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/test/output_multi/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/test/output_multi/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/test/output_multi/number_of_states.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-14 14:16:00.323087 onion_clustering-0.2.2/test/output_uni/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1662 2024-05-14 13:55:06.000000 onion_clustering-0.2.2/test/output_uni/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-14 13:55:01.000000 onion_clustering-0.2.2/test/output_uni/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-14 13:55:01.000000 onion_clustering-0.2.2/test/output_uni/number_of_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3375 2024-05-08 09:25:50.000000 onion_clustering-0.2.2/test/test_multi.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     2941 2024-05-14 13:56:18.000000 onion_clustering-0.2.2/test/test_uni.py
```

### Comparing `onion_clustering-0.2.1/LICENSE` & `onion_clustering-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/PKG-INFO` & `onion_clustering-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.1
+Version: 0.2.2
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.2.1/README.md` & `onion_clustering-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/examples/example_script.py` & `onion_clustering-0.2.2/examples/example_script.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/examples/example_script_2d.py` & `onion_clustering-0.2.2/examples/example_script_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/justfile` & `onion_clustering-0.2.2/justfile`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/pyproject.toml` & `onion_clustering-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onion_clustering"
-version = "0.2.1"
+version = "0.2.2"
 description = "Code for unsupervised clustering of time-correlated data."
 # license = "MIT"
 maintainers = [
   { name = "Matteo Becchi", email = "bechmath@gmail.com" },
 ]
 dependencies = [
   "matplotlib",
```

### Comparing `onion_clustering-0.2.1/src/onion_clustering/classes.py` & `onion_clustering-0.2.2/src/onion_clustering/classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/src/onion_clustering/first_classes.py` & `onion_clustering-0.2.2/src/onion_clustering/first_classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/src/onion_clustering/functions.py` & `onion_clustering-0.2.2/src/onion_clustering/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from typing import List, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.optimize
 import scipy.signal
+from scipy.integrate import quad
 
 from onion_clustering.first_classes import Parameters, StateMulti, StateUni
 
 
 def read_input_data() -> str:
     """
     Attempt to read the content of 'data_directory.txt' file
@@ -417,81 +418,224 @@
         only_th = (st_0.mean + st_1.mean) / 2 - st_0.sigma**2 / 2 / (
             st_1.mean - st_0.mean
         ) * np.log(st_0.area / st_1.area)
         return only_th, 1
     if delta >= 0:
         th_plus = (-coeff_b + np.sqrt(delta)) / (2 * coeff_a)
         th_minus = (-coeff_b - np.sqrt(delta)) / (2 * coeff_a)
+        # if st_0.mean < th_plus and st_1.mean > th_plus:
+        #     return th_plus, 1
         intercept_plus = gaussian(th_plus, st_0.mean, st_0.sigma, st_0.area)
         intercept_minus = gaussian(th_minus, st_0.mean, st_0.sigma, st_0.area)
         if intercept_plus >= intercept_minus:
             return th_plus, 1
         return th_minus, 1
     th_aver = (st_0.mean / st_0.sigma + st_1.mean / st_1.sigma) / (
         1 / st_0.sigma + 1 / st_1.sigma
     )
     return th_aver, 2
 
 
+def shared_area_between_gaussians(
+    area1, mean1, sigma1, area2, mean2, sigma2
+) -> Tuple[float, float]:
+    """
+    Computes the shared area between two Gaussians.
+
+    Parameters
+    ----------
+
+    area1, mean1, sigma1 : float
+        The parameters of Gaussian 1.
+
+    area2, mean2, sigma2 : float
+        The parameters of Gaussian 2.
+
+    Returns
+    -------
+
+    shared_fraction_1 : float
+        The fraction of the area of the first Gaussian in common with the
+        second Gaussian.
+
+    shared_fraction_2 : float
+        The fraction of the area of the second Gaussian in common with the
+        first Gaussian.
+    """
+
+    def gauss_1(x):
+        gauss = gaussian(x, mean1, sigma1, area1)
+        return gauss
+
+    def gauss_2(x):
+        gauss = gaussian(x, mean2, sigma2, area2)
+        return gauss
+
+    def min_of_gaussians(x):
+        min_values = np.minimum(
+            gaussian(x, mean1, sigma1, area1),
+            gaussian(x, mean2, sigma2, area2),
+        )
+        return min_values
+
+    area_gaussian_1, _ = quad(gauss_1, -np.inf, np.inf)
+    area_gaussian_2, _ = quad(gauss_2, -np.inf, np.inf)
+    shared_area, _ = quad(min_of_gaussians, -np.inf, np.inf)
+    shared_fraction_1 = shared_area / area_gaussian_1
+    shared_fraction_2 = shared_area / area_gaussian_2
+
+    return shared_fraction_1, shared_fraction_2
+
+
+def final_state_settings(
+    list_of_states: List[StateUni],
+    m_range: np.ndarray,
+) -> List[StateUni]:
+    """
+    Final adjustemts and output in the list of identified states.
+
+    Parameters
+    ----------
+
+    list_of_states : list[StateUni]
+        The list of final states.
+
+    m_range : np.ndarray of shape (2,)
+        Range of values in the data matrix.
+
+    Returns
+    -------
+
+    list_of_states : list[StateUni]
+        Now with the correct thresholds asssigned to each state.
+    """
+    # Calculate the final threshold values
+    # and their types based on the intercept between neighboring states.
+    list_of_states[0].th_inf[0] = m_range[0]
+    list_of_states[0].th_inf[1] = 0
+
+    for i in range(len(list_of_states) - 1):
+        th_val, th_type = find_intersection(
+            list_of_states[i], list_of_states[i + 1]
+        )
+        list_of_states[i].th_sup[0] = th_val
+        list_of_states[i].th_sup[1] = th_type
+        list_of_states[i + 1].th_inf[0] = th_val
+        list_of_states[i + 1].th_inf[1] = th_type
+
+    list_of_states[-1].th_sup[0] = m_range[1]
+    list_of_states[-1].th_sup[1] = 0
+
+    # Write the final states and final thresholds to text files.
+    with open("final_states.txt", "a", encoding="utf-8") as file:
+        print("####################################", file=file)
+        print("# Mu \t Sigma \t A \t state_fraction", file=file)
+        for state in list_of_states:
+            print(state.mean, state.sigma, state.area, state.perc, file=file)
+    with open("final_thresholds.txt", "a", encoding="utf-8") as file:
+        print("####################################", file=file)
+        print("# Threshold_value \t Threshold type", file=file)
+        for state in list_of_states:
+            print(state.th_inf[0], state.th_inf[1], file=file)
+        print(
+            list_of_states[-1].th_sup[0],
+            list_of_states[-1].th_sup[1],
+            file=file,
+        )
+
+    return list_of_states
+
+
 def set_final_states(
     list_of_states: List[StateUni],
     all_the_labels: np.ndarray,
-    m_range: np.ndarray,
+    area_max_overlap: float,
 ) -> Tuple[List[StateUni], np.ndarray]:
     """
     Assigns final states and relabels labels based on specific criteria.
 
-    Args:
-    - list_of_states (list[StateUni]): List of StateUni objects representing
-        potential states.
-    - all_the_labels (np.ndarray): 2D NumPy array containing labels for each
-        data point.
-    - m_range (list[float]): Range of values in the data.
-
-    Returns:
-    - tuple: A tuple containing the final list of states
-    (list[StateUni]) and the newly labeled data (np.ndarray).
+    Parameters
+    ----------
+
+    list_of_states : List[StateUni]
+        List of StateUni objects representing potential states.
+
+    all_the_labels : np.ndarray of shape (n_particles, n_windows)
+        The proposed labels for each data point.
+
+    area_max_overlap : float
+        The threshold for merging two states together if they overlap.
+
+    Returns
+    -------
+
+    updated_states : List[StateUni]
+        Final list of StateUni objects representing potential states.
+
+    all_the_labels : np.ndarray of shape (n_particles, n_windows)
+        The definitive labels for each data point.
     """
-    ### Step 1: Merge together the strongly overlapping states
     # Find all the possible merges: j could be merged into i --> [j, i]
-
     proposed_merge = []
     for i, st_0 in enumerate(list_of_states):
         for j, st_1 in enumerate(list_of_states):
-            if j != i:
-                if (
+            if j > i:
+                # Condition 1: area overlap
+                shared_area_1, shared_area_2 = shared_area_between_gaussians(
+                    st_1.area,
+                    st_1.mean,
+                    st_1.sigma,
+                    st_0.area,
+                    st_0.mean,
+                    st_0.sigma,
+                )
+                thresh = area_max_overlap
+                if shared_area_1 > thresh >= shared_area_2:
+                    proposed_merge.append([j, i])
+                elif shared_area_2 > thresh >= shared_area_1:
+                    proposed_merge.append([i, j])
+                elif shared_area_1 > thresh and shared_area_2 > thresh:
+                    proposed_merge.append(
+                        [j, i] if shared_area_1 > shared_area_2 else [i, j]
+                    )
+                # Condition 2: mean proximity
+                elif (
                     st_0.peak > st_1.peak
-                    and abs(st_1.mean - st_0.mean) < st_0.sigma
+                    and np.abs(st_0.mean - st_1.mean) < st_0.sigma
+                    and st_1.sigma < 2 * st_0.sigma
                 ):
                     proposed_merge.append([j, i])
+                elif (
+                    st_1.peak > st_0.peak
+                    and np.abs(st_0.mean - st_1.mean) < st_1.sigma
+                    and st_0.sigma < 2 * st_1.sigma
+                ):
+                    proposed_merge.append([i, j])
 
     # Find the best merges (merge into the closest candidate)
     best_merge = []
     states_to_be_merged = np.unique([pair[0] for pair in proposed_merge])
     for j in states_to_be_merged:
         candidate_merge = []
         for pair in proposed_merge:
             if pair[0] == j:
                 candidate_merge.append(pair)
         if len(candidate_merge) == 1:
             best_merge.append(candidate_merge[0])
         else:
-            list_of_distances = [
-                np.linalg.norm(
-                    list_of_states[pair[1]].mean - list_of_states[pair[0]].mean
-                )
-                for pair in candidate_merge
+            importance = [
+                list_of_states[pair[1]].perc for pair in candidate_merge
             ]
-            best_merge.append(candidate_merge[np.argmin(list_of_distances)])
+            best_merge.append(candidate_merge[np.argmax(importance)])
 
     # Settle merging chains
     # if [i, j], all the [k, i] become [k, j]
     for pair in best_merge:
         for j, elem in enumerate(best_merge):
-            if elem[1] == pair[0]:
+            if elem[1] == pair[0] and elem[0] != pair[1]:
                 best_merge[j][1] = pair[1]
 
     # Relabel the labels in all_the_labels
     relabel_dic = {}
     for pair in best_merge:
         relabel_dic[pair[0]] = pair[1]
     if_env0 = np.any(np.unique(all_the_labels) == 0)
@@ -517,65 +661,24 @@
     states_to_remove = set(s0 for s0, s1 in best_merge)
     updated_states = [
         state
         for i, state in enumerate(list_of_states)
         if i not in states_to_remove
     ]
 
-    # Compute the fraction of data points in each state
-    for st_id, state in enumerate(updated_states):
-        num_of_points = np.sum(all_the_labels == st_id + 1)
-        state.perc = num_of_points / all_the_labels.size
-
-    # Step 2: Calculate the final threshold values
-    # and their types based on the intercept between neighboring states.
-    updated_states[0].th_inf[0] = m_range[0]
-    updated_states[0].th_inf[1] = 0
-
-    for i in range(len(updated_states) - 1):
-        th_val, th_type = find_intersection(
-            updated_states[i], updated_states[i + 1]
-        )
-        updated_states[i].th_sup[0] = th_val
-        updated_states[i].th_sup[1] = th_type
-        updated_states[i + 1].th_inf[0] = th_val
-        updated_states[i + 1].th_inf[1] = th_type
-
-    updated_states[-1].th_sup[0] = m_range[1]
-    updated_states[-1].th_sup[1] = 0
-
-    # Step 3: Write the final states and final thresholds to text files.
-    # The data is saved in two separate files:
-    # 'final_states.txt' and 'final_thresholds.txt'.
-    with open("final_states.txt", "a", encoding="utf-8") as file:
-        print("####################################", file=file)
-        print("# Mu \t Sigma \t A \t state_fraction", file=file)
-        for state in updated_states:
-            print(state.mean, state.sigma, state.area, state.perc, file=file)
-    with open("final_thresholds.txt", "a", encoding="utf-8") as file:
-        print("####################################", file=file)
-        for state in updated_states:
-            print(state.th_inf[0], state.th_inf[1], file=file)
-        print(
-            updated_states[-1].th_sup[0],
-            updated_states[-1].th_sup[1],
-            file=file,
-        )
-
-    # Step 5: Return the 'updated_states' as the output of the function.
     return updated_states, all_the_labels
 
 
 def find_max_prob_state(
     window: np.ndarray,
     old_label: int,
     list_of_states: List[StateUni],
 ) -> int:
     """
-    Assign a singla window to the state for which the belonging
+    Assign a single window to the state for which the belonging
     is the most probable.
 
     Parameters
     ----------
 
     window : np.ndarray of shape (tau_window,)
         The signal window to assign to a state.
@@ -596,70 +699,96 @@
     -----
 
     I am using the meadian here, instead of the mean, because it's more
     robust against outliers. Not sure if this is the best chioce.
     """
     median_x = np.median(window)
     new_label = old_label
-    if median_x < list_of_states[old_label - 1].th_inf[0]:
-        new_label -= 1
-    elif median_x > list_of_states[old_label - 1].th_sup[0]:
-        new_label += 1
+    state = list_of_states[old_label - 1]
+    gauss_max = gaussian(median_x, state.mean, state.sigma, state.area)
+    for i, state in enumerate(list_of_states):
+        gauss = gaussian(median_x, state.mean, state.sigma, state.area)
+        if gauss > gauss_max:
+            new_label = i + 1
     return new_label
 
 
 def max_prob_assignment(
     list_of_states: List[StateUni],
     matrix: np.ndarray,
     all_the_labels: np.ndarray,
+    m_range: np.ndarray,
     tau_window: int,
+    number_of_sigmas: float,
 ) -> Tuple[np.ndarray, List[StateUni]]:
     """
     After all the states have been identified, assign each window.
-    Each signal window is assignet to the most probable state.
+    Each signal window is assigned to the most probable state.
 
     Parameters
     ----------
 
     list_of_states : List[StateUni]
         List of the identified states.
 
     matrix : np.ndarray of shape (num_of_particles, num_of_timesteps)
         The data to cluster.
 
     all_the_labels : np.ndarray of shape (num_of_particles, num_of_windows)
         The temporary labels assigned to the signal windows.
 
+    m_range : np.ndarray of shape (2,)
+        Range of values in the data matrix.
+
     tau_window : int
         The time resolution of the analysis.
 
     Returns
     -------
 
     final_labels : np.ndarray of shape (num_of_particles, num_of_windows)
         The definitive labels for all the signal windows.
 
-    list_of_states : List[StateUni]
+    updated_states : List[StateUni]
         List of the identified states, with updated percetages.
     """
     final_labels = np.zeros(all_the_labels.shape, dtype=int)
     for i, mol in enumerate(all_the_labels):
         for j, old_label in enumerate(mol):
             if old_label > 0:
                 window = matrix[i][tau_window * j : tau_window * (j + 1)]
                 new_label = find_max_prob_state(
                     window, old_label, list_of_states
                 )
-                final_labels[i][j] = new_label
+                s_range = (
+                    2.0
+                    * number_of_sigmas
+                    * list_of_states[new_label - 1].sigma
+                )
+                if np.max(window) - np.min(window) < s_range:
+                    final_labels[i][j] = new_label
 
     for i, state in enumerate(list_of_states):
         num_of_points = np.sum(final_labels == i + 1)
         state.perc = num_of_points / final_labels.size
 
-    return final_labels, list_of_states
+    states_to_remove = []
+    for i, state in enumerate(list_of_states):
+        if state.perc == 0.0:
+            states_to_remove.append(i)
+
+    for i in states_to_remove[::-1]:
+        list_of_states.pop(i)
+
+    updated_states = final_state_settings(
+        list_of_states,
+        m_range,
+    )
+
+    return final_labels, updated_states
 
 
 def relabel_states_2d(
     all_the_labels: np.ndarray, states_list: list[StateMulti]
 ) -> Tuple[np.ndarray, List[StateMulti]]:
     """
     Reorders labels and merges strongly overlapping states in a
```

### Comparing `onion_clustering-0.2.1/src/onion_clustering/main.py` & `onion_clustering-0.2.2/src/onion_clustering/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     plot_histo,
     read_input_data,
     relabel_states,
     set_final_states,
 )
 
 OUTPUT_FILE = "states_output.txt"
+AREA_MAX_OVERLAP = 0.8
 
 
 def all_the_input_stuff(number_of_sigmas: float) -> ClusteringObject1D:
     """
     Reads input parameters and raw data from specified files and directories,
     processes the raw data, and creates output files.
 
@@ -722,22 +723,26 @@
     if len(tmp_cl_ob.states) == 0:
         print("* No possible classification was found. ")
         # We need to free the memory otherwise it accumulates
         del tmp_cl_ob
         return 0, 1.0, [1.0]
 
     list_of_states, tmp_labels = set_final_states(
-        tmp_cl_ob.states, tmp_labels, tmp_cl_ob.data.range
+        tmp_cl_ob.states,
+        tmp_labels,
+        AREA_MAX_OVERLAP,
     )
 
     tmp_cl_ob.data.labels, tmp_cl_ob.states = max_prob_assignment(
         list_of_states,
         tmp_cl_ob.data.matrix,
         tmp_labels,
+        tmp_cl_ob.data.range,
         tau_w,
+        tmp_cl_ob.number_of_sigmas,
     )
 
     list_of_pop = [state.perc for state in tmp_cl_ob.states]
     fraction_0 = 1 - np.sum(list_of_pop)
     list_of_pop.insert(0, fraction_0)
     n_states = len(tmp_cl_ob.states)
 
@@ -775,23 +780,28 @@
 
     cl_ob.preparing_the_data()
 
     cl_ob, tmp_labels, _ = iterative_search(cl_ob, "", full_out)
     if len(cl_ob.states) == 0:
         print("* No possible classification was found. ")
         return cl_ob
+
     list_of_states, tmp_labels = set_final_states(
-        cl_ob.states, tmp_labels, cl_ob.data.range
+        cl_ob.states,
+        tmp_labels,
+        AREA_MAX_OVERLAP,
     )
 
     cl_ob.data.labels, cl_ob.states = max_prob_assignment(
         list_of_states,
         cl_ob.data.matrix,
         tmp_labels,
+        cl_ob.data.range,
         cl_ob.par.tau_w,
+        cl_ob.number_of_sigmas,
     )
 
     return cl_ob
 
 
 def time_resolution_analysis(
     cl_ob: ClusteringObject1D,
@@ -869,14 +879,21 @@
         Useful for debugging.
 
     number_of_sigmas : float
         The signal windos are classified inside a state with a certain mean
         and std_dev if all the points differ from the mean less than
         std_dev * number_of_sigmas.
 
+    Returns
+    -------
+
+    clustering_object : ClusteringObject1D
+        The clusteriong object, with the input data, the parameters and the
+        results of the clustering.
+
     Notes
     -----
 
     all_the_input_stuff() reads the data and the parameters
 
     time_resolution_analysis() explore the parameter
         (tau_window, t_smooth) space.
```

### Comparing `onion_clustering-0.2.1/src/onion_clustering/main_2d.py` & `onion_clustering-0.2.2/src/onion_clustering/main_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/src/onion_clustering/utilities.py` & `onion_clustering-0.2.2/src/onion_clustering/utilities.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/src/onion_clustering.egg-info/PKG-INFO` & `onion_clustering-0.2.2/src/onion_clustering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.1
+Version: 0.2.2
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.2.1/src/onion_clustering.egg-info/SOURCES.txt` & `onion_clustering-0.2.2/src/onion_clustering.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.coverage
 .gitignore
 LICENSE
 README.md
 justfile
 pyproject.toml
 pytest.ini
 examples/example_script.py
```

### Comparing `onion_clustering-0.2.1/test/output_uni/final_states.txt` & `onion_clustering-0.2.2/test/output_uni/final_states.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 ####################################
 # Mu 	 Sigma 	 A 	 state_fraction
-0.04892510754413383 0.0288408773799436 527047.6891876374 0.5156112732178715
-0.1367047182092299 0.05585033639005192 167626.7077460476 0.16578619164156627
-0.29519390857730726 0.08902590374377187 238092.09183591892 0.25758110567269077
-0.5030446160410642 0.07324156207714633 35875.01628934908 0.02305707203815261
+0.04892510754413383 0.0288408773799436 527047.6891876374 0.5106637487449799
+0.1367047182092299 0.05585033639005192 167626.7077460476 0.14831591992971888
+0.29519390857730726 0.08902590374377187 238092.09183591892 0.2797243662148594
+0.5030446160410642 0.07324156207714633 35875.01628934908 0.023327685742971886
 ####################################
 # Mu 	 Sigma 	 A 	 state_fraction
-0.04728970760791858 0.02175885422664187 487915.7122986365 0.48912838855421686
-0.12238384510777277 0.055025420679579926 180185.57722333298 0.18094644201807228
-0.3172125305527501 0.11704851245493808 357114.92306615046 0.32593459776606426
-0.4559904699064358 0.09569746963864592 1980.5443778251902 0.002925765562248996
-0.5612466691529839 0.027762586622335286 2126.7123695486493 0.0008549824297188755
+0.04728970760791858 0.02175885422664187 487915.7122986365 0.47903724272088355
+0.12238384510777277 0.055025420679579926 180185.57722333298 0.16448214733935743
+0.3172125305527501 0.11704851245493808 357114.92306615046 0.35540403802710846
+0.5612466691529839 0.027762586622335286 2126.7123695486493 0.000733402359437751
 ####################################
 # Mu 	 Sigma 	 A 	 state_fraction
-0.04892510754413383 0.0288408773799436 527047.6891876374 0.46089764030612246
-0.11570641898479693 0.06326317553136362 210078.33319256912 0.14766023596938777
-0.2940075049253417 0.15778224806616864 406101.82306752447 0.35169204400510207
+0.04892510754413383 0.0288408773799436 527047.6891876374 0.5000697544642857
+0.11570641898479693 0.06326317553136362 210078.33319256912 0.12445192920918367
+0.2940075049253417 0.15778224806616864 406101.82306752447 0.3271484375
 ####################################
 # Mu 	 Sigma 	 A 	 state_fraction
-0.04728970760791858 0.02175885422664187 487915.7122986365 0.4396424585459184
-0.10085567417138075 0.05924642469454584 219275.10726036548 0.16774952168367346
-0.3072228050491294 0.137037804726867 397281.0735281235 0.39260801977040816
+0.04728970760791858 0.02175885422664187 487915.7122986365 0.4708227040816326
+0.10085567417138075 0.05924642469454584 219275.10726036548 0.15050023915816327
+0.3072228050491294 0.137037804726867 397281.0735281235 0.3755580357142857
 ####################################
 # Mu 	 Sigma 	 A 	 state_fraction
-0.04892510754413383 0.0288408773799436 527047.6891876374 0.46089764030612246
-0.11570641898479693 0.06326317553136362 210078.33319256912 0.14766023596938777
-0.2940075049253417 0.15778224806616864 406101.82306752447 0.35169204400510207
+0.04892510754413383 0.0288408773799436 527047.6891876374 0.5000697544642857
+0.11570641898479693 0.06326317553136362 210078.33319256912 0.12445192920918367
+0.2940075049253417 0.15778224806616864 406101.82306752447 0.3271484375
```

### Comparing `onion_clustering-0.2.1/test/test_multi.py` & `onion_clustering-0.2.2/test/test_multi.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.1/test/test_uni.py` & `onion_clustering-0.2.2/test/test_uni.py`

 * *Files identical despite different names*

