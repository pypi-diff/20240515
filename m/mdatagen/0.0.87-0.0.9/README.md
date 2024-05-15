# Comparing `tmp/mdatagen-0.0.87.tar.gz` & `tmp/mdatagen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdatagen-0.0.87.tar", last modified: Wed Jan 10 14:31:40 2024, max compression
+gzip compressed data, was "mdatagen-0.0.9.tar", last modified: Wed May 15 14:47:14 2024, max compression
```

## Comparing `mdatagen-0.0.87.tar` & `mdatagen-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-01-10 14:31:40.901199 mdatagen-0.0.87/
--rw-rw-rw-   0        0        0     1096 2023-12-23 12:24:58.000000 mdatagen-0.0.87/LICENSE
--rw-rw-rw-   0        0        0     3411 2024-01-10 14:31:40.901199 mdatagen-0.0.87/PKG-INFO
--rw-rw-rw-   0        0        0     2991 2024-01-10 14:29:27.000000 mdatagen-0.0.87/README.md
-drwxrwxrwx   0        0        0        0 2024-01-10 14:31:40.871713 mdatagen-0.0.87/mdatagen/
--rw-rw-rw-   0        0        0        0 2023-12-23 12:24:58.000000 mdatagen-0.0.87/mdatagen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 14:31:40.883576 mdatagen-0.0.87/mdatagen/multivariate/
--rw-rw-rw-   0        0        0        0 2023-12-23 12:24:58.000000 mdatagen-0.0.87/mdatagen/multivariate/__init__.py
--rw-rw-rw-   0        0        0     8210 2023-12-24 20:21:03.000000 mdatagen-0.0.87/mdatagen/multivariate/mMAR.py
--rw-rw-rw-   0        0        0     4151 2023-12-24 20:20:58.000000 mdatagen-0.0.87/mdatagen/multivariate/mMCAR.py
--rw-rw-rw-   0        0        0    21709 2023-12-24 20:20:54.000000 mdatagen-0.0.87/mdatagen/multivariate/mMNAR.py
-drwxrwxrwx   0        0        0        0 2024-01-10 14:31:40.897052 mdatagen-0.0.87/mdatagen/univariate/
--rw-rw-rw-   0        0        0        0 2023-12-23 12:24:58.000000 mdatagen-0.0.87/mdatagen/univariate/__init__.py
--rw-rw-rw-   0        0        0     8008 2023-12-24 20:21:13.000000 mdatagen-0.0.87/mdatagen/univariate/uMAR.py
--rw-rw-rw-   0        0        0     4710 2023-12-24 20:21:18.000000 mdatagen-0.0.87/mdatagen/univariate/uMCAR.py
--rw-rw-rw-   0        0        0     4278 2023-12-24 20:21:26.000000 mdatagen-0.0.87/mdatagen/univariate/uMNAR.py
-drwxrwxrwx   0        0        0        0 2024-01-10 14:31:40.900243 mdatagen-0.0.87/mdatagen/utils/
--rw-rw-rw-   0        0        0        0 2023-12-23 12:24:58.000000 mdatagen-0.0.87/mdatagen/utils/__init__.py
--rw-rw-rw-   0        0        0     6049 2023-12-24 20:21:38.000000 mdatagen-0.0.87/mdatagen/utils/feature_choice.py
--rw-rw-rw-   0        0        0     3885 2023-12-24 20:21:45.000000 mdatagen-0.0.87/mdatagen/utils/math_calcs.py
-drwxrwxrwx   0        0        0        0 2024-01-10 14:31:40.883576 mdatagen-0.0.87/mdatagen.egg-info/
--rw-rw-rw-   0        0        0     3411 2024-01-10 14:31:40.000000 mdatagen-0.0.87/mdatagen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2024-01-10 14:31:40.000000 mdatagen-0.0.87/mdatagen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-10 14:31:40.000000 mdatagen-0.0.87/mdatagen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-01-10 14:31:40.000000 mdatagen-0.0.87/mdatagen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-10 14:31:40.000000 mdatagen-0.0.87/mdatagen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-01-10 14:31:40.901199 mdatagen-0.0.87/setup.cfg
--rw-rw-rw-   0        0        0      807 2024-01-10 14:29:43.000000 mdatagen-0.0.87/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:14.850809 mdatagen-0.0.9/
+-rw-rw-rw-   0        0        0     1096 2023-12-23 12:24:58.000000 mdatagen-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3484 2024-05-15 14:47:14.850809 mdatagen-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3062 2024-02-16 16:08:26.000000 mdatagen-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:14.826645 mdatagen-0.0.9/mdatagen/
+-rw-rw-rw-   0        0        0      202 2024-02-16 16:19:58.000000 mdatagen-0.0.9/mdatagen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:14.835162 mdatagen-0.0.9/mdatagen/multivariate/
+-rw-rw-rw-   0        0        0        0 2023-12-23 12:24:58.000000 mdatagen-0.0.9/mdatagen/multivariate/__init__.py
+-rw-rw-rw-   0        0        0     8579 2024-05-15 13:03:59.000000 mdatagen-0.0.9/mdatagen/multivariate/mMAR.py
+-rw-rw-rw-   0        0        0     4433 2024-05-15 13:03:12.000000 mdatagen-0.0.9/mdatagen/multivariate/mMCAR.py
+-rw-rw-rw-   0        0        0    22202 2024-05-15 14:37:06.000000 mdatagen-0.0.9/mdatagen/multivariate/mMNAR.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:14.835162 mdatagen-0.0.9/mdatagen/univariate/
+-rw-rw-rw-   0        0        0        0 2023-12-23 12:24:58.000000 mdatagen-0.0.9/mdatagen/univariate/__init__.py
+-rw-rw-rw-   0        0        0     7985 2024-05-15 14:14:12.000000 mdatagen-0.0.9/mdatagen/univariate/uMAR.py
+-rw-rw-rw-   0        0        0     4689 2024-02-16 16:30:54.000000 mdatagen-0.0.9/mdatagen/univariate/uMCAR.py
+-rw-rw-rw-   0        0        0     4257 2024-02-16 16:31:00.000000 mdatagen-0.0.9/mdatagen/univariate/uMNAR.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:14.835162 mdatagen-0.0.9/mdatagen/utils/
+-rw-rw-rw-   0        0        0        0 2023-12-23 12:24:58.000000 mdatagen-0.0.9/mdatagen/utils/__init__.py
+-rw-rw-rw-   0        0        0     5951 2024-02-16 16:31:08.000000 mdatagen-0.0.9/mdatagen/utils/feature_choice.py
+-rw-rw-rw-   0        0        0     3826 2024-05-15 13:55:59.000000 mdatagen-0.0.9/mdatagen/utils/math_calcs.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:14.835162 mdatagen-0.0.9/mdatagen.egg-info/
+-rw-rw-rw-   0        0        0     3484 2024-05-15 14:47:14.000000 mdatagen-0.0.9/mdatagen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2024-05-15 14:47:14.000000 mdatagen-0.0.9/mdatagen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:47:14.000000 mdatagen-0.0.9/mdatagen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-15 14:47:14.000000 mdatagen-0.0.9/mdatagen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 14:47:14.000000 mdatagen-0.0.9/mdatagen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-15 14:47:14.850809 mdatagen-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      809 2024-05-15 14:24:29.000000 mdatagen-0.0.9/setup.py
```

### Comparing `mdatagen-0.0.87/LICENSE` & `mdatagen-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mdatagen-0.0.87/PKG-INFO` & `mdatagen-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mdatagen
-Version: 0.0.87
+Version: 0.0.9
 Summary: mdatagen: A Python Library for the Generation of Artificial Missing Data
 Home-page: https://github.com/ArthurMangussi/pymdatagen
 Author: Arthur Dantas Mangussi
 Author-email: mangussiarthur@gmail.com
 License: MIT
 Keywords: machine learning,preprocessing data
