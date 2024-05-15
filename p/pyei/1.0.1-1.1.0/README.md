# Comparing `tmp/pyei-1.0.1.tar.gz` & `tmp/pyei-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyei-1.0.1.tar", last modified: Tue Aug 29 01:58:17 2023, max compression
+gzip compressed data, was "pyei-1.1.0.tar", last modified: Sun Feb 11 23:26:10 2024, max compression
```

## Comparing `pyei-1.0.1.tar` & `pyei-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 karin      (501) staff       (20)        0 2023-08-29 01:58:17.503961 pyei-1.0.1/
--rw-r--r--   0 karin      (501) staff       (20)     1097 2023-08-28 00:52:09.000000 pyei-1.0.1/LICENSE
--rw-r--r--   0 karin      (501) staff       (20)     5698 2023-08-29 01:58:17.503853 pyei-1.0.1/PKG-INFO
--rw-r--r--   0 karin      (501) staff       (20)     5482 2023-08-28 00:52:09.000000 pyei-1.0.1/README.md
-drwxr-xr-x   0 karin      (501) staff       (20)        0 2023-08-29 01:58:17.503030 pyei-1.0.1/pyei/
--rw-r--r--   0 karin      (501) staff       (20)      192 2023-08-29 01:56:03.000000 pyei-1.0.1/pyei/__init__.py
--rw-r--r--   0 karin      (501) staff       (20)      928 2023-08-28 00:52:09.000000 pyei-1.0.1/pyei/data.py
--rw-r--r--   0 karin      (501) staff       (20)     3112 2023-08-28 00:52:09.000000 pyei-1.0.1/pyei/distribution_utils.py
--rw-r--r--   0 karin      (501) staff       (20)    12890 2023-08-28 00:52:09.000000 pyei-1.0.1/pyei/goodmans_er.py
--rw-r--r--   0 karin      (501) staff       (20)    21115 2023-08-29 01:23:12.000000 pyei-1.0.1/pyei/greiner_quinn_gibbs_sampling.py
--rw-r--r--   0 karin      (501) staff       (20)     4049 2023-08-29 01:23:12.000000 pyei-1.0.1/pyei/io_utils.py
--rw-r--r--   0 karin      (501) staff       (20)    30800 2023-08-29 01:23:12.000000 pyei-1.0.1/pyei/plot_utils.py
--rw-r--r--   0 karin      (501) staff       (20)    45805 2023-08-28 00:52:09.000000 pyei-1.0.1/pyei/r_by_c.py
--rw-r--r--   0 karin      (501) staff       (20)     5098 2023-08-28 00:52:09.000000 pyei-1.0.1/pyei/r_by_c_models.py
--rw-r--r--   0 karin      (501) staff       (20)     3256 2023-08-28 00:52:09.000000 pyei-1.0.1/pyei/r_by_c_utils.py
--rw-r--r--   0 karin      (501) staff       (20)    41260 2023-08-28 00:52:09.000000 pyei-1.0.1/pyei/two_by_two.py
-drwxr-xr-x   0 karin      (501) staff       (20)        0 2023-08-29 01:58:17.503676 pyei-1.0.1/pyei.egg-info/
--rw-r--r--   0 karin      (501) staff       (20)     5698 2023-08-29 01:58:17.000000 pyei-1.0.1/pyei.egg-info/PKG-INFO
--rw-r--r--   0 karin      (501) staff       (20)      392 2023-08-29 01:58:17.000000 pyei-1.0.1/pyei.egg-info/SOURCES.txt
--rw-r--r--   0 karin      (501) staff       (20)        1 2023-08-29 01:58:17.000000 pyei-1.0.1/pyei.egg-info/dependency_links.txt
--rw-r--r--   0 karin      (501) staff       (20)      107 2023-08-29 01:58:17.000000 pyei-1.0.1/pyei.egg-info/requires.txt
--rw-r--r--   0 karin      (501) staff       (20)        5 2023-08-29 01:58:17.000000 pyei-1.0.1/pyei.egg-info/top_level.txt
--rw-r--r--   0 karin      (501) staff       (20)       38 2023-08-29 01:58:17.504006 pyei-1.0.1/setup.cfg
--rw-r--r--   0 karin      (501) staff       (20)     1364 2023-08-28 00:52:09.000000 pyei-1.0.1/setup.py
+drwxr-xr-x   0 karin      (501) staff       (20)        0 2024-02-11 23:26:10.198873 pyei-1.1.0/
+-rw-r--r--   0 karin      (501) staff       (20)     1097 2024-02-11 20:35:26.000000 pyei-1.1.0/LICENSE
+-rw-r--r--   0 karin      (501) staff       (20)     6020 2024-02-11 23:26:10.198677 pyei-1.1.0/PKG-INFO
+-rw-r--r--   0 karin      (501) staff       (20)     5503 2024-02-11 23:22:20.000000 pyei-1.1.0/README.md
+drwxr-xr-x   0 karin      (501) staff       (20)        0 2024-02-11 23:26:10.197711 pyei-1.1.0/pyei/
+-rw-r--r--   0 karin      (501) staff       (20)      193 2024-02-11 23:22:20.000000 pyei-1.1.0/pyei/__init__.py
+-rw-r--r--   0 karin      (501) staff       (20)      929 2024-02-11 23:22:20.000000 pyei-1.1.0/pyei/data.py
+-rw-r--r--   0 karin      (501) staff       (20)     3112 2024-02-11 20:35:26.000000 pyei-1.1.0/pyei/distribution_utils.py
+-rw-r--r--   0 karin      (501) staff       (20)    12890 2024-02-11 20:35:26.000000 pyei-1.1.0/pyei/goodmans_er.py
+-rw-r--r--   0 karin      (501) staff       (20)    21115 2024-02-11 20:35:26.000000 pyei-1.1.0/pyei/greiner_quinn_gibbs_sampling.py
+-rw-r--r--   0 karin      (501) staff       (20)     4051 2024-02-11 23:22:20.000000 pyei-1.1.0/pyei/io_utils.py
+-rw-r--r--   0 karin      (501) staff       (20)    30801 2024-02-11 23:22:20.000000 pyei-1.1.0/pyei/plot_utils.py
+-rw-r--r--   0 karin      (501) staff       (20)    45814 2024-02-11 23:22:20.000000 pyei-1.1.0/pyei/r_by_c.py
+-rw-r--r--   0 karin      (501) staff       (20)     5100 2024-02-11 23:22:20.000000 pyei-1.1.0/pyei/r_by_c_models.py
+-rw-r--r--   0 karin      (501) staff       (20)     3257 2024-02-11 23:22:20.000000 pyei-1.1.0/pyei/r_by_c_utils.py
+-rw-r--r--   0 karin      (501) staff       (20)    41244 2024-02-11 23:22:20.000000 pyei-1.1.0/pyei/two_by_two.py
+drwxr-xr-x   0 karin      (501) staff       (20)        0 2024-02-11 23:26:10.198489 pyei-1.1.0/pyei.egg-info/
+-rw-r--r--   0 karin      (501) staff       (20)     6020 2024-02-11 23:26:10.000000 pyei-1.1.0/pyei.egg-info/PKG-INFO
+-rw-r--r--   0 karin      (501) staff       (20)      392 2024-02-11 23:26:10.000000 pyei-1.1.0/pyei.egg-info/SOURCES.txt
+-rw-r--r--   0 karin      (501) staff       (20)        1 2024-02-11 23:26:10.000000 pyei-1.1.0/pyei.egg-info/dependency_links.txt
+-rw-r--r--   0 karin      (501) staff       (20)      106 2024-02-11 23:26:10.000000 pyei-1.1.0/pyei.egg-info/requires.txt
+-rw-r--r--   0 karin      (501) staff       (20)        5 2024-02-11 23:26:10.000000 pyei-1.1.0/pyei.egg-info/top_level.txt
+-rw-r--r--   0 karin      (501) staff       (20)       38 2024-02-11 23:26:10.198911 pyei-1.1.0/setup.cfg
+-rw-r--r--   0 karin      (501) staff       (20)     1364 2024-02-11 20:35:26.000000 pyei-1.1.0/setup.py
```

### Comparing `pyei-1.0.1/LICENSE` & `pyei-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyei-1.0.1/PKG-INFO` & `pyei-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: pyei
-Version: 1.0.1
-Home-page: https://github.com/mggg/ecological-inference
-Author: Metric Geometry and Gerrymandering Group
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyEI
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03397/status.svg)](https://doi.org/10.21105/joss.03397)
 
 PyEI is a Python library for ecological inference. The target audience is the analyst with an interest in the phenomenon called Racially Polarized Voting.
 
 Racially Polarized Voting is a legal concept developed through case law under the Voting Rights Act of 1965; its genesis is in the majority opinion of ***Thornburg v. Gingles (1982)***. Considered the “evidentiary linchpin” for vote dilution cases, RPV is a necessary, but not sufficient, condition that plaintiffs must satisfy for a valid claim. 
@@ -61,15 +53,15 @@
 Feel free to file an issue if you are running into trouble or if there is a feature you'd particularly like to see, and we will do our best to get to it!
 
 
 ## Want to contribute to PyEI? Start here.
 
 Contributions are welcome! 
 
-Uses Python>=3.7. After cloning the environment, you should be able to use either `virtualenv` or `conda` to run the code. The second (`conda`) is probably easier for development, but `virtualenv` is used for the project's CI.
+Uses Python 3.10. After cloning the environment, you should be able to use either `virtualenv` or `conda` to run the code. The second (`conda`) is probably easier for development, but `virtualenv` is used for the project's CI.
 
 Here is how to create and activate each environment. See the docs for more elaborate details:
 
 ### Install with virtualenv
 
 ```bash
 virtualenv pyei_venv           # create virtualenv
@@ -78,15 +70,16 @@
 python -m pip install -e .     # install project locally
 python -m pip install -r requirements-dev.txt  # install dev requirements
 ```
 
 ### Install with conda
 
 ```bash
-conda create --name pyei --channel conda-forge python=3.8 --file requirements.txt --file requirements-dev.txt # create conda environment and install requirements
+conda create --name pyei --channel conda-forge python=3.10 --file requirements.txt --file requirements-dev.txt # create conda environment and install requirements
+conda activate pyei
 pip install -e . #install project locally
 ```
 
 ### Testing
 
 After making changes, make sure everything works by running
```

### Comparing `pyei-1.0.1/README.md` & `pyei-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: pyei
+Version: 1.1.0
+Home-page: https://github.com/mggg/ecological-inference
+Author: Metric Geometry and Gerrymandering Group
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pymc>=5.10.0
+Requires-Dist: arviz
+Requires-Dist: scikit-learn
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: seaborn
+Requires-Dist: graphviz
+Requires-Dist: numpy
+Requires-Dist: jax
+Requires-Dist: numpyro
+Requires-Dist: jaxlib
+Requires-Dist: numba
+Requires-Dist: netCDF4
+
 # PyEI
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03397/status.svg)](https://doi.org/10.21105/joss.03397)
 
 PyEI is a Python library for ecological inference. The target audience is the analyst with an interest in the phenomenon called Racially Polarized Voting.
 
 Racially Polarized Voting is a legal concept developed through case law under the Voting Rights Act of 1965; its genesis is in the majority opinion of ***Thornburg v. Gingles (1982)***. Considered the “evidentiary linchpin” for vote dilution cases, RPV is a necessary, but not sufficient, condition that plaintiffs must satisfy for a valid claim. 
@@ -53,15 +74,15 @@
 Feel free to file an issue if you are running into trouble or if there is a feature you'd particularly like to see, and we will do our best to get to it!
 
 
 ## Want to contribute to PyEI? Start here.
 
 Contributions are welcome! 
 
-Uses Python>=3.7. After cloning the environment, you should be able to use either `virtualenv` or `conda` to run the code. The second (`conda`) is probably easier for development, but `virtualenv` is used for the project's CI.
+Uses Python 3.10. After cloning the environment, you should be able to use either `virtualenv` or `conda` to run the code. The second (`conda`) is probably easier for development, but `virtualenv` is used for the project's CI.
 
 Here is how to create and activate each environment. See the docs for more elaborate details:
 
 ### Install with virtualenv
 
 ```bash
 virtualenv pyei_venv           # create virtualenv
@@ -70,15 +91,16 @@
 python -m pip install -e .     # install project locally
 python -m pip install -r requirements-dev.txt  # install dev requirements
 ```
 
 ### Install with conda
 
 ```bash
-conda create --name pyei --channel conda-forge python=3.8 --file requirements.txt --file requirements-dev.txt # create conda environment and install requirements
+conda create --name pyei --channel conda-forge python=3.10 --file requirements.txt --file requirements-dev.txt # create conda environment and install requirements
+conda activate pyei
 pip install -e . #install project locally
 ```
 
 ### Testing
 
 After making changes, make sure everything works by running
```

### Comparing `pyei-1.0.1/pyei/data.py` & `pyei-1.1.0/pyei/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helpers for managing data files."""
+
 from dataclasses import dataclass
 
 import pandas as pd
 
 __all__ = ["Datasets"]
```

### Comparing `pyei-1.0.1/pyei/distribution_utils.py` & `pyei-1.1.0/pyei/distribution_utils.py`

 * *Files identical despite different names*

### Comparing `pyei-1.0.1/pyei/goodmans_er.py` & `pyei-1.1.0/pyei/goodmans_er.py`

 * *Files identical despite different names*

### Comparing `pyei-1.0.1/pyei/greiner_quinn_gibbs_sampling.py` & `pyei-1.1.0/pyei/greiner_quinn_gibbs_sampling.py`

 * *Files identical despite different names*

### Comparing `pyei-1.0.1/pyei/io_utils.py` & `pyei-1.1.0/pyei/io_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,17 @@
             "precinct_pops",
             "precinct_names",
             "demographic_group_name",
             "candidate_name",
             "demographic_group_fraction",
             "votes_fraction",
         ]
-        ei_object.sim_trace.posterior.attrs[
-            "is_two_by_two"
-        ] = "true"  # store whether 2 by 2 or r by c
+        ei_object.sim_trace.posterior.attrs["is_two_by_two"] = (
+            "true"  # store whether 2 by 2 or r by c
+        )
 
     else:  # r by c
         # attr_list=[]
         attr_list = [
             "model_name",
             "precinct_pops",
             "precinct_names",
```

### Comparing `pyei-1.0.1/pyei/plot_utils.py` & `pyei-1.1.0/pyei/plot_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Plotting functions for visualizing ei outputs
 
 """
+
 import warnings
 import seaborn as sns
 import pandas as pd
 from matplotlib import pyplot as plt
 from matplotlib import ticker as mticker
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Rectangle
```

### Comparing `pyei-1.0.1/pyei/r_by_c.py` & `pyei-1.1.0/pyei/r_by_c.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 equal to 2
 
 TODO: Investigate better or reparametrized priors for multinomial-dir
 TODO: Greiner-Quinn Model
 TODO: Refactor to integrate with two_by_two
 """
 
-
 import warnings
 from pymc import sampling_jax
 import numpy as np
 from .plot_utils import (
     plot_boxplots,
     plot_kdes,
     plot_intervals_all_precincts,
@@ -299,18 +298,18 @@
         # # compute credible intervals
         percentiles = [2.5, 97.5]
         self.turnout_adjusted_credible_interval_95_mean_voting_prefs = np.zeros(
             (self.num_groups_and_num_candidates[0], self.num_groups_and_num_candidates[1] - 1, 2)
         )
         for row in range(self.num_groups_and_num_candidates[0]):
             for col in range(self.num_groups_and_num_candidates[1] - 1):
-                self.turnout_adjusted_credible_interval_95_mean_voting_prefs[row][col][
-                    :
-                ] = np.percentile(
-                    self.turnout_adjusted_sampled_voting_prefs[:, row, col], percentiles
+                self.turnout_adjusted_credible_interval_95_mean_voting_prefs[row][col][:] = (
+                    np.percentile(
+                        self.turnout_adjusted_sampled_voting_prefs[:, row, col], percentiles
+                    )
                 )
 
     def calculate_summary(self):
         """Calculate point estimates (post. means) and 95% equal-tailed credible intervals
 
         Sets
             self.sampled_voting_prefs
```

### Comparing `pyei-1.0.1/pyei/r_by_c_models.py` & `pyei-1.1.0/pyei/r_by_c_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Functions that return pymc models for RowByColumnEI
 """
 
 import pymc as pm
-import aesara.tensor as at
+import pytensor.tensor as at
 import numpy as np
 
 __all__ = ["ei_multinom_dirichlet_modified", "ei_multinom_dirichlet"]
 
 
 def ei_multinom_dirichlet(group_fractions, votes_fractions, precinct_pops, lmbda1=4, lmbda2=2):
     """
```

### Comparing `pyei-1.0.1/pyei/r_by_c_utils.py` & `pyei-1.1.0/pyei/r_by_c_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utilities for RowByColumnEI
 """
+
 import warnings
 
 
 def check_dimensions_of_input(
     group_fractions,
     votes_fractions,
     precinct_pops,
```

### Comparing `pyei-1.0.1/pyei/two_by_two.py` & `pyei-1.1.0/pyei/two_by_two.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 """
 
 import warnings
 import pymc as pm
 from pymc import sampling_jax
 import numpy as np
-import aesara.tensor as at
-import aesara
+import pytensor.tensor as at
+import pytensor
 from .plot_utils import (
     plot_conf_or_credible_interval,
     plot_boxplots,
     plot_kdes,
     plot_precincts,
     plot_polarization_kde,
     plot_summary,
@@ -103,17 +103,15 @@
             "sigma_i_sq",
             sigma_lower**2
             + 2 * (sigma_12 - sigma_lower**2) * group_fraction
             + (sigma_upper * 2 + sigma_lower**2 - 2 * sigma_12) * group_fraction**2,
         )
 
         votes_frac_mean = mu_i + w_i * (upper_b - tn_mean_upper) / (sigma_upper**2)
-        votes_frac_var = pm.Deterministic(
-            "votes_frac_var", sigma_i_sq - w_i**2 / (sigma_upper**2)
-        )
+        votes_frac_var = pm.Deterministic("votes_frac_var", sigma_i_sq - w_i**2 / (sigma_upper**2))
 
         votes_frac_l_bound = group_fraction * upper_b
         votes_frac_u_bound = (1 - group_fraction) + group_fraction * upper_b
 
         votes_frac_stdev = pm.math.sqrt(votes_frac_var)
         pm.TruncatedNormal(
             "votes_fraction",
@@ -284,15 +282,15 @@
     A theano tensor giving the log probability of b_1, b_2 (given the other parameters)
 
     Notes
     -----
     See Wakefield 2004 equation 4
     """
 
-    result, _ = aesara.scan(
+    result, _ = pytensor.scan(
         fn=log_binom_sum,
         outputs_info={"taps": [-1], "initial": at.as_tensor(np.array([0.0]))},
         sequences=[
             at.as_tensor(lower),
             at.as_tensor(upper),
             at.as_tensor(obs_votes),
             at.as_tensor(n_0),
```

### Comparing `pyei-1.0.1/pyei.egg-info/PKG-INFO` & `pyei-1.1.0/pyei.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 Metadata-Version: 2.1
 Name: pyei
-Version: 1.0.1
+Version: 1.1.0
 Home-page: https://github.com/mggg/ecological-inference
 Author: Metric Geometry and Gerrymandering Group
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymc>=5.10.0
+Requires-Dist: arviz
+Requires-Dist: scikit-learn
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: seaborn
+Requires-Dist: graphviz
+Requires-Dist: numpy
+Requires-Dist: jax
+Requires-Dist: numpyro
+Requires-Dist: jaxlib
+Requires-Dist: numba
+Requires-Dist: netCDF4
 
 # PyEI
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03397/status.svg)](https://doi.org/10.21105/joss.03397)
 
 PyEI is a Python library for ecological inference. The target audience is the analyst with an interest in the phenomenon called Racially Polarized Voting.
 
@@ -61,15 +74,15 @@
 Feel free to file an issue if you are running into trouble or if there is a feature you'd particularly like to see, and we will do our best to get to it!
 
 
 ## Want to contribute to PyEI? Start here.
 
 Contributions are welcome! 
 
-Uses Python>=3.7. After cloning the environment, you should be able to use either `virtualenv` or `conda` to run the code. The second (`conda`) is probably easier for development, but `virtualenv` is used for the project's CI.
+Uses Python 3.10. After cloning the environment, you should be able to use either `virtualenv` or `conda` to run the code. The second (`conda`) is probably easier for development, but `virtualenv` is used for the project's CI.
 
 Here is how to create and activate each environment. See the docs for more elaborate details:
 
 ### Install with virtualenv
 
 ```bash
 virtualenv pyei_venv           # create virtualenv
@@ -78,15 +91,16 @@
 python -m pip install -e .     # install project locally
 python -m pip install -r requirements-dev.txt  # install dev requirements
 ```
 
 ### Install with conda
 
 ```bash
-conda create --name pyei --channel conda-forge python=3.8 --file requirements.txt --file requirements-dev.txt # create conda environment and install requirements
+conda create --name pyei --channel conda-forge python=3.10 --file requirements.txt --file requirements-dev.txt # create conda environment and install requirements
+conda activate pyei
 pip install -e . #install project locally
 ```
 
 ### Testing
 
 After making changes, make sure everything works by running
```

### Comparing `pyei-1.0.1/setup.py` & `pyei-1.1.0/setup.py`

 * *Files identical despite different names*