-Requires-Python: >=3.11
+Requires-Python: >=3.10.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mdatagen: A Python Library for the Generation of Artificial Missing Data
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
 [![Documentation](https://img.shields.io/badge/Documentation-Link-green.svg)](docs/)
@@ -30,29 +30,30 @@
 To install the package, please use the `pip` installation as follows:
 
 ```bash
 pip install mdatagen
 ```
 
 ### Usage examples
-For examples on how to use the mdatagen package, from basic examples that generate artificial missing data under a mechanism to complete examples using Multiple Imputation by Chained Equations (MICE) from scikit-learn for imputation, follow this [examples](examples/).
+For examples on how to use the mdatagen package, from basic examples that generate artificial missing data under a mechanism to complete examples using Multiple Imputation by Chained Equations (MICE) from scikit-learn for imputation, follow these [examples](examples/).
 
 
 ## Contribuitions
 Contributions are welcome! Feel free to open issues, submit pull requests, or provide feedback.
 
 ## Citation
-If you use **mdatagen** in your research, please cite the [mdatagen paper]()
+If you use **mdatagen** in your research, please cite the [original paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8605316)
 
 Bibtex entry:
 ```bash
-@article{mdatagen2024,
-  author  = {Arthur D Mangussi and Filipe Loyola Lopes and Miriam Seone Santos and Ricardo Cardoso Pereira and Ana Carolina Lorena and Pedro Henriques Abreu},
-  title   = {mdatagen: A Python Library for the Generation of Artificial Missing Data},
-  journal = {Journal of Machine Learning Research},
-  year    = {2024},
-  volume  = {24},
-  pages   = {1--6},
-}
+@ARTICLE{Santos2019,
+  author={Santos, Miriam Seoane and Pereira, Ricardo Cardoso and Costa, Adriana Fonseca and Soares, Jastin Pompeu and Santos, João and Abreu, Pedro Henriques},
+  journal={IEEE Access}, 
+  title={Generating Synthetic Missing Data: A Review by Missing Mechanism}, 
+  year={2019},
+  volume={7},
+  number={},
+  pages={11651-11667},
+  doi={10.1109/ACCESS.2019.2891360}}
 ```
 ## Acknowledgements
 The authors gratefully acknowledge the Brazilian funding agencies FAPESP (Fundação Amparo à Pesquisa do Estado de São Paulo) under grants 2022/10553-6, and 2021/06870-3. Moreover, this research was supported in part by the Coordenação de Aperfeiçoamento de Pessoalde Nível Superior - Brasil (CAPES) - Finance Code 001, and Portuguese Recovery and Resilience Plan (PRR) through project C645008882-00000055 Center for Responsable AI.
```

### Comparing `mdatagen-0.0.87/README.md` & `mdatagen-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,29 +17,30 @@
 To install the package, please use the `pip` installation as follows:
 
 ```bash
 pip install mdatagen
 ```
 
 ### Usage examples
-For examples on how to use the mdatagen package, from basic examples that generate artificial missing data under a mechanism to complete examples using Multiple Imputation by Chained Equations (MICE) from scikit-learn for imputation, follow this [examples](examples/).
+For examples on how to use the mdatagen package, from basic examples that generate artificial missing data under a mechanism to complete examples using Multiple Imputation by Chained Equations (MICE) from scikit-learn for imputation, follow these [examples](examples/).
 
 
 ## Contribuitions
 Contributions are welcome! Feel free to open issues, submit pull requests, or provide feedback.
 
 ## Citation
-If you use **mdatagen** in your research, please cite the [mdatagen paper]()
+If you use **mdatagen** in your research, please cite the [original paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8605316)
 
 Bibtex entry:
 ```bash
-@article{mdatagen2024,
-  author  = {Arthur D Mangussi and Filipe Loyola Lopes and Miriam Seone Santos and Ricardo Cardoso Pereira and Ana Carolina Lorena and Pedro Henriques Abreu},
-  title   = {mdatagen: A Python Library for the Generation of Artificial Missing Data},
-  journal = {Journal of Machine Learning Research},
-  year    = {2024},
-  volume  = {24},
-  pages   = {1--6},
-}
+@ARTICLE{Santos2019,
+  author={Santos, Miriam Seoane and Pereira, Ricardo Cardoso and Costa, Adriana Fonseca and Soares, Jastin Pompeu and Santos, João and Abreu, Pedro Henriques},
+  journal={IEEE Access}, 
+  title={Generating Synthetic Missing Data: A Review by Missing Mechanism}, 
+  year={2019},
+  volume={7},
+  number={},
+  pages={11651-11667},
+  doi={10.1109/ACCESS.2019.2891360}}
 ```
 ## Acknowledgements
 The authors gratefully acknowledge the Brazilian funding agencies FAPESP (Fundação Amparo à Pesquisa do Estado de São Paulo) under grants 2022/10553-6, and 2021/06870-3. Moreover, this research was supported in part by the Coordenação de Aperfeiçoamento de Pessoalde Nível Superior - Brasil (CAPES) - Finance Code 001, and Portuguese Recovery and Resilience Plan (PRR) through project C645008882-00000055 Center for Responsable AI.
```

### Comparing `mdatagen-0.0.87/mdatagen/multivariate/mMAR.py` & `mdatagen-0.0.9/mdatagen/multivariate/mMAR.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  =============================================================================
 # Aeronautics Institute of Technologies (ITA) - Brazil
 # University of Coimbra (UC) - Portugal
 # Arthur Dantas Mangussi - mangussiarthur@gmail.com
 # =============================================================================
 
 __author__ = 'Arthur Dantas Mangussi'
-__version__ = '0.0.8'
+
 
 import warnings
 
 import numpy as np
 import pandas as pd
 from mdatagen.utils.feature_choice import FeatureChoice
 from mdatagen.utils.math_calcs import MathCalcs
@@ -22,37 +22,41 @@
     """
     A class to generate missing data in a dataset based on the Missing At Random (MAR) mechanism for multiple features simultaneously.
 
     Args:
         X (pd.DataFrame): The dataset to receive the missing data.
         y (np.array): The label values from dataset
         n_xmiss (int): The number of features in the dataset that will receive missing values. Default is 2.
+        missTarget (bool, optional): A flag to generate missing into the target.
 
     Example Usage:
 
     ```python
     # Create an instance of the MAR class
-    generator = MAR(X, y, missing_rate=20, n_xmiss=4)
+    generator = MAR(X, y, n_xmiss=4)
 
     # Generate missing values using the random strategy
     data_md = generator.random(missing_rate = 20)
     ```
     """
 
-    def __init__(self, X: pd.DataFrame, y: np.array, n_xmiss: int = 2):
+    def __init__(self, X: pd.DataFrame, y: np.array, n_xmiss: int = 2, missTarget:bool=False):
         if not isinstance(X, pd.DataFrame):
             raise TypeError('Dataset must be a Pandas Dataframe')
         if not isinstance(y, np.ndarray):
             raise TypeError('y must be a numpy array')
 
         self.n_xmiss = n_xmiss
         self.X = X
         self.y = y
         self.dataset = self.X.copy()
-        self.dataset['target'] = y
+        self.missTarget = missTarget
+
+        if missTarget:
+            self.dataset['target'] = y
 
     def random(self, missing_rate: int = 10) -> pd.DataFrame:
         """
         Function to generate arficial missing data in n_xmiss features chosen randomly.
         The lower values in observed feature for each feature x_miss will determine
         the miss locations in x_miss.
 
@@ -103,14 +107,16 @@
             if x_miss not in xmiss_multiva:
                 pos_xmiss = self.dataset[x_obs].sort_values()[:N].index
                 self.dataset.loc[pos_xmiss, x_miss] = np.nan
 
                 xmiss_multiva.append(x_miss)
                 cont += 1
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
 
     def correlated(self, missing_rate: int = 10) -> pd.DataFrame:
         """
         Function to generate missing data in features from dataset, except the class (target).
         The lower values in observed feature for each correlated pair will determine the
         miss locations in feature x_miss.
@@ -155,14 +161,16 @@
                 x_obs = set(pair).difference(x_miss).pop()
                 cutK = 1.5 * mr
 
             N = round(len(self.dataset) * cutK)
             pos_xmiss = self.dataset[x_obs].sort_values()[:N].index
             self.dataset.loc[pos_xmiss, x_miss] = np.nan
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
 
     def median(self, missing_rate: int = 10) -> pd.DataFrame:
         """
         Function to generate missing data in features from dataset.
         The median in observed feature for each correlated pair will create two groups.
         The group is chosen randomly, and lower values will determine the miss locations
@@ -223,8 +231,10 @@
                 pos_xmiss = g1.sort_values()[:N].index
 
             else:
                 pos_xmiss = g2.sort_values()[:N].index
 
             self.dataset.loc[pos_xmiss, x_miss] = np.nan
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
```

### Comparing `mdatagen-0.0.87/mdatagen/multivariate/mMCAR.py` & `mdatagen-0.0.9/mdatagen/multivariate/mMCAR.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # =============================================================================
 # Aeronautics Institute of Technologies (ITA) - Brazil
 # University of Coimbra (UC) - Portugal
 # Arthur Dantas Mangussi - mangussiarthur@gmail.com
 # =============================================================================
 
 __author__ = 'Arthur Dantas Mangussi'
-__version__ = '0.0.8'
+
 
 import warnings
 
 import numpy as np
 import pandas as pd
 
 
@@ -20,26 +20,27 @@
     """
     A class to generate missing data in a dataset based on the Missing Completely At Random (MCAR) mechanism for multiple features simultaneously.
 
     Args:
         X (pd.DataFrame): The dataset to receive the missing data.
         y (np.array): The label values from dataset
         missing_rate (int, optional): The rate of missing data to be generated. Default is 10.
+        missTarget (bool, optional): A flag to generate missing into the target.
 
     Example Usage:
     ```python
     # Create an instance of the MCAR class
     generator = MCAR(X, y, missing_rate=20)
 
     # Generate missing values using the random strategy
     data_md = generator.random()
     ```
     """
 
-    def __init__(self, X: pd.DataFrame, y: np.array, missing_rate: int = 10):
+    def __init__(self, X: pd.DataFrame, y: np.array, missing_rate: int = 10, missTarget:bool=False):
         if not isinstance(X, pd.DataFrame):
             raise TypeError('Dataset must be a Pandas Dataframe')
         if not isinstance(y, np.ndarray):
             raise TypeError('y must be a numpy array')
 
         if missing_rate >= 100:
             raise ValueError(
@@ -47,15 +48,19 @@
             )
         elif missing_rate < 0:
             raise ValueError('Missing rate must be between [0,100]')
 
         self.X = X
         self.y = y
         self.dataset = self.X.copy()
-        self.dataset['target'] = y
+        self.missing_rate = missing_rate
+        self.missTarget = missTarget
+
+        if missTarget:
+            self.dataset['target'] = y
 
     def random(self) -> pd.DataFrame:
         """
         Function to randomly generate missing data in all dataset.
 
         Returns:
             dataset (DataFrame): The dataset with missing values generated under
@@ -112,8 +117,11 @@
             )
 
         for x_miss in columns:
             pos_xmiss = np.random.binomial(
                 n=1, p=self.missing_rate / 100, size=self.dataset.shape[0]
             ).astype(bool)
             self.dataset.loc[pos_xmiss, x_miss] = np.nan
+        
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
```

### Comparing `mdatagen-0.0.87/mdatagen/multivariate/mMNAR.py` & `mdatagen-0.0.9/mdatagen/multivariate/mMNAR.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # =============================================================================
 # Aeronautics Institute of Technologies (ITA) - Brazil
 # University of Coimbra (UC) - Portugal
 # Arthur Dantas Mangussi - mangussiarthur@gmail.com
 # =============================================================================
 
 __author__ = 'Arthur Dantas Mangussi'
-__version__ = '0.0.8'
+
 
 import warnings
 
 import numpy as np
 import pandas as pd
 from scipy.stats import mannwhitneyu
 from mdatagen.utils.feature_choice import FeatureChoice
@@ -26,14 +26,15 @@
         X (pd.DataFrame): The dataset to receive the missing data.
         y (np.array): The label values from dataset
         missing_rate (int, optional): The rate of missing data to be generated. Default is 10.
 
     Keyword Args:
         n_xmiss (int, optional): The number of features in the dataset that will receive missing values. Default is the number of features in dataset.
         threshold (float, optional): The threshold to select the locations in feature (xmiss) to receive missing values where 0 indicates de lowest and 1 highest values. Default is 0
+        missTarget (bool, optional): A flag to generate missing into the target.
 
     Example Usage:
     ```python
     # Create an instance of the MNAR class
     generator = MNAR(X, y)
 
     # Generate missing values using the random strategy
@@ -45,21 +46,25 @@
         if not isinstance(X, pd.DataFrame):
             raise TypeError('Dataset must be a Pandas Dataframe')
         if not isinstance(y, np.ndarray):
             raise TypeError('y must be a numpy array')
         self.X = X
         self.y = y
         self.dataset = self.X.copy()
-        self.dataset['target'] = y
+        self.missTarget = kwargs.get('missTarget', False)
+
+        if self.missTarget:
+            self.dataset['target'] = y
 
         self.n = self.dataset.shape[0]
         self.p = self.dataset.shape[1]
 
         self.n_xmiss = kwargs.get('n_xmiss', self.p)
         self.threshold = kwargs.get('threshold', 0)
+               
 
     def random(self, missing_rate: int = 10, deterministic:bool = False):
         """
         Function to randomly choose the feature (x_miss) in dataset for generate missing
         data. The miss locations on x_miss is the lower values based on unobserved feature
         or feature x_miss itself.
 
@@ -125,14 +130,16 @@
 
                 self.dataset.loc[pos_xmiss, x_miss] = np.nan
 
                 xmiss_multiva.append(x_miss)
                 options_xmiss.remove(x_miss)
                 cont += 1
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
 
     def correlated(self, missing_rate: int = 10, deterministic:bool = False):
         """
         Function to generate missing data in dataset based on correlated pair.
         The feature (x_miss) most correlated with the class for each pair will
         receive the missing data based on lower values of an unobserved feature
@@ -194,14 +201,16 @@
                 ordered_id = np.lexsort((np.random.random(x_f.size), x_f))
                 pos_xmiss = FeatureChoice.miss_locations(
                 ordered_id, self.threshold, N
             )
 
             self.dataset.loc[pos_xmiss, x_miss] = np.nan
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
 
     def median(self, missing_rate: int = 10, deterministic:bool = False):
         """
         Function to generate missing data in all dataset based on median from
         each feature. The miss locations are chosen by lower values from a unobserved feature
         or feature x_miss itself.
@@ -227,48 +236,38 @@
                 'Features will be all NaN, you should decrease the missing rate'
             )
 
         mr = missing_rate / 100
 
         # For each column in dataset
         for col in self.dataset.columns:
-            cutK = 2 * mr
-            N = round(len(self.dataset) * cutK)
+            N = round(len(self.dataset) * mr)
 
             if len(self.dataset[col].unique()) == 2:  # Binary feature
                 g1_index = np.random.choice(
                     self.dataset[col].index,
                     round(len(self.dataset) / 2),
                     replace=False,
                 )
-                g2_index = np.random.choice(
-                    self.dataset[col].index,
-                    round(len(self.dataset) / 2),
-                    replace=False,
-                )
+                g2_index = np.array([i for i in self.dataset[col].index if i not in g1_index])
 
             else:  # Continuos or ordinal feature
                 median_xobs = self.dataset[col].median()
 
                 g1 = self.dataset[col][self.dataset[col] <= median_xobs]
                 g2 = self.dataset[col][self.dataset[col] > median_xobs]
 
-                if len(g1) != len(
-                    g2
-                ):  # If median do not divide in equal-size groups
+                # If median do not divide in equal-size groups
+                if len(g1) != len(g2):  
                     g1_index = np.random.choice(
                         self.dataset[col].index,
                         round(len(self.dataset) / 2),
                         replace=False,
                     )
-                    g2_index = np.random.choice(
-                        self.dataset[col].index,
-                        round(len(self.dataset) / 2),
-                        replace=False,
-                    )
+                    g2_index = np.array([i for i in self.dataset[col].index if i not in g1_index])
                 else:
                     g1_index = g1.index
                     g2_index = g2.index
 
             choice = np.random.choice([0, 1])
             if choice == 0:
                 x_f = self.dataset.loc[g1_index, col].values
@@ -287,14 +286,16 @@
                 ordered_id = np.lexsort((np.random.random(x_f.size), x_f))
                 pos_xmiss = FeatureChoice.miss_locations(
                 ordered_id, self.threshold, N
             )
 
             self.dataset.loc[pos_xmiss, col] = np.nan
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
 
     def MBOUV(
         self, missing_rate: int = 10, depend_on_external=None, ascending=True
     ):
         """
         Function to generate missing data based on Missigness Based on Own and Unobserved Values (MBOUV).
@@ -303,17 +304,17 @@
             missing_rate (int, optional): The rate of missing data to be generated. Default is 10.
 
         Returns:
             dataset (DataFrame): The dataset with missing values generated under
             the MNAR mechanism.
 
         Reference:
-        [2] R. C. Pereira, P. H. Abreu, P. P. Rodrigues, and M. A. T. Figuereido. 2023.
-        Imputation of Data Missing Not At Random:Artificial Generation and Benchmark
-        Analysis. Submitted to Expert Systems with Applications.
+        [2] Pereira, R. C., Abreu, P. H., Rodrigues, P. P., Figueiredo, M. A. T., (2024). 
+        Imputation of data Missing Not at Random: Artificial generation and benchmark analysis. 
+        Expert Systems with Applications, 249(B), 123654.
 
 
         """
 
         if depend_on_external is None:
             depend_on_external = []
 
@@ -364,14 +365,16 @@
                 self.dataset.loc[indices_end, col] = np.nan
             else:
                 ordered_indices = FeatureChoice.get_ordered_indices(
                     col, self.dataset, ascending
                 )
                 self.dataset.loc[ordered_indices[:num_mv], col] = np.nan
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
 
     def MBOV_randomness(
         self,
         missing_rate: int = 10,
         randomness: float = 0,
         columns: list = None
@@ -386,17 +389,17 @@
             columns (list): A list of strings containing columns names.
 
         Returns:
             dataset (DataFrame): The dataset with missing values generated under
             the MNAR mechanism.
 
         Reference:
-        [2] R. C. Pereira, P. H. Abreu, P. P. Rodrigues, and M. A. T. Figuereido. 2023.
-        Imputation of Data Missing Not At Random:Artificial Generation and Benchmark
-        Analysis. Submitted to Expert Systems with Applications.
+        [2] Pereira, R. C., Abreu, P. H., Rodrigues, P. P., Figueiredo, M. A. T., (2024). 
+        Imputation of data Missing Not at Random: Artificial generation and benchmark analysis. 
+        Expert Systems with Applications, 249(B), 123654.
 
         """
         if not (0 <= randomness <= 0.5):
             raise ValueError('randomness must be in range [0,0.5]')
 
         if columns is None:
             raise TypeError(
@@ -430,14 +433,16 @@
 
             pos_xmis = np.concatenate(
                 [pos_xmis_deterministic, pos_xmiss_randomness]
             )
 
             self.dataset.loc[pos_xmis, col] = np.nan
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
 
     def MBOV_median(self, missing_rate: int = 10, columns: list = None):
         """
         Function to generate missing data based on Missigness Based on Own Values (MBOV) using
         a median to choose miss locations in each feature.
 
@@ -446,17 +451,17 @@
             columns (list): A list of strings containing columns names.
 
         Returns:
             dataset (DataFrame): The dataset with missing values generated under
             the MNAR mechanism.
 
         Reference:
-        [2] R. C. Pereira, P. H. Abreu, P. P. Rodrigues, and M. A. T. Figuereido. 2023.
-        Imputation of Data Missing Not At Random:Artificial Generation and Benchmark
-        Analysis. Submitted to Expert Systems with Applications.
+        [2] Pereira, R. C., Abreu, P. H., Rodrigues, P. P., Figueiredo, M. A. T., (2024). 
+        Imputation of data Missing Not at Random: Artificial generation and benchmark analysis. 
+        Expert Systems with Applications, 249(B), 123654.
 
         """
 
         if missing_rate >= 100:
             raise ValueError(
                 'Missing Rate is too high, the whole feature will be deleted!'
             )
@@ -468,24 +473,26 @@
                 'You must inform columns from dataset to generate missing data'
             )
 
         mr = missing_rate / 100
         N = round(len(self.dataset) * mr)
 
         for col in columns:
-            if col.dtype == 'object':
+            if self.dataset[col].dtype == 'object':
                 raise TypeError(
                     'Only continuos or ordinal feature are accepted'
                 )
 
             median_att = self.dataset[col].median()
 
             pos_xmis = np.argsort(np.abs(self.dataset[col] - median_att))[:N]
             self.dataset.loc[pos_xmis, col] = np.nan
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
 
     def MBIR(
         self,
         missing_rate: int = 10,
         columns: list = None,
         statistical_method: str = 'Mann-Whitney',
@@ -500,17 +507,17 @@
             The options are ["Mann-Whitney", "Bayesian"]. Default is Mann-Whitney
 
         Returns:
             dataset (DataFrame): The dataset with missing values generated under
             the MNAR mechanism.
 
         Reference:
-        [2] R. C. Pereira, P. H. Abreu, P. P. Rodrigues, and M. A. T. Figuereido. 2023.
-        Imputation of Data Missing Not At Random:Artificial Generation and Benchmark
-        Analysis. Submitted to Expert Systems with Applications.
+        [2] Pereira, R. C., Abreu, P. H., Rodrigues, P. P., Figueiredo, M. A. T., (2024). 
+        Imputation of data Missing Not at Random: Artificial generation and benchmark analysis. 
+        Expert Systems with Applications, 249(B), 123654.
 
         """
         if missing_rate >= 100:
             raise ValueError(
                 'Missing Rate is too high, the whole feature will be deleted!'
             )
         elif missing_rate < 0:
@@ -563,8 +570,10 @@
                 most_significant_diff, key=most_significant_diff.get
             )
             pos_xmis = self.dataset[most_feature].sort_values()[:N].index
             self.dataset.loc[pos_xmis, x_miss] = np.nan
             df_columns.remove(most_feature)
             self.dataset = self.dataset.drop(columns=most_feature)
 
+        if not self.missTarget:
+            self.dataset['target'] = self.y
         return self.dataset
```

### Comparing `mdatagen-0.0.87/mdatagen/univariate/uMAR.py` & `mdatagen-0.0.9/mdatagen/univariate/uMAR.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # =============================================================================
 # Aeronautics Institute of Technologies (ITA) - Brazil
 # University of Coimbra (UC) - Portugal
 # Arthur Dantas Mangussi - mangussiarthur@gmail.com
 # =============================================================================
 
 __author__ = 'Arthur Dantas Mangussi'
-__version__ = '0.0.8'
 
 
 import random
 
 import numpy as np
 import pandas as pd
 from mdatagen.utils.feature_choice import FeatureChoice
```

### Comparing `mdatagen-0.0.87/mdatagen/univariate/uMCAR.py` & `mdatagen-0.0.9/mdatagen/univariate/uMCAR.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # =============================================================================
 # Aeronautics Institute of Technologies (ITA) - Brazil
 # University of Coimbra (UC) - Portugal
 # Arthur Dantas Mangussi - mangussiarthur@gmail.com
 # =============================================================================
 
 __author__ = 'Arthur Dantas Mangussi'
-__version__ = '0.0.8'
+
 
 import numpy as np
 import pandas as pd
 from mdatagen.utils.math_calcs import MathCalcs
 
 
 # ==========================================================================
```

### Comparing `mdatagen-0.0.87/mdatagen/univariate/uMNAR.py` & `mdatagen-0.0.9/mdatagen/univariate/uMNAR.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # =============================================================================
 # Aeronautics Institute of Technologies (ITA) - Brazil
 # University of Coimbra (UC) - Portugal
 # Arthur Dantas Mangussi - mangussiarthur@gmail.com
 # =============================================================================
 
 __author__ = 'Arthur Dantas Mangussi'
-__version__ = '0.0.8'
+
 
 import numpy as np
 import pandas as pd
 from mdatagen.utils.feature_choice import FeatureChoice
 
 
 # ==========================================================================
```

### Comparing `mdatagen-0.0.87/mdatagen/utils/feature_choice.py` & `mdatagen-0.0.9/mdatagen/utils/feature_choice.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # =============================================================================
 # Aeronautics Institute of Technologies (ITA) - Brazil
 # University of Coimbra (UC) - Portugal
 # Arthur Dantas Mangussi - mangussiarthur@gmail.com
 # =============================================================================
 
 __author__ = 'Arthur Dantas Mangussi'
-__version__ = '0.0.8'
+
 
 import numpy as np
 import pandas as pd
 from mdatagen.utils.math_calcs import MathCalcs
 
 
 class FeatureChoice:
@@ -23,16 +23,14 @@
             x_miss = MathCalcs._find_correlation(X, y, 'target')
 
         x_obs = None
         if flag:
             x_obs = MathCalcs._find_correlation(X, y, x_miss)
 
             if x_obs == 'target':
-                print('Finding the most correlated feature execpt class')
-
                 x_obs = MathCalcs._find_correlation(X, y, x_miss, flag=True)
 
         return x_miss, x_obs
 
     @staticmethod
     def get_ordered_indices(col, dataset, ascending):
         x_f = dataset.loc[:, col].values
```

### Comparing `mdatagen-0.0.87/mdatagen/utils/math_calcs.py` & `mdatagen-0.0.9/mdatagen/utils/math_calcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # =============================================================================
 # Aeronautics Institute of Technologies (ITA) - Brazil
 # University of Coimbra (UC) - Portugal
 # Arthur Dantas Mangussi - mangussiarthur@gmail.com
 # =============================================================================
 
 __author__ = 'Arthur Dantas Mangussi'
-__version__ = '0.0.8'
+
 
 import numpy as np
 import pandas as pd
 from sklearn.feature_selection import mutual_info_classif
 
 
 class MathCalcs:
@@ -99,15 +99,13 @@
         return matriz_correlacao, matriz_correlacao_X
 
     @staticmethod
     def define_groups(dataset, x_obs):
         g1_index = np.random.choice(
             dataset[x_obs].index, round(len(dataset) / 2), replace=False
         )
-        g2_index = np.random.choice(
-            dataset[x_obs].index, round(len(dataset) / 2), replace=False
-        )
+        g2_index = np.array([i for i in dataset[x_obs].index if i not in g1_index])
 
         g1 = dataset.loc[g1_index, x_obs]
         g2 = dataset.loc[g2_index, x_obs]
 
         return g1, g2
```

### Comparing `mdatagen-0.0.87/mdatagen.egg-info/PKG-INFO` & `mdatagen-0.0.9/mdatagen.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mdatagen
-Version: 0.0.87
+Version: 0.0.9
 Summary: mdatagen: A Python Library for the Generation of Artificial Missing Data
 Home-page: https://github.com/ArthurMangussi/pymdatagen
 Author: Arthur Dantas Mangussi
 Author-email: mangussiarthur@gmail.com
 License: MIT
 Keywords: machine learning,preprocessing data
-Requires-Python: >=3.11
+Requires-Python: >=3.10.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mdatagen: A Python Library for the Generation of Artificial Missing Data
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
 [![Documentation](https://img.shields.io/badge/Documentation-Link-green.svg)](docs/)
@@ -30,29 +30,30 @@
 To install the package, please use the `pip` installation as follows:
 
 ```bash
 pip install mdatagen
 ```
 
 ### Usage examples
-For examples on how to use the mdatagen package, from basic examples that generate artificial missing data under a mechanism to complete examples using Multiple Imputation by Chained Equations (MICE) from scikit-learn for imputation, follow this [examples](examples/).
+For examples on how to use the mdatagen package, from basic examples that generate artificial missing data under a mechanism to complete examples using Multiple Imputation by Chained Equations (MICE) from scikit-learn for imputation, follow these [examples](examples/).
 
 
 ## Contribuitions
 Contributions are welcome! Feel free to open issues, submit pull requests, or provide feedback.
 
 ## Citation
-If you use **mdatagen** in your research, please cite the [mdatagen paper]()
+If you use **mdatagen** in your research, please cite the [original paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8605316)
 
 Bibtex entry:
 ```bash
-@article{mdatagen2024,
-  author  = {Arthur D Mangussi and Filipe Loyola Lopes and Miriam Seone Santos and Ricardo Cardoso Pereira and Ana Carolina Lorena and Pedro Henriques Abreu},
-  title   = {mdatagen: A Python Library for the Generation of Artificial Missing Data},
-  journal = {Journal of Machine Learning Research},
-  year    = {2024},
-  volume  = {24},
-  pages   = {1--6},
-}
+@ARTICLE{Santos2019,
+  author={Santos, Miriam Seoane and Pereira, Ricardo Cardoso and Costa, Adriana Fonseca and Soares, Jastin Pompeu and Santos, João and Abreu, Pedro Henriques},
+  journal={IEEE Access}, 
+  title={Generating Synthetic Missing Data: A Review by Missing Mechanism}, 
+  year={2019},
+  volume={7},
+  number={},
+  pages={11651-11667},
+  doi={10.1109/ACCESS.2019.2891360}}
 ```
 ## Acknowledgements
 The authors gratefully acknowledge the Brazilian funding agencies FAPESP (Fundação Amparo à Pesquisa do Estado de São Paulo) under grants 2022/10553-6, and 2021/06870-3. Moreover, this research was supported in part by the Coordenação de Aperfeiçoamento de Pessoalde Nível Superior - Brasil (CAPES) - Finance Code 001, and Portuguese Recovery and Resilience Plan (PRR) through project C645008882-00000055 Center for Responsable AI.
```

### Comparing `mdatagen-0.0.87/mdatagen.egg-info/SOURCES.txt` & `mdatagen-0.0.9/mdatagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdatagen-0.0.87/setup.py` & `mdatagen-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='mdatagen',
-    version='0.0.87',
+    version='0.0.9',
     keywords=['machine learning', 'preprocessing data'],
     license='MIT',
     author='Arthur Dantas Mangussi',
     author_email='mangussiarthur@gmail.com',
     url='https://github.com/ArthurMangussi/pymdatagen',
     
     packages=find_packages(),
     description='mdatagen: A Python Library for the Generation of Artificial Missing Data',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
-    python_requires='>=3.11', 
+    python_requires='>=3.10.12', 
     install_requires=[
         'numpy >= 1.25.0',
         'pandas >= 2.0.3',
         'scikit-learn == 1.3.0']
 )
```

