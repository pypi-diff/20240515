# Comparing `tmp/mineralML-0.0.0.5.tar.gz` & `tmp/mineralML-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mineralML-0.0.0.5.tar", last modified: Thu Jan 25 17:17:07 2024, max compression
+gzip compressed data, was "mineralML-0.0.0.6.tar", last modified: Wed May 15 21:54:14 2024, max compression
```

## Comparing `mineralML-0.0.0.5.tar` & `mineralML-0.0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:17:07.481983 mineralML-0.0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-25 17:16:56.000000 mineralML-0.0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-01-25 17:17:07.481983 mineralML-0.0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-01-25 17:16:56.000000 mineralML-0.0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-25 17:17:07.481983 mineralML-0.0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:17:07.477983 mineralML-0.0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:17:07.481983 mineralML-0.0.0.5/src/mineralML/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)   537737 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/ae_best_model.pt
--rw-r--r--   0 runner    (1001) docker     (127)   648436 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/ae_tanh.npz
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/mineral_classes_ae.npz
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/mineral_classes_nn.npz
--rw-r--r--   0 runner    (1001) docker     (127)    24738 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/nn_best_model.pt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/scaler_ae.npz
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/scaler_nn.npz
--rw-r--r--   0 runner    (1001) docker     (127)   243771 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/stoichiometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    33473 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)    28645 2024-01-25 17:16:57.000000 mineralML-0.0.0.5/src/mineralML/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:17:07.481983 mineralML-0.0.0.5/src/mineralML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-01-25 17:17:07.000000 mineralML-0.0.0.5/src/mineralML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-25 17:17:07.000000 mineralML-0.0.0.5/src/mineralML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 17:17:07.000000 mineralML-0.0.0.5/src/mineralML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-25 17:17:07.000000 mineralML-0.0.0.5/src/mineralML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-25 17:17:07.000000 mineralML-0.0.0.5/src/mineralML.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:54:14.879085 mineralML-0.0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    34903 2024-05-15 21:54:05.000000 mineralML-0.0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-15 21:54:14.879085 mineralML-0.0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-15 21:54:05.000000 mineralML-0.0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 21:54:14.879085 mineralML-0.0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:54:14.875085 mineralML-0.0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:54:14.879085 mineralML-0.0.0.6/src/mineralML/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   537737 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/ae_best_model.pt
+-rw-r--r--   0 runner    (1001) docker     (127)   648436 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/ae_tanh.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/mineral_classes_ae.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/mineral_classes_nn.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    24738 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/nn_best_model.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/scaler_ae.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/scaler_nn.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   258718 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/stoichiometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34287 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30642 2024-05-15 21:54:06.000000 mineralML-0.0.0.6/src/mineralML/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:54:14.879085 mineralML-0.0.0.6/src/mineralML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-15 21:54:14.000000 mineralML-0.0.0.6/src/mineralML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-15 21:54:14.000000 mineralML-0.0.0.6/src/mineralML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:54:14.000000 mineralML-0.0.0.6/src/mineralML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 21:54:14.000000 mineralML-0.0.0.6/src/mineralML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 21:54:14.000000 mineralML-0.0.0.6/src/mineralML.egg-info/top_level.txt
```

### Comparing `mineralML-0.0.0.5/PKG-INFO` & `mineralML-0.0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mineralML
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: mineralML
 Home-page: https://github.com/sarahshi/mineralML
 Author: Sarah C. Shi
 Author-email: sarah.c.shi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,20 +16,20 @@
 # mineralML
 [![PyPI](https://badgen.net/pypi/v/mineralML)](https://pypi.org/project/mineralML/)
 [![Build Status](https://github.com/SarahShi/mineralML/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/mineralML/actions/workflows/main.yml)
 [![Documentation Status](https://readthedocs.org/projects/mineralml/badge/?version=latest)](https://mineralml.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/SarahShi/mineralML/branch/main/graph/badge.svg)](https://codecov.io/gh/SarahShi/mineralML/branch/main)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SarahShi/mineralML/blob/main/mineralML_colab.ipynb)
 [![Python 3.7](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 We present mineralML (mineral classification using Machine Learning) for classifying common igneous minerals based on oxide data collected by EPMA, with functions for calculating stoichiometries and crystallographic sites based on this classification. Utilizing this package allows for the identification of misclassified mineral phases and poor-quality data. We streamline data processing and cleaning to allow for the rapid transition to usable data, improving the utility of data curated in these databases and furthering computing and modeling capabilities. 
 
 ## Documentation
-Read the [documentation](https:/mineralML.readthedocs.io/en/latest/) for a run-through of the mineralML code. 
+Read the [documentation](https://mineralml.readthedocs.io/en/latest/?badge=latest) for a run-through of the mineralML code. 
 
 ## Run on the Cloud 
 If you do not have Python installed locally, run mineralML on [Google Colab](https://colab.research.google.com/github/SarahShi/mineralML/blob/main/mineralML_colab.ipynb). The Cloud-based version runs rapidly, with test cases of >10,000 microanalyses classified within 4 seconds. 
 
 ## Run and Install Locally
 Obtain a version of Python between 3.7 and 3.11 if you do not already have it installed. mineralML can be installed with one line. Open terminal and type the following:
```

### Comparing `mineralML-0.0.0.5/README.md` & `mineralML-0.0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # mineralML
 [![PyPI](https://badgen.net/pypi/v/mineralML)](https://pypi.org/project/mineralML/)
 [![Build Status](https://github.com/SarahShi/mineralML/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/mineralML/actions/workflows/main.yml)
 [![Documentation Status](https://readthedocs.org/projects/mineralml/badge/?version=latest)](https://mineralml.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/SarahShi/mineralML/branch/main/graph/badge.svg)](https://codecov.io/gh/SarahShi/mineralML/branch/main)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SarahShi/mineralML/blob/main/mineralML_colab.ipynb)
 [![Python 3.7](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 We present mineralML (mineral classification using Machine Learning) for classifying common igneous minerals based on oxide data collected by EPMA, with functions for calculating stoichiometries and crystallographic sites based on this classification. Utilizing this package allows for the identification of misclassified mineral phases and poor-quality data. We streamline data processing and cleaning to allow for the rapid transition to usable data, improving the utility of data curated in these databases and furthering computing and modeling capabilities. 
 
 ## Documentation
-Read the [documentation](https:/mineralML.readthedocs.io/en/latest/) for a run-through of the mineralML code. 
+Read the [documentation](https://mineralml.readthedocs.io/en/latest/?badge=latest) for a run-through of the mineralML code. 
 
 ## Run on the Cloud 
 If you do not have Python installed locally, run mineralML on [Google Colab](https://colab.research.google.com/github/SarahShi/mineralML/blob/main/mineralML_colab.ipynb). The Cloud-based version runs rapidly, with test cases of >10,000 microanalyses classified within 4 seconds. 
 
 ## Run and Install Locally
 Obtain a version of Python between 3.7 and 3.11 if you do not already have it installed. mineralML can be installed with one line. Open terminal and type the following:
```

### Comparing `mineralML-0.0.0.5/setup.py` & `mineralML-0.0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `mineralML-0.0.0.5/src/mineralML/ae_best_model.pt` & `mineralML-0.0.0.6/src/mineralML/ae_best_model.pt`

 * *Files identical despite different names*

### Comparing `mineralML-0.0.0.5/src/mineralML/ae_tanh.npz` & `mineralML-0.0.0.6/src/mineralML/ae_tanh.npz`

 * *Files identical despite different names*

### Comparing `mineralML-0.0.0.5/src/mineralML/confusion_matrix.py` & `mineralML-0.0.0.6/src/mineralML/confusion_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,32 @@
-# %% 
+# %%
 
 import numpy as np
 import pandas as pd
 import warnings
 import seaborn as sns
 
 import matplotlib
 from matplotlib import pyplot as plt
 
-# %% 
+# %%
 
-def pp_matrix(df_cm, annot=True, cmap="BuGn", fmt=".2f",
-    fz=12, lw=0.5, cbar=False, figsize=[10.5, 10.5],
-    show_null_values=0, pred_val_axis="x"):  #, savefig = None,):
 
+def pp_matrix(
+    df_cm,
+    annot=True,
+    cmap="BuGn",
+    fmt=".2f",
+    fz=12,
+    lw=0.5,
+    cbar=False,
+    figsize=[10.5, 10.5],
+    show_null_values=0,
+    pred_val_axis="x",
+):  # , savefig = None,):
     """
 
     Creates and displays a confusion matrix visualization using Seaborn's heatmap function.
 
     Parameters:
         df_cm (pd.DataFrame): DataFrame containing the confusion matrix without totals.
         annot (bool, optional): If True, display the text in each cell. Default is True.
@@ -55,19 +64,29 @@
     insert_totals(df_cm)
     df_cm = df_cm.astype(int)
 
     fig1 = plt.figure("Conf matrix default", figsize)
     ax1 = fig1.gca()  # Get Current Axis
     ax1.cla()  # clear existing plot
 
-    ax = sns.heatmap(df_cm, annot=annot, annot_kws={"size": fz}, linewidths=lw, ax=ax1, cbar=cbar, cmap=cmap, linecolor="w", fmt=fmt,)
+    ax = sns.heatmap(
+        df_cm,
+        annot=annot,
+        annot_kws={"size": fz},
+        linewidths=lw,
+        ax=ax1,
+        cbar=cbar,
+        cmap=cmap,
+        linecolor="w",
+        fmt=fmt,
+    )
 
     # set ticklabels rotation
-    ax.set_xticklabels(ax.get_xticklabels(), rotation=45, fontsize=13, ha='right')
-    ax.set_yticklabels(ax.get_yticklabels(), rotation=35, fontsize=13, va='top')
+    ax.set_xticklabels(ax.get_xticklabels(), rotation=45, fontsize=13, ha="right")
+    ax.set_yticklabels(ax.get_yticklabels(), rotation=35, fontsize=13, va="top")
 
     # Turn off all the ticks
     for t in ax.xaxis.get_major_ticks():
         t.tick1On = False
         t.tick2On = False
     for t in ax.yaxis.get_major_ticks():
         t.tick1On = False
@@ -85,15 +104,17 @@
     for t in ax.collections[0].axes.texts:  # ax.texts:
         pos = np.array(t.get_position()) - [0.5, 0.5]
         lin = int(pos[1])
         col = int(pos[0])
         posi += 1
 
         # set text
-        txt_res = config_cell_text_and_colors(array_df, lin, col, t, facecolors, posi, fz, fmt, show_null_values)
+        txt_res = config_cell_text_and_colors(
+            array_df, lin, col, t, facecolors, posi, fz, fmt, show_null_values
+        )
 
         text_add.extend(txt_res[0])
         text_del.extend(txt_res[1])
 
     # remove the old ones
     for item in text_del:
         item.remove()
@@ -102,59 +123,61 @@
         ax.text(item["x"], item["y"], item["text"], **item["kw"])
 
     # titles and legends
     ax.set_xlabel(xlbl)
     ax.set_ylabel(ylbl)
     plt.tight_layout()  # set layout slim
 
-    # if savefig != None: 
+    # if savefig != None:
     #     plt.savefig(savefig + '.pdf')
 
 
 def insert_totals(df_cm):
-
     """
 
     Inserts total sums for each row and column into the confusion matrix DataFrame.
 
     This function adds a 'sum_row' column and a 'sum_col' row to the DataFrame, representing
     the total counts across each row and column, respectively. It also sets the bottom-right
     cell to the grand total.
 
     Parameters:
         df_cm (pd.DataFrame): DataFrame representing the confusion matrix.
 
     Returns:
         None: The function modifies the DataFrame in place.
-    
+
     Note:
         If 'sum_row' or 'sum_col' already exist in the DataFrame, they will be recalculated.
 
     """
 
     # Check if 'sum_row' and 'sum_col' already exist and remove them if they do
-    if 'sum_row' in df_cm.columns:
-        df_cm.drop('sum_row', axis=1, inplace=True)
-    if 'sum_col' in df_cm.index:
-        df_cm.drop('sum_col', axis=0, inplace=True)
-    
+    if "sum_row" in df_cm.columns:
+        df_cm.drop("sum_row", axis=1, inplace=True)
+    if "sum_col" in df_cm.index:
+        df_cm.drop("sum_col", axis=0, inplace=True)
+
     # Calculate the sum of each column to create 'sum_row'
     sum_col = df_cm.sum(axis=0).astype(int)  # sum columns
     sum_lin = df_cm.sum(axis=1).astype(int)  # sum rows
-    
-    # Add 'sum_row' and 'sum_col' to the dataframe
-    df_cm['sum_row'] = sum_lin
-    df_cm.loc['sum_col'] = sum_col
-    df_cm.at['sum_col', 'sum_row'] = sum_lin.sum()  # Set the bottom right cell to the grand total
 
+    # Add 'sum_row' and 'sum_col' to the dataframe
+    df_cm["sum_row"] = sum_lin
+    df_cm.loc["sum_col"] = sum_col
+    df_cm.at[
+        "sum_col", "sum_row"
+    ] = sum_lin.sum()  # Set the bottom right cell to the grand total
 
-def config_cell_text_and_colors(array_df, lin, col, oText, facecolors, posi, fz, fmt, show_null_values=0):
 
+def config_cell_text_and_colors(
+    array_df, lin, col, oText, facecolors, posi, fz, fmt, show_null_values=0
+):
     """
-    
+
     Configures cell text and colors for confusion matrix visualization.
 
     Adjusts the text and background colors of cells in the confusion matrix based on their values.
     Totals and percentages are calculated for the last row and column cells.
 
     Parameters:
         array_df (np.ndarray): 2D numpy array of the confusion matrix.
@@ -169,15 +192,15 @@
 
     Returns:
         tuple: A tuple containing two lists: text elements to add and to delete.
 
     Note:
         The function modifies text and background colors based on the value in each cell.
 
-            """
+    """
 
     import matplotlib.font_manager as fm
 
     text_add = []
     text_del = []
     cell_val = array_df[lin][col]
     tot_all = array_df[-1][-1]
@@ -204,31 +227,46 @@
         else:
             per_ok = per_err = 0
 
         per_ok_s = ["%.1f%%" % (per_ok), "100%"][per_ok == 100]
 
         # text to DEL
         text_del.append(oText)
-        
-        warnings.filterwarnings("ignore", category=DeprecationWarning) 
+
+        warnings.filterwarnings("ignore", category=DeprecationWarning)
 
         # text to ADD
         font_prop = fm.FontProperties(weight="bold", size=fz)
-        text_kwargs = dict(color="k", ha="center",va="center", gid="sum", fontproperties=font_prop,)
+        text_kwargs = dict(
+            color="k",
+            ha="center",
+            va="center",
+            gid="sum",
+            fontproperties=font_prop,
+        )
         lis_txt = ["%d" % (cell_val), per_ok_s, "%.1f%%" % (per_err)]
         lis_kwa = [text_kwargs]
         dic = text_kwargs.copy()
         dic["color"] = "g"
         lis_kwa.append(dic)
         dic = text_kwargs.copy()
         dic["color"] = "r"
         lis_kwa.append(dic)
-        lis_pos = [(oText._x, oText._y - 0.3), (oText._x, oText._y), (oText._x, oText._y + 0.3),]
+        lis_pos = [
+            (oText._x, oText._y - 0.3),
+            (oText._x, oText._y),
+            (oText._x, oText._y + 0.3),
+        ]
         for i in range(len(lis_txt)):
-            newText = dict(x=lis_pos[i][0], y=lis_pos[i][1], text=lis_txt[i], kw=lis_kwa[i],)
+            newText = dict(
+                x=lis_pos[i][0],
+                y=lis_pos[i][1],
+                text=lis_txt[i],
+                kw=lis_kwa[i],
+            )
             text_add.append(newText)
 
         # set background color for sum cells (last line and last column)
         carr = [0.27, 0.30, 0.27, 1.0]
         if (col == ccl - 1) and (lin == ccl - 1):
             carr = [0.17, 0.20, 0.17, 1.0]
         facecolors[posi] = carr
@@ -251,8 +289,7 @@
             oText.set_color("k")
             # set background color in the diagonal to blue
             facecolors[posi] = [0.35, 0.8, 0.55, 1.0]
         else:
             oText.set_color("r")
 
     return text_add, text_del
-
```

### Comparing `mineralML-0.0.0.5/src/mineralML/core.py` & `mineralML-0.0.0.6/src/mineralML/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,44 +135,44 @@
         raise FileNotFoundError(f"The scaler file was not found at {scaler_path}.")
     except Exception as e:
         raise e  # Propagate other exceptions up
 
     return mean, std
 
 
-def create_dataloader(df, batch_size=128, shuffle=False):
+# def create_dataloader(df, batch_size=128, shuffle=False):
 
-    """
+#     """
 
-    Creates a DataLoader for the given DataFrame. It normalizes the input features and converts 
-    the 'Mineral' column to categorical codes based on predefined mineral classes. The resulting 
-    DataLoader can be used to iterate over the dataset in batches during model training or evaluation.
-    The function relies on the 'load_minclass_nn' function to obtain the list of category names 
-    for the 'Mineral' column and the 'norm_data' function to normalize the feature columns 
-    before creating the DataLoader.
-
-    Parameters:
-        df (DataFrame): The DataFrame containing features and mineral labels to load into the DataLoader.
-        batch_size (int): The number of samples to load per batch. Defaults to 128.
-        shuffle (bool): Whether to shuffle the data before loading it. Defaults to False.
+#     Creates a DataLoader for the given DataFrame. It normalizes the input features and converts 
+#     the 'Mineral' column to categorical codes based on predefined mineral classes. The resulting 
+#     DataLoader can be used to iterate over the dataset in batches during model training or evaluation.
+#     The function relies on the 'load_minclass_nn' function to obtain the list of category names 
+#     for the 'Mineral' column and the 'norm_data' function to normalize the feature columns 
+#     before creating the DataLoader.
+
+#     Parameters:
+#         df (DataFrame): The DataFrame containing features and mineral labels to load into the DataLoader.
+#         batch_size (int): The number of samples to load per batch. Defaults to 128.
+#         shuffle (bool): Whether to shuffle the data before loading it. Defaults to False.
 
-    Returns:
-        dataloader (DataLoader): A PyTorch DataLoader object ready for model consumption.
+#     Returns:
+#         dataloader (DataLoader): A PyTorch DataLoader object ready for model consumption.
     
-    """
+#     """
 
-    min_cat, _ = load_minclass_nn()
-    data_x = norm_data(df)
-    df['Mineral'] = pd.Categorical(df['Mineral'], categories=min_cat)
-    data_y = df['Mineral'].cat.codes.values
+#     min_cat, _ = load_minclass_nn()
+#     data_x = norm_data_nn(df)
+#     df['Mineral'] = pd.Categorical(df['Mineral'], categories=min_cat)
+#     data_y = df['Mineral'].cat.codes.values
 
-    label_dataset = LabelDataset(data_x, data_y)
-    dataloader = DataLoader(label_dataset, batch_size, shuffle)
+#     label_dataset = LabelDataset(data_x, data_y)
+#     dataloader = DataLoader(label_dataset, batch_size, shuffle)
 
-    return dataloader
+#     return dataloader
 
 
 def weights_init(m):
 
     """
 
     Applies an initialization scheme to the weights and biases of a Batch Normalization layer
```

### Comparing `mineralML-0.0.0.5/src/mineralML/mineral_classes_ae.npz` & `mineralML-0.0.0.6/src/mineralML/mineral_classes_ae.npz`

 * *Files identical despite different names*

### Comparing `mineralML-0.0.0.5/src/mineralML/mineral_classes_nn.npz` & `mineralML-0.0.0.6/src/mineralML/mineral_classes_nn.npz`

 * *Files identical despite different names*

### Comparing `mineralML-0.0.0.5/src/mineralML/nn_best_model.pt` & `mineralML-0.0.0.6/src/mineralML/nn_best_model.pt`

 * *Files identical despite different names*

### Comparing `mineralML-0.0.0.5/src/mineralML/scaler_ae.npz` & `mineralML-0.0.0.6/src/mineralML/scaler_ae.npz`

 * *Files identical despite different names*

### Comparing `mineralML-0.0.0.5/src/mineralML/scaler_nn.npz` & `mineralML-0.0.0.6/src/mineralML/scaler_nn.npz`

 * *Files identical despite different names*

### Comparing `mineralML-0.0.0.5/src/mineralML/stoichiometry.py` & `mineralML-0.0.0.6/src/mineralML/stoichiometry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # %%
 
 import numpy as np
 import pandas as pd
 import scipy
 
-# %% 
+# %%
 
 
 def import_excel(filename, sheet_name, sample_label=None, GEOROC=False, suffix=None):
-
     """
 
-    Import excel sheet of oxides in wt%, headings should be of the form SiO2_Liq (for the melt/liquid), 
-    SiO2_Ol (for olivine comps), SiO2_Cpx (for clinopyroxene compositions). Order does not matter. 
-    
-    Parameters: 
+    Import excel sheet of oxides in wt%, headings should be of the form SiO2_Liq (for the melt/liquid),
+    SiO2_Ol (for olivine comps), SiO2_Cpx (for clinopyroxene compositions). Order does not matter.
+
+    Parameters:
         filename: .xlsx, .csv, .xls file
-            Compositional data as an Excel spreadsheet (.xlsx, .xls) or a comma separated values (.csv) file 
+            Compositional data as an Excel spreadsheet (.xlsx, .xls) or a comma separated values (.csv) file
             with columns labelled SiO2_Liq, SiO2_Ol, SiO2_Cpx etc, and each row corresponding to an analysis.
         filename: str
             specifies the file name (e.g., Python_OlLiq_Thermometers_Test.xlsx)
-    Returns: 
-        
+    Returns:
+
         pandas DataFrames stored in a dictionary. E.g., Access Cpxs using output.Cpxs
             my_input = pandas dataframe of the entire spreadsheet
             mylabels = sample labels
             Experimental_press_temp = User-entered PT
             Liqs=pandas dataframe of liquid oxides
             Ols=pandas dataframe of olivine oxides
             Cpxs=pandas dataframe of cpx oxides
@@ -33,459 +32,572 @@
             Kspars=pandas dataframe of kspar oxides
             Opxs=pandas dataframe of opx oxides
             Amps=pandas dataframe of amphibole oxides
             Sps=pandas dataframe of spinel oxides
 
     """
 
-    if 'csv' in filename:
+    if "csv" in filename:
         my_input = pd.read_csv(filename)
 
-    elif 'xls' in filename:
+    elif "xls" in filename:
         if sheet_name is not None:
             my_input = pd.read_excel(filename, sheet_name=sheet_name)
-            #my_input[my_input < 0] = 0
+            # my_input[my_input < 0] = 0
         else:
             my_input = pd.read_excel(filename)
-            #my_input[my_input < 0] = 0
+            # my_input[my_input < 0] = 0
 
     if suffix is not None:
         if any(my_input.columns.str.contains(suffix)):
-            w.warn('We notice you have specified a suffix, but some of your columns already have this suffix. '
-        'e.g., If you already have _Liq in the file, you shouldnt specify suffix="_Liq" during the import')
-
+            w.warn(
+                "We notice you have specified a suffix, but some of your columns already have this suffix. "
+                'e.g., If you already have _Liq in the file, you shouldnt specify suffix="_Liq" during the import'
+            )
 
     my_input_c = my_input.copy()
     if suffix is not None:
-        my_input_c=my_input_c.add_suffix(suffix)
+        my_input_c = my_input_c.add_suffix(suffix)
 
     if any(my_input.columns.str.contains("_cpx")):
-        w.warn("You've got a column heading with a lower case _cpx, this is okay if this column is for your"
-        " own use, but if its an input to Thermobar, it needs to be capitalized (_Cpx)" )
+        w.warn(
+            "You've got a column heading with a lower case _cpx, this is okay if this column is for your"
+            " own use, but if its an input to Thermobar, it needs to be capitalized (_Cpx)"
+        )
 
     if any(my_input.columns.str.contains("_opx")):
-        w.warn("You've got a column heading with a lower case _opx, this is okay if this column is for your"
-        " own use, but if its an input to Thermobar, it needs to be capitalized (_Opx)" )
+        w.warn(
+            "You've got a column heading with a lower case _opx, this is okay if this column is for your"
+            " own use, but if its an input to Thermobar, it needs to be capitalized (_Opx)"
+        )
 
     if any(my_input.columns.str.contains("_plag")):
-        w.warn("You've got a column heading with a lower case _plag, this is okay if this column is for your"
-        " own use, but if its an input to Thermobar, it needs to be capitalized (_Plag)" )
+        w.warn(
+            "You've got a column heading with a lower case _plag, this is okay if this column is for your"
+            " own use, but if its an input to Thermobar, it needs to be capitalized (_Plag)"
+        )
 
     if any(my_input.columns.str.contains("_kspar")):
-       w.warn("You've got a column heading with a lower case _kspar, this is okay if this column is for your"
-        " own use, but if its an input to Thermobar, it needs to be capitalized (_Kspar)" )
+        w.warn(
+            "You've got a column heading with a lower case _kspar, this is okay if this column is for your"
+            " own use, but if its an input to Thermobar, it needs to be capitalized (_Kspar)"
+        )
 
     if any(my_input.columns.str.contains("_sp")):
-        w.warn("You've got a column heading with a lower case _sp, this is okay if this column is for your"
-        " own use, but if its an input to Thermobar, it needs to be capitalized (_Sp)" )
+        w.warn(
+            "You've got a column heading with a lower case _sp, this is okay if this column is for your"
+            " own use, but if its an input to Thermobar, it needs to be capitalized (_Sp)"
+        )
 
     if any(my_input.columns.str.contains("_ol")):
-        w.warn("You've got a column heading with a lower case _ol, this is okay if this column is for your"
-        " own use, but if its an input to Thermobar, it needs to be capitalized (_Ol)" )
+        w.warn(
+            "You've got a column heading with a lower case _ol, this is okay if this column is for your"
+            " own use, but if its an input to Thermobar, it needs to be capitalized (_Ol)"
+        )
 
     if any(my_input.columns.str.contains("_amp")):
-        w.warn("You've got a column heading with a lower case _amp, this is okay if this campumn is for your"
-        " own use, but if its an input to Thermobar, it needs to be capitalized (_Amp)" )
+        w.warn(
+            "You've got a column heading with a lower case _amp, this is okay if this campumn is for your"
+            " own use, but if its an input to Thermobar, it needs to be capitalized (_Amp)"
+        )
 
     if any(my_input.columns.str.contains("_liq")):
-        w.warn("You've got a column heading with a lower case _liq, this is okay if this column is for your"
-        " own use, but if its an input to Thermobar, it needs to be capitalized (_Liq)" )
+        w.warn(
+            "You've got a column heading with a lower case _liq, this is okay if this column is for your"
+            " own use, but if its an input to Thermobar, it needs to be capitalized (_Liq)"
+        )
 
     if suffix is not None:
-        if any(my_input.columns.str.contains("FeO")) and (all(my_input.columns.str.contains("FeOt")==False)):
-            raise ValueError("No FeOt found. You've got a column heading with FeO. To avoid errors based on common EPMA outputs"
-            " thermobar only recognises columns with FeOt for all phases except liquid"
-            " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests")
-
-    if any(my_input.columns.str.contains("FeO_")) and (all(my_input.columns.str.contains("FeOt_")==False)):
-
-        if any(my_input.columns.str.contains("FeO_Liq")) and any(my_input.columns.str.contains("Fe2O3_Liq")):
-            my_input_c['FeOt_Liq']=my_input_c['FeO_Liq']+my_input_c['Fe2O3_Liq']*0.89998
-
+        if any(my_input.columns.str.contains("FeO")) and (
+            all(my_input.columns.str.contains("FeOt") == False)
+        ):
+            raise ValueError(
+                "No FeOt found. You've got a column heading with FeO. To avoid errors based on common EPMA outputs"
+                " thermobar only recognises columns with FeOt for all phases except liquid"
+                " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests"
+            )
+
+    if any(my_input.columns.str.contains("FeO_")) and (
+        all(my_input.columns.str.contains("FeOt_") == False)
+    ):
+        if any(my_input.columns.str.contains("FeO_Liq")) and any(
+            my_input.columns.str.contains("Fe2O3_Liq")
+        ):
+            my_input_c["FeOt_Liq"] = (
+                my_input_c["FeO_Liq"] + my_input_c["Fe2O3_Liq"] * 0.89998
+            )
 
         else:
-            raise ValueError("No FeOt found. You've got a column heading with FeO. To avoid errors based on common EPMA outputs"
-        " thermobar only recognises columns with FeOt for all phases except liquid"
-        " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests")
+            raise ValueError(
+                "No FeOt found. You've got a column heading with FeO. To avoid errors based on common EPMA outputs"
+                " thermobar only recognises columns with FeOt for all phases except liquid"
+                " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests"
+            )
 
     # if any(my_input.columns.str.contains("Fe2O3_")) and (all(my_input.columns.str.contains("FeOt_")==False)):
     #     raise ValueError("No FeOt column found. You've got a column heading with Fe2O3. To avoid errors based on common EPMA outputs"
     #     " thermobar only recognises columns with FeOt for all phases except liquid"
     #     " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests")
 
-    if any(my_input.columns.str.contains("FeOT_")) and (all(my_input.columns.str.contains("FeOt_")==False)):
-        raise ValueError("No FeOt column found. You've got a column heading with FeOT. Change to a lower case t")
+    if any(my_input.columns.str.contains("FeOT_")) and (
+        all(my_input.columns.str.contains("FeOt_") == False)
+    ):
+        raise ValueError(
+            "No FeOt column found. You've got a column heading with FeOT. Change to a lower case t"
+        )
 
     #   myLabels=my_input.Sample_ID
 
     # Experimental_press_temp1 = my_input.reindex(df_ideal_exp.columns, axis=1)
     # This deals with the fact almost everyone will enter as FeO, but the code uses FeOt for these minerals.
     # E.g., if users only enter FeO (not FeOt and Fe2O3), allocates a FeOt
     # column. If enter FeO and Fe2O3, put a FeOt column
 
     if GEOROC is True:
-        my_input_c.loc[np.isnan(my_input_c['FeOt_Liq']) is True, 'FeOt_Liq'] = my_input_c.loc[np.isnan(
-            my_input_c['FeOt_Liq']) is True, 'FeO_Liq'] + my_input_c.loc[np.isnan(my_input_c['FeOt_Liq']) is True, 'Fe2O3_Liq'] * 0.8999998
+        my_input_c.loc[np.isnan(my_input_c["FeOt_Liq"]) is True, "FeOt_Liq"] = (
+            my_input_c.loc[np.isnan(my_input_c["FeOt_Liq"]) is True, "FeO_Liq"]
+            + my_input_c.loc[np.isnan(my_input_c["FeOt_Liq"]) is True, "Fe2O3_Liq"]
+            * 0.8999998
+        )
 
     myOxides1 = my_input_c.reindex(df_ideal_oxide.columns, axis=1).fillna(0)
-    myOxides1 = myOxides1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myOxides1 = myOxides1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myOxides1[myOxides1 < 0] = 0
 
     myLiquids1 = my_input_c.reindex(df_ideal_liq.columns, axis=1).fillna(0)
-    myLiquids1 = myLiquids1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myLiquids1 = myLiquids1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myLiquids1[myLiquids1 < 0] = 0
 
     myCPXs1 = my_input_c.reindex(df_ideal_cpx.columns, axis=1).fillna(0)
-    myCPXs1 = myCPXs1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myCPXs1 = myCPXs1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myCPXs1[myCPXs1 < 0] = 0
 
     myOls1 = my_input_c.reindex(df_ideal_ol.columns, axis=1).fillna(0)
-    myOls1 = myOls1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myOls1 = myOls1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myOls1[myOls1 < 0] = 0
 
     myPlags1 = my_input_c.reindex(df_ideal_plag.columns, axis=1).fillna(0)
-    myPlags1 = myPlags1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myPlags1 = myPlags1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myPlags1[myPlags1 < 0] = 0
 
     myKspars1 = my_input_c.reindex(df_ideal_kspar.columns, axis=1).fillna(0)
-    myKspars1 = myKspars1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myKspars1 = myKspars1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myKspars1[myKspars1 < 0] = 0
 
     myOPXs1 = my_input_c.reindex(df_ideal_opx.columns, axis=1).fillna(0)
-    myOPXs1 = myOPXs1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myOPXs1 = myOPXs1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myOPXs1[myOPXs1 < 0] = 0
 
     mySps1 = my_input_c.reindex(df_ideal_sp.columns, axis=1).fillna(0)
-    mySps1 = mySps1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    mySps1 = mySps1.apply(pd.to_numeric, errors="coerce").fillna(0)
     mySps1[mySps1 < 0] = 0
 
     myAmphs1 = my_input_c.reindex(df_ideal_amp.columns, axis=1).fillna(0)
-    myAmphs1 = myAmphs1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myAmphs1 = myAmphs1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myAmphs1[myAmphs1 < 0] = 0
 
     myGts1 = my_input_c.reindex(df_ideal_gt.columns, axis=1).fillna(0)
-    myGts1 = myGts1.apply(pd.to_numeric, errors='coerce').fillna(0)
+    myGts1 = myGts1.apply(pd.to_numeric, errors="coerce").fillna(0)
     myGts1[myGts1 < 0] = 0
 
     # Adding sample Names
     if "Sample_ID_Cpx" in my_input_c:
-        myCPXs1['Sample_ID_Cpx'] = my_input_c['Sample_ID_Cpx']
+        myCPXs1["Sample_ID_Cpx"] = my_input_c["Sample_ID_Cpx"]
     else:
-        myCPXs1['Sample_ID_Cpx'] = my_input.index
+        myCPXs1["Sample_ID_Cpx"] = my_input.index
 
     if "Sample_ID_Opx" in my_input_c:
-        myOPXs1['Sample_ID_Opx'] = my_input_c['Sample_ID_Opx']
+        myOPXs1["Sample_ID_Opx"] = my_input_c["Sample_ID_Opx"]
     else:
-        myOPXs1['Sample_ID_Opx'] = my_input.index
+        myOPXs1["Sample_ID_Opx"] = my_input.index
 
     if "Sample_ID_Liq" in my_input_c:
-        myLiquids1['Sample_ID_Liq'] = my_input_c['Sample_ID_Liq']
+        myLiquids1["Sample_ID_Liq"] = my_input_c["Sample_ID_Liq"]
     else:
-        myLiquids1['Sample_ID_Liq'] = my_input.index
+        myLiquids1["Sample_ID_Liq"] = my_input.index
 
     if "Sample_ID_Plag" in my_input_c:
-        myPlags1['Sample_ID_Plag'] = my_input_c['Sample_ID_Plag']
+        myPlags1["Sample_ID_Plag"] = my_input_c["Sample_ID_Plag"]
     else:
-        myPlags1['Sample_ID_Plag'] = my_input.index
+        myPlags1["Sample_ID_Plag"] = my_input.index
 
     if "Sample_ID_Amp" in my_input_c:
-        myAmphs1['Sample_ID_Amp'] = my_input_c['Sample_ID_Amp']
+        myAmphs1["Sample_ID_Amp"] = my_input_c["Sample_ID_Amp"]
     else:
-        myAmphs1['Sample_ID_Amp'] = my_input.index
+        myAmphs1["Sample_ID_Amp"] = my_input.index
 
     if "Sample_ID_Gt" in my_input_c:
-        myGts1['Sample_ID_Gt'] = my_input_c['Sample_ID_Gt']
+        myGts1["Sample_ID_Gt"] = my_input_c["Sample_ID_Gt"]
     else:
-        myGts1['Sample_ID_Gt'] = my_input.index
+        myGts1["Sample_ID_Gt"] = my_input.index
 
     if "Sample_ID_Ol" in my_input_c:
-        myOls1['Sample_ID_Ol'] = my_input_c['Sample_ID_Ol']
+        myOls1["Sample_ID_Ol"] = my_input_c["Sample_ID_Ol"]
     else:
-        myOls1['Sample_ID_Ol'] = my_input.index
+        myOls1["Sample_ID_Ol"] = my_input.index
 
     if "Sample_ID_Kspar" in my_input_c:
-        myKspars1['Sample_ID_Kspar'] = my_input_c['Sample_ID_Kspar']
+        myKspars1["Sample_ID_Kspar"] = my_input_c["Sample_ID_Kspar"]
     else:
-        myKspars1['Sample_ID_Kspar'] = my_input.index
+        myKspars1["Sample_ID_Kspar"] = my_input.index
 
     if "Sample_ID_Sp" in my_input_c:
-        mySps1['Sample_ID_Sp'] = my_input_c['Sample_ID_Sp']
+        mySps1["Sample_ID_Sp"] = my_input_c["Sample_ID_Sp"]
     else:
-        mySps1['Sample_ID_Sp'] = my_input.index
+        mySps1["Sample_ID_Sp"] = my_input.index
 
-    return {'my_input': my_input, 'my_oxides': myOxides1, # 'Experimental_press_temp': Experimental_press_temp1, 
-            'Cpxs': myCPXs1, 'Opxs': myOPXs1, 'Liqs': myLiquids1, 'Gts': myGts1,
-            'Plags': myPlags1, 'Kspars': myKspars1, 'Amps': myAmphs1, 'Ols': myOls1, 'Sps': mySps1}  # , 'y1': y1 ,'y2': y2}
+    return {
+        "my_input": my_input,
+        "my_oxides": myOxides1,  # 'Experimental_press_temp': Experimental_press_temp1,
+        "Cpxs": myCPXs1,
+        "Opxs": myOPXs1,
+        "Liqs": myLiquids1,
+        "Gts": myGts1,
+        "Plags": myPlags1,
+        "Kspars": myKspars1,
+        "Amps": myAmphs1,
+        "Ols": myOls1,
+        "Sps": mySps1,
+    }  # , 'y1': y1 ,'y2': y2}
 
 
+# %%
 
-# %% 
 
 def calculate_mol_proportions(comps):
-
     """
-    
-    Import mineral compositions using comps=My_Oxides, returns mole proportions. 
+
+    Import mineral compositions using comps=My_Oxides, returns mole proportions.
 
     Parameters
     -------
     comps: pandas.DataFrame
             Panda DataFrame of oxide compositions with column headings SiO2, MgO etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for oxides with column headings of the form SiO2_mol_prop
-    
-    """
 
-    oxide_mass_ox = {'SiO2': 60.0843, 'MgO': 40.3044, 'FeOt': 71.8464, 'CaO': 56.0774,'Al2O3': 101.961, 'Na2O': 61.9789, 'K2O': 94.196, 'MnO': 70.9375, 'TiO2': 79.7877, 'Cr2O3': 151.9982, 'P2O5': 141.937}
+    """
 
-    oxide_mass_df = pd.DataFrame.from_dict(oxide_mass_ox, orient='index').T
-    oxide_mass_df['Sample_ID'] = 'MolWt'
-    oxide_mass_df.set_index('Sample_ID', inplace=True)
+    oxide_mass_ox = {
+        "SiO2": 60.0843,
+        "MgO": 40.3044,
+        "FeOt": 71.8464,
+        "CaO": 56.0774,
+        "Al2O3": 101.961,
+        "Na2O": 61.9789,
+        "K2O": 94.196,
+        "MnO": 70.9375,
+        "TiO2": 79.7877,
+        "Cr2O3": 151.9982,
+        "P2O5": 141.937,
+    }
+
+    oxide_mass_df = pd.DataFrame.from_dict(oxide_mass_ox, orient="index").T
+    oxide_mass_df["Sample_ID"] = "MolWt"
+    oxide_mass_df.set_index("Sample_ID", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     wt = comps.reindex(oxide_mass_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    wt_combo = pd.concat([oxide_mass_df, wt],)
+    wt_combo = pd.concat(
+        [oxide_mass_df, wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = wt_combo.div(
-        wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = wt_combo.div(wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
 
-
 def SiteCalculator(phase_filt, append, phase_name):
-
     phase_nosuf = phase_filt.copy()
 
     amp_sites = get_amp_sites_from_input_not_amp(phase_nosuf, append)
     cpx_sites = calculate_cpx_sites_from_input_not_cpx(phase_nosuf, append)
     opx_phase_nosuf = phase_nosuf.copy()
-    opx_phase_nosuf.columns = [col.replace(append, '_Opx') for col in opx_phase_nosuf.columns]
+    opx_phase_nosuf.columns = [
+        col.replace(append, "_Opx") for col in opx_phase_nosuf.columns
+    ]
     opx_sites = calculate_orthopyroxene_components(opx_phase_nosuf)
     plag_sites = calculate_plagioclase_components(phase_nosuf, append)
     ol_sites = calculate_olivine_components(phase_nosuf, append)
     sp_sites = calculate_spinel_components(phase_nosuf, append)
     ox_sites = calculate_oxide_components(phase_nosuf, append)
     ap_sites = calculate_apatite_components(phase_nosuf, append)
     bt_sites = calculate_biotite_components(phase_nosuf, append)
     qz_sites = calculate_quartz_components(phase_nosuf, append)
     gt_sites = calculate_garnet_components(phase_nosuf, append)
     kspar_sites = calculate_kspar_components(phase_nosuf, append)
 
-    phase_nosuf['Phase'] = phase_name
+    phase_nosuf["Phase"] = phase_name
 
-    phase_nosuf['Ca_B_Amp'] = amp_sites['Ca_B_Amp']
-    phase_nosuf['Na_K_A_Amp'] = amp_sites['Na_A_Amp'] + amp_sites['K_A_Amp']
-    phase_nosuf['Al_T_Amp'] = amp_sites['Al_T_Amp']
-    phase_nosuf['Si_T_Amp'] = amp_sites['Si_T_Amp']
-    phase_nosuf['Amp_Cation_Sum'] = amp_sites['Amp_Cation_Sum']
-
-    phase_nosuf['Ca_CaMgFe_Cpx'] = cpx_sites['Ca_CaMgFe_Cpx']
-    phase_nosuf['Jd_Cpx'] = cpx_sites['Jd_Cpx']
-    phase_nosuf['DiHd_Cpx_1996'] = cpx_sites['DiHd_Cpx_1996']
+    phase_nosuf["Ca_B_Amp"] = amp_sites["Ca_B_Amp"]
+    phase_nosuf["Na_K_A_Amp"] = amp_sites["Na_A_Amp"] + amp_sites["K_A_Amp"]
+    phase_nosuf["Al_T_Amp"] = amp_sites["Al_T_Amp"]
+    phase_nosuf["Si_T_Amp"] = amp_sites["Si_T_Amp"]
+    phase_nosuf["Amp_Cation_Sum"] = amp_sites["Amp_Cation_Sum"]
+
+    phase_nosuf["Ca_CaMgFe_Cpx"] = cpx_sites["Ca_CaMgFe_Cpx"]
+    phase_nosuf["Jd_Cpx"] = cpx_sites["Jd_Cpx"]
+    phase_nosuf["DiHd_Cpx_1996"] = cpx_sites["DiHd_Cpx_1996"]
 
     # DHZ pg 101
-    # cation occupation, Fe3+ technically also goes into Cpx. 
-    phase_nosuf['Si_Al_T_Cpx'] = cpx_sites['Si_Cpx_cat_6ox'] + cpx_sites['Al_Cpx_cat_6ox']
-    phase_nosuf['Al_Fe_Ti_Cr_Mg_Fe_Mn_M1_Cpx'] = cpx_sites['Al_Cpx_cat_6ox'] + cpx_sites['Fet_Cpx_cat_6ox'] 
-    + cpx_sites['Ti_Cpx_cat_6ox'] + cpx_sites['Cr_Cpx_cat_6ox'] + cpx_sites['Mg_Cpx_cat_6ox'] 
-    + cpx_sites['Fet_Cpx_cat_6ox'] + cpx_sites['Mn_Cpx_cat_6ox']
-    phase_nosuf['Mg_Fe_Mn_Ca_Na_M2_Cpx'] = cpx_sites['Mg_Cpx_cat_6ox'] + cpx_sites['Fet_Cpx_cat_6ox']
-    + cpx_sites['Mn_Cpx_cat_6ox'] + cpx_sites['Ca_Cpx_cat_6ox'] + cpx_sites['Na_Cpx_cat_6ox']
-    phase_nosuf['Cpx_Cation_Sum'] = cpx_sites['Cpx_Cation_Sum']
+    # cation occupation, Fe3+ technically also goes into Cpx.
+    phase_nosuf["Si_Al_T_Cpx"] = (
+        cpx_sites["Si_Cpx_cat_6ox"] + cpx_sites["Al_Cpx_cat_6ox"]
+    )
+    phase_nosuf["Al_Fe_Ti_Cr_Mg_Fe_Mn_M1_Cpx"] = (
+        cpx_sites["Al_Cpx_cat_6ox"] + cpx_sites["Fet_Cpx_cat_6ox"]
+    )
+    (
+        +cpx_sites["Ti_Cpx_cat_6ox"]
+        + cpx_sites["Cr_Cpx_cat_6ox"]
+        + cpx_sites["Mg_Cpx_cat_6ox"]
+    )
+    +cpx_sites["Fet_Cpx_cat_6ox"] + cpx_sites["Mn_Cpx_cat_6ox"]
+    phase_nosuf["Mg_Fe_Mn_Ca_Na_M2_Cpx"] = (
+        cpx_sites["Mg_Cpx_cat_6ox"] + cpx_sites["Fet_Cpx_cat_6ox"]
+    )
+    (
+        +cpx_sites["Mn_Cpx_cat_6ox"]
+        + cpx_sites["Ca_Cpx_cat_6ox"]
+        + cpx_sites["Na_Cpx_cat_6ox"]
+    )
+    phase_nosuf["Cpx_Cation_Sum"] = cpx_sites["Cpx_Cation_Sum"]
 
     # (Mg, Fe, Ca) (Mg, Fe, Al) (Si, Al)2O6.
-    phase_nosuf['Ca_CaMgFe_Opx'] = opx_sites['Ca_CaMgFe_Opx']
-    phase_nosuf['Si_Al_T_Opx'] = opx_sites['Si_Opx_cat_6ox'] + opx_sites['Al_Opx_cat_6ox']
-    phase_nosuf['Mg_Fe_Ca_Al_M_Opx'] = opx_sites['Mg_Opx_cat_6ox'] + opx_sites['Fet_Opx_cat_6ox'] 
-    + opx_sites['Ca_Opx_cat_6ox'] + opx_sites['Al_Opx_cat_6ox']
-    phase_nosuf['Opx_Cation_Sum'] = opx_sites['Opx_Cation_Sum']
-
-    # Orthopyroxenes have a general formula (Mg, Fe, Ca) (Mg, Fe, Al) (Si, Al)2O6. 
-
-    phase_nosuf['Na_Ca_M_Plag'] = plag_sites['Na_Ca_M_Plag']
-    phase_nosuf['Si_Al_T_Plag'] = plag_sites['Si_Al_T_Plag']
-    phase_nosuf['Plag_Cation_Sum'] = plag_sites['Plag_Cation_Sum']
-
-    phase_nosuf['Mg_Fe_M_Ol'] = ol_sites['Mg_Fe_M_Ol']
-    phase_nosuf['Si_T_Ol'] = ol_sites['Si_T_Ol']
-    phase_nosuf['Mg_Fe_Ca_Mn_M_Ol'] = ol_sites['Mg_Fe_Ca_Mn_M_Ol']
-    phase_nosuf['Ol_Cation_Sum'] = ol_sites['Ol_Cation_Sum']
+    phase_nosuf["Ca_CaMgFe_Opx"] = opx_sites["Ca_CaMgFe_Opx"]
+    phase_nosuf["Si_Al_T_Opx"] = (
+        opx_sites["Si_Opx_cat_6ox"] + opx_sites["Al_Opx_cat_6ox"]
+    )
+    phase_nosuf["Mg_Fe_Ca_Al_M_Opx"] = (
+        opx_sites["Mg_Opx_cat_6ox"] + opx_sites["Fet_Opx_cat_6ox"]
+    )
+    +opx_sites["Ca_Opx_cat_6ox"] + opx_sites["Al_Opx_cat_6ox"]
+    phase_nosuf["Opx_Cation_Sum"] = opx_sites["Opx_Cation_Sum"]
+
+    # Orthopyroxenes have a general formula (Mg, Fe, Ca) (Mg, Fe, Al) (Si, Al)2O6.
+
+    phase_nosuf["Na_Ca_M_Plag"] = plag_sites["Na_Ca_M_Plag"]
+    phase_nosuf["Si_Al_T_Plag"] = plag_sites["Si_Al_T_Plag"]
+    phase_nosuf["Plag_Cation_Sum"] = plag_sites["Plag_Cation_Sum"]
+
+    phase_nosuf["Mg_Fe_M_Ol"] = ol_sites["Mg_Fe_M_Ol"]
+    phase_nosuf["Si_T_Ol"] = ol_sites["Si_T_Ol"]
+    phase_nosuf["Mg_Fe_Ca_Mn_M_Ol"] = ol_sites["Mg_Fe_Ca_Mn_M_Ol"]
+    phase_nosuf["Ol_Cation_Sum"] = ol_sites["Ol_Cation_Sum"]
 
     # there must be some Fe3+ but don't have a great estimate of speciation
-    phase_nosuf['Mg_Fe_M_Sp'] = sp_sites['Mg_Fe_M_Sp']
-    phase_nosuf['Al_B_Sp'] = sp_sites['Al_B_Sp']
-    phase_nosuf['Sp_Cation_Sum'] = sp_sites['Sp_Cation_Sum']
-
-    phase_nosuf['Fe_Ti_Ox'] = ox_sites['Fe_Ti_Ox']
-    phase_nosuf['Ox_Cation_Sum'] = ox_sites['Ox_Cation_Sum']
-
-    phase_nosuf['Ca_P_Ap'] = ap_sites['Ca_P_Ap']
-    phase_nosuf['Ap_Cation_Sum'] = ap_sites['Ap_Cation_Sum']
-
-    phase_nosuf['Mg_Fe_M_Bt'] = bt_sites['Mg_Fe_M_Bt']
-    phase_nosuf['Si_Al_T_Bt'] = bt_sites['Si_Al_T_Bt']
-    phase_nosuf['Bt_Cation_Sum'] = bt_sites['Bt_Cation_Sum']
-
-    phase_nosuf['Si_Al_Ti_Qz'] = qz_sites['Si_Al_Ti_Qz']
-    phase_nosuf['Qz_Cation_Sum'] = qz_sites['Qz_Cation_Sum']
-
-    phase_nosuf['Mg_MgFeCa_Gt'] = gt_sites['Mg_MgFeCa_Gt']
-    phase_nosuf['Fe_MgFeCa_Gt'] = gt_sites['Fe_MgFeCa_Gt']
-    phase_nosuf['Ca_MgFeCa_Gt'] = gt_sites['Ca_MgFeCa_Gt']
-    phase_nosuf[''] = gt_sites['Ca_Mg_Fe_Mn_X_Gt']
-    phase_nosuf['Al_Fe_Mn_Cr_Y_Gt'] = gt_sites['Al_Fe_Mn_Cr_Y_Gt']
-    phase_nosuf['Gt_Cation_Sum'] = gt_sites['Gt_Cation_Sum']
-
-    phase_nosuf['Na_Ca_M_Kspar'] = kspar_sites['Na_Ca_M_Kspar']
-    phase_nosuf['Si_Al_T_Kspar'] = kspar_sites['Si_Al_T_Kspar']
-    phase_nosuf['Kspar_Cation_Sum'] = kspar_sites['Kspar_Cation_Sum']
+    phase_nosuf["Mg_Fe_M_Sp"] = sp_sites["Mg_Fe_M_Sp"]
+    phase_nosuf["Al_B_Sp"] = sp_sites["Al_B_Sp"]
+    phase_nosuf["Sp_Cation_Sum"] = sp_sites["Sp_Cation_Sum"]
+
+    phase_nosuf["Fe_Ti_Ox"] = ox_sites["Fe_Ti_Ox"]
+    phase_nosuf["Ox_Cation_Sum"] = ox_sites["Ox_Cation_Sum"]
+
+    phase_nosuf["Ca_P_Ap"] = ap_sites["Ca_P_Ap"]
+    phase_nosuf["Ap_Cation_Sum"] = ap_sites["Ap_Cation_Sum"]
+
+    phase_nosuf["Mg_Fe_M_Bt"] = bt_sites["Mg_Fe_M_Bt"]
+    phase_nosuf["Si_Al_T_Bt"] = bt_sites["Si_Al_T_Bt"]
+    phase_nosuf["Bt_Cation_Sum"] = bt_sites["Bt_Cation_Sum"]
+
+    phase_nosuf["Si_Al_Ti_Qz"] = qz_sites["Si_Al_Ti_Qz"]
+    phase_nosuf["Qz_Cation_Sum"] = qz_sites["Qz_Cation_Sum"]
+
+    phase_nosuf["Mg_MgFeCa_Gt"] = gt_sites["Mg_MgFeCa_Gt"]
+    phase_nosuf["Fe_MgFeCa_Gt"] = gt_sites["Fe_MgFeCa_Gt"]
+    phase_nosuf["Ca_MgFeCa_Gt"] = gt_sites["Ca_MgFeCa_Gt"]
+    phase_nosuf[""] = gt_sites["Ca_Mg_Fe_Mn_X_Gt"]
+    phase_nosuf["Al_Fe_Mn_Cr_Y_Gt"] = gt_sites["Al_Fe_Mn_Cr_Y_Gt"]
+    phase_nosuf["Gt_Cation_Sum"] = gt_sites["Gt_Cation_Sum"]
+
+    phase_nosuf["Na_Ca_M_Kspar"] = kspar_sites["Na_Ca_M_Kspar"]
+    phase_nosuf["Si_Al_T_Kspar"] = kspar_sites["Si_Al_T_Kspar"]
+    phase_nosuf["Kspar_Cation_Sum"] = kspar_sites["Kspar_Cation_Sum"]
 
     return phase_nosuf
 
+
 # %% OLIVINE
 
 
 def calculate_mol_proportions_olivine(ol_comps):
-
     """
-    
+
     Import Olivine compositions using ol_comps=My_Olivines, returns mole proportions
 
     Parameters
     -------
     ol_comps: pandas.DataFrame
             Panda DataFrame of olivine compositions with column headings SiO2_Ol, MgO_Ol etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for olivines with column headings of the form SiO2_Ol_mol_prop
 
     """
 
-    oxide_mass_ol = {'SiO2_Ol': 60.0843, 'MgO_Ol': 40.3044, 'FeOt_Ol': 71.8464, 'CaO_Ol': 56.0774,'Al2O3_Ol': 101.961, 'Na2O_Ol': 61.9789, 'K2O_Ol': 94.196, 'MnO_Ol': 70.9375, 'TiO2_Ol': 79.7877}
-    oxide_mass_ol_df = pd.DataFrame.from_dict(oxide_mass_ol, orient='index').T
-    oxide_mass_ol_df['Sample_ID_Ol'] = 'MolWt'
-    oxide_mass_ol_df.set_index('Sample_ID_Ol', inplace=True)
+    oxide_mass_ol = {
+        "SiO2_Ol": 60.0843,
+        "MgO_Ol": 40.3044,
+        "FeOt_Ol": 71.8464,
+        "CaO_Ol": 56.0774,
+        "Al2O3_Ol": 101.961,
+        "Na2O_Ol": 61.9789,
+        "K2O_Ol": 94.196,
+        "MnO_Ol": 70.9375,
+        "TiO2_Ol": 79.7877,
+    }
+    oxide_mass_ol_df = pd.DataFrame.from_dict(oxide_mass_ol, orient="index").T
+    oxide_mass_ol_df["Sample_ID_Ol"] = "MolWt"
+    oxide_mass_ol_df.set_index("Sample_ID_Ol", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     ol_wt = ol_comps.reindex(oxide_mass_ol_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    ol_wt_combo = pd.concat([oxide_mass_ol_df, ol_wt],)
+    ol_wt_combo = pd.concat(
+        [oxide_mass_ol_df, ol_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = ol_wt_combo.div(
-        ol_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = ol_wt_combo.div(ol_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
 
 def calculate_oxygens_olivine(ol_comps):
-
     """
-    
-    Import olivine compositions using ol_comps=My_Ols, returns number of oxygens 
+
+    Import olivine compositions using ol_comps=My_Ols, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     ol_comps: pandas.DataFrame
         olivine compositions with column headings SiO2_Ol, MgO_Ol etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Ol_ox
 
     """
 
-    oxygen_num_ol = {'SiO2_Ol': 2, 'MgO_Ol': 1, 'FeOt_Ol': 1, 'CaO_Ol': 1, 'Al2O3_Ol': 3, 'Na2O_Ol': 1, 'K2O_Ol': 1, 'MnO_Ol': 1, 'TiO2_Ol': 2, 'Cr2O3_Ol': 3, 'P2O5_Ol': 5}
-    oxygen_num_ol_df = pd.DataFrame.from_dict(oxygen_num_ol, orient='index').T
-    oxygen_num_ol_df['Sample_ID_Ol'] = 'OxNum'
-    oxygen_num_ol_df.set_index('Sample_ID_Ol', inplace=True)
+    oxygen_num_ol = {
+        "SiO2_Ol": 2,
+        "MgO_Ol": 1,
+        "FeOt_Ol": 1,
+        "CaO_Ol": 1,
+        "Al2O3_Ol": 3,
+        "Na2O_Ol": 1,
+        "K2O_Ol": 1,
+        "MnO_Ol": 1,
+        "TiO2_Ol": 2,
+        "Cr2O3_Ol": 3,
+        "P2O5_Ol": 5,
+    }
+    oxygen_num_ol_df = pd.DataFrame.from_dict(oxygen_num_ol, orient="index").T
+    oxygen_num_ol_df["Sample_ID_Ol"] = "OxNum"
+    oxygen_num_ol_df.set_index("Sample_ID_Ol", inplace=True)
 
     mol_prop = calculate_mol_proportions_olivine(ol_comps=ol_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
-    ox_num_reindex = oxygen_num_ol_df.reindex(
-        mol_prop.columns, axis=1).fillna(0)
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
+    ox_num_reindex = oxygen_num_ol_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
     oxygens_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
 
 def calculate_4oxygens_olivine(ol_comps):
-
     """
-    
+
     Import olivine compositions using ol_comps=My_Ols, returns cations on the basis of 4 oxygens.
 
     Parameters
     -------
     ol_comps: pandas.DataFrame
         olivine compositions with column headings SiO2_Ol, MgO_Ol etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 4 oxygens, with column headings of the form... Ol_cat_4ox.
-    
-    """
 
-    cation_num_ol = {'SiO2_Ol': 1, 'MgO_Ol': 1, 'FeOt_Ol': 1, 'CaO_Ol': 1, 'Al2O3_Ol': 2, 'Na2O_Ol': 2, 'K2O_Ol': 2, 'MnO_Ol': 1, 'TiO2_Ol': 1, 'Cr2O3_Ol': 2, 'P2O5_Ol': 2}
+    """
 
-    cation_num_ol_df = pd.DataFrame.from_dict(cation_num_ol, orient='index').T
-    cation_num_ol_df['Sample_ID_Ol'] = 'CatNum'
-    cation_num_ol_df.set_index('Sample_ID_Ol', inplace=True)
+    cation_num_ol = {
+        "SiO2_Ol": 1,
+        "MgO_Ol": 1,
+        "FeOt_Ol": 1,
+        "CaO_Ol": 1,
+        "Al2O3_Ol": 2,
+        "Na2O_Ol": 2,
+        "K2O_Ol": 2,
+        "MnO_Ol": 1,
+        "TiO2_Ol": 1,
+        "Cr2O3_Ol": 2,
+        "P2O5_Ol": 2,
+    }
+
+    cation_num_ol_df = pd.DataFrame.from_dict(cation_num_ol, orient="index").T
+    cation_num_ol_df["Sample_ID_Ol"] = "CatNum"
+    cation_num_ol_df.set_index("Sample_ID_Ol", inplace=True)
 
     oxygens = calculate_oxygens_olivine(ol_comps=ol_comps)
-    renorm_factor = 4 / (oxygens.sum(axis='columns'))
+    renorm_factor = 4 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_olivine(ol_comps=ol_comps)
-    mol_prop['oxy_renorm_factor_ol'] = renorm_factor
-    mol_prop_4 = mol_prop.multiply(mol_prop['oxy_renorm_factor_ol'], axis='rows')
-    mol_prop_4.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_4.columns]
+    mol_prop["oxy_renorm_factor_ol"] = renorm_factor
+    mol_prop_4 = mol_prop.multiply(mol_prop["oxy_renorm_factor_ol"], axis="rows")
+    mol_prop_4.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_4.columns
+    ]
 
-    ox_num_reindex = cation_num_ol_df.reindex(
-        mol_prop_4.columns, axis=1).fillna(0)
+    ox_num_reindex = cation_num_ol_df.reindex(mol_prop_4.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_4])
     cation_4 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_4.columns = [str(col).replace('_mol_prop', '_cat_4ox')
-                        for col in mol_prop.columns]
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_4_2=cation_4.rename(columns={
-                            'SiO2_Ol_cat_4ox': 'Si_Ol_cat_4ox',
-                            'TiO2_Ol_cat_4ox': 'Ti_Ol_cat_4ox',
-                            'Al2O3_Ol_cat_4ox': 'Al_Ol_cat_4ox',
-                            'FeOt_Ol_cat_4ox': 'Fet_Ol_cat_4ox',
-                            'MnO_Ol_cat_4ox': 'Mn_Ol_cat_4ox',
-                            'MgO_Ol_cat_4ox': 'Mg_Ol_cat_4ox',
-                            'CaO_Ol_cat_4ox': 'Ca_Ol_cat_4ox',
-                            'Na2O_Ol_cat_4ox': 'Na_Ol_cat_4ox',
-                            'K2O_Ol_cat_4ox': 'K_Ol_cat_4ox',
-                            'Cr2O3_Ol_cat_4ox': 'Cr_Ol_cat_4ox',
-                            'P2O5_Ol_cat_4ox': 'P_Ol_cat_4ox',})
+    cation_4.columns = [
+        str(col).replace("_mol_prop", "_cat_4ox") for col in mol_prop.columns
+    ]
+
+    cation_4_2 = cation_4.rename(
+        columns={
+            "SiO2_Ol_cat_4ox": "Si_Ol_cat_4ox",
+            "TiO2_Ol_cat_4ox": "Ti_Ol_cat_4ox",
+            "Al2O3_Ol_cat_4ox": "Al_Ol_cat_4ox",
+            "FeOt_Ol_cat_4ox": "Fet_Ol_cat_4ox",
+            "MnO_Ol_cat_4ox": "Mn_Ol_cat_4ox",
+            "MgO_Ol_cat_4ox": "Mg_Ol_cat_4ox",
+            "CaO_Ol_cat_4ox": "Ca_Ol_cat_4ox",
+            "Na2O_Ol_cat_4ox": "Na_Ol_cat_4ox",
+            "K2O_Ol_cat_4ox": "K_Ol_cat_4ox",
+            "Cr2O3_Ol_cat_4ox": "Cr_Ol_cat_4ox",
+            "P2O5_Ol_cat_4ox": "P_Ol_cat_4ox",
+        }
+    )
 
     return cation_4_2
 
+
 def calculate_cat_proportions_olivine(ol_comps):
-    
     """
-    
+
     Import Olivine compositions using ol_comps=My_Olivines, returns cation proportions
 
     Parameters
     -------
     ol_comps: pandas.DataFrame
             olivine compositions with column headings SiO2_Ol, MgO_Ol etc.
 
@@ -494,56 +606,82 @@
     pandas DataFrame
         cation proportions for olivine with column headings of the form SiO2_Ol_cat_prop
         For simplicity, and consistency of column heading types, oxide names are preserved,
         so outputs are Na2O_Ol_cat_prop rather than Na_Ol_cat_prop.
 
     """
 
-    oxide_mass_ol = {'SiO2_Ol': 60.0843, 'MgO_Ol': 40.3044, 'FeOt_Ol': 71.8464, 'CaO_Ol': 56.0774,'Al2O3_Ol': 101.961, 'Na2O_Ol': 61.9789, 'K2O_Ol': 94.196, 'MnO_Ol': 70.9375, 'TiO2_Ol': 79.7877}
-    oxide_mass_ol_df = pd.DataFrame.from_dict(oxide_mass_ol, orient='index').T
-    oxide_mass_ol_df['Sample_ID_Ol'] = 'MolWt'
-    oxide_mass_ol_df.set_index('Sample_ID_Ol', inplace=True)
-
-    cation_num_ol = {'SiO2_Ol': 1, 'MgO_Ol': 1, 'FeOt_Ol': 1, 'CaO_Ol': 1, 'Al2O3_Ol': 2, 'Na2O_Ol': 2, 'K2O_Ol': 2, 'MnO_Ol': 1, 'TiO2_Ol': 1, 'P2O5_Ol': 2}
-    cation_num_ol_df = pd.DataFrame.from_dict(cation_num_ol, orient='index').T
-    cation_num_ol_df['Sample_ID_Ol'] = 'CatNum'
-    cation_num_ol_df.set_index('Sample_ID_Ol', inplace=True)
+    oxide_mass_ol = {
+        "SiO2_Ol": 60.0843,
+        "MgO_Ol": 40.3044,
+        "FeOt_Ol": 71.8464,
+        "CaO_Ol": 56.0774,
+        "Al2O3_Ol": 101.961,
+        "Na2O_Ol": 61.9789,
+        "K2O_Ol": 94.196,
+        "MnO_Ol": 70.9375,
+        "TiO2_Ol": 79.7877,
+    }
+    oxide_mass_ol_df = pd.DataFrame.from_dict(oxide_mass_ol, orient="index").T
+    oxide_mass_ol_df["Sample_ID_Ol"] = "MolWt"
+    oxide_mass_ol_df.set_index("Sample_ID_Ol", inplace=True)
+
+    cation_num_ol = {
+        "SiO2_Ol": 1,
+        "MgO_Ol": 1,
+        "FeOt_Ol": 1,
+        "CaO_Ol": 1,
+        "Al2O3_Ol": 2,
+        "Na2O_Ol": 2,
+        "K2O_Ol": 2,
+        "MnO_Ol": 1,
+        "TiO2_Ol": 1,
+        "P2O5_Ol": 2,
+    }
+    cation_num_ol_df = pd.DataFrame.from_dict(cation_num_ol, orient="index").T
+    cation_num_ol_df["Sample_ID_Ol"] = "CatNum"
+    cation_num_ol_df.set_index("Sample_ID_Ol", inplace=True)
 
     mol_prop_no_cat_num = calculate_mol_proportions_olivine(ol_comps=ol_comps)
-    mol_prop_no_cat_num.columns = [str(col).replace(
-        '_mol_prop', '') for col in mol_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_ol_df.reindex(
-        oxide_mass_ol_df.columns, axis=1).fillna(0)
+    mol_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_ol_df.reindex(oxide_mass_ol_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_no_cat_num])
     cation_prop_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
     cation_prop_anhyd.columns = [
-        str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
 
-    cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                        'SiO2_Ol_cat_prop': 'Si_Ol_cat_prop',
-                        'TiO2_Ol_cat_prop': 'Ti_Ol_cat_prop',
-                        'Al2O3_Ol_cat_prop': 'Al_Ol_cat_prop',
-                        'FeOt_Ol_cat_prop': 'Fet_Ol_cat_prop',
-                        'MnO_Ol_cat_prop': 'Mn_Ol_cat_prop',
-                        'MgO_Ol_cat_prop': 'Mg_Ol_cat_prop',
-                        'CaO_Ol_cat_prop': 'Ca_Ol_cat_prop',
-                        'Na2O_Ol_cat_prop': 'Na_Ol_cat_prop',
-                        'K2O_Ol_cat_prop': 'K_Ol_cat_prop',
-                        'Cr2O3_Ol_cat_prop': 'Cr_Ol_cat_prop',
-                        'P2O5_Ol_cat_prop': 'P_Ol_cat_prop',
-                        })
+    cation_prop_anhyd2 = cation_prop_anhyd.rename(
+        columns={
+            "SiO2_Ol_cat_prop": "Si_Ol_cat_prop",
+            "TiO2_Ol_cat_prop": "Ti_Ol_cat_prop",
+            "Al2O3_Ol_cat_prop": "Al_Ol_cat_prop",
+            "FeOt_Ol_cat_prop": "Fet_Ol_cat_prop",
+            "MnO_Ol_cat_prop": "Mn_Ol_cat_prop",
+            "MgO_Ol_cat_prop": "Mg_Ol_cat_prop",
+            "CaO_Ol_cat_prop": "Ca_Ol_cat_prop",
+            "Na2O_Ol_cat_prop": "Na_Ol_cat_prop",
+            "K2O_Ol_cat_prop": "K_Ol_cat_prop",
+            "Cr2O3_Ol_cat_prop": "Cr_Ol_cat_prop",
+            "P2O5_Ol_cat_prop": "P_Ol_cat_prop",
+        }
+    )
 
     return cation_prop_anhyd2
 
 
 def calculate_olivine_components(ol_comps, append):
-
     """
-    
+
     Import olivine compositions using ol_comps=My_Ols, returns components on the basis of 4 oxygens.
 
     Parameters
     -------
     ol_comps: pandas.DataFrame
         olivine compositions with column headings SiO2_Ol, MgO_Ol etc.
 
@@ -551,85 +689,112 @@
     -------
     pandas DataFrame
         components on the basis of 4 oxygens, with column headings of the form... Ol_cat_4ox.
 
     """
 
     ol_comps_new = ol_comps.copy()
-    ol_comps_new.columns = [col.replace(append, '_Ol') for col in ol_comps_new.columns]
+    ol_comps_new.columns = [col.replace(append, "_Ol") for col in ol_comps_new.columns]
     ol_comps = ol_comps_new.copy()
 
     ol_calc = calculate_4oxygens_olivine(ol_comps=ol_comps)
-    ol_calc['Ol_Cation_Sum'] = (ol_calc['Si_Ol_cat_4ox']+ol_calc['Ti_Ol_cat_4ox']+ol_calc['Al_Ol_cat_4ox']+ol_calc['Fet_Ol_cat_4ox']+ol_calc['Mn_Ol_cat_4ox']+ol_calc['Mg_Ol_cat_4ox']+ol_calc['Ca_Ol_cat_4ox']+ol_calc['Na_Ol_cat_4ox']+ol_calc['K_Ol_cat_4ox'])
+    ol_calc["Ol_Cation_Sum"] = (
+        ol_calc["Si_Ol_cat_4ox"]
+        + ol_calc["Ti_Ol_cat_4ox"]
+        + ol_calc["Al_Ol_cat_4ox"]
+        + ol_calc["Fet_Ol_cat_4ox"]
+        + ol_calc["Mn_Ol_cat_4ox"]
+        + ol_calc["Mg_Ol_cat_4ox"]
+        + ol_calc["Ca_Ol_cat_4ox"]
+        + ol_calc["Na_Ol_cat_4ox"]
+        + ol_calc["K_Ol_cat_4ox"]
+    )
 
-    ol_calc['Mg_Fe_M_Ol'] = ol_calc['Mg_Ol_cat_4ox'] + ol_calc['Fet_Ol_cat_4ox']
-    ol_calc['Si_T_Ol'] = ol_calc['Si_Ol_cat_4ox'] 
+    ol_calc["Mg_Fe_M_Ol"] = ol_calc["Mg_Ol_cat_4ox"] + ol_calc["Fet_Ol_cat_4ox"]
+    ol_calc["Si_T_Ol"] = ol_calc["Si_Ol_cat_4ox"]
 
     # G. Cressey, R.A. Howie, in Encyclopedia of Geology, 2005
-    # Ni not often measured. 
+    # Ni not often measured.
     # Mg-Fe olivines - Mg2+ and Fe2+ can occupy M1 and M2 with almost equal preference. Slight tendency for Fe2+ to occupy the M1 site rather than the M2 site
     # Mg-Fe olivines - small proportion of Ca and Mn present. Substitution of Mn2+ for Fe2+ in fayalite also occurs.
-    # Ca olivines: Ca2+ occupies the (larger) M2 site, while Mg2+ and Fe2+ are randomly distributed on the M1 sites. 
-    ol_calc['Mg_Fe_Ca_Mn_M_Ol'] = ol_calc['Mg_Ol_cat_4ox'] + ol_calc['Fet_Ol_cat_4ox'] + ol_calc['Ca_Ol_cat_4ox'] + ol_calc['Mn_Ol_cat_4ox']
+    # Ca olivines: Ca2+ occupies the (larger) M2 site, while Mg2+ and Fe2+ are randomly distributed on the M1 sites.
+    ol_calc["Mg_Fe_Ca_Mn_M_Ol"] = (
+        ol_calc["Mg_Ol_cat_4ox"]
+        + ol_calc["Fet_Ol_cat_4ox"]
+        + ol_calc["Ca_Ol_cat_4ox"]
+        + ol_calc["Mn_Ol_cat_4ox"]
+    )
 
     cat_prop = calculate_cat_proportions_olivine(ol_comps=ol_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([ol_comps, ol_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
 # %% PLAGIOCLASE
 
 
 def calculate_mol_proportions_plagioclase(*, plag_comps=None):
-
     """
-    
+
     Import plagioclase compositions using plag_comps=My_plagioclases, returns mole proportions
 
     Parameters
     -------
     plag_comps: pandas.DataFrame
             Panda DataFrame of plagioclase compositions with column headings SiO2_Plag, MgO_Plag etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for plagioclases with column headings of the form SiO2_Plag_mol_prop
 
     """
 
-    oxide_mass_plag = {'SiO2_Plag': 60.0843, 'MgO_Plag': 40.3044, 'FeOt_Plag': 71.8464, 'CaO_Plag': 56.0774, 'Al2O3_Plag': 101.961, 'Na2O_Plag': 61.9789, 'K2O_Plag': 94.196, 'MnO_Plag': 70.9375, 'TiO2_Plag': 79.8788, 'Cr2O3_Plag': 151.9982}
-    oxide_mass_plag_df = pd.DataFrame.from_dict(oxide_mass_plag, orient='index').T
-    oxide_mass_plag_df['Sample_ID_Plag'] = 'MolWt'
-    oxide_mass_plag_df.set_index('Sample_ID_Plag', inplace=True)
+    oxide_mass_plag = {
+        "SiO2_Plag": 60.0843,
+        "MgO_Plag": 40.3044,
+        "FeOt_Plag": 71.8464,
+        "CaO_Plag": 56.0774,
+        "Al2O3_Plag": 101.961,
+        "Na2O_Plag": 61.9789,
+        "K2O_Plag": 94.196,
+        "MnO_Plag": 70.9375,
+        "TiO2_Plag": 79.8788,
+        "Cr2O3_Plag": 151.9982,
+    }
+    oxide_mass_plag_df = pd.DataFrame.from_dict(oxide_mass_plag, orient="index").T
+    oxide_mass_plag_df["Sample_ID_Plag"] = "MolWt"
+    oxide_mass_plag_df.set_index("Sample_ID_Plag", inplace=True)
 
     if plag_comps is not None:
         plag_comps = plag_comps
         # This makes it match the columns in the oxide mass dataframe
-        plag_wt = plag_comps.reindex(
-            oxide_mass_plag_df.columns, axis=1).fillna(0)
+        plag_wt = plag_comps.reindex(oxide_mass_plag_df.columns, axis=1).fillna(0)
         # Combine the molecular weight and weight percent dataframes
-        plag_wt_combo = pd.concat([oxide_mass_plag_df, plag_wt],)
+        plag_wt_combo = pd.concat(
+            [oxide_mass_plag_df, plag_wt],
+        )
         # Drop the calculation column
         plag_prop_anhyd = plag_wt_combo.div(
-            plag_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
+            plag_wt_combo.loc["MolWt", :], axis="columns"
+        ).drop(["MolWt"])
         plag_prop_anhyd.columns = [
-            str(col) + '_mol_prop' for col in plag_prop_anhyd.columns]
+            str(col) + "_mol_prop" for col in plag_prop_anhyd.columns
+        ]
         return plag_prop_anhyd
 
 
-
 def calculate_mol_fractions_plagioclase(*, plag_comps=None):
-
     """
     Import plagioclase compositions using plag_comps=My_plagioclases, returns mole fractions
 
     Parameters
     -------
     plag_comps: pandas.DataFrame
             plagioclase compositions with column headings SiO2_Plag, MgO_Plag etc.
@@ -639,29 +804,27 @@
     pandas DataFrame
         mole fractions for plagioclases with column headings of the form SiO2_Plag_mol_frac
 
     """
 
     if plag_comps is not None:
         plag_comps = plag_comps
-        plag_prop = calculate_mol_proportions_plagioclase(
-            plag_comps=plag_comps)
-        plag_prop['sum'] = plag_prop.sum(axis='columns')
-        plag_frac_anhyd = plag_prop.div(plag_prop['sum'], axis='rows')
-        plag_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-        plag_frac_anhyd.columns = [str(col).replace(
-            'prop', 'frac') for col in plag_frac_anhyd.columns]
+        plag_prop = calculate_mol_proportions_plagioclase(plag_comps=plag_comps)
+        plag_prop["sum"] = plag_prop.sum(axis="columns")
+        plag_frac_anhyd = plag_prop.div(plag_prop["sum"], axis="rows")
+        plag_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+        plag_frac_anhyd.columns = [
+            str(col).replace("prop", "frac") for col in plag_frac_anhyd.columns
+        ]
         return plag_frac_anhyd
 
 
-
 def calculate_cat_proportions_plagioclase(*, plag_comps=None, oxide_headers=False):
-    
     """
-    
+
     Import plagioclase compositions using plag_comps=My_plagioclases, returns cation proportions
 
     Parameters
     -------
     plag_comps: pandas.DataFrame
             plagioclase compositions with column headings SiO2_Plag, MgO_Plag etc.
     oxide_headers: bool
@@ -670,186 +833,247 @@
         This is used for rapid matrix division for
         pre-processing of data for cation fractions etc
 
     Returns
     -------
     pandas DataFrame
         cation proportions for plagioclase with column headings of the form ...Plag_cat_prop
-        
-    """
 
-    oxide_mass_plag = {'SiO2_Plag': 60.0843, 'MgO_Plag': 40.3044, 'FeOt_Plag': 71.8464, 'CaO_Plag': 56.0774, 'Al2O3_Plag': 101.961, 'Na2O_Plag': 61.9789, 'K2O_Plag': 94.196, 'MnO_Plag': 70.9375, 'TiO2_Plag': 79.8788, 'Cr2O3_Plag': 151.9982}
-    oxide_mass_plag_df = pd.DataFrame.from_dict(oxide_mass_plag, orient='index').T
-    oxide_mass_plag_df['Sample_ID_Plag'] = 'MolWt'
-    oxide_mass_plag_df.set_index('Sample_ID_Plag', inplace=True)
-
-    cation_num_plag = {'SiO2_Plag': 1, 'MgO_Plag': 1, 'FeOt_Plag': 1, 'CaO_Plag': 1, 'Al2O3_Plag': 2, 'Na2O_Plag': 2, 'K2O_Plag': 2, 'MnO_Plag': 1, 'TiO2_Plag': 1, 'Cr2O3_Plag': 2}
-
-    cation_num_plag_df = pd.DataFrame.from_dict(cation_num_plag, orient='index').T
-    cation_num_plag_df['Sample_ID_Plag'] = 'CatNum'
-    cation_num_plag_df.set_index('Sample_ID_Plag', inplace=True)
+    """
 
-    plag_prop_no_cat_num = calculate_mol_proportions_plagioclase(
-        plag_comps=plag_comps)
-    plag_prop_no_cat_num.columns = [str(col).replace(
-        '_mol_prop', '') for col in plag_prop_no_cat_num.columns]
+    oxide_mass_plag = {
+        "SiO2_Plag": 60.0843,
+        "MgO_Plag": 40.3044,
+        "FeOt_Plag": 71.8464,
+        "CaO_Plag": 56.0774,
+        "Al2O3_Plag": 101.961,
+        "Na2O_Plag": 61.9789,
+        "K2O_Plag": 94.196,
+        "MnO_Plag": 70.9375,
+        "TiO2_Plag": 79.8788,
+        "Cr2O3_Plag": 151.9982,
+    }
+    oxide_mass_plag_df = pd.DataFrame.from_dict(oxide_mass_plag, orient="index").T
+    oxide_mass_plag_df["Sample_ID_Plag"] = "MolWt"
+    oxide_mass_plag_df.set_index("Sample_ID_Plag", inplace=True)
+
+    cation_num_plag = {
+        "SiO2_Plag": 1,
+        "MgO_Plag": 1,
+        "FeOt_Plag": 1,
+        "CaO_Plag": 1,
+        "Al2O3_Plag": 2,
+        "Na2O_Plag": 2,
+        "K2O_Plag": 2,
+        "MnO_Plag": 1,
+        "TiO2_Plag": 1,
+        "Cr2O3_Plag": 2,
+    }
+
+    cation_num_plag_df = pd.DataFrame.from_dict(cation_num_plag, orient="index").T
+    cation_num_plag_df["Sample_ID_Plag"] = "CatNum"
+    cation_num_plag_df.set_index("Sample_ID_Plag", inplace=True)
+
+    plag_prop_no_cat_num = calculate_mol_proportions_plagioclase(plag_comps=plag_comps)
+    plag_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in plag_prop_no_cat_num.columns
+    ]
     ox_num_reindex = cation_num_plag_df.reindex(
-        oxide_mass_plag_df.columns, axis=1).fillna(0)
+        oxide_mass_plag_df.columns, axis=1
+    ).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, plag_prop_no_cat_num])
     cation_prop_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
     cation_prop_anhyd.columns = [
-        str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Plag_cat_prop': 'Si_Plag_cat_prop',
-                            'TiO2_Plag_cat_prop': 'Ti_Plag_cat_prop',
-                            'Al2O3_Plag_cat_prop': 'Al_Plag_cat_prop',
-                            'FeOt_Plag_cat_prop': 'Fet_Plag_cat_prop',
-                            'MnO_Plag_cat_prop': 'Mn_Plag_cat_prop',
-                            'MgO_Plag_cat_prop': 'Mg_Plag_cat_prop',
-                            'CaO_Plag_cat_prop': 'Ca_Plag_cat_prop',
-                            'Na2O_Plag_cat_prop': 'Na_Plag_cat_prop',
-                            'K2O_Plag_cat_prop': 'K_Plag_cat_prop',
-                            'Cr2O3_Plag_cat_prop': 'Cr_Plag_cat_prop',
-                            'P2O5_Plag_cat_prop': 'P_Plag_cat_prop',
-                            })
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Plag_cat_prop": "Si_Plag_cat_prop",
+                "TiO2_Plag_cat_prop": "Ti_Plag_cat_prop",
+                "Al2O3_Plag_cat_prop": "Al_Plag_cat_prop",
+                "FeOt_Plag_cat_prop": "Fet_Plag_cat_prop",
+                "MnO_Plag_cat_prop": "Mn_Plag_cat_prop",
+                "MgO_Plag_cat_prop": "Mg_Plag_cat_prop",
+                "CaO_Plag_cat_prop": "Ca_Plag_cat_prop",
+                "Na2O_Plag_cat_prop": "Na_Plag_cat_prop",
+                "K2O_Plag_cat_prop": "K_Plag_cat_prop",
+                "Cr2O3_Plag_cat_prop": "Cr_Plag_cat_prop",
+                "P2O5_Plag_cat_prop": "P_Plag_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
 
-
 def calculate_cat_fractions_plagioclase(plag_comps):
-    
     """
-    
+
     Import plagioclase compositions using plag_comps=My_plagioclases, returns cation fractions
 
-    Parameters: 
-        plag_comps (pandas.DataFrame): plagioclase compositions with column headings SiO2_Plag, 
+    Parameters:
+        plag_comps (pandas.DataFrame): plagioclase compositions with column headings SiO2_Plag,
                                        MgO_Plag etc.
 
-    Returns: 
-        cat_frac_anhyd2 (pandas.DataFrame): cation fractions for plagioclase with column headings 
+    Returns:
+        cat_frac_anhyd2 (pandas.DataFrame): cation fractions for plagioclase with column headings
                                             of the form ...Plag_cat_frac.
 
     """
 
     cat_prop = calculate_cat_proportions_plagioclase(plag_comps=plag_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
-    cat_frac_anhyd['An_Plag'] = cat_frac_anhyd['Ca_Plag_cat_frac'] / (cat_frac_anhyd['Ca_Plag_cat_frac'] + cat_frac_anhyd['Na_Plag_cat_frac'] + cat_frac_anhyd['K_Plag_cat_frac'])
-    cat_frac_anhyd['Ab_Plag'] = cat_frac_anhyd['Na_Plag_cat_frac'] / (cat_frac_anhyd['Ca_Plag_cat_frac'] + cat_frac_anhyd['Na_Plag_cat_frac'] + cat_frac_anhyd['K_Plag_cat_frac'])
-    cat_frac_anhyd['Or_Plag'] = 1 - cat_frac_anhyd['An_Plag'] - cat_frac_anhyd['Ab_Plag']
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
+    cat_frac_anhyd["An_Plag"] = cat_frac_anhyd["Ca_Plag_cat_frac"] / (
+        cat_frac_anhyd["Ca_Plag_cat_frac"]
+        + cat_frac_anhyd["Na_Plag_cat_frac"]
+        + cat_frac_anhyd["K_Plag_cat_frac"]
+    )
+    cat_frac_anhyd["Ab_Plag"] = cat_frac_anhyd["Na_Plag_cat_frac"] / (
+        cat_frac_anhyd["Ca_Plag_cat_frac"]
+        + cat_frac_anhyd["Na_Plag_cat_frac"]
+        + cat_frac_anhyd["K_Plag_cat_frac"]
+    )
+    cat_frac_anhyd["Or_Plag"] = (
+        1 - cat_frac_anhyd["An_Plag"] - cat_frac_anhyd["Ab_Plag"]
+    )
     cat_frac_anhyd2 = pd.concat([plag_comps, cat_prop, cat_frac_anhyd], axis=1)
     return cat_frac_anhyd2
 
 
-
-
 def calculate_oxygens_plagioclase(plag_comps):
-    
     """
-    
-    Import plagioclase compositions using plag_comps=My_Plags, returns number of oxygens 
+
+    Import plagioclase compositions using plag_comps=My_Plags, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
-    
+
     Parameters
     -------
     plag_comps: pandas.DataFrame
         plagioclase compositions with column headings SiO2_Plag, MgO_Plag etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Plag_ox
 
     """
 
-    oxygen_num_plag = {'SiO2_Plag': 2, 'MgO_Plag': 1, 'FeOt_Plag': 1, 'CaO_Plag': 1, 'Al2O3_Plag': 3, 'Na2O_Plag': 1, 'K2O_Plag': 1, 'MnO_Plag': 1, 'TiO2_Plag': 2, 'Cr2O3_Plag': 3, 'P2O5_Plag': 5}
-    oxygen_num_plag_df = pd.DataFrame.from_dict(oxygen_num_plag, orient='index').T
-    oxygen_num_plag_df['Sample_ID_Plag'] = 'OxNum'
-    oxygen_num_plag_df.set_index('Sample_ID_Plag', inplace=True)
+    oxygen_num_plag = {
+        "SiO2_Plag": 2,
+        "MgO_Plag": 1,
+        "FeOt_Plag": 1,
+        "CaO_Plag": 1,
+        "Al2O3_Plag": 3,
+        "Na2O_Plag": 1,
+        "K2O_Plag": 1,
+        "MnO_Plag": 1,
+        "TiO2_Plag": 2,
+        "Cr2O3_Plag": 3,
+        "P2O5_Plag": 5,
+    }
+    oxygen_num_plag_df = pd.DataFrame.from_dict(oxygen_num_plag, orient="index").T
+    oxygen_num_plag_df["Sample_ID_Plag"] = "OxNum"
+    oxygen_num_plag_df.set_index("Sample_ID_Plag", inplace=True)
 
     mol_prop = calculate_mol_proportions_plagioclase(plag_comps=plag_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
-    ox_num_reindex = oxygen_num_plag_df.reindex(
-        mol_prop.columns, axis=1).fillna(0)
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
+    ox_num_reindex = oxygen_num_plag_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
     oxygens_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
+
 def calculate_8oxygens_plagioclase(plag_comps):
-    
     """
-    
+
     Import plagioclase compositions using plag_comps=My_Plags, returns cations on the basis of 8 oxygens.
 
     Parameters
     -------
     plag_comps: pandas.DataFrame
         plagioclase compositions with column headings SiO2_Plag, MgO_Plag etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 8 oxygens, with column headings of the form... Plag_cat_8ox.
 
     """
-    cation_num_plag = {'SiO2_Plag': 1, 'MgO_Plag': 1, 'FeOt_Plag': 1, 'CaO_Plag': 1, 'Al2O3_Plag': 2, 'Na2O_Plag': 2, 'K2O_Plag': 2, 'MnO_Plag': 1, 'TiO2_Plag': 1, 'Cr2O3_Plag': 2, 'P2O5_Plag': 2}
-
-    cation_num_plag_df = pd.DataFrame.from_dict(cation_num_plag, orient='index').T
-    cation_num_plag_df['Sample_ID_Plag'] = 'CatNum'
-    cation_num_plag_df.set_index('Sample_ID_Plag', inplace=True)
+    cation_num_plag = {
+        "SiO2_Plag": 1,
+        "MgO_Plag": 1,
+        "FeOt_Plag": 1,
+        "CaO_Plag": 1,
+        "Al2O3_Plag": 2,
+        "Na2O_Plag": 2,
+        "K2O_Plag": 2,
+        "MnO_Plag": 1,
+        "TiO2_Plag": 1,
+        "Cr2O3_Plag": 2,
+        "P2O5_Plag": 2,
+    }
+
+    cation_num_plag_df = pd.DataFrame.from_dict(cation_num_plag, orient="index").T
+    cation_num_plag_df["Sample_ID_Plag"] = "CatNum"
+    cation_num_plag_df.set_index("Sample_ID_Plag", inplace=True)
 
     oxygens = calculate_oxygens_plagioclase(plag_comps=plag_comps)
-    renorm_factor = 8 / (oxygens.sum(axis='columns'))
+    renorm_factor = 8 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_plagioclase(plag_comps=plag_comps)
-    mol_prop['oxy_renorm_factor_plag'] = renorm_factor
-    mol_prop_8 = mol_prop.multiply(mol_prop['oxy_renorm_factor_plag'], axis='rows')
-    mol_prop_8.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_8.columns]
+    mol_prop["oxy_renorm_factor_plag"] = renorm_factor
+    mol_prop_8 = mol_prop.multiply(mol_prop["oxy_renorm_factor_plag"], axis="rows")
+    mol_prop_8.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_8.columns
+    ]
 
-    ox_num_reindex = cation_num_plag_df.reindex(
-        mol_prop_8.columns, axis=1).fillna(0)
+    ox_num_reindex = cation_num_plag_df.reindex(mol_prop_8.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_8])
     cation_8 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_8.columns = [str(col).replace('_mol_prop', '_cat_8ox')
-                        for col in mol_prop.columns]
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_8_2=cation_8.rename(columns={
-                            'SiO2_Plag_cat_8ox': 'Si_Plag_cat_8ox',
-                            'TiO2_Plag_cat_8ox': 'Ti_Plag_cat_8ox',
-                            'Al2O3_Plag_cat_8ox': 'Al_Plag_cat_8ox',
-                            'FeOt_Plag_cat_8ox': 'Fet_Plag_cat_8ox',
-                            'MnO_Plag_cat_8ox': 'Mn_Plag_cat_8ox',
-                            'MgO_Plag_cat_8ox': 'Mg_Plag_cat_8ox',
-                            'CaO_Plag_cat_8ox': 'Ca_Plag_cat_8ox',
-                            'Na2O_Plag_cat_8ox': 'Na_Plag_cat_8ox',
-                            'K2O_Plag_cat_8ox': 'K_Plag_cat_8ox',
-                            'Cr2O3_Plag_cat_8ox': 'Cr_Plag_cat_8ox',
-                            'P2O5_Plag_cat_8ox': 'P_Plag_cat_8ox',})
+    cation_8.columns = [
+        str(col).replace("_mol_prop", "_cat_8ox") for col in mol_prop.columns
+    ]
+
+    cation_8_2 = cation_8.rename(
+        columns={
+            "SiO2_Plag_cat_8ox": "Si_Plag_cat_8ox",
+            "TiO2_Plag_cat_8ox": "Ti_Plag_cat_8ox",
+            "Al2O3_Plag_cat_8ox": "Al_Plag_cat_8ox",
+            "FeOt_Plag_cat_8ox": "Fet_Plag_cat_8ox",
+            "MnO_Plag_cat_8ox": "Mn_Plag_cat_8ox",
+            "MgO_Plag_cat_8ox": "Mg_Plag_cat_8ox",
+            "CaO_Plag_cat_8ox": "Ca_Plag_cat_8ox",
+            "Na2O_Plag_cat_8ox": "Na_Plag_cat_8ox",
+            "K2O_Plag_cat_8ox": "K_Plag_cat_8ox",
+            "Cr2O3_Plag_cat_8ox": "Cr_Plag_cat_8ox",
+            "P2O5_Plag_cat_8ox": "P_Plag_cat_8ox",
+        }
+    )
 
     return cation_8_2
 
-def calculate_plagioclase_components(plag_comps, append):
 
+def calculate_plagioclase_components(plag_comps, append):
     """
-    
+
     Import plagioclase compositions using plag_comps=My_Plags, returns components on the basis of 8 oxygens.
 
     Parameters
     -------
     plag_comps: pandas.DataFrame
         plagioclase compositions with column headings SiO2_Plag, MgO_Plag etc.
 
@@ -857,128 +1081,165 @@
     -------
     pandas DataFrame
         cations on the basis of 8 oxygens, with column headings of the form... Plag_cat_8ox.
 
     """
 
     plag_comps_new = plag_comps.copy()
-    plag_comps_new.columns = [col.replace(append, '_Plag') for col in plag_comps_new.columns]
+    plag_comps_new.columns = [
+        col.replace(append, "_Plag") for col in plag_comps_new.columns
+    ]
     plag_comps = plag_comps_new.copy()
 
     plag_calc = calculate_8oxygens_plagioclase(plag_comps=plag_comps)
-    plag_calc['Plag_Cation_Sum'] = (plag_calc['Si_Plag_cat_8ox']+plag_calc['Ti_Plag_cat_8ox']
-    +plag_calc['Al_Plag_cat_8ox']+plag_calc['Fet_Plag_cat_8ox']+plag_calc['Mn_Plag_cat_8ox']
-    +plag_calc['Mg_Plag_cat_8ox']+plag_calc['Ca_Plag_cat_8ox']+plag_calc['Na_Plag_cat_8ox']
-    +plag_calc['K_Plag_cat_8ox']+plag_calc['Cr_Plag_cat_8ox'])
+    plag_calc["Plag_Cation_Sum"] = (
+        plag_calc["Si_Plag_cat_8ox"]
+        + plag_calc["Ti_Plag_cat_8ox"]
+        + plag_calc["Al_Plag_cat_8ox"]
+        + plag_calc["Fet_Plag_cat_8ox"]
+        + plag_calc["Mn_Plag_cat_8ox"]
+        + plag_calc["Mg_Plag_cat_8ox"]
+        + plag_calc["Ca_Plag_cat_8ox"]
+        + plag_calc["Na_Plag_cat_8ox"]
+        + plag_calc["K_Plag_cat_8ox"]
+        + plag_calc["Cr_Plag_cat_8ox"]
+    )
 
     # M site
-    plag_calc['Na_Ca_M_Plag'] = plag_calc['Na_Plag_cat_8ox'] + plag_calc['Ca_Plag_cat_8ox']
+    plag_calc["Na_Ca_M_Plag"] = (
+        plag_calc["Na_Plag_cat_8ox"] + plag_calc["Ca_Plag_cat_8ox"]
+    )
     # T site
-    plag_calc['Si_Al_T_Plag'] = plag_calc['Si_Plag_cat_8ox'] + plag_calc['Al_Plag_cat_8ox']
+    plag_calc["Si_Al_T_Plag"] = (
+        plag_calc["Si_Plag_cat_8ox"] + plag_calc["Al_Plag_cat_8ox"]
+    )
 
     cat_prop = calculate_cat_proportions_plagioclase(plag_comps=plag_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
-    cat_frac_anhyd['An_Plag'] = cat_frac_anhyd['Ca_Plag_cat_frac'] / \
-        (cat_frac_anhyd['Ca_Plag_cat_frac'] +
-         cat_frac_anhyd['Na_Plag_cat_frac'] + cat_frac_anhyd['K_Plag_cat_frac'])
-    cat_frac_anhyd['Ab_Plag'] = cat_frac_anhyd['Na_Plag_cat_frac'] / \
-        (cat_frac_anhyd['Ca_Plag_cat_frac'] +
-         cat_frac_anhyd['Na_Plag_cat_frac'] + cat_frac_anhyd['K_Plag_cat_frac'])
-    cat_frac_anhyd['Or_Plag'] = 1 - \
-        cat_frac_anhyd['An_Plag'] - cat_frac_anhyd['Ab_Plag']
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
+    cat_frac_anhyd["An_Plag"] = cat_frac_anhyd["Ca_Plag_cat_frac"] / (
+        cat_frac_anhyd["Ca_Plag_cat_frac"]
+        + cat_frac_anhyd["Na_Plag_cat_frac"]
+        + cat_frac_anhyd["K_Plag_cat_frac"]
+    )
+    cat_frac_anhyd["Ab_Plag"] = cat_frac_anhyd["Na_Plag_cat_frac"] / (
+        cat_frac_anhyd["Ca_Plag_cat_frac"]
+        + cat_frac_anhyd["Na_Plag_cat_frac"]
+        + cat_frac_anhyd["K_Plag_cat_frac"]
+    )
+    cat_frac_anhyd["Or_Plag"] = (
+        1 - cat_frac_anhyd["An_Plag"] - cat_frac_anhyd["Ab_Plag"]
+    )
     cat_frac_anhyd2 = pd.concat([plag_comps, plag_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-# %% CLINOPYROXENE 
-
+# %% CLINOPYROXENE
 
 
 def calculate_mol_proportions_clinopyroxene(cpx_comps):
-    
     """
-    
+
     Import clinopyroxene compositions using cpx_comps=My_Cpxs, returns mole proportions
 
     Parameters
     -------
     cpx_comps: pandas.DataFrame
         clinopyroxene compositions with column headings SiO2_Cpx, MgO_Cpx etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for clinopyroxene with column headings of the form SiO2_Cpx_mol_prop
 
     """
 
-    oxide_mass_cpx = {'SiO2_Cpx': 60.0843, 'MgO_Cpx': 40.3044, 'FeOt_Cpx': 71.8464, 'CaO_Cpx': 56.0774, 'Al2O3_Cpx': 101.961, 'Na2O_Cpx': 61.9789, 'K2O_Cpx': 94.196, 'MnO_Cpx': 70.9375, 'TiO2_Cpx': 79.8788, 'Cr2O3_Cpx': 151.9982}
-
-    oxide_mass_cpx_df = pd.DataFrame.from_dict(oxide_mass_cpx, orient='index').T
-    oxide_mass_cpx_df['Sample_ID_Cpx'] = 'MolWt'
-    oxide_mass_cpx_df.set_index('Sample_ID_Cpx', inplace=True)
+    oxide_mass_cpx = {
+        "SiO2_Cpx": 60.0843,
+        "MgO_Cpx": 40.3044,
+        "FeOt_Cpx": 71.8464,
+        "CaO_Cpx": 56.0774,
+        "Al2O3_Cpx": 101.961,
+        "Na2O_Cpx": 61.9789,
+        "K2O_Cpx": 94.196,
+        "MnO_Cpx": 70.9375,
+        "TiO2_Cpx": 79.8788,
+        "Cr2O3_Cpx": 151.9982,
+    }
+
+    oxide_mass_cpx_df = pd.DataFrame.from_dict(oxide_mass_cpx, orient="index").T
+    oxide_mass_cpx_df["Sample_ID_Cpx"] = "MolWt"
+    oxide_mass_cpx_df.set_index("Sample_ID_Cpx", inplace=True)
 
     # This makes the input match the columns in the oxide mass dataframe
     cpx_wt = cpx_comps.reindex(oxide_mass_cpx_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    cpx_wt_combo = pd.concat([oxide_mass_cpx_df, cpx_wt],)
+    cpx_wt_combo = pd.concat(
+        [oxide_mass_cpx_df, cpx_wt],
+    )
     # Drop the calculation column
     mol_prop_anhyd = cpx_wt_combo.div(
-        cpx_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+        cpx_wt_combo.loc["MolWt", :], axis="columns"
+    ).drop(["MolWt"])
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
 
-
 def calculate_oxygens_clinopyroxene(cpx_comps):
-    
     """
-    
+
     Import clinopyroxene compositions using cpx_comps=My_Cpxs, returns number of oxygens (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     cpx_comps: pandas.DataFrame
         clinopyroxene compositions with column headings SiO2_Cpx, MgO_Cpx etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Cpx_ox
 
     """
-    
-    oxygen_num_cpx = {'SiO2_Cpx': 2, 'MgO_Cpx': 1, 'FeOt_Cpx': 1, 'CaO_Cpx': 1, 'Al2O3_Cpx': 3, 'Na2O_Cpx': 1, 'K2O_Cpx': 1, 'MnO_Cpx': 1, 'TiO2_Cpx': 2, 'Cr2O3_Cpx': 3}
-    oxygen_num_cpx_df = pd.DataFrame.from_dict(oxygen_num_cpx, orient='index').T
-    oxygen_num_cpx_df['Sample_ID_Cpx'] = 'OxNum'
-    oxygen_num_cpx_df.set_index('Sample_ID_Cpx', inplace=True)
+
+    oxygen_num_cpx = {
+        "SiO2_Cpx": 2,
+        "MgO_Cpx": 1,
+        "FeOt_Cpx": 1,
+        "CaO_Cpx": 1,
+        "Al2O3_Cpx": 3,
+        "Na2O_Cpx": 1,
+        "K2O_Cpx": 1,
+        "MnO_Cpx": 1,
+        "TiO2_Cpx": 2,
+        "Cr2O3_Cpx": 3,
+    }
+    oxygen_num_cpx_df = pd.DataFrame.from_dict(oxygen_num_cpx, orient="index").T
+    oxygen_num_cpx_df["Sample_ID_Cpx"] = "OxNum"
+    oxygen_num_cpx_df.set_index("Sample_ID_Cpx", inplace=True)
 
     mol_prop = calculate_mol_proportions_clinopyroxene(cpx_comps=cpx_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
-    ox_num_reindex = oxygen_num_cpx_df.reindex(
-        mol_prop.columns, axis=1).fillna(0)
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
+    ox_num_reindex = oxygen_num_cpx_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
     oxygens_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
     return oxygens_anhyd
 
 
-
 def calculate_6oxygens_clinopyroxene(cpx_comps):
-    
     """
-    
+
     Import clinopyroxene compositions using cpx_comps=My_Cpxs, returns cations on the basis of 6 oxygens.
 
     Parameters
     -------
     cpx_comps: pandas.DataFrame
         clinopyroxene compositions with column headings SiO2_Cpx, MgO_Cpx etc.
 
@@ -986,69 +1247,93 @@
     Returns
     -------
     pandas DataFrame
         cations on the basis of 6 oxygens, with column headings of the form ...Cpx_cat_6ox.
 
     """
 
-    cation_num_cpx = {'SiO2_Cpx': 1, 'MgO_Cpx': 1, 'FeOt_Cpx': 1, 'CaO_Cpx': 1, 'Al2O3_Cpx': 2, 'Na2O_Cpx': 2, 'K2O_Cpx': 2, 'MnO_Cpx': 1,'TiO2_Cpx': 1, 'Cr2O3_Cpx': 2}
-    cation_num_cpx_df = pd.DataFrame.from_dict(cation_num_cpx, orient='index').T
-    cation_num_cpx_df['Sample_ID_Cpx'] = 'CatNum'
-    cation_num_cpx_df.set_index('Sample_ID_Cpx', inplace=True)
+    cation_num_cpx = {
+        "SiO2_Cpx": 1,
+        "MgO_Cpx": 1,
+        "FeOt_Cpx": 1,
+        "CaO_Cpx": 1,
+        "Al2O3_Cpx": 2,
+        "Na2O_Cpx": 2,
+        "K2O_Cpx": 2,
+        "MnO_Cpx": 1,
+        "TiO2_Cpx": 1,
+        "Cr2O3_Cpx": 2,
+    }
+    cation_num_cpx_df = pd.DataFrame.from_dict(cation_num_cpx, orient="index").T
+    cation_num_cpx_df["Sample_ID_Cpx"] = "CatNum"
+    cation_num_cpx_df.set_index("Sample_ID_Cpx", inplace=True)
 
     oxygens = calculate_oxygens_clinopyroxene(cpx_comps=cpx_comps)
-    renorm_factor = 6 / (oxygens.sum(axis='columns'))
+    renorm_factor = 6 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_clinopyroxene(cpx_comps=cpx_comps)
-    mol_prop['oxy_renorm_factor'] = renorm_factor
-    mol_prop_6 = mol_prop.multiply(mol_prop['oxy_renorm_factor'], axis='rows')
-    mol_prop_6.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_6.columns]
+    mol_prop["oxy_renorm_factor"] = renorm_factor
+    mol_prop_6 = mol_prop.multiply(mol_prop["oxy_renorm_factor"], axis="rows")
+    mol_prop_6.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_6.columns
+    ]
 
-    ox_num_reindex = cation_num_cpx_df.reindex(
-        mol_prop_6.columns, axis=1).fillna(0)
+    ox_num_reindex = cation_num_cpx_df.reindex(mol_prop_6.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_6])
     cation_6 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_6.columns = [str(col).replace('_mol_prop', '_cat_6ox')
-                        for col in mol_prop.columns]
-    cation_6['Al_IV_cat_6ox'] = 2 - cation_6['SiO2_Cpx_cat_6ox']
-    cation_6['Al_VI_cat_6ox'] = cation_6['Al2O3_Cpx_cat_6ox'] - \
-        cation_6['Al_IV_cat_6ox']
+    cation_6.columns = [
+        str(col).replace("_mol_prop", "_cat_6ox") for col in mol_prop.columns
+    ]
+    cation_6["Al_IV_cat_6ox"] = 2 - cation_6["SiO2_Cpx_cat_6ox"]
+    cation_6["Al_VI_cat_6ox"] = (
+        cation_6["Al2O3_Cpx_cat_6ox"] - cation_6["Al_IV_cat_6ox"]
+    )
     cation_6.Al_VI_cat_6ox[cation_6.Al_VI_cat_6ox < 0] = 0
 
-    cation_6_2=cation_6.rename(columns={
-                        'SiO2_Cpx_cat_6ox': 'Si_Cpx_cat_6ox',
-                        'TiO2_Cpx_cat_6ox': 'Ti_Cpx_cat_6ox',
-                        'Al2O3_Cpx_cat_6ox': 'Al_Cpx_cat_6ox',
-                        'FeOt_Cpx_cat_6ox': 'Fet_Cpx_cat_6ox',
-                        'MnO_Cpx_cat_6ox': 'Mn_Cpx_cat_6ox',
-                        'MgO_Cpx_cat_6ox': 'Mg_Cpx_cat_6ox',
-                        'CaO_Cpx_cat_6ox': 'Ca_Cpx_cat_6ox',
-                        'Na2O_Cpx_cat_6ox': 'Na_Cpx_cat_6ox',
-                        'K2O_Cpx_cat_6ox': 'K_Cpx_cat_6ox',
-                        'Cr2O3_Cpx_cat_6ox': 'Cr_Cpx_cat_6ox',
-                        'P2O5_Cpx_cat_6ox': 'P_Cpx_cat_6ox_frac',
-                        })
-
-    cation_6_2['En_Simple_MgFeCa_Cpx']=(cation_6_2['Mg_Cpx_cat_6ox']/(cation_6_2['Mg_Cpx_cat_6ox']
-    +cation_6_2['Fet_Cpx_cat_6ox']+cation_6_2['Ca_Cpx_cat_6ox']))
-
-    cation_6_2['Fs_Simple_MgFeCa_Cpx']=(cation_6_2['Fet_Cpx_cat_6ox']/(cation_6_2['Mg_Cpx_cat_6ox']
-    +cation_6_2['Fet_Cpx_cat_6ox']+cation_6_2['Ca_Cpx_cat_6ox']))
-
-    cation_6_2['Wo_Simple_MgFeCa_Cpx']=(cation_6_2['Ca_Cpx_cat_6ox']/(cation_6_2['Mg_Cpx_cat_6ox']
-    +cation_6_2['Fet_Cpx_cat_6ox']+cation_6_2['Ca_Cpx_cat_6ox']))
+    cation_6_2 = cation_6.rename(
+        columns={
+            "SiO2_Cpx_cat_6ox": "Si_Cpx_cat_6ox",
+            "TiO2_Cpx_cat_6ox": "Ti_Cpx_cat_6ox",
+            "Al2O3_Cpx_cat_6ox": "Al_Cpx_cat_6ox",
+            "FeOt_Cpx_cat_6ox": "Fet_Cpx_cat_6ox",
+            "MnO_Cpx_cat_6ox": "Mn_Cpx_cat_6ox",
+            "MgO_Cpx_cat_6ox": "Mg_Cpx_cat_6ox",
+            "CaO_Cpx_cat_6ox": "Ca_Cpx_cat_6ox",
+            "Na2O_Cpx_cat_6ox": "Na_Cpx_cat_6ox",
+            "K2O_Cpx_cat_6ox": "K_Cpx_cat_6ox",
+            "Cr2O3_Cpx_cat_6ox": "Cr_Cpx_cat_6ox",
+            "P2O5_Cpx_cat_6ox": "P_Cpx_cat_6ox_frac",
+        }
+    )
+
+    cation_6_2["En_Simple_MgFeCa_Cpx"] = cation_6_2["Mg_Cpx_cat_6ox"] / (
+        cation_6_2["Mg_Cpx_cat_6ox"]
+        + cation_6_2["Fet_Cpx_cat_6ox"]
+        + cation_6_2["Ca_Cpx_cat_6ox"]
+    )
+
+    cation_6_2["Fs_Simple_MgFeCa_Cpx"] = cation_6_2["Fet_Cpx_cat_6ox"] / (
+        cation_6_2["Mg_Cpx_cat_6ox"]
+        + cation_6_2["Fet_Cpx_cat_6ox"]
+        + cation_6_2["Ca_Cpx_cat_6ox"]
+    )
+
+    cation_6_2["Wo_Simple_MgFeCa_Cpx"] = cation_6_2["Ca_Cpx_cat_6ox"] / (
+        cation_6_2["Mg_Cpx_cat_6ox"]
+        + cation_6_2["Fet_Cpx_cat_6ox"]
+        + cation_6_2["Ca_Cpx_cat_6ox"]
+    )
     return cation_6_2
 
 
 def calculate_clinopyroxene_components(cpx_comps):
-    
     """
-    
+
     Import clinopyroxene compositions using cpx_comps=My_Cpxs, returns clinopyroxene components along with entered Cpx compositions
 
     Parameters
     -------
 
     cpx_comps: pandas.DataFrame
         clinopyroxene compositions with column headings SiO2_Cpx, MgO_Cpx etc.
@@ -1059,257 +1344,402 @@
         Clinopyroxene components (column headings: Cation_Sum, CrCaTs, a_cpx_En, Mgno_Cpx, Jd, CaTs, CaTi, DiHd_1996, DiHd_2003, En_Fs), cations on bases of 6 oxygens (column headings of form  Cr2O3_Cpx_cat_6ox), as well as inputted Cpx compositions (column headings of form MgO_Cpx)
 
     """
     cpx_calc = calculate_6oxygens_clinopyroxene(cpx_comps=cpx_comps)
 
     # Sum of cations, used by Neave and Putirka (2017) to filter out bad
     # clinopyroxene analyses
-    cpx_calc['Cpx_Cation_Sum'] = (cpx_calc['Si_Cpx_cat_6ox'] + cpx_calc['Ti_Cpx_cat_6ox'] + cpx_calc['Al_Cpx_cat_6ox'] + cpx_calc['Fet_Cpx_cat_6ox'] + cpx_calc['Mn_Cpx_cat_6ox'] + cpx_calc['Mg_Cpx_cat_6ox'] + cpx_calc['Ca_Cpx_cat_6ox'] + cpx_calc['Na_Cpx_cat_6ox'] + cpx_calc['K_Cpx_cat_6ox'] + cpx_calc['Cr_Cpx_cat_6ox'])
-
-    cpx_calc['Ca_CaMgFe_Cpx']=cpx_calc['Ca_Cpx_cat_6ox']/(cpx_calc['Ca_Cpx_cat_6ox']+cpx_calc['Fet_Cpx_cat_6ox'] +cpx_calc['Mg_Cpx_cat_6ox'])
-
-
-    cpx_calc['Lindley_Fe3_Cpx'] = (cpx_calc['Na_Cpx_cat_6ox'] + cpx_calc['Al_IV_cat_6ox'] - cpx_calc['Al_VI_cat_6ox'] - 2 * cpx_calc['Ti_Cpx_cat_6ox'] - cpx_calc['Cr_Cpx_cat_6ox'])  # This is cell FR
-    cpx_calc.loc[(cpx_calc['Lindley_Fe3_Cpx'] < 0.0000000001),  'Lindley_Fe3_Cpx'] = 0
-    cpx_calc.loc[(cpx_calc['Lindley_Fe3_Cpx'] >= cpx_calc['Fet_Cpx_cat_6ox'] ),  'Lindley_Fe3_Cpx'] = (cpx_calc['Fet_Cpx_cat_6ox'])
-    cpx_calc['Lindley_Fe2_Cpx']=cpx_calc['Fet_Cpx_cat_6ox']-cpx_calc['Lindley_Fe3_Cpx']
-    cpx_calc['Lindley_Fe3_Cpx_prop']=cpx_calc['Lindley_Fe3_Cpx']/cpx_calc['Fet_Cpx_cat_6ox']
+    cpx_calc["Cpx_Cation_Sum"] = (
+        cpx_calc["Si_Cpx_cat_6ox"]
+        + cpx_calc["Ti_Cpx_cat_6ox"]
+        + cpx_calc["Al_Cpx_cat_6ox"]
+        + cpx_calc["Fet_Cpx_cat_6ox"]
+        + cpx_calc["Mn_Cpx_cat_6ox"]
+        + cpx_calc["Mg_Cpx_cat_6ox"]
+        + cpx_calc["Ca_Cpx_cat_6ox"]
+        + cpx_calc["Na_Cpx_cat_6ox"]
+        + cpx_calc["K_Cpx_cat_6ox"]
+        + cpx_calc["Cr_Cpx_cat_6ox"]
+    )
+
+    cpx_calc["Ca_CaMgFe_Cpx"] = cpx_calc["Ca_Cpx_cat_6ox"] / (
+        cpx_calc["Ca_Cpx_cat_6ox"]
+        + cpx_calc["Fet_Cpx_cat_6ox"]
+        + cpx_calc["Mg_Cpx_cat_6ox"]
+    )
+
+    cpx_calc["Lindley_Fe3_Cpx"] = (
+        cpx_calc["Na_Cpx_cat_6ox"]
+        + cpx_calc["Al_IV_cat_6ox"]
+        - cpx_calc["Al_VI_cat_6ox"]
+        - 2 * cpx_calc["Ti_Cpx_cat_6ox"]
+        - cpx_calc["Cr_Cpx_cat_6ox"]
+    )  # This is cell FR
+    cpx_calc.loc[(cpx_calc["Lindley_Fe3_Cpx"] < 0.0000000001), "Lindley_Fe3_Cpx"] = 0
+    cpx_calc.loc[
+        (cpx_calc["Lindley_Fe3_Cpx"] >= cpx_calc["Fet_Cpx_cat_6ox"]), "Lindley_Fe3_Cpx"
+    ] = cpx_calc["Fet_Cpx_cat_6ox"]
+    cpx_calc["Lindley_Fe2_Cpx"] = (
+        cpx_calc["Fet_Cpx_cat_6ox"] - cpx_calc["Lindley_Fe3_Cpx"]
+    )
+    cpx_calc["Lindley_Fe3_Cpx_prop"] = (
+        cpx_calc["Lindley_Fe3_Cpx"] / cpx_calc["Fet_Cpx_cat_6ox"]
+    )
 
     # Cpx Components that don't nee if and else statements and don't rely on
     # others.
-    cpx_calc['CrCaTs_Cpx'] = 0.5 * cpx_calc['Cr_Cpx_cat_6ox']
-    cpx_calc['a_cpx_En'] = ((1 - cpx_calc['Ca_Cpx_cat_6ox'] - cpx_calc['Na_Cpx_cat_6ox'] - cpx_calc['K_Cpx_cat_6ox']) * (1 - 0.5 * (cpx_calc['Al_Cpx_cat_6ox']+ cpx_calc['Cr_Cpx_cat_6ox'] + cpx_calc['Na_Cpx_cat_6ox'] + cpx_calc['K_Cpx_cat_6ox'])))
-    cpx_calc['Mgno_Cpx'] = (cpx_comps['MgO_Cpx'] / 40.3044) / (cpx_comps['MgO_Cpx'] / 40.3044 + cpx_comps['FeOt_Cpx'] / 71.844)
-
-    AlVI_minus_Na = cpx_calc['Al_VI_cat_6ox']-cpx_calc['Na_Cpx_cat_6ox']
-    cpx_calc['Jd_Cpx'] = cpx_calc['Na_Cpx_cat_6ox']
-    cpx_calc['Jd_from 0=Na, 1=Al'] = 0
-    cpx_calc['CaTs_Cpx'] = cpx_calc['Al_VI_cat_6ox'] -cpx_calc['Na_Cpx_cat_6ox']
+    cpx_calc["CrCaTs_Cpx"] = 0.5 * cpx_calc["Cr_Cpx_cat_6ox"]
+    cpx_calc["a_cpx_En"] = (
+        1
+        - cpx_calc["Ca_Cpx_cat_6ox"]
+        - cpx_calc["Na_Cpx_cat_6ox"]
+        - cpx_calc["K_Cpx_cat_6ox"]
+    ) * (
+        1
+        - 0.5
+        * (
+            cpx_calc["Al_Cpx_cat_6ox"]
+            + cpx_calc["Cr_Cpx_cat_6ox"]
+            + cpx_calc["Na_Cpx_cat_6ox"]
+            + cpx_calc["K_Cpx_cat_6ox"]
+        )
+    )
+    cpx_calc["Mgno_Cpx"] = (cpx_comps["MgO_Cpx"] / 40.3044) / (
+        cpx_comps["MgO_Cpx"] / 40.3044 + cpx_comps["FeOt_Cpx"] / 71.844
+    )
+
+    AlVI_minus_Na = cpx_calc["Al_VI_cat_6ox"] - cpx_calc["Na_Cpx_cat_6ox"]
+    cpx_calc["Jd_Cpx"] = cpx_calc["Na_Cpx_cat_6ox"]
+    cpx_calc["Jd_from 0=Na, 1=Al"] = 0
+    cpx_calc["CaTs_Cpx"] = cpx_calc["Al_VI_cat_6ox"] - cpx_calc["Na_Cpx_cat_6ox"]
 
     # If value of AlVI<Na cat frac
-    cpx_calc.loc[(AlVI_minus_Na<0), 'Jd_from 0=Na, 1=Al']=1
-    cpx_calc.loc[(AlVI_minus_Na<0), 'Jd_Cpx']=cpx_calc['Al_VI_cat_6ox']
-    cpx_calc.loc[(AlVI_minus_Na<0), 'CaTs_Cpx']=0
+    cpx_calc.loc[(AlVI_minus_Na < 0), "Jd_from 0=Na, 1=Al"] = 1
+    cpx_calc.loc[(AlVI_minus_Na < 0), "Jd_Cpx"] = cpx_calc["Al_VI_cat_6ox"]
+    cpx_calc.loc[(AlVI_minus_Na < 0), "CaTs_Cpx"] = 0
 
     # If value of AlIV>CaTs
-    AlVI_minus_CaTs = cpx_calc['Al_IV_cat_6ox']-cpx_calc['CaTs_Cpx']
-    #default, if is bigger
-    cpx_calc['CaTi_Cpx'] = (cpx_calc['Al_IV_cat_6ox'] - cpx_calc['CaTs_Cpx']) / 2
-    cpx_calc.loc[(AlVI_minus_CaTs<0), 'CaTi_Cpx'] = 0
+    AlVI_minus_CaTs = cpx_calc["Al_IV_cat_6ox"] - cpx_calc["CaTs_Cpx"]
+    # default, if is bigger
+    cpx_calc["CaTi_Cpx"] = (cpx_calc["Al_IV_cat_6ox"] - cpx_calc["CaTs_Cpx"]) / 2
+    cpx_calc.loc[(AlVI_minus_CaTs < 0), "CaTi_Cpx"] = 0
 
     #  If CaO-CaTs-CaTi-CrCaTs is >0
-    Ca_CaTs_CaTi_CrCaTs=(cpx_calc['Ca_Cpx_cat_6ox'] - cpx_calc['CaTs_Cpx'] - cpx_calc['CaTi_Cpx'] - cpx_calc['CrCaTs_Cpx'])
-
-    cpx_calc['DiHd_Cpx_1996']= (cpx_calc['Ca_Cpx_cat_6ox'] - cpx_calc['CaTs_Cpx'] - cpx_calc['CaTi_Cpx'] - cpx_calc['CrCaTs_Cpx'] )
-    cpx_calc.loc[(Ca_CaTs_CaTi_CrCaTs<0), 'DiHd_Cpx_1996']=0
-
-    cpx_calc['EnFs_Cpx'] = ((cpx_calc['Fet_Cpx_cat_6ox'] + cpx_calc['Mg_Cpx_cat_6ox']) - cpx_calc['DiHd_Cpx_1996']) / 2
-    cpx_calc['DiHd_Cpx_2003'] = (cpx_calc['Ca_Cpx_cat_6ox'] - cpx_calc['CaTs_Cpx'] - cpx_calc['CaTi_Cpx'] - cpx_calc['CrCaTs_Cpx'])
-    cpx_calc['Di_Cpx'] = cpx_calc['DiHd_Cpx_2003'] * (cpx_calc['Mg_Cpx_cat_6ox'] / (cpx_calc['Mg_Cpx_cat_6ox'] + cpx_calc['Mn_Cpx_cat_6ox'] + cpx_calc['Fet_Cpx_cat_6ox']))
-    cpx_calc['DiHd_Cpx_1996'].clip(lower=0, inplace=True)
-    cpx_calc['DiHd_Cpx_2003'].clip(lower=0, inplace=True)
-    cpx_calc['Jd_Cpx'].clip(lower=0, inplace=True)
-
-    cpx_calc['FeIII_Wang21']=(cpx_calc['Na_Cpx_cat_6ox']+cpx_calc['Al_IV_cat_6ox']-cpx_calc['Al_VI_cat_6ox']-2*cpx_calc['Ti_Cpx_cat_6ox']-cpx_calc['Cr_Cpx_cat_6ox'])
-    cpx_calc['FeII_Wang21']=cpx_calc['Fet_Cpx_cat_6ox']-cpx_calc['FeIII_Wang21']
+    Ca_CaTs_CaTi_CrCaTs = (
+        cpx_calc["Ca_Cpx_cat_6ox"]
+        - cpx_calc["CaTs_Cpx"]
+        - cpx_calc["CaTi_Cpx"]
+        - cpx_calc["CrCaTs_Cpx"]
+    )
+
+    cpx_calc["DiHd_Cpx_1996"] = (
+        cpx_calc["Ca_Cpx_cat_6ox"]
+        - cpx_calc["CaTs_Cpx"]
+        - cpx_calc["CaTi_Cpx"]
+        - cpx_calc["CrCaTs_Cpx"]
+    )
+    cpx_calc.loc[(Ca_CaTs_CaTi_CrCaTs < 0), "DiHd_Cpx_1996"] = 0
+
+    cpx_calc["EnFs_Cpx"] = (
+        (cpx_calc["Fet_Cpx_cat_6ox"] + cpx_calc["Mg_Cpx_cat_6ox"])
+        - cpx_calc["DiHd_Cpx_1996"]
+    ) / 2
+    cpx_calc["DiHd_Cpx_2003"] = (
+        cpx_calc["Ca_Cpx_cat_6ox"]
+        - cpx_calc["CaTs_Cpx"]
+        - cpx_calc["CaTi_Cpx"]
+        - cpx_calc["CrCaTs_Cpx"]
+    )
+    cpx_calc["Di_Cpx"] = cpx_calc["DiHd_Cpx_2003"] * (
+        cpx_calc["Mg_Cpx_cat_6ox"]
+        / (
+            cpx_calc["Mg_Cpx_cat_6ox"]
+            + cpx_calc["Mn_Cpx_cat_6ox"]
+            + cpx_calc["Fet_Cpx_cat_6ox"]
+        )
+    )
+    cpx_calc["DiHd_Cpx_1996"].clip(lower=0, inplace=True)
+    cpx_calc["DiHd_Cpx_2003"].clip(lower=0, inplace=True)
+    cpx_calc["Jd_Cpx"].clip(lower=0, inplace=True)
+
+    cpx_calc["FeIII_Wang21"] = (
+        cpx_calc["Na_Cpx_cat_6ox"]
+        + cpx_calc["Al_IV_cat_6ox"]
+        - cpx_calc["Al_VI_cat_6ox"]
+        - 2 * cpx_calc["Ti_Cpx_cat_6ox"]
+        - cpx_calc["Cr_Cpx_cat_6ox"]
+    )
+    cpx_calc["FeII_Wang21"] = cpx_calc["Fet_Cpx_cat_6ox"] - cpx_calc["FeIII_Wang21"]
 
     # Merging new Cpx compnoents with inputted cpx composition
-    cpx_combined = pd.concat([cpx_comps, cpx_calc], axis='columns')
+    cpx_combined = pd.concat([cpx_comps, cpx_calc], axis="columns")
 
     return cpx_combined
 
 
 def calculate_clinopyroxene_liquid_components(
-        *, cpx_comps=None, liq_comps=None, meltmatch=None, Fe3Fet_Liq=None):
-    
-    
+    *, cpx_comps=None, liq_comps=None, meltmatch=None, Fe3Fet_Liq=None
+):
     """
     Import clinopyroxene compositions using cpx_comps=My_Cpxs and liquid compositions using liq_comps=My_Liquids,
         returns clinopyroxene and liquid components.
 
-    Parameters: 
+    Parameters:
         liq_comps (pandas.DataFrame): liquid compositions with column headings SiO2_Liq, MgO_Liq etc.
         cpx_comps (pandas.DataFrame): clinopyroxene compositions with column headings SiO2_Cpx, MgO_Cpx etc.
         meltmatch (pandas.DataFrame): merged clinopyroxene and liquid compositions used for melt matching
         Fe3Fet_Liq (int, float, pandas.Series): overwrites Fe3FeT ratio inliquid input
 
-    Returns: 
+    Returns:
 
-        combo_liq_cpxs (pandas.DataFrame): Merged dataframe of inputted liquids, liquid mole fractions, liquid 
-                                           cation fractions, inputted cpx compositions, cpx cations on 6 oxygen basis, 
+        combo_liq_cpxs (pandas.DataFrame): Merged dataframe of inputted liquids, liquid mole fractions, liquid
+                                           cation fractions, inputted cpx compositions, cpx cations on 6 oxygen basis,
                                            cpx components and cpx-liquid components.
     """
 
     # For when users enter a combined dataframe meltmatch=""
     if meltmatch is not None:
         combo_liq_cpxs = meltmatch
         if "Sample_ID_Cpx" in combo_liq_cpxs:
             combo_liq_cpxs = combo_liq_cpxs.drop(
-                ['Sample_ID_Cpx'], axis=1) #.astype('float64')
-        if  "Sample_ID_Liq" in combo_liq_cpxs:
+                ["Sample_ID_Cpx"], axis=1
+            )  # .astype('float64')
+        if "Sample_ID_Liq" in combo_liq_cpxs:
             combo_liq_cpxs = combo_liq_cpxs.drop(
-                ['Sample_ID_Liq'], axis=1)#.astype('float64')
+                ["Sample_ID_Liq"], axis=1
+            )  # .astype('float64')
 
     if liq_comps is not None and cpx_comps is not None:
-        liq_comps_c=liq_comps.copy()
+        liq_comps_c = liq_comps.copy()
         if Fe3Fet_Liq is not None:
-            liq_comps_c['Fe3Fet_Liq']=Fe3Fet_Liq
+            liq_comps_c["Fe3Fet_Liq"] = Fe3Fet_Liq
 
         if len(liq_comps) != len(cpx_comps):
             raise Exception(
-                "inputted dataframes for liq_comps and cpx_comps need to have the same number of rows")
+                "inputted dataframes for liq_comps and cpx_comps need to have the same number of rows"
+            )
         else:
             myCPXs1_comp = calculate_clinopyroxene_components(
-                cpx_comps=cpx_comps).reset_index(drop=True)
+                cpx_comps=cpx_comps
+            ).reset_index(drop=True)
             myLiquids1_comps = calculate_anhydrous_cat_fractions_liquid(
-                liq_comps=liq_comps_c).reset_index(drop=True)
-            combo_liq_cpxs = pd.concat(
-                [myLiquids1_comps, myCPXs1_comp], axis=1)
+                liq_comps=liq_comps_c
+            ).reset_index(drop=True)
+            combo_liq_cpxs = pd.concat([myLiquids1_comps, myCPXs1_comp], axis=1)
             if "Sample_ID_Cpx" in combo_liq_cpxs:
-                combo_liq_cpxs.drop(['Sample_ID_Cpx'], axis=1)
+                combo_liq_cpxs.drop(["Sample_ID_Cpx"], axis=1)
             if "Sample_ID_Liq" in combo_liq_cpxs:
-                combo_liq_cpxs.drop(['Sample_ID_Liq'], axis=1)
+                combo_liq_cpxs.drop(["Sample_ID_Liq"], axis=1)
 
     # Measured Kd Fe-Mg (using 2+)
-    combo_liq_cpxs['Kd_Fe_Mg_Fe2'] = ((combo_liq_cpxs['Fet_Cpx_cat_6ox'] / combo_liq_cpxs['Mg_Cpx_cat_6ox']) / ((combo_liq_cpxs['Fet_Liq_cat_frac'] * (1 - combo_liq_cpxs['Fe3Fet_Liq']) / combo_liq_cpxs['Mg_Liq_cat_frac'])))
+    combo_liq_cpxs["Kd_Fe_Mg_Fe2"] = (
+        combo_liq_cpxs["Fet_Cpx_cat_6ox"] / combo_liq_cpxs["Mg_Cpx_cat_6ox"]
+    ) / (
+        combo_liq_cpxs["Fet_Liq_cat_frac"]
+        * (1 - combo_liq_cpxs["Fe3Fet_Liq"])
+        / combo_liq_cpxs["Mg_Liq_cat_frac"]
+    )
 
     # Measured Kd Fe-Mg using 2+ in the liquid and Cpx based on Lindley
-    combo_liq_cpxs['Kd_Fe_Mg_Fe2_Lind'] = ((combo_liq_cpxs['Lindley_Fe2_Cpx'] / combo_liq_cpxs['Mg_Cpx_cat_6ox']) / ((combo_liq_cpxs['Fet_Liq_cat_frac'] * (1 - combo_liq_cpxs['Fe3Fet_Liq']) / combo_liq_cpxs['Mg_Liq_cat_frac'])))
-
+    combo_liq_cpxs["Kd_Fe_Mg_Fe2_Lind"] = (
+        combo_liq_cpxs["Lindley_Fe2_Cpx"] / combo_liq_cpxs["Mg_Cpx_cat_6ox"]
+    ) / (
+        combo_liq_cpxs["Fet_Liq_cat_frac"]
+        * (1 - combo_liq_cpxs["Fe3Fet_Liq"])
+        / combo_liq_cpxs["Mg_Liq_cat_frac"]
+    )
 
     # Measured Kd Fe-Mg using Fet
-    combo_liq_cpxs['Kd_Fe_Mg_Fet'] = ((combo_liq_cpxs['Fet_Cpx_cat_6ox'] / combo_liq_cpxs['Mg_Cpx_cat_6ox']) / ((combo_liq_cpxs['Fet_Liq_cat_frac'] / combo_liq_cpxs['Mg_Liq_cat_frac'])))
-
-    combo_liq_cpxs['lnK_Jd_liq'] = np.log((combo_liq_cpxs['Jd_Cpx'].astype(float)) / ((combo_liq_cpxs['Na_Liq_cat_frac']) * (combo_liq_cpxs['Al_Liq_cat_frac']) * ((combo_liq_cpxs['Si_Liq_cat_frac'])**2)))
-
-    combo_liq_cpxs['lnK_Jd_DiHd_liq_1996'] = np.log((combo_liq_cpxs['Jd_Cpx'].astype(float)) * (combo_liq_cpxs['Ca_Liq_cat_frac'].astype(float)) * ((combo_liq_cpxs['Fet_Liq_cat_frac'].astype(float)) + (combo_liq_cpxs['Mg_Liq_cat_frac'].astype(float))) / ((combo_liq_cpxs['DiHd_Cpx_1996'].astype(float)) * (combo_liq_cpxs['Na_Liq_cat_frac'].astype(float)) * (combo_liq_cpxs['Al_Liq_cat_frac'].astype(float))))
-
-    combo_liq_cpxs['lnK_Jd_DiHd_liq_2003'] = np.log((combo_liq_cpxs['Jd_Cpx'].astype(float)) * (combo_liq_cpxs['Ca_Liq_cat_frac'].astype(float)) * ((combo_liq_cpxs['Fet_Liq_cat_frac'].astype(float)) + (combo_liq_cpxs['Mg_Liq_cat_frac'].astype(float))) / ((combo_liq_cpxs['DiHd_2003'].astype(float)) * (combo_liq_cpxs['Na_Liq_cat_frac'].astype(float)) * (combo_liq_cpxs['Al_Liq_cat_frac'].astype(float))))
-
-    combo_liq_cpxs['Kd_Fe_Mg_IdealWB'] = 0.109 + 0.186 * combo_liq_cpxs['Mgno_Cpx']  # equation 35 of wood and blundy
-
-    combo_liq_cpxs['Mgno_Liq_noFe3']= (combo_liq_cpxs['MgO_Liq'] / 40.3044) / ((combo_liq_cpxs['MgO_Liq'] / 40.3044) +(combo_liq_cpxs['FeOt_Liq']) / 71.844)
-
-    combo_liq_cpxs['Mgno_Liq_Fe2']=(combo_liq_cpxs['MgO_Liq'] / 40.3044) / ((combo_liq_cpxs['MgO_Liq'] / 40.3044) + (combo_liq_cpxs['FeOt_Liq'] * (1 - combo_liq_cpxs['Fe3Fet_Liq']) / 71.844))
-
+    combo_liq_cpxs["Kd_Fe_Mg_Fet"] = (
+        combo_liq_cpxs["Fet_Cpx_cat_6ox"] / combo_liq_cpxs["Mg_Cpx_cat_6ox"]
+    ) / (combo_liq_cpxs["Fet_Liq_cat_frac"] / combo_liq_cpxs["Mg_Liq_cat_frac"])
+
+    combo_liq_cpxs["lnK_Jd_liq"] = np.log(
+        (combo_liq_cpxs["Jd_Cpx"].astype(float))
+        / (
+            (combo_liq_cpxs["Na_Liq_cat_frac"])
+            * (combo_liq_cpxs["Al_Liq_cat_frac"])
+            * ((combo_liq_cpxs["Si_Liq_cat_frac"]) ** 2)
+        )
+    )
+
+    combo_liq_cpxs["lnK_Jd_DiHd_liq_1996"] = np.log(
+        (combo_liq_cpxs["Jd_Cpx"].astype(float))
+        * (combo_liq_cpxs["Ca_Liq_cat_frac"].astype(float))
+        * (
+            (combo_liq_cpxs["Fet_Liq_cat_frac"].astype(float))
+            + (combo_liq_cpxs["Mg_Liq_cat_frac"].astype(float))
+        )
+        / (
+            (combo_liq_cpxs["DiHd_Cpx_1996"].astype(float))
+            * (combo_liq_cpxs["Na_Liq_cat_frac"].astype(float))
+            * (combo_liq_cpxs["Al_Liq_cat_frac"].astype(float))
+        )
+    )
+
+    combo_liq_cpxs["lnK_Jd_DiHd_liq_2003"] = np.log(
+        (combo_liq_cpxs["Jd_Cpx"].astype(float))
+        * (combo_liq_cpxs["Ca_Liq_cat_frac"].astype(float))
+        * (
+            (combo_liq_cpxs["Fet_Liq_cat_frac"].astype(float))
+            + (combo_liq_cpxs["Mg_Liq_cat_frac"].astype(float))
+        )
+        / (
+            (combo_liq_cpxs["DiHd_2003"].astype(float))
+            * (combo_liq_cpxs["Na_Liq_cat_frac"].astype(float))
+            * (combo_liq_cpxs["Al_Liq_cat_frac"].astype(float))
+        )
+    )
+
+    combo_liq_cpxs["Kd_Fe_Mg_IdealWB"] = (
+        0.109 + 0.186 * combo_liq_cpxs["Mgno_Cpx"]
+    )  # equation 35 of wood and blundy
+
+    combo_liq_cpxs["Mgno_Liq_noFe3"] = (combo_liq_cpxs["MgO_Liq"] / 40.3044) / (
+        (combo_liq_cpxs["MgO_Liq"] / 40.3044) + (combo_liq_cpxs["FeOt_Liq"]) / 71.844
+    )
+
+    combo_liq_cpxs["Mgno_Liq_Fe2"] = (combo_liq_cpxs["MgO_Liq"] / 40.3044) / (
+        (combo_liq_cpxs["MgO_Liq"] / 40.3044)
+        + (combo_liq_cpxs["FeOt_Liq"] * (1 - combo_liq_cpxs["Fe3Fet_Liq"]) / 71.844)
+    )
 
     # Different ways to calculate DeltaFeMg
-    combo_liq_cpxs['DeltaFeMg_WB'] = abs(combo_liq_cpxs['Kd_Fe_Mg_Fe2'] - combo_liq_cpxs['Kd_Fe_Mg_IdealWB'])
+    combo_liq_cpxs["DeltaFeMg_WB"] = abs(
+        combo_liq_cpxs["Kd_Fe_Mg_Fe2"] - combo_liq_cpxs["Kd_Fe_Mg_IdealWB"]
+    )
     # Adding back in sample names
     if meltmatch is not None and "Sample_ID_Cpx" in meltmatch:
-        combo_liq_cpxs['Sample_ID_Cpx'] = meltmatch['Sample_ID_Cpx']
-        combo_liq_cpxs['Sample_ID_Liq'] = meltmatch['Sample_ID_Liq']
+        combo_liq_cpxs["Sample_ID_Cpx"] = meltmatch["Sample_ID_Cpx"]
+        combo_liq_cpxs["Sample_ID_Liq"] = meltmatch["Sample_ID_Liq"]
     if meltmatch is not None and "Sample_ID_Cpx" not in meltmatch:
-        combo_liq_cpxs['Sample_ID_Cpx'] = meltmatch.index
-        combo_liq_cpxs['Sample_ID_Liq'] = meltmatch.index
+        combo_liq_cpxs["Sample_ID_Cpx"] = meltmatch.index
+        combo_liq_cpxs["Sample_ID_Liq"] = meltmatch.index
     if liq_comps is not None and "Sample_ID_Liq" in liq_comps:
-        combo_liq_cpxs['Sample_ID_Liq'] = liq_comps['Sample_ID_Liq']
+        combo_liq_cpxs["Sample_ID_Liq"] = liq_comps["Sample_ID_Liq"]
     if liq_comps is not None and "Sample_ID_Liq" not in liq_comps:
-        combo_liq_cpxs['Sample_ID_Liq'] = liq_comps.index
+        combo_liq_cpxs["Sample_ID_Liq"] = liq_comps.index
     if cpx_comps is not None and "Sample_ID_Cpx" not in cpx_comps:
-        combo_liq_cpxs['Sample_ID_Cpx'] = cpx_comps.index
+        combo_liq_cpxs["Sample_ID_Cpx"] = cpx_comps.index
     if cpx_comps is not None and "Sample_ID_Cpx" in cpx_comps:
-        combo_liq_cpxs['Sample_ID_Cpx'] = cpx_comps['Sample_ID_Cpx']
+        combo_liq_cpxs["Sample_ID_Cpx"] = cpx_comps["Sample_ID_Cpx"]
 
     combo_liq_cpxs.replace([np.inf, -np.inf], np.nan, inplace=True)
 
     return combo_liq_cpxs
 
 
 def calculate_cpx_sites_from_input_not_cpx(dfin, col_drop):
-
-    cpx_comps_lie=dfin.copy()
-    cpx_comps_lie.columns = [col.replace(col_drop, '_Cpx') for col in cpx_comps_lie.columns]
-    cpx_sites=calculate_clinopyroxene_components(cpx_comps=cpx_comps_lie)
+    cpx_comps_lie = dfin.copy()
+    cpx_comps_lie.columns = [
+        col.replace(col_drop, "_Cpx") for col in cpx_comps_lie.columns
+    ]
+    cpx_sites = calculate_clinopyroxene_components(cpx_comps=cpx_comps_lie)
 
     return cpx_sites
 
 
-
-
-# %% ORTHOPYROXENE 
+# %% ORTHOPYROXENE
 
 
 def calculate_mol_proportions_orthopyroxene(opx_comps):
-
     """
-    
+
     Import orthopyroxene compositions using opx_comps=My_Opxs, returns mole proportions
 
     Parameters
     -------
     opx_comps: pandas.DataFrame
         orthopyroxene compositions with column headings SiO2_Opx, MgO_Opx etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for orthopyroxene with column headings of the form SiO2_Opx_mol_prop
 
     """
 
-    oxide_mass_opx = {'SiO2_Opx': 60.0843, 'MgO_Opx': 40.3044, 'FeOt_Opx': 71.8464, 'CaO_Opx': 56.0774, 'Al2O3_Opx': 101.961, 'Na2O_Opx': 61.9789, 'K2O_Opx': 94.196, 'MnO_Opx': 70.9375, 'TiO2_Opx': 79.8788, 'Cr2O3_Opx': 151.9982}
-    oxide_mass_opx_df = pd.DataFrame.from_dict(oxide_mass_opx, orient='index').T
-    oxide_mass_opx_df['Sample_ID_Opx'] = 'MolWt'
-    oxide_mass_opx_df.set_index('Sample_ID_Opx', inplace=True)
+    oxide_mass_opx = {
+        "SiO2_Opx": 60.0843,
+        "MgO_Opx": 40.3044,
+        "FeOt_Opx": 71.8464,
+        "CaO_Opx": 56.0774,
+        "Al2O3_Opx": 101.961,
+        "Na2O_Opx": 61.9789,
+        "K2O_Opx": 94.196,
+        "MnO_Opx": 70.9375,
+        "TiO2_Opx": 79.8788,
+        "Cr2O3_Opx": 151.9982,
+    }
+    oxide_mass_opx_df = pd.DataFrame.from_dict(oxide_mass_opx, orient="index").T
+    oxide_mass_opx_df["Sample_ID_Opx"] = "MolWt"
+    oxide_mass_opx_df.set_index("Sample_ID_Opx", inplace=True)
 
     # This makes the input match the columns in the oxide mass dataframe
     opx_wt = opx_comps.reindex(oxide_mass_opx_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    opx_wt_combo = pd.concat([oxide_mass_opx_df, opx_wt],)
+    opx_wt_combo = pd.concat(
+        [oxide_mass_opx_df, opx_wt],
+    )
     # Drop the calculation column
     mol_prop_anhyd = opx_wt_combo.div(
-        opx_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+        opx_wt_combo.loc["MolWt", :], axis="columns"
+    ).drop(["MolWt"])
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
 
     return mol_prop_anhyd
 
 
-
 def calculate_oxygens_orthopyroxene(opx_comps):
-
     """
-    
+
     Import orthopyroxene compositions using opx_comps=My_Opxs, returns number of oxygens (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     opx_comps: pandas.DataFrame
         Panda DataFrame of orthopyroxene compositions with column headings SiO2_Opx, MgO_Opx etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Opx_ox
 
     """
 
-    oxygen_num_opx = {'SiO2_Opx': 2, 'MgO_Opx': 1, 'FeOt_Opx': 1, 'CaO_Opx': 1,'Al2O3_Opx': 3, 'Na2O_Opx': 1, 'K2O_Opx': 1, 'MnO_Opx': 1, 'TiO2_Opx': 2, 'Cr2O3_Opx': 3}
-    oxygen_num_opx_df = pd.DataFrame.from_dict(oxygen_num_opx, orient='index').T
-    oxygen_num_opx_df['Sample_ID_Opx'] = 'OxNum'
-    oxygen_num_opx_df.set_index('Sample_ID_Opx', inplace=True)
+    oxygen_num_opx = {
+        "SiO2_Opx": 2,
+        "MgO_Opx": 1,
+        "FeOt_Opx": 1,
+        "CaO_Opx": 1,
+        "Al2O3_Opx": 3,
+        "Na2O_Opx": 1,
+        "K2O_Opx": 1,
+        "MnO_Opx": 1,
+        "TiO2_Opx": 2,
+        "Cr2O3_Opx": 3,
+    }
+    oxygen_num_opx_df = pd.DataFrame.from_dict(oxygen_num_opx, orient="index").T
+    oxygen_num_opx_df["Sample_ID_Opx"] = "OxNum"
+    oxygen_num_opx_df.set_index("Sample_ID_Opx", inplace=True)
 
     mol_prop = calculate_mol_proportions_orthopyroxene(opx_comps=opx_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
-    ox_num_reindex = oxygen_num_opx_df.reindex(
-        mol_prop.columns, axis=1).fillna(0)
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
+    ox_num_reindex = oxygen_num_opx_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
     oxygens_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
     return oxygens_anhyd
 
 
-
 def calculate_6oxygens_orthopyroxene(opx_comps):
-    
     """
-    
+
     Import orthopyroxene compositions using opx_comps=My_Opxs, returns cations on the basis of 6 oxygens.
 
     Parameters
     -------
 
     opx_comps: pandas.DataFrame
         Orthopyroxene compositions with column headings SiO2_Opx, MgO_Opx etc.
@@ -1317,69 +1747,97 @@
     Returns
     -------
     pandas DataFrame
         cations on the basis of 6 oxygens, with column headings of the form ...Opx_cat_6ox.
 
     """
 
-    cation_num_opx = {'SiO2_Opx': 1, 'MgO_Opx': 1, 'FeOt_Opx': 1, 'CaO_Opx': 1, 'Al2O3_Opx': 2, 'Na2O_Opx': 2, 'K2O_Opx': 2, 'MnO_Opx': 1, 'TiO2_Opx': 1, 'Cr2O3_Opx': 2}
-    cation_num_opx_df = pd.DataFrame.from_dict(cation_num_opx, orient='index').T
-    cation_num_opx_df['Sample_ID_Opx'] = 'CatNum'
-    cation_num_opx_df.set_index('Sample_ID_Opx', inplace=True)
+    cation_num_opx = {
+        "SiO2_Opx": 1,
+        "MgO_Opx": 1,
+        "FeOt_Opx": 1,
+        "CaO_Opx": 1,
+        "Al2O3_Opx": 2,
+        "Na2O_Opx": 2,
+        "K2O_Opx": 2,
+        "MnO_Opx": 1,
+        "TiO2_Opx": 1,
+        "Cr2O3_Opx": 2,
+    }
+    cation_num_opx_df = pd.DataFrame.from_dict(cation_num_opx, orient="index").T
+    cation_num_opx_df["Sample_ID_Opx"] = "CatNum"
+    cation_num_opx_df.set_index("Sample_ID_Opx", inplace=True)
 
     oxygens = calculate_oxygens_orthopyroxene(opx_comps=opx_comps)
-    renorm_factor = 6 / (oxygens.sum(axis='columns'))
+    renorm_factor = 6 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_orthopyroxene(opx_comps=opx_comps)
-    mol_prop['oxy_renorm_factor_opx'] = renorm_factor
-    mol_prop_6 = mol_prop.multiply(mol_prop['oxy_renorm_factor_opx'], axis='rows')
-    mol_prop_6.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_6.columns]
+    mol_prop["oxy_renorm_factor_opx"] = renorm_factor
+    mol_prop_6 = mol_prop.multiply(mol_prop["oxy_renorm_factor_opx"], axis="rows")
+    mol_prop_6.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_6.columns
+    ]
 
-    ox_num_reindex = cation_num_opx_df.reindex(
-        mol_prop_6.columns, axis=1).fillna(0)
+    ox_num_reindex = cation_num_opx_df.reindex(mol_prop_6.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_6])
     cation_6 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_6.columns = [str(col).replace('_mol_prop', '_cat_6ox')
-                        for col in mol_prop.columns]
-    cation_6['Al_IV_Opx_cat_6ox'] = 2 - cation_6['SiO2_Opx_cat_6ox']
-    cation_6['Al_VI_Opx_cat_6ox'] = cation_6['Al2O3_Opx_cat_6ox'] - cation_6['Al_IV_Opx_cat_6ox']
+    cation_6.columns = [
+        str(col).replace("_mol_prop", "_cat_6ox") for col in mol_prop.columns
+    ]
+    cation_6["Al_IV_Opx_cat_6ox"] = 2 - cation_6["SiO2_Opx_cat_6ox"]
+    cation_6["Al_VI_Opx_cat_6ox"] = (
+        cation_6["Al2O3_Opx_cat_6ox"] - cation_6["Al_IV_Opx_cat_6ox"]
+    )
     cation_6.Al_VI_Opx_cat_6ox[cation_6.Al_VI_Opx_cat_6ox < 0] = 0
-    cation_6['Si_Ti_Opx_cat_6ox'] = cation_6['SiO2_Opx_cat_6ox'] + cation_6['TiO2_Opx_cat_6ox']
-
-    cation_6_2=cation_6.rename(columns={
-                            'SiO2_Opx_cat_6ox': 'Si_Opx_cat_6ox',
-                            'TiO2_Opx_cat_6ox': 'Ti_Opx_cat_6ox',
-                            'Al2O3_Opx_cat_6ox': 'Al_Opx_cat_6ox',
-                            'FeOt_Opx_cat_6ox': 'Fet_Opx_cat_6ox',
-                            'MnO_Opx_cat_6ox': 'Mn_Opx_cat_6ox',
-                            'MgO_Opx_cat_6ox': 'Mg_Opx_cat_6ox',
-                            'CaO_Opx_cat_6ox': 'Ca_Opx_cat_6ox',
-                            'Na2O_Opx_cat_6ox': 'Na_Opx_cat_6ox',
-                            'K2O_Opx_cat_6ox': 'K_Opx_cat_6ox',
-                            'Cr2O3_Opx_cat_6ox': 'Cr_Opx_cat_6ox',
-                            'P2O5_Opx_cat_6ox': 'P_Opx_cat_6ox_frac',
-                            })
-
-    cation_6_2['En_Simple_MgFeCa_Opx']=(cation_6_2['Mg_Opx_cat_6ox']/(cation_6_2['Mg_Opx_cat_6ox']+cation_6_2['Fet_Opx_cat_6ox']+cation_6_2['Ca_Opx_cat_6ox']))
-
-    cation_6_2['Fs_Simple_MgFeCa_Opx']=(cation_6_2['Fet_Opx_cat_6ox']/(cation_6_2['Mg_Opx_cat_6ox']+cation_6_2['Fet_Opx_cat_6ox']+cation_6_2['Ca_Opx_cat_6ox']))
-
-    cation_6_2['Wo_Simple_MgFeCa_Opx']=(cation_6_2['Ca_Opx_cat_6ox']/(cation_6_2['Mg_Opx_cat_6ox']+cation_6_2['Fet_Opx_cat_6ox']+cation_6_2['Ca_Opx_cat_6ox']))
+    cation_6["Si_Ti_Opx_cat_6ox"] = (
+        cation_6["SiO2_Opx_cat_6ox"] + cation_6["TiO2_Opx_cat_6ox"]
+    )
+
+    cation_6_2 = cation_6.rename(
+        columns={
+            "SiO2_Opx_cat_6ox": "Si_Opx_cat_6ox",
+            "TiO2_Opx_cat_6ox": "Ti_Opx_cat_6ox",
+            "Al2O3_Opx_cat_6ox": "Al_Opx_cat_6ox",
+            "FeOt_Opx_cat_6ox": "Fet_Opx_cat_6ox",
+            "MnO_Opx_cat_6ox": "Mn_Opx_cat_6ox",
+            "MgO_Opx_cat_6ox": "Mg_Opx_cat_6ox",
+            "CaO_Opx_cat_6ox": "Ca_Opx_cat_6ox",
+            "Na2O_Opx_cat_6ox": "Na_Opx_cat_6ox",
+            "K2O_Opx_cat_6ox": "K_Opx_cat_6ox",
+            "Cr2O3_Opx_cat_6ox": "Cr_Opx_cat_6ox",
+            "P2O5_Opx_cat_6ox": "P_Opx_cat_6ox_frac",
+        }
+    )
+
+    cation_6_2["En_Simple_MgFeCa_Opx"] = cation_6_2["Mg_Opx_cat_6ox"] / (
+        cation_6_2["Mg_Opx_cat_6ox"]
+        + cation_6_2["Fet_Opx_cat_6ox"]
+        + cation_6_2["Ca_Opx_cat_6ox"]
+    )
+
+    cation_6_2["Fs_Simple_MgFeCa_Opx"] = cation_6_2["Fet_Opx_cat_6ox"] / (
+        cation_6_2["Mg_Opx_cat_6ox"]
+        + cation_6_2["Fet_Opx_cat_6ox"]
+        + cation_6_2["Ca_Opx_cat_6ox"]
+    )
+
+    cation_6_2["Wo_Simple_MgFeCa_Opx"] = cation_6_2["Ca_Opx_cat_6ox"] / (
+        cation_6_2["Mg_Opx_cat_6ox"]
+        + cation_6_2["Fet_Opx_cat_6ox"]
+        + cation_6_2["Ca_Opx_cat_6ox"]
+    )
 
     return cation_6_2
 
 
-
-
 def calculate_orthopyroxene_components(opx_comps):
-    
     """
-    
+
     Import orthopyroxene compositions using opx_comps=My_Opxs, returns orthopyroxene components along with entered Cpx compositions
 
     Parameters
     -------
     opx_comps: pandas.DataFrame
         Panda DataFrame of orthopyroxene compositions with column headings SiO2_Cpx, MgO_Cpx etc.
 
@@ -1390,38 +1848,81 @@
         -cations on bases of 6 oxygens (column headings of form  Cr2O3_Opx_cat_6ox, as well as Cation_Sum_Opx)
         -orthopyroxene components (NaAlSi2O6, FmTiAlSiO6, CrAl2SiO6, FmAl2SiO6, CaFmSi2O6, Fm2Si2O6, En_Opx, Di_Opx, Mgno_Opx)
 
     """
 
     opx_calc = calculate_6oxygens_orthopyroxene(opx_comps=opx_comps)
     # Sum of cations, used to filter bad analyses
-    opx_calc['Opx_Cation_Sum'] = (opx_calc['Si_Opx_cat_6ox'] + opx_calc['Ti_Opx_cat_6ox'] + opx_calc['Al_Opx_cat_6ox'] + opx_calc['Fet_Opx_cat_6ox'] + opx_calc['Mn_Opx_cat_6ox'] + opx_calc['Mg_Opx_cat_6ox'] + opx_calc['Ca_Opx_cat_6ox'] +opx_calc['Na_Opx_cat_6ox'] + opx_calc['K_Opx_cat_6ox'] + opx_calc['Cr_Opx_cat_6ox'])
-
-    opx_calc['Ca_CaMgFe_Opx']=opx_calc['Ca_Opx_cat_6ox']/(opx_calc['Ca_Opx_cat_6ox']+opx_calc['Fet_Opx_cat_6ox']+opx_calc['Mg_Opx_cat_6ox'])
-
-    opx_calc['NaAlSi2O6'] = opx_calc['Na_Opx_cat_6ox']
-    opx_calc['FmTiAlSiO6'] = opx_calc['Ti_Opx_cat_6ox']
-    opx_calc['CrAl2SiO6'] = opx_calc['Cr_Opx_cat_6ox']
-    opx_calc['FmAl2SiO6'] = opx_calc['Al_VI_Opx_cat_6ox'] - opx_calc['NaAlSi2O6'] - opx_calc['CrAl2SiO6']
+    opx_calc["Opx_Cation_Sum"] = (
+        opx_calc["Si_Opx_cat_6ox"]
+        + opx_calc["Ti_Opx_cat_6ox"]
+        + opx_calc["Al_Opx_cat_6ox"]
+        + opx_calc["Fet_Opx_cat_6ox"]
+        + opx_calc["Mn_Opx_cat_6ox"]
+        + opx_calc["Mg_Opx_cat_6ox"]
+        + opx_calc["Ca_Opx_cat_6ox"]
+        + opx_calc["Na_Opx_cat_6ox"]
+        + opx_calc["K_Opx_cat_6ox"]
+        + opx_calc["Cr_Opx_cat_6ox"]
+    )
+
+    opx_calc["Ca_CaMgFe_Opx"] = opx_calc["Ca_Opx_cat_6ox"] / (
+        opx_calc["Ca_Opx_cat_6ox"]
+        + opx_calc["Fet_Opx_cat_6ox"]
+        + opx_calc["Mg_Opx_cat_6ox"]
+    )
+
+    opx_calc["NaAlSi2O6"] = opx_calc["Na_Opx_cat_6ox"]
+    opx_calc["FmTiAlSiO6"] = opx_calc["Ti_Opx_cat_6ox"]
+    opx_calc["CrAl2SiO6"] = opx_calc["Cr_Opx_cat_6ox"]
+    opx_calc["FmAl2SiO6"] = (
+        opx_calc["Al_VI_Opx_cat_6ox"] - opx_calc["NaAlSi2O6"] - opx_calc["CrAl2SiO6"]
+    )
     opx_calc.FmAl2SiO6[opx_calc.FmAl2SiO6 < 0] = 0
-    opx_calc['CaFmSi2O6'] = opx_calc['Ca_Opx_cat_6ox']
-    opx_calc['Fm2Si2O6'] = (((opx_calc['Fet_Opx_cat_6ox'] + opx_calc['Mg_Opx_cat_6ox'] + opx_calc['Mn_Opx_cat_6ox'])- opx_calc['FmTiAlSiO6'] - opx_calc['FmAl2SiO6'] - opx_calc['CaFmSi2O6']) / 2)
-    opx_calc['En_Opx'] = opx_calc['Fm2Si2O6'] * (opx_calc['Mg_Opx_cat_6ox'] / (opx_calc['Mg_Opx_cat_6ox'] + opx_calc['Fet_Opx_cat_6ox'] + opx_calc['Mn_Opx_cat_6ox']))
-    opx_calc['Di_Opx'] = opx_calc['CaFmSi2O6'] * (opx_calc['Mg_Opx_cat_6ox'] / (opx_calc['Mg_Opx_cat_6ox'] + opx_calc['Fet_Opx_cat_6ox'] + opx_calc['Mn_Opx_cat_6ox']))
-    opx_calc['Mgno_OPX'] = (opx_comps['MgO_Opx'] / 40.3044) / (opx_comps['MgO_Opx'] / 40.3044 + opx_comps['FeOt_Opx'] / 71.844)
+    opx_calc["CaFmSi2O6"] = opx_calc["Ca_Opx_cat_6ox"]
+    opx_calc["Fm2Si2O6"] = (
+        (
+            opx_calc["Fet_Opx_cat_6ox"]
+            + opx_calc["Mg_Opx_cat_6ox"]
+            + opx_calc["Mn_Opx_cat_6ox"]
+        )
+        - opx_calc["FmTiAlSiO6"]
+        - opx_calc["FmAl2SiO6"]
+        - opx_calc["CaFmSi2O6"]
+    ) / 2
+    opx_calc["En_Opx"] = opx_calc["Fm2Si2O6"] * (
+        opx_calc["Mg_Opx_cat_6ox"]
+        / (
+            opx_calc["Mg_Opx_cat_6ox"]
+            + opx_calc["Fet_Opx_cat_6ox"]
+            + opx_calc["Mn_Opx_cat_6ox"]
+        )
+    )
+    opx_calc["Di_Opx"] = opx_calc["CaFmSi2O6"] * (
+        opx_calc["Mg_Opx_cat_6ox"]
+        / (
+            opx_calc["Mg_Opx_cat_6ox"]
+            + opx_calc["Fet_Opx_cat_6ox"]
+            + opx_calc["Mn_Opx_cat_6ox"]
+        )
+    )
+    opx_calc["Mgno_OPX"] = (opx_comps["MgO_Opx"] / 40.3044) / (
+        opx_comps["MgO_Opx"] / 40.3044 + opx_comps["FeOt_Opx"] / 71.844
+    )
 
     opx_calc = pd.concat([opx_comps, opx_calc], axis=1)
 
     return opx_calc
 
+
 def calculate_orthopyroxene_liquid_components(
-        *, opx_comps=None, liq_comps=None, meltmatch=None, Fe3Fet_Liq=None):
-    
+    *, opx_comps=None, liq_comps=None, meltmatch=None, Fe3Fet_Liq=None
+):
     """
-    
+
     Import orthopyroxene compositions using opx_comps=My_Opxs and liquid compositions using liq_comps=My_Liquids,
         returns orthopyroxene and liquid components.
 
     Parameters
     -------
     liq_comps: pandas.DataFrame
         liquid compositions with column headings SiO2_Liq, MgO_Liq etc.
@@ -1439,91 +1940,144 @@
        inputted opx compositions, opx cations on 6 oxygen basis, opx components and opx-liquid components.
 
     """
     # For when users enter a combined dataframe meltmatch=""
     if meltmatch is not None:
         combo_liq_opxs = meltmatch
     if liq_comps is not None and opx_comps is not None:
-        liq_comps_c=liq_comps.copy()
+        liq_comps_c = liq_comps.copy()
         if Fe3Fet_Liq is not None:
-            liq_comps_c['Fe3Fet_Liq']=Fe3Fet_Liq
+            liq_comps_c["Fe3Fet_Liq"] = Fe3Fet_Liq
 
         if len(liq_comps) != len(opx_comps):
             raise Exception(
-                "inputted dataframes for liq_comps and opx_comps need to have the same number of rows")
+                "inputted dataframes for liq_comps and opx_comps need to have the same number of rows"
+            )
         else:
             myOPXs1_comp = calculate_orthopyroxene_components(opx_comps=opx_comps)
-            myLiquids1_comps = calculate_anhydrous_cat_fractions_liquid(liq_comps=liq_comps_c)
+            myLiquids1_comps = calculate_anhydrous_cat_fractions_liquid(
+                liq_comps=liq_comps_c
+            )
             combo_liq_opxs = pd.concat([myLiquids1_comps, myOPXs1_comp], axis=1)
 
-    combo_liq_opxs['ln_Fm2Si2O6_liq'] = (np.log(combo_liq_opxs['Fm2Si2O6'].astype('float64') / (combo_liq_opxs['Si_Liq_cat_frac']**2 * (combo_liq_opxs['Fet_Liq_cat_frac'] + combo_liq_opxs['Mn_Liq_cat_frac'] + combo_liq_opxs['Mg_Liq_cat_frac'])**2)))
-
-    combo_liq_opxs['ln_FmAl2SiO6_liq'] = (np.log(combo_liq_opxs['FmAl2SiO6'].astype('float64') / (combo_liq_opxs['Si_Liq_cat_frac'] * combo_liq_opxs['Al_Liq_cat_frac']**2 * (combo_liq_opxs['Fet_Liq_cat_frac']+ combo_liq_opxs['Mn_Liq_cat_frac'] + combo_liq_opxs['Mg_Liq_cat_frac']))))
-    combo_liq_opxs['Kd_Fe_Mg_Fet'] = ((combo_liq_opxs['FeOt_Opx'] / 71.844) / (combo_liq_opxs['MgO_Opx'] / 40.3044)) / ((combo_liq_opxs['FeOt_Liq'] / 71.844) / (combo_liq_opxs['MgO_Liq'] / 40.3044))
-
-    combo_liq_opxs['Kd_Fe_Mg_Fe2'] = ((combo_liq_opxs['FeOt_Opx'] / 71.844) / (combo_liq_opxs['MgO_Opx'] / 40.3044)) / (((1 - combo_liq_opxs['Fe3Fet_Liq']) * combo_liq_opxs['FeOt_Liq'] / 71.844) / (combo_liq_opxs['MgO_Liq'] / 40.3044))
-
-    combo_liq_opxs['Ideal_Kd'] = 0.4805 - 0.3733 * combo_liq_opxs['Si_Liq_cat_frac']
-    combo_liq_opxs['Delta_Kd_Fe_Mg_Fe2'] = abs(combo_liq_opxs['Ideal_Kd'] - combo_liq_opxs['Kd_Fe_Mg_Fe2'])
+    combo_liq_opxs["ln_Fm2Si2O6_liq"] = np.log(
+        combo_liq_opxs["Fm2Si2O6"].astype("float64")
+        / (
+            combo_liq_opxs["Si_Liq_cat_frac"] ** 2
+            * (
+                combo_liq_opxs["Fet_Liq_cat_frac"]
+                + combo_liq_opxs["Mn_Liq_cat_frac"]
+                + combo_liq_opxs["Mg_Liq_cat_frac"]
+            )
+            ** 2
+        )
+    )
+
+    combo_liq_opxs["ln_FmAl2SiO6_liq"] = np.log(
+        combo_liq_opxs["FmAl2SiO6"].astype("float64")
+        / (
+            combo_liq_opxs["Si_Liq_cat_frac"]
+            * combo_liq_opxs["Al_Liq_cat_frac"] ** 2
+            * (
+                combo_liq_opxs["Fet_Liq_cat_frac"]
+                + combo_liq_opxs["Mn_Liq_cat_frac"]
+                + combo_liq_opxs["Mg_Liq_cat_frac"]
+            )
+        )
+    )
+    combo_liq_opxs["Kd_Fe_Mg_Fet"] = (
+        (combo_liq_opxs["FeOt_Opx"] / 71.844) / (combo_liq_opxs["MgO_Opx"] / 40.3044)
+    ) / ((combo_liq_opxs["FeOt_Liq"] / 71.844) / (combo_liq_opxs["MgO_Liq"] / 40.3044))
+
+    combo_liq_opxs["Kd_Fe_Mg_Fe2"] = (
+        (combo_liq_opxs["FeOt_Opx"] / 71.844) / (combo_liq_opxs["MgO_Opx"] / 40.3044)
+    ) / (
+        ((1 - combo_liq_opxs["Fe3Fet_Liq"]) * combo_liq_opxs["FeOt_Liq"] / 71.844)
+        / (combo_liq_opxs["MgO_Liq"] / 40.3044)
+    )
+
+    combo_liq_opxs["Ideal_Kd"] = 0.4805 - 0.3733 * combo_liq_opxs["Si_Liq_cat_frac"]
+    combo_liq_opxs["Delta_Kd_Fe_Mg_Fe2"] = abs(
+        combo_liq_opxs["Ideal_Kd"] - combo_liq_opxs["Kd_Fe_Mg_Fe2"]
+    )
     b = np.empty(len(combo_liq_opxs), dtype=str)
-    
-    for i in range(0, len(combo_liq_opxs)):
 
-        if combo_liq_opxs['Delta_Kd_Fe_Mg_Fe2'].iloc[i] > 0.06:
+    for i in range(0, len(combo_liq_opxs)):
+        if combo_liq_opxs["Delta_Kd_Fe_Mg_Fe2"].iloc[i] > 0.06:
             b[i] = str("No")
-        if combo_liq_opxs['Delta_Kd_Fe_Mg_Fe2'].iloc[i] < 0.06:
+        if combo_liq_opxs["Delta_Kd_Fe_Mg_Fe2"].iloc[i] < 0.06:
             b[i] = str("Yes")
     combo_liq_opxs.insert(1, "Kd Eq (Put2008+-0.06)", b)
 
-    combo_liq_opxs['Mgno_Liq_noFe3']= ((combo_liq_opxs['MgO_Liq'] / 40.3044) / ((combo_liq_opxs['MgO_Liq'] / 40.3044) + (combo_liq_opxs['FeOt_Liq']) / 71.844))
-    combo_liq_opxs['Mgno_Liq_Fe2']=((combo_liq_opxs['MgO_Liq'] / 40.3044) / ((combo_liq_opxs['MgO_Liq'] / 40.3044) + (combo_liq_opxs['FeOt_Liq'] * (1 - combo_liq_opxs['Fe3Fet_Liq']) / 71.844)))
+    combo_liq_opxs["Mgno_Liq_noFe3"] = (combo_liq_opxs["MgO_Liq"] / 40.3044) / (
+        (combo_liq_opxs["MgO_Liq"] / 40.3044) + (combo_liq_opxs["FeOt_Liq"]) / 71.844
+    )
+    combo_liq_opxs["Mgno_Liq_Fe2"] = (combo_liq_opxs["MgO_Liq"] / 40.3044) / (
+        (combo_liq_opxs["MgO_Liq"] / 40.3044)
+        + (combo_liq_opxs["FeOt_Liq"] * (1 - combo_liq_opxs["Fe3Fet_Liq"]) / 71.844)
+    )
 
     return combo_liq_opxs
 
 
 # %% K-FELDSPAR
 
 
 def calculate_mol_proportions_kspar(kspar_comps):
-    
     """
-    
+
     Import Kspar compositions using kspar_comps=My_Kspar, returns mole proportions
 
     Parameters
     -------
     kspar_comps: pandas.DataFrame
             Panda DataFrame of kspar compositions with column headings SiO2_Kspar, MgO_Kspar etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for kspar with column headings of the form SiO2_Kspar_mol_prop
 
     """
 
-    oxide_mass_sp = {'SiO2_Kspar': 60.0843, 'MgO_Kspar': 40.3044, 'FeOt_Kspar': 71.8464, 'CaO_Kspar': 56.0774,'Al2O3_Kspar': 101.961, 'Na2O_Kspar': 61.9789, 'K2O_Kspar': 94.196, 'MnO_Kspar': 70.9375, 'TiO2_Kspar': 79.7877, 'Cr2O3_Kspar': 151.9982, 'P2O5_Kspar': 141.937}
-    oxide_mass_ksp_df = pd.DataFrame.from_dict(oxide_mass_sp, orient='index').T
-    oxide_mass_ksp_df['Sample_ID_Kspar'] = 'MolWt'
-    oxide_mass_ksp_df.set_index('Sample_ID_Kspar', inplace=True)
+    oxide_mass_sp = {
+        "SiO2_Kspar": 60.0843,
+        "MgO_Kspar": 40.3044,
+        "FeOt_Kspar": 71.8464,
+        "CaO_Kspar": 56.0774,
+        "Al2O3_Kspar": 101.961,
+        "Na2O_Kspar": 61.9789,
+        "K2O_Kspar": 94.196,
+        "MnO_Kspar": 70.9375,
+        "TiO2_Kspar": 79.7877,
+        "Cr2O3_Kspar": 151.9982,
+        "P2O5_Kspar": 141.937,
+    }
+    oxide_mass_ksp_df = pd.DataFrame.from_dict(oxide_mass_sp, orient="index").T
+    oxide_mass_ksp_df["Sample_ID_Kspar"] = "MolWt"
+    oxide_mass_ksp_df.set_index("Sample_ID_Kspar", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     ksp_wt = kspar_comps.reindex(oxide_mass_ksp_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    ksp_wt_combo = pd.concat([oxide_mass_ksp_df, ksp_wt],)
+    ksp_wt_combo = pd.concat(
+        [oxide_mass_ksp_df, ksp_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = ksp_wt_combo.div(ksp_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
-    
+    mol_prop_anhyd = ksp_wt_combo.div(
+        ksp_wt_combo.loc["MolWt", :], axis="columns"
+    ).drop(["MolWt"])
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
+
     return mol_prop_anhyd
 
+
 def calculate_cat_proportions_kspar(*, kspar_comps=None, oxide_headers=False):
-    
     """
-    
+
     Import kspar compositions using kspar_comps=My_kspars, returns cation proportions
 
     Parameters
     -------
     kspar_comps: pandas.DataFrame
             kspar compositions with column headings SiO2_Kspar, MgO_Kspar etc.
 
@@ -1533,225 +2087,332 @@
         This is used for rapid matrix division for
         pre-processing of data for cation fractions etc
 
     Returns
     -------
     pandas DataFrame
         cation proportions for kspar with column headings of the form... Ksp_cat_prop
-   
+
     """
 
-    cation_num_sp = {'SiO2_Kspar': 1, 'MgO_Kspar': 1, 'FeOt_Kspar': 1, 'CaO_Kspar': 1, 'Al2O3_Kspar': 2, 'Na2O_Kspar': 2, 'K2O_Kspar': 2, 'MnO_Kspar': 1, 'TiO2_Kspar': 1, 'Cr2O3_Kspar': 2, 'P2O5_Kspar': 2}
-    cation_num_ksp_df = pd.DataFrame.from_dict(cation_num_sp, orient='index').T
-    cation_num_ksp_df['Sample_ID_Kspar'] = 'CatNum'
-    cation_num_ksp_df.set_index('Sample_ID_Kspar', inplace=True)
-
-    oxide_mass_sp = {'SiO2_Kspar': 60.0843, 'MgO_Kspar': 40.3044, 'FeOt_Kspar': 71.8464, 'CaO_Kspar': 56.0774,'Al2O3_Kspar': 101.961, 'Na2O_Kspar': 61.9789, 'K2O_Kspar': 94.196, 'MnO_Kspar': 70.9375, 'TiO2_Kspar': 79.7877, 'Cr2O3_Kspar': 151.9982, 'P2O5_Kspar': 141.937}
-    oxide_mass_ksp_df = pd.DataFrame.from_dict(oxide_mass_sp, orient='index').T
-    oxide_mass_ksp_df['Sample_ID_Kspar'] = 'MolWt'
-    oxide_mass_ksp_df.set_index('Sample_ID_Kspar', inplace=True)
+    cation_num_sp = {
+        "SiO2_Kspar": 1,
+        "MgO_Kspar": 1,
+        "FeOt_Kspar": 1,
+        "CaO_Kspar": 1,
+        "Al2O3_Kspar": 2,
+        "Na2O_Kspar": 2,
+        "K2O_Kspar": 2,
+        "MnO_Kspar": 1,
+        "TiO2_Kspar": 1,
+        "Cr2O3_Kspar": 2,
+        "P2O5_Kspar": 2,
+    }
+    cation_num_ksp_df = pd.DataFrame.from_dict(cation_num_sp, orient="index").T
+    cation_num_ksp_df["Sample_ID_Kspar"] = "CatNum"
+    cation_num_ksp_df.set_index("Sample_ID_Kspar", inplace=True)
+
+    oxide_mass_sp = {
+        "SiO2_Kspar": 60.0843,
+        "MgO_Kspar": 40.3044,
+        "FeOt_Kspar": 71.8464,
+        "CaO_Kspar": 56.0774,
+        "Al2O3_Kspar": 101.961,
+        "Na2O_Kspar": 61.9789,
+        "K2O_Kspar": 94.196,
+        "MnO_Kspar": 70.9375,
+        "TiO2_Kspar": 79.7877,
+        "Cr2O3_Kspar": 151.9982,
+        "P2O5_Kspar": 141.937,
+    }
+    oxide_mass_ksp_df = pd.DataFrame.from_dict(oxide_mass_sp, orient="index").T
+    oxide_mass_ksp_df["Sample_ID_Kspar"] = "MolWt"
+    oxide_mass_ksp_df.set_index("Sample_ID_Kspar", inplace=True)
 
     ksp_prop_no_cat_num = calculate_mol_proportions_kspar(kspar_comps=kspar_comps)
-    ksp_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in ksp_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_ksp_df.reindex(oxide_mass_ksp_df.columns, axis=1).fillna(0)
+    ksp_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in ksp_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_ksp_df.reindex(
+        oxide_mass_ksp_df.columns, axis=1
+    ).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, ksp_prop_no_cat_num])
-    cation_prop_anhyd = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
-    
+    cation_prop_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
+
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Kspar_cat_prop': 'Si_Kspar_cat_prop',
-                            'TiO2_Kspar_cat_prop': 'Ti_Kspar_cat_prop',
-                            'Al2O3_Kspar_cat_prop': 'Al_Kspar_cat_prop',
-                            'FeOt_Kspar_cat_prop': 'Fet_Kspar_cat_prop',
-                            'MnO_Kspar_cat_prop': 'Mn_Kspar_cat_prop',
-                            'MgO_Kspar_cat_prop': 'Mg_Kspar_cat_prop',
-                            'CaO_Kspar_cat_prop': 'Ca_Kspar_cat_prop',
-                            'Na2O_Kspar_cat_prop': 'Na_Kspar_cat_prop',
-                            'K2O_Kspar_cat_prop': 'K_Kspar_cat_prop',
-                            'Cr2O3_Kspar_cat_prop': 'Cr_Kspar_cat_prop',
-                            'P2O5_Kspar_cat_prop': 'P_Kspar_cat_prop',
-                            })
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Kspar_cat_prop": "Si_Kspar_cat_prop",
+                "TiO2_Kspar_cat_prop": "Ti_Kspar_cat_prop",
+                "Al2O3_Kspar_cat_prop": "Al_Kspar_cat_prop",
+                "FeOt_Kspar_cat_prop": "Fet_Kspar_cat_prop",
+                "MnO_Kspar_cat_prop": "Mn_Kspar_cat_prop",
+                "MgO_Kspar_cat_prop": "Mg_Kspar_cat_prop",
+                "CaO_Kspar_cat_prop": "Ca_Kspar_cat_prop",
+                "Na2O_Kspar_cat_prop": "Na_Kspar_cat_prop",
+                "K2O_Kspar_cat_prop": "K_Kspar_cat_prop",
+                "Cr2O3_Kspar_cat_prop": "Cr_Kspar_cat_prop",
+                "P2O5_Kspar_cat_prop": "P_Kspar_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
-def calculate_oxygens_kspar(kspar_comps):
 
+def calculate_oxygens_kspar(kspar_comps):
     """
-    
-    Import kspar compositions using kspar_comps=My_Kspars, returns number of oxygens 
+
+    Import kspar compositions using kspar_comps=My_Kspars, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     kspar_comps: pandas.DataFrame
         kspar compositions with column headings SiO2_Kspar, MgO_Kspar etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Kspar_ox
-    
+
     """
 
-    oxygen_num_sp = {'SiO2_Kspar': 2, 'MgO_Kspar': 1, 'FeOt_Kspar': 1, 'CaO_Kspar': 1, 'Al2O3_Kspar': 3, 'Na2O_Kspar': 1, 'K2O_Kspar': 1, 'MnO_Kspar': 1, 'TiO2_Kspar': 2, 'Cr2O3_Kspar': 3, 'P2O5_Kspar': 5}
-    oxygen_num_ksp_df = pd.DataFrame.from_dict(oxygen_num_sp, orient='index').T
-    oxygen_num_ksp_df['Sample_ID_Kspar'] = 'OxNum'
-    oxygen_num_ksp_df.set_index('Sample_ID_Kspar', inplace=True)
+    oxygen_num_sp = {
+        "SiO2_Kspar": 2,
+        "MgO_Kspar": 1,
+        "FeOt_Kspar": 1,
+        "CaO_Kspar": 1,
+        "Al2O3_Kspar": 3,
+        "Na2O_Kspar": 1,
+        "K2O_Kspar": 1,
+        "MnO_Kspar": 1,
+        "TiO2_Kspar": 2,
+        "Cr2O3_Kspar": 3,
+        "P2O5_Kspar": 5,
+    }
+    oxygen_num_ksp_df = pd.DataFrame.from_dict(oxygen_num_sp, orient="index").T
+    oxygen_num_ksp_df["Sample_ID_Kspar"] = "OxNum"
+    oxygen_num_ksp_df.set_index("Sample_ID_Kspar", inplace=True)
 
     mol_prop = calculate_mol_proportions_kspar(kspar_comps=kspar_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_ksp_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
-def calculate_8oxygens_kspar(kspar_comps):
 
+def calculate_8oxygens_kspar(kspar_comps):
     """
-    
+
     Import kspar compositions using kspar_comps=My_Kspars, returns cations on the basis of 8 oxygens.
 
     Parameters
     -------
     kspar_comps: pandas.DataFrame
         kspar compositions with column headings SiO2_Kspar, MgO_Kspar etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 8 oxygens, with column headings of the form... Ksp_cat_8ox.
-    
-    """
 
-    cation_num_sp = {'SiO2_Kspar': 1, 'MgO_Kspar': 1, 'FeOt_Kspar': 1, 'CaO_Kspar': 1, 'Al2O3_Kspar': 2, 'Na2O_Kspar': 2, 'K2O_Kspar': 2, 'MnO_Kspar': 1, 'TiO2_Kspar': 1, 'Cr2O3_Kspar': 2, 'P2O5_Kspar': 2}
+    """
 
-    cation_num_ksp_df = pd.DataFrame.from_dict(cation_num_sp, orient='index').T
-    cation_num_ksp_df['Sample_ID_Kspar'] = 'CatNum'
-    cation_num_ksp_df.set_index('Sample_ID_Kspar', inplace=True)
+    cation_num_sp = {
+        "SiO2_Kspar": 1,
+        "MgO_Kspar": 1,
+        "FeOt_Kspar": 1,
+        "CaO_Kspar": 1,
+        "Al2O3_Kspar": 2,
+        "Na2O_Kspar": 2,
+        "K2O_Kspar": 2,
+        "MnO_Kspar": 1,
+        "TiO2_Kspar": 1,
+        "Cr2O3_Kspar": 2,
+        "P2O5_Kspar": 2,
+    }
+
+    cation_num_ksp_df = pd.DataFrame.from_dict(cation_num_sp, orient="index").T
+    cation_num_ksp_df["Sample_ID_Kspar"] = "CatNum"
+    cation_num_ksp_df.set_index("Sample_ID_Kspar", inplace=True)
 
     oxygens = calculate_oxygens_kspar(kspar_comps=kspar_comps)
-    renorm_factor = 8 / (oxygens.sum(axis='columns'))
+    renorm_factor = 8 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_kspar(kspar_comps=kspar_comps)
-    mol_prop['oxy_renorm_factor_sp'] = renorm_factor
-    mol_prop_8 = mol_prop.multiply(mol_prop['oxy_renorm_factor_sp'], axis='rows')
-    mol_prop_8.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop_8.columns]
+    mol_prop["oxy_renorm_factor_sp"] = renorm_factor
+    mol_prop_8 = mol_prop.multiply(mol_prop["oxy_renorm_factor_sp"], axis="rows")
+    mol_prop_8.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_8.columns
+    ]
 
     ox_num_reindex = cation_num_ksp_df.reindex(mol_prop_8.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_8])
-    cation_8 = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_8.columns = [str(col).replace('_mol_prop', '_cat_8ox')
-                        for col in mol_prop.columns]
+    cation_8 = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_8_2=cation_8.rename(columns={
-                            'SiO2_Kspar_cat_8ox': 'Si_Kspar_cat_8ox',
-                            'TiO2_Kspar_cat_8ox': 'Ti_Kspar_cat_8ox',
-                            'Al2O3_Kspar_cat_8ox': 'Al_Kspar_cat_8ox',
-                            'FeOt_Kspar_cat_8ox': 'Fet_Kspar_cat_8ox',
-                            'MnO_Kspar_cat_8ox': 'Mn_Kspar_cat_8ox',
-                            'MgO_Kspar_cat_8ox': 'Mg_Kspar_cat_8ox',
-                            'CaO_Kspar_cat_8ox': 'Ca_Kspar_cat_8ox',
-                            'Na2O_Kspar_cat_8ox': 'Na_Kspar_cat_8ox',
-                            'K2O_Kspar_cat_8ox': 'K_Kspar_cat_8ox',
-                            'Cr2O3_Kspar_cat_8ox': 'Cr_Kspar_cat_8ox',
-                            'P2O5_Kspar_cat_8ox': 'P_Kspar_cat_8ox',})
+    cation_8.columns = [
+        str(col).replace("_mol_prop", "_cat_8ox") for col in mol_prop.columns
+    ]
+
+    cation_8_2 = cation_8.rename(
+        columns={
+            "SiO2_Kspar_cat_8ox": "Si_Kspar_cat_8ox",
+            "TiO2_Kspar_cat_8ox": "Ti_Kspar_cat_8ox",
+            "Al2O3_Kspar_cat_8ox": "Al_Kspar_cat_8ox",
+            "FeOt_Kspar_cat_8ox": "Fet_Kspar_cat_8ox",
+            "MnO_Kspar_cat_8ox": "Mn_Kspar_cat_8ox",
+            "MgO_Kspar_cat_8ox": "Mg_Kspar_cat_8ox",
+            "CaO_Kspar_cat_8ox": "Ca_Kspar_cat_8ox",
+            "Na2O_Kspar_cat_8ox": "Na_Kspar_cat_8ox",
+            "K2O_Kspar_cat_8ox": "K_Kspar_cat_8ox",
+            "Cr2O3_Kspar_cat_8ox": "Cr_Kspar_cat_8ox",
+            "P2O5_Kspar_cat_8ox": "P_Kspar_cat_8ox",
+        }
+    )
 
     return cation_8_2
 
 
 def calculate_kspar_components(kspar_comps, append):
-
     """
-    
+
     Import kspar compositions using kspar_comps=My_Kspars, returns cations on the basis of 8 oxygens.
 
     Parameters
     -------
     kspar_comps: pandas.DataFrame
         kspar compositions with column headings SiO2_Kspar, MgO_Kspar etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 8 oxygens, with column headings of the form... Ksp_cat_8ox.
-    
+
     """
 
     kspar_comps_new = kspar_comps.copy()
-    kspar_comps_new.columns = [col.replace(append, '_Kspar') for col in kspar_comps_new.columns]
+    kspar_comps_new.columns = [
+        col.replace(append, "_Kspar") for col in kspar_comps_new.columns
+    ]
     kspar_comps = kspar_comps_new.copy()
 
     kspar_calc = calculate_8oxygens_kspar(kspar_comps=kspar_comps)
-    kspar_calc['Kspar_Cation_Sum'] = (kspar_calc['Si_Kspar_cat_8ox']+kspar_calc['Ti_Kspar_cat_8ox']+kspar_calc['Al_Kspar_cat_8ox']+kspar_calc['Fet_Kspar_cat_8ox']+kspar_calc['Mn_Kspar_cat_8ox']+kspar_calc['Mg_Kspar_cat_8ox']+kspar_calc['Ca_Kspar_cat_8ox']+kspar_calc['Na_Kspar_cat_8ox']+kspar_calc['K_Kspar_cat_8ox']+kspar_calc['Cr_Kspar_cat_8ox']+kspar_calc['P_Kspar_cat_8ox'])
-
-    kspar_calc['Na_Ca_M_Kspar'] = kspar_calc['Na_Kspar_cat_8ox'] + kspar_calc['Ca_Kspar_cat_8ox']
-    kspar_calc['Si_Al_T_Kspar'] = kspar_calc['Si_Kspar_cat_8ox'] + kspar_calc['Al_Kspar_cat_8ox']
+    kspar_calc["Kspar_Cation_Sum"] = (
+        kspar_calc["Si_Kspar_cat_8ox"]
+        + kspar_calc["Ti_Kspar_cat_8ox"]
+        + kspar_calc["Al_Kspar_cat_8ox"]
+        + kspar_calc["Fet_Kspar_cat_8ox"]
+        + kspar_calc["Mn_Kspar_cat_8ox"]
+        + kspar_calc["Mg_Kspar_cat_8ox"]
+        + kspar_calc["Ca_Kspar_cat_8ox"]
+        + kspar_calc["Na_Kspar_cat_8ox"]
+        + kspar_calc["K_Kspar_cat_8ox"]
+        + kspar_calc["Cr_Kspar_cat_8ox"]
+        + kspar_calc["P_Kspar_cat_8ox"]
+    )
+
+    kspar_calc["Na_Ca_M_Kspar"] = (
+        kspar_calc["Na_Kspar_cat_8ox"] + kspar_calc["Ca_Kspar_cat_8ox"]
+    )
+    kspar_calc["Si_Al_T_Kspar"] = (
+        kspar_calc["Si_Kspar_cat_8ox"] + kspar_calc["Al_Kspar_cat_8ox"]
+    )
 
     cat_prop = calculate_cat_proportions_kspar(kspar_comps=kspar_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
-    cat_frac_anhyd['An_Kspar'] = cat_frac_anhyd['Ca_Kspar_cat_frac'] / (cat_frac_anhyd['Ca_Kspar_cat_frac'] + cat_frac_anhyd['Na_Kspar_cat_frac'] + cat_frac_anhyd['K_Kspar_cat_frac'])
-    cat_frac_anhyd['Ab_Kspar'] = cat_frac_anhyd['Na_Kspar_cat_frac'] / (cat_frac_anhyd['Ca_Kspar_cat_frac'] + cat_frac_anhyd['Na_Kspar_cat_frac'] + cat_frac_anhyd['K_Kspar_cat_frac'])
-    cat_frac_anhyd['Or_Kspar'] = 1 - cat_frac_anhyd['An_Kspar'] - cat_frac_anhyd['Ab_Kspar']
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
+    cat_frac_anhyd["An_Kspar"] = cat_frac_anhyd["Ca_Kspar_cat_frac"] / (
+        cat_frac_anhyd["Ca_Kspar_cat_frac"]
+        + cat_frac_anhyd["Na_Kspar_cat_frac"]
+        + cat_frac_anhyd["K_Kspar_cat_frac"]
+    )
+    cat_frac_anhyd["Ab_Kspar"] = cat_frac_anhyd["Na_Kspar_cat_frac"] / (
+        cat_frac_anhyd["Ca_Kspar_cat_frac"]
+        + cat_frac_anhyd["Na_Kspar_cat_frac"]
+        + cat_frac_anhyd["K_Kspar_cat_frac"]
+    )
+    cat_frac_anhyd["Or_Kspar"] = (
+        1 - cat_frac_anhyd["An_Kspar"] - cat_frac_anhyd["Ab_Kspar"]
+    )
     cat_frac_anhyd2 = pd.concat([kspar_comps, kspar_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-# %% SPINEL 
+# %% SPINEL
 
 
 def calculate_mol_proportions_spinel(sp_comps):
-    
     """
-    
+
     Import spinel compositions using sp_comps=My_Spinels, returns mole proportions
 
     Parameters
     -------
     sp_comps: pandas.DataFrame
             Panda DataFrame of spinel compositions with column headings SiO2_Sp, MgO_Sp etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for spinels with column headings of the form SiO2_Sp_mol_prop
-    
+
     """
 
-    oxide_mass_sp = {'SiO2_Sp': 60.0843, 'MgO_Sp': 40.3044, 'FeOt_Sp': 71.8464, 'CaO_Sp': 56.0774,'Al2O3_Sp': 101.961, 'Na2O_Sp': 61.9789, 'K2O_Sp': 94.196, 'MnO_Sp': 70.9375, 'TiO2_Sp': 79.7877, 'Cr2O3_Sp': 151.9982, 'P2O5_Sp': 141.937}
-    oxide_mass_sp_df = pd.DataFrame.from_dict(oxide_mass_sp, orient='index').T
-    oxide_mass_sp_df['Sample_ID_Sp'] = 'MolWt'
-    oxide_mass_sp_df.set_index('Sample_ID_Sp', inplace=True)
+    oxide_mass_sp = {
+        "SiO2_Sp": 60.0843,
+        "MgO_Sp": 40.3044,
+        "FeOt_Sp": 71.8464,
+        "CaO_Sp": 56.0774,
+        "Al2O3_Sp": 101.961,
+        "Na2O_Sp": 61.9789,
+        "K2O_Sp": 94.196,
+        "MnO_Sp": 70.9375,
+        "TiO2_Sp": 79.7877,
+        "Cr2O3_Sp": 151.9982,
+        "P2O5_Sp": 141.937,
+    }
+    oxide_mass_sp_df = pd.DataFrame.from_dict(oxide_mass_sp, orient="index").T
+    oxide_mass_sp_df["Sample_ID_Sp"] = "MolWt"
+    oxide_mass_sp_df.set_index("Sample_ID_Sp", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     sp_wt = sp_comps.reindex(oxide_mass_sp_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    sp_wt_combo = pd.concat([oxide_mass_sp_df, sp_wt],)
+    sp_wt_combo = pd.concat(
+        [oxide_mass_sp_df, sp_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = sp_wt_combo.div(
-        sp_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = sp_wt_combo.div(sp_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
-def calculate_cat_proportions_spinel(*, sp_comps=None, oxide_headers=False):
 
+def calculate_cat_proportions_spinel(*, sp_comps=None, oxide_headers=False):
     """
-    
+
     Import spinel compositions using sp_comps=My_spinels, returns cation proportions
 
     Parameters
     -------
     sp_comps: pandas.DataFrame
             spinel compositions with column headings SiO2_Sp, MgO_Sp etc.
 
@@ -1761,145 +2422,210 @@
         This is used for rapid matrix division for
         pre-processing of data for cation fractions etc
 
     Returns
     -------
     pandas DataFrame
         cation proportions for spinel with column headings of the form... Sp_cat_prop
-    
+
     """
 
-    cation_num_sp = {'SiO2_Sp': 1, 'MgO_Sp': 1, 'FeOt_Sp': 1, 'CaO_Sp': 1, 'Al2O3_Sp': 2, 'Na2O_Sp': 2, 'K2O_Sp': 2, 'MnO_Sp': 1, 'TiO2_Sp': 1, 'Cr2O3_Sp': 2, 'P2O5_Sp': 2}
-    cation_num_sp_df = pd.DataFrame.from_dict(cation_num_sp, orient='index').T
-    cation_num_sp_df['Sample_ID_Sp'] = 'CatNum'
-    cation_num_sp_df.set_index('Sample_ID_Sp', inplace=True)
-
-    oxide_mass_sp = {'SiO2_Sp': 60.0843, 'MgO_Sp': 40.3044, 'FeOt_Sp': 71.8464, 'CaO_Sp': 56.0774,'Al2O3_Sp': 101.961, 'Na2O_Sp': 61.9789, 'K2O_Sp': 94.196, 'MnO_Sp': 70.9375, 'TiO2_Sp': 79.7877, 'Cr2O3_Sp': 151.9982, 'P2O5_Sp': 141.937}
-    oxide_mass_sp_df = pd.DataFrame.from_dict(oxide_mass_sp, orient='index').T
-    oxide_mass_sp_df['Sample_ID_Sp'] = 'MolWt'
-    oxide_mass_sp_df.set_index('Sample_ID_Sp', inplace=True)
+    cation_num_sp = {
+        "SiO2_Sp": 1,
+        "MgO_Sp": 1,
+        "FeOt_Sp": 1,
+        "CaO_Sp": 1,
+        "Al2O3_Sp": 2,
+        "Na2O_Sp": 2,
+        "K2O_Sp": 2,
+        "MnO_Sp": 1,
+        "TiO2_Sp": 1,
+        "Cr2O3_Sp": 2,
+        "P2O5_Sp": 2,
+    }
+    cation_num_sp_df = pd.DataFrame.from_dict(cation_num_sp, orient="index").T
+    cation_num_sp_df["Sample_ID_Sp"] = "CatNum"
+    cation_num_sp_df.set_index("Sample_ID_Sp", inplace=True)
+
+    oxide_mass_sp = {
+        "SiO2_Sp": 60.0843,
+        "MgO_Sp": 40.3044,
+        "FeOt_Sp": 71.8464,
+        "CaO_Sp": 56.0774,
+        "Al2O3_Sp": 101.961,
+        "Na2O_Sp": 61.9789,
+        "K2O_Sp": 94.196,
+        "MnO_Sp": 70.9375,
+        "TiO2_Sp": 79.7877,
+        "Cr2O3_Sp": 151.9982,
+        "P2O5_Sp": 141.937,
+    }
+    oxide_mass_sp_df = pd.DataFrame.from_dict(oxide_mass_sp, orient="index").T
+    oxide_mass_sp_df["Sample_ID_Sp"] = "MolWt"
+    oxide_mass_sp_df.set_index("Sample_ID_Sp", inplace=True)
 
     sp_prop_no_cat_num = calculate_mol_proportions_spinel(sp_comps=sp_comps)
-    sp_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in sp_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_sp_df.reindex(oxide_mass_sp_df.columns, axis=1).fillna(0)
+    sp_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in sp_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_sp_df.reindex(oxide_mass_sp_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, sp_prop_no_cat_num])
-    cation_prop_anhyd = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+    cation_prop_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
     cation_prop_anhyd.columns = [
-        str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
 
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Sp_cat_prop': 'Si_Sp_cat_prop',
-                            'TiO2_Sp_cat_prop': 'Ti_Sp_cat_prop',
-                            'Al2O3_Sp_cat_prop': 'Al_Sp_cat_prop',
-                            'FeOt_Sp_cat_prop': 'Fet_Sp_cat_prop',
-                            'MnO_Sp_cat_prop': 'Mn_Sp_cat_prop',
-                            'MgO_Sp_cat_prop': 'Mg_Sp_cat_prop',
-                            'CaO_Sp_cat_prop': 'Ca_Sp_cat_prop',
-                            'Na2O_Sp_cat_prop': 'Na_Sp_cat_prop',
-                            'K2O_Sp_cat_prop': 'K_Sp_cat_prop',
-                            'Cr2O3_Sp_cat_prop': 'Cr_Sp_cat_prop',
-                            'P2O5_Sp_cat_prop': 'P_Sp_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Sp_cat_prop": "Si_Sp_cat_prop",
+                "TiO2_Sp_cat_prop": "Ti_Sp_cat_prop",
+                "Al2O3_Sp_cat_prop": "Al_Sp_cat_prop",
+                "FeOt_Sp_cat_prop": "Fet_Sp_cat_prop",
+                "MnO_Sp_cat_prop": "Mn_Sp_cat_prop",
+                "MgO_Sp_cat_prop": "Mg_Sp_cat_prop",
+                "CaO_Sp_cat_prop": "Ca_Sp_cat_prop",
+                "Na2O_Sp_cat_prop": "Na_Sp_cat_prop",
+                "K2O_Sp_cat_prop": "K_Sp_cat_prop",
+                "Cr2O3_Sp_cat_prop": "Cr_Sp_cat_prop",
+                "P2O5_Sp_cat_prop": "P_Sp_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
-def calculate_oxygens_spinel(sp_comps):
 
+def calculate_oxygens_spinel(sp_comps):
     """
-    
-    Import spinel compositions using sp_comps=My_Sps, returns number of oxygens 
+
+    Import spinel compositions using sp_comps=My_Sps, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     sp_comps: pandas.DataFrame
         spinel compositions with column headings SiO2_Sp, MgO_Sp etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Sp_ox
 
     """
 
-    oxygen_num_sp = {'SiO2_Sp': 2, 'MgO_Sp': 1, 'FeOt_Sp': 1, 'CaO_Sp': 1, 'Al2O3_Sp': 3, 'Na2O_Sp': 1, 'K2O_Sp': 1, 'MnO_Sp': 1, 'TiO2_Sp': 2, 'Cr2O3_Sp': 3, 'P2O5_Sp': 5}
-    oxygen_num_sp_df = pd.DataFrame.from_dict(oxygen_num_sp, orient='index').T
-    oxygen_num_sp_df['Sample_ID_Sp'] = 'OxNum'
-    oxygen_num_sp_df.set_index('Sample_ID_Sp', inplace=True)
+    oxygen_num_sp = {
+        "SiO2_Sp": 2,
+        "MgO_Sp": 1,
+        "FeOt_Sp": 1,
+        "CaO_Sp": 1,
+        "Al2O3_Sp": 3,
+        "Na2O_Sp": 1,
+        "K2O_Sp": 1,
+        "MnO_Sp": 1,
+        "TiO2_Sp": 2,
+        "Cr2O3_Sp": 3,
+        "P2O5_Sp": 5,
+    }
+    oxygen_num_sp_df = pd.DataFrame.from_dict(oxygen_num_sp, orient="index").T
+    oxygen_num_sp_df["Sample_ID_Sp"] = "OxNum"
+    oxygen_num_sp_df.set_index("Sample_ID_Sp", inplace=True)
 
     mol_prop = calculate_mol_proportions_spinel(sp_comps=sp_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_sp_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
-def calculate_4oxygens_spinel(sp_comps):
 
+def calculate_4oxygens_spinel(sp_comps):
     """
-    
+
     Import spinel compositions using sp_comps=My_Sps, returns cations on the basis of 4 oxygens.
 
     Parameters
     -------
     sp_comps: pandas.DataFrame
         spinel compositions with column headings SiO2_Sp, MgO_Sp etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 4 oxygens, with column headings of the form... Sp_cat_4ox.
 
     """
 
-    cation_num_sp = {'SiO2_Sp': 1, 'MgO_Sp': 1, 'FeOt_Sp': 1, 'CaO_Sp': 1, 'Al2O3_Sp': 2, 'Na2O_Sp': 2, 'K2O_Sp': 2, 'MnO_Sp': 1, 'TiO2_Sp': 1, 'Cr2O3_Sp': 2, 'P2O5_Sp': 2}
-    cation_num_sp_df = pd.DataFrame.from_dict(cation_num_sp, orient='index').T
-    cation_num_sp_df['Sample_ID_Sp'] = 'CatNum'
-    cation_num_sp_df.set_index('Sample_ID_Sp', inplace=True)
+    cation_num_sp = {
+        "SiO2_Sp": 1,
+        "MgO_Sp": 1,
+        "FeOt_Sp": 1,
+        "CaO_Sp": 1,
+        "Al2O3_Sp": 2,
+        "Na2O_Sp": 2,
+        "K2O_Sp": 2,
+        "MnO_Sp": 1,
+        "TiO2_Sp": 1,
+        "Cr2O3_Sp": 2,
+        "P2O5_Sp": 2,
+    }
+    cation_num_sp_df = pd.DataFrame.from_dict(cation_num_sp, orient="index").T
+    cation_num_sp_df["Sample_ID_Sp"] = "CatNum"
+    cation_num_sp_df.set_index("Sample_ID_Sp", inplace=True)
 
     oxygens = calculate_oxygens_spinel(sp_comps=sp_comps)
-    renorm_factor = 4 / (oxygens.sum(axis='columns'))
+    renorm_factor = 4 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_spinel(sp_comps=sp_comps)
-    mol_prop['oxy_renorm_factor_sp'] = renorm_factor
-    mol_prop_4 = mol_prop.multiply(mol_prop['oxy_renorm_factor_sp'], axis='rows')
-    mol_prop_4.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_4.columns]
+    mol_prop["oxy_renorm_factor_sp"] = renorm_factor
+    mol_prop_4 = mol_prop.multiply(mol_prop["oxy_renorm_factor_sp"], axis="rows")
+    mol_prop_4.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_4.columns
+    ]
 
     ox_num_reindex = cation_num_sp_df.reindex(mol_prop_4.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_4])
     cation_4 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_4.columns = [str(col).replace('_mol_prop', '_cat_4ox')
-                        for col in mol_prop.columns]
-
-    cation_4_2=cation_4.rename(columns={
-                            'SiO2_Sp_cat_4ox': 'Si_Sp_cat_4ox',
-                            'TiO2_Sp_cat_4ox': 'Ti_Sp_cat_4ox',
-                            'Al2O3_Sp_cat_4ox': 'Al_Sp_cat_4ox',
-                            'FeOt_Sp_cat_4ox': 'Fet_Sp_cat_4ox',
-                            'MnO_Sp_cat_4ox': 'Mn_Sp_cat_4ox',
-                            'MgO_Sp_cat_4ox': 'Mg_Sp_cat_4ox',
-                            'CaO_Sp_cat_4ox': 'Ca_Sp_cat_4ox',
-                            'Na2O_Sp_cat_4ox': 'Na_Sp_cat_4ox',
-                            'K2O_Sp_cat_4ox': 'K_Sp_cat_4ox',
-                            'Cr2O3_Sp_cat_4ox': 'Cr_Sp_cat_4ox',
-                            'P2O5_Sp_cat_4ox': 'P_Sp_cat_4ox', })
+    cation_4.columns = [
+        str(col).replace("_mol_prop", "_cat_4ox") for col in mol_prop.columns
+    ]
+
+    cation_4_2 = cation_4.rename(
+        columns={
+            "SiO2_Sp_cat_4ox": "Si_Sp_cat_4ox",
+            "TiO2_Sp_cat_4ox": "Ti_Sp_cat_4ox",
+            "Al2O3_Sp_cat_4ox": "Al_Sp_cat_4ox",
+            "FeOt_Sp_cat_4ox": "Fet_Sp_cat_4ox",
+            "MnO_Sp_cat_4ox": "Mn_Sp_cat_4ox",
+            "MgO_Sp_cat_4ox": "Mg_Sp_cat_4ox",
+            "CaO_Sp_cat_4ox": "Ca_Sp_cat_4ox",
+            "Na2O_Sp_cat_4ox": "Na_Sp_cat_4ox",
+            "K2O_Sp_cat_4ox": "K_Sp_cat_4ox",
+            "Cr2O3_Sp_cat_4ox": "Cr_Sp_cat_4ox",
+            "P2O5_Sp_cat_4ox": "P_Sp_cat_4ox",
+        }
+    )
 
     return cation_4_2
 
-def calculate_spinel_components(sp_comps, append):
 
+def calculate_spinel_components(sp_comps, append):
     """
-    
+
     Import spinel compositions using sp_comps=My_Sps, returns components on the basis of 4 oxygens.
 
     Parameters
     -------
     sp_comps: pandas.DataFrame
         spinel compositions with column headings SiO2_Sp, MgO_Sp etc.
 
@@ -1907,315 +2633,438 @@
     -------
     pandas DataFrame
         components on the basis of 4 oxygens, with column headings of the form... Sp_cat_4ox.
 
     """
 
     sp_comps_new = sp_comps.copy()
-    sp_comps_new.columns = [col.replace(append, '_Sp') for col in sp_comps_new.columns]
+    sp_comps_new.columns = [col.replace(append, "_Sp") for col in sp_comps_new.columns]
     sp_comps = sp_comps_new.copy()
 
     sp_calc = calculate_4oxygens_spinel(sp_comps=sp_comps)
-    sp_calc['Sp_Cation_Sum'] = (sp_calc['Si_Sp_cat_4ox']+sp_calc['Ti_Sp_cat_4ox']+sp_calc['Al_Sp_cat_4ox']+sp_calc['Fet_Sp_cat_4ox']+sp_calc['Mn_Sp_cat_4ox']+sp_calc['Mg_Sp_cat_4ox']+sp_calc['Ca_Sp_cat_4ox']+sp_calc['Na_Sp_cat_4ox']+sp_calc['K_Sp_cat_4ox']+sp_calc['Cr_Sp_cat_4ox']+sp_calc['P_Sp_cat_4ox'])
-
-    sp_calc['Mg_Fe_M_Sp'] = sp_calc['Mg_Sp_cat_4ox'] + sp_calc['Fet_Sp_cat_4ox']
-    sp_calc['Al_B_Sp'] = sp_calc['Al_Sp_cat_4ox']
-    sp_calc['Mg_Fe_Mn_M_Sp'] = sp_calc['Mg_Sp_cat_4ox'] + sp_calc['Fet_Sp_cat_4ox'] + sp_calc['Mn_Sp_cat_4ox']
-    sp_calc['Al_Ti_Cr_B_Sp'] = sp_calc['Al_Sp_cat_4ox'] + sp_calc['Ti_Sp_cat_4ox'] + sp_calc['Cr_Sp_cat_4ox']
-
-    sp_calc['Fe_Ti_Ox'] = sp_calc['Fet_Sp_cat_4ox'] +  sp_calc['Ti_Sp_cat_4ox']
-    sp_calc['Fe_Mg_Mn_A_Ox'] = sp_calc['Fet_Sp_cat_4ox'] + sp_calc['Mg_Sp_cat_4ox'] + sp_calc['Mn_Sp_cat_4ox']
-    sp_calc['Ti_B_Ox'] = sp_calc['Ti_Sp_cat_4ox'] 
+    sp_calc["Sp_Cation_Sum"] = (
+        sp_calc["Si_Sp_cat_4ox"]
+        + sp_calc["Ti_Sp_cat_4ox"]
+        + sp_calc["Al_Sp_cat_4ox"]
+        + sp_calc["Fet_Sp_cat_4ox"]
+        + sp_calc["Mn_Sp_cat_4ox"]
+        + sp_calc["Mg_Sp_cat_4ox"]
+        + sp_calc["Ca_Sp_cat_4ox"]
+        + sp_calc["Na_Sp_cat_4ox"]
+        + sp_calc["K_Sp_cat_4ox"]
+        + sp_calc["Cr_Sp_cat_4ox"]
+        + sp_calc["P_Sp_cat_4ox"]
+    )
+
+    sp_calc["Mg_Fe_M_Sp"] = sp_calc["Mg_Sp_cat_4ox"] + sp_calc["Fet_Sp_cat_4ox"]
+    sp_calc["Al_B_Sp"] = sp_calc["Al_Sp_cat_4ox"]
+    sp_calc["Mg_Fe_Mn_M_Sp"] = (
+        sp_calc["Mg_Sp_cat_4ox"] + sp_calc["Fet_Sp_cat_4ox"] + sp_calc["Mn_Sp_cat_4ox"]
+    )
+    sp_calc["Al_Ti_Cr_B_Sp"] = (
+        sp_calc["Al_Sp_cat_4ox"] + sp_calc["Ti_Sp_cat_4ox"] + sp_calc["Cr_Sp_cat_4ox"]
+    )
+
+    sp_calc["Fe_Ti_Ox"] = sp_calc["Fet_Sp_cat_4ox"] + sp_calc["Ti_Sp_cat_4ox"]
+    sp_calc["Fe_Mg_Mn_A_Ox"] = (
+        sp_calc["Fet_Sp_cat_4ox"] + sp_calc["Mg_Sp_cat_4ox"] + sp_calc["Mn_Sp_cat_4ox"]
+    )
+    sp_calc["Ti_B_Ox"] = sp_calc["Ti_Sp_cat_4ox"]
 
     cat_prop = calculate_cat_proportions_spinel(sp_comps=sp_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([sp_comps, sp_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-# %% APATITE 
+# %% APATITE
 
 
 def calculate_mol_proportions_apatite(ap_comps):
-
     """
-    
+
     Import Apatite compositions using ap_comps=My_Apatites, returns mole proportions
 
     Parameters
     -------
     ap_comps: pandas.DataFrame
             Panda DataFrame of apatite compositions with column headings SiO2_Ap, MgO_Ap etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for apatites with column headings of the form SiO2_Ap_mol_prop
 
     """
 
-    oxide_mass_ap = {'SiO2_Ap': 60.0843, 'MgO_Ap': 40.3044, 'FeOt_Ap': 71.8464, 'CaO_Ap': 56.0774, 'Al2O3_Ap': 101.961, 'Na2O_Ap': 61.9789, 'K2O_Ap': 94.196, 'MnO_Ap': 70.9375, 'TiO2_Ap': 79.7877, 'Cr2O3_Ap': 151.9982, 'P2O5_Ap': 141.937}
-    oxide_mass_ap_df = pd.DataFrame.from_dict(oxide_mass_ap, orient='index').T
-    oxide_mass_ap_df['Sample_ID_Ap'] = 'MolWt'
-    oxide_mass_ap_df.set_index('Sample_ID_Ap', inplace=True)
+    oxide_mass_ap = {
+        "SiO2_Ap": 60.0843,
+        "MgO_Ap": 40.3044,
+        "FeOt_Ap": 71.8464,
+        "CaO_Ap": 56.0774,
+        "Al2O3_Ap": 101.961,
+        "Na2O_Ap": 61.9789,
+        "K2O_Ap": 94.196,
+        "MnO_Ap": 70.9375,
+        "TiO2_Ap": 79.7877,
+        "Cr2O3_Ap": 151.9982,
+        "P2O5_Ap": 141.937,
+    }
+    oxide_mass_ap_df = pd.DataFrame.from_dict(oxide_mass_ap, orient="index").T
+    oxide_mass_ap_df["Sample_ID_Ap"] = "MolWt"
+    oxide_mass_ap_df.set_index("Sample_ID_Ap", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     ap_wt = ap_comps.reindex(oxide_mass_ap_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    ap_wt_combo = pd.concat([oxide_mass_ap_df, ap_wt],)
+    ap_wt_combo = pd.concat(
+        [oxide_mass_ap_df, ap_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = ap_wt_combo.div(
-        ap_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = ap_wt_combo.div(ap_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
+
 def calculate_cat_proportions_apatite(*, ap_comps=None, oxide_headers=False):
-    
     """
-    
+
     Import apatite compositions using ap_comps=My_Apatites, returns cation proportions
 
     Parameters
     -------
     ap_comps: pandas.DataFrame
             apatite compositions with column headings SiO2_Ap, MgO_Ap etc.
-    
+
     oxide_headers: bool
         default=False, returns as Ti_Ap_cat_prop.
         =True returns Ti_Ap_cat_prop.
         This is used for rapid matrix division for
         pre-processing of data for cation fractions etc
 
     Returns
     -------
     pandas DataFrame
         cation proportions for apatite with column headings of the form... Ap_cat_prop
-    
-    """
 
-    cation_num_ap = {'SiO2_Ap': 1, 'MgO_Ap': 1, 'FeOt_Ap': 1, 'CaO_Ap': 1, 'Al2O3_Ap': 2, 'Na2O_Ap': 2,
-                   'K2O_Ap': 2, 'MnO_Ap': 1, 'TiO2_Ap': 1, 'Cr2O3_Ap': 2, 'P2O5_Ap': 2}
-    cation_num_ap_df = pd.DataFrame.from_dict(cation_num_ap, orient='index').T
-    cation_num_ap_df['Sample_ID_Ap'] = 'CatNum'
-    cation_num_ap_df.set_index('Sample_ID_Ap', inplace=True)
-
-    oxide_mass_ap = {'SiO2_Ap': 60.0843, 'MgO_Ap': 40.3044, 'FeOt_Ap': 71.8464, 'CaO_Ap': 56.0774,'Al2O3_Ap': 101.961, 'Na2O_Ap': 61.9789, 'K2O_Ap': 94.196, 'MnO_Ap': 70.9375, 'TiO2_Ap': 79.7877, 'Cr2O3_Ap': 151.9982, 'P2O5_Ap': 141.937}
+    """
 
-    oxide_mass_ap_df = pd.DataFrame.from_dict(oxide_mass_ap, orient='index').T
-    oxide_mass_ap_df['Sample_ID_Ap'] = 'MolWt'
-    oxide_mass_ap_df.set_index('Sample_ID_Ap', inplace=True)
+    cation_num_ap = {
+        "SiO2_Ap": 1,
+        "MgO_Ap": 1,
+        "FeOt_Ap": 1,
+        "CaO_Ap": 1,
+        "Al2O3_Ap": 2,
+        "Na2O_Ap": 2,
+        "K2O_Ap": 2,
+        "MnO_Ap": 1,
+        "TiO2_Ap": 1,
+        "Cr2O3_Ap": 2,
+        "P2O5_Ap": 2,
+    }
+    cation_num_ap_df = pd.DataFrame.from_dict(cation_num_ap, orient="index").T
+    cation_num_ap_df["Sample_ID_Ap"] = "CatNum"
+    cation_num_ap_df.set_index("Sample_ID_Ap", inplace=True)
+
+    oxide_mass_ap = {
+        "SiO2_Ap": 60.0843,
+        "MgO_Ap": 40.3044,
+        "FeOt_Ap": 71.8464,
+        "CaO_Ap": 56.0774,
+        "Al2O3_Ap": 101.961,
+        "Na2O_Ap": 61.9789,
+        "K2O_Ap": 94.196,
+        "MnO_Ap": 70.9375,
+        "TiO2_Ap": 79.7877,
+        "Cr2O3_Ap": 151.9982,
+        "P2O5_Ap": 141.937,
+    }
+
+    oxide_mass_ap_df = pd.DataFrame.from_dict(oxide_mass_ap, orient="index").T
+    oxide_mass_ap_df["Sample_ID_Ap"] = "MolWt"
+    oxide_mass_ap_df.set_index("Sample_ID_Ap", inplace=True)
 
     ap_prop_no_cat_num = calculate_mol_proportions_apatite(ap_comps=ap_comps)
-    ap_prop_no_cat_num.columns = [str(col).replace(
-        '_mol_prop', '') for col in ap_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_ap_df.reindex(oxide_mass_ap_df.columns, axis=1).fillna(0)
+    ap_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in ap_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_ap_df.reindex(oxide_mass_ap_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, ap_prop_no_cat_num])
     cation_prop_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Ap_cat_prop': 'Si_Ap_cat_prop',
-                            'TiO2_Ap_cat_prop': 'Ti_Ap_cat_prop',
-                            'Al2O3_Ap_cat_prop': 'Al_Ap_cat_prop',
-                            'FeOt_Ap_cat_prop': 'Fet_Ap_cat_prop',
-                            'MnO_Ap_cat_prop': 'Mn_Ap_cat_prop',
-                            'MgO_Ap_cat_prop': 'Mg_Ap_cat_prop',
-                            'CaO_Ap_cat_prop': 'Ca_Ap_cat_prop',
-                            'Na2O_Ap_cat_prop': 'Na_Ap_cat_prop',
-                            'K2O_Ap_cat_prop': 'K_Ap_cat_prop',
-                            'Cr2O3_Ap_cat_prop': 'Cr_Ap_cat_prop',
-                            'P2O5_Ap_cat_prop': 'P_Ap_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Ap_cat_prop": "Si_Ap_cat_prop",
+                "TiO2_Ap_cat_prop": "Ti_Ap_cat_prop",
+                "Al2O3_Ap_cat_prop": "Al_Ap_cat_prop",
+                "FeOt_Ap_cat_prop": "Fet_Ap_cat_prop",
+                "MnO_Ap_cat_prop": "Mn_Ap_cat_prop",
+                "MgO_Ap_cat_prop": "Mg_Ap_cat_prop",
+                "CaO_Ap_cat_prop": "Ca_Ap_cat_prop",
+                "Na2O_Ap_cat_prop": "Na_Ap_cat_prop",
+                "K2O_Ap_cat_prop": "K_Ap_cat_prop",
+                "Cr2O3_Ap_cat_prop": "Cr_Ap_cat_prop",
+                "P2O5_Ap_cat_prop": "P_Ap_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
+
 def calculate_oxygens_apatite(ap_comps):
-    
     """
-    
-    Import apatite compositions using ap_comps=My_Aps, returns number of oxygens 
+
+    Import apatite compositions using ap_comps=My_Aps, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     ap_comps: pandas.DataFrame
         apatite compositions with column headings SiO2_Ap, MgO_Ap etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Ap_ox
-    
+
     """
 
-    oxygen_num_ap = {'SiO2_Ap': 2, 'MgO_Ap': 1, 'FeOt_Ap': 1, 'CaO_Ap': 1, 'Al2O3_Ap': 3, 'Na2O_Ap': 1, 'K2O_Ap': 1, 'MnO_Ap': 1, 'TiO2_Ap': 2, 'Cr2O3_Ap': 3, 'P2O5_Ap': 5}
-    oxygen_num_ap_df = pd.DataFrame.from_dict(oxygen_num_ap, orient='index').T
-    oxygen_num_ap_df['Sample_ID_Ap'] = 'OxNum'
-    oxygen_num_ap_df.set_index('Sample_ID_Ap', inplace=True)
+    oxygen_num_ap = {
+        "SiO2_Ap": 2,
+        "MgO_Ap": 1,
+        "FeOt_Ap": 1,
+        "CaO_Ap": 1,
+        "Al2O3_Ap": 3,
+        "Na2O_Ap": 1,
+        "K2O_Ap": 1,
+        "MnO_Ap": 1,
+        "TiO2_Ap": 2,
+        "Cr2O3_Ap": 3,
+        "P2O5_Ap": 5,
+    }
+    oxygen_num_ap_df = pd.DataFrame.from_dict(oxygen_num_ap, orient="index").T
+    oxygen_num_ap_df["Sample_ID_Ap"] = "OxNum"
+    oxygen_num_ap_df.set_index("Sample_ID_Ap", inplace=True)
 
     mol_prop = calculate_mol_proportions_apatite(ap_comps=ap_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
-    ox_num_reindex = oxygen_num_ap_df.reindex(
-        mol_prop.columns, axis=1).fillna(0)
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
+    ox_num_reindex = oxygen_num_ap_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
     oxygens_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
-def calculate_12oxygens_apatite(ap_comps):
 
+def calculate_12oxygens_apatite(ap_comps):
     """
-    
+
     Import apatite compositions using ap_comps=My_Aps, returns cations on the basis of 12 oxygens.
 
     Parameters
     -------
     ap_comps: pandas.DataFrame
         apatite compositions with column headings SiO2_Ap, MgO_Ap etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 12 oxygens, with column headings of the form... Ap_cat_12ox.
-    
-    """
 
-    cation_num_ap = {'SiO2_Ap': 1, 'MgO_Ap': 1, 'FeOt_Ap': 1, 'CaO_Ap': 1, 'Al2O3_Ap': 2, 'Na2O_Ap': 2, 'K2O_Ap': 2, 'MnO_Ap': 1, 'TiO2_Ap': 1, 'Cr2O3_Ap': 2, 'P2O5_Ap': 2}
+    """
 
-    cation_num_ap_df = pd.DataFrame.from_dict(cation_num_ap, orient='index').T
-    cation_num_ap_df['Sample_ID_Ap'] = 'CatNum'
-    cation_num_ap_df.set_index('Sample_ID_Ap', inplace=True)
+    cation_num_ap = {
+        "SiO2_Ap": 1,
+        "MgO_Ap": 1,
+        "FeOt_Ap": 1,
+        "CaO_Ap": 1,
+        "Al2O3_Ap": 2,
+        "Na2O_Ap": 2,
+        "K2O_Ap": 2,
+        "MnO_Ap": 1,
+        "TiO2_Ap": 1,
+        "Cr2O3_Ap": 2,
+        "P2O5_Ap": 2,
+    }
+
+    cation_num_ap_df = pd.DataFrame.from_dict(cation_num_ap, orient="index").T
+    cation_num_ap_df["Sample_ID_Ap"] = "CatNum"
+    cation_num_ap_df.set_index("Sample_ID_Ap", inplace=True)
 
     oxygens = calculate_oxygens_apatite(ap_comps=ap_comps)
-    renorm_factor = 12 / (oxygens.sum(axis='columns'))
+    renorm_factor = 12 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_apatite(ap_comps=ap_comps)
-    mol_prop['oxy_renorm_factor_ap'] = renorm_factor
-    mol_prop_12 = mol_prop.multiply(mol_prop['oxy_renorm_factor_ap'], axis='rows')
-    mol_prop_12.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_12.columns]
+    mol_prop["oxy_renorm_factor_ap"] = renorm_factor
+    mol_prop_12 = mol_prop.multiply(mol_prop["oxy_renorm_factor_ap"], axis="rows")
+    mol_prop_12.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_12.columns
+    ]
 
     ox_num_reindex = cation_num_ap_df.reindex(mol_prop_12.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_12])
     cation_12 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_12.columns = [str(col).replace('_mol_prop', '_cat_12ox')
-                        for col in mol_prop.columns]
-
-    cation_12_2=cation_12.rename(columns={
-                            'SiO2_Ap_cat_12ox': 'Si_Ap_cat_12ox',
-                            'TiO2_Ap_cat_12ox': 'Ti_Ap_cat_12ox',
-                            'Al2O3_Ap_cat_12ox': 'Al_Ap_cat_12ox',
-                            'FeOt_Ap_cat_12ox': 'Fet_Ap_cat_12ox',
-                            'MnO_Ap_cat_12ox': 'Mn_Ap_cat_12ox',
-                            'MgO_Ap_cat_12ox': 'Mg_Ap_cat_12ox',
-                            'CaO_Ap_cat_12ox': 'Ca_Ap_cat_12ox',
-                            'Na2O_Ap_cat_12ox': 'Na_Ap_cat_12ox',
-                            'K2O_Ap_cat_12ox': 'K_Ap_cat_12ox',
-                            'Cr2O3_Ap_cat_12ox': 'Cr_Ap_cat_12ox',
-                            'P2O5_Ap_cat_12ox': 'P_Ap_cat_12ox',})
+    cation_12.columns = [
+        str(col).replace("_mol_prop", "_cat_12ox") for col in mol_prop.columns
+    ]
+
+    cation_12_2 = cation_12.rename(
+        columns={
+            "SiO2_Ap_cat_12ox": "Si_Ap_cat_12ox",
+            "TiO2_Ap_cat_12ox": "Ti_Ap_cat_12ox",
+            "Al2O3_Ap_cat_12ox": "Al_Ap_cat_12ox",
+            "FeOt_Ap_cat_12ox": "Fet_Ap_cat_12ox",
+            "MnO_Ap_cat_12ox": "Mn_Ap_cat_12ox",
+            "MgO_Ap_cat_12ox": "Mg_Ap_cat_12ox",
+            "CaO_Ap_cat_12ox": "Ca_Ap_cat_12ox",
+            "Na2O_Ap_cat_12ox": "Na_Ap_cat_12ox",
+            "K2O_Ap_cat_12ox": "K_Ap_cat_12ox",
+            "Cr2O3_Ap_cat_12ox": "Cr_Ap_cat_12ox",
+            "P2O5_Ap_cat_12ox": "P_Ap_cat_12ox",
+        }
+    )
 
     return cation_12_2
 
-def calculate_apatite_components(ap_comps, append):
 
+def calculate_apatite_components(ap_comps, append):
     """
-    
+
     Import apatite compositions using ap_comps=My_Aps, returns cations on the basis of 12 oxygens.
 
     Parameters
     -------
     ap_comps: pandas.DataFrame
         apatite compositions with column headings SiO2_Ap, MgO_Ap etc.
 
     Returns
     -------
     pandas DataFrame
         components on the basis of 12 oxygens, with column headings of the form... Ap_cat_12ox.
-    
+
     """
 
     ap_comps_new = ap_comps.copy()
-    ap_comps_new.columns = [col.replace(append, '_Ap') for col in ap_comps_new.columns]
+    ap_comps_new.columns = [col.replace(append, "_Ap") for col in ap_comps_new.columns]
     ap_comps = ap_comps_new.copy()
 
     ap_calc = calculate_12oxygens_apatite(ap_comps=ap_comps)
-    ap_calc['Ap_Cation_Sum'] = (ap_calc['Si_Ap_cat_12ox']+ap_calc['Ti_Ap_cat_12ox']+ap_calc['Al_Ap_cat_12ox']+ap_calc['Fet_Ap_cat_12ox']+ap_calc['Mn_Ap_cat_12ox']+ap_calc['Mg_Ap_cat_12ox']+ap_calc['Ca_Ap_cat_12ox']+ap_calc['Na_Ap_cat_12ox']+ap_calc['K_Ap_cat_12ox']+ap_calc['Cr_Ap_cat_12ox']+ap_calc['P_Ap_cat_12ox'])
+    ap_calc["Ap_Cation_Sum"] = (
+        ap_calc["Si_Ap_cat_12ox"]
+        + ap_calc["Ti_Ap_cat_12ox"]
+        + ap_calc["Al_Ap_cat_12ox"]
+        + ap_calc["Fet_Ap_cat_12ox"]
+        + ap_calc["Mn_Ap_cat_12ox"]
+        + ap_calc["Mg_Ap_cat_12ox"]
+        + ap_calc["Ca_Ap_cat_12ox"]
+        + ap_calc["Na_Ap_cat_12ox"]
+        + ap_calc["K_Ap_cat_12ox"]
+        + ap_calc["Cr_Ap_cat_12ox"]
+        + ap_calc["P_Ap_cat_12ox"]
+    )
 
-    # OH, F, Cl not always measured. 
+    # OH, F, Cl not always measured.
     # Ca and P as cations
-    ap_calc['Ca_P_Ap'] = ap_calc['Ca_Ap_cat_12ox'] + ap_calc['P_Ap_cat_12ox']
-    ap_calc['Ca_Mn_Na_M_Ap'] = ap_calc['Ca_Ap_cat_12ox'] + ap_calc['Mn_Ap_cat_12ox'] + ap_calc['Na_Ap_cat_12ox']
-    ap_calc['P_Si_T_Ap'] = ap_calc['P_Ap_cat_12ox'] + ap_calc['Si_Ap_cat_12ox']
+    ap_calc["Ca_P_Ap"] = ap_calc["Ca_Ap_cat_12ox"] + ap_calc["P_Ap_cat_12ox"]
+    ap_calc["Ca_Mn_Na_M_Ap"] = (
+        ap_calc["Ca_Ap_cat_12ox"]
+        + ap_calc["Mn_Ap_cat_12ox"]
+        + ap_calc["Na_Ap_cat_12ox"]
+    )
+    ap_calc["P_Si_T_Ap"] = ap_calc["P_Ap_cat_12ox"] + ap_calc["Si_Ap_cat_12ox"]
 
     cat_prop = calculate_cat_proportions_apatite(ap_comps=ap_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([ap_comps, ap_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-# %% GARNET 
+# %% GARNET
 
 
 def calculate_mol_proportions_garnet(gt_comps):
-
     """
-    
+
     Import Garnet compositions using gt_comps=My_Garnets, returns mole proportions
 
     Parameters
     -------
     gt_comps: pandas.DataFrame
             Panda DataFrame of garnet compositions with column headings SiO2_Gt, MgO_Gt etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for garnets with column headings of the form SiO2_Gt_mol_prop
-    
+
     """
 
-    oxide_mass_gt = {'SiO2_Gt': 60.0843, 'MgO_Gt': 40.3044, 'FeOt_Gt': 71.8464, 'CaO_Gt': 56.0774, 'Al2O3_Gt': 101.961, 'Na2O_Gt': 61.9789, 'K2O_Gt': 94.196, 'MnO_Gt': 70.9375, 'TiO2_Gt': 79.7877, 'Cr2O3_Gt': 151.9982, 'P2O5_Gt': 141.937, 'NiO_Gt': 74.6994}
-    oxide_mass_gt_df = pd.DataFrame.from_dict(oxide_mass_gt, orient='index').T
-    oxide_mass_gt_df['Sample_ID_Gt'] = 'MolWt'
-    oxide_mass_gt_df.set_index('Sample_ID_Gt', inplace=True)
+    oxide_mass_gt = {
+        "SiO2_Gt": 60.0843,
+        "MgO_Gt": 40.3044,
+        "FeOt_Gt": 71.8464,
+        "CaO_Gt": 56.0774,
+        "Al2O3_Gt": 101.961,
+        "Na2O_Gt": 61.9789,
+        "K2O_Gt": 94.196,
+        "MnO_Gt": 70.9375,
+        "TiO2_Gt": 79.7877,
+        "Cr2O3_Gt": 151.9982,
+        "P2O5_Gt": 141.937,
+        "NiO_Gt": 74.6994,
+    }
+    oxide_mass_gt_df = pd.DataFrame.from_dict(oxide_mass_gt, orient="index").T
+    oxide_mass_gt_df["Sample_ID_Gt"] = "MolWt"
+    oxide_mass_gt_df.set_index("Sample_ID_Gt", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     gt_wt = gt_comps.reindex(oxide_mass_gt_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    gt_wt_combo = pd.concat([oxide_mass_gt_df, gt_wt],)
+    gt_wt_combo = pd.concat(
+        [oxide_mass_gt_df, gt_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = gt_wt_combo.div(
-        gt_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
-    
+    mol_prop_anhyd = gt_wt_combo.div(gt_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
+
     return mol_prop_anhyd
 
 
 def calculate_cat_proportions_garnet(*, gt_comps=None, oxide_headers=False):
-
     """
-    
+
     Import garnet compositions using gt_comps=My_garnets, returns cation proportions
 
     Parameters
     -------
     gt_comps: pandas.DataFrame
             garnet compositions with column headings SiO2_Plag, MgO_Plag etc.
     oxide_headers: bool
@@ -2224,233 +3073,351 @@
         This is used for rapid matrix division for
         pre-processing of data for cation fractions etc
 
     Returns
     -------
     pandas DataFrame
         cation proportions for garnet with column headings of the form... Gt_cat_prop
-    
-    """
 
-    cation_num_gt = {'SiO2_Gt': 1, 'MgO_Gt': 1, 'FeOt_Gt': 1, 'CaO_Gt': 1, 'Al2O3_Gt': 2, 'Na2O_Gt': 2, 'K2O_Gt': 2, 'MnO_Gt': 1, 'TiO2_Gt': 1, 'Cr2O3_Gt': 2, 'P2O5_Gt': 2, 'NiO_Gt': 1}
-    cation_num_gt_df = pd.DataFrame.from_dict(cation_num_gt, orient='index').T
-    cation_num_gt_df['Sample_ID_Gt'] = 'CatNum'
-    cation_num_gt_df.set_index('Sample_ID_Gt', inplace=True)
-
-    oxide_mass_gt = {'SiO2_Gt': 60.0843, 'MgO_Gt': 40.3044, 'FeOt_Gt': 71.8464, 'CaO_Gt': 56.0774,'Al2O3_Gt': 101.961, 'Na2O_Gt': 61.9789, 'K2O_Gt': 94.196, 'MnO_Gt': 70.9375, 'TiO2_Gt': 79.7877, 'Cr2O3_Gt': 151.9982, 'P2O5_Gt': 141.937, 'NiO_Gt': 74.6994}
+    """
 
-    oxide_mass_gt_df = pd.DataFrame.from_dict(oxide_mass_gt, orient='index').T
-    oxide_mass_gt_df['Sample_ID_Gt'] = 'MolWt'
-    oxide_mass_gt_df.set_index('Sample_ID_Gt', inplace=True)
+    cation_num_gt = {
+        "SiO2_Gt": 1,
+        "MgO_Gt": 1,
+        "FeOt_Gt": 1,
+        "CaO_Gt": 1,
+        "Al2O3_Gt": 2,
+        "Na2O_Gt": 2,
+        "K2O_Gt": 2,
+        "MnO_Gt": 1,
+        "TiO2_Gt": 1,
+        "Cr2O3_Gt": 2,
+        "P2O5_Gt": 2,
+        "NiO_Gt": 1,
+    }
+    cation_num_gt_df = pd.DataFrame.from_dict(cation_num_gt, orient="index").T
+    cation_num_gt_df["Sample_ID_Gt"] = "CatNum"
+    cation_num_gt_df.set_index("Sample_ID_Gt", inplace=True)
+
+    oxide_mass_gt = {
+        "SiO2_Gt": 60.0843,
+        "MgO_Gt": 40.3044,
+        "FeOt_Gt": 71.8464,
+        "CaO_Gt": 56.0774,
+        "Al2O3_Gt": 101.961,
+        "Na2O_Gt": 61.9789,
+        "K2O_Gt": 94.196,
+        "MnO_Gt": 70.9375,
+        "TiO2_Gt": 79.7877,
+        "Cr2O3_Gt": 151.9982,
+        "P2O5_Gt": 141.937,
+        "NiO_Gt": 74.6994,
+    }
+
+    oxide_mass_gt_df = pd.DataFrame.from_dict(oxide_mass_gt, orient="index").T
+    oxide_mass_gt_df["Sample_ID_Gt"] = "MolWt"
+    oxide_mass_gt_df.set_index("Sample_ID_Gt", inplace=True)
 
     gt_prop_no_cat_num = calculate_mol_proportions_garnet(gt_comps=gt_comps)
-    gt_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in gt_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_gt_df.reindex(
-        oxide_mass_gt_df.columns, axis=1).fillna(0)
+    gt_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in gt_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_gt_df.reindex(oxide_mass_gt_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, gt_prop_no_cat_num])
     cation_prop_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Gt_cat_prop': 'Si_Gt_cat_prop',
-                            'TiO2_Gt_cat_prop': 'Ti_Gt_cat_prop',
-                            'Al2O3_Gt_cat_prop': 'Al_Gt_cat_prop',
-                            'FeOt_Gt_cat_prop': 'Fet_Gt_cat_prop',
-                            'MnO_Gt_cat_prop': 'Mn_Gt_cat_prop',
-                            'MgO_Gt_cat_prop': 'Mg_Gt_cat_prop',
-                            'CaO_Gt_cat_prop': 'Ca_Gt_cat_prop',
-                            'Na2O_Gt_cat_prop': 'Na_Gt_cat_prop',
-                            'K2O_Gt_cat_prop': 'K_Gt_cat_prop',
-                            'Cr2O3_Gt_cat_prop': 'Cr_Gt_cat_prop',
-                            'P2O5_Gt_cat_prop': 'P_Gt_cat_prop',
-                            'NiO_Gt_cat_prop': 'Ni_Gt_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Gt_cat_prop": "Si_Gt_cat_prop",
+                "TiO2_Gt_cat_prop": "Ti_Gt_cat_prop",
+                "Al2O3_Gt_cat_prop": "Al_Gt_cat_prop",
+                "FeOt_Gt_cat_prop": "Fet_Gt_cat_prop",
+                "MnO_Gt_cat_prop": "Mn_Gt_cat_prop",
+                "MgO_Gt_cat_prop": "Mg_Gt_cat_prop",
+                "CaO_Gt_cat_prop": "Ca_Gt_cat_prop",
+                "Na2O_Gt_cat_prop": "Na_Gt_cat_prop",
+                "K2O_Gt_cat_prop": "K_Gt_cat_prop",
+                "Cr2O3_Gt_cat_prop": "Cr_Gt_cat_prop",
+                "P2O5_Gt_cat_prop": "P_Gt_cat_prop",
+                "NiO_Gt_cat_prop": "Ni_Gt_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
+
 def calculate_oxygens_garnet(gt_comps):
-    
     """
-    
-    Import garnet compositions using gt_comps=My_Gts, returns number of oxygens 
+
+    Import garnet compositions using gt_comps=My_Gts, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     gt_comps: pandas.DataFrame
         garnet compositions with column headings SiO2_Gt, MgO_Gt etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Gt_ox
-    
+
     """
 
-    oxygen_num_gt = {'SiO2_Gt': 2, 'MgO_Gt': 1, 'FeOt_Gt': 1, 'CaO_Gt': 1, 'Al2O3_Gt': 3, 'Na2O_Gt': 1, 'K2O_Gt': 1, 'MnO_Gt': 1, 'TiO2_Gt': 2, 'Cr2O3_Gt': 3, 'P2O5_Gt': 5, 'NiO_Gt': 1}
-    oxygen_num_gt_df = pd.DataFrame.from_dict(oxygen_num_gt, orient='index').T
-    oxygen_num_gt_df['Sample_ID_Gt'] = 'OxNum'
-    oxygen_num_gt_df.set_index('Sample_ID_Gt', inplace=True)
+    oxygen_num_gt = {
+        "SiO2_Gt": 2,
+        "MgO_Gt": 1,
+        "FeOt_Gt": 1,
+        "CaO_Gt": 1,
+        "Al2O3_Gt": 3,
+        "Na2O_Gt": 1,
+        "K2O_Gt": 1,
+        "MnO_Gt": 1,
+        "TiO2_Gt": 2,
+        "Cr2O3_Gt": 3,
+        "P2O5_Gt": 5,
+        "NiO_Gt": 1,
+    }
+    oxygen_num_gt_df = pd.DataFrame.from_dict(oxygen_num_gt, orient="index").T
+    oxygen_num_gt_df["Sample_ID_Gt"] = "OxNum"
+    oxygen_num_gt_df.set_index("Sample_ID_Gt", inplace=True)
 
     mol_prop = calculate_mol_proportions_garnet(gt_comps=gt_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_gt_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
     oxygens_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
-def calculate_12oxygens_garnet(gt_comps):
 
+def calculate_12oxygens_garnet(gt_comps):
     """
-    
+
     Import garnet compositions using gt_comps=My_Gts, returns cations on the basis of 4 oxygens.
 
     Parameters
     -------
     gt_comps: pandas.DataFrame
         garnet compositions with column headings SiO2_Gt, MgO_Gt etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 12 oxygens, with column headings of the form... Gt_cat_12ox.
-    
-    """
 
-    cation_num_gt = {'SiO2_Gt': 1, 'MgO_Gt': 1, 'FeOt_Gt': 1, 'CaO_Gt': 1, 'Al2O3_Gt': 2, 'Na2O_Gt': 2, 'K2O_Gt': 2, 'MnO_Gt': 1, 'TiO2_Gt': 1, 'Cr2O3_Gt': 2, 'P2O5_Gt': 2, 'NiO_Gt': 1}
+    """
 
-    cation_num_gt_df = pd.DataFrame.from_dict(cation_num_gt, orient='index').T
-    cation_num_gt_df['Sample_ID_Gt'] = 'CatNum'
-    cation_num_gt_df.set_index('Sample_ID_Gt', inplace=True)
+    cation_num_gt = {
+        "SiO2_Gt": 1,
+        "MgO_Gt": 1,
+        "FeOt_Gt": 1,
+        "CaO_Gt": 1,
+        "Al2O3_Gt": 2,
+        "Na2O_Gt": 2,
+        "K2O_Gt": 2,
+        "MnO_Gt": 1,
+        "TiO2_Gt": 1,
+        "Cr2O3_Gt": 2,
+        "P2O5_Gt": 2,
+        "NiO_Gt": 1,
+    }
+
+    cation_num_gt_df = pd.DataFrame.from_dict(cation_num_gt, orient="index").T
+    cation_num_gt_df["Sample_ID_Gt"] = "CatNum"
+    cation_num_gt_df.set_index("Sample_ID_Gt", inplace=True)
 
     oxygens = calculate_oxygens_garnet(gt_comps=gt_comps)
-    renorm_factor = 12 / (oxygens.sum(axis='columns'))
+    renorm_factor = 12 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_garnet(gt_comps=gt_comps)
-    mol_prop['oxy_renorm_factor_gt'] = renorm_factor
-    mol_prop_12 = mol_prop.multiply(mol_prop['oxy_renorm_factor_gt'], axis='rows')
-    mol_prop_12.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_12.columns]
+    mol_prop["oxy_renorm_factor_gt"] = renorm_factor
+    mol_prop_12 = mol_prop.multiply(mol_prop["oxy_renorm_factor_gt"], axis="rows")
+    mol_prop_12.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_12.columns
+    ]
 
     ox_num_reindex = cation_num_gt_df.reindex(mol_prop_12.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_12])
     cation_12 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_12.columns = [str(col).replace('_mol_prop', '_cat_12ox')
-                        for col in mol_prop.columns]
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_12_2=cation_12.rename(columns={
-                            'SiO2_Gt_cat_12ox': 'Si_Gt_cat_12ox',
-                            'TiO2_Gt_cat_12ox': 'Ti_Gt_cat_12ox',
-                            'Al2O3_Gt_cat_12ox': 'Al_Gt_cat_12ox',
-                            'FeOt_Gt_cat_12ox': 'Fet_Gt_cat_12ox',
-                            'MnO_Gt_cat_12ox': 'Mn_Gt_cat_12ox',
-                            'MgO_Gt_cat_12ox': 'Mg_Gt_cat_12ox',
-                            'CaO_Gt_cat_12ox': 'Ca_Gt_cat_12ox',
-                            'Na2O_Gt_cat_12ox': 'Na_Gt_cat_12ox',
-                            'K2O_Gt_cat_12ox': 'K_Gt_cat_12ox',
-                            'Cr2O3_Gt_cat_12ox': 'Cr_Gt_cat_12ox',
-                            'P2O5_Gt_cat_12ox': 'P_Gt_cat_12ox',
-                            'NiO_Gt_cat_12ox': 'Ni_Gt_cat_12ox',})
+    cation_12.columns = [
+        str(col).replace("_mol_prop", "_cat_12ox") for col in mol_prop.columns
+    ]
+
+    cation_12_2 = cation_12.rename(
+        columns={
+            "SiO2_Gt_cat_12ox": "Si_Gt_cat_12ox",
+            "TiO2_Gt_cat_12ox": "Ti_Gt_cat_12ox",
+            "Al2O3_Gt_cat_12ox": "Al_Gt_cat_12ox",
+            "FeOt_Gt_cat_12ox": "Fet_Gt_cat_12ox",
+            "MnO_Gt_cat_12ox": "Mn_Gt_cat_12ox",
+            "MgO_Gt_cat_12ox": "Mg_Gt_cat_12ox",
+            "CaO_Gt_cat_12ox": "Ca_Gt_cat_12ox",
+            "Na2O_Gt_cat_12ox": "Na_Gt_cat_12ox",
+            "K2O_Gt_cat_12ox": "K_Gt_cat_12ox",
+            "Cr2O3_Gt_cat_12ox": "Cr_Gt_cat_12ox",
+            "P2O5_Gt_cat_12ox": "P_Gt_cat_12ox",
+            "NiO_Gt_cat_12ox": "Ni_Gt_cat_12ox",
+        }
+    )
 
     return cation_12_2
 
 
 def calculate_garnet_components(gt_comps, append):
-
     """
-    
+
     Import garnet compositions using gt_comps=My_Gts, returns cations on the basis of 12 oxygens.
 
     Parameters
     -------
     gt_comps: pandas.DataFrame
         garnet compositions with column headings SiO2_Gt, MgO_Gt etc.
 
     Returns
     -------
     pandas DataFrame
         components on the basis of 12 oxygens, with column headings of the form... Gt_cat_12ox.
-    
+
     """
 
     gt_comps_new = gt_comps.copy()
-    gt_comps_new.columns = [col.replace(append, '_Gt') for col in gt_comps_new.columns]
+    gt_comps_new.columns = [col.replace(append, "_Gt") for col in gt_comps_new.columns]
     gt_comps = gt_comps_new.copy()
 
     gt_calc = calculate_12oxygens_garnet(gt_comps=gt_comps)
-    gt_calc['Gt_Cation_Sum'] = (gt_calc['Si_Gt_cat_12ox']+gt_calc['Ti_Gt_cat_12ox']+gt_calc['Al_Gt_cat_12ox']+gt_calc['Fet_Gt_cat_12ox']+gt_calc['Mn_Gt_cat_12ox']+gt_calc['Mg_Gt_cat_12ox']+gt_calc['Ca_Gt_cat_12ox']+gt_calc['Na_Gt_cat_12ox']+gt_calc['K_Gt_cat_12ox']+gt_calc['Cr_Gt_cat_12ox']+gt_calc['P_Gt_cat_12ox']+gt_calc['Ni_Gt_cat_12ox'])
-
-    gt_calc['Mg_MgFeCa_Gt'] = gt_calc['Mg_Gt_cat_12ox'] / (gt_calc['Mg_Gt_cat_12ox'] + gt_calc['Fet_Gt_cat_12ox'] + gt_calc['Ca_Gt_cat_12ox'])
-    gt_calc['Fe_MgFeCa_Gt'] = gt_calc['Fet_Gt_cat_12ox'] / (gt_calc['Mg_Gt_cat_12ox'] + gt_calc['Fet_Gt_cat_12ox'] + gt_calc['Ca_Gt_cat_12ox'])
-    gt_calc['Ca_MgFeCa_Gt'] = gt_calc['Ca_Gt_cat_12ox'] / (gt_calc['Mg_Gt_cat_12ox'] + gt_calc['Fet_Gt_cat_12ox'] + gt_calc['Ca_Gt_cat_12ox'])
-
-    gt_calc['Al_AlCr_Gt'] = gt_calc['Al_Gt_cat_12ox'] / (gt_calc['Al_Gt_cat_12ox'] + gt_calc['Cr_Gt_cat_12ox'])
-    gt_calc['Cr_AlCr_Gt'] = gt_calc['Cr_Gt_cat_12ox'] / (gt_calc['Al_Gt_cat_12ox'] + gt_calc['Cr_Gt_cat_12ox'])
+    gt_calc["Gt_Cation_Sum"] = (
+        gt_calc["Si_Gt_cat_12ox"]
+        + gt_calc["Ti_Gt_cat_12ox"]
+        + gt_calc["Al_Gt_cat_12ox"]
+        + gt_calc["Fet_Gt_cat_12ox"]
+        + gt_calc["Mn_Gt_cat_12ox"]
+        + gt_calc["Mg_Gt_cat_12ox"]
+        + gt_calc["Ca_Gt_cat_12ox"]
+        + gt_calc["Na_Gt_cat_12ox"]
+        + gt_calc["K_Gt_cat_12ox"]
+        + gt_calc["Cr_Gt_cat_12ox"]
+        + gt_calc["P_Gt_cat_12ox"]
+        + gt_calc["Ni_Gt_cat_12ox"]
+    )
+
+    gt_calc["Mg_MgFeCa_Gt"] = gt_calc["Mg_Gt_cat_12ox"] / (
+        gt_calc["Mg_Gt_cat_12ox"]
+        + gt_calc["Fet_Gt_cat_12ox"]
+        + gt_calc["Ca_Gt_cat_12ox"]
+    )
+    gt_calc["Fe_MgFeCa_Gt"] = gt_calc["Fet_Gt_cat_12ox"] / (
+        gt_calc["Mg_Gt_cat_12ox"]
+        + gt_calc["Fet_Gt_cat_12ox"]
+        + gt_calc["Ca_Gt_cat_12ox"]
+    )
+    gt_calc["Ca_MgFeCa_Gt"] = gt_calc["Ca_Gt_cat_12ox"] / (
+        gt_calc["Mg_Gt_cat_12ox"]
+        + gt_calc["Fet_Gt_cat_12ox"]
+        + gt_calc["Ca_Gt_cat_12ox"]
+    )
+
+    gt_calc["Al_AlCr_Gt"] = gt_calc["Al_Gt_cat_12ox"] / (
+        gt_calc["Al_Gt_cat_12ox"] + gt_calc["Cr_Gt_cat_12ox"]
+    )
+    gt_calc["Cr_AlCr_Gt"] = gt_calc["Cr_Gt_cat_12ox"] / (
+        gt_calc["Al_Gt_cat_12ox"] + gt_calc["Cr_Gt_cat_12ox"]
+    )
 
     # HOW TO HANDLE Fe2+ AND Fe3+
-    gt_calc['Ca_Mg_Fe_Mn_X_Gt'] = gt_calc['Ca_Gt_cat_12ox'] + gt_calc['Mg_Gt_cat_12ox'] + gt_calc['Fet_Gt_cat_12ox'] + gt_calc['Mn_Gt_cat_12ox']
-    gt_calc['Al_Fe_Mn_Cr_Y_Gt'] = gt_calc['Al_Gt_cat_12ox'] + gt_calc['Fet_Gt_cat_12ox'] + gt_calc['Mn_Gt_cat_12ox'] + gt_calc['Cr_Gt_cat_12ox']
+    gt_calc["Ca_Mg_Fe_Mn_X_Gt"] = (
+        gt_calc["Ca_Gt_cat_12ox"]
+        + gt_calc["Mg_Gt_cat_12ox"]
+        + gt_calc["Fet_Gt_cat_12ox"]
+        + gt_calc["Mn_Gt_cat_12ox"]
+    )
+    gt_calc["Al_Fe_Mn_Cr_Y_Gt"] = (
+        gt_calc["Al_Gt_cat_12ox"]
+        + gt_calc["Fet_Gt_cat_12ox"]
+        + gt_calc["Mn_Gt_cat_12ox"]
+        + gt_calc["Cr_Gt_cat_12ox"]
+    )
 
     cat_prop = calculate_cat_proportions_garnet(gt_comps=gt_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([gt_comps, gt_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-# %% AMPHIBOLE 
+# %% AMPHIBOLE
 
-def calculate_mol_proportions_amphibole(amp_comps):
 
+def calculate_mol_proportions_amphibole(amp_comps):
     """
-    
+
     Import amphibole compositions using amp_comps=My_amphiboles, returns mole proportions
 
     Parameters
     -------
     amp_comps: pandas.DataFrame
             Panda DataFrame of amphibole compositions with column headings SiO2_Amp, MgO_Amp etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for amphiboles with column headings of the form SiO2_Amp_mol_prop
 
     """
 
-    oxide_mass_amp = {'SiO2_Amp': 60.0843, 'MgO_Amp': 40.3044, 'FeOt_Amp': 71.8464, 'CaO_Amp': 56.0774, 'Al2O3_Amp': 101.961,'Na2O_Amp': 61.9789, 'K2O_Amp': 94.196, 'MnO_Amp': 70.9375, 'TiO2_Amp': 79.8788, 'Cr2O3_Amp': 151.9982}
-    oxide_mass_amp_df = pd.DataFrame.from_dict(oxide_mass_amp, orient='index').T
-    oxide_mass_amp_df['Sample_ID_Amp'] = 'MolWt'
-    oxide_mass_amp_df.set_index('Sample_ID_Amp', inplace=True)
+    oxide_mass_amp = {
+        "SiO2_Amp": 60.0843,
+        "MgO_Amp": 40.3044,
+        "FeOt_Amp": 71.8464,
+        "CaO_Amp": 56.0774,
+        "Al2O3_Amp": 101.961,
+        "Na2O_Amp": 61.9789,
+        "K2O_Amp": 94.196,
+        "MnO_Amp": 70.9375,
+        "TiO2_Amp": 79.8788,
+        "Cr2O3_Amp": 151.9982,
+    }
+    oxide_mass_amp_df = pd.DataFrame.from_dict(oxide_mass_amp, orient="index").T
+    oxide_mass_amp_df["Sample_ID_Amp"] = "MolWt"
+    oxide_mass_amp_df.set_index("Sample_ID_Amp", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     amp_wt = amp_comps.reindex(oxide_mass_amp_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    amp_wt_combo = pd.concat([oxide_mass_amp_df, amp_wt],)
+    amp_wt_combo = pd.concat(
+        [oxide_mass_amp_df, amp_wt],
+    )
     # Drop the calculation column
     mol_prop_anhyd = amp_wt_combo.div(
-        amp_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+        amp_wt_combo.loc["MolWt", :], axis="columns"
+    ).drop(["MolWt"])
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
 
 def calculate_cat_proportions_amphibole(*, amp_comps=None, oxide_headers=False):
-
     """
     Import amphibole compositions using amp_comps=My_amphiboles, returns cation proportions
 
     Parameters
     -------
     amp_comps: pandas.DataFrame
             amphibole compositions with column headings SiO2_Amp, MgO_Amp etc.
@@ -2458,81 +3425,112 @@
     Returns
     -------
     pandas DataFrame
         cation proportions for amphibole with column headings of the form ...Amp_cat_prop
 
     """
 
-    cation_num_amp = {'SiO2_Amp': 1, 'MgO_Amp': 1, 'FeOt_Amp': 1, 'CaO_Amp': 1, 'Al2O3_Amp': 2, 'Na2O_Amp': 2, 'K2O_Amp': 2, 'MnO_Amp': 1, 'TiO2_Amp': 1, 'Cr2O3_Amp': 2}
-
-    cation_num_amp_df = pd.DataFrame.from_dict(cation_num_amp, orient='index').T
-    cation_num_amp_df['Sample_ID_Amp'] = 'CatNum'
-    cation_num_amp_df.set_index('Sample_ID_Amp', inplace=True)
+    cation_num_amp = {
+        "SiO2_Amp": 1,
+        "MgO_Amp": 1,
+        "FeOt_Amp": 1,
+        "CaO_Amp": 1,
+        "Al2O3_Amp": 2,
+        "Na2O_Amp": 2,
+        "K2O_Amp": 2,
+        "MnO_Amp": 1,
+        "TiO2_Amp": 1,
+        "Cr2O3_Amp": 2,
+    }
+
+    cation_num_amp_df = pd.DataFrame.from_dict(cation_num_amp, orient="index").T
+    cation_num_amp_df["Sample_ID_Amp"] = "CatNum"
+    cation_num_amp_df.set_index("Sample_ID_Amp", inplace=True)
 
     amp_prop_no_cat_num = calculate_mol_proportions_amphibole(amp_comps=amp_comps)
-    amp_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in amp_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_amp_df.reindex(oxide_mass_amp_df.columns, axis=1).fillna(0)
+    amp_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in amp_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_amp_df.reindex(
+        oxide_mass_amp_df.columns, axis=1
+    ).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, amp_prop_no_cat_num])
     cation_prop_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
 
-    cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                        'SiO2_Amp_cat_prop': 'Si_Amp_cat_prop',
-                        'TiO2_Amp_cat_prop': 'Ti_Amp_cat_prop',
-                        'Al2O3_Amp_cat_prop': 'Al_Amp_cat_prop',
-                        'FeOt_Amp_cat_prop': 'Fet_Amp_cat_prop',
-                        'MnO_Amp_cat_prop': 'Mn_Amp_cat_prop',
-                        'MgO_Amp_cat_prop': 'Mg_Amp_cat_prop',
-                        'CaO_Amp_cat_prop': 'Ca_Amp_cat_prop',
-                        'Na2O_Amp_cat_prop': 'Na_Amp_cat_prop',
-                        'K2O_Amp_cat_prop': 'K_Amp_cat_prop',
-                        'Cr2O3_Amp_cat_prop': 'Cr_Amp_cat_prop',
-                        'P2O5_Amp_cat_prop': 'P_Amp_cat_prop',
-                        })
+    cation_prop_anhyd2 = cation_prop_anhyd.rename(
+        columns={
+            "SiO2_Amp_cat_prop": "Si_Amp_cat_prop",
+            "TiO2_Amp_cat_prop": "Ti_Amp_cat_prop",
+            "Al2O3_Amp_cat_prop": "Al_Amp_cat_prop",
+            "FeOt_Amp_cat_prop": "Fet_Amp_cat_prop",
+            "MnO_Amp_cat_prop": "Mn_Amp_cat_prop",
+            "MgO_Amp_cat_prop": "Mg_Amp_cat_prop",
+            "CaO_Amp_cat_prop": "Ca_Amp_cat_prop",
+            "Na2O_Amp_cat_prop": "Na_Amp_cat_prop",
+            "K2O_Amp_cat_prop": "K_Amp_cat_prop",
+            "Cr2O3_Amp_cat_prop": "Cr_Amp_cat_prop",
+            "P2O5_Amp_cat_prop": "P_Amp_cat_prop",
+        }
+    )
 
     return cation_prop_anhyd2
 
 
 def calculate_oxygens_amphibole(amp_comps):
-
     """
-    
+
     Import amphiboles compositions using amp_comps=My_Amps, returns number of oxygens (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     amp_comps: pandas.DataFrame
         amphiboles compositions with column headings SiO2_Amp, MgO_Amp etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Amp_ox
 
     """
 
-    oxygen_num_amp = {'SiO2_Amp': 2, 'MgO_Amp': 1, 'FeOt_Amp': 1, 'CaO_Amp': 1, 'Al2O3_Amp': 3, 'Na2O_Amp': 1, 'K2O_Amp': 1, 'MnO_Amp': 1, 'TiO2_Amp': 2, 'Cr2O3_Amp': 3}
-    oxygen_num_amp_df = pd.DataFrame.from_dict(oxygen_num_amp, orient='index').T
-    oxygen_num_amp_df['Sample_ID_Amp'] = 'OxNum'
-    oxygen_num_amp_df.set_index('Sample_ID_Amp', inplace=True)
+    oxygen_num_amp = {
+        "SiO2_Amp": 2,
+        "MgO_Amp": 1,
+        "FeOt_Amp": 1,
+        "CaO_Amp": 1,
+        "Al2O3_Amp": 3,
+        "Na2O_Amp": 1,
+        "K2O_Amp": 1,
+        "MnO_Amp": 1,
+        "TiO2_Amp": 2,
+        "Cr2O3_Amp": 3,
+    }
+    oxygen_num_amp_df = pd.DataFrame.from_dict(oxygen_num_amp, orient="index").T
+    oxygen_num_amp_df["Sample_ID_Amp"] = "OxNum"
+    oxygen_num_amp_df.set_index("Sample_ID_Amp", inplace=True)
 
     mol_prop = calculate_mol_proportions_amphibole(amp_comps=amp_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '') for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_amp_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
     return oxygens_anhyd
 
 
 def calculate_23oxygens_amphibole(amp_comps):
-
     """
-    
+
     Import amphibole compositions using amp_comps=My_Amps, returns cations on the basis of 23 oxygens.
 
     Parameters
     -------
     amp_comps: pandas.DataFrame
         amphibole compositions with column headings SiO2_Amp, MgO_Amp etc.
 
@@ -2540,96 +3538,149 @@
     -------
     pandas DataFrame
         cations on the basis of 23 oxygens, with column headings of the form Si_Amp_cat_23ox.
         For simplicity, and consistency of column labelling to aid calculations, oxide names are preserved,
         so outputs are Na_Amp_cat_23ox rather than Na_Amp_cat_23ox.
 
     """
-    
-    cation_num_amp = {'SiO2_Amp': 1, 'MgO_Amp': 1, 'FeOt_Amp': 1, 'CaO_Amp': 1, 'Al2O3_Amp': 2, 'Na2O_Amp': 2, 'K2O_Amp': 2, 'MnO_Amp': 1, 'TiO2_Amp': 1, 'Cr2O3_Amp': 2}
 
-    cation_num_amp_df = pd.DataFrame.from_dict(cation_num_amp, orient='index').T
-    cation_num_amp_df['Sample_ID_Amp'] = 'CatNum'
-    cation_num_amp_df.set_index('Sample_ID_Amp', inplace=True)
+    cation_num_amp = {
+        "SiO2_Amp": 1,
+        "MgO_Amp": 1,
+        "FeOt_Amp": 1,
+        "CaO_Amp": 1,
+        "Al2O3_Amp": 2,
+        "Na2O_Amp": 2,
+        "K2O_Amp": 2,
+        "MnO_Amp": 1,
+        "TiO2_Amp": 1,
+        "Cr2O3_Amp": 2,
+    }
+
+    cation_num_amp_df = pd.DataFrame.from_dict(cation_num_amp, orient="index").T
+    cation_num_amp_df["Sample_ID_Amp"] = "CatNum"
+    cation_num_amp_df.set_index("Sample_ID_Amp", inplace=True)
 
     oxygens = calculate_oxygens_amphibole(amp_comps=amp_comps)
-    renorm_factor = 23 / (oxygens.sum(axis='columns'))
+    renorm_factor = 23 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_amphibole(amp_comps=amp_comps)
-    mol_prop['oxy_renorm_factor'] = renorm_factor
-    mol_prop_23 = mol_prop.multiply(mol_prop['oxy_renorm_factor'], axis='rows')
-    mol_prop_23.columns = [str(col).replace('_mol_prop', '') for col in mol_prop_23.columns]
+    mol_prop["oxy_renorm_factor"] = renorm_factor
+    mol_prop_23 = mol_prop.multiply(mol_prop["oxy_renorm_factor"], axis="rows")
+    mol_prop_23.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_23.columns
+    ]
 
     ox_num_reindex = cation_num_amp_df.reindex(mol_prop_23.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_23])
-    cation_23_ox = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_23_ox.columns = [str(col).replace('_mol_prop', '_cat_23ox') for col in mol_prop.columns]
-
-    cation_23=cation_23_ox.rename(columns={
-                            'SiO2_Amp_cat_23ox': 'Si_Amp_cat_23ox',
-                            'TiO2_Amp_cat_23ox': 'Ti_Amp_cat_23ox',
-                            'Al2O3_Amp_cat_23ox': 'Al_Amp_cat_23ox',
-                            'FeOt_Amp_cat_23ox': 'Fet_Amp_cat_23ox',
-                            'MnO_Amp_cat_23ox': 'Mn_Amp_cat_23ox',
-                            'MgO_Amp_cat_23ox': 'Mg_Amp_cat_23ox',
-                            'CaO_Amp_cat_23ox': 'Ca_Amp_cat_23ox',
-                            'Na2O_Amp_cat_23ox': 'Na_Amp_cat_23ox',
-                            'K2O_Amp_cat_23ox': 'K_Amp_cat_23ox',
-                            'Cr2O3_Amp_cat_23ox': 'Cr_Amp_cat_23ox',
-                            'P2O5_Amp_cat_23ox': 'P_Amp_cat_23ox_frac',})
-
-    cation_23['cation_sum_Si_Mg'] = (cation_23['Si_Amp_cat_23ox'] + cation_23['Ti_Amp_cat_23ox'] + cation_23['Al_Amp_cat_23ox'] + cation_23['Cr_Amp_cat_23ox'] + cation_23['Fet_Amp_cat_23ox'] + cation_23['Mn_Amp_cat_23ox'] + cation_23['Mg_Amp_cat_23ox'])
-    cation_23['cation_sum_Si_Ca'] = (cation_23['cation_sum_Si_Mg'] + cation_23['Ca_Amp_cat_23ox'])
-    cation_23['Amp_Cation_Sum'] = cation_23['cation_sum_Si_Ca'] + cation_23['Na_Amp_cat_23ox'] + +cation_23['K_Amp_cat_23ox']
-    cation_23['Mgno_Amp'] = cation_23['Mg_Amp_cat_23ox'] / (cation_23['Mg_Amp_cat_23ox'] + cation_23['Fet_Amp_cat_23ox'])
+    cation_23_ox = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+
+    cation_23_ox.columns = [
+        str(col).replace("_mol_prop", "_cat_23ox") for col in mol_prop.columns
+    ]
+
+    cation_23 = cation_23_ox.rename(
+        columns={
+            "SiO2_Amp_cat_23ox": "Si_Amp_cat_23ox",
+            "TiO2_Amp_cat_23ox": "Ti_Amp_cat_23ox",
+            "Al2O3_Amp_cat_23ox": "Al_Amp_cat_23ox",
+            "FeOt_Amp_cat_23ox": "Fet_Amp_cat_23ox",
+            "MnO_Amp_cat_23ox": "Mn_Amp_cat_23ox",
+            "MgO_Amp_cat_23ox": "Mg_Amp_cat_23ox",
+            "CaO_Amp_cat_23ox": "Ca_Amp_cat_23ox",
+            "Na2O_Amp_cat_23ox": "Na_Amp_cat_23ox",
+            "K2O_Amp_cat_23ox": "K_Amp_cat_23ox",
+            "Cr2O3_Amp_cat_23ox": "Cr_Amp_cat_23ox",
+            "P2O5_Amp_cat_23ox": "P_Amp_cat_23ox_frac",
+        }
+    )
+
+    cation_23["cation_sum_Si_Mg"] = (
+        cation_23["Si_Amp_cat_23ox"]
+        + cation_23["Ti_Amp_cat_23ox"]
+        + cation_23["Al_Amp_cat_23ox"]
+        + cation_23["Cr_Amp_cat_23ox"]
+        + cation_23["Fet_Amp_cat_23ox"]
+        + cation_23["Mn_Amp_cat_23ox"]
+        + cation_23["Mg_Amp_cat_23ox"]
+    )
+    cation_23["cation_sum_Si_Ca"] = (
+        cation_23["cation_sum_Si_Mg"] + cation_23["Ca_Amp_cat_23ox"]
+    )
+    cation_23["Amp_Cation_Sum"] = (
+        cation_23["cation_sum_Si_Ca"]
+        + cation_23["Na_Amp_cat_23ox"]
+        + +cation_23["K_Amp_cat_23ox"]
+    )
+    cation_23["Mgno_Amp"] = cation_23["Mg_Amp_cat_23ox"] / (
+        cation_23["Mg_Amp_cat_23ox"] + cation_23["Fet_Amp_cat_23ox"]
+    )
 
     return cation_23
 
+
 # Ridolfi Amphiboles, using Cl and F, does on 13 cations.
 
 
 def calculate_mol_proportions_amphibole_ridolfi(amp_comps):
-
     """
-    
+
     Import amphibole compositions using amp_comps=My_amphiboles, returns mole proportions
 
     Parameters
     -------
     amp_comps: pandas.DataFrame
             Panda DataFrame of amphibole compositions with column headings SiO2_Amp, MgO_Amp etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for amphiboles with column headings of the form SiO2_Amp_mol_prop
 
     """
 
-    oxide_mass_amp_Ridolfi = {'SiO2_Amp': 60.084, 'MgO_Amp': 40.304, 'FeOt_Amp': 71.846, 'CaO_Amp': 56.079, 'Al2O3_Amp': 101.961, 'Na2O_Amp': 61.979, 'K2O_Amp': 94.195, 'MnO_Amp': 70.937, 'TiO2_Amp': 79.898, 'Cr2O3_Amp': 151.9902, 'F_Amp': 18.998, 'Cl_Amp': 35.453}
-    oxide_mass_amp_df_Ridolfi = pd.DataFrame.from_dict(oxide_mass_amp_Ridolfi, orient='index').T
-    oxide_mass_amp_df_Ridolfi['Sample_ID_Amp'] = 'MolWt'
-    oxide_mass_amp_df_Ridolfi.set_index('Sample_ID_Amp', inplace=True)
+    oxide_mass_amp_Ridolfi = {
+        "SiO2_Amp": 60.084,
+        "MgO_Amp": 40.304,
+        "FeOt_Amp": 71.846,
+        "CaO_Amp": 56.079,
+        "Al2O3_Amp": 101.961,
+        "Na2O_Amp": 61.979,
+        "K2O_Amp": 94.195,
+        "MnO_Amp": 70.937,
+        "TiO2_Amp": 79.898,
+        "Cr2O3_Amp": 151.9902,
+        "F_Amp": 18.998,
+        "Cl_Amp": 35.453,
+    }
+    oxide_mass_amp_df_Ridolfi = pd.DataFrame.from_dict(
+        oxide_mass_amp_Ridolfi, orient="index"
+    ).T
+    oxide_mass_amp_df_Ridolfi["Sample_ID_Amp"] = "MolWt"
+    oxide_mass_amp_df_Ridolfi.set_index("Sample_ID_Amp", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     amp_wt = amp_comps.reindex(oxide_mass_amp_df_Ridolfi.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    amp_wt_combo = pd.concat([oxide_mass_amp_df_Ridolfi, amp_wt],)
+    amp_wt_combo = pd.concat(
+        [oxide_mass_amp_df_Ridolfi, amp_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = amp_wt_combo.div(amp_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
-    
-    return mol_prop_anhyd
+    mol_prop_anhyd = amp_wt_combo.div(
+        amp_wt_combo.loc["MolWt", :], axis="columns"
+    ).drop(["MolWt"])
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
 
+    return mol_prop_anhyd
 
 
 def calculate_cat_proportions_amphibole_ridolfi(*, amp_comps=None):
-    
     """
-    
+
     Import amphibole compositions using amp_comps=My_amphiboles, returns cation proportions
 
     Parameters
     -------
     amp_comps: pandas.DataFrame
             amphibole compositions with column headings SiO2_Amp, MgO_Amp etc.
 
@@ -2638,26 +3689,35 @@
     pandas DataFrame
         cation proportions for amphibole with column headings of the form SiO2_Amp_cat_prop
         For simplicity, and consistency of column heading types, oxide names are preserved,
         so outputs are Na2O_Amp_cat_prop rather than Na_Amp_cat_prop.
 
     """
 
-    amp_prop_no_cat_num = calculate_mol_proportions_amphibole_ridolfi(amp_comps=amp_comps)
-    amp_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in amp_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_amp_df_Ridolfi.reindex(oxide_mass_amp_df_Ridolfi.columns, axis=1).fillna(0)
+    amp_prop_no_cat_num = calculate_mol_proportions_amphibole_ridolfi(
+        amp_comps=amp_comps
+    )
+    amp_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in amp_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_amp_df_Ridolfi.reindex(
+        oxide_mass_amp_df_Ridolfi.columns, axis=1
+    ).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, amp_prop_no_cat_num])
-    cation_prop_anhyd = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
-    
+    cation_prop_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
+
     return cation_prop_anhyd
 
 
 def calculate_13cations_amphibole_ridolfi(amp_comps):
-    
     """Import amphibole compositions using amp_comps=My_amphiboles, returns
     components calculated on basis of 13 cations following Ridolfi supporting information
 
     Parameters
     -------
     amp_comps: pandas.DataFrame
             amphibole compositions with column headings SiO2_Amp, MgO_Amp etc.
@@ -2665,249 +3725,323 @@
     Returns
     -------
     pandas DataFrame
         cation fractions for amphiboles with column headings of the form SiO2_Amp_13_cat...
 
     """
     cats = calculate_cat_proportions_amphibole_ridolfi(amp_comps=amp_comps)
-    cats['cation_sum_Si_Mg'] = (cats['SiO2_Amp_cat_prop'] + cats['TiO2_Amp_cat_prop'] + cats['Al2O3_Amp_cat_prop'] + cats['Cr2O3_Amp_cat_prop'] + cats['FeOt_Amp_cat_prop'] + cats['MnO_Amp_cat_prop'] + cats['MgO_Amp_cat_prop'])
-
-    sum_SiMg = cats['cation_sum_Si_Mg']
-    cats.drop(['cation_sum_Si_Mg'], axis=1, inplace=True)
-    cat_13 = 13 * cats.divide(sum_SiMg, axis='rows')
-    cat_13.columns = [str(col).replace('_cat_prop', '_13_cat') for col in cat_13.columns]
-    cat_13['cation_sum_Si_Mg'] = sum_SiMg
-    cation_13_noox=cat_13.rename(columns={
-                            'SiO2_Amp_13_cat': 'Si_Amp_13_cat',
-                            'TiO2_Amp_13_cat': 'Ti_Amp_13_cat',
-                            'Al2O3_Amp_13_cat': 'Al_Amp_13_cat',
-                            'FeOt_Amp_13_cat': 'Fet_Amp_13_cat',
-                            'MnO_Amp_13_cat': 'Mn_Amp_13_cat',
-                            'MgO_Amp_13_cat': 'Mg_Amp_13_cat',
-                            'CaO_Amp_13_cat': 'Ca_Amp_13_cat',
-                            'Na2O_Amp_13_cat': 'Na_Amp_13_cat',
-                            'K2O_Amp_13_cat': 'K_Amp_13_cat',
-                            'Cr2O3_Amp_13_cat': 'Cr_Amp_13_cat',
-                            'P2O5_Amp_13_cat': 'P_Amp_13_cat_frac'})
+    cats["cation_sum_Si_Mg"] = (
+        cats["SiO2_Amp_cat_prop"]
+        + cats["TiO2_Amp_cat_prop"]
+        + cats["Al2O3_Amp_cat_prop"]
+        + cats["Cr2O3_Amp_cat_prop"]
+        + cats["FeOt_Amp_cat_prop"]
+        + cats["MnO_Amp_cat_prop"]
+        + cats["MgO_Amp_cat_prop"]
+    )
+
+    sum_SiMg = cats["cation_sum_Si_Mg"]
+    cats.drop(["cation_sum_Si_Mg"], axis=1, inplace=True)
+    cat_13 = 13 * cats.divide(sum_SiMg, axis="rows")
+    cat_13.columns = [
+        str(col).replace("_cat_prop", "_13_cat") for col in cat_13.columns
+    ]
+    cat_13["cation_sum_Si_Mg"] = sum_SiMg
+    cation_13_noox = cat_13.rename(
+        columns={
+            "SiO2_Amp_13_cat": "Si_Amp_13_cat",
+            "TiO2_Amp_13_cat": "Ti_Amp_13_cat",
+            "Al2O3_Amp_13_cat": "Al_Amp_13_cat",
+            "FeOt_Amp_13_cat": "Fet_Amp_13_cat",
+            "MnO_Amp_13_cat": "Mn_Amp_13_cat",
+            "MgO_Amp_13_cat": "Mg_Amp_13_cat",
+            "CaO_Amp_13_cat": "Ca_Amp_13_cat",
+            "Na2O_Amp_13_cat": "Na_Amp_13_cat",
+            "K2O_Amp_13_cat": "K_Amp_13_cat",
+            "Cr2O3_Amp_13_cat": "Cr_Amp_13_cat",
+            "P2O5_Amp_13_cat": "P_Amp_13_cat_frac",
+        }
+    )
 
     cat_13_out = pd.concat([cats, cation_13_noox], axis=1)
 
     return cat_13_out
 
 
 def calculate_sites_ridolfi(amp_comps):
-
-    amp_comps_c=amp_comps.copy()
-    norm_cations=calculate_13cations_amphibole_ridolfi(amp_comps_c)
+    amp_comps_c = amp_comps.copy()
+    norm_cations = calculate_13cations_amphibole_ridolfi(amp_comps_c)
 
     # Ridolfi T sites
-    norm_cations['Si_T_Amp']=norm_cations['Si_Amp_13_cat']
-    norm_cations['Al_IV_T_Amp']=0
-    norm_cations['Ti_T_Amp']=0
+    norm_cations["Si_T_Amp"] = norm_cations["Si_Amp_13_cat"]
+    norm_cations["Al_IV_T_Amp"] = 0
+    norm_cations["Ti_T_Amp"] = 0
     # Ridolfi C Sites
-    norm_cations['Cr_C_Amp']=0
-    norm_cations['Fe3_C_Amp']=0
-    norm_cations['Mg_C_Amp']=0
-    norm_cations['Fe2_C_Amp']=0
-    norm_cations['Mn_C_Amp_Amp']=0
+    norm_cations["Cr_C_Amp"] = 0
+    norm_cations["Fe3_C_Amp"] = 0
+    norm_cations["Mg_C_Amp"] = 0
+    norm_cations["Fe2_C_Amp"] = 0
+    norm_cations["Mn_C_Amp_Amp"] = 0
     # Ridolfi B sites
-    norm_cations['Ca_B_Amp']=norm_cations['Ca_Amp_13_cat']
-    norm_cations['Na_B_Amp']=0
+    norm_cations["Ca_B_Amp"] = norm_cations["Ca_Amp_13_cat"]
+    norm_cations["Na_B_Amp"] = 0
     # Ridolfi A sites
-    norm_cations['Na_A_Amp']=0
-    norm_cations['K_A_Amp']=norm_cations['K_Amp_13_cat']
+    norm_cations["Na_A_Amp"] = 0
+    norm_cations["K_A_Amp"] = norm_cations["K_Amp_13_cat"]
 
     # if sum greater than 8, equal to difference
-    norm_cations['Al_IV_T_Amp']=8-norm_cations['Si_T_Amp']
+    norm_cations["Al_IV_T_Amp"] = 8 - norm_cations["Si_T_Amp"]
     # But if SiTi grater than 8
-    Si_Al_less8=(norm_cations['Si_Amp_13_cat']+norm_cations['Al_Amp_13_cat'])<8
-    norm_cations.loc[(Si_Al_less8), 'Al_IV_T_Amp']=norm_cations['Al_Amp_13_cat']
+    Si_Al_less8 = (norm_cations["Si_Amp_13_cat"] + norm_cations["Al_Amp_13_cat"]) < 8
+    norm_cations.loc[(Si_Al_less8), "Al_IV_T_Amp"] = norm_cations["Al_Amp_13_cat"]
 
     # Ti, If Si + Al (IV)<8, 8-Si-AlIV
-    Si_Al_sites_less8=(norm_cations['Si_T_Amp']+norm_cations['Al_IV_T_Amp'])<8
-    norm_cations.loc[(Si_Al_sites_less8), 'Ti_T_Amp']=8-norm_cations['Si_T_Amp']-norm_cations['Al_IV_T_Amp']
+    Si_Al_sites_less8 = (norm_cations["Si_T_Amp"] + norm_cations["Al_IV_T_Amp"]) < 8
+    norm_cations.loc[(Si_Al_sites_less8), "Ti_T_Amp"] = (
+        8 - norm_cations["Si_T_Amp"] - norm_cations["Al_IV_T_Amp"]
+    )
 
     #  AL VI, any AL left
-    norm_cations['Al_VI_C_Amp']=norm_cations['Al_Amp_13_cat']-norm_cations['Al_IV_T_Amp']
+    norm_cations["Al_VI_C_Amp"] = (
+        norm_cations["Al_Amp_13_cat"] - norm_cations["Al_IV_T_Amp"]
+    )
 
     # Ti C Sites, any Ti left
-    norm_cations['Ti_C_Amp']=norm_cations['Ti_Amp_13_cat']-norm_cations['Ti_T_Amp']
+    norm_cations["Ti_C_Amp"] = norm_cations["Ti_Amp_13_cat"] - norm_cations["Ti_T_Amp"]
 
     # CR site, All Cr
-    norm_cations['Cr_C_Amp']=norm_cations['Cr_Amp_13_cat']
+    norm_cations["Cr_C_Amp"] = norm_cations["Cr_Amp_13_cat"]
 
     # Calculate charge for Fe
-    norm_cations['Charge']=(norm_cations['Si_Amp_13_cat']*4+norm_cations['Ti_Amp_13_cat']*4+norm_cations['Al_Amp_13_cat']*3+
-    norm_cations['Cr_Amp_13_cat']*3+norm_cations['Fet_Amp_13_cat']*2+norm_cations['Mn_Amp_13_cat']*2+norm_cations['Mg_Amp_13_cat']*2
-    +norm_cations['Ca_Amp_13_cat']*2+norm_cations['Na_Amp_13_cat']+norm_cations['K_Amp_13_cat'])
+    norm_cations["Charge"] = (
+        norm_cations["Si_Amp_13_cat"] * 4
+        + norm_cations["Ti_Amp_13_cat"] * 4
+        + norm_cations["Al_Amp_13_cat"] * 3
+        + norm_cations["Cr_Amp_13_cat"] * 3
+        + norm_cations["Fet_Amp_13_cat"] * 2
+        + norm_cations["Mn_Amp_13_cat"] * 2
+        + norm_cations["Mg_Amp_13_cat"] * 2
+        + norm_cations["Ca_Amp_13_cat"] * 2
+        + norm_cations["Na_Amp_13_cat"]
+        + norm_cations["K_Amp_13_cat"]
+    )
 
     # If DG2 (charge)>46, set Fe3 to zero, else set to 46-charge
-    norm_cations['Fe3_C']=46-norm_cations['Charge']
-    High_Charge=norm_cations['Charge']>46
-    norm_cations.loc[(High_Charge), 'Fe3_C']=0
-
-    norm_cations['Fe2_C_Amp']=norm_cations['Fet_Amp_13_cat']-norm_cations['Fe3_C_Amp']
+    norm_cations["Fe3_C"] = 46 - norm_cations["Charge"]
+    High_Charge = norm_cations["Charge"] > 46
+    norm_cations.loc[(High_Charge), "Fe3_C"] = 0
+
+    norm_cations["Fe2_C_Amp"] = (
+        norm_cations["Fet_Amp_13_cat"] - norm_cations["Fe3_C_Amp"]
+    )
 
     #  Allocate all Mg
-    norm_cations['Mg_C_Amp']=norm_cations['Mg_Amp_13_cat']
+    norm_cations["Mg_C_Amp"] = norm_cations["Mg_Amp_13_cat"]
 
     # Allocate all Mn
-    norm_cations['Mn_C_Amp']=norm_cations['Mn_Amp_13_cat']
+    norm_cations["Mn_C_Amp"] = norm_cations["Mn_Amp_13_cat"]
 
     # Na B site,
 
-    norm_cations['Na_B_Amp']=2-norm_cations['Ca_Amp_13_cat']
-    Ca_greaterthanNa=norm_cations['Na_Amp_13_cat']<(2-norm_cations['Ca_Amp_13_cat'])
-    norm_cations.loc[(Ca_greaterthanNa), 'Na_B_Amp']=norm_cations['Na_Amp_13_cat']
+    norm_cations["Na_B_Amp"] = 2 - norm_cations["Ca_Amp_13_cat"]
+    Ca_greaterthanNa = norm_cations["Na_Amp_13_cat"] < (
+        2 - norm_cations["Ca_Amp_13_cat"]
+    )
+    norm_cations.loc[(Ca_greaterthanNa), "Na_B_Amp"] = norm_cations["Na_Amp_13_cat"]
 
     # All Na left after B
-    norm_cations['Na_A_Amp']=norm_cations['Na_Amp_13_cat']-norm_cations['Na_B_Amp']
+    norm_cations["Na_A_Amp"] = norm_cations["Na_Amp_13_cat"] - norm_cations["Na_B_Amp"]
     if "Sample_ID_Amp" in amp_comps.columns:
-        myAmps1_label = amp_comps_c.drop(['Sample_ID_Amp'], axis='columns')
+        myAmps1_label = amp_comps_c.drop(["Sample_ID_Amp"], axis="columns")
     else:
         myAmps1_label = amp_comps_c
-    norm_cations['Sum_input'] = myAmps1_label.sum(axis='columns')
-    Sum_input=norm_cations['Sum_input']
-    Low_sum=norm_cations['Sum_input'] <90
-
-   # Other checks in Ridolfi's spreadsheet
-    norm_cations['H2O_calc']=(2-norm_cations['F_Amp_13_cat']-norm_cations['Cl_Amp_13_cat'])*norm_cations['cation_sum_Si_Mg']*17/13/2
-    norm_cations.loc[(Low_sum), 'H2O_calc']=0
-
-    norm_cations['Charge']=(norm_cations['Si_Amp_13_cat']*4+norm_cations['Ti_Amp_13_cat']*4+norm_cations['Al_Amp_13_cat']*3+
-    norm_cations['Cr_Amp_13_cat']*3+norm_cations['Fet_Amp_13_cat']*2+norm_cations['Mn_Amp_13_cat']*2+norm_cations['Mg_Amp_13_cat']*2
-    +norm_cations['Ca_Amp_13_cat']*2+norm_cations['Na_Amp_13_cat']+norm_cations['K_Amp_13_cat'])
-
-    norm_cations['Fe3_calc']=46-norm_cations['Charge']
-    High_Charge=norm_cations['Charge']>46
-    norm_cations.loc[(High_Charge), 'Fe3_calc']=0
-
-    norm_cations['Fe2_calc']=norm_cations['Fet_Amp_13_cat']-norm_cations['Fe3_calc']
-
-    norm_cations['Fe2O3_calc']=norm_cations['Fe3_calc']*norm_cations['cation_sum_Si_Mg']*159.691/13/2
-    norm_cations.loc[(Low_sum), 'Fe2O3_calc']=0
-
-    norm_cations['FeO_calc']=norm_cations['Fe2_calc']*norm_cations['cation_sum_Si_Mg']*71.846/13
-    norm_cations.loc[(Low_sum), 'Fe2O3_calc']=0
-
-    norm_cations['O=F,Cl']=-(amp_comps_c['F_Amp']*0.421070639014633+amp_comps_c['Cl_Amp']*0.225636758525372)
-    norm_cations.loc[(Low_sum), 'O=F,Cl']=0
-
-    norm_cations['Total_recalc']=(Sum_input-amp_comps_c['FeOt_Amp']+norm_cations['H2O_calc']+norm_cations['Fe2O3_calc']
-    +norm_cations['FeO_calc']+norm_cations['O=F,Cl'])
-    norm_cations.loc[(Low_sum), 'Total']=0
+    norm_cations["Sum_input"] = myAmps1_label.sum(axis="columns")
+    Sum_input = norm_cations["Sum_input"]
+    Low_sum = norm_cations["Sum_input"] < 90
+
+    # Other checks in Ridolfi's spreadsheet
+    norm_cations["H2O_calc"] = (
+        (2 - norm_cations["F_Amp_13_cat"] - norm_cations["Cl_Amp_13_cat"])
+        * norm_cations["cation_sum_Si_Mg"]
+        * 17
+        / 13
+        / 2
+    )
+    norm_cations.loc[(Low_sum), "H2O_calc"] = 0
+
+    norm_cations["Charge"] = (
+        norm_cations["Si_Amp_13_cat"] * 4
+        + norm_cations["Ti_Amp_13_cat"] * 4
+        + norm_cations["Al_Amp_13_cat"] * 3
+        + norm_cations["Cr_Amp_13_cat"] * 3
+        + norm_cations["Fet_Amp_13_cat"] * 2
+        + norm_cations["Mn_Amp_13_cat"] * 2
+        + norm_cations["Mg_Amp_13_cat"] * 2
+        + norm_cations["Ca_Amp_13_cat"] * 2
+        + norm_cations["Na_Amp_13_cat"]
+        + norm_cations["K_Amp_13_cat"]
+    )
+
+    norm_cations["Fe3_calc"] = 46 - norm_cations["Charge"]
+    High_Charge = norm_cations["Charge"] > 46
+    norm_cations.loc[(High_Charge), "Fe3_calc"] = 0
+
+    norm_cations["Fe2_calc"] = norm_cations["Fet_Amp_13_cat"] - norm_cations["Fe3_calc"]
+
+    norm_cations["Fe2O3_calc"] = (
+        norm_cations["Fe3_calc"] * norm_cations["cation_sum_Si_Mg"] * 159.691 / 13 / 2
+    )
+    norm_cations.loc[(Low_sum), "Fe2O3_calc"] = 0
+
+    norm_cations["FeO_calc"] = (
+        norm_cations["Fe2_calc"] * norm_cations["cation_sum_Si_Mg"] * 71.846 / 13
+    )
+    norm_cations.loc[(Low_sum), "Fe2O3_calc"] = 0
+
+    norm_cations["O=F,Cl"] = -(
+        amp_comps_c["F_Amp"] * 0.421070639014633
+        + amp_comps_c["Cl_Amp"] * 0.225636758525372
+    )
+    norm_cations.loc[(Low_sum), "O=F,Cl"] = 0
+
+    norm_cations["Total_recalc"] = (
+        Sum_input
+        - amp_comps_c["FeOt_Amp"]
+        + norm_cations["H2O_calc"]
+        + norm_cations["Fe2O3_calc"]
+        + norm_cations["FeO_calc"]
+        + norm_cations["O=F,Cl"]
+    )
+    norm_cations.loc[(Low_sum), "Total"] = 0
 
     # Set up a column for a fail message
-    norm_cations['Fail Msg']=""
-    norm_cations['Input_Check']=True
+    norm_cations["Fail Msg"] = ""
+    norm_cations["Input_Check"] = True
 
     # Check that old total isn't <90
 
-    norm_cations.loc[(Low_sum), 'Input_Check']=False
-    norm_cations.loc[(Low_sum), 'Fail Msg']="Cation oxide Total<90"
+    norm_cations.loc[(Low_sum), "Input_Check"] = False
+    norm_cations.loc[(Low_sum), "Fail Msg"] = "Cation oxide Total<90"
 
     # First check, that new total is >98.5 (e.g with recalculated H2O etc).
 
-    Low_total_Recalc=norm_cations['Total_recalc']<98.5
-    norm_cations.loc[(Low_total_Recalc), 'Input_Check']=False
-    norm_cations.loc[(Low_total_Recalc), 'Fail Msg']="Recalc Total<98.5"
+    Low_total_Recalc = norm_cations["Total_recalc"] < 98.5
+    norm_cations.loc[(Low_total_Recalc), "Input_Check"] = False
+    norm_cations.loc[(Low_total_Recalc), "Fail Msg"] = "Recalc Total<98.5"
 
     # Next, check that new total isn't >102
-    High_total_Recalc=norm_cations['Total_recalc']>102
-    norm_cations.loc[(High_total_Recalc), 'Input_Check']=False
-    norm_cations.loc[(High_total_Recalc), 'Fail Msg']="Recalc Total>102"
+    High_total_Recalc = norm_cations["Total_recalc"] > 102
+    norm_cations.loc[(High_total_Recalc), "Input_Check"] = False
+    norm_cations.loc[(High_total_Recalc), "Fail Msg"] = "Recalc Total>102"
 
     # Next, check that charge isn't >46.5 ("unbalanced")
-    Unbalanced_Charge=norm_cations['Charge']>46.5
-    norm_cations.loc[(Unbalanced_Charge), 'Input_Check']=False
-    norm_cations.loc[(Unbalanced_Charge), 'Fail Msg']="unbalanced charge (>46.5)"
+    Unbalanced_Charge = norm_cations["Charge"] > 46.5
+    norm_cations.loc[(Unbalanced_Charge), "Input_Check"] = False
+    norm_cations.loc[(Unbalanced_Charge), "Fail Msg"] = "unbalanced charge (>46.5)"
 
     # Next check that Fe2+ is greater than 0, else unbalanced
-    Negative_Fe2=norm_cations['Fe2_calc']<0
-    norm_cations.loc[(Negative_Fe2), 'Input_Check']=False
-    norm_cations.loc[(Negative_Fe2), 'Fail Msg']="unbalanced charge (Fe2<0)"
+    Negative_Fe2 = norm_cations["Fe2_calc"] < 0
+    norm_cations.loc[(Negative_Fe2), "Input_Check"] = False
+    norm_cations.loc[(Negative_Fe2), "Fail Msg"] = "unbalanced charge (Fe2<0)"
 
     # Check that Mg# calculated using just Fe2 is >54, else low Mg
-    norm_cations['Mgno_Fe2']=norm_cations['Mg_Amp_13_cat']/(norm_cations['Mg_Amp_13_cat']+norm_cations['Fe2_calc'])
-    norm_cations['Mgno_FeT']=norm_cations['Mg_Amp_13_cat']/(norm_cations['Mg_Amp_13_cat']+norm_cations['Fet_Amp_13_cat'])
+    norm_cations["Mgno_Fe2"] = norm_cations["Mg_Amp_13_cat"] / (
+        norm_cations["Mg_Amp_13_cat"] + norm_cations["Fe2_calc"]
+    )
+    norm_cations["Mgno_FeT"] = norm_cations["Mg_Amp_13_cat"] / (
+        norm_cations["Mg_Amp_13_cat"] + norm_cations["Fet_Amp_13_cat"]
+    )
+
+    Low_Mgno = 100 * norm_cations["Mgno_Fe2"] < 54
+    norm_cations.loc[(Low_Mgno), "Input_Check"] = False
+    norm_cations.loc[(Low_Mgno), "Fail Msg"] = "Low Mg# (<54)"
 
-    Low_Mgno=100*norm_cations['Mgno_Fe2']<54
-    norm_cations.loc[(Low_Mgno), 'Input_Check']=False
-    norm_cations.loc[(Low_Mgno), 'Fail Msg']="Low Mg# (<54)"
-
-    #Only ones that matter are low Ca, high Ca, BJ3>60, low B cations"
+    # Only ones that matter are low Ca, high Ca, BJ3>60, low B cations"
 
     # If Column CU<1.5,"low Ca"
-    Ca_low=norm_cations['Ca_Amp_13_cat']<1.5
-    norm_cations.loc[(Ca_low), 'Input_Check']=False
-    norm_cations.loc[(Ca_low), 'Fail Msg']="Low Ca (<1.5)"
+    Ca_low = norm_cations["Ca_Amp_13_cat"] < 1.5
+    norm_cations.loc[(Ca_low), "Input_Check"] = False
+    norm_cations.loc[(Ca_low), "Fail Msg"] = "Low Ca (<1.5)"
 
     # If Column CU>2.05, "high Ca"
-    Ca_high=norm_cations['Ca_Amp_13_cat']>2.05
-    norm_cations.loc[(Ca_high), 'Input_Check']=False
-    norm_cations.loc[(Ca_high), 'Fail Msg']="High Ca (>2.05)"
+    Ca_high = norm_cations["Ca_Amp_13_cat"] > 2.05
+    norm_cations.loc[(Ca_high), "Input_Check"] = False
+    norm_cations.loc[(Ca_high), "Fail Msg"] = "High Ca (>2.05)"
 
     # Check that CW<1.99, else "Low B cations"
-    norm_cations['Na_calc']=2-norm_cations['Ca_Amp_13_cat']
-    Ca_greaterthanNa=norm_cations['Na_Amp_13_cat']<(2-norm_cations['Ca_Amp_13_cat'])
-    norm_cations.loc[(Ca_greaterthanNa), 'Na_calc']=norm_cations['Na_Amp_13_cat']
-    norm_cations['B_Sum']=norm_cations['Na_calc']+norm_cations['Ca_Amp_13_cat']
-
-
-    Low_B_Cations=norm_cations['B_Sum']<1.99
-    norm_cations.loc[(Low_B_Cations), 'Input_Check']=False
-    norm_cations.loc[(Low_B_Cations), 'Fail Msg']="Low B Cations"
+    norm_cations["Na_calc"] = 2 - norm_cations["Ca_Amp_13_cat"]
+    Ca_greaterthanNa = norm_cations["Na_Amp_13_cat"] < (
+        2 - norm_cations["Ca_Amp_13_cat"]
+    )
+    norm_cations.loc[(Ca_greaterthanNa), "Na_calc"] = norm_cations["Na_Amp_13_cat"]
+    norm_cations["B_Sum"] = norm_cations["Na_calc"] + norm_cations["Ca_Amp_13_cat"]
+
+    Low_B_Cations = norm_cations["B_Sum"] < 1.99
+    norm_cations.loc[(Low_B_Cations), "Input_Check"] = False
+    norm_cations.loc[(Low_B_Cations), "Fail Msg"] = "Low B Cations"
 
     # Printing composition
-    norm_cations['A_Sum']=norm_cations['Na_A_Amp']+norm_cations['K_A_Amp']
-    norm_cations['class']="N/A"
+    norm_cations["A_Sum"] = norm_cations["Na_A_Amp"] + norm_cations["K_A_Amp"]
+    norm_cations["class"] = "N/A"
     # If <1.5, low Ca,
-    lowCa=norm_cations['Ca_B_Amp']<1.5
-    norm_cations.loc[(lowCa), 'classification']="low-Ca"
+    lowCa = norm_cations["Ca_B_Amp"] < 1.5
+    norm_cations.loc[(lowCa), "classification"] = "low-Ca"
     # Else, if high Ca, If Mgno<5, its low Mg
-    LowMgno=norm_cations['Mgno_Fe2']<0.5
-    norm_cations.loc[((~lowCa)&(LowMgno)), 'classification']="low-Mg"
+    LowMgno = norm_cations["Mgno_Fe2"] < 0.5
+    norm_cations.loc[((~lowCa) & (LowMgno)), "classification"] = "low-Mg"
     # Else, if Si>6.5, its a Mg-hornblende
-    MgHbl=norm_cations['Si_T']>=6.5
-    norm_cations.loc[((~lowCa)&(~LowMgno)&(MgHbl)), 'classification']="Mg-Hornblende"
+    MgHbl = norm_cations["Si_T"] >= 6.5
+    norm_cations.loc[
+        ((~lowCa) & (~LowMgno) & (MgHbl)), "classification"
+    ] = "Mg-Hornblende"
     # Else if Ti_C >0.5, Kaerstiertei
-    Kaer=norm_cations['Ti_C_Amp']>0.5
-    norm_cations.loc[((~lowCa)&(~LowMgno)&(~MgHbl)&(Kaer)), 'classification']="kaersutite"
+    Kaer = norm_cations["Ti_C_Amp"] > 0.5
+    norm_cations.loc[
+        ((~lowCa) & (~LowMgno) & (~MgHbl) & (Kaer)), "classification"
+    ] = "kaersutite"
     # Else if A_Sum<0.5, Tschermakitic pargasite
-    Tsh=norm_cations['A_Sum']<0.5
-    norm_cations.loc[((~lowCa)&(~LowMgno)&(~MgHbl)&(~Kaer)&(Tsh)), 'classification']="Tschermakitic pargasite"
+    Tsh = norm_cations["A_Sum"] < 0.5
+    norm_cations.loc[
+        ((~lowCa) & (~LowMgno) & (~MgHbl) & (~Kaer) & (Tsh)), "classification"
+    ] = "Tschermakitic pargasite"
     # Else if Fe3+>AL VI C sum, Mg-hastingsite
-    MgHast=(norm_cations['Fe3_calc']>norm_cations['Al_VI_C'])
-    norm_cations.loc[((~lowCa)&(~LowMgno)&(~MgHbl)&(~Kaer)&(~Tsh)&(MgHast)), 'classification']="Mg-hastingsite"
+    MgHast = norm_cations["Fe3_calc"] > norm_cations["Al_VI_C"]
+    norm_cations.loc[
+        ((~lowCa) & (~LowMgno) & (~MgHbl) & (~Kaer) & (~Tsh) & (MgHast)),
+        "classification",
+    ] = "Mg-hastingsite"
     # Else, its Pargasite
-    norm_cations.loc[((~lowCa)&(~LowMgno)&(~MgHbl)&(~Kaer)&(~Tsh)&(~MgHast)), 'classification']="Pargasite"
+    norm_cations.loc[
+        ((~lowCa) & (~LowMgno) & (~MgHbl) & (~Kaer) & (~Tsh) & (~MgHast)),
+        "classification",
+    ] = "Pargasite"
 
     return norm_cations
 
 
 def get_amp_sites_from_input_not_amp(dfin, col_drop):
-
     """
     get amp_sites from amp_comps input from import_excel() function.
     """
 
-    amp_comps_lie=dfin.copy()
-    amp_comps_lie.columns = [col.replace(col_drop, '_Amp') for col in amp_comps_lie.columns]
-    amp_amfu_df=calculate_23oxygens_amphibole(amp_comps_lie)
-    amp_sites=get_amp_sites_leake(amp_amfu_df)
+    amp_comps_lie = dfin.copy()
+    amp_comps_lie.columns = [
+        col.replace(col_drop, "_Amp") for col in amp_comps_lie.columns
+    ]
+    amp_amfu_df = calculate_23oxygens_amphibole(amp_comps_lie)
+    amp_sites = get_amp_sites_leake(amp_amfu_df)
 
-    amp_sites['Na_K_A_Amp'] = amp_sites['Na_A_Amp'] + amp_sites['K_A_Amp']
+    amp_sites["Na_K_A_Amp"] = amp_sites["Na_A_Amp"] + amp_sites["K_A_Amp"]
 
-    out=pd.concat([dfin, amp_sites], axis=1)
+    out = pd.concat([dfin, amp_sites], axis=1)
 
     return out
 
 
 def get_amp_sites_leake(amp_apfu_df):
-
     """
     get_amp_sites takes generalized atom per formula unit calculations from
     calculate_23oxygens_amphibole and puts them in the proper cation sites
     according to Leake et al., 1997.
 
     Parameters
     ----------
@@ -2926,297 +4060,498 @@
         B  = M4 sites (2 total)
         A = A site (0 - 1 total)
 
     """
     norm_cations = amp_apfu_df.copy()
 
     # Take unambigous ones and allocate them, set everything else to zero
-    norm_cations['Si_T_Amp']=norm_cations['Si_Amp_cat_23ox']
-    norm_cations['Al_T_Amp']=0
-    norm_cations['Al_C_Amp']=0
-    norm_cations['Ti_C_Amp']=norm_cations['Ti_Amp_cat_23ox']
-    norm_cations['Mg_C_Amp']=0
-    norm_cations['Fe_C_Amp']=0
-    norm_cations['Mn_C_Amp']=0
-    norm_cations['Cr_C_Amp']=norm_cations['Cr_Amp_cat_23ox']
-    norm_cations['Mg_B_Amp']=0
-    norm_cations['Fe_B_Amp']=0
-    norm_cations['Mn_B_Amp']=0
-    norm_cations['Na_B_Amp']=0
-    norm_cations['Ca_B_Amp']=norm_cations['Ca_Amp_cat_23ox']
-    norm_cations['Na_A_Amp']=0
-    norm_cations['K_A_Amp']=norm_cations['K_Amp_cat_23ox']
-    norm_cations['Ca_A_Amp']=0 # This is very ambigous, Leake have Ca A in some of their plots, but no way to put it in A based on workflow of site allocation.
+    norm_cations["Si_T_Amp"] = norm_cations["Si_Amp_cat_23ox"]
+    norm_cations["Al_T_Amp"] = 0
+    norm_cations["Al_C_Amp"] = 0
+    norm_cations["Ti_C_Amp"] = norm_cations["Ti_Amp_cat_23ox"]
+    norm_cations["Mg_C_Amp"] = 0
+    norm_cations["Fe_C_Amp"] = 0
+    norm_cations["Mn_C_Amp"] = 0
+    norm_cations["Cr_C_Amp"] = norm_cations["Cr_Amp_cat_23ox"]
+    norm_cations["Mg_B_Amp"] = 0
+    norm_cations["Fe_B_Amp"] = 0
+    norm_cations["Mn_B_Amp"] = 0
+    norm_cations["Na_B_Amp"] = 0
+    norm_cations["Ca_B_Amp"] = norm_cations["Ca_Amp_cat_23ox"]
+    norm_cations["Na_A_Amp"] = 0
+    norm_cations["K_A_Amp"] = norm_cations["K_Amp_cat_23ox"]
+    norm_cations[
+        "Ca_A_Amp"
+    ] = 0  # This is very ambigous, Leake have Ca A in some of their plots, but no way to put it in A based on workflow of site allocation.
 
     # 5a) Leake T Sites. Place all Si here, if Si<8, fill rest of T with Al.
 
-    #If Si + Al is greater than 8, need to split Al between Al_T and Al_C as it can't all go here
-    Si_Ti_sum_gr8=(norm_cations['Si_Amp_cat_23ox']+norm_cations['Al_Amp_cat_23ox'])>8
+    # If Si + Al is greater than 8, need to split Al between Al_T and Al_C as it can't all go here
+    Si_Ti_sum_gr8 = (
+        norm_cations["Si_Amp_cat_23ox"] + norm_cations["Al_Amp_cat_23ox"]
+    ) > 8
     # Calculate the amount of Ti sites left to fill after putting Si in. dont need to worry
     # about overallocating Ti, as already know they sum to more than 8.
-    Al_T_Si_Ti_sum_gr8=8-norm_cations['Si_Amp_cat_23ox']
+    Al_T_Si_Ti_sum_gr8 = 8 - norm_cations["Si_Amp_cat_23ox"]
     # Got to be careful here, if Si on 23ox is >8, Al_T_Si_Ti_sum_gr8 ends up negative. Add another check
-    Si_l_8=(norm_cations['Si_Amp_cat_23ox']<=8)
+    Si_l_8 = norm_cations["Si_Amp_cat_23ox"] <= 8
     # If Si is less than 8 already, set Ti to the difference
-    norm_cations.loc[(Si_Ti_sum_gr8&Si_l_8), 'Al_T_Amp']=Al_T_Si_Ti_sum_gr8
+    norm_cations.loc[(Si_Ti_sum_gr8 & Si_l_8), "Al_T_Amp"] = Al_T_Si_Ti_sum_gr8
     # If Si is greater than 8, set Al_T to zero
-    norm_cations.loc[(Si_Ti_sum_gr8&(~Si_l_8)), 'Al_T_Amp']=0
-
+    norm_cations.loc[(Si_Ti_sum_gr8 & (~Si_l_8)), "Al_T_Amp"] = 0
 
     # Put remaining Al
-    norm_cations.loc[(Si_Ti_sum_gr8), 'Al_C_Amp']=norm_cations['Al_Amp_cat_23ox']-norm_cations['Al_T_Amp']
-
-    #If Si+Al<8, put all Al in tetrahedlra sites
-    Si_Ti_sum_less8=(norm_cations['Si_Amp_cat_23ox']+norm_cations['Al_Amp_cat_23ox'])<8
-    norm_cations.loc[(Si_Ti_sum_less8), 'Al_T_Amp']=norm_cations['Al_Amp_cat_23ox']
-    norm_cations.loc[(Si_Ti_sum_less8), 'Al_C_Amp']=0
+    norm_cations.loc[(Si_Ti_sum_gr8), "Al_C_Amp"] = (
+        norm_cations["Al_Amp_cat_23ox"] - norm_cations["Al_T_Amp"]
+    )
+
+    # If Si+Al<8, put all Al in tetrahedlra sites
+    Si_Ti_sum_less8 = (
+        norm_cations["Si_Amp_cat_23ox"] + norm_cations["Al_Amp_cat_23ox"]
+    ) < 8
+    norm_cations.loc[(Si_Ti_sum_less8), "Al_T_Amp"] = norm_cations["Al_Amp_cat_23ox"]
+    norm_cations.loc[(Si_Ti_sum_less8), "Al_C_Amp"] = 0
 
     # 5b) Leake Octaherdal C sites.
-    #already filled some with Al in lines above. Place Ti (unambg), Cr (unamb).
+    # already filled some with Al in lines above. Place Ti (unambg), Cr (unamb).
     # Fill sites with Mg, Fe, and Mn to bring total to 5.
 
     # If Sites sum to less than 5, place all elements here
-    Al_Ti_Cr_Mg_Fe_Mn_less5=(norm_cations['Al_C_Amp']+norm_cations['Ti_Amp_cat_23ox']+norm_cations['Fet_Amp_cat_23ox']+norm_cations['Cr_Amp_cat_23ox']+norm_cations['Mn_Amp_cat_23ox']+norm_cations['Mg_Amp_cat_23ox'])<5
-
-    norm_cations.loc[(Al_Ti_Cr_Mg_Fe_Mn_less5), 'Fe_C_Amp']=norm_cations['Fet_Amp_cat_23ox']
-    norm_cations.loc[(Al_Ti_Cr_Mg_Fe_Mn_less5), 'Mn_C_Amp']=norm_cations['Mn_Amp_cat_23ox']
-    norm_cations.loc[(Al_Ti_Cr_Mg_Fe_Mn_less5), 'Mg_C_Amp']=norm_cations['Mg_Amp_cat_23ox']
-
-
-    #If sites sum to more than 5, after placing Ti and Cr here, fill rest with Mg, Fe and Mn
-    Al_Ti_Cr_Mg_Fe_Mn_more5=(norm_cations['Al_C_Amp']+norm_cations['Ti_Amp_cat_23ox']+norm_cations['Fet_Amp_cat_23ox']+norm_cations['Cr_Amp_cat_23ox']+norm_cations['Mn_Amp_cat_23ox']+norm_cations['Mg_Amp_cat_23ox'])>5
+    Al_Ti_Cr_Mg_Fe_Mn_less5 = (
+        norm_cations["Al_C_Amp"]
+        + norm_cations["Ti_Amp_cat_23ox"]
+        + norm_cations["Fet_Amp_cat_23ox"]
+        + norm_cations["Cr_Amp_cat_23ox"]
+        + norm_cations["Mn_Amp_cat_23ox"]
+        + norm_cations["Mg_Amp_cat_23ox"]
+    ) < 5
+
+    norm_cations.loc[(Al_Ti_Cr_Mg_Fe_Mn_less5), "Fe_C_Amp"] = norm_cations[
+        "Fet_Amp_cat_23ox"
+    ]
+    norm_cations.loc[(Al_Ti_Cr_Mg_Fe_Mn_less5), "Mn_C_Amp"] = norm_cations[
+        "Mn_Amp_cat_23ox"
+    ]
+    norm_cations.loc[(Al_Ti_Cr_Mg_Fe_Mn_less5), "Mg_C_Amp"] = norm_cations[
+        "Mg_Amp_cat_23ox"
+    ]
+
+    # If sites sum to more than 5, after placing Ti and Cr here, fill rest with Mg, Fe and Mn
+    Al_Ti_Cr_Mg_Fe_Mn_more5 = (
+        norm_cations["Al_C_Amp"]
+        + norm_cations["Ti_Amp_cat_23ox"]
+        + norm_cations["Fet_Amp_cat_23ox"]
+        + norm_cations["Cr_Amp_cat_23ox"]
+        + norm_cations["Mn_Amp_cat_23ox"]
+        + norm_cations["Mg_Amp_cat_23ox"]
+    ) > 5
 
     # First, check if Al+Cr+Ti sum to 5. If not, allocate Mg
-    sum_C_Al_Cr_Ti=norm_cations['Al_C_Amp']+norm_cations['Cr_C_Amp']+norm_cations['Ti_C_Amp']
-    check_C_Al_Cr_Ti=sum_C_Al_Cr_Ti<5
-    norm_cations.loc[((Al_Ti_Cr_Mg_Fe_Mn_more5)&(check_C_Al_Cr_Ti)), 'Mg_C_Amp']=norm_cations['Mg_Amp_cat_23ox']
+    sum_C_Al_Cr_Ti = (
+        norm_cations["Al_C_Amp"] + norm_cations["Cr_C_Amp"] + norm_cations["Ti_C_Amp"]
+    )
+    check_C_Al_Cr_Ti = sum_C_Al_Cr_Ti < 5
+    norm_cations.loc[
+        ((Al_Ti_Cr_Mg_Fe_Mn_more5) & (check_C_Al_Cr_Ti)), "Mg_C_Amp"
+    ] = norm_cations["Mg_Amp_cat_23ox"]
 
     # Now check you haven't added too much MgO to take you over 5
-    sum_C_Al_Cr_Ti_Mg=norm_cations['Al_C_Amp']+norm_cations['Cr_C_Amp']+norm_cations['Ti_C_Amp']+norm_cations['Mg_C_Amp']
-    check_C_Al_Cr_Ti_Mg_low=sum_C_Al_Cr_Ti_Mg<=5
-    check_C_Al_Cr_Ti_Mg_high=sum_C_Al_Cr_Ti_Mg>5
+    sum_C_Al_Cr_Ti_Mg = (
+        norm_cations["Al_C_Amp"]
+        + norm_cations["Cr_C_Amp"]
+        + norm_cations["Ti_C_Amp"]
+        + norm_cations["Mg_C_Amp"]
+    )
+    check_C_Al_Cr_Ti_Mg_low = sum_C_Al_Cr_Ti_Mg <= 5
+    check_C_Al_Cr_Ti_Mg_high = sum_C_Al_Cr_Ti_Mg > 5
     # If sum is >5, replace Mg with only the magnesium left needed to get to 5.
-    norm_cations.loc[((Al_Ti_Cr_Mg_Fe_Mn_more5)&(check_C_Al_Cr_Ti_Mg_high)), 'Mg_C_Amp']=5-sum_C_Al_Cr_Ti
+    norm_cations.loc[
+        ((Al_Ti_Cr_Mg_Fe_Mn_more5) & (check_C_Al_Cr_Ti_Mg_high)), "Mg_C_Amp"
+    ] = 5 - sum_C_Al_Cr_Ti
 
     # Now check if you are back under 5 again,  ready to allocate Fe
-    sum_C_Al_Cr_Ti_Mg2=norm_cations['Al_C_Amp']+norm_cations['Cr_C_Amp']+norm_cations['Ti_C_Amp']+norm_cations['Mg_C_Amp']
-    check_C_Al_Cr_Ti_Mg_low2=sum_C_Al_Cr_Ti_Mg2<5
-    norm_cations.loc[((Al_Ti_Cr_Mg_Fe_Mn_more5)&(check_C_Al_Cr_Ti_Mg_low2)), 'Fe_C_Amp']=norm_cations['Fet_Amp_cat_23ox']
+    sum_C_Al_Cr_Ti_Mg2 = (
+        norm_cations["Al_C_Amp"]
+        + norm_cations["Cr_C_Amp"]
+        + norm_cations["Ti_C_Amp"]
+        + norm_cations["Mg_C_Amp"]
+    )
+    check_C_Al_Cr_Ti_Mg_low2 = sum_C_Al_Cr_Ti_Mg2 < 5
+    norm_cations.loc[
+        ((Al_Ti_Cr_Mg_Fe_Mn_more5) & (check_C_Al_Cr_Ti_Mg_low2)), "Fe_C_Amp"
+    ] = norm_cations["Fet_Amp_cat_23ox"]
 
     # Now check you haven't added too much FeO to take you over 5
-    sum_C_Al_Cr_Ti_Mg_Fe=(norm_cations['Al_C_Amp']+norm_cations['Cr_C_Amp']
-    +norm_cations['Ti_C_Amp']+norm_cations['Mg_C_Amp']+norm_cations['Fe_C_Amp'])
-    check_C_Al_Cr_Ti_Mg_Fe_low=sum_C_Al_Cr_Ti_Mg_Fe<=5
-    check_C_Al_Cr_Ti_Mg_Fe_high=sum_C_Al_Cr_Ti_Mg_Fe>5
+    sum_C_Al_Cr_Ti_Mg_Fe = (
+        norm_cations["Al_C_Amp"]
+        + norm_cations["Cr_C_Amp"]
+        + norm_cations["Ti_C_Amp"]
+        + norm_cations["Mg_C_Amp"]
+        + norm_cations["Fe_C_Amp"]
+    )
+    check_C_Al_Cr_Ti_Mg_Fe_low = sum_C_Al_Cr_Ti_Mg_Fe <= 5
+    check_C_Al_Cr_Ti_Mg_Fe_high = sum_C_Al_Cr_Ti_Mg_Fe > 5
     # If sum is >5, replace Fe with only the Fe left needed to get to 5.
-    norm_cations.loc[((Al_Ti_Cr_Mg_Fe_Mn_more5)&(check_C_Al_Cr_Ti_Mg_Fe_high)), 'Fe_C_Amp']=5-sum_C_Al_Cr_Ti_Mg2
+    norm_cations.loc[
+        ((Al_Ti_Cr_Mg_Fe_Mn_more5) & (check_C_Al_Cr_Ti_Mg_Fe_high)), "Fe_C_Amp"
+    ] = 5 - sum_C_Al_Cr_Ti_Mg2
 
     # Now check if you are back under 5 again,  ready to allocate Mn
-    sum_C_Al_Cr_Ti_Mg_Fe2=(norm_cations['Al_C_Amp']+norm_cations['Cr_C_Amp']+norm_cations['Ti_C_Amp']
-    +norm_cations['Mg_C_Amp']+norm_cations['Fe_C_Amp'])
-    check_C_Al_Cr_Ti_Mg_Fe_low2=sum_C_Al_Cr_Ti_Mg_Fe2<5
-    norm_cations.loc[((Al_Ti_Cr_Mg_Fe_Mn_more5)&(check_C_Al_Cr_Ti_Mg_Fe_low2)), 'Mn_C_Amp']=norm_cations['Mn_Amp_cat_23ox']
+    sum_C_Al_Cr_Ti_Mg_Fe2 = (
+        norm_cations["Al_C_Amp"]
+        + norm_cations["Cr_C_Amp"]
+        + norm_cations["Ti_C_Amp"]
+        + norm_cations["Mg_C_Amp"]
+        + norm_cations["Fe_C_Amp"]
+    )
+    check_C_Al_Cr_Ti_Mg_Fe_low2 = sum_C_Al_Cr_Ti_Mg_Fe2 < 5
+    norm_cations.loc[
+        ((Al_Ti_Cr_Mg_Fe_Mn_more5) & (check_C_Al_Cr_Ti_Mg_Fe_low2)), "Mn_C_Amp"
+    ] = norm_cations["Mn_Amp_cat_23ox"]
 
     # Now check you haven't added too much Mn to take you over 5
-    sum_C_Al_Cr_Ti_Mg_Fe_Mn=(norm_cations['Al_C_Amp']+norm_cations['Cr_C_Amp']
-    +norm_cations['Ti_C_Amp']+norm_cations['Mg_C_Amp']+norm_cations['Fe_C_Amp']+norm_cations['Mn_C_Amp'])
-    check_C_Al_Cr_Ti_Mg_Fe_Mn_low=sum_C_Al_Cr_Ti_Mg_Fe_Mn<=5
-    check_C_Al_Cr_Ti_Mg_Fe_Mn_high=sum_C_Al_Cr_Ti_Mg_Fe_Mn>5
+    sum_C_Al_Cr_Ti_Mg_Fe_Mn = (
+        norm_cations["Al_C_Amp"]
+        + norm_cations["Cr_C_Amp"]
+        + norm_cations["Ti_C_Amp"]
+        + norm_cations["Mg_C_Amp"]
+        + norm_cations["Fe_C_Amp"]
+        + norm_cations["Mn_C_Amp"]
+    )
+    check_C_Al_Cr_Ti_Mg_Fe_Mn_low = sum_C_Al_Cr_Ti_Mg_Fe_Mn <= 5
+    check_C_Al_Cr_Ti_Mg_Fe_Mn_high = sum_C_Al_Cr_Ti_Mg_Fe_Mn > 5
     # If sum is >5, replace Mn with only the Mn left needed to get to 5.
-    norm_cations.loc[((Al_Ti_Cr_Mg_Fe_Mn_more5)&(check_C_Al_Cr_Ti_Mg_Fe_Mn_high)), 'Mn_C_Amp']=5-sum_C_Al_Cr_Ti_Mg_Fe2
-
+    norm_cations.loc[
+        ((Al_Ti_Cr_Mg_Fe_Mn_more5) & (check_C_Al_Cr_Ti_Mg_Fe_Mn_high)), "Mn_C_Amp"
+    ] = 5 - sum_C_Al_Cr_Ti_Mg_Fe2
 
     # 5c) Leake. B Sites-
     # if any Mg, Fe, Mn or Ca remaining put here;
-    Mg_remaining=norm_cations['Mg_Amp_cat_23ox']-norm_cations['Mg_C_Amp']
-    Fe_remaining=norm_cations['Fet_Amp_cat_23ox']-norm_cations['Fe_C_Amp']
-    Mn_remaining=norm_cations['Mn_Amp_cat_23ox']-norm_cations['Mn_C_Amp']
-
-    norm_cations['Mg_B_Amp']= Mg_remaining
-    norm_cations['Fe_B_Amp']= Fe_remaining
-    norm_cations['Mn_B_Amp']= Mn_remaining
+    Mg_remaining = norm_cations["Mg_Amp_cat_23ox"] - norm_cations["Mg_C_Amp"]
+    Fe_remaining = norm_cations["Fet_Amp_cat_23ox"] - norm_cations["Fe_C_Amp"]
+    Mn_remaining = norm_cations["Mn_Amp_cat_23ox"] - norm_cations["Mn_C_Amp"]
+
+    norm_cations["Mg_B_Amp"] = Mg_remaining
+    norm_cations["Fe_B_Amp"] = Fe_remaining
+    norm_cations["Mn_B_Amp"] = Mn_remaining
 
     # If B sites sum to less than 2, fill sites with Ca to bring total to 2
 
     # If B sites sum to less than 2, fill sites with Na to bring total to 2
 
-    Sum_B=norm_cations['Mg_B_Amp']+norm_cations['Fe_B_Amp']+norm_cations['Mn_B_Amp']+norm_cations['Ca_B_Amp']
-    Left_to_fill_B=2- Sum_B
+    Sum_B = (
+        norm_cations["Mg_B_Amp"]
+        + norm_cations["Fe_B_Amp"]
+        + norm_cations["Mn_B_Amp"]
+        + norm_cations["Ca_B_Amp"]
+    )
+    Left_to_fill_B = 2 - Sum_B
     # Check there is actually enough Na to fill B this way fully, if so allocate the amount you need
-    Enough_Na=norm_cations['Na_Amp_cat_23ox']>=Left_to_fill_B
-    norm_cations.loc[((Sum_B<2)&(Enough_Na)), 'Na_B_Amp']=Left_to_fill_B
+    Enough_Na = norm_cations["Na_Amp_cat_23ox"] >= Left_to_fill_B
+    norm_cations.loc[((Sum_B < 2) & (Enough_Na)), "Na_B_Amp"] = Left_to_fill_B
     #  If there isn't enough Na2O, allocate all Na2O you have
-    norm_cations.loc[((Sum_B<2)&(~Enough_Na)), 'Na_B_Amp']=norm_cations['Na_Amp_cat_23ox']
-    Na_left_AfterB=norm_cations['Na_Amp_cat_23ox']-norm_cations['Na_B_Amp']
+    norm_cations.loc[((Sum_B < 2) & (~Enough_Na)), "Na_B_Amp"] = norm_cations[
+        "Na_Amp_cat_23ox"
+    ]
+    Na_left_AfterB = norm_cations["Na_Amp_cat_23ox"] - norm_cations["Na_B_Amp"]
 
     # A sites
-    norm_cations['K_A_Amp']=norm_cations['K_Amp_cat_23ox']
-    norm_cations['Na_A_Amp']=Na_left_AfterB
-
-    norm_cations['Sum_T']=norm_cations['Al_T_Amp']+norm_cations['Si_T_Amp']
-    norm_cations['Sum_C']=(norm_cations['Al_C_Amp']+norm_cations['Cr_C_Amp']+norm_cations['Mg_C_Amp']+norm_cations['Fe_C_Amp']+norm_cations['Mn_C_Amp'])
-    norm_cations['Sum_B']=(norm_cations['Mg_B_Amp']+norm_cations['Fe_B_Amp']+norm_cations['Mn_B_Amp']+norm_cations['Ca_B_Amp']+norm_cations['Na_B_Amp'])
-    norm_cations['Sum_A']=norm_cations['K_A_Amp']+norm_cations['Na_A_Amp']
+    norm_cations["K_A_Amp"] = norm_cations["K_Amp_cat_23ox"]
+    norm_cations["Na_A_Amp"] = Na_left_AfterB
 
-    norm_cations['Amp_Cation_Sum'] = norm_cations['cation_sum_Si_Ca'] + norm_cations['Na_Amp_cat_23ox'] + +norm_cations['K_Amp_cat_23ox']
-    norm_cations['Mgno_Amp']=norm_cations['Mg_Amp_cat_23ox']/(norm_cations['Mg_Amp_cat_23ox']+norm_cations['Fet_Amp_cat_23ox'])
+    norm_cations["Sum_T"] = norm_cations["Al_T_Amp"] + norm_cations["Si_T_Amp"]
+    norm_cations["Sum_C"] = (
+        norm_cations["Al_C_Amp"]
+        + norm_cations["Cr_C_Amp"]
+        + norm_cations["Mg_C_Amp"]
+        + norm_cations["Fe_C_Amp"]
+        + norm_cations["Mn_C_Amp"]
+    )
+    norm_cations["Sum_B"] = (
+        norm_cations["Mg_B_Amp"]
+        + norm_cations["Fe_B_Amp"]
+        + norm_cations["Mn_B_Amp"]
+        + norm_cations["Ca_B_Amp"]
+        + norm_cations["Na_B_Amp"]
+    )
+    norm_cations["Sum_A"] = norm_cations["K_A_Amp"] + norm_cations["Na_A_Amp"]
+
+    norm_cations["Amp_Cation_Sum"] = (
+        norm_cations["cation_sum_Si_Ca"]
+        + norm_cations["Na_Amp_cat_23ox"]
+        + +norm_cations["K_Amp_cat_23ox"]
+    )
+    norm_cations["Mgno_Amp"] = norm_cations["Mg_Amp_cat_23ox"] / (
+        norm_cations["Mg_Amp_cat_23ox"] + norm_cations["Fet_Amp_cat_23ox"]
+    )
 
-    #norm_cations['factor']=np.max()
+    # norm_cations['factor']=np.max()
     # Ones being used, uses FW for Si, Fy,
     return norm_cations
 
 
 def get_amp_sites_avferric_zhang(amp_comps):
-
-    norm_cations=get_amp_sites_from_input(amp_comps)
+    norm_cations = get_amp_sites_from_input(amp_comps)
 
     # Taken from Zhang et al. 2017 Supplement
-    norm_cations['factor_8SiAl']=8/(norm_cations['Si_Amp_cat_23ox']+norm_cations['Al_Amp_cat_23ox'])
+    norm_cations["factor_8SiAl"] = 8 / (
+        norm_cations["Si_Amp_cat_23ox"] + norm_cations["Al_Amp_cat_23ox"]
+    )
+
+    norm_cations["factor_15eK"] = 15 / (
+        norm_cations["Si_Amp_cat_23ox"]
+        + norm_cations["Ti_Amp_cat_23ox"]
+        + norm_cations["Al_Amp_cat_23ox"]
+        + norm_cations["Cr_Amp_cat_23ox"]
+        + +norm_cations["Fet_Amp_cat_23ox"]
+        + norm_cations["Mg_Amp_cat_23ox"]
+        + norm_cations["Ca_Amp_cat_23ox"]
+        + norm_cations["Mn_Amp_cat_23ox"]
+        + norm_cations["Na_Amp_cat_23ox"]
+    )
+
+    norm_cations["factor_13eCNK"] = 13 / (
+        norm_cations["Si_Amp_cat_23ox"]
+        + norm_cations["Ti_Amp_cat_23ox"]
+        + norm_cations["Al_Amp_cat_23ox"]
+        + norm_cations["Cr_Amp_cat_23ox"]
+        + norm_cations["Fet_Amp_cat_23ox"]
+        + norm_cations["Mg_Amp_cat_23ox"]
+        + norm_cations["Ca_Amp_cat_23ox"]
+        + norm_cations["Mn_Amp_cat_23ox"]
+    )
 
-    norm_cations['factor_15eK']=(15/(norm_cations['Si_Amp_cat_23ox']+norm_cations['Ti_Amp_cat_23ox']+norm_cations['Al_Amp_cat_23ox']+norm_cations['Cr_Amp_cat_23ox']++norm_cations['Fet_Amp_cat_23ox']+norm_cations['Mg_Amp_cat_23ox']+norm_cations['Ca_Amp_cat_23ox']+norm_cations['Mn_Amp_cat_23ox']+norm_cations['Na_Amp_cat_23ox']))
-
-    norm_cations['factor_13eCNK']=13/((norm_cations['Si_Amp_cat_23ox']+norm_cations['Ti_Amp_cat_23ox']+norm_cations['Al_Amp_cat_23ox']+norm_cations['Cr_Amp_cat_23ox']+norm_cations['Fet_Amp_cat_23ox']+norm_cations['Mg_Amp_cat_23ox']+norm_cations['Ca_Amp_cat_23ox']+norm_cations['Mn_Amp_cat_23ox']))
-
-    norm_cations['All ferric']=23/(23+(0.5*norm_cations['Fet_Amp_cat_23ox']))
+    norm_cations["All ferric"] = 23 / (23 + (0.5 * norm_cations["Fet_Amp_cat_23ox"]))
 
     # Minimum Factors
-    norm_cations['8Si_Min']=8/norm_cations['Si_Amp_cat_23ox']
-
-    norm_cations['16CAT_Min']=(16/(norm_cations['Si_Amp_cat_23ox']+norm_cations['Ti_Amp_cat_23ox']+norm_cations['Al_Amp_cat_23ox']+norm_cations['Cr_Amp_cat_23ox']++norm_cations['Fet_Amp_cat_23ox']+norm_cations['Mg_Amp_cat_23ox']+norm_cations['Ca_Amp_cat_23ox']+norm_cations['Mn_Amp_cat_23ox']+norm_cations['Na_Amp_cat_23ox']+norm_cations['K_Amp_cat_23ox']))
-
-    norm_cations['15eNK_Min']=15/((norm_cations['Si_Amp_cat_23ox']+norm_cations['Ti_Amp_cat_23ox']+norm_cations['Al_Amp_cat_23ox']+norm_cations['Cr_Amp_cat_23ox']+norm_cations['Fet_Amp_cat_23ox']+norm_cations['Mg_Amp_cat_23ox']+norm_cations['Ca_Amp_cat_23ox']+norm_cations['Mn_Amp_cat_23ox']))
-
-    norm_cations['Min_MinFactor']=norm_cations[['8Si_Min', '16CAT_Min', '15eNK_Min']].min(axis=1)
-
-
-    #If Min_MinFactor<1, allocate to min factor
-    norm_cations['Min_factor']=norm_cations['Min_MinFactor']
-    Min_Min_Factor_g1=norm_cations['Min_MinFactor']>1
-    norm_cations.loc[Min_Min_Factor_g1, 'Min_factor']=1
-
-    norm_cations['Max_factor']=norm_cations[['factor_8SiAl', 'factor_15eK', 'factor_13eCNK', 'All ferric']].max(axis=1)
-
-    norm_cations['Av_factor']=0.5*(norm_cations['Max_factor']+norm_cations['Min_factor'])
+    norm_cations["8Si_Min"] = 8 / norm_cations["Si_Amp_cat_23ox"]
 
+    norm_cations["16CAT_Min"] = 16 / (
+        norm_cations["Si_Amp_cat_23ox"]
+        + norm_cations["Ti_Amp_cat_23ox"]
+        + norm_cations["Al_Amp_cat_23ox"]
+        + norm_cations["Cr_Amp_cat_23ox"]
+        + +norm_cations["Fet_Amp_cat_23ox"]
+        + norm_cations["Mg_Amp_cat_23ox"]
+        + norm_cations["Ca_Amp_cat_23ox"]
+        + norm_cations["Mn_Amp_cat_23ox"]
+        + norm_cations["Na_Amp_cat_23ox"]
+        + norm_cations["K_Amp_cat_23ox"]
+    )
+
+    norm_cations["15eNK_Min"] = 15 / (
+        norm_cations["Si_Amp_cat_23ox"]
+        + norm_cations["Ti_Amp_cat_23ox"]
+        + norm_cations["Al_Amp_cat_23ox"]
+        + norm_cations["Cr_Amp_cat_23ox"]
+        + norm_cations["Fet_Amp_cat_23ox"]
+        + norm_cations["Mg_Amp_cat_23ox"]
+        + norm_cations["Ca_Amp_cat_23ox"]
+        + norm_cations["Mn_Amp_cat_23ox"]
+    )
+
+    norm_cations["Min_MinFactor"] = norm_cations[
+        ["8Si_Min", "16CAT_Min", "15eNK_Min"]
+    ].min(axis=1)
+
+    # If Min_MinFactor<1, allocate to min factor
+    norm_cations["Min_factor"] = norm_cations["Min_MinFactor"]
+    Min_Min_Factor_g1 = norm_cations["Min_MinFactor"] > 1
+    norm_cations.loc[Min_Min_Factor_g1, "Min_factor"] = 1
+
+    norm_cations["Max_factor"] = norm_cations[
+        ["factor_8SiAl", "factor_15eK", "factor_13eCNK", "All ferric"]
+    ].max(axis=1)
+
+    norm_cations["Av_factor"] = 0.5 * (
+        norm_cations["Max_factor"] + norm_cations["Min_factor"]
+    )
 
     # Then things times by factors
-    Si_factor=norm_cations['Av_factor']*norm_cations['Si_Amp_cat_23ox']
-    Ti_factor=norm_cations['Av_factor']*norm_cations['Ti_Amp_cat_23ox']
-    Al_factor=norm_cations['Av_factor']*norm_cations['Al_Amp_cat_23ox']
-    Cr_factor=norm_cations['Av_factor']*norm_cations['Cr_Amp_cat_23ox']
-    Fe_factor=norm_cations['Av_factor']*norm_cations['Fet_Amp_cat_23ox']
-    Mg_factor=norm_cations['Av_factor']*norm_cations['Mg_Amp_cat_23ox']
-    Ca_factor=norm_cations['Av_factor']*norm_cations['Ca_Amp_cat_23ox']
-    Mn_factor=norm_cations['Av_factor']*norm_cations['Mn_Amp_cat_23ox']
-    Na_factor=norm_cations['Av_factor']*norm_cations['Na_Amp_cat_23ox']
-    K_factor=norm_cations['Av_factor']*norm_cations['K_Amp_cat_23ox']
-
-    norm_cations['Si_T_ideal']=norm_cations['Av_factor']*norm_cations['Si_Amp_cat_23ox']
+    Si_factor = norm_cations["Av_factor"] * norm_cations["Si_Amp_cat_23ox"]
+    Ti_factor = norm_cations["Av_factor"] * norm_cations["Ti_Amp_cat_23ox"]
+    Al_factor = norm_cations["Av_factor"] * norm_cations["Al_Amp_cat_23ox"]
+    Cr_factor = norm_cations["Av_factor"] * norm_cations["Cr_Amp_cat_23ox"]
+    Fe_factor = norm_cations["Av_factor"] * norm_cations["Fet_Amp_cat_23ox"]
+    Mg_factor = norm_cations["Av_factor"] * norm_cations["Mg_Amp_cat_23ox"]
+    Ca_factor = norm_cations["Av_factor"] * norm_cations["Ca_Amp_cat_23ox"]
+    Mn_factor = norm_cations["Av_factor"] * norm_cations["Mn_Amp_cat_23ox"]
+    Na_factor = norm_cations["Av_factor"] * norm_cations["Na_Amp_cat_23ox"]
+    K_factor = norm_cations["Av_factor"] * norm_cations["K_Amp_cat_23ox"]
+
+    norm_cations["Si_T_ideal"] = (
+        norm_cations["Av_factor"] * norm_cations["Si_Amp_cat_23ox"]
+    )
     # Allocate Al to Tetrahedral. If 8-Si_T< Al_factor, equal to 8-Si_T
 
-    norm_cations['Al_IV_T_ideal']=8-norm_cations['Si_T_ideal']
+    norm_cations["Al_IV_T_ideal"] = 8 - norm_cations["Si_T_ideal"]
     # But if 8-SiT>Al factor, allocate all Al_Factor
-    eight_m_siT_g=(8-norm_cations['Si_T_ideal'])>Al_factor
-    norm_cations.loc[ eight_m_siT_g, 'Al_IV_T_ideal']=Al_factor
+    eight_m_siT_g = (8 - norm_cations["Si_T_ideal"]) > Al_factor
+    norm_cations.loc[eight_m_siT_g, "Al_IV_T_ideal"] = Al_factor
     # And if SiT>8, allocate to zero
-    Si_T_g_8= norm_cations['Si_T_ideal']>8
-    norm_cations.loc[Si_T_g_8, 'Al_IV_T_ideal']=0
+    Si_T_g_8 = norm_cations["Si_T_ideal"] > 8
+    norm_cations.loc[Si_T_g_8, "Al_IV_T_ideal"] = 0
 
     # Ti sites, if Si + Al>8, allocate 0 (as all filled up)
-    norm_cations['Ti_T_ideal']=0
+    norm_cations["Ti_T_ideal"] = 0
     # If Si and Al<8, if 8-Si-Al is > Ti_factor, Ti Factor (as all Ti can go in site)
-    Si_Al_l8=(norm_cations['Si_T_ideal']+norm_cations['Al_IV_T_ideal'])<8
-    eight_Si_Ti_gTiFactor=(8-norm_cations['Si_T_ideal']-norm_cations['Al_IV_T_ideal'])>Ti_factor
-    norm_cations.loc[(( Si_Al_l8)&(eight_Si_Ti_gTiFactor)), 'Ti_T_ideal']=Ti_factor
-    norm_cations.loc[(( Si_Al_l8)&(~eight_Si_Ti_gTiFactor)), 'Ti_T_ideal']=(8-norm_cations['Si_T_ideal']-norm_cations['Al_IV_T_ideal'])
+    Si_Al_l8 = (norm_cations["Si_T_ideal"] + norm_cations["Al_IV_T_ideal"]) < 8
+    eight_Si_Ti_gTiFactor = (
+        8 - norm_cations["Si_T_ideal"] - norm_cations["Al_IV_T_ideal"]
+    ) > Ti_factor
+    norm_cations.loc[((Si_Al_l8) & (eight_Si_Ti_gTiFactor)), "Ti_T_ideal"] = Ti_factor
+    norm_cations.loc[((Si_Al_l8) & (~eight_Si_Ti_gTiFactor)), "Ti_T_ideal"] = (
+        8 - norm_cations["Si_T_ideal"] - norm_cations["Al_IV_T_ideal"]
+    )
 
     # Al VI C site
-    norm_cations['Al_VI_C_ideal']=Al_factor-norm_cations['Al_IV_T_ideal']
+    norm_cations["Al_VI_C_ideal"] = Al_factor - norm_cations["Al_IV_T_ideal"]
     # Unless Alfactor-Al_VI equal to or less than zero, in which case none left
-    Alfactor_Al_l0=(Al_factor-norm_cations['Al_IV_T_ideal'])<=0
-    norm_cations.loc[(Alfactor_Al_l0), 'Al_VI_C_ideal']=0
+    Alfactor_Al_l0 = (Al_factor - norm_cations["Al_IV_T_ideal"]) <= 0
+    norm_cations.loc[(Alfactor_Al_l0), "Al_VI_C_ideal"] = 0
 
     # Ti C site. If Ti Factor + Al_VI_C_ideal<5, equal to Ti Factor
-    norm_cations['Ti_C_ideal']=Ti_factor
+    norm_cations["Ti_C_ideal"] = Ti_factor
     # Else if >5, equal to 5-Al VI
-    Ti_fac_Al_VI_g5=(Ti_factor+ norm_cations['Al_VI_C_ideal'])>5
-    norm_cations.loc[(Ti_fac_Al_VI_g5), 'Ti_C_ideal']=5-norm_cations['Al_VI_C_ideal']
+    Ti_fac_Al_VI_g5 = (Ti_factor + norm_cations["Al_VI_C_ideal"]) > 5
+    norm_cations.loc[(Ti_fac_Al_VI_g5), "Ti_C_ideal"] = (
+        5 - norm_cations["Al_VI_C_ideal"]
+    )
 
     # Cr C site. If Al_C + Ti_C + Cr Factor . Equal to Cr factor
-    norm_cations['Cr_C_ideal']=Cr_factor
-    C_Al_Ti_Cr_g5=(norm_cations['Ti_C_ideal']+ norm_cations['Al_VI_C_ideal']+Cr_factor)>5
-    norm_cations.loc[(C_Al_Ti_Cr_g5), 'Cr_C_ideal']=5-norm_cations['Al_VI_C_ideal']-norm_cations['Ti_C_ideal']
+    norm_cations["Cr_C_ideal"] = Cr_factor
+    C_Al_Ti_Cr_g5 = (
+        norm_cations["Ti_C_ideal"] + norm_cations["Al_VI_C_ideal"] + Cr_factor
+    ) > 5
+    norm_cations.loc[(C_Al_Ti_Cr_g5), "Cr_C_ideal"] = (
+        5 - norm_cations["Al_VI_C_ideal"] - norm_cations["Ti_C_ideal"]
+    )
 
     #  Fe3 C site
-    NewSum=(Si_factor*2+Ti_factor*2+Al_factor*3/2+Cr_factor*3/2+Fe_factor+Mg_factor+Ca_factor+Mn_factor+Na_factor/2+K_factor/2)
-    norm_cations['Fe3_C_ideal']=(23-NewSum)*2
+    NewSum = (
+        Si_factor * 2
+        + Ti_factor * 2
+        + Al_factor * 3 / 2
+        + Cr_factor * 3 / 2
+        + Fe_factor
+        + Mg_factor
+        + Ca_factor
+        + Mn_factor
+        + Na_factor / 2
+        + K_factor / 2
+    )
+    norm_cations["Fe3_C_ideal"] = (23 - NewSum) * 2
 
     # Mg C site - If Al, Ti, Fe3, Cr already 5, set to zero
-    norm_cations['Mg_C_ideal']=0
+    norm_cations["Mg_C_ideal"] = 0
 
     # If sum not 5, if sum + Mg<5, allocate Mg factor, else do 5- sum
-    Sum_beforeMgC=(norm_cations['Ti_C_ideal']+ norm_cations['Al_VI_C_ideal']
-    +norm_cations['Cr_C_ideal']+norm_cations['Fe3_C_ideal'])
-    Sum_beforeMgC_l5=Sum_beforeMgC<5
-    Sum_beforeMgC_Mg_l5=(Sum_beforeMgC+Mg_factor)<5
-    norm_cations.loc[((Sum_beforeMgC_l5)&(Sum_beforeMgC_Mg_l5)), 'Mg_C_ideal']=Mg_factor
-    norm_cations.loc[((Sum_beforeMgC_l5)&(~Sum_beforeMgC_Mg_l5)), 'Mg_C_ideal']=5-Sum_beforeMgC_l5
+    Sum_beforeMgC = (
+        norm_cations["Ti_C_ideal"]
+        + norm_cations["Al_VI_C_ideal"]
+        + norm_cations["Cr_C_ideal"]
+        + norm_cations["Fe3_C_ideal"]
+    )
+    Sum_beforeMgC_l5 = Sum_beforeMgC < 5
+    Sum_beforeMgC_Mg_l5 = (Sum_beforeMgC + Mg_factor) < 5
+    norm_cations.loc[
+        ((Sum_beforeMgC_l5) & (Sum_beforeMgC_Mg_l5)), "Mg_C_ideal"
+    ] = Mg_factor
+    norm_cations.loc[((Sum_beforeMgC_l5) & (~Sum_beforeMgC_Mg_l5)), "Mg_C_ideal"] = (
+        5 - Sum_beforeMgC_l5
+    )
 
     # Fe2_C site. If revious sum>5, alocate zero
-    norm_cations['Fe2_C_ideal']=0
+    norm_cations["Fe2_C_ideal"] = 0
     # If previous sum<5
-    Sum_beforeFeC=(norm_cations['Ti_C_ideal']+ norm_cations['Al_VI_C_ideal']+norm_cations['Cr_C_ideal']+norm_cations['Fe3_C_ideal']+norm_cations['Mg_C_ideal'])
-    Sum_beforeFeC_l5=Sum_beforeFeC<5
-    Sum_beforeFeC_Fe_l5=(Sum_beforeFeC+(Fe_factor-norm_cations['Fe3_C_ideal']))<5
-    norm_cations.loc[((Sum_beforeFeC_l5)&(Sum_beforeFeC_Fe_l5)), 'Fe2_C_ideal']=Fe_factor-norm_cations['Fe3_C_ideal']
-    norm_cations.loc[((Sum_beforeFeC_l5)&(~Sum_beforeFeC_Fe_l5)), 'Fe2_C_ideal']=5- Sum_beforeFeC
+    Sum_beforeFeC = (
+        norm_cations["Ti_C_ideal"]
+        + norm_cations["Al_VI_C_ideal"]
+        + norm_cations["Cr_C_ideal"]
+        + norm_cations["Fe3_C_ideal"]
+        + norm_cations["Mg_C_ideal"]
+    )
+    Sum_beforeFeC_l5 = Sum_beforeFeC < 5
+    Sum_beforeFeC_Fe_l5 = (
+        Sum_beforeFeC + (Fe_factor - norm_cations["Fe3_C_ideal"])
+    ) < 5
+    norm_cations.loc[((Sum_beforeFeC_l5) & (Sum_beforeFeC_Fe_l5)), "Fe2_C_ideal"] = (
+        Fe_factor - norm_cations["Fe3_C_ideal"]
+    )
+    norm_cations.loc[((Sum_beforeFeC_l5) & (~Sum_beforeFeC_Fe_l5)), "Fe2_C_ideal"] = (
+        5 - Sum_beforeFeC
+    )
 
     # Mn Site, if sum>=5, set to zero
-    norm_cations['Mn_C_ideal']=0
+    norm_cations["Mn_C_ideal"] = 0
     # IF previous sum <5
-    Sum_beforeMnC=(norm_cations['Ti_C_ideal']+ norm_cations['Al_VI_C_ideal']+norm_cations['Cr_C_ideal']+norm_cations['Fe3_C_ideal']+norm_cations['Mg_C_ideal']+norm_cations['Fe2_C_ideal'])
-    Sum_beforeMnC_l5=Sum_beforeMnC<5
-    Sum_beforeMnC_Mn_l5=(Sum_beforeMnC+Mn_factor)<5
-    norm_cations.loc[((Sum_beforeMnC_l5)&(Sum_beforeMnC_Mn_l5)), 'Mn_C_ideal']=Mn_factor
-    norm_cations.loc[((Sum_beforeMnC_l5)&(~Sum_beforeMnC_Mn_l5)), 'Mn_C_ideal']=5-Sum_beforeMnC
+    Sum_beforeMnC = (
+        norm_cations["Ti_C_ideal"]
+        + norm_cations["Al_VI_C_ideal"]
+        + norm_cations["Cr_C_ideal"]
+        + norm_cations["Fe3_C_ideal"]
+        + norm_cations["Mg_C_ideal"]
+        + norm_cations["Fe2_C_ideal"]
+    )
+    Sum_beforeMnC_l5 = Sum_beforeMnC < 5
+    Sum_beforeMnC_Mn_l5 = (Sum_beforeMnC + Mn_factor) < 5
+    norm_cations.loc[
+        ((Sum_beforeMnC_l5) & (Sum_beforeMnC_Mn_l5)), "Mn_C_ideal"
+    ] = Mn_factor
+    norm_cations.loc[((Sum_beforeMnC_l5) & (~Sum_beforeMnC_Mn_l5)), "Mn_C_ideal"] = (
+        5 - Sum_beforeMnC
+    )
 
     # Mg B site, if any Mg left, put here.
-    norm_cations['Mg_B_ideal']=0
-    Mg_left_B=(Mg_factor-norm_cations['Mg_C_ideal'])>0
-    norm_cations.loc[(Mg_left_B), 'Mg_B_ideal']=Mg_factor-norm_cations['Mg_C_ideal']
+    norm_cations["Mg_B_ideal"] = 0
+    Mg_left_B = (Mg_factor - norm_cations["Mg_C_ideal"]) > 0
+    norm_cations.loc[(Mg_left_B), "Mg_B_ideal"] = Mg_factor - norm_cations["Mg_C_ideal"]
 
     # Fe B site, if any Fe2 left, but here
-    norm_cations['Fe2_B_ideal']=0
-    Fe2_left_B=(Fe_factor-norm_cations['Fe2_C_ideal']-norm_cations['Fe3_C_ideal'])>0
-    norm_cations.loc[(Fe2_left_B), 'Fe2_B_ideal']=Fe_factor-norm_cations['Fe2_C_ideal']-norm_cations['Fe3_C_ideal']
+    norm_cations["Fe2_B_ideal"] = 0
+    Fe2_left_B = (
+        Fe_factor - norm_cations["Fe2_C_ideal"] - norm_cations["Fe3_C_ideal"]
+    ) > 0
+    norm_cations.loc[(Fe2_left_B), "Fe2_B_ideal"] = (
+        Fe_factor - norm_cations["Fe2_C_ideal"] - norm_cations["Fe3_C_ideal"]
+    )
 
     # Mn B site, if any Mn left, put here.
-    norm_cations['Mn_B_ideal']=0
-    Mn_left_B=(Mn_factor-norm_cations['Mn_C_ideal'])>0
-    norm_cations.loc[(Mn_left_B), 'Mn_B_ideal']=Mn_factor-norm_cations['Mn_C_ideal']
+    norm_cations["Mn_B_ideal"] = 0
+    Mn_left_B = (Mn_factor - norm_cations["Mn_C_ideal"]) > 0
+    norm_cations.loc[(Mn_left_B), "Mn_B_ideal"] = Mn_factor - norm_cations["Mn_C_ideal"]
 
     # Ca B site, all Ca
-    norm_cations['Ca_B_ideal']=Ca_factor
+    norm_cations["Ca_B_ideal"] = Ca_factor
 
     # Na, if Mg+Fe+Mn+Ca B >2, 0
-    norm_cations['Na_B_ideal']=0
-    Sum_beforeNa=(norm_cations['Mn_B_ideal']+norm_cations['Fe2_B_ideal']+norm_cations['Mg_B_ideal']+norm_cations['Ca_B_ideal'])
-    Sum_beforeNa_l2=Sum_beforeNa<2
-    Sum_before_Na_Na_l2=(Sum_beforeNa+Na_factor)<2
-    norm_cations.loc[((Sum_beforeNa_l2)&(Sum_before_Na_Na_l2)), 'Na_B_ideal']=Na_factor
-    norm_cations.loc[((Sum_beforeNa_l2)&(~Sum_before_Na_Na_l2)), 'Na_B_ideal']=2-Sum_beforeNa
+    norm_cations["Na_B_ideal"] = 0
+    Sum_beforeNa = (
+        norm_cations["Mn_B_ideal"]
+        + norm_cations["Fe2_B_ideal"]
+        + norm_cations["Mg_B_ideal"]
+        + norm_cations["Ca_B_ideal"]
+    )
+    Sum_beforeNa_l2 = Sum_beforeNa < 2
+    Sum_before_Na_Na_l2 = (Sum_beforeNa + Na_factor) < 2
+    norm_cations.loc[
+        ((Sum_beforeNa_l2) & (Sum_before_Na_Na_l2)), "Na_B_ideal"
+    ] = Na_factor
+    norm_cations.loc[((Sum_beforeNa_l2) & (~Sum_before_Na_Na_l2)), "Na_B_ideal"] = (
+        2 - Sum_beforeNa
+    )
 
     # Na_A - any Na left
-    norm_cations['Na_A_ideal']=Na_factor-norm_cations['Na_B_ideal']
-    norm_cations['K_A_ideal']=K_factor
+    norm_cations["Na_A_ideal"] = Na_factor - norm_cations["Na_B_ideal"]
+    norm_cations["K_A_ideal"] = K_factor
 
     return norm_cations
 
-def get_amp_sites2(amp_apfu_df):
 
+def get_amp_sites2(amp_apfu_df):
     """
 
     get_amp_sites takes generalized atom per formula unit calculations from
     calculate_23oxygens_amphibole and puts them in the proper cation sites
     according to Leake et al., 1997.
 
     Parameters
@@ -3239,15 +4574,15 @@
     """
 
     # new column names to drop the amp_cat_23ox. Can make this more flexible or we can just force the formatting
     # of the output inside the function. Mostly I didnt want to type it out a bunch so we can omit this little
     # loop if we want to formalize things
     newnames = []
     for name in amp_apfu_df.columns.tolist():
-        newnames.append(norm_cations.split('_')[0])
+        newnames.append(norm_cations.split("_")[0])
 
     norm_cations = amp_apfu_df.copy()
     norm_cations.columns = newnames
 
     samples = norm_cations.index.tolist()
 
     # containers to fill later
@@ -3265,79 +4600,115 @@
     Ca_B = np.empty(len(samples))
     Na_A = np.empty(len(samples))
     K_A = np.empty(len(samples))
     Cr_C = np.empty(len(samples))
 
     for sample, i in zip(samples, range(len(samples))):
         # these are all the cations that have no site ambiguity
-        Si_T[i] = norm_cations.loc[sample, 'SiO2']
-        K_A[i] = norm_cations.loc[sample, 'K2O']
-        Ti_C[i] = norm_cations.loc[sample, 'TiO2']
-        Ca_B[i] = norm_cations.loc[sample, 'CaO']
-        Cr_C[i] = norm_cations.loc[sample, 'Cr2O3']
+        Si_T[i] = norm_cations.loc[sample, "SiO2"]
+        K_A[i] = norm_cations.loc[sample, "K2O"]
+        Ti_C[i] = norm_cations.loc[sample, "TiO2"]
+        Ca_B[i] = norm_cations.loc[sample, "CaO"]
+        Cr_C[i] = norm_cations.loc[sample, "Cr2O3"]
 
         # site ambiguous cations. Follows Leake et al., (1997) logic
-        if Si_T[i] + norm_cations.loc[sample, 'Al2O3'] > 8:
-            Al_T[i] = 8 - norm_cations.loc[sample, 'SiO2']
-            Al_C[i] = norm_cations.loc[sample, 'SiO2'] + \
-                norm_cations.loc[sample, 'Al2O3'] - 8
+        if Si_T[i] + norm_cations.loc[sample, "Al2O3"] > 8:
+            Al_T[i] = 8 - norm_cations.loc[sample, "SiO2"]
+            Al_C[i] = (
+                norm_cations.loc[sample, "SiO2"] + norm_cations.loc[sample, "Al2O3"] - 8
+            )
         else:
-            Al_T[i] = norm_cations.loc[sample, 'Al2O3']
+            Al_T[i] = norm_cations.loc[sample, "Al2O3"]
             Al_C[i] = 0
 
-        if Al_C[i] + Ti_C[i] + Cr_C[i] + norm_cations.loc[sample, 'MgO'] > 5:
+        if Al_C[i] + Ti_C[i] + Cr_C[i] + norm_cations.loc[sample, "MgO"] > 5:
             Mg_C[i] = 5 - Al_C[i] + Ti_C[i] + Cr_C[i]
-            Mg_B[i] = Al_C[i] + Ti_C[i] + Cr_C[i] + \
-                norm_cations.loc[sample, 'MgO'] - 5
+            Mg_B[i] = Al_C[i] + Ti_C[i] + Cr_C[i] + norm_cations.loc[sample, "MgO"] - 5
         else:
-            Mg_C[i] = norm_cations.loc[sample, 'MgO']
+            Mg_C[i] = norm_cations.loc[sample, "MgO"]
             Mg_B[i] = 0
 
         if Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] > 5:
             Fe_C[i] = 0
-            Fe_B[i] = norm_cations.loc[sample, 'FeOt']
+            Fe_B[i] = norm_cations.loc[sample, "FeOt"]
         else:
             Fe_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i])
-            Fe_B[i] = norm_cations.loc[sample, 'FeOt'] - Fe_C[i]
+            Fe_B[i] = norm_cations.loc[sample, "FeOt"] - Fe_C[i]
 
         if Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] + Fe_C[i] > 5:
             Mn_C[i] = 0
-            Mn_B[i] = norm_cations.loc[sample, 'MnO']
+            Mn_B[i] = norm_cations.loc[sample, "MnO"]
         else:
             Mn_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] + Fe_C[i])
-            Mn_B[i] = norm_cations.loc[sample, 'MnO'] - Mn_C[i]
+            Mn_B[i] = norm_cations.loc[sample, "MnO"] - Mn_C[i]
 
         if Mg_B[i] + Fe_B[i] + Mn_B[i] + Ca_B[i] > 2:
             Na_B[i] = 0
-            Na_A[i] = norm_cations.loc[sample, 'Na2O']
+            Na_A[i] = norm_cations.loc[sample, "Na2O"]
         else:
             Na_B[i] = 2 - (Mg_B[i] + Fe_B[i] + Mn_B[i] + Ca_B[i])
             # Euan has as if Na A >0, set as 0, otherwise, =Na cations 23 O -
             # Na from A site. Ask jordan where he got this from.
-            Na_A[i] = norm_cations.loc[sample, 'Na2O'] - Na_B[i]
+            Na_A[i] = norm_cations.loc[sample, "Na2O"] - Na_B[i]
 
     # making the dataframe for the output
-    Sum_T=Al_T+Si_T
-    Sum_C=Al_C+Cr_C+Mg_C+Fe_C+Mn_C
-    Sum_B=Mg_B+Fe_B+Mn_B+Ca_B+Na_B
-    Sum_A=K_A+Na_A
-
-    site_vals = np.array([Si_T, Al_T, Al_C, Ti_C, Mg_C, Fe_C, Mn_C, Cr_C, Mg_B,
-    Fe_B, Mn_B, Na_B, Ca_B, Na_A, K_A])
-    sites_df = pd.DataFrame(site_vals.T, columns=['Si_T', 'Al_T_Amp', 'Al_C_Amp', 'Ti_C_Amp', 'Mg_C_Amp', 'Fe_C_Amp', 'Mn_C_Amp', 'Cr_C_Amp', 'Mg_B_Amp', 'Fe_B_Amp', 'Mn_B_Amp', 'Na_B_Amp', 'Ca_B_Amp', 'Na_A_Amp', 'K_A_Amp'],index=amp_apfu_df.index)
-    sites_df['Sum_T'] =   Sum_T
-    sites_df['Sum_C'] =   Sum_C
-    sites_df['Sum_B'] =   Sum_B
-    sites_df['Sum_A'] =   Sum_A
+    Sum_T = Al_T + Si_T
+    Sum_C = Al_C + Cr_C + Mg_C + Fe_C + Mn_C
+    Sum_B = Mg_B + Fe_B + Mn_B + Ca_B + Na_B
+    Sum_A = K_A + Na_A
+
+    site_vals = np.array(
+        [
+            Si_T,
+            Al_T,
+            Al_C,
+            Ti_C,
+            Mg_C,
+            Fe_C,
+            Mn_C,
+            Cr_C,
+            Mg_B,
+            Fe_B,
+            Mn_B,
+            Na_B,
+            Ca_B,
+            Na_A,
+            K_A,
+        ]
+    )
+    sites_df = pd.DataFrame(
+        site_vals.T,
+        columns=[
+            "Si_T",
+            "Al_T_Amp",
+            "Al_C_Amp",
+            "Ti_C_Amp",
+            "Mg_C_Amp",
+            "Fe_C_Amp",
+            "Mn_C_Amp",
+            "Cr_C_Amp",
+            "Mg_B_Amp",
+            "Fe_B_Amp",
+            "Mn_B_Amp",
+            "Na_B_Amp",
+            "Ca_B_Amp",
+            "Na_A_Amp",
+            "K_A_Amp",
+        ],
+        index=amp_apfu_df.index,
+    )
+    sites_df["Sum_T"] = Sum_T
+    sites_df["Sum_C"] = Sum_C
+    sites_df["Sum_B"] = Sum_B
+    sites_df["Sum_A"] = Sum_A
 
     return sites_df
 
 
 def amp_components_ferric_ferrous(sites_df, norm_cations):
-
     """
 
     amp_components_ferric_ferrous calculates the Fe3+ and Fe2+ apfu values of
     amphibole and adjusts the generic stoichiometry such that charge balance is
     maintained. This is based off the "f parameters" listed in Holland and Blundy
     (1994). Following Mutch et al. (2016) spreadsheet.
 
@@ -3356,69 +4727,107 @@
             1) FeOt is replaced by individual Fe2O3 and FeO columns
             2) all apfu values from the generic mineral recalculation have been
                 adjusted by the "f" parameter from Holland and Blundy (1994)
                 to maintain charge balance and stoichiometry
 
     """
     # A group
-    f1 = 16 / sites_df.sum(axis='columns')
-    f2 = 8 / sites_df['Si_T']
-    f3 = 15 / (sites_df.sum(axis='columns') - (sites_df['Na_B_Amp'] + sites_df['Na_A_Amp']) - sites_df['K_A_Amp'] + sites_df['Mn_C_Amp'])
-    f4 = 2 / sites_df['Ca_B_Amp']
+    f1 = 16 / sites_df.sum(axis="columns")
+    f2 = 8 / sites_df["Si_T"]
+    f3 = 15 / (
+        sites_df.sum(axis="columns")
+        - (sites_df["Na_B_Amp"] + sites_df["Na_A_Amp"])
+        - sites_df["K_A_Amp"]
+        + sites_df["Mn_C_Amp"]
+    )
+    f4 = 2 / sites_df["Ca_B_Amp"]
     f5 = 1
-    fa = pd.DataFrame({'f1': f1, 'f2': f2, 'f3': f3, 'f4': f4, 'f5': f5, })
+    fa = pd.DataFrame(
+        {
+            "f1": f1,
+            "f2": f2,
+            "f3": f3,
+            "f4": f4,
+            "f5": f5,
+        }
+    )
 
     # B group
-    f6 = 8 / (sites_df['Si_T'] + sites_df['Al_T_Amp'] + sites_df['Al_C_Amp'])
-    f7 = 15 / (sites_df.sum(axis='columns') - sites_df['K_A_Amp'])
-    f8 = 12.9 / (sites_df.sum(axis='columns') - (sites_df['Na_A_Amp'] + sites_df['Na_B_Amp'] +
-    sites_df['K_A_Amp']) - (sites_df['Mn_B_Amp'] + sites_df['Mn_C_Amp']) - sites_df['Ca_B_Amp'])
-    f9 = 36 / (46 - (sites_df['Al_T_Amp'] + sites_df['Al_C_Amp']) - sites_df['Si_T'] - sites_df['Ti_C_Amp'])
-    f10 = 46 / ((sites_df['Fe_C_Amp'] + sites_df['Fe_B_Amp']) + 46)
-    fb = pd.DataFrame({'f6': f6, 'f7': f7, 'f8': f8, 'f9': f9, 'f10': f10, })
+    f6 = 8 / (sites_df["Si_T"] + sites_df["Al_T_Amp"] + sites_df["Al_C_Amp"])
+    f7 = 15 / (sites_df.sum(axis="columns") - sites_df["K_A_Amp"])
+    f8 = 12.9 / (
+        sites_df.sum(axis="columns")
+        - (sites_df["Na_A_Amp"] + sites_df["Na_B_Amp"] + sites_df["K_A_Amp"])
+        - (sites_df["Mn_B_Amp"] + sites_df["Mn_C_Amp"])
+        - sites_df["Ca_B_Amp"]
+    )
+    f9 = 36 / (
+        46
+        - (sites_df["Al_T_Amp"] + sites_df["Al_C_Amp"])
+        - sites_df["Si_T"]
+        - sites_df["Ti_C_Amp"]
+    )
+    f10 = 46 / ((sites_df["Fe_C_Amp"] + sites_df["Fe_B_Amp"]) + 46)
+    fb = pd.DataFrame(
+        {
+            "f6": f6,
+            "f7": f7,
+            "f8": f8,
+            "f9": f9,
+            "f10": f10,
+        }
+    )
 
-    f_ave = (fa.min(axis='columns') + fb.max(axis='columns')) / 2
+    f_ave = (fa.min(axis="columns") + fb.max(axis="columns")) / 2
     # f_ave = (2/3)*fa.min(axis = 'columns') + (1/3)*fb.max(axis = 'columns')
 
-    norm_cations_hb = norm_cations.multiply(f_ave, axis='rows')
-    norm_cations_hb['Fe2O3_Amp_cat_23ox'] = 46 * (1 - f_ave)
-    norm_cations_hb['FeO_Amp_cat_23ox'] = norm_cations_hb['Fet_Amp_cat_23ox'] - norm_cations_hb['Fe2O3_Amp_cat_23ox']
-    norm_cations_hb.drop(columns=['Fet_Amp_cat_23ox', 'oxy_renorm_factor',
-                         'cation_sum_Si_Mg', 'cation_sum_Si_Ca', 'Amp_Cation_Sum'], inplace=True)
+    norm_cations_hb = norm_cations.multiply(f_ave, axis="rows")
+    norm_cations_hb["Fe2O3_Amp_cat_23ox"] = 46 * (1 - f_ave)
+    norm_cations_hb["FeO_Amp_cat_23ox"] = (
+        norm_cations_hb["Fet_Amp_cat_23ox"] - norm_cations_hb["Fe2O3_Amp_cat_23ox"]
+    )
+    norm_cations_hb.drop(
+        columns=[
+            "Fet_Amp_cat_23ox",
+            "oxy_renorm_factor",
+            "cation_sum_Si_Mg",
+            "cation_sum_Si_Ca",
+            "Amp_Cation_Sum",
+        ],
+        inplace=True,
+    )
     # newnames = []
     # for name in norm_cations_hb.columns.tolist():
     #     newnames.append(norm_cations.split('_')[0])
 
-    #norm_cations_hb.columns = newnames
+    # norm_cations_hb.columns = newnames
 
     return norm_cations_hb, f_ave
 
 
-
 def get_amp_sites_ferric_ferrous(amp_apfu_df):
-
     """
     get_amp_sites_ferric_ferrous is very similar to get_amp_sites, however it now
     incorporates the newly calculated Fe2O3 and FeO apfu values such that all
     Fe2O3 gets incorporated into the octahedral sites before any FeO. For more
     information see Leake et al., 1997 Appendix A.
 
-    Parameters: 
-        amp_apfu_df (pandas DataFrame): amphibole apfu values for each cation, now reflecting Fe2O3 
+    Parameters:
+        amp_apfu_df (pandas DataFrame): amphibole apfu values for each cation, now reflecting Fe2O3
             and FeO values. This is the output from amp_components_ferric_ferrous and does
             not need to be modified at all.
 
-    Returns: 
+    Returns:
         sites_df (pandas DataFrame): a samples by cation sites dimension dataframe where each column corresponds
             to a cation site in amphibole. The suffix at the end corresponds to which site
-            the cation is in: 
+            the cation is in:
             T = tetrahedral sites (8 total)
             C = octahedral sites (5 total)
             B  = M4 sites (2 total)
-            A = A site (0 - 1 total). 
+            A = A site (0 - 1 total).
             See Leake et al., 1997 for a discussion on cation site prioritization
     """
     samples = amp_apfu_df.index.tolist()
     Si_T = np.empty(len(samples))
     Al_T = np.empty(len(samples))
     Al_C = np.empty(len(samples))
     Ti_C = np.empty(len(samples))
@@ -3433,70 +4842,119 @@
     Ca_B = np.empty(len(samples))
     Na_A = np.empty(len(samples))
     K_A = np.empty(len(samples))
     Cr_C = np.empty(len(samples))
     Fe3_C = np.empty(len(samples))
 
     for sample, i in zip(samples, range(len(samples))):
-        Si_T[i] = amp_apfu_df.loc[sample, 'Si_Amp_cat_23ox']
-        K_A[i] = amp_apfu_df.loc[sample, 'K_Amp_cat_23ox']
-        Ti_C[i] = amp_apfu_df.loc[sample, 'Ti_Amp_cat_23ox']
-        Ca_B[i] = amp_apfu_df.loc[sample, 'Ca_Amp_cat_23ox']
-        Cr_C[i] = amp_apfu_df.loc[sample, 'Cr_Amp_cat_23ox']
-        Fe3_C[i] = amp_apfu_df.loc[sample, 'Fe2O3_Amp_cat_23ox']
-
-        if Si_T[i] + amp_apfu_df.loc[sample, 'Al_Amp_cat_23ox'] > 8:
-            Al_T[i] = 8 - amp_apfu_df.loc[sample, 'Si_Amp_cat_23ox']
-            Al_C[i] = amp_apfu_df.loc[sample, 'Si_Amp_cat_23ox'] + \
-                amp_apfu_df.loc[sample, 'Al_Amp_cat_23ox'] - 8
+        Si_T[i] = amp_apfu_df.loc[sample, "Si_Amp_cat_23ox"]
+        K_A[i] = amp_apfu_df.loc[sample, "K_Amp_cat_23ox"]
+        Ti_C[i] = amp_apfu_df.loc[sample, "Ti_Amp_cat_23ox"]
+        Ca_B[i] = amp_apfu_df.loc[sample, "Ca_Amp_cat_23ox"]
+        Cr_C[i] = amp_apfu_df.loc[sample, "Cr_Amp_cat_23ox"]
+        Fe3_C[i] = amp_apfu_df.loc[sample, "Fe2O3_Amp_cat_23ox"]
+
+        if Si_T[i] + amp_apfu_df.loc[sample, "Al_Amp_cat_23ox"] > 8:
+            Al_T[i] = 8 - amp_apfu_df.loc[sample, "Si_Amp_cat_23ox"]
+            Al_C[i] = (
+                amp_apfu_df.loc[sample, "Si_Amp_cat_23ox"]
+                + amp_apfu_df.loc[sample, "Al_Amp_cat_23ox"]
+                - 8
+            )
         else:
-            Al_T[i] = amp_apfu_df.loc[sample, 'Al_Amp_cat_23ox']
+            Al_T[i] = amp_apfu_df.loc[sample, "Al_Amp_cat_23ox"]
             Al_C[i] = 0
-        if Al_C[i] + Ti_C[i] + Cr_C[i] + Fe3_C[i] + \
-                amp_apfu_df.loc[sample, 'Mg_Amp_cat_23ox'] > 5:
+        if (
+            Al_C[i]
+            + Ti_C[i]
+            + Cr_C[i]
+            + Fe3_C[i]
+            + amp_apfu_df.loc[sample, "Mg_Amp_cat_23ox"]
+            > 5
+        ):
             Mg_C[i] = 5 - Al_C[i] + Ti_C[i] + Cr_C[i] + Fe3_C[i]
-            Mg_B[i] = Al_C[i] + Ti_C[i] + Cr_C[i] + \
-                Fe3_C[i] + amp_apfu_df.loc[sample, 'Mg_Amp_cat_23ox'] - 5
+            Mg_B[i] = (
+                Al_C[i]
+                + Ti_C[i]
+                + Cr_C[i]
+                + Fe3_C[i]
+                + amp_apfu_df.loc[sample, "Mg_Amp_cat_23ox"]
+                - 5
+            )
         else:
-            Mg_C[i] = amp_apfu_df.loc[sample, 'Mg_Amp_cat_23ox']
+            Mg_C[i] = amp_apfu_df.loc[sample, "Mg_Amp_cat_23ox"]
             Mg_B[i] = 0
 
         if Al_C[i] + Ti_C[i] + Cr_C[i] + Fe3_C[i] + Mg_C[i] > 5:
             Fe2_C[i] = 0
-            Fe2_B[i] = amp_apfu_df.loc[sample, 'FeO_Amp_cat_23ox']
+            Fe2_B[i] = amp_apfu_df.loc[sample, "FeO_Amp_cat_23ox"]
         else:
             Fe2_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] + Fe3_C[i] + Mg_C[i])
-            Fe2_B[i] = amp_apfu_df.loc[sample, 'FeO_Amp_cat_23ox'] - Fe2_C[i]
+            Fe2_B[i] = amp_apfu_df.loc[sample, "FeO_Amp_cat_23ox"] - Fe2_C[i]
 
         if Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] + Fe3_C[i] + Fe2_C[i] > 5:
             Mn_C[i] = 0
-            Mn_B[i] = amp_apfu_df.loc[sample, 'Mn_Amp_cat_23ox']
+            Mn_B[i] = amp_apfu_df.loc[sample, "Mn_Amp_cat_23ox"]
         else:
-            Mn_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] +
-                           Mg_C[i] + Fe2_C[i] + Fe3_C[i])
-            Mn_B[i] = amp_apfu_df.loc[sample, 'Mn_Amp_cat_23ox'] - Mn_C[i]
+            Mn_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] + Fe2_C[i] + Fe3_C[i])
+            Mn_B[i] = amp_apfu_df.loc[sample, "Mn_Amp_cat_23ox"] - Mn_C[i]
 
         if Mg_B[i] + Fe2_B[i] + Mn_B[i] + Ca_B[i] > 2:
             Na_B[i] = 0
-            Na_A[i] = amp_apfu_df.loc[sample, 'Na_Amp_cat_23ox']
+            Na_A[i] = amp_apfu_df.loc[sample, "Na_Amp_cat_23ox"]
         else:
             Na_B[i] = 2 - (Mg_B[i] + Fe2_B[i] + Mn_B[i] + Ca_B[i])
-            Na_A[i] = amp_apfu_df.loc[sample, 'Na_Amp_cat_23ox'] - Na_B[i]
+            Na_A[i] = amp_apfu_df.loc[sample, "Na_Amp_cat_23ox"] - Na_B[i]
 
-    site_vals = np.array([Si_T, Al_T, Al_C, Ti_C, Mg_C, Fe3_C, Fe2_C, Mn_C, Cr_C,
-    Mg_B, Fe2_B, Mn_B, Na_B, Ca_B, Na_A, K_A])
-    sites_df = pd.DataFrame(site_vals.T, columns=['Si_T', 'Al_T_Amp', 'Al_C_Amp', 'Ti_C_Amp', 'Mg_C_Amp', 'Fe3_C',
-    'Fe2_C','Mn_C_Amp', 'Cr_C_Amp', 'Mg_B_Amp','Fe2_B','Mn_B_Amp', 'Na_B_Amp','Ca_B_Amp', 'Na_A_Amp', 'K_A_Amp'],
-                            index=amp_apfu_df.index)
+    site_vals = np.array(
+        [
+            Si_T,
+            Al_T,
+            Al_C,
+            Ti_C,
+            Mg_C,
+            Fe3_C,
+            Fe2_C,
+            Mn_C,
+            Cr_C,
+            Mg_B,
+            Fe2_B,
+            Mn_B,
+            Na_B,
+            Ca_B,
+            Na_A,
+            K_A,
+        ]
+    )
+    sites_df = pd.DataFrame(
+        site_vals.T,
+        columns=[
+            "Si_T",
+            "Al_T_Amp",
+            "Al_C_Amp",
+            "Ti_C_Amp",
+            "Mg_C_Amp",
+            "Fe3_C",
+            "Fe2_C",
+            "Mn_C_Amp",
+            "Cr_C_Amp",
+            "Mg_B_Amp",
+            "Fe2_B",
+            "Mn_B_Amp",
+            "Na_B_Amp",
+            "Ca_B_Amp",
+            "Na_A_Amp",
+            "K_A_Amp",
+        ],
+        index=amp_apfu_df.index,
+    )
     return sites_df
 
 
-
 def get_amp_sites_mutch(amp_apfu_df):
-
     """
 
     get_amp_sites takes generalized atom per formula unit calculations from
     calculate_23oxygens_amphibole and puts them in the proper cation sites
     according to the spreasheet of Mutch et al. Gives negative numbers for Na. .
 
     Parameters
@@ -3539,72 +4997,122 @@
     Ca_B = np.empty(len(samples))
     Na_A = np.empty(len(samples))
     K_A = np.empty(len(samples))
     Cr_C = np.empty(len(samples))
 
     for sample, i in zip(samples, range(len(samples))):
         # these are all the cations that have no site ambiguity
-        Si_T[i] = norm_cations.loc[sample, 'Si_Amp_cat_23ox']
-        K_A[i] = norm_cations.loc[sample, 'K_Amp_cat_23ox']
-        Ti_C[i] = norm_cations.loc[sample, 'Ti_Amp_cat_23ox']
-        Ca_B[i] = norm_cations.loc[sample, 'Ca_Amp_cat_23ox']
-        Cr_C[i] = norm_cations.loc[sample, 'Cr_Amp_cat_23ox']
+        Si_T[i] = norm_cations.loc[sample, "Si_Amp_cat_23ox"]
+        K_A[i] = norm_cations.loc[sample, "K_Amp_cat_23ox"]
+        Ti_C[i] = norm_cations.loc[sample, "Ti_Amp_cat_23ox"]
+        Ca_B[i] = norm_cations.loc[sample, "Ca_Amp_cat_23ox"]
+        Cr_C[i] = norm_cations.loc[sample, "Cr_Amp_cat_23ox"]
 
         # site ambiguous cations. Follows Leake et al., (1997) logic
-        if Si_T[i] + norm_cations.loc[sample, 'Al_Amp_cat_23ox'] > 8:
-            Al_T[i] = 8 - norm_cations.loc[sample, 'Si_Amp_cat_23ox']
-            Al_C[i] = norm_cations.loc[sample, 'Si_Amp_cat_23ox'] + \
-                norm_cations.loc[sample, 'Al_Amp_cat_23ox'] - 8
+        if Si_T[i] + norm_cations.loc[sample, "Al_Amp_cat_23ox"] > 8:
+            Al_T[i] = 8 - norm_cations.loc[sample, "Si_Amp_cat_23ox"]
+            Al_C[i] = (
+                norm_cations.loc[sample, "Si_Amp_cat_23ox"]
+                + norm_cations.loc[sample, "Al_Amp_cat_23ox"]
+                - 8
+            )
         else:
-            Al_T[i] = norm_cations.loc[sample, 'Al_Amp_cat_23ox']
+            Al_T[i] = norm_cations.loc[sample, "Al_Amp_cat_23ox"]
             Al_C[i] = 0
 
-        if Al_C[i] + Ti_C[i] + Cr_C[i] + norm_cations.loc[sample, 'Mg_Amp_cat_23ox'] > 5:
+        if (
+            Al_C[i] + Ti_C[i] + Cr_C[i] + norm_cations.loc[sample, "Mg_Amp_cat_23ox"]
+            > 5
+        ):
             Mg_C[i] = 5 - Al_C[i] + Ti_C[i] + Cr_C[i]
-            Mg_B[i] = Al_C[i] + Ti_C[i] + Cr_C[i] + \
-                norm_cations.loc[sample, 'Mg_Amp_cat_23ox'] - 5
+            Mg_B[i] = (
+                Al_C[i]
+                + Ti_C[i]
+                + Cr_C[i]
+                + norm_cations.loc[sample, "Mg_Amp_cat_23ox"]
+                - 5
+            )
         else:
-            Mg_C[i] = norm_cations.loc[sample, 'Mg_Amp_cat_23ox']
+            Mg_C[i] = norm_cations.loc[sample, "Mg_Amp_cat_23ox"]
             Mg_B[i] = 0
 
         if Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] > 5:
             Fe_C[i] = 0
-            Fe_B[i] = norm_cations.loc[sample, 'Fet_Amp_cat_23ox']
+            Fe_B[i] = norm_cations.loc[sample, "Fet_Amp_cat_23ox"]
         else:
             Fe_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i])
-            Fe_B[i] = norm_cations.loc[sample, 'Fet_Amp_cat_23ox'] - Fe_C[i]
+            Fe_B[i] = norm_cations.loc[sample, "Fet_Amp_cat_23ox"] - Fe_C[i]
 
         if Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] + Fe_C[i] > 5:
             Mn_C[i] = 0
-            Mn_B[i] = norm_cations.loc[sample, 'Mn_Amp_cat_23ox']
+            Mn_B[i] = norm_cations.loc[sample, "Mn_Amp_cat_23ox"]
         else:
             Mn_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] + Fe_C[i])
-            Mn_B[i] = norm_cations.loc[sample, 'Mn_Amp_cat_23ox'] - Mn_C[i]
+            Mn_B[i] = norm_cations.loc[sample, "Mn_Amp_cat_23ox"] - Mn_C[i]
 
-        if Mg_B[i] + Fe_B[i] + Mn_B[i] + Ca_B[i] + \
-                amp_apfu_df['Na_Amp_cat_23ox'].iloc[i] > 2:
+        if (
+            Mg_B[i]
+            + Fe_B[i]
+            + Mn_B[i]
+            + Ca_B[i]
+            + amp_apfu_df["Na_Amp_cat_23ox"].iloc[i]
+            > 2
+        ):
             Na_B[i] = 2 - (Mg_B[i] + Fe_B[i] + Mn_B[i] + Ca_B[i])
-            Na_A[i] = amp_apfu_df['Na_Amp_cat_23ox'].iloc[i] - Na_B[i]
+            Na_A[i] = amp_apfu_df["Na_Amp_cat_23ox"].iloc[i] - Na_B[i]
         else:
-            Na_B[i] = amp_apfu_df['Na_Amp_cat_23ox'].iloc[i]
+            Na_B[i] = amp_apfu_df["Na_Amp_cat_23ox"].iloc[i]
             # Euan has as if Na A >0, set as 0, otherwise, =Na cations 23 O -
             # Na from A site. Ask jordan where he got this from.
-            Na_A[i] = amp_apfu_df['Na_Amp_cat_23ox'].iloc[i] - Na_B[i]
+            Na_A[i] = amp_apfu_df["Na_Amp_cat_23ox"].iloc[i] - Na_B[i]
 
-    site_vals = np.array([Si_T, Al_T, Al_C, Ti_C, Mg_C, Fe_C, Mn_C, Cr_C, Mg_B,
-    Fe_B, Mn_B, Na_B, Ca_B, Na_A, K_A])
-    sites_df = pd.DataFrame(site_vals.T, columns=['Si_T', 'Al_T_Amp', 'Al_C_Amp', 'Ti_C_Amp',
-     'Mg_C_Amp', 'Fe_C_Amp', 'Mn_C_Amp', 'Cr_C_Amp', 'Mg_B_Amp', 'Fe_B_Amp', 'Mn_B_Amp', 'Na_B_Amp', 'Ca_B_Amp', 'Na_A_Amp', 'K_A_Amp'],
-    index=amp_apfu_df.index)
+    site_vals = np.array(
+        [
+            Si_T,
+            Al_T,
+            Al_C,
+            Ti_C,
+            Mg_C,
+            Fe_C,
+            Mn_C,
+            Cr_C,
+            Mg_B,
+            Fe_B,
+            Mn_B,
+            Na_B,
+            Ca_B,
+            Na_A,
+            K_A,
+        ]
+    )
+    sites_df = pd.DataFrame(
+        site_vals.T,
+        columns=[
+            "Si_T",
+            "Al_T_Amp",
+            "Al_C_Amp",
+            "Ti_C_Amp",
+            "Mg_C_Amp",
+            "Fe_C_Amp",
+            "Mn_C_Amp",
+            "Cr_C_Amp",
+            "Mg_B_Amp",
+            "Fe_B_Amp",
+            "Mn_B_Amp",
+            "Na_B_Amp",
+            "Ca_B_Amp",
+            "Na_A_Amp",
+            "K_A_Amp",
+        ],
+        index=amp_apfu_df.index,
+    )
     return sites_df
 
 
-
 def amp_components_ferric_ferrous_mutch(sites_df, norm_cations):
-   
     """
 
     amp_components_ferric_ferrous calculates the Fe3+ and Fe2+ apfu values of
     amphibole and adjusts the generic stoichiometry such that charge balance is
     maintained. This is based off the "f parameters" listed in Holland and Blundy
     (1994), using the averaging in the spreadsheet supplied by Euan Mutch
 
@@ -3623,46 +5131,92 @@
             1) FeOt is replaced by individual Fe2O3 and FeO columns
             2) all apfu values from the generic mineral recalculation have been
                 adjusted by the "f" parameter from Holland and Blundy (1994)
                 to maintain charge balance and stoichiometry
 
     """
     # A group
-    f1 = 16 / sites_df.sum(axis='columns')
-    f2 = 8 / sites_df['Si_T']
-    #f3 = 15/(sites_df.sum(axis = 'columns') - (sites_df['Na_B_Amp'] + sites_df['Na_A_Amp']) - sites_df['K_A_Amp'] + sites_df['Mn_C_Amp'])
-    f3 = 15 / (sites_df.sum(axis='columns') - sites_df['K_A_Amp'] - (sites_df['Na_A_Amp'] + sites_df['Na_B_Amp']) + sites_df['Mn_B_Amp'])
+    f1 = 16 / sites_df.sum(axis="columns")
+    f2 = 8 / sites_df["Si_T"]
+    # f3 = 15/(sites_df.sum(axis = 'columns') - (sites_df['Na_B_Amp'] + sites_df['Na_A_Amp']) - sites_df['K_A_Amp'] + sites_df['Mn_C_Amp'])
+    f3 = 15 / (
+        sites_df.sum(axis="columns")
+        - sites_df["K_A_Amp"]
+        - (sites_df["Na_A_Amp"] + sites_df["Na_B_Amp"])
+        + sites_df["Mn_B_Amp"]
+    )
 
-    f4 = 2 / sites_df['Ca_B_Amp']
+    f4 = 2 / sites_df["Ca_B_Amp"]
     f5 = 1
-    fa = pd.DataFrame({'f1': f1, 'f2': f2, 'f3': f3, 'f4': f4, 'f5': f5, })
+    fa = pd.DataFrame(
+        {
+            "f1": f1,
+            "f2": f2,
+            "f3": f3,
+            "f4": f4,
+            "f5": f5,
+        }
+    )
 
     # B group
-    f6 = 8 / (sites_df['Si_T'] + sites_df['Al_T_Amp'] + sites_df['Al_C_Amp'])
-    f7 = 15 / (sites_df.sum(axis='columns') - sites_df['K_A_Amp'])
-    f8 = 12.9 / (sites_df.sum(axis='columns') - (sites_df['Na_A_Amp'] + sites_df['K_A_Amp'] + sites_df['K_A_Amp']) - sites_df['Ca_B_Amp'] - (sites_df['Mn_C_Amp'] + sites_df['Mn_B_Amp']))
-    f8 = (13 / (sites_df.sum(axis='columns') - (sites_df['K_A_Amp'] + sites_df['Na_A_Amp'] + sites_df['Na_B_Amp']) - (sites_df['Mn_B_Amp'] + sites_df['Mn_C_Amp']) - sites_df['Ca_B_Amp']))
-
-    f9 = 36 / (46 - (sites_df['Al_T_Amp'] + sites_df['Al_C_Amp']) - sites_df['Si_T'] - sites_df['Ti_C_Amp'])
-    f10 = 46 / ((sites_df['Fe_C_Amp'] + sites_df['Fe_B_Amp']) + 46)
-    fb = pd.DataFrame({'f6': f6, 'f7': f7, 'f8': f8, 'f9': f9, 'f10': f10, })
-
-    #f_ave = (fa.min(axis = 'columns') + fb.max(axis = 'columns'))/2
-    f_ave = (2 / 3) * fa.min(axis='columns') + (1 / 3) * fb.max(axis='columns')
-
-    norm_cations_hb = norm_cations.multiply(f_ave, axis='rows')
-    norm_cations_hb['Fe2O3_Amp_cat_23ox'] = 46 * (1 - f_ave)
-    norm_cations_hb['FeO_Amp_cat_23ox'] = norm_cations_hb['Fet_Amp_cat_23ox'] - norm_cations_hb['Fe2O3_Amp_cat_23ox']
-    norm_cations_hb.drop(columns=['Fet_Amp_cat_23ox', 'oxy_renorm_factor', 'cation_sum_Si_Mg', 'cation_sum_Si_Ca', 'Amp_Cation_Sum'], inplace=True)
+    f6 = 8 / (sites_df["Si_T"] + sites_df["Al_T_Amp"] + sites_df["Al_C_Amp"])
+    f7 = 15 / (sites_df.sum(axis="columns") - sites_df["K_A_Amp"])
+    f8 = 12.9 / (
+        sites_df.sum(axis="columns")
+        - (sites_df["Na_A_Amp"] + sites_df["K_A_Amp"] + sites_df["K_A_Amp"])
+        - sites_df["Ca_B_Amp"]
+        - (sites_df["Mn_C_Amp"] + sites_df["Mn_B_Amp"])
+    )
+    f8 = 13 / (
+        sites_df.sum(axis="columns")
+        - (sites_df["K_A_Amp"] + sites_df["Na_A_Amp"] + sites_df["Na_B_Amp"])
+        - (sites_df["Mn_B_Amp"] + sites_df["Mn_C_Amp"])
+        - sites_df["Ca_B_Amp"]
+    )
+
+    f9 = 36 / (
+        46
+        - (sites_df["Al_T_Amp"] + sites_df["Al_C_Amp"])
+        - sites_df["Si_T"]
+        - sites_df["Ti_C_Amp"]
+    )
+    f10 = 46 / ((sites_df["Fe_C_Amp"] + sites_df["Fe_B_Amp"]) + 46)
+    fb = pd.DataFrame(
+        {
+            "f6": f6,
+            "f7": f7,
+            "f8": f8,
+            "f9": f9,
+            "f10": f10,
+        }
+    )
+
+    # f_ave = (fa.min(axis = 'columns') + fb.max(axis = 'columns'))/2
+    f_ave = (2 / 3) * fa.min(axis="columns") + (1 / 3) * fb.max(axis="columns")
+
+    norm_cations_hb = norm_cations.multiply(f_ave, axis="rows")
+    norm_cations_hb["Fe2O3_Amp_cat_23ox"] = 46 * (1 - f_ave)
+    norm_cations_hb["FeO_Amp_cat_23ox"] = (
+        norm_cations_hb["Fet_Amp_cat_23ox"] - norm_cations_hb["Fe2O3_Amp_cat_23ox"]
+    )
+    norm_cations_hb.drop(
+        columns=[
+            "Fet_Amp_cat_23ox",
+            "oxy_renorm_factor",
+            "cation_sum_Si_Mg",
+            "cation_sum_Si_Ca",
+            "Amp_Cation_Sum",
+        ],
+        inplace=True,
+    )
 
     return norm_cations_hb
 
 
 def get_amp_sites_ferric_ferrous_mutch(amp_apfu_df):
-
     """
     get_amp_sites_ferric_ferrous is very similar to get_amp_sites, however it now
     incorporates the newly calculated Fe2O3 and FeO apfu values such that all
     Fe2O3 gets incorporated into the octahedral sites before any FeO. For more
     information see Leake et al., 1997 Appendix A.
 
     Parameters
@@ -3673,16 +5227,16 @@
         not need to be modified at all.
 
     Returns
     -------
     sites_df : pandas DataFrame
     a samples by cation sites dimension dataframe where each column corresponds
         to a cation site in amphibole. The suffix at the end corresponds to which site
-        the cation is in: T = tetrahedral sites (8 total); C = octahedral sites (5 total); 
-        B  = M4 sites (2 total); A = A site (0 - 1 total). 
+        the cation is in: T = tetrahedral sites (8 total); C = octahedral sites (5 total);
+        B  = M4 sites (2 total); A = A site (0 - 1 total).
         See Leake et al., 1997 for a discussion on cation site prioritization
     """
     samples = amp_apfu_df.index.tolist()
     Si_T = np.empty(len(samples))
     Al_T = np.empty(len(samples))
     Al_C = np.empty(len(samples))
     Ti_C = np.empty(len(samples))
@@ -3697,110 +5251,181 @@
     Ca_B = np.empty(len(samples))
     Na_A = np.empty(len(samples))
     K_A = np.empty(len(samples))
     Cr_C = np.empty(len(samples))
     Fe3_C = np.empty(len(samples))
 
     for sample, i in zip(samples, range(len(samples))):
-        Si_T[i] = amp_apfu_df.loc[sample, 'Si_Amp_cat_23ox']
-        K_A[i] = amp_apfu_df.loc[sample, 'K_Amp_cat_23ox']
-        Ti_C[i] = amp_apfu_df.loc[sample, 'Ti_Amp_cat_23ox']
-        Ca_B[i] = amp_apfu_df.loc[sample, 'Ca_Amp_cat_23ox']
-        Cr_C[i] = amp_apfu_df.loc[sample, 'Cr_Amp_cat_23ox']
-        Fe3_C[i] = amp_apfu_df.loc[sample, 'Fe2O3_Amp_cat_23ox']
-
-        if Si_T[i] + amp_apfu_df.loc[sample, 'Al_Amp_cat_23ox'] > 8:
-            Al_T[i] = 8 - amp_apfu_df.loc[sample, 'Si_Amp_cat_23ox']
-            Al_C[i] = amp_apfu_df.loc[sample, 'Si_Amp_cat_23ox'] + \
-                amp_apfu_df.loc[sample, 'Al_Amp_cat_23ox'] - 8
+        Si_T[i] = amp_apfu_df.loc[sample, "Si_Amp_cat_23ox"]
+        K_A[i] = amp_apfu_df.loc[sample, "K_Amp_cat_23ox"]
+        Ti_C[i] = amp_apfu_df.loc[sample, "Ti_Amp_cat_23ox"]
+        Ca_B[i] = amp_apfu_df.loc[sample, "Ca_Amp_cat_23ox"]
+        Cr_C[i] = amp_apfu_df.loc[sample, "Cr_Amp_cat_23ox"]
+        Fe3_C[i] = amp_apfu_df.loc[sample, "Fe2O3_Amp_cat_23ox"]
+
+        if Si_T[i] + amp_apfu_df.loc[sample, "Al_Amp_cat_23ox"] > 8:
+            Al_T[i] = 8 - amp_apfu_df.loc[sample, "Si_Amp_cat_23ox"]
+            Al_C[i] = (
+                amp_apfu_df.loc[sample, "Si_Amp_cat_23ox"]
+                + amp_apfu_df.loc[sample, "Al_Amp_cat_23ox"]
+                - 8
+            )
         else:
-            Al_T[i] = amp_apfu_df.loc[sample, 'Al_Amp_cat_23ox']
+            Al_T[i] = amp_apfu_df.loc[sample, "Al_Amp_cat_23ox"]
             Al_C[i] = 0
-        if Al_C[i] + Ti_C[i] + Cr_C[i] + Fe3_C[i] + \
-                amp_apfu_df.loc[sample, 'Mg_Amp_cat_23ox'] > 5:
+        if (
+            Al_C[i]
+            + Ti_C[i]
+            + Cr_C[i]
+            + Fe3_C[i]
+            + amp_apfu_df.loc[sample, "Mg_Amp_cat_23ox"]
+            > 5
+        ):
             Mg_C[i] = 5 - Al_C[i] + Ti_C[i] + Cr_C[i] + Fe3_C[i]
-            Mg_B[i] = Al_C[i] + Ti_C[i] + Cr_C[i] + \
-                Fe3_C[i] + amp_apfu_df.loc[sample, 'Mg_Amp_cat_23ox'] - 5
+            Mg_B[i] = (
+                Al_C[i]
+                + Ti_C[i]
+                + Cr_C[i]
+                + Fe3_C[i]
+                + amp_apfu_df.loc[sample, "Mg_Amp_cat_23ox"]
+                - 5
+            )
         else:
-            Mg_C[i] = amp_apfu_df.loc[sample, 'Mg_Amp_cat_23ox']
+            Mg_C[i] = amp_apfu_df.loc[sample, "Mg_Amp_cat_23ox"]
             Mg_B[i] = 0
 
         if Al_C[i] + Ti_C[i] + Cr_C[i] + Fe3_C[i] + Mg_C[i] > 5:
             Fe2_C[i] = 0
-            Fe2_B[i] = amp_apfu_df.loc[sample, 'FeO_Amp_cat_23ox']
+            Fe2_B[i] = amp_apfu_df.loc[sample, "FeO_Amp_cat_23ox"]
         else:
             Fe2_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] + Fe3_C[i] + Mg_C[i])
-            Fe2_B[i] = amp_apfu_df.loc[sample, 'FeO_Amp_cat_23ox'] - Fe2_C[i]
+            Fe2_B[i] = amp_apfu_df.loc[sample, "FeO_Amp_cat_23ox"] - Fe2_C[i]
 
         if Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] + Fe3_C[i] + Fe2_C[i] > 5:
             Mn_C[i] = 0
-            Mn_B[i] = amp_apfu_df.loc[sample, 'Mn_Amp_cat_23ox']
+            Mn_B[i] = amp_apfu_df.loc[sample, "Mn_Amp_cat_23ox"]
         else:
-            Mn_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] +
-                           Mg_C[i] + Fe2_C[i] + Fe3_C[i])
-            Mn_B[i] = amp_apfu_df.loc[sample, 'Mn_Amp_cat_23ox'] - Mn_C[i]
+            Mn_C[i] = 5 - (Al_C[i] + Ti_C[i] + Cr_C[i] + Mg_C[i] + Fe2_C[i] + Fe3_C[i])
+            Mn_B[i] = amp_apfu_df.loc[sample, "Mn_Amp_cat_23ox"] - Mn_C[i]
 
-        if Mg_B[i] + Fe2_B[i] + Mn_B[i] + Ca_B[i] + \
-                amp_apfu_df.loc[sample, 'Na_Amp_cat_23ox'] > 2:
+        if (
+            Mg_B[i]
+            + Fe2_B[i]
+            + Mn_B[i]
+            + Ca_B[i]
+            + amp_apfu_df.loc[sample, "Na_Amp_cat_23ox"]
+            > 2
+        ):
             Na_B[i] = 2 - (Mg_B[i] + Fe2_B[i] + Mn_B[i] + Ca_B[i])
-            Na_A[i] = amp_apfu_df.loc[sample, 'Na_Amp_cat_23ox'] - Na_B[i]
+            Na_A[i] = amp_apfu_df.loc[sample, "Na_Amp_cat_23ox"] - Na_B[i]
 
         else:
-            Na_B[i] = amp_apfu_df.loc[sample, 'Na_Amp_cat_23ox']
+            Na_B[i] = amp_apfu_df.loc[sample, "Na_Amp_cat_23ox"]
             # Euan has as if Na A >0, set as 0, otherwise, =Na cations 23 O -
             # Na from A site. Ask jordan where he got this from.
-            Na_A[i] = amp_apfu_df.loc[sample, 'Na_Amp_cat_23ox'] - Na_B[i]
+            Na_A[i] = amp_apfu_df.loc[sample, "Na_Amp_cat_23ox"] - Na_B[i]
 
-    site_vals = np.array([Si_T, Al_T, Al_C, Ti_C, Mg_C, Fe3_C, Fe2_C, Mn_C, Cr_C, Mg_B,
-    Fe2_B, Mn_B, Na_B, Ca_B, Na_A, K_A])
-    sites_df = pd.DataFrame(site_vals.T, columns=['Si_T', 'Al_T_Amp', 'Al_C_Amp', 'Ti_C_Amp', 'Mg_C_Amp', 'Fe3_C', 'Fe2_C', 'Mn_C_Amp', 'Cr_C_Amp', 'Mg_B_Amp', 'Fe2_B', 'Mn_B_Amp', 'Na_B_Amp', 'Ca_B_Amp', 'Na_A_Amp', 'K_A_Amp'],
-    index=amp_apfu_df.index)
+    site_vals = np.array(
+        [
+            Si_T,
+            Al_T,
+            Al_C,
+            Ti_C,
+            Mg_C,
+            Fe3_C,
+            Fe2_C,
+            Mn_C,
+            Cr_C,
+            Mg_B,
+            Fe2_B,
+            Mn_B,
+            Na_B,
+            Ca_B,
+            Na_A,
+            K_A,
+        ]
+    )
+    sites_df = pd.DataFrame(
+        site_vals.T,
+        columns=[
+            "Si_T",
+            "Al_T_Amp",
+            "Al_C_Amp",
+            "Ti_C_Amp",
+            "Mg_C_Amp",
+            "Fe3_C",
+            "Fe2_C",
+            "Mn_C_Amp",
+            "Cr_C_Amp",
+            "Mg_B_Amp",
+            "Fe2_B",
+            "Mn_B_Amp",
+            "Na_B_Amp",
+            "Ca_B_Amp",
+            "Na_A_Amp",
+            "K_A_Amp",
+        ],
+        index=amp_apfu_df.index,
+    )
 
     return sites_df
 
 
 # %% BIOTITE
 
 
 def calculate_mol_proportions_biotite(bt_comps):
-
     """
 
     Import Biotite compositions using bt_comps=My_Biotites, returns mole proportions
-    
+
     Parameters
     -------
     bt_comps: pandas.DataFrame
             Panda DataFrame of biotite compositions with column headings SiO2_Bt, MgO_Bt etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for biotites with column headings of the form SiO2_Bt_mol_prop
 
     """
 
-    oxide_mass_bt = {'SiO2_Bt': 60.0843, 'MgO_Bt': 40.3044, 'FeOt_Bt': 71.8464, 'CaO_Bt': 56.0774,'Al2O3_Bt': 101.961, 'Na2O_Bt': 61.9789, 'K2O_Bt': 94.196, 'MnO_Bt': 70.9375, 'TiO2_Bt': 79.7877, 'Cr2O3_Bt': 151.9982, 'P2O5_Bt': 141.937}
-    oxide_mass_bt_df = pd.DataFrame.from_dict(oxide_mass_bt, orient='index').T
-    oxide_mass_bt_df['Sample_ID_Bt'] = 'MolWt'
-    oxide_mass_bt_df.set_index('Sample_ID_Bt', inplace=True)
+    oxide_mass_bt = {
+        "SiO2_Bt": 60.0843,
+        "MgO_Bt": 40.3044,
+        "FeOt_Bt": 71.8464,
+        "CaO_Bt": 56.0774,
+        "Al2O3_Bt": 101.961,
+        "Na2O_Bt": 61.9789,
+        "K2O_Bt": 94.196,
+        "MnO_Bt": 70.9375,
+        "TiO2_Bt": 79.7877,
+        "Cr2O3_Bt": 151.9982,
+        "P2O5_Bt": 141.937,
+    }
+    oxide_mass_bt_df = pd.DataFrame.from_dict(oxide_mass_bt, orient="index").T
+    oxide_mass_bt_df["Sample_ID_Bt"] = "MolWt"
+    oxide_mass_bt_df.set_index("Sample_ID_Bt", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     bt_wt = bt_comps.reindex(oxide_mass_bt_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    bt_wt_combo = pd.concat([oxide_mass_bt_df, bt_wt],)
+    bt_wt_combo = pd.concat(
+        [oxide_mass_bt_df, bt_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = bt_wt_combo.div(
-        bt_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = bt_wt_combo.div(bt_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
-def calculate_cat_proportions_biotite(*, bt_comps=None, oxide_headers=False):
 
+def calculate_cat_proportions_biotite(*, bt_comps=None, oxide_headers=False):
     """
 
     Import biotite compositions using bt_comps=My_biotites, returns cation proportions
 
     Parameters
     -------
     bt_comps: pandas.DataFrame
@@ -3814,216 +5439,316 @@
     Returns
     -------
     pandas DataFrame
         cation proportions for biotite with column headings of the form... Bt_cat_prop
 
     """
 
-    cation_num_bt = {'SiO2_Bt': 1, 'MgO_Bt': 1, 'FeOt_Bt': 1, 'CaO_Bt': 1, 'Al2O3_Bt': 2, 'Na2O_Bt': 2, 'K2O_Bt': 2, 'MnO_Bt': 1, 'TiO2_Bt': 1, 'Cr2O3_Bt': 2, 'P2O5_Bt': 2}
-    cation_num_bt_df = pd.DataFrame.from_dict(cation_num_bt, orient='index').T
-    cation_num_bt_df['Sample_ID_Bt'] = 'CatNum'
-    cation_num_bt_df.set_index('Sample_ID_Bt', inplace=True)
-
-    oxide_mass_bt = {'SiO2_Bt': 60.0843, 'MgO_Bt': 40.3044, 'FeOt_Bt': 71.8464, 'CaO_Bt': 56.0774,'Al2O3_Bt': 101.961, 'Na2O_Bt': 61.9789, 'K2O_Bt': 94.196, 'MnO_Bt': 70.9375, 'TiO2_Bt': 79.7877, 'Cr2O3_Bt': 151.9982, 'P2O5_Bt': 141.937}
-
-    oxide_mass_bt_df = pd.DataFrame.from_dict(oxide_mass_bt, orient='index').T
-    oxide_mass_bt_df['Sample_ID_Bt'] = 'MolWt'
-    oxide_mass_bt_df.set_index('Sample_ID_Bt', inplace=True)
+    cation_num_bt = {
+        "SiO2_Bt": 1,
+        "MgO_Bt": 1,
+        "FeOt_Bt": 1,
+        "CaO_Bt": 1,
+        "Al2O3_Bt": 2,
+        "Na2O_Bt": 2,
+        "K2O_Bt": 2,
+        "MnO_Bt": 1,
+        "TiO2_Bt": 1,
+        "Cr2O3_Bt": 2,
+        "P2O5_Bt": 2,
+    }
+    cation_num_bt_df = pd.DataFrame.from_dict(cation_num_bt, orient="index").T
+    cation_num_bt_df["Sample_ID_Bt"] = "CatNum"
+    cation_num_bt_df.set_index("Sample_ID_Bt", inplace=True)
+
+    oxide_mass_bt = {
+        "SiO2_Bt": 60.0843,
+        "MgO_Bt": 40.3044,
+        "FeOt_Bt": 71.8464,
+        "CaO_Bt": 56.0774,
+        "Al2O3_Bt": 101.961,
+        "Na2O_Bt": 61.9789,
+        "K2O_Bt": 94.196,
+        "MnO_Bt": 70.9375,
+        "TiO2_Bt": 79.7877,
+        "Cr2O3_Bt": 151.9982,
+        "P2O5_Bt": 141.937,
+    }
+
+    oxide_mass_bt_df = pd.DataFrame.from_dict(oxide_mass_bt, orient="index").T
+    oxide_mass_bt_df["Sample_ID_Bt"] = "MolWt"
+    oxide_mass_bt_df.set_index("Sample_ID_Bt", inplace=True)
 
     bt_prop_no_cat_num = calculate_mol_proportions_biotite(bt_comps=bt_comps)
-    bt_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in bt_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_bt_df.reindex(oxide_mass_bt_df.columns, axis=1).fillna(0)
+    bt_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in bt_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_bt_df.reindex(oxide_mass_bt_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, bt_prop_no_cat_num])
-    cation_prop_anhyd = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
-    
+    cation_prop_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
+
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Bt_cat_prop': 'Si_Bt_cat_prop',
-                            'TiO2_Bt_cat_prop': 'Ti_Bt_cat_prop',
-                            'Al2O3_Bt_cat_prop': 'Al_Bt_cat_prop',
-                            'FeOt_Bt_cat_prop': 'Fet_Bt_cat_prop',
-                            'MnO_Bt_cat_prop': 'Mn_Bt_cat_prop',
-                            'MgO_Bt_cat_prop': 'Mg_Bt_cat_prop',
-                            'CaO_Bt_cat_prop': 'Ca_Bt_cat_prop',
-                            'Na2O_Bt_cat_prop': 'Na_Bt_cat_prop',
-                            'K2O_Bt_cat_prop': 'K_Bt_cat_prop',
-                            'Cr2O3_Bt_cat_prop': 'Cr_Bt_cat_prop',
-                            'P2O5_Bt_cat_prop': 'P_Bt_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Bt_cat_prop": "Si_Bt_cat_prop",
+                "TiO2_Bt_cat_prop": "Ti_Bt_cat_prop",
+                "Al2O3_Bt_cat_prop": "Al_Bt_cat_prop",
+                "FeOt_Bt_cat_prop": "Fet_Bt_cat_prop",
+                "MnO_Bt_cat_prop": "Mn_Bt_cat_prop",
+                "MgO_Bt_cat_prop": "Mg_Bt_cat_prop",
+                "CaO_Bt_cat_prop": "Ca_Bt_cat_prop",
+                "Na2O_Bt_cat_prop": "Na_Bt_cat_prop",
+                "K2O_Bt_cat_prop": "K_Bt_cat_prop",
+                "Cr2O3_Bt_cat_prop": "Cr_Bt_cat_prop",
+                "P2O5_Bt_cat_prop": "P_Bt_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
+
 def calculate_oxygens_biotite(bt_comps):
-    
     """
-    
+
     Import biotite compositions using bt_comps=My_Bts, returns number of oxygens (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     bt_comps: pandas.DataFrame
         biotite compositions with column headings SiO2_Bt, MgO_Bt etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Bt_ox
     """
 
-    oxygen_num_bt = {'SiO2_Bt': 2, 'MgO_Bt': 1, 'FeOt_Bt': 1, 'CaO_Bt': 1, 'Al2O3_Bt': 3, 'Na2O_Bt': 1, 'K2O_Bt': 1, 'MnO_Bt': 1, 'TiO2_Bt': 2, 'Cr2O3_Bt': 3, 'P2O5_Bt': 5}
-    oxygen_num_bt_df = pd.DataFrame.from_dict(oxygen_num_bt, orient='index').T
-    oxygen_num_bt_df['Sample_ID_Bt'] = 'OxNum'
-    oxygen_num_bt_df.set_index('Sample_ID_Bt', inplace=True)
+    oxygen_num_bt = {
+        "SiO2_Bt": 2,
+        "MgO_Bt": 1,
+        "FeOt_Bt": 1,
+        "CaO_Bt": 1,
+        "Al2O3_Bt": 3,
+        "Na2O_Bt": 1,
+        "K2O_Bt": 1,
+        "MnO_Bt": 1,
+        "TiO2_Bt": 2,
+        "Cr2O3_Bt": 3,
+        "P2O5_Bt": 5,
+    }
+    oxygen_num_bt_df = pd.DataFrame.from_dict(oxygen_num_bt, orient="index").T
+    oxygen_num_bt_df["Sample_ID_Bt"] = "OxNum"
+    oxygen_num_bt_df.set_index("Sample_ID_Bt", inplace=True)
 
     mol_prop = calculate_mol_proportions_biotite(bt_comps=bt_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '') for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_bt_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
+
 def calculate_10oxygens_biotite(bt_comps):
-    
     """
-    
+
     Import biotite compositions using bt_comps=My_Bts, returns cations on the basis of 10 oxygens.
-    
+
     Parameters
     -------
     bt_comps: pandas.DataFrame
         biotite compositions with column headings SiO2_Bt, MgO_Bt etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 10 oxygens, with column headings of the form... Bt_cat_10ox.
 
     """
 
-    cation_num_bt = {'SiO2_Bt': 1, 'MgO_Bt': 1, 'FeOt_Bt': 1, 'CaO_Bt': 1, 'Al2O3_Bt': 2, 'Na2O_Bt': 2, 'K2O_Bt': 2, 'MnO_Bt': 1, 'TiO2_Bt': 1, 'Cr2O3_Bt': 2, 'P2O5_Bt': 2}
-
-    cation_num_bt_df = pd.DataFrame.from_dict(cation_num_bt, orient='index').T
-    cation_num_bt_df['Sample_ID_Bt'] = 'CatNum'
-    cation_num_bt_df.set_index('Sample_ID_Bt', inplace=True)
+    cation_num_bt = {
+        "SiO2_Bt": 1,
+        "MgO_Bt": 1,
+        "FeOt_Bt": 1,
+        "CaO_Bt": 1,
+        "Al2O3_Bt": 2,
+        "Na2O_Bt": 2,
+        "K2O_Bt": 2,
+        "MnO_Bt": 1,
+        "TiO2_Bt": 1,
+        "Cr2O3_Bt": 2,
+        "P2O5_Bt": 2,
+    }
+
+    cation_num_bt_df = pd.DataFrame.from_dict(cation_num_bt, orient="index").T
+    cation_num_bt_df["Sample_ID_Bt"] = "CatNum"
+    cation_num_bt_df.set_index("Sample_ID_Bt", inplace=True)
 
     oxygens = calculate_oxygens_biotite(bt_comps=bt_comps)
-    renorm_factor = 10 / (oxygens.sum(axis='columns'))
+    renorm_factor = 10 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_biotite(bt_comps=bt_comps)
-    mol_prop['oxy_renorm_factor_bt'] = renorm_factor
-    mol_prop_10 = mol_prop.multiply(mol_prop['oxy_renorm_factor_bt'], axis='rows')
-    mol_prop_10.columns = [str(col).replace('_mol_prop', '') for col in mol_prop_10.columns]
+    mol_prop["oxy_renorm_factor_bt"] = renorm_factor
+    mol_prop_10 = mol_prop.multiply(mol_prop["oxy_renorm_factor_bt"], axis="rows")
+    mol_prop_10.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_10.columns
+    ]
 
     ox_num_reindex = cation_num_bt_df.reindex(mol_prop_10.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_10])
-    cation_10 = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_10.columns = [str(col).replace('_mol_prop', '_cat_10ox') for col in mol_prop.columns]
-
-    cation_10_2=cation_10.rename(columns={
-                            'SiO2_Bt_cat_10ox': 'Si_Bt_cat_10ox',
-                            'TiO2_Bt_cat_10ox': 'Ti_Bt_cat_10ox',
-                            'Al2O3_Bt_cat_10ox': 'Al_Bt_cat_10ox',
-                            'FeOt_Bt_cat_10ox': 'Fet_Bt_cat_10ox',
-                            'MnO_Bt_cat_10ox': 'Mn_Bt_cat_10ox',
-                            'MgO_Bt_cat_10ox': 'Mg_Bt_cat_10ox',
-                            'CaO_Bt_cat_10ox': 'Ca_Bt_cat_10ox',
-                            'Na2O_Bt_cat_10ox': 'Na_Bt_cat_10ox',
-                            'K2O_Bt_cat_10ox': 'K_Bt_cat_10ox',
-                            'Cr2O3_Bt_cat_10ox': 'Cr_Bt_cat_10ox',
-                            'P2O5_Bt_cat_10ox': 'P_Bt_cat_10ox',})
+    cation_10 = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+
+    cation_10.columns = [
+        str(col).replace("_mol_prop", "_cat_10ox") for col in mol_prop.columns
+    ]
+
+    cation_10_2 = cation_10.rename(
+        columns={
+            "SiO2_Bt_cat_10ox": "Si_Bt_cat_10ox",
+            "TiO2_Bt_cat_10ox": "Ti_Bt_cat_10ox",
+            "Al2O3_Bt_cat_10ox": "Al_Bt_cat_10ox",
+            "FeOt_Bt_cat_10ox": "Fet_Bt_cat_10ox",
+            "MnO_Bt_cat_10ox": "Mn_Bt_cat_10ox",
+            "MgO_Bt_cat_10ox": "Mg_Bt_cat_10ox",
+            "CaO_Bt_cat_10ox": "Ca_Bt_cat_10ox",
+            "Na2O_Bt_cat_10ox": "Na_Bt_cat_10ox",
+            "K2O_Bt_cat_10ox": "K_Bt_cat_10ox",
+            "Cr2O3_Bt_cat_10ox": "Cr_Bt_cat_10ox",
+            "P2O5_Bt_cat_10ox": "P_Bt_cat_10ox",
+        }
+    )
 
     return cation_10_2
 
 
 def calculate_biotite_components(bt_comps, append):
-    
     """
-    
+
     Import Biotite compositions using bt_comps=My_Biotites, returns mole proportions
-    
+
     Parameters
     -------
     bt_comps: pandas.DataFrame
             Panda DataFrame of biotite compositions with column headings SiO2_Bt, MgO_Bt etc.
-    
+
     Returns
     -------
     pandas DataFrame
         components for biotites with column headings of the form SiO2_Bt_mol_prop
 
     """
 
     bt_comps_new = bt_comps.copy()
-    bt_comps_new.columns = [col.replace(append, '_Bt') for col in bt_comps_new.columns]
+    bt_comps_new.columns = [col.replace(append, "_Bt") for col in bt_comps_new.columns]
     bt_comps = bt_comps_new.copy()
 
     bt_calc = calculate_10oxygens_biotite(bt_comps=bt_comps)
-    bt_calc['Bt_Cation_Sum'] = (bt_calc['Si_Bt_cat_10ox']+bt_calc['Ti_Bt_cat_10ox']+bt_calc['Al_Bt_cat_10ox']+bt_calc['Fet_Bt_cat_10ox']+bt_calc['Mn_Bt_cat_10ox']+bt_calc['Mg_Bt_cat_10ox']+bt_calc['Ca_Bt_cat_10ox']+bt_calc['Na_Bt_cat_10ox']+bt_calc['K_Bt_cat_10ox']+bt_calc['Cr_Bt_cat_10ox']+bt_calc['P_Bt_cat_10ox'])
-
-    bt_calc['Mg_Fe_M_Bt'] = bt_calc['Mg_Bt_cat_10ox'] + bt_calc['Fet_Bt_cat_10ox']
-    bt_calc['Si_Al_T_Bt'] = bt_calc['Si_Bt_cat_10ox'] + bt_calc['Al_Bt_cat_10ox']
-
-    bt_calc['Mg_Fe_Mn_Ti_M_Bt'] = bt_calc['Mg_Bt_cat_10ox'] + bt_calc['Fet_Bt_cat_10ox'] + bt_calc['Mn_Bt_cat_10ox'] + bt_calc['Ti_Bt_cat_10ox']
+    bt_calc["Bt_Cation_Sum"] = (
+        bt_calc["Si_Bt_cat_10ox"]
+        + bt_calc["Ti_Bt_cat_10ox"]
+        + bt_calc["Al_Bt_cat_10ox"]
+        + bt_calc["Fet_Bt_cat_10ox"]
+        + bt_calc["Mn_Bt_cat_10ox"]
+        + bt_calc["Mg_Bt_cat_10ox"]
+        + bt_calc["Ca_Bt_cat_10ox"]
+        + bt_calc["Na_Bt_cat_10ox"]
+        + bt_calc["K_Bt_cat_10ox"]
+        + bt_calc["Cr_Bt_cat_10ox"]
+        + bt_calc["P_Bt_cat_10ox"]
+    )
+
+    bt_calc["Mg_Fe_M_Bt"] = bt_calc["Mg_Bt_cat_10ox"] + bt_calc["Fet_Bt_cat_10ox"]
+    bt_calc["Si_Al_T_Bt"] = bt_calc["Si_Bt_cat_10ox"] + bt_calc["Al_Bt_cat_10ox"]
+
+    bt_calc["Mg_Fe_Mn_Ti_M_Bt"] = (
+        bt_calc["Mg_Bt_cat_10ox"]
+        + bt_calc["Fet_Bt_cat_10ox"]
+        + bt_calc["Mn_Bt_cat_10ox"]
+        + bt_calc["Ti_Bt_cat_10ox"]
+    )
 
     cat_prop = calculate_cat_proportions_biotite(bt_comps=bt_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac') for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([bt_comps, bt_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-
-# %% MUSCOVITE 
+# %% MUSCOVITE
 
 
 def calculate_mol_proportions_muscovite(ms_comps):
-
     """
-    
+
     Import Muscovite compositions using ms_comps=My_Muscovites, returns mole proportions
-   
+
     Parameters
     -------
     ms_comps: pandas.DataFrame
             Panda DataFrame of muscovite compositions with column headings SiO2_Ms, MgO_Ms etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for muscovites with column headings of the form SiO2_Ms_mol_prop
 
     """
 
-    oxide_mass_ms = {'SiO2_Ms': 60.0843, 'MgO_Ms': 40.3044, 'FeOt_Ms': 71.8464, 'CaO_Ms': 56.0774,'Al2O3_Ms': 101.961, 'Na2O_Ms': 61.9789, 'K2O_Ms': 94.196, 'MnO_Ms': 70.9375, 'TiO2_Ms': 79.7877, 'Cr2O3_Ms': 151.9982, 'P2O5_Ms': 141.937}
-    oxide_mass_ms_df = pd.DataFrame.from_dict(oxide_mass_ms, orient='index').T
-    oxide_mass_ms_df['Sample_ID_Ms'] = 'MolWt'
-    oxide_mass_ms_df.set_index('Sample_ID_Ms', inplace=True)
+    oxide_mass_ms = {
+        "SiO2_Ms": 60.0843,
+        "MgO_Ms": 40.3044,
+        "FeOt_Ms": 71.8464,
+        "CaO_Ms": 56.0774,
+        "Al2O3_Ms": 101.961,
+        "Na2O_Ms": 61.9789,
+        "K2O_Ms": 94.196,
+        "MnO_Ms": 70.9375,
+        "TiO2_Ms": 79.7877,
+        "Cr2O3_Ms": 151.9982,
+        "P2O5_Ms": 141.937,
+    }
+    oxide_mass_ms_df = pd.DataFrame.from_dict(oxide_mass_ms, orient="index").T
+    oxide_mass_ms_df["Sample_ID_Ms"] = "MolWt"
+    oxide_mass_ms_df.set_index("Sample_ID_Ms", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     ms_wt = ms_comps.reindex(oxide_mass_ms_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    ms_wt_combo = pd.concat([oxide_mass_ms_df, ms_wt],)
+    ms_wt_combo = pd.concat(
+        [oxide_mass_ms_df, ms_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = ms_wt_combo.div(
-        ms_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = ms_wt_combo.div(ms_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
-def calculate_cat_proportions_muscovite(*, ms_comps=None, oxide_headers=False):
 
+def calculate_cat_proportions_muscovite(*, ms_comps=None, oxide_headers=False):
     """
-    
+
     Import muscovite compositions using ms_comps=My_muscovites, returns cation proportions
 
     Parameters
     -------
     ms_comps: pandas.DataFrame
             muscovite compositions with column headings SiO2_Ms, MgO_Ms etc.
     oxide_headers: bool
@@ -4035,220 +5760,318 @@
     Returns
     -------
     pandas DataFrame
         cation proportions for muscovite with column headings of the form... Ms_cat_prop
 
     """
 
-    cation_num_ms = {'SiO2_Ms': 1, 'MgO_Ms': 1, 'FeOt_Ms': 1, 'CaO_Ms': 1, 'Al2O3_Ms': 2, 'Na2O_Ms': 2, 'K2O_Ms': 2, 'MnO_Ms': 1, 'TiO2_Ms': 1, 'Cr2O3_Ms': 2, 'P2O5_Ms': 2}
-    cation_num_ms_df = pd.DataFrame.from_dict(cation_num_ms, orient='index').T
-    cation_num_ms_df['Sample_ID_Ms'] = 'CatNum'
-    cation_num_ms_df.set_index('Sample_ID_Ms', inplace=True)
-
-    oxide_mass_ms = {'SiO2_Ms': 60.0843, 'MgO_Ms': 40.3044, 'FeOt_Ms': 71.8464, 'CaO_Ms': 56.0774,'Al2O3_Ms': 101.961, 'Na2O_Ms': 61.9789, 'K2O_Ms': 94.196, 'MnO_Ms': 70.9375, 'TiO2_Ms': 79.7877, 'Cr2O3_Ms': 151.9982, 'P2O5_Ms': 141.937}
-
-    oxide_mass_ms_df = pd.DataFrame.from_dict(oxide_mass_ms, orient='index').T
-    oxide_mass_ms_df['Sample_ID_Ms'] = 'MolWt'
-    oxide_mass_ms_df.set_index('Sample_ID_Ms', inplace=True)
+    cation_num_ms = {
+        "SiO2_Ms": 1,
+        "MgO_Ms": 1,
+        "FeOt_Ms": 1,
+        "CaO_Ms": 1,
+        "Al2O3_Ms": 2,
+        "Na2O_Ms": 2,
+        "K2O_Ms": 2,
+        "MnO_Ms": 1,
+        "TiO2_Ms": 1,
+        "Cr2O3_Ms": 2,
+        "P2O5_Ms": 2,
+    }
+    cation_num_ms_df = pd.DataFrame.from_dict(cation_num_ms, orient="index").T
+    cation_num_ms_df["Sample_ID_Ms"] = "CatNum"
+    cation_num_ms_df.set_index("Sample_ID_Ms", inplace=True)
+
+    oxide_mass_ms = {
+        "SiO2_Ms": 60.0843,
+        "MgO_Ms": 40.3044,
+        "FeOt_Ms": 71.8464,
+        "CaO_Ms": 56.0774,
+        "Al2O3_Ms": 101.961,
+        "Na2O_Ms": 61.9789,
+        "K2O_Ms": 94.196,
+        "MnO_Ms": 70.9375,
+        "TiO2_Ms": 79.7877,
+        "Cr2O3_Ms": 151.9982,
+        "P2O5_Ms": 141.937,
+    }
+
+    oxide_mass_ms_df = pd.DataFrame.from_dict(oxide_mass_ms, orient="index").T
+    oxide_mass_ms_df["Sample_ID_Ms"] = "MolWt"
+    oxide_mass_ms_df.set_index("Sample_ID_Ms", inplace=True)
 
     ms_prop_no_cat_num = calculate_mol_proportions_muscovite(ms_comps=ms_comps)
-    ms_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in ms_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_ms_df.reindex(oxide_mass_ms_df.columns, axis=1).fillna(0)
+    ms_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in ms_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_ms_df.reindex(oxide_mass_ms_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, ms_prop_no_cat_num])
-    cation_prop_anhyd = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
-    
+    cation_prop_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
+
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Ms_cat_prop': 'Si_Ms_cat_prop',
-                            'TiO2_Ms_cat_prop': 'Ti_Ms_cat_prop',
-                            'Al2O3_Ms_cat_prop': 'Al_Ms_cat_prop',
-                            'FeOt_Ms_cat_prop': 'Fet_Ms_cat_prop',
-                            'MnO_Ms_cat_prop': 'Mn_Ms_cat_prop',
-                            'MgO_Ms_cat_prop': 'Mg_Ms_cat_prop',
-                            'CaO_Ms_cat_prop': 'Ca_Ms_cat_prop',
-                            'Na2O_Ms_cat_prop': 'Na_Ms_cat_prop',
-                            'K2O_Ms_cat_prop': 'K_Ms_cat_prop',
-                            'Cr2O3_Ms_cat_prop': 'Cr_Ms_cat_prop',
-                            'P2O5_Ms_cat_prop': 'P_Ms_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Ms_cat_prop": "Si_Ms_cat_prop",
+                "TiO2_Ms_cat_prop": "Ti_Ms_cat_prop",
+                "Al2O3_Ms_cat_prop": "Al_Ms_cat_prop",
+                "FeOt_Ms_cat_prop": "Fet_Ms_cat_prop",
+                "MnO_Ms_cat_prop": "Mn_Ms_cat_prop",
+                "MgO_Ms_cat_prop": "Mg_Ms_cat_prop",
+                "CaO_Ms_cat_prop": "Ca_Ms_cat_prop",
+                "Na2O_Ms_cat_prop": "Na_Ms_cat_prop",
+                "K2O_Ms_cat_prop": "K_Ms_cat_prop",
+                "Cr2O3_Ms_cat_prop": "Cr_Ms_cat_prop",
+                "P2O5_Ms_cat_prop": "P_Ms_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
+
 def calculate_oxygens_muscovite(ms_comps):
-    
     """
-    
+
     Import muscovite compositions using ms_comps=My_Mss, returns number of oxygens (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     ms_comps: pandas.DataFrame
         muscovite compositions with column headings SiO2_Ms, MgO_Ms etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Ms_ox
 
     """
 
-    oxygen_num_ms = {'SiO2_Ms': 2, 'MgO_Ms': 1, 'FeOt_Ms': 1, 'CaO_Ms': 1, 'Al2O3_Ms': 3, 'Na2O_Ms': 1, 'K2O_Ms': 1, 'MnO_Ms': 1, 'TiO2_Ms': 2, 'Cr2O3_Ms': 3, 'P2O5_Ms': 5}
-    oxygen_num_ms_df = pd.DataFrame.from_dict(oxygen_num_ms, orient='index').T
-    oxygen_num_ms_df['Sample_ID_Ms'] = 'OxNum'
-    oxygen_num_ms_df.set_index('Sample_ID_Ms', inplace=True)
+    oxygen_num_ms = {
+        "SiO2_Ms": 2,
+        "MgO_Ms": 1,
+        "FeOt_Ms": 1,
+        "CaO_Ms": 1,
+        "Al2O3_Ms": 3,
+        "Na2O_Ms": 1,
+        "K2O_Ms": 1,
+        "MnO_Ms": 1,
+        "TiO2_Ms": 2,
+        "Cr2O3_Ms": 3,
+        "P2O5_Ms": 5,
+    }
+    oxygen_num_ms_df = pd.DataFrame.from_dict(oxygen_num_ms, orient="index").T
+    oxygen_num_ms_df["Sample_ID_Ms"] = "OxNum"
+    oxygen_num_ms_df.set_index("Sample_ID_Ms", inplace=True)
 
     mol_prop = calculate_mol_proportions_muscovite(ms_comps=ms_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '') for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_ms_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
+
 def calculate_10oxygens_muscovite(ms_comps):
-    
     """
-    
+
     Import muscovite compositions using ms_comps=My_Mss, returns cations on the basis of 10 oxygens.
-    
+
     Parameters
     -------
     ms_comps: pandas.DataFrame
         muscovite compositions with column headings SiO2_Ms, MgO_Ms etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 10 oxygens, with column headings of the form... Ms_cat_10ox.
 
     """
 
-    cation_num_ms = {'SiO2_Ms': 1, 'MgO_Ms': 1, 'FeOt_Ms': 1, 'CaO_Ms': 1, 'Al2O3_Ms': 2, 'Na2O_Ms': 2, 'K2O_Ms': 2, 'MnO_Ms': 1, 'TiO2_Ms': 1, 'Cr2O3_Ms': 2, 'P2O5_Ms': 2}
-
-    cation_num_ms_df = pd.DataFrame.from_dict(cation_num_ms, orient='index').T
-    cation_num_ms_df['Sample_ID_Ms'] = 'CatNum'
-    cation_num_ms_df.set_index('Sample_ID_Ms', inplace=True)
+    cation_num_ms = {
+        "SiO2_Ms": 1,
+        "MgO_Ms": 1,
+        "FeOt_Ms": 1,
+        "CaO_Ms": 1,
+        "Al2O3_Ms": 2,
+        "Na2O_Ms": 2,
+        "K2O_Ms": 2,
+        "MnO_Ms": 1,
+        "TiO2_Ms": 1,
+        "Cr2O3_Ms": 2,
+        "P2O5_Ms": 2,
+    }
+
+    cation_num_ms_df = pd.DataFrame.from_dict(cation_num_ms, orient="index").T
+    cation_num_ms_df["Sample_ID_Ms"] = "CatNum"
+    cation_num_ms_df.set_index("Sample_ID_Ms", inplace=True)
 
     oxygens = calculate_oxygens_muscovite(ms_comps=ms_comps)
-    renorm_factor = 10 / (oxygens.sum(axis='columns'))
+    renorm_factor = 10 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_muscovite(ms_comps=ms_comps)
-    mol_prop['oxy_renorm_factor_ms'] = renorm_factor
-    mol_prop_10 = mol_prop.multiply(mol_prop['oxy_renorm_factor_ms'], axis='rows')
-    mol_prop_10.columns = [str(col).replace('_mol_prop', '') for col in mol_prop_10.columns]
+    mol_prop["oxy_renorm_factor_ms"] = renorm_factor
+    mol_prop_10 = mol_prop.multiply(mol_prop["oxy_renorm_factor_ms"], axis="rows")
+    mol_prop_10.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_10.columns
+    ]
 
     ox_num_reindex = cation_num_ms_df.reindex(mol_prop_10.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_10])
-    cation_10 = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_10.columns = [str(col).replace('_mol_prop', '_cat_10ox') for col in mol_prop.columns]
-
-    cation_10_2=cation_10.rename(columns={
-                            'SiO2_Ms_cat_10ox': 'Si_Ms_cat_10ox',
-                            'TiO2_Ms_cat_10ox': 'Ti_Ms_cat_10ox',
-                            'Al2O3_Ms_cat_10ox': 'Al_Ms_cat_10ox',
-                            'FeOt_Ms_cat_10ox': 'Fet_Ms_cat_10ox',
-                            'MnO_Ms_cat_10ox': 'Mn_Ms_cat_10ox',
-                            'MgO_Ms_cat_10ox': 'Mg_Ms_cat_10ox',
-                            'CaO_Ms_cat_10ox': 'Ca_Ms_cat_10ox',
-                            'Na2O_Ms_cat_10ox': 'Na_Ms_cat_10ox',
-                            'K2O_Ms_cat_10ox': 'K_Ms_cat_10ox',
-                            'Cr2O3_Ms_cat_10ox': 'Cr_Ms_cat_10ox',
-                            'P2O5_Ms_cat_10ox': 'P_Ms_cat_10ox',})
+    cation_10 = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+
+    cation_10.columns = [
+        str(col).replace("_mol_prop", "_cat_10ox") for col in mol_prop.columns
+    ]
+
+    cation_10_2 = cation_10.rename(
+        columns={
+            "SiO2_Ms_cat_10ox": "Si_Ms_cat_10ox",
+            "TiO2_Ms_cat_10ox": "Ti_Ms_cat_10ox",
+            "Al2O3_Ms_cat_10ox": "Al_Ms_cat_10ox",
+            "FeOt_Ms_cat_10ox": "Fet_Ms_cat_10ox",
+            "MnO_Ms_cat_10ox": "Mn_Ms_cat_10ox",
+            "MgO_Ms_cat_10ox": "Mg_Ms_cat_10ox",
+            "CaO_Ms_cat_10ox": "Ca_Ms_cat_10ox",
+            "Na2O_Ms_cat_10ox": "Na_Ms_cat_10ox",
+            "K2O_Ms_cat_10ox": "K_Ms_cat_10ox",
+            "Cr2O3_Ms_cat_10ox": "Cr_Ms_cat_10ox",
+            "P2O5_Ms_cat_10ox": "P_Ms_cat_10ox",
+        }
+    )
 
     return cation_10_2
 
 
 def calculate_muscovite_components(ms_comps, append):
-    
     """
-    
+
     Import Muscovite compositions using ms_comps=My_Muscovites, returns mole proportions
-    
+
     Parameters
     -------
     ms_comps: pandas.DataFrame
             Panda DataFrame of muscovite compositions with column headings SiO2_Ms, MgO_Ms etc.
-    
+
     Returns
     -------
     pandas DataFrame
         components for muscovites with column headings of the form SiO2_Ms_mol_prop
 
     """
 
     ms_comps_new = ms_comps.copy()
-    ms_comps_new.columns = [col.replace(append, '_Ms') for col in ms_comps_new.columns]
+    ms_comps_new.columns = [col.replace(append, "_Ms") for col in ms_comps_new.columns]
     ms_comps = ms_comps_new.copy()
 
     ms_calc = calculate_10oxygens_muscovite(ms_comps=ms_comps)
-    ms_calc['Ms_Cation_Sum'] = (ms_calc['Si_Ms_cat_10ox']+ms_calc['Ti_Ms_cat_10ox']+ms_calc['Al_Ms_cat_10ox']+ms_calc['Fet_Ms_cat_10ox']+ms_calc['Mn_Ms_cat_10ox']+ms_calc['Mg_Ms_cat_10ox']+ms_calc['Ca_Ms_cat_10ox']+ms_calc['Na_Ms_cat_10ox']+ms_calc['K_Ms_cat_10ox']+ms_calc['Cr_Ms_cat_10ox']+ms_calc['P_Ms_cat_10ox'])
-
-    ms_calc['K_Na_M_Ms'] = ms_calc['K_Ms_cat_10ox'] + ms_calc['Na_Ms_cat_10ox'] 
-    ms_calc['Mg_Fe_Al_O_Ms'] = ms_calc['Mg_Ms_cat_10ox'] + ms_calc['Fet_Ms_cat_10ox'] + ms_calc['Al_Ms_cat_10ox']
-    ms_calc['Si_Al_T_Ms'] = ms_calc['Si_Ms_cat_10ox'] + ms_calc['Al_Ms_cat_10ox']
+    ms_calc["Ms_Cation_Sum"] = (
+        ms_calc["Si_Ms_cat_10ox"]
+        + ms_calc["Ti_Ms_cat_10ox"]
+        + ms_calc["Al_Ms_cat_10ox"]
+        + ms_calc["Fet_Ms_cat_10ox"]
+        + ms_calc["Mn_Ms_cat_10ox"]
+        + ms_calc["Mg_Ms_cat_10ox"]
+        + ms_calc["Ca_Ms_cat_10ox"]
+        + ms_calc["Na_Ms_cat_10ox"]
+        + ms_calc["K_Ms_cat_10ox"]
+        + ms_calc["Cr_Ms_cat_10ox"]
+        + ms_calc["P_Ms_cat_10ox"]
+    )
+
+    ms_calc["K_Na_M_Ms"] = ms_calc["K_Ms_cat_10ox"] + ms_calc["Na_Ms_cat_10ox"]
+    ms_calc["Mg_Fe_Al_O_Ms"] = (
+        ms_calc["Mg_Ms_cat_10ox"]
+        + ms_calc["Fet_Ms_cat_10ox"]
+        + ms_calc["Al_Ms_cat_10ox"]
+    )
+    ms_calc["Si_Al_T_Ms"] = ms_calc["Si_Ms_cat_10ox"] + ms_calc["Al_Ms_cat_10ox"]
 
     cat_prop = calculate_cat_proportions_muscovite(ms_comps=ms_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac') for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([ms_comps, ms_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
+# %% RUTILE
 
 
-
-# %% RUTILE 
-
 def calculate_mol_proportions_rutile(rt_comps):
-
     """
-    
+
     Import Rutile compositions using rt_comps=My_Rutiles, returns mole proportions
 
     Parameters
     -------
     rt_comps: pandas.DataFrame
             Panda DataFrame of rutile compositions with column headings SiO2_Rt, MgO_Rt etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for rutiles with column headings of the form SiO2_Rt_mol_prop
 
     """
 
-    oxide_mass_rt = {'SiO2_Rt': 60.0843, 'MgO_Rt': 40.3044, 'FeOt_Rt': 71.8464, 'CaO_Rt': 56.0774, 'Al2O3_Rt': 101.961, 'Na2O_Rt': 61.9789, 'K2O_Rt': 94.196, 'MnO_Rt': 70.9375, 'TiO2_Rt': 79.7877, 'Cr2O3_Rt': 151.9982, 'P2O5_Rt': 141.937, 'ZrO2_Rt':123.218}
-    oxide_mass_rt_df = pd.DataFrame.from_dict(oxide_mass_rt, orient='index').T
-    oxide_mass_rt_df['Sample_ID_Rt'] = 'MolWt'
-    oxide_mass_rt_df.set_index('Sample_ID_Rt', inplace=True)
+    oxide_mass_rt = {
+        "SiO2_Rt": 60.0843,
+        "MgO_Rt": 40.3044,
+        "FeOt_Rt": 71.8464,
+        "CaO_Rt": 56.0774,
+        "Al2O3_Rt": 101.961,
+        "Na2O_Rt": 61.9789,
+        "K2O_Rt": 94.196,
+        "MnO_Rt": 70.9375,
+        "TiO2_Rt": 79.7877,
+        "Cr2O3_Rt": 151.9982,
+        "P2O5_Rt": 141.937,
+        "ZrO2_Rt": 123.218,
+    }
+    oxide_mass_rt_df = pd.DataFrame.from_dict(oxide_mass_rt, orient="index").T
+    oxide_mass_rt_df["Sample_ID_Rt"] = "MolWt"
+    oxide_mass_rt_df.set_index("Sample_ID_Rt", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     rt_wt = rt_comps.reindex(oxide_mass_rt_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    rt_wt_combo = pd.concat([oxide_mass_rt_df, rt_wt],)
+    rt_wt_combo = pd.concat(
+        [oxide_mass_rt_df, rt_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = rt_wt_combo.div(
-        rt_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = rt_wt_combo.div(rt_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
 
 def calculate_cat_proportions_rutile(*, rt_comps=None, oxide_headers=False):
-    
     """
-    
+
     Import rutile compositions using rt_comps=My_rutiles, returns cation proportions
-    
+
     Parameters
     -------
     rt_comps: pandas.DataFrame
             rutile compositions with column headings SiO2_Plag, MgO_Plag etc.
     oxide_headers: bool
         default=False, returns as Ti_Rt_cat_prop.
         =True returns Ti_Rt_cat_prop.
@@ -4258,222 +6081,315 @@
     Returns
     -------
     pandas DataFrame
         cation proportions for rutile with column headings of the form... Rt_cat_prop
 
     """
 
-    cation_num_rt = {'SiO2_Rt': 1, 'MgO_Rt': 1, 'FeOt_Rt': 1, 'CaO_Rt': 1, 'Al2O3_Rt': 2, 'Na2O_Rt': 2, 'K2O_Rt': 2, 'MnO_Rt': 1, 'TiO2_Rt': 1, 'Cr2O3_Rt': 2, 'P2O5_Rt': 2, 'ZrO2_Rt': 1}
-    cation_num_rt_df = pd.DataFrame.from_dict(cation_num_rt, orient='index').T
-    cation_num_rt_df['Sample_ID_Rt'] = 'CatNum'
-    cation_num_rt_df.set_index('Sample_ID_Rt', inplace=True)
-
-    oxide_mass_rt = {'SiO2_Rt': 60.0843, 'MgO_Rt': 40.3044, 'FeOt_Rt': 71.8464, 'CaO_Rt': 56.0774,'Al2O3_Rt': 101.961, 'Na2O_Rt': 61.9789, 'K2O_Rt': 94.196,'MnO_Rt': 70.9375, 'TiO2_Rt': 79.7877, 'Cr2O3_Rt': 151.9982, 'P2O5_Rt': 141.937, 'ZrO2_Rt':123.218}
-
-    oxide_mass_rt_df = pd.DataFrame.from_dict(oxide_mass_rt, orient='index').T
-    oxide_mass_rt_df['Sample_ID_Rt'] = 'MolWt'
-    oxide_mass_rt_df.set_index('Sample_ID_Rt', inplace=True)
-
-    rt_prop_no_cat_num = calculate_mol_proportions_rutile(
-        rt_comps=rt_comps)
-    rt_prop_no_cat_num.columns = [str(col).replace(
-        '_mol_prop', '') for col in rt_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_rt_df.reindex(
-        oxide_mass_rt_df.columns, axis=1).fillna(0)
+    cation_num_rt = {
+        "SiO2_Rt": 1,
+        "MgO_Rt": 1,
+        "FeOt_Rt": 1,
+        "CaO_Rt": 1,
+        "Al2O3_Rt": 2,
+        "Na2O_Rt": 2,
+        "K2O_Rt": 2,
+        "MnO_Rt": 1,
+        "TiO2_Rt": 1,
+        "Cr2O3_Rt": 2,
+        "P2O5_Rt": 2,
+        "ZrO2_Rt": 1,
+    }
+    cation_num_rt_df = pd.DataFrame.from_dict(cation_num_rt, orient="index").T
+    cation_num_rt_df["Sample_ID_Rt"] = "CatNum"
+    cation_num_rt_df.set_index("Sample_ID_Rt", inplace=True)
+
+    oxide_mass_rt = {
+        "SiO2_Rt": 60.0843,
+        "MgO_Rt": 40.3044,
+        "FeOt_Rt": 71.8464,
+        "CaO_Rt": 56.0774,
+        "Al2O3_Rt": 101.961,
+        "Na2O_Rt": 61.9789,
+        "K2O_Rt": 94.196,
+        "MnO_Rt": 70.9375,
+        "TiO2_Rt": 79.7877,
+        "Cr2O3_Rt": 151.9982,
+        "P2O5_Rt": 141.937,
+        "ZrO2_Rt": 123.218,
+    }
+
+    oxide_mass_rt_df = pd.DataFrame.from_dict(oxide_mass_rt, orient="index").T
+    oxide_mass_rt_df["Sample_ID_Rt"] = "MolWt"
+    oxide_mass_rt_df.set_index("Sample_ID_Rt", inplace=True)
+
+    rt_prop_no_cat_num = calculate_mol_proportions_rutile(rt_comps=rt_comps)
+    rt_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in rt_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_rt_df.reindex(oxide_mass_rt_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, rt_prop_no_cat_num])
     cation_prop_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
     cation_prop_anhyd.columns = [
-        str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Rt_cat_prop': 'Si_Rt_cat_prop',
-                            'TiO2_Rt_cat_prop': 'Ti_Rt_cat_prop',
-                            'Al2O3_Rt_cat_prop': 'Al_Rt_cat_prop',
-                            'FeOt_Rt_cat_prop': 'Fet_Rt_cat_prop',
-                            'MnO_Rt_cat_prop': 'Mn_Rt_cat_prop',
-                            'MgO_Rt_cat_prop': 'Mg_Rt_cat_prop',
-                            'CaO_Rt_cat_prop': 'Ca_Rt_cat_prop',
-                            'Na2O_Rt_cat_prop': 'Na_Rt_cat_prop',
-                            'K2O_Rt_cat_prop': 'K_Rt_cat_prop',
-                            'Cr2O3_Rt_cat_prop': 'Cr_Rt_cat_prop',
-                            'P2O5_Rt_cat_prop': 'P_Rt_cat_prop',
-                            'ZrO2_Rt_cat_prop': 'Zr_Rt_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Rt_cat_prop": "Si_Rt_cat_prop",
+                "TiO2_Rt_cat_prop": "Ti_Rt_cat_prop",
+                "Al2O3_Rt_cat_prop": "Al_Rt_cat_prop",
+                "FeOt_Rt_cat_prop": "Fet_Rt_cat_prop",
+                "MnO_Rt_cat_prop": "Mn_Rt_cat_prop",
+                "MgO_Rt_cat_prop": "Mg_Rt_cat_prop",
+                "CaO_Rt_cat_prop": "Ca_Rt_cat_prop",
+                "Na2O_Rt_cat_prop": "Na_Rt_cat_prop",
+                "K2O_Rt_cat_prop": "K_Rt_cat_prop",
+                "Cr2O3_Rt_cat_prop": "Cr_Rt_cat_prop",
+                "P2O5_Rt_cat_prop": "P_Rt_cat_prop",
+                "ZrO2_Rt_cat_prop": "Zr_Rt_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
+
 def calculate_oxygens_rutile(rt_comps):
-    
     """
-    
-    Import rutile compositions using rt_comps=My_Rts, returns number of oxygens 
+
+    Import rutile compositions using rt_comps=My_Rts, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     rt_comps: pandas.DataFrame
         rutile compositions with column headings SiO2_Rt, MgO_Rt etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Rt_ox
 
     """
 
-    oxygen_num_rt = {'SiO2_Rt': 2, 'MgO_Rt': 1, 'FeOt_Rt': 1, 'CaO_Rt': 1, 'Al2O3_Rt': 3, 'Na2O_Rt': 1, 'K2O_Rt': 1, 'MnO_Rt': 1, 'TiO2_Rt': 2, 'Cr2O3_Rt': 3, 'P2O5_Rt': 5, 'ZrO2_Rt': 2}
-    oxygen_num_rt_df = pd.DataFrame.from_dict(oxygen_num_rt, orient='index').T
-    oxygen_num_rt_df['Sample_ID_Rt'] = 'OxNum'
-    oxygen_num_rt_df.set_index('Sample_ID_Rt', inplace=True)
+    oxygen_num_rt = {
+        "SiO2_Rt": 2,
+        "MgO_Rt": 1,
+        "FeOt_Rt": 1,
+        "CaO_Rt": 1,
+        "Al2O3_Rt": 3,
+        "Na2O_Rt": 1,
+        "K2O_Rt": 1,
+        "MnO_Rt": 1,
+        "TiO2_Rt": 2,
+        "Cr2O3_Rt": 3,
+        "P2O5_Rt": 5,
+        "ZrO2_Rt": 2,
+    }
+    oxygen_num_rt_df = pd.DataFrame.from_dict(oxygen_num_rt, orient="index").T
+    oxygen_num_rt_df["Sample_ID_Rt"] = "OxNum"
+    oxygen_num_rt_df.set_index("Sample_ID_Rt", inplace=True)
 
     mol_prop = calculate_mol_proportions_rutile(rt_comps=rt_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
-    ox_num_reindex = oxygen_num_rt_df.reindex(
-        mol_prop.columns, axis=1).fillna(0)
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
+    ox_num_reindex = oxygen_num_rt_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
     oxygens_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
+
 def calculate_2oxygens_rutile(rt_comps):
-    
     """
-    
+
     Import rutile compositions using rt_comps=My_Rts, returns cations on the basis of 4 oxygens.
 
     Parameters
     -------
     rt_comps: pandas.DataFrame
         rutile compositions with column headings SiO2_Rt, MgO_Rt etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 2 oxygens, with column headings of the form... Rt_cat_2ox.
 
     """
 
-    cation_num_rt = {'SiO2_Rt': 1, 'MgO_Rt': 1, 'FeOt_Rt': 1, 'CaO_Rt': 1, 'Al2O3_Rt': 2, 'Na2O_Rt': 2, 'K2O_Rt': 2, 'MnO_Rt': 1, 'TiO2_Rt': 1, 'Cr2O3_Rt': 2, 'P2O5_Rt': 2, 'ZrO2_Rt': 1}
-
-    cation_num_rt_df = pd.DataFrame.from_dict(cation_num_rt, orient='index').T
-    cation_num_rt_df['Sample_ID_Rt'] = 'CatNum'
-    cation_num_rt_df.set_index('Sample_ID_Rt', inplace=True)
+    cation_num_rt = {
+        "SiO2_Rt": 1,
+        "MgO_Rt": 1,
+        "FeOt_Rt": 1,
+        "CaO_Rt": 1,
+        "Al2O3_Rt": 2,
+        "Na2O_Rt": 2,
+        "K2O_Rt": 2,
+        "MnO_Rt": 1,
+        "TiO2_Rt": 1,
+        "Cr2O3_Rt": 2,
+        "P2O5_Rt": 2,
+        "ZrO2_Rt": 1,
+    }
+
+    cation_num_rt_df = pd.DataFrame.from_dict(cation_num_rt, orient="index").T
+    cation_num_rt_df["Sample_ID_Rt"] = "CatNum"
+    cation_num_rt_df.set_index("Sample_ID_Rt", inplace=True)
 
     oxygens = calculate_oxygens_rutile(rt_comps=rt_comps)
-    renorm_factor = 2 / (oxygens.sum(axis='columns'))
+    renorm_factor = 2 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_rutile(rt_comps=rt_comps)
-    mol_prop['oxy_renorm_factor_rt'] = renorm_factor
-    mol_prop_2 = mol_prop.multiply(mol_prop['oxy_renorm_factor_rt'], axis='rows')
-    mol_prop_2.columns = [str(col).replace('_mol_prop', '') for col in mol_prop_2.columns]
+    mol_prop["oxy_renorm_factor_rt"] = renorm_factor
+    mol_prop_2 = mol_prop.multiply(mol_prop["oxy_renorm_factor_rt"], axis="rows")
+    mol_prop_2.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_2.columns
+    ]
 
     ox_num_reindex = cation_num_rt_df.reindex(mol_prop_2.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_2])
-    cation_2 = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_2.columns = [str(col).replace('_mol_prop', '_cat_2ox') for col in mol_prop.columns]
+    cation_2 = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_2_2=cation_2.rename(columns={
-                            'SiO2_Rt_cat_2ox': 'Si_Rt_cat_2ox',
-                            'TiO2_Rt_cat_2ox': 'Ti_Rt_cat_2ox',
-                            'Al2O3_Rt_cat_2ox': 'Al_Rt_cat_2ox',
-                            'FeOt_Rt_cat_2ox': 'Fet_Rt_cat_2ox',
-                            'MnO_Rt_cat_2ox': 'Mn_Rt_cat_2ox',
-                            'MgO_Rt_cat_2ox': 'Mg_Rt_cat_2ox',
-                            'CaO_Rt_cat_2ox': 'Ca_Rt_cat_2ox',
-                            'Na2O_Rt_cat_2ox': 'Na_Rt_cat_2ox',
-                            'K2O_Rt_cat_2ox': 'K_Rt_cat_2ox',
-                            'Cr2O3_Rt_cat_2ox': 'Cr_Rt_cat_2ox',
-                            'P2O5_Rt_cat_2ox': 'P_Rt_cat_2ox',
-                            'ZrO2_Rt_cat_2ox': 'Zr_Rt_cat_2ox',})
+    cation_2.columns = [
+        str(col).replace("_mol_prop", "_cat_2ox") for col in mol_prop.columns
+    ]
+
+    cation_2_2 = cation_2.rename(
+        columns={
+            "SiO2_Rt_cat_2ox": "Si_Rt_cat_2ox",
+            "TiO2_Rt_cat_2ox": "Ti_Rt_cat_2ox",
+            "Al2O3_Rt_cat_2ox": "Al_Rt_cat_2ox",
+            "FeOt_Rt_cat_2ox": "Fet_Rt_cat_2ox",
+            "MnO_Rt_cat_2ox": "Mn_Rt_cat_2ox",
+            "MgO_Rt_cat_2ox": "Mg_Rt_cat_2ox",
+            "CaO_Rt_cat_2ox": "Ca_Rt_cat_2ox",
+            "Na2O_Rt_cat_2ox": "Na_Rt_cat_2ox",
+            "K2O_Rt_cat_2ox": "K_Rt_cat_2ox",
+            "Cr2O3_Rt_cat_2ox": "Cr_Rt_cat_2ox",
+            "P2O5_Rt_cat_2ox": "P_Rt_cat_2ox",
+            "ZrO2_Rt_cat_2ox": "Zr_Rt_cat_2ox",
+        }
+    )
 
     return cation_2_2
 
-def calculate_rutile_components(rt_comps, append):
 
+def calculate_rutile_components(rt_comps, append):
     """
-    
+
     Import rutile compositions using rt_comps=My_Rts, returns cations on the basis of 4 oxygens.
 
     Parameters
     -------
     rt_comps: pandas.DataFrame
         rutile compositions with column headings SiO2_Rt, MgO_Rt etc.
 
     Returns
     -------
     pandas DataFrame
         components on the basis of 2 oxygens, with column headings of the form... Rt_cat_2ox.
-    
+
     """
 
     rt_comps_new = rt_comps.copy()
-    rt_comps_new.columns = [col.replace(append, '_Rt') for col in rt_comps_new.columns]
+    rt_comps_new.columns = [col.replace(append, "_Rt") for col in rt_comps_new.columns]
     rt_comps = rt_comps_new.copy()
 
     rt_calc = calculate_2oxygens_rutile(rt_comps=rt_comps)
-    rt_calc['Rt_Cation_Sum'] = (rt_calc['Si_Rt_cat_2ox']+rt_calc['Ti_Rt_cat_2ox']+rt_calc['Al_Rt_cat_2ox']+rt_calc['Fet_Rt_cat_2ox']+rt_calc['Mn_Rt_cat_2ox']+rt_calc['Mg_Rt_cat_2ox']+rt_calc['Ca_Rt_cat_2ox']+rt_calc['Na_Rt_cat_2ox']+rt_calc['K_Rt_cat_2ox']+rt_calc['Cr_Rt_cat_2ox']+rt_calc['P_Rt_cat_2ox']+rt_calc['Zr_Rt_cat_2ox'])
+    rt_calc["Rt_Cation_Sum"] = (
+        rt_calc["Si_Rt_cat_2ox"]
+        + rt_calc["Ti_Rt_cat_2ox"]
+        + rt_calc["Al_Rt_cat_2ox"]
+        + rt_calc["Fet_Rt_cat_2ox"]
+        + rt_calc["Mn_Rt_cat_2ox"]
+        + rt_calc["Mg_Rt_cat_2ox"]
+        + rt_calc["Ca_Rt_cat_2ox"]
+        + rt_calc["Na_Rt_cat_2ox"]
+        + rt_calc["K_Rt_cat_2ox"]
+        + rt_calc["Cr_Rt_cat_2ox"]
+        + rt_calc["P_Rt_cat_2ox"]
+        + rt_calc["Zr_Rt_cat_2ox"]
+    )
 
-    rt_calc['Ti_Zr_Rt'] = rt_calc['Ti_Rt_cat_2ox'] + rt_calc['Zr_Rt_cat_2ox']
+    rt_calc["Ti_Zr_Rt"] = rt_calc["Ti_Rt_cat_2ox"] + rt_calc["Zr_Rt_cat_2ox"]
 
     cat_prop = calculate_cat_proportions_rutile(rt_comps=rt_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([rt_comps, rt_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-# %% TOURMALINE 
+# %% TOURMALINE
 
 
 def calculate_mol_proportions_tourmaline(trm_comps):
-
     """
     Import Muscovite compositions using trm_comps=My_Muscovites, returns mole proportions
-    
+
     Parameters
     -------
     trm_comps: pandas.DataFrame
             Panda DataFrame of tourmaline compositions with column headings SiO2_Trm, MgO_Trm etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for tourmalines with column headings of the form SiO2_Trm_mol_prop
 
     """
 
-    oxide_mass_trm = {'SiO2_Trm': 60.0843, 'MgO_Trm': 40.3044, 'FeOt_Trm': 71.8464, 'CaO_Trm': 56.0774,'Al2O3_Trm': 101.961, 'Na2O_Trm': 61.9789, 'K2O_Trm': 94.196, 'MnO_Trm': 70.9375, 'TiO2_Trm': 79.7877, 'Cr2O3_Trm': 151.9982, 'P2O5_Trm': 141.937}
-    oxide_mass_trm_df = pd.DataFrame.from_dict(oxide_mass_trm, orient='index').T
-    oxide_mass_trm_df['Sample_ID_Trm'] = 'MolWt'
-    oxide_mass_trm_df.set_index('Sample_ID_Trm', inplace=True)
+    oxide_mass_trm = {
+        "SiO2_Trm": 60.0843,
+        "MgO_Trm": 40.3044,
+        "FeOt_Trm": 71.8464,
+        "CaO_Trm": 56.0774,
+        "Al2O3_Trm": 101.961,
+        "Na2O_Trm": 61.9789,
+        "K2O_Trm": 94.196,
+        "MnO_Trm": 70.9375,
+        "TiO2_Trm": 79.7877,
+        "Cr2O3_Trm": 151.9982,
+        "P2O5_Trm": 141.937,
+    }
+    oxide_mass_trm_df = pd.DataFrame.from_dict(oxide_mass_trm, orient="index").T
+    oxide_mass_trm_df["Sample_ID_Trm"] = "MolWt"
+    oxide_mass_trm_df.set_index("Sample_ID_Trm", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     trm_wt = trm_comps.reindex(oxide_mass_trm_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    trm_wt_combo = pd.concat([oxide_mass_trm_df, trm_wt],)
+    trm_wt_combo = pd.concat(
+        [oxide_mass_trm_df, trm_wt],
+    )
     # Drop the calculation column
     mol_prop_anhyd = trm_wt_combo.div(
-        trm_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+        trm_wt_combo.loc["MolWt", :], axis="columns"
+    ).drop(["MolWt"])
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
-def calculate_cat_proportions_tourmaline(*, trm_comps=None, oxide_headers=False):
 
+def calculate_cat_proportions_tourmaline(*, trm_comps=None, oxide_headers=False):
     """
-    
+
     Import tourmaline compositions using trm_comps=My_tourmalines, returns cation proportions
 
     Parameters
     -------
     trm_comps: pandas.DataFrame
             tourmaline compositions with column headings SiO2_Trm, MgO_Trm etc.
     oxide_headers: bool
@@ -4485,183 +6401,279 @@
     Returns
     -------
     pandas DataFrame
         cation proportions for tourmaline with column headings of the form... Trm_cat_prop
 
     """
 
-    cation_num_trm = {'SiO2_Trm': 1, 'MgO_Trm': 1, 'FeOt_Trm': 1, 'CaO_Trm': 1, 'Al2O3_Trm': 2, 'Na2O_Trm': 2, 'K2O_Trm': 2, 'MnO_Trm': 1, 'TiO2_Trm': 1, 'Cr2O3_Trm': 2, 'P2O5_Trm': 2}
-    cation_num_trm_df = pd.DataFrame.from_dict(cation_num_trm, orient='index').T
-    cation_num_trm_df['Sample_ID_Trm'] = 'CatNum'
-    cation_num_trm_df.set_index('Sample_ID_Trm', inplace=True)
-
-    oxide_mass_trm = {'SiO2_Trm': 60.0843, 'MgO_Trm': 40.3044, 'FeOt_Trm': 71.8464, 'CaO_Trm': 56.0774,'Al2O3_Trm': 101.961, 'Na2O_Trm': 61.9789, 'K2O_Trm': 94.196, 'MnO_Trm': 70.9375, 'TiO2_Trm': 79.7877, 'Cr2O3_Trm': 151.9982, 'P2O5_Trm': 141.937}
-
-    oxide_mass_trm_df = pd.DataFrame.from_dict(oxide_mass_trm, orient='index').T
-    oxide_mass_trm_df['Sample_ID_Trm'] = 'MolWt'
-    oxide_mass_trm_df.set_index('Sample_ID_Trm', inplace=True)
+    cation_num_trm = {
+        "SiO2_Trm": 1,
+        "MgO_Trm": 1,
+        "FeOt_Trm": 1,
+        "CaO_Trm": 1,
+        "Al2O3_Trm": 2,
+        "Na2O_Trm": 2,
+        "K2O_Trm": 2,
+        "MnO_Trm": 1,
+        "TiO2_Trm": 1,
+        "Cr2O3_Trm": 2,
+        "P2O5_Trm": 2,
+    }
+    cation_num_trm_df = pd.DataFrame.from_dict(cation_num_trm, orient="index").T
+    cation_num_trm_df["Sample_ID_Trm"] = "CatNum"
+    cation_num_trm_df.set_index("Sample_ID_Trm", inplace=True)
+
+    oxide_mass_trm = {
+        "SiO2_Trm": 60.0843,
+        "MgO_Trm": 40.3044,
+        "FeOt_Trm": 71.8464,
+        "CaO_Trm": 56.0774,
+        "Al2O3_Trm": 101.961,
+        "Na2O_Trm": 61.9789,
+        "K2O_Trm": 94.196,
+        "MnO_Trm": 70.9375,
+        "TiO2_Trm": 79.7877,
+        "Cr2O3_Trm": 151.9982,
+        "P2O5_Trm": 141.937,
+    }
+
+    oxide_mass_trm_df = pd.DataFrame.from_dict(oxide_mass_trm, orient="index").T
+    oxide_mass_trm_df["Sample_ID_Trm"] = "MolWt"
+    oxide_mass_trm_df.set_index("Sample_ID_Trm", inplace=True)
 
     trm_prop_no_cat_num = calculate_mol_proportions_tourmaline(trm_comps=trm_comps)
-    trm_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in trm_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_trm_df.reindex(oxide_mass_trm_df.columns, axis=1).fillna(0)
+    trm_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in trm_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_trm_df.reindex(
+        oxide_mass_trm_df.columns, axis=1
+    ).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, trm_prop_no_cat_num])
-    cation_prop_anhyd = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
-    
+    cation_prop_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
+
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Trm_cat_prop': 'Si_Trm_cat_prop',
-                            'TiO2_Trm_cat_prop': 'Ti_Trm_cat_prop',
-                            'Al2O3_Trm_cat_prop': 'Al_Trm_cat_prop',
-                            'FeOt_Trm_cat_prop': 'Fet_Trm_cat_prop',
-                            'MnO_Trm_cat_prop': 'Mn_Trm_cat_prop',
-                            'MgO_Trm_cat_prop': 'Mg_Trm_cat_prop',
-                            'CaO_Trm_cat_prop': 'Ca_Trm_cat_prop',
-                            'Na2O_Trm_cat_prop': 'Na_Trm_cat_prop',
-                            'K2O_Trm_cat_prop': 'K_Trm_cat_prop',
-                            'Cr2O3_Trm_cat_prop': 'Cr_Trm_cat_prop',
-                            'P2O5_Trm_cat_prop': 'P_Trm_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Trm_cat_prop": "Si_Trm_cat_prop",
+                "TiO2_Trm_cat_prop": "Ti_Trm_cat_prop",
+                "Al2O3_Trm_cat_prop": "Al_Trm_cat_prop",
+                "FeOt_Trm_cat_prop": "Fet_Trm_cat_prop",
+                "MnO_Trm_cat_prop": "Mn_Trm_cat_prop",
+                "MgO_Trm_cat_prop": "Mg_Trm_cat_prop",
+                "CaO_Trm_cat_prop": "Ca_Trm_cat_prop",
+                "Na2O_Trm_cat_prop": "Na_Trm_cat_prop",
+                "K2O_Trm_cat_prop": "K_Trm_cat_prop",
+                "Cr2O3_Trm_cat_prop": "Cr_Trm_cat_prop",
+                "P2O5_Trm_cat_prop": "P_Trm_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
+
 def calculate_oxygens_tourmaline(trm_comps):
-    
     """
-    
+
     Import tourmaline compositions using trm_comps=My_Trms, returns number of oxygens (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     trm_comps: pandas.DataFrame
         tourmaline compositions with column headings SiO2_Trm, MgO_Trm etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Trm_ox
 
     """
 
-    oxygen_num_trm = {'SiO2_Trm': 2, 'MgO_Trm': 1, 'FeOt_Trm': 1, 'CaO_Trm': 1, 'Al2O3_Trm': 3, 'Na2O_Trm': 1, 'K2O_Trm': 1, 'MnO_Trm': 1, 'TiO2_Trm': 2, 'Cr2O3_Trm': 3, 'P2O5_Trm': 5}
-    oxygen_num_trm_df = pd.DataFrame.from_dict(oxygen_num_trm, orient='index').T
-    oxygen_num_trm_df['Sample_ID_Trm'] = 'OxNum'
-    oxygen_num_trm_df.set_index('Sample_ID_Trm', inplace=True)
+    oxygen_num_trm = {
+        "SiO2_Trm": 2,
+        "MgO_Trm": 1,
+        "FeOt_Trm": 1,
+        "CaO_Trm": 1,
+        "Al2O3_Trm": 3,
+        "Na2O_Trm": 1,
+        "K2O_Trm": 1,
+        "MnO_Trm": 1,
+        "TiO2_Trm": 2,
+        "Cr2O3_Trm": 3,
+        "P2O5_Trm": 5,
+    }
+    oxygen_num_trm_df = pd.DataFrame.from_dict(oxygen_num_trm, orient="index").T
+    oxygen_num_trm_df["Sample_ID_Trm"] = "OxNum"
+    oxygen_num_trm_df.set_index("Sample_ID_Trm", inplace=True)
 
     mol_prop = calculate_mol_proportions_tourmaline(trm_comps=trm_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '') for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_trm_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
+
 def calculate_18oxygens_tourmaline(trm_comps):
-    
     """
-    
+
     Import tourmaline compositions using trm_comps=My_Trms, returns cations on the basis of 10 oxygens.
-    
+
     Parameters
     -------
     trm_comps: pandas.DataFrame
         tourmaline compositions with column headings SiO2_Trm, MgO_Trm etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 10 oxygens, with column headings of the form... Trm_cat_18ox.
 
     """
 
-    cation_num_trm = {'SiO2_Trm': 1, 'MgO_Trm': 1, 'FeOt_Trm': 1, 'CaO_Trm': 1, 'Al2O3_Trm': 2, 'Na2O_Trm': 2, 'K2O_Trm': 2, 'MnO_Trm': 1, 'TiO2_Trm': 1, 'Cr2O3_Trm': 2, 'P2O5_Trm': 2}
-
-    cation_num_trm_df = pd.DataFrame.from_dict(cation_num_trm, orient='index').T
-    cation_num_trm_df['Sample_ID_Trm'] = 'CatNum'
-    cation_num_trm_df.set_index('Sample_ID_Trm', inplace=True)
+    cation_num_trm = {
+        "SiO2_Trm": 1,
+        "MgO_Trm": 1,
+        "FeOt_Trm": 1,
+        "CaO_Trm": 1,
+        "Al2O3_Trm": 2,
+        "Na2O_Trm": 2,
+        "K2O_Trm": 2,
+        "MnO_Trm": 1,
+        "TiO2_Trm": 1,
+        "Cr2O3_Trm": 2,
+        "P2O5_Trm": 2,
+    }
+
+    cation_num_trm_df = pd.DataFrame.from_dict(cation_num_trm, orient="index").T
+    cation_num_trm_df["Sample_ID_Trm"] = "CatNum"
+    cation_num_trm_df.set_index("Sample_ID_Trm", inplace=True)
 
     oxygens = calculate_oxygens_tourmaline(trm_comps=trm_comps)
-    renorm_factor = 10 / (oxygens.sum(axis='columns'))
+    renorm_factor = 10 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_tourmaline(trm_comps=trm_comps)
-    mol_prop['oxy_renorm_factor_trm'] = renorm_factor
-    mol_prop_10 = mol_prop.multiply(mol_prop['oxy_renorm_factor_trm'], axis='rows')
-    mol_prop_10.columns = [str(col).replace('_mol_prop', '') for col in mol_prop_10.columns]
+    mol_prop["oxy_renorm_factor_trm"] = renorm_factor
+    mol_prop_10 = mol_prop.multiply(mol_prop["oxy_renorm_factor_trm"], axis="rows")
+    mol_prop_10.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_10.columns
+    ]
 
     ox_num_reindex = cation_num_trm_df.reindex(mol_prop_10.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_10])
-    cation_10 = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_10.columns = [str(col).replace('_mol_prop', '_cat_18ox') for col in mol_prop.columns]
-
-    cation_10_2=cation_10.rename(columns={
-                            'SiO2_Trm_cat_18ox': 'Si_Trm_cat_18ox',
-                            'TiO2_Trm_cat_18ox': 'Ti_Trm_cat_18ox',
-                            'Al2O3_Trm_cat_18ox': 'Al_Trm_cat_18ox',
-                            'FeOt_Trm_cat_18ox': 'Fet_Trm_cat_18ox',
-                            'MnO_Trm_cat_18ox': 'Mn_Trm_cat_18ox',
-                            'MgO_Trm_cat_18ox': 'Mg_Trm_cat_18ox',
-                            'CaO_Trm_cat_18ox': 'Ca_Trm_cat_18ox',
-                            'Na2O_Trm_cat_18ox': 'Na_Trm_cat_18ox',
-                            'K2O_Trm_cat_18ox': 'K_Trm_cat_18ox',
-                            'Cr2O3_Trm_cat_18ox': 'Cr_Trm_cat_18ox',
-                            'P2O5_Trm_cat_18ox': 'P_Trm_cat_18ox',})
+    cation_10 = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+
+    cation_10.columns = [
+        str(col).replace("_mol_prop", "_cat_18ox") for col in mol_prop.columns
+    ]
+
+    cation_10_2 = cation_10.rename(
+        columns={
+            "SiO2_Trm_cat_18ox": "Si_Trm_cat_18ox",
+            "TiO2_Trm_cat_18ox": "Ti_Trm_cat_18ox",
+            "Al2O3_Trm_cat_18ox": "Al_Trm_cat_18ox",
+            "FeOt_Trm_cat_18ox": "Fet_Trm_cat_18ox",
+            "MnO_Trm_cat_18ox": "Mn_Trm_cat_18ox",
+            "MgO_Trm_cat_18ox": "Mg_Trm_cat_18ox",
+            "CaO_Trm_cat_18ox": "Ca_Trm_cat_18ox",
+            "Na2O_Trm_cat_18ox": "Na_Trm_cat_18ox",
+            "K2O_Trm_cat_18ox": "K_Trm_cat_18ox",
+            "Cr2O3_Trm_cat_18ox": "Cr_Trm_cat_18ox",
+            "P2O5_Trm_cat_18ox": "P_Trm_cat_18ox",
+        }
+    )
 
     return cation_10_2
 
 
 def calculate_tourmaline_components(trm_comps, append):
-    
     """
-    
+
     Import Muscovite compositions using trm_comps=My_Muscovites, returns mole proportions
-    
+
     Parameters
     -------
     trm_comps: pandas.DataFrame
             Panda DataFrame of tourmaline compositions with column headings SiO2_Trm, MgO_Trm etc.
-    
+
     Returns
     -------
     pandas DataFrame
         components for tourmalines with column headings of the form SiO2_Trm_mol_prop
 
     """
 
     trm_comps_new = trm_comps.copy()
-    trm_comps_new.columns = [col.replace(append, '_Trm') for col in trm_comps_new.columns]
+    trm_comps_new.columns = [
+        col.replace(append, "_Trm") for col in trm_comps_new.columns
+    ]
     trm_comps = trm_comps_new.copy()
 
     trm_calc = calculate_18oxygens_tourmaline(trm_comps=trm_comps)
-    trm_calc['Trm_Cation_Sum'] = (trm_calc['Si_Trm_cat_18ox']+trm_calc['Ti_Trm_cat_18ox']+trm_calc['Al_Trm_cat_18ox']+trm_calc['Fet_Trm_cat_18ox']+trm_calc['Mn_Trm_cat_18ox']+trm_calc['Mg_Trm_cat_18ox']+trm_calc['Ca_Trm_cat_18ox']+trm_calc['Na_Trm_cat_18ox']+trm_calc['K_Trm_cat_18ox']+trm_calc['Cr_Trm_cat_18ox']+trm_calc['P_Trm_cat_18ox'])
-
-    trm_calc['Na_Ca_K_X_Trm'] = trm_calc['Na_Trm_cat_18ox'] + trm_calc['Ca_Trm_cat_18ox'] + trm_calc['K_Trm_cat_18ox'] 
-    trm_calc['Mg_Fe_Mn_Al_Y_Trm'] = trm_calc['Mg_Trm_cat_18ox'] + trm_calc['Fet_Trm_cat_18ox'] + trm_calc['Mn_Trm_cat_18ox'] + trm_calc['Al_Trm_cat_18ox'] 
-    trm_calc['Mg_Fe_Al_Z_Trm'] = trm_calc['Mg_Trm_cat_18ox'] + trm_calc['Fet_Trm_cat_18ox'] + trm_calc['Al_Trm_cat_18ox'] 
+    trm_calc["Trm_Cation_Sum"] = (
+        trm_calc["Si_Trm_cat_18ox"]
+        + trm_calc["Ti_Trm_cat_18ox"]
+        + trm_calc["Al_Trm_cat_18ox"]
+        + trm_calc["Fet_Trm_cat_18ox"]
+        + trm_calc["Mn_Trm_cat_18ox"]
+        + trm_calc["Mg_Trm_cat_18ox"]
+        + trm_calc["Ca_Trm_cat_18ox"]
+        + trm_calc["Na_Trm_cat_18ox"]
+        + trm_calc["K_Trm_cat_18ox"]
+        + trm_calc["Cr_Trm_cat_18ox"]
+        + trm_calc["P_Trm_cat_18ox"]
+    )
+
+    trm_calc["Na_Ca_K_X_Trm"] = (
+        trm_calc["Na_Trm_cat_18ox"]
+        + trm_calc["Ca_Trm_cat_18ox"]
+        + trm_calc["K_Trm_cat_18ox"]
+    )
+    trm_calc["Mg_Fe_Mn_Al_Y_Trm"] = (
+        trm_calc["Mg_Trm_cat_18ox"]
+        + trm_calc["Fet_Trm_cat_18ox"]
+        + trm_calc["Mn_Trm_cat_18ox"]
+        + trm_calc["Al_Trm_cat_18ox"]
+    )
+    trm_calc["Mg_Fe_Al_Z_Trm"] = (
+        trm_calc["Mg_Trm_cat_18ox"]
+        + trm_calc["Fet_Trm_cat_18ox"]
+        + trm_calc["Al_Trm_cat_18ox"]
+    )
 
     cat_prop = calculate_cat_proportions_tourmaline(trm_comps=trm_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac') for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([trm_comps, trm_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-
 # %% OXIDES - MAGNETITE-ILMENITE
 
 
 def calculate_mol_proportions_oxide(ox_comps):
-
     """
-    
-    Import Oxide compositions using ox_comps=My_Oxides, returns mole proportions. 
+
+    Import Oxide compositions using ox_comps=My_Oxides, returns mole proportions.
     Retain _Ox appendix
 
     Parameters
     -------
     ox_comps: pandas.DataFrame
             Panda DataFrame of oxide compositions with column headings SiO2_Ox, MgO_Ox etc.
 
@@ -4669,298 +6681,430 @@
     -------
     pandas DataFrame
         mole proportions for oxides with column headings of the form SiO2_Ox_mol_prop
 
 
     """
 
-    oxide_mass_ox = {'SiO2_Ox': 60.0843, 'MgO_Ox': 40.3044, 'FeOt_Ox': 71.8464, 'CaO_Ox': 56.0774,'Al2O3_Ox': 101.961, 'Na2O_Ox': 61.9789, 'K2O_Ox': 94.196, 'MnO_Ox': 70.9375, 'TiO2_Ox': 79.7877, 'Cr2O3_Ox': 151.9982, 'P2O5_Ox': 141.937}
-
-    oxide_mass_ox_df = pd.DataFrame.from_dict(oxide_mass_ox, orient='index').T
-    oxide_mass_ox_df['Sample_ID_Ox'] = 'MolWt'
-    oxide_mass_ox_df.set_index('Sample_ID_Ox', inplace=True)
+    oxide_mass_ox = {
+        "SiO2_Ox": 60.0843,
+        "MgO_Ox": 40.3044,
+        "FeOt_Ox": 71.8464,
+        "CaO_Ox": 56.0774,
+        "Al2O3_Ox": 101.961,
+        "Na2O_Ox": 61.9789,
+        "K2O_Ox": 94.196,
+        "MnO_Ox": 70.9375,
+        "TiO2_Ox": 79.7877,
+        "Cr2O3_Ox": 151.9982,
+        "P2O5_Ox": 141.937,
+    }
+
+    oxide_mass_ox_df = pd.DataFrame.from_dict(oxide_mass_ox, orient="index").T
+    oxide_mass_ox_df["Sample_ID_Ox"] = "MolWt"
+    oxide_mass_ox_df.set_index("Sample_ID_Ox", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     ox_wt = ox_comps.reindex(oxide_mass_ox_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    ox_wt_combo = pd.concat([oxide_mass_ox_df, ox_wt],)
+    ox_wt_combo = pd.concat(
+        [oxide_mass_ox_df, ox_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = ox_wt_combo.div(ox_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
-    
+    mol_prop_anhyd = ox_wt_combo.div(ox_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
+
     return mol_prop_anhyd
 
 
 def calculate_cat_proportions_oxide(*, ox_comps=None, oxide_headers=False):
-
     """
-    
+
     Import oxide compositions using ox_comps=My_oxides, returns cation proportions
     Retain _Ox appendix
 
     Parameters
     -------
     ox_comps: pandas.DataFrame
             oxide compositions with column headings SiO2_Ox, MgO_Ox etc.
 
     oxide_headers: bool
         default=False, returns as Ti_Ox_cat_prop.
         =True returns Ti_Ox_cat_prop.
         This is used for rapid matrix division for
         pre-processing of data for cation fractions etc
-    
+
     Returns
     -------
     pandas DataFrame
         cation proportions for oxide with column headings of the form... Sp_cat_prop
 
     """
 
-    cation_num_ox = {'SiO2_Ox': 1, 'MgO_Ox': 1, 'FeOt_Ox': 1, 'CaO_Ox': 1, 'Al2O3_Ox': 2, 'Na2O_Ox': 2, 'K2O_Ox': 2, 'MnO_Ox': 1, 'TiO2_Ox': 1, 'Cr2O3_Ox': 2, 'P2O5_Ox': 2}
-    cation_num_ox_df = pd.DataFrame.from_dict(cation_num_ox, orient='index').T
-    cation_num_ox_df['Sample_ID_Ox'] = 'CatNum'
-    cation_num_ox_df.set_index('Sample_ID_Ox', inplace=True)
-
-    oxide_mass_ox = {'SiO2_Ox': 60.0843, 'MgO_Ox': 40.3044, 'FeOt_Ox': 71.8464, 'CaO_Ox': 56.0774,'Al2O3_Ox': 101.961, 'Na2O_Ox': 61.9789, 'K2O_Ox': 94.196, 'MnO_Ox': 70.9375, 'TiO2_Ox': 79.7877, 'Cr2O3_Ox': 151.9982, 'P2O5_Ox': 141.937}
-    oxide_mass_ox_df = pd.DataFrame.from_dict(oxide_mass_ox, orient='index').T
-    oxide_mass_ox_df['Sample_ID_Ox'] = 'MolWt'
-    oxide_mass_ox_df.set_index('Sample_ID_Ox', inplace=True)
+    cation_num_ox = {
+        "SiO2_Ox": 1,
+        "MgO_Ox": 1,
+        "FeOt_Ox": 1,
+        "CaO_Ox": 1,
+        "Al2O3_Ox": 2,
+        "Na2O_Ox": 2,
+        "K2O_Ox": 2,
+        "MnO_Ox": 1,
+        "TiO2_Ox": 1,
+        "Cr2O3_Ox": 2,
+        "P2O5_Ox": 2,
+    }
+    cation_num_ox_df = pd.DataFrame.from_dict(cation_num_ox, orient="index").T
+    cation_num_ox_df["Sample_ID_Ox"] = "CatNum"
+    cation_num_ox_df.set_index("Sample_ID_Ox", inplace=True)
+
+    oxide_mass_ox = {
+        "SiO2_Ox": 60.0843,
+        "MgO_Ox": 40.3044,
+        "FeOt_Ox": 71.8464,
+        "CaO_Ox": 56.0774,
+        "Al2O3_Ox": 101.961,
+        "Na2O_Ox": 61.9789,
+        "K2O_Ox": 94.196,
+        "MnO_Ox": 70.9375,
+        "TiO2_Ox": 79.7877,
+        "Cr2O3_Ox": 151.9982,
+        "P2O5_Ox": 141.937,
+    }
+    oxide_mass_ox_df = pd.DataFrame.from_dict(oxide_mass_ox, orient="index").T
+    oxide_mass_ox_df["Sample_ID_Ox"] = "MolWt"
+    oxide_mass_ox_df.set_index("Sample_ID_Ox", inplace=True)
 
     ox_prop_no_cat_num = calculate_mol_proportions_oxide(ox_comps=ox_comps)
-    ox_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in ox_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_ox_df.reindex(oxide_mass_ox_df.columns, axis=1).fillna(0)
+    ox_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in ox_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_ox_df.reindex(oxide_mass_ox_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, ox_prop_no_cat_num])
-    cation_prop_anhyd = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-    cation_prop_anhyd.columns = [str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
-    
+    cation_prop_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+    cation_prop_anhyd.columns = [
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
+
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Ox_cat_prop': 'Si_Ox_cat_prop',
-                            'TiO2_Ox_cat_prop': 'Ti_Ox_cat_prop',
-                            'Al2O3_Ox_cat_prop': 'Al_Ox_cat_prop',
-                            'FeOt_Ox_cat_prop': 'Fet_Ox_cat_prop',
-                            'MnO_Ox_cat_prop': 'Mn_Ox_cat_prop',
-                            'MgO_Ox_cat_prop': 'Mg_Ox_cat_prop',
-                            'CaO_Ox_cat_prop': 'Ca_Ox_cat_prop',
-                            'Na2O_Ox_cat_prop': 'Na_Ox_cat_prop',
-                            'K2O_Ox_cat_prop': 'K_Ox_cat_prop',
-                            'Cr2O3_Ox_cat_prop': 'Cr_Ox_cat_prop',
-                            'P2O5_Ox_cat_prop': 'P_Ox_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Ox_cat_prop": "Si_Ox_cat_prop",
+                "TiO2_Ox_cat_prop": "Ti_Ox_cat_prop",
+                "Al2O3_Ox_cat_prop": "Al_Ox_cat_prop",
+                "FeOt_Ox_cat_prop": "Fet_Ox_cat_prop",
+                "MnO_Ox_cat_prop": "Mn_Ox_cat_prop",
+                "MgO_Ox_cat_prop": "Mg_Ox_cat_prop",
+                "CaO_Ox_cat_prop": "Ca_Ox_cat_prop",
+                "Na2O_Ox_cat_prop": "Na_Ox_cat_prop",
+                "K2O_Ox_cat_prop": "K_Ox_cat_prop",
+                "Cr2O3_Ox_cat_prop": "Cr_Ox_cat_prop",
+                "P2O5_Ox_cat_prop": "P_Ox_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
-def calculate_oxygens_oxide(ox_comps):
 
+def calculate_oxygens_oxide(ox_comps):
     """
-    
-    Import oxide compositions using ox_comps=My_Oxs, returns number of oxygens 
+
+    Import oxide compositions using ox_comps=My_Oxs, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit). Retain _Ox appendix
 
     Parameters
     -------
     ox_comps: pandas.DataFrame
         oxide compositions with column headings SiO2_Ox, MgO_Ox etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Ox
 
     """
 
-    oxygen_num_ox = {'SiO2_Ox': 2, 'MgO_Ox': 1, 'FeOt_Ox': 1, 'CaO_Ox': 1, 'Al2O3_Ox': 3, 'Na2O_Ox': 1,'K2O_Ox': 1, 'MnO_Ox': 1, 'TiO2_Ox': 2, 'Cr2O3_Ox': 3, 'P2O5_Ox': 5}
-    oxygen_num_ox_df = pd.DataFrame.from_dict(oxygen_num_ox, orient='index').T
-    oxygen_num_ox_df['Sample_ID_Ox'] = 'OxNum'
-    oxygen_num_ox_df.set_index('Sample_ID_Ox', inplace=True)
+    oxygen_num_ox = {
+        "SiO2_Ox": 2,
+        "MgO_Ox": 1,
+        "FeOt_Ox": 1,
+        "CaO_Ox": 1,
+        "Al2O3_Ox": 3,
+        "Na2O_Ox": 1,
+        "K2O_Ox": 1,
+        "MnO_Ox": 1,
+        "TiO2_Ox": 2,
+        "Cr2O3_Ox": 3,
+        "P2O5_Ox": 5,
+    }
+    oxygen_num_ox_df = pd.DataFrame.from_dict(oxygen_num_ox, orient="index").T
+    oxygen_num_ox_df["Sample_ID_Ox"] = "OxNum"
+    oxygen_num_ox_df.set_index("Sample_ID_Ox", inplace=True)
 
     mol_prop = calculate_mol_proportions_oxide(ox_comps=ox_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '') for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_ox_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
-def calculate_oxygens_oxide(ox_comps):
 
+def calculate_oxygens_oxide(ox_comps):
     """
-    
-    Import oxide compositions using ox_comps=My_Oxs, returns number of oxygens 
+
+    Import oxide compositions using ox_comps=My_Oxs, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit). Retain _Ox appendix
 
     Parameters
     -------
     ox_comps: pandas.DataFrame
         oxide compositions with column headings SiO2_Ox, MgO_Ox etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Ox
 
     """
 
-    oxygen_num_ox = {'SiO2_Ox': 2, 'MgO_Ox': 1, 'FeOt_Ox': 1, 'CaO_Ox': 1, 'Al2O3_Ox': 3, 'Na2O_Ox': 1,'K2O_Ox': 1, 'MnO_Ox': 1, 'TiO2_Ox': 2, 'Cr2O3_Ox': 3, 'P2O5_Ox': 5}
-    oxygen_num_ox_df = pd.DataFrame.from_dict(oxygen_num_ox, orient='index').T
-    oxygen_num_ox_df['Sample_ID_Ox'] = 'OxNum'
-    oxygen_num_ox_df.set_index('Sample_ID_Ox', inplace=True)
+    oxygen_num_ox = {
+        "SiO2_Ox": 2,
+        "MgO_Ox": 1,
+        "FeOt_Ox": 1,
+        "CaO_Ox": 1,
+        "Al2O3_Ox": 3,
+        "Na2O_Ox": 1,
+        "K2O_Ox": 1,
+        "MnO_Ox": 1,
+        "TiO2_Ox": 2,
+        "Cr2O3_Ox": 3,
+        "P2O5_Ox": 5,
+    }
+    oxygen_num_ox_df = pd.DataFrame.from_dict(oxygen_num_ox, orient="index").T
+    oxygen_num_ox_df["Sample_ID_Ox"] = "OxNum"
+    oxygen_num_ox_df.set_index("Sample_ID_Ox", inplace=True)
 
     mol_prop = calculate_mol_proportions_oxide(ox_comps=ox_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '') for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_ox_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
-def calculate_3oxygens_oxide(ox_comps):
 
+def calculate_3oxygens_oxide(ox_comps):
     """
-    
+
     Import oxide compositions using ox_comps=My_Oxs, returns cations on the basis of 4 oxygens.
     Retain _Ox appendix
 
     Parameters
     -------
     ox_comps: pandas.DataFrame
         oxide compositions with column headings SiO2_Ox, MgO_Ox etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 3 oxygens, with column headings of the form... Sp_cat_3ox.
-        
+
     """
 
-    cation_num_ox = {'SiO2_Ox': 1, 'MgO_Ox': 1, 'FeOt_Ox': 1, 'CaO_Ox': 1, 'Al2O3_Ox': 2, 'Na2O_Ox': 2,'K2O_Ox': 2, 'MnO_Ox': 1, 'TiO2_Ox': 1, 'Cr2O3_Ox': 2, 'P2O5_Ox': 2}
-    cation_num_ox_df = pd.DataFrame.from_dict(cation_num_ox, orient='index').T
-    cation_num_ox_df['Sample_ID_Ox'] = 'CatNum'
-    cation_num_ox_df.set_index('Sample_ID_Ox', inplace=True)
+    cation_num_ox = {
+        "SiO2_Ox": 1,
+        "MgO_Ox": 1,
+        "FeOt_Ox": 1,
+        "CaO_Ox": 1,
+        "Al2O3_Ox": 2,
+        "Na2O_Ox": 2,
+        "K2O_Ox": 2,
+        "MnO_Ox": 1,
+        "TiO2_Ox": 1,
+        "Cr2O3_Ox": 2,
+        "P2O5_Ox": 2,
+    }
+    cation_num_ox_df = pd.DataFrame.from_dict(cation_num_ox, orient="index").T
+    cation_num_ox_df["Sample_ID_Ox"] = "CatNum"
+    cation_num_ox_df.set_index("Sample_ID_Ox", inplace=True)
 
     oxygens = calculate_oxygens_oxide(ox_comps=ox_comps)
-    renorm_factor = 3 / (oxygens.sum(axis='columns'))
+    renorm_factor = 3 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_oxide(ox_comps=ox_comps)
-    mol_prop['oxy_renorm_factor_ox'] = renorm_factor
-    mol_prop_3 = mol_prop.multiply(mol_prop['oxy_renorm_factor_ox'], axis='rows')
-    mol_prop_3.columns = [str(col).replace('_mol_prop', '') for col in mol_prop_3.columns]
+    mol_prop["oxy_renorm_factor_ox"] = renorm_factor
+    mol_prop_3 = mol_prop.multiply(mol_prop["oxy_renorm_factor_ox"], axis="rows")
+    mol_prop_3.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_3.columns
+    ]
 
     ox_num_reindex = cation_num_ox_df.reindex(mol_prop_3.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_3])
-    cation_3 = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_3.columns = [str(col).replace('_mol_prop', '_cat_3ox') for col in mol_prop.columns]
-
-    cation_3_2=cation_3.rename(columns={
-                            'SiO2_Ox_cat_3ox': 'Si_Ox_cat_3ox',
-                            'TiO2_Ox_cat_3ox': 'Ti_Ox_cat_3ox',
-                            'Al2O3_Ox_cat_3ox': 'Al_Ox_cat_3ox',
-                            'FeOt_Ox_cat_3ox': 'Fet_Ox_cat_3ox',
-                            'MnO_Ox_cat_3ox': 'Mn_Ox_cat_3ox',
-                            'MgO_Ox_cat_3ox': 'Mg_Ox_cat_3ox',
-                            'CaO_Ox_cat_3ox': 'Ca_Ox_cat_3ox',
-                            'Na2O_Ox_cat_3ox': 'Na_Ox_cat_3ox',
-                            'K2O_Ox_cat_3ox': 'K_Ox_cat_3ox',
-                            'Cr2O3_Ox_cat_3ox': 'Cr_Ox_cat_3ox',
-                            'P2O5_Ox_cat_3ox': 'P_Ox_cat_3ox',})
+    cation_3 = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
+
+    cation_3.columns = [
+        str(col).replace("_mol_prop", "_cat_3ox") for col in mol_prop.columns
+    ]
+
+    cation_3_2 = cation_3.rename(
+        columns={
+            "SiO2_Ox_cat_3ox": "Si_Ox_cat_3ox",
+            "TiO2_Ox_cat_3ox": "Ti_Ox_cat_3ox",
+            "Al2O3_Ox_cat_3ox": "Al_Ox_cat_3ox",
+            "FeOt_Ox_cat_3ox": "Fet_Ox_cat_3ox",
+            "MnO_Ox_cat_3ox": "Mn_Ox_cat_3ox",
+            "MgO_Ox_cat_3ox": "Mg_Ox_cat_3ox",
+            "CaO_Ox_cat_3ox": "Ca_Ox_cat_3ox",
+            "Na2O_Ox_cat_3ox": "Na_Ox_cat_3ox",
+            "K2O_Ox_cat_3ox": "K_Ox_cat_3ox",
+            "Cr2O3_Ox_cat_3ox": "Cr_Ox_cat_3ox",
+            "P2O5_Ox_cat_3ox": "P_Ox_cat_3ox",
+        }
+    )
 
     return cation_3_2
 
-def calculate_oxide_components(ox_comps, append):
 
+def calculate_oxide_components(ox_comps, append):
     """
-    
+
     Import oxide compositions using ox_comps=My_Oxs, returns cations on the basis of 4 oxygens.
     Retain _Ox appendix
 
     Parameters
     -------
     ox_comps: pandas.DataFrame
         oxide compositions with column headings SiO2_Ox, MgO_Ox etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 3 oxygens, with column headings of the form... Sp_cat_3ox.
 
     """
-    
+
     ox_comps_new = ox_comps.copy()
-    ox_comps_new.columns = [col.replace(append, '_Ox') for col in ox_comps_new.columns]
+    ox_comps_new.columns = [col.replace(append, "_Ox") for col in ox_comps_new.columns]
     ox_comps = ox_comps_new.copy()
 
     ox_calc = calculate_3oxygens_oxide(ox_comps=ox_comps)
-    ox_calc['Ox_Cation_Sum'] = (ox_calc['Si_Ox_cat_3ox']+ox_calc['Ti_Ox_cat_3ox']+ox_calc['Al_Ox_cat_3ox']+ox_calc['Fet_Ox_cat_3ox']+ox_calc['Mn_Ox_cat_3ox']+ox_calc['Mg_Ox_cat_3ox']+ox_calc['Ca_Ox_cat_3ox']+ox_calc['Na_Ox_cat_3ox']+ox_calc['K_Ox_cat_3ox']+ox_calc['Cr_Ox_cat_3ox']+ox_calc['P_Ox_cat_3ox'])
+    ox_calc["Ox_Cation_Sum"] = (
+        ox_calc["Si_Ox_cat_3ox"]
+        + ox_calc["Ti_Ox_cat_3ox"]
+        + ox_calc["Al_Ox_cat_3ox"]
+        + ox_calc["Fet_Ox_cat_3ox"]
+        + ox_calc["Mn_Ox_cat_3ox"]
+        + ox_calc["Mg_Ox_cat_3ox"]
+        + ox_calc["Ca_Ox_cat_3ox"]
+        + ox_calc["Na_Ox_cat_3ox"]
+        + ox_calc["K_Ox_cat_3ox"]
+        + ox_calc["Cr_Ox_cat_3ox"]
+        + ox_calc["P_Ox_cat_3ox"]
+    )
 
     # Both octahedral sites
     # Zr4+ substitutes for Ti4+.
     # Cr and V substitute for Fe3+
     # Hard to determine speciation
-    ox_calc['Fe_Ti_Ox'] = ox_calc['Fet_Ox_cat_3ox'] +  ox_calc['Ti_Ox_cat_3ox']
-    ox_calc['Fe_Mg_Mn_A_Ox'] = ox_calc['Fet_Ox_cat_3ox'] + ox_calc['Mg_Ox_cat_3ox'] + ox_calc['Mn_Ox_cat_3ox']
-    ox_calc['Ti_B_Ox'] = ox_calc['Ti_Ox_cat_3ox'] 
-
-    ox_calc['Mg_Fe_M_Ox'] = ox_calc['Mg_Ox_cat_3ox'] + ox_calc['Fet_Ox_cat_3ox']
-    ox_calc['Al_B_Ox'] = ox_calc['Al_Ox_cat_3ox']
-    ox_calc['Al_Ti_Cr_B_Ox'] = ox_calc['Al_Ox_cat_3ox'] + ox_calc['Ti_Ox_cat_3ox'] + ox_calc['Cr_Ox_cat_3ox']
+    ox_calc["Fe_Ti_Ox"] = ox_calc["Fet_Ox_cat_3ox"] + ox_calc["Ti_Ox_cat_3ox"]
+    ox_calc["Fe_Mg_Mn_A_Ox"] = (
+        ox_calc["Fet_Ox_cat_3ox"] + ox_calc["Mg_Ox_cat_3ox"] + ox_calc["Mn_Ox_cat_3ox"]
+    )
+    ox_calc["Ti_B_Ox"] = ox_calc["Ti_Ox_cat_3ox"]
+
+    ox_calc["Mg_Fe_M_Ox"] = ox_calc["Mg_Ox_cat_3ox"] + ox_calc["Fet_Ox_cat_3ox"]
+    ox_calc["Al_B_Ox"] = ox_calc["Al_Ox_cat_3ox"]
+    ox_calc["Al_Ti_Cr_B_Ox"] = (
+        ox_calc["Al_Ox_cat_3ox"] + ox_calc["Ti_Ox_cat_3ox"] + ox_calc["Cr_Ox_cat_3ox"]
+    )
 
     cat_prop = calculate_cat_proportions_oxide(ox_comps=ox_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([ox_comps, ox_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-# %% ZIRCON 
+# %% ZIRCON
+
 
 def calculate_mol_proportions_zircon(zr_comps):
-    
     """
-    
+
     Import zircon compositions using zr_comps=My_Zircons, returns mole proportions
 
     Parameters
     -------
     zr_comps: pandas.DataFrame
             Panda DataFrame of zircon compositions with column headings SiO2_Zr, MgO_Zr etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for zircons with column headings of the form SiO2_Zr_mol_prop
 
     """
 
-    oxide_mass_zr = {'SiO2_Zr': 60.0843, 'MgO_Zr': 40.3044, 'FeOt_Zr': 71.8464, 'CaO_Zr': 56.0774,'Al2O3_Zr': 101.961, 'Na2O_Zr': 61.9789, 'K2O_Zr': 94.196, 'MnO_Zr': 70.9375, 'TiO2_Zr': 79.7877, 'Cr2O3_Zr': 151.9982, 'P2O5_Zr': 141.937, 'ZrO2_Zr': 123.218, 'HfO2_Zr': 210.49}
-    oxide_mass_zr_df = pd.DataFrame.from_dict(oxide_mass_zr, orient='index').T
-    oxide_mass_zr_df['Sample_ID_Zr'] = 'MolWt'
-    oxide_mass_zr_df.set_index('Sample_ID_Zr', inplace=True)
+    oxide_mass_zr = {
+        "SiO2_Zr": 60.0843,
+        "MgO_Zr": 40.3044,
+        "FeOt_Zr": 71.8464,
+        "CaO_Zr": 56.0774,
+        "Al2O3_Zr": 101.961,
+        "Na2O_Zr": 61.9789,
+        "K2O_Zr": 94.196,
+        "MnO_Zr": 70.9375,
+        "TiO2_Zr": 79.7877,
+        "Cr2O3_Zr": 151.9982,
+        "P2O5_Zr": 141.937,
+        "ZrO2_Zr": 123.218,
+        "HfO2_Zr": 210.49,
+    }
+    oxide_mass_zr_df = pd.DataFrame.from_dict(oxide_mass_zr, orient="index").T
+    oxide_mass_zr_df["Sample_ID_Zr"] = "MolWt"
+    oxide_mass_zr_df.set_index("Sample_ID_Zr", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     zr_wt = zr_comps.reindex(oxide_mass_zr_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    zr_wt_combo = pd.concat([oxide_mass_zr_df, zr_wt],)
+    zr_wt_combo = pd.concat(
+        [oxide_mass_zr_df, zr_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = zr_wt_combo.div(
-        zr_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = zr_wt_combo.div(zr_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
-def calculate_cat_proportions_zircon(*, zr_comps=None, oxide_headers=False):
 
+def calculate_cat_proportions_zircon(*, zr_comps=None, oxide_headers=False):
     """
-    
+
     Import zircon compositions using zr_comps=My_zircons, returns cation proportions
 
     Parameters
     -------
     zr_comps: pandas.DataFrame
             zircon compositions with column headings SiO2_Zr, MgO_Zr etc.
     oxide_headers: bool
@@ -4972,146 +7116,219 @@
     Returns
     -------
     pandas DataFrame
         cation proportions for zircon with column headings of the form... Zr_cat_prop
 
     """
 
-    cation_num_zr = {'SiO2_Zr': 1, 'MgO_Zr': 1, 'FeOt_Zr': 1, 'CaO_Zr': 1, 'Al2O3_Zr': 2, 'Na2O_Zr': 2, 'K2O_Zr': 2, 'MnO_Zr': 1, 'TiO2_Zr': 1, 'Cr2O3_Zr': 2, 'P2O5_Zr': 2, 'ZrO2_Zr': 1, 'HfO2': 1}
-    cation_num_zr_df = pd.DataFrame.from_dict(cation_num_zr, orient='index').T
-    cation_num_zr_df['Sample_ID_Zr'] = 'CatNum'
-    cation_num_zr_df.set_index('Sample_ID_Zr', inplace=True)
-
-    oxide_mass_zr = {'SiO2_Zr': 60.0843, 'MgO_Zr': 40.3044, 'FeOt_Zr': 71.8464, 'CaO_Zr': 56.0774,'Al2O3_Zr': 101.961, 'Na2O_Zr': 61.9789, 'K2O_Zr': 94.196, 'MnO_Zr': 70.9375, 'TiO2_Zr': 79.7877, 'Cr2O3_Zr': 151.9982, 'P2O5_Zr': 141.937, 'ZrO2': 123.218, 'HfO2': 210.49}
-    oxide_mass_zr_df = pd.DataFrame.from_dict(oxide_mass_zr, orient='index').T
-    oxide_mass_zr_df['Sample_ID_Zr'] = 'MolWt'
-    oxide_mass_zr_df.set_index('Sample_ID_Zr', inplace=True)
+    cation_num_zr = {
+        "SiO2_Zr": 1,
+        "MgO_Zr": 1,
+        "FeOt_Zr": 1,
+        "CaO_Zr": 1,
+        "Al2O3_Zr": 2,
+        "Na2O_Zr": 2,
+        "K2O_Zr": 2,
+        "MnO_Zr": 1,
+        "TiO2_Zr": 1,
+        "Cr2O3_Zr": 2,
+        "P2O5_Zr": 2,
+        "ZrO2_Zr": 1,
+        "HfO2": 1,
+    }
+    cation_num_zr_df = pd.DataFrame.from_dict(cation_num_zr, orient="index").T
+    cation_num_zr_df["Sample_ID_Zr"] = "CatNum"
+    cation_num_zr_df.set_index("Sample_ID_Zr", inplace=True)
+
+    oxide_mass_zr = {
+        "SiO2_Zr": 60.0843,
+        "MgO_Zr": 40.3044,
+        "FeOt_Zr": 71.8464,
+        "CaO_Zr": 56.0774,
+        "Al2O3_Zr": 101.961,
+        "Na2O_Zr": 61.9789,
+        "K2O_Zr": 94.196,
+        "MnO_Zr": 70.9375,
+        "TiO2_Zr": 79.7877,
+        "Cr2O3_Zr": 151.9982,
+        "P2O5_Zr": 141.937,
+        "ZrO2": 123.218,
+        "HfO2": 210.49,
+    }
+    oxide_mass_zr_df = pd.DataFrame.from_dict(oxide_mass_zr, orient="index").T
+    oxide_mass_zr_df["Sample_ID_Zr"] = "MolWt"
+    oxide_mass_zr_df.set_index("Sample_ID_Zr", inplace=True)
 
     zr_prop_no_cat_num = calculate_mol_proportions_zircon(zr_comps=zr_comps)
-    zr_prop_no_cat_num.columns = [str(col).replace('_mol_prop', '') for col in zr_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_zr_df.reindex(oxide_mass_zr_df.columns, axis=1).fillna(0)
+    zr_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in zr_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_zr_df.reindex(oxide_mass_zr_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, zr_prop_no_cat_num])
-    cation_prop_anhyd = df_calc_comb.multiply(df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+    cation_prop_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
     cation_prop_anhyd.columns = [
-        str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
 
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Zr_cat_prop': 'Si_Zr_cat_prop',
-                            'TiO2_Zr_cat_prop': 'Ti_Zr_cat_prop',
-                            'Al2O3_Zr_cat_prop': 'Al_Zr_cat_prop',
-                            'FeOt_Zr_cat_prop': 'Fet_Zr_cat_prop',
-                            'MnO_Zr_cat_prop': 'Mn_Zr_cat_prop',
-                            'MgO_Zr_cat_prop': 'Mg_Zr_cat_prop',
-                            'CaO_Zr_cat_prop': 'Ca_Zr_cat_prop',
-                            'Na2O_Zr_cat_prop': 'Na_Zr_cat_prop',
-                            'K2O_Zr_cat_prop': 'K_Zr_cat_prop',
-                            'Cr2O3_Zr_cat_prop': 'Cr_Zr_cat_prop',
-                            'P2O5_Zr_cat_prop': 'P_Zr_cat_prop',
-                            'ZrO2_Zr_cat_prop': 'Zr_Zr_cat_prop',
-                            'HfO2_Zr_cat_prop': 'Hf_Zr_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Zr_cat_prop": "Si_Zr_cat_prop",
+                "TiO2_Zr_cat_prop": "Ti_Zr_cat_prop",
+                "Al2O3_Zr_cat_prop": "Al_Zr_cat_prop",
+                "FeOt_Zr_cat_prop": "Fet_Zr_cat_prop",
+                "MnO_Zr_cat_prop": "Mn_Zr_cat_prop",
+                "MgO_Zr_cat_prop": "Mg_Zr_cat_prop",
+                "CaO_Zr_cat_prop": "Ca_Zr_cat_prop",
+                "Na2O_Zr_cat_prop": "Na_Zr_cat_prop",
+                "K2O_Zr_cat_prop": "K_Zr_cat_prop",
+                "Cr2O3_Zr_cat_prop": "Cr_Zr_cat_prop",
+                "P2O5_Zr_cat_prop": "P_Zr_cat_prop",
+                "ZrO2_Zr_cat_prop": "Zr_Zr_cat_prop",
+                "HfO2_Zr_cat_prop": "Hf_Zr_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
-def calculate_oxygens_zircon(zr_comps):
 
+def calculate_oxygens_zircon(zr_comps):
     """
-    
-    Import zircon compositions using zr_comps=My_Zrs, returns number of oxygens 
+
+    Import zircon compositions using zr_comps=My_Zrs, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     zr_comps: pandas.DataFrame
         zircon compositions with column headings SiO2_Zr, MgO_Zr etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Zr_ox
 
     """
 
-    oxygen_num_zr = {'SiO2_Zr': 2, 'MgO_Zr': 1, 'FeOt_Zr': 1, 'CaO_Zr': 1, 'Al2O3_Zr': 3, 'Na2O_Zr': 1, 'K2O_Zr': 1, 'MnO_Zr': 1, 'TiO2_Zr': 2, 'Cr2O3_Zr': 3, 'P2O5_Zr': 5, 'ZrO2': 2, 'HfO2': 2}
-    oxygen_num_zr_df = pd.DataFrame.from_dict(oxygen_num_zr, orient='index').T
-    oxygen_num_zr_df['Sample_ID_Zr'] = 'OxNum'
-    oxygen_num_zr_df.set_index('Sample_ID_Zr', inplace=True)
+    oxygen_num_zr = {
+        "SiO2_Zr": 2,
+        "MgO_Zr": 1,
+        "FeOt_Zr": 1,
+        "CaO_Zr": 1,
+        "Al2O3_Zr": 3,
+        "Na2O_Zr": 1,
+        "K2O_Zr": 1,
+        "MnO_Zr": 1,
+        "TiO2_Zr": 2,
+        "Cr2O3_Zr": 3,
+        "P2O5_Zr": 5,
+        "ZrO2": 2,
+        "HfO2": 2,
+    }
+    oxygen_num_zr_df = pd.DataFrame.from_dict(oxygen_num_zr, orient="index").T
+    oxygen_num_zr_df["Sample_ID_Zr"] = "OxNum"
+    oxygen_num_zr_df.set_index("Sample_ID_Zr", inplace=True)
 
     mol_prop = calculate_mol_proportions_zircon(zr_comps=zr_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
     ox_num_reindex = oxygen_num_zr_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
-    oxygens_anhyd = df_calc_comb.multiply(df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+    oxygens_anhyd = df_calc_comb.multiply(
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
-def calculate_4oxygens_zircon(zr_comps):
 
+def calculate_4oxygens_zircon(zr_comps):
     """
-    
+
     Import zircon compositions using zr_comps=My_Zrs, returns cations on the basis of 4 oxygens.
 
     Parameters
     -------
     zr_comps: pandas.DataFrame
         zircon compositions with column headings SiO2_Zr, MgO_Zr etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 4 oxygens, with column headings of the form... Zr_cat_4ox.
 
     """
 
-    cation_num_zr = {'SiO2_Zr': 1, 'MgO_Zr': 1, 'FeOt_Zr': 1, 'CaO_Zr': 1, 'Al2O3_Zr': 2, 'Na2O_Zr': 2, 'K2O_Zr': 2, 'MnO_Zr': 1, 'TiO2_Zr': 1, 'Cr2O3_Zr': 2, 'P2O5_Zr': 2, 'ZrO2_Zr': 1, 'HfO2_Zr': 1}
-    cation_num_zr_df = pd.DataFrame.from_dict(cation_num_zr, orient='index').T
-    cation_num_zr_df['Sample_ID_Zr'] = 'CatNum'
-    cation_num_zr_df.set_index('Sample_ID_Zr', inplace=True)
+    cation_num_zr = {
+        "SiO2_Zr": 1,
+        "MgO_Zr": 1,
+        "FeOt_Zr": 1,
+        "CaO_Zr": 1,
+        "Al2O3_Zr": 2,
+        "Na2O_Zr": 2,
+        "K2O_Zr": 2,
+        "MnO_Zr": 1,
+        "TiO2_Zr": 1,
+        "Cr2O3_Zr": 2,
+        "P2O5_Zr": 2,
+        "ZrO2_Zr": 1,
+        "HfO2_Zr": 1,
+    }
+    cation_num_zr_df = pd.DataFrame.from_dict(cation_num_zr, orient="index").T
+    cation_num_zr_df["Sample_ID_Zr"] = "CatNum"
+    cation_num_zr_df.set_index("Sample_ID_Zr", inplace=True)
 
     oxygens = calculate_oxygens_zircon(zr_comps=zr_comps)
-    renorm_factor = 4 / (oxygens.sum(axis='columns'))
+    renorm_factor = 4 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_zircon(zr_comps=zr_comps)
-    mol_prop['oxy_renorm_factor_zr'] = renorm_factor
-    mol_prop_4 = mol_prop.multiply(mol_prop['oxy_renorm_factor_zr'], axis='rows')
-    mol_prop_4.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_4.columns]
+    mol_prop["oxy_renorm_factor_zr"] = renorm_factor
+    mol_prop_4 = mol_prop.multiply(mol_prop["oxy_renorm_factor_zr"], axis="rows")
+    mol_prop_4.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_4.columns
+    ]
 
     ox_num_reindex = cation_num_zr_df.reindex(mol_prop_4.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_4])
     cation_4 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
-
-    cation_4.columns = [str(col).replace('_mol_prop', '_cat_4ox')
-                        for col in mol_prop.columns]
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_4_2=cation_4.rename(columns={
-                            'SiO2_Zr_cat_4ox': 'Si_Zr_cat_4ox',
-                            'TiO2_Zr_cat_4ox': 'Ti_Zr_cat_4ox',
-                            'Al2O3_Zr_cat_4ox': 'Al_Zr_cat_4ox',
-                            'FeOt_Zr_cat_4ox': 'Fet_Zr_cat_4ox',
-                            'MnO_Zr_cat_4ox': 'Mn_Zr_cat_4ox',
-                            'MgO_Zr_cat_4ox': 'Mg_Zr_cat_4ox',
-                            'CaO_Zr_cat_4ox': 'Ca_Zr_cat_4ox',
-                            'Na2O_Zr_cat_4ox': 'Na_Zr_cat_4ox',
-                            'K2O_Zr_cat_4ox': 'K_Zr_cat_4ox',
-                            'Cr2O3_Zr_cat_4ox': 'Cr_Zr_cat_4ox',
-                            'P2O5_Zr_cat_4ox': 'P_Zr_cat_4ox', 
-                            'ZrO2_Zr_cat_4ox': 'Zr_Zr_cat_4ox',
-                            'HfO2_Zr_cat_4ox': 'Hf_Zr_cat_4ox',})
+    cation_4.columns = [
+        str(col).replace("_mol_prop", "_cat_4ox") for col in mol_prop.columns
+    ]
+
+    cation_4_2 = cation_4.rename(
+        columns={
+            "SiO2_Zr_cat_4ox": "Si_Zr_cat_4ox",
+            "TiO2_Zr_cat_4ox": "Ti_Zr_cat_4ox",
+            "Al2O3_Zr_cat_4ox": "Al_Zr_cat_4ox",
+            "FeOt_Zr_cat_4ox": "Fet_Zr_cat_4ox",
+            "MnO_Zr_cat_4ox": "Mn_Zr_cat_4ox",
+            "MgO_Zr_cat_4ox": "Mg_Zr_cat_4ox",
+            "CaO_Zr_cat_4ox": "Ca_Zr_cat_4ox",
+            "Na2O_Zr_cat_4ox": "Na_Zr_cat_4ox",
+            "K2O_Zr_cat_4ox": "K_Zr_cat_4ox",
+            "Cr2O3_Zr_cat_4ox": "Cr_Zr_cat_4ox",
+            "P2O5_Zr_cat_4ox": "P_Zr_cat_4ox",
+            "ZrO2_Zr_cat_4ox": "Zr_Zr_cat_4ox",
+            "HfO2_Zr_cat_4ox": "Hf_Zr_cat_4ox",
+        }
+    )
 
     return cation_4_2
 
-def calculate_zircon_components(zr_comps, append):
 
+def calculate_zircon_components(zr_comps, append):
     """
-    
+
     Import zircon compositions using zr_comps=My_Zrs, returns components on the basis of 4 oxygens.
 
     Parameters
     -------
     zr_comps: pandas.DataFrame
         zircon compositions with column headings SiO2_Zr, MgO_Zr etc.
 
@@ -5119,77 +7336,103 @@
     -------
     pandas DataFrame
         components on the basis of 4 oxygens, with column headings of the form... Zr_cat_4ox.
 
     """
 
     zr_comps_new = zr_comps.copy()
-    zr_comps_new.columns = [col.replace(append, '_Zr') for col in zr_comps_new.columns]
+    zr_comps_new.columns = [col.replace(append, "_Zr") for col in zr_comps_new.columns]
     zr_comps = zr_comps_new.copy()
 
     zr_calc = calculate_4oxygens_zircon(zr_comps=zr_comps)
-    zr_calc['Zr_Cation_Sum'] = (zr_calc['Si_Zr_cat_4ox']+zr_calc['Ti_Zr_cat_4ox']+zr_calc['Al_Zr_cat_4ox']+zr_calc['Fet_Zr_cat_4ox']+zr_calc['Mn_Zr_cat_4ox']+zr_calc['Mg_Zr_cat_4ox']+zr_calc['Ca_Zr_cat_4ox']+zr_calc['Na_Zr_cat_4ox']+zr_calc['K_Zr_cat_4ox']+zr_calc['Cr_Zr_cat_4ox']+zr_calc['P_Zr_cat_4ox']) #+zr_calc['Zr_Zr_cat_4ox']+zr_calc['Hf_Zr_cat_4ox'])
+    zr_calc["Zr_Cation_Sum"] = (
+        zr_calc["Si_Zr_cat_4ox"]
+        + zr_calc["Ti_Zr_cat_4ox"]
+        + zr_calc["Al_Zr_cat_4ox"]
+        + zr_calc["Fet_Zr_cat_4ox"]
+        + zr_calc["Mn_Zr_cat_4ox"]
+        + zr_calc["Mg_Zr_cat_4ox"]
+        + zr_calc["Ca_Zr_cat_4ox"]
+        + zr_calc["Na_Zr_cat_4ox"]
+        + zr_calc["K_Zr_cat_4ox"]
+        + zr_calc["Cr_Zr_cat_4ox"]
+        + zr_calc["P_Zr_cat_4ox"]
+    )  # +zr_calc['Zr_Zr_cat_4ox']+zr_calc['Hf_Zr_cat_4ox'])
 
     # zr_calc['Zr_Hf_Zr'] = zr_calc['Zr_Zr_cat_4ox'] + zr_calc['Hf_Zr_cat_4ox']
-    zr_calc['Si_Zr'] = zr_calc['Si_Zr_cat_4ox']
+    zr_calc["Si_Zr"] = zr_calc["Si_Zr_cat_4ox"]
 
     cat_prop = calculate_cat_proportions_zircon(zr_comps=zr_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([zr_comps, zr_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
 
 
-# %% QUARTZ 
+# %% QUARTZ
 
-def calculate_mol_proportions_quartz(qz_comps):
 
+def calculate_mol_proportions_quartz(qz_comps):
     """
-    
+
     Import Quartz compositions using qz_comps=My_Quartzs, returns mole proportions
 
     Parameters
     -------
     qz_comps: pandas.DataFrame
             Panda DataFrame of quartz compositions with column headings SiO2_Qz, MgO_Qz etc.
 
     Returns
     -------
     pandas DataFrame
         mole proportions for quartzs with column headings of the form SiO2_Qz_mol_prop
 
     """
 
-    oxide_mass_qz = {'SiO2_Qz': 60.0843, 'MgO_Qz': 40.3044, 'FeOt_Qz': 71.8464, 'CaO_Qz': 56.0774,'Al2O3_Qz': 101.961, 'Na2O_Qz': 61.9789, 'K2O_Qz': 94.196, 'MnO_Qz': 70.9375, 'TiO2_Qz': 79.7877, 'Cr2O3_Qz': 151.9982, 'P2O5_Qz': 141.937}
-    oxide_mass_qz_df = pd.DataFrame.from_dict(oxide_mass_qz, orient='index').T
-    oxide_mass_qz_df['Sample_ID_Qz'] = 'MolWt'
-    oxide_mass_qz_df.set_index('Sample_ID_Qz', inplace=True)
+    oxide_mass_qz = {
+        "SiO2_Qz": 60.0843,
+        "MgO_Qz": 40.3044,
+        "FeOt_Qz": 71.8464,
+        "CaO_Qz": 56.0774,
+        "Al2O3_Qz": 101.961,
+        "Na2O_Qz": 61.9789,
+        "K2O_Qz": 94.196,
+        "MnO_Qz": 70.9375,
+        "TiO2_Qz": 79.7877,
+        "Cr2O3_Qz": 151.9982,
+        "P2O5_Qz": 141.937,
+    }
+    oxide_mass_qz_df = pd.DataFrame.from_dict(oxide_mass_qz, orient="index").T
+    oxide_mass_qz_df["Sample_ID_Qz"] = "MolWt"
+    oxide_mass_qz_df.set_index("Sample_ID_Qz", inplace=True)
 
     # This makes it match the columns in the oxide mass dataframe
     qz_wt = qz_comps.reindex(oxide_mass_qz_df.columns, axis=1).fillna(0)
     # Combine the molecular weight and weight percent dataframes
-    qz_wt_combo = pd.concat([oxide_mass_qz_df, qz_wt],)
+    qz_wt_combo = pd.concat(
+        [oxide_mass_qz_df, qz_wt],
+    )
     # Drop the calculation column
-    mol_prop_anhyd = qz_wt_combo.div(
-        qz_wt_combo.loc['MolWt', :], axis='columns').drop(['MolWt'])
-    mol_prop_anhyd.columns = [
-        str(col) + '_mol_prop' for col in mol_prop_anhyd.columns]
+    mol_prop_anhyd = qz_wt_combo.div(qz_wt_combo.loc["MolWt", :], axis="columns").drop(
+        ["MolWt"]
+    )
+    mol_prop_anhyd.columns = [str(col) + "_mol_prop" for col in mol_prop_anhyd.columns]
     return mol_prop_anhyd
 
 
 def calculate_cat_proportions_quartz(*, qz_comps=None, oxide_headers=False):
-    
     """
-    
+
     Import quartz compositions using qz_comps=My_quartzs, returns cation proportions
-    
+
     Parameters
     -------
     qz_comps: pandas.DataFrame
             quartz compositions with column headings SiO2_Plag, MgO_Plag etc.
     oxide_headers: bool
         default=False, returns as Ti_Qz_cat_prop.
         =True returns Ti_Qz_cat_prop.
@@ -5199,150 +7442,208 @@
     Returns
     -------
     pandas DataFrame
         cation proportions for quartz with column headings of the form... Qz_cat_prop
 
     """
 
-    cation_num_qz = {'SiO2_Qz': 1, 'MgO_Qz': 1, 'FeOt_Qz': 1, 'CaO_Qz': 1, 'Al2O3_Qz': 2, 'Na2O_Qz': 2, 'K2O_Qz': 2, 'MnO_Qz': 1, 'TiO2_Qz': 1, 'Cr2O3_Qz': 2, 'P2O5_Qz': 2}
-    cation_num_qz_df = pd.DataFrame.from_dict(cation_num_qz, orient='index').T
-    cation_num_qz_df['Sample_ID_Qz'] = 'CatNum'
-    cation_num_qz_df.set_index('Sample_ID_Qz', inplace=True)
-
-    oxide_mass_qz = {'SiO2_Qz': 60.0843, 'MgO_Qz': 40.3044, 'FeOt_Qz': 71.8464, 'CaO_Qz': 56.0774,'Al2O3_Qz': 101.961, 'Na2O_Qz': 61.9789, 'K2O_Qz': 94.196, 'MnO_Qz': 70.9375, 'TiO2_Qz': 79.7877, 'Cr2O3_Qz': 151.9982, 'P2O5_Qz': 141.937}
-
-    oxide_mass_qz_df = pd.DataFrame.from_dict(oxide_mass_qz, orient='index').T
-    oxide_mass_qz_df['Sample_ID_Qz'] = 'MolWt'
-    oxide_mass_qz_df.set_index('Sample_ID_Qz', inplace=True)
-
-    qz_prop_no_cat_num = calculate_mol_proportions_quartz(
-        qz_comps=qz_comps)
-    qz_prop_no_cat_num.columns = [str(col).replace(
-        '_mol_prop', '') for col in qz_prop_no_cat_num.columns]
-    ox_num_reindex = cation_num_qz_df.reindex(
-        oxide_mass_qz_df.columns, axis=1).fillna(0)
+    cation_num_qz = {
+        "SiO2_Qz": 1,
+        "MgO_Qz": 1,
+        "FeOt_Qz": 1,
+        "CaO_Qz": 1,
+        "Al2O3_Qz": 2,
+        "Na2O_Qz": 2,
+        "K2O_Qz": 2,
+        "MnO_Qz": 1,
+        "TiO2_Qz": 1,
+        "Cr2O3_Qz": 2,
+        "P2O5_Qz": 2,
+    }
+    cation_num_qz_df = pd.DataFrame.from_dict(cation_num_qz, orient="index").T
+    cation_num_qz_df["Sample_ID_Qz"] = "CatNum"
+    cation_num_qz_df.set_index("Sample_ID_Qz", inplace=True)
+
+    oxide_mass_qz = {
+        "SiO2_Qz": 60.0843,
+        "MgO_Qz": 40.3044,
+        "FeOt_Qz": 71.8464,
+        "CaO_Qz": 56.0774,
+        "Al2O3_Qz": 101.961,
+        "Na2O_Qz": 61.9789,
+        "K2O_Qz": 94.196,
+        "MnO_Qz": 70.9375,
+        "TiO2_Qz": 79.7877,
+        "Cr2O3_Qz": 151.9982,
+        "P2O5_Qz": 141.937,
+    }
+
+    oxide_mass_qz_df = pd.DataFrame.from_dict(oxide_mass_qz, orient="index").T
+    oxide_mass_qz_df["Sample_ID_Qz"] = "MolWt"
+    oxide_mass_qz_df.set_index("Sample_ID_Qz", inplace=True)
+
+    qz_prop_no_cat_num = calculate_mol_proportions_quartz(qz_comps=qz_comps)
+    qz_prop_no_cat_num.columns = [
+        str(col).replace("_mol_prop", "") for col in qz_prop_no_cat_num.columns
+    ]
+    ox_num_reindex = cation_num_qz_df.reindex(oxide_mass_qz_df.columns, axis=1).fillna(
+        0
+    )
     df_calc_comb = pd.concat([ox_num_reindex, qz_prop_no_cat_num])
     cation_prop_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
     cation_prop_anhyd.columns = [
-        str(col) + '_cat_prop' for col in cation_prop_anhyd.columns]
+        str(col) + "_cat_prop" for col in cation_prop_anhyd.columns
+    ]
     if oxide_headers is True:
         return cation_prop_anhyd
     if oxide_headers is False:
-        cation_prop_anhyd2=cation_prop_anhyd.rename(columns={
-                            'SiO2_Qz_cat_prop': 'Si_Qz_cat_prop',
-                            'TiO2_Qz_cat_prop': 'Ti_Qz_cat_prop',
-                            'Al2O3_Qz_cat_prop': 'Al_Qz_cat_prop',
-                            'FeOt_Qz_cat_prop': 'Fet_Qz_cat_prop',
-                            'MnO_Qz_cat_prop': 'Mn_Qz_cat_prop',
-                            'MgO_Qz_cat_prop': 'Mg_Qz_cat_prop',
-                            'CaO_Qz_cat_prop': 'Ca_Qz_cat_prop',
-                            'Na2O_Qz_cat_prop': 'Na_Qz_cat_prop',
-                            'K2O_Qz_cat_prop': 'K_Qz_cat_prop',
-                            'Cr2O3_Qz_cat_prop': 'Cr_Qz_cat_prop',
-                            'P2O5_Qz_cat_prop': 'P_Qz_cat_prop',})
+        cation_prop_anhyd2 = cation_prop_anhyd.rename(
+            columns={
+                "SiO2_Qz_cat_prop": "Si_Qz_cat_prop",
+                "TiO2_Qz_cat_prop": "Ti_Qz_cat_prop",
+                "Al2O3_Qz_cat_prop": "Al_Qz_cat_prop",
+                "FeOt_Qz_cat_prop": "Fet_Qz_cat_prop",
+                "MnO_Qz_cat_prop": "Mn_Qz_cat_prop",
+                "MgO_Qz_cat_prop": "Mg_Qz_cat_prop",
+                "CaO_Qz_cat_prop": "Ca_Qz_cat_prop",
+                "Na2O_Qz_cat_prop": "Na_Qz_cat_prop",
+                "K2O_Qz_cat_prop": "K_Qz_cat_prop",
+                "Cr2O3_Qz_cat_prop": "Cr_Qz_cat_prop",
+                "P2O5_Qz_cat_prop": "P_Qz_cat_prop",
+            }
+        )
 
         return cation_prop_anhyd2
 
+
 def calculate_oxygens_quartz(qz_comps):
-    
     """
-    
-    Import quartz compositions using qz_comps=My_Qzs, returns number of oxygens 
+
+    Import quartz compositions using qz_comps=My_Qzs, returns number of oxygens
     (e.g., mol proportions * number of O in formula unit)
 
     Parameters
     -------
     qz_comps: pandas.DataFrame
         quartz compositions with column headings SiO2_Qz, MgO_Qz etc.
 
     Returns
     -------
     pandas DataFrame
         number of oxygens with column headings of the form SiO2_Qz
 
     """
 
-    oxygen_num_qz = {'SiO2_Qz': 2, 'MgO_Qz': 1, 'FeOt_Qz': 1, 'CaO_Qz': 1, 'Al2O3_Qz': 3, 'Na2O_Qz': 1, 'K2O_Qz': 1, 'MnO_Qz': 1, 'TiO2_Qz': 2, 'Cr2O3_Qz': 3, 'P2O5_Qz': 5}
-    oxygen_num_qz_df = pd.DataFrame.from_dict(oxygen_num_qz, orient='index').T
-    oxygen_num_qz_df['Sample_ID_Qz'] = 'OxNum'
-    oxygen_num_qz_df.set_index('Sample_ID_Qz', inplace=True)
+    oxygen_num_qz = {
+        "SiO2_Qz": 2,
+        "MgO_Qz": 1,
+        "FeOt_Qz": 1,
+        "CaO_Qz": 1,
+        "Al2O3_Qz": 3,
+        "Na2O_Qz": 1,
+        "K2O_Qz": 1,
+        "MnO_Qz": 1,
+        "TiO2_Qz": 2,
+        "Cr2O3_Qz": 3,
+        "P2O5_Qz": 5,
+    }
+    oxygen_num_qz_df = pd.DataFrame.from_dict(oxygen_num_qz, orient="index").T
+    oxygen_num_qz_df["Sample_ID_Qz"] = "OxNum"
+    oxygen_num_qz_df.set_index("Sample_ID_Qz", inplace=True)
 
     mol_prop = calculate_mol_proportions_quartz(qz_comps=qz_comps)
-    mol_prop.columns = [str(col).replace('_mol_prop', '')
-                        for col in mol_prop.columns]
-    ox_num_reindex = oxygen_num_qz_df.reindex(
-        mol_prop.columns, axis=1).fillna(0)
+    mol_prop.columns = [str(col).replace("_mol_prop", "") for col in mol_prop.columns]
+    ox_num_reindex = oxygen_num_qz_df.reindex(mol_prop.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop])
     oxygens_anhyd = df_calc_comb.multiply(
-        df_calc_comb.loc['OxNum', :], axis='columns').drop(['OxNum'])
-    oxygens_anhyd.columns = [str(col) + '_ox' for col in oxygens_anhyd.columns]
+        df_calc_comb.loc["OxNum", :], axis="columns"
+    ).drop(["OxNum"])
+    oxygens_anhyd.columns = [str(col) + "_ox" for col in oxygens_anhyd.columns]
 
     return oxygens_anhyd
 
+
 def calculate_2oxygens_quartz(qz_comps):
-    
     """
-    
+
     Import quartz compositions using qz_comps=My_Qzs, returns cations on the basis of 4 oxygens.
 
     Parameters
     -------
     qz_comps: pandas.DataFrame
         quartz compositions with column headings SiO2_Qz, MgO_Qz etc.
 
     Returns
     -------
     pandas DataFrame
         cations on the basis of 2 oxygens, with column headings of the form... Qz_cat_2ox.
 
     """
 
-    cation_num_qz = {'SiO2_Qz': 1, 'MgO_Qz': 1, 'FeOt_Qz': 1, 'CaO_Qz': 1, 'Al2O3_Qz': 2, 'Na2O_Qz': 2, 'K2O_Qz': 2, 'MnO_Qz': 1, 'TiO2_Qz': 1, 'Cr2O3_Qz': 2, 'P2O5_Qz': 2}
-
-    cation_num_qz_df = pd.DataFrame.from_dict(cation_num_qz, orient='index').T
-    cation_num_qz_df['Sample_ID_Qz'] = 'CatNum'
-    cation_num_qz_df.set_index('Sample_ID_Qz', inplace=True)
+    cation_num_qz = {
+        "SiO2_Qz": 1,
+        "MgO_Qz": 1,
+        "FeOt_Qz": 1,
+        "CaO_Qz": 1,
+        "Al2O3_Qz": 2,
+        "Na2O_Qz": 2,
+        "K2O_Qz": 2,
+        "MnO_Qz": 1,
+        "TiO2_Qz": 1,
+        "Cr2O3_Qz": 2,
+        "P2O5_Qz": 2,
+    }
+
+    cation_num_qz_df = pd.DataFrame.from_dict(cation_num_qz, orient="index").T
+    cation_num_qz_df["Sample_ID_Qz"] = "CatNum"
+    cation_num_qz_df.set_index("Sample_ID_Qz", inplace=True)
 
     oxygens = calculate_oxygens_quartz(qz_comps=qz_comps)
-    renorm_factor = 2 / (oxygens.sum(axis='columns'))
+    renorm_factor = 2 / (oxygens.sum(axis="columns"))
     mol_prop = calculate_mol_proportions_quartz(qz_comps=qz_comps)
-    mol_prop['oxy_renorm_factor_qz'] = renorm_factor
-    mol_prop_2 = mol_prop.multiply(mol_prop['oxy_renorm_factor_qz'], axis='rows')
-    mol_prop_2.columns = [str(col).replace('_mol_prop', '')
-                          for col in mol_prop_2.columns]
+    mol_prop["oxy_renorm_factor_qz"] = renorm_factor
+    mol_prop_2 = mol_prop.multiply(mol_prop["oxy_renorm_factor_qz"], axis="rows")
+    mol_prop_2.columns = [
+        str(col).replace("_mol_prop", "") for col in mol_prop_2.columns
+    ]
 
-    ox_num_reindex = cation_num_qz_df.reindex(
-        mol_prop_2.columns, axis=1).fillna(0)
+    ox_num_reindex = cation_num_qz_df.reindex(mol_prop_2.columns, axis=1).fillna(0)
     df_calc_comb = pd.concat([ox_num_reindex, mol_prop_2])
     cation_2 = df_calc_comb.multiply(
-        df_calc_comb.loc['CatNum', :], axis='columns').drop(['CatNum'])
+        df_calc_comb.loc["CatNum", :], axis="columns"
+    ).drop(["CatNum"])
 
-    cation_2.columns = [str(col).replace('_mol_prop', '_cat_2ox')
-                        for col in mol_prop.columns]
-
-    cation_2_2=cation_2.rename(columns={
-                            'SiO2_Qz_cat_2ox': 'Si_Qz_cat_2ox',
-                            'TiO2_Qz_cat_2ox': 'Ti_Qz_cat_2ox',
-                            'Al2O3_Qz_cat_2ox': 'Al_Qz_cat_2ox',
-                            'FeOt_Qz_cat_2ox': 'Fet_Qz_cat_2ox',
-                            'MnO_Qz_cat_2ox': 'Mn_Qz_cat_2ox',
-                            'MgO_Qz_cat_2ox': 'Mg_Qz_cat_2ox',
-                            'CaO_Qz_cat_2ox': 'Ca_Qz_cat_2ox',
-                            'Na2O_Qz_cat_2ox': 'Na_Qz_cat_2ox',
-                            'K2O_Qz_cat_2ox': 'K_Qz_cat_2ox',
-                            'Cr2O3_Qz_cat_2ox': 'Cr_Qz_cat_2ox',
-                            'P2O5_Qz_cat_2ox': 'P_Qz_cat_2ox',})
+    cation_2.columns = [
+        str(col).replace("_mol_prop", "_cat_2ox") for col in mol_prop.columns
+    ]
+
+    cation_2_2 = cation_2.rename(
+        columns={
+            "SiO2_Qz_cat_2ox": "Si_Qz_cat_2ox",
+            "TiO2_Qz_cat_2ox": "Ti_Qz_cat_2ox",
+            "Al2O3_Qz_cat_2ox": "Al_Qz_cat_2ox",
+            "FeOt_Qz_cat_2ox": "Fet_Qz_cat_2ox",
+            "MnO_Qz_cat_2ox": "Mn_Qz_cat_2ox",
+            "MgO_Qz_cat_2ox": "Mg_Qz_cat_2ox",
+            "CaO_Qz_cat_2ox": "Ca_Qz_cat_2ox",
+            "Na2O_Qz_cat_2ox": "Na_Qz_cat_2ox",
+            "K2O_Qz_cat_2ox": "K_Qz_cat_2ox",
+            "Cr2O3_Qz_cat_2ox": "Cr_Qz_cat_2ox",
+            "P2O5_Qz_cat_2ox": "P_Qz_cat_2ox",
+        }
+    )
 
     return cation_2_2
 
-def calculate_quartz_components(qz_comps, append):
 
+def calculate_quartz_components(qz_comps, append):
     """
-    
+
     Import quartz compositions using qz_comps=My_Qzs, returns cations on the basis of 4 oxygens.
 
     Parameters
     -------
     qz_comps: pandas.DataFrame
         quartz compositions with column headings SiO2_Qz, MgO_Qz etc.
 
@@ -5350,25 +7651,39 @@
     -------
     pandas DataFrame
         components on the basis of 2 oxygens, with column headings of the form... Qz_cat_2ox.
 
     """
 
     qz_comps_new = qz_comps.copy()
-    qz_comps_new.columns = [col.replace(append, '_Qz') for col in qz_comps_new.columns]
+    qz_comps_new.columns = [col.replace(append, "_Qz") for col in qz_comps_new.columns]
     qz_comps = qz_comps_new.copy()
 
     qz_calc = calculate_2oxygens_quartz(qz_comps=qz_comps)
-    qz_calc['Qz_Cation_Sum'] = (qz_calc['Si_Qz_cat_2ox']+qz_calc['Ti_Qz_cat_2ox']+qz_calc['Al_Qz_cat_2ox']+qz_calc['Fet_Qz_cat_2ox']+qz_calc['Mn_Qz_cat_2ox']+qz_calc['Mg_Qz_cat_2ox']+qz_calc['Ca_Qz_cat_2ox']+qz_calc['Na_Qz_cat_2ox']+qz_calc['K_Qz_cat_2ox']+qz_calc['Cr_Qz_cat_2ox']+qz_calc['P_Qz_cat_2ox'])
-
-    qz_calc['Si_Al_Ti_Qz'] = qz_calc['Si_Qz_cat_2ox'] + qz_calc['Al_Qz_cat_2ox'] + qz_calc['Ti_Qz_cat_2ox']
+    qz_calc["Qz_Cation_Sum"] = (
+        qz_calc["Si_Qz_cat_2ox"]
+        + qz_calc["Ti_Qz_cat_2ox"]
+        + qz_calc["Al_Qz_cat_2ox"]
+        + qz_calc["Fet_Qz_cat_2ox"]
+        + qz_calc["Mn_Qz_cat_2ox"]
+        + qz_calc["Mg_Qz_cat_2ox"]
+        + qz_calc["Ca_Qz_cat_2ox"]
+        + qz_calc["Na_Qz_cat_2ox"]
+        + qz_calc["K_Qz_cat_2ox"]
+        + qz_calc["Cr_Qz_cat_2ox"]
+        + qz_calc["P_Qz_cat_2ox"]
+    )
+
+    qz_calc["Si_Al_Ti_Qz"] = (
+        qz_calc["Si_Qz_cat_2ox"] + qz_calc["Al_Qz_cat_2ox"] + qz_calc["Ti_Qz_cat_2ox"]
+    )
 
     cat_prop = calculate_cat_proportions_quartz(qz_comps=qz_comps)
-    cat_prop['sum'] = cat_prop.sum(axis='columns')
-    cat_frac_anhyd = cat_prop.div(cat_prop['sum'], axis='rows')
-    cat_frac_anhyd.drop(['sum'], axis='columns', inplace=True)
-    cat_frac_anhyd.columns = [str(col).replace('prop', 'frac')
-                              for col in cat_frac_anhyd.columns]
+    cat_prop["sum"] = cat_prop.sum(axis="columns")
+    cat_frac_anhyd = cat_prop.div(cat_prop["sum"], axis="rows")
+    cat_frac_anhyd.drop(["sum"], axis="columns", inplace=True)
+    cat_frac_anhyd.columns = [
+        str(col).replace("prop", "frac") for col in cat_frac_anhyd.columns
+    ]
     cat_frac_anhyd2 = pd.concat([qz_comps, qz_calc, cat_frac_anhyd], axis=1)
 
     return cat_frac_anhyd2
-
```

### Comparing `mineralML-0.0.0.5/src/mineralML/supervised.py` & `mineralML-0.0.0.6/src/mineralML/supervised.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,315 +1,356 @@
 # %%
 
 import os
 import math
 import time
 import copy
+import warnings
 
 import numpy as np
 import pandas as pd
 
 from sklearn.preprocessing import StandardScaler
-from sklearn.model_selection import train_test_split 
+from sklearn.model_selection import train_test_split
 from sklearn.metrics import classification_report, confusion_matrix
 
 import torch
 import torch.nn as nn
 from torch.nn.modules.activation import LeakyReLU
 from torch.utils.data import DataLoader
 import torch.nn.functional as F
 
 from mineralML.core import *
 
 # %%
 
 
 def load_minclass_nn():
-
     """
-    Loads mineral classes and their corresponding mappings from a .npz file. 
-    The file is expected to contain an array of class names under the 'classes' key. 
+    Loads mineral classes and their corresponding mappings from a .npz file.
+    The file is expected to contain an array of class names under the 'classes' key.
     This function creates a dictionary that maps an integer code to each class name.
 
     Returns:
         min_cat (list): A list of mineral class names.
-        mapping (dict): A dictionary that maps each integer code to its corresponding 
+        mapping (dict): A dictionary that maps each integer code to its corresponding
         class name in the 'min_cat' list.
     """
 
     current_dir = os.path.dirname(__file__)
-    filepath = os.path.join(current_dir, 'mineral_classes_nn.npz')
+    filepath = os.path.join(current_dir, "mineral_classes_nn.npz")
 
     with np.load(filepath, allow_pickle=True) as data:
-        min_cat = data['classes'].tolist()
+        min_cat = data["classes"].tolist()
     mapping = {code: cat for code, cat in enumerate(min_cat)}
 
     return min_cat, mapping
 
 
 def prep_df_nn(df):
-
     """
-
-    Prepares a DataFrame for analysis by performing data cleaning specific to mineralogical data. 
-    It filters the DataFrame for selected minerals, handles missing values, and separates the data 
-    into two DataFrames: one that includes specified minerals and another that excludes them.
-    The function defines a list of oxide column names and minerals to include and exclude. It drops 
-    rows where the specified oxides and 'Mineral' column have fewer than six non-NaN values. 
+    Prepares a DataFrame for analysis by performing data cleaning specific to mineralogical data.
+    It handles missing values and ensures the presence of required oxide columns.
+    The function defines a list of oxide column names and drops rows where the specified oxides
+    have fewer than six non-NaN values.
 
     Parameters:
         df (DataFrame): The input DataFrame containing mineral composition data along with 'Mineral' column.
 
     Returns:
-        df_in (DataFrame): A DataFrame with rows including only the specified minerals and 'NaN' filled with zero.
-        df_ex (DataFrame): A DataFrame with rows excluding the specified minerals and 'NaN' filled with zero.
-    
-    """
-
-    if "FeO" in df.columns and "FeOt" not in df.columns:
-        raise ValueError("No 'FeOt' column found. You have a 'FeO' column. mineralML only recognizes 'FeOt' as a column. Please convert to FeOt.")
-    if "Fe2O3" in df.columns and "FeOt" not in df.columns:
-        raise ValueError("No 'FeOt' column found. You have a 'Fe2O3' column. mineralML only recognizes 'FeOt' as a column. Please convert to FeOt.")
-
-    oxidesandmin = ['SiO2', 'TiO2', 'Al2O3', 'FeOt', 'MnO', 'MgO', 'CaO', 'Na2O', 'K2O', 'Cr2O3', 'Mineral']
-    include_minerals = ['Amphibole', 'Biotite', 'Clinopyroxene', 'Garnet', 'Ilmenite', 
-                        'KFeldspar', 'Magnetite', 'Muscovite', 'Olivine', 'Orthopyroxene', 
-                        'Plagioclase', 'Spinel']
-    exclude_minerals = ['Tourmaline', 'Quartz', 'Rutile', 'Apatite', 'Zircon']
-    df.dropna(subset=oxidesandmin, thresh=6, inplace=True)
-
-    if 'Mineral' in df.columns:
-        include_minerals = ['Amphibole', 'Biotite', 'Clinopyroxene', 'Garnet', 'Ilmenite', 
-                            'KFeldspar', 'Magnetite', 'Muscovite', 'Olivine', 'Orthopyroxene', 
-                            'Plagioclase', 'Spinel']
-        exclude_minerals = ['Tourmaline', 'Quartz', 'Rutile', 'Apatite', 'Zircon']
-        df_in = df[df['Mineral'].isin(include_minerals)]
-        df_ex = df[df['Mineral'].isin(exclude_minerals)]
-    else:
-        df_in = df.copy()
-        df_ex = pd.DataFrame(columns=df.columns)  
+        df (DataFrame): The cleaned DataFrame with 'NaN' filled with zero for oxides.
+    """
 
-    df_in = df_in[oxidesandmin].fillna(0)
-    df_ex = df_ex[oxidesandmin].fillna(0)
+    if "FeO" in df.columns:
+        if "FeOt" not in df.columns:
+            raise ValueError(
+                "No 'FeOt' column found. You have a 'FeO' column. "
+                "mineralML only recognizes 'FeOt' as a column. Please convert to FeOt."
+            )
+    if "Fe2O3" in df.columns:
+        if "FeOt" not in df.columns:
+            raise ValueError(
+                "No 'FeOt' column found. You have a 'Fe2O3' column. "
+                "mineralML only recognizes 'FeOt' as a column. Please convert to FeOt."
+            )
+
+    oxides = [
+        "SiO2",
+        "TiO2",
+        "Al2O3",
+        "FeOt",
+        "MnO",
+        "MgO",
+        "CaO",
+        "Na2O",
+        "K2O",
+        "Cr2O3",
+    ]
+
+    # Ensure all required columns are present in the DataFrame
+    for col in oxides + ["Mineral", "SampleID"]:
+        if col not in df.columns:
+            df[col] = np.nan
+            warnings.warn(
+                f"The column '{col}' was missing and has been filled with NaN.",
+                UserWarning,
+                stacklevel=2,
+            )
+
+    # Drop rows with fewer than 6 non-NaN values in the oxides columns
+    df.dropna(subset=oxides, thresh=6, inplace=True)
+
+    # Fill remaining NaN values with 0 for oxides, keep NaN for 'Mineral'
+    df[oxides] = df[oxides].fillna(0)
 
-    df_in = df_in.reset_index(drop=True)
-    df_ex = df_ex.reset_index(drop=True)
+    # Ensure only oxides, 'Mineral', and 'SampleID' columns are kept
+    df = df[oxides + ["Mineral", "SampleID"]]
 
-    return df_in, df_ex
+    # Ensure SampleID is the index
+    df.set_index("SampleID", inplace=True)
 
+    return df
 
-def norm_data_nn(df):
 
+def norm_data_nn(df):
     """
 
-    Normalizes the oxide composition data in the input DataFrame using a predefined StandardScaler. 
-    It ensures that the dataframe has been preprocessed accordingly before applying the transformation. 
-    The function expects that the scaler is already fitted and available for use as defined in the 
+    Normalizes the oxide composition data in the input DataFrame using a predefined StandardScaler.
+    It ensures that the dataframe has been preprocessed accordingly before applying the transformation.
+    The function expects that the scaler is already fitted and available for use as defined in the
     'load_scaler' function.
 
     Parameters:
         df (DataFrame): The input DataFrame containing the oxide composition data.
 
     Returns:
         array_x (ndarray): An array of the transformed oxide composition data.
 
     """
 
-    oxides = ['SiO2', 'TiO2', 'Al2O3', 'FeOt', 'MnO', 'MgO', 'CaO', 'Na2O', 'K2O', 'Cr2O3']
-    mean, std = load_scaler('scaler_nn.npz')
+    oxides = [
+        "SiO2",
+        "TiO2",
+        "Al2O3",
+        "FeOt",
+        "MnO",
+        "MgO",
+        "CaO",
+        "Na2O",
+        "K2O",
+        "Cr2O3",
+    ]
+    mean, std = load_scaler("scaler_nn.npz")
 
     scaled_df = df[oxides].copy()
 
     if df[oxides].isnull().any().any():
         df, _ = prep_df_nn(df)
-    else: 
-        df = df 
+    else:
+        df = df
 
-    for col in df[oxides].columns: 
+    for col in df[oxides].columns:
         scaled_df[col] = (df[col] - mean[col]) / std[col]
 
     array_x = scaled_df.to_numpy()
-    
+
     return array_x
 
 
 def balance(train_x, train_y, n=1000):
-
     """
 
-    Balances the training dataset by oversampling the minority class using the RandomOverSampler method. 
-    It aims to equalize the number of samples for each class in the dataset to prevent the model from 
+    Balances the training dataset by oversampling the minority class using the RandomOverSampler method.
+    It aims to equalize the number of samples for each class in the dataset to prevent the model from
     being biased towards the majority class.
 
     Parameters:
         train_x (numpy.ndarray): The feature matrix for the training data.
         train_y (numpy.ndarray): The corresponding label vector for the training data.
 
     Returns:
         train_x (numpy.ndarray): The feature matrix after oversampling the minority class.
         train_y (numpy.ndarray): The label vector after oversampling the minority class.
 
-    The function creates a new balanced DataFrame with an equal number of samples for each class. 
-    Classes are oversampled to reach a count of 1000 samples per class, with the random state set 
-    for reproducibility. The function returns the resampled feature matrix and label vector suitable 
+    The function creates a new balanced DataFrame with an equal number of samples for each class.
+    Classes are oversampled to reach a count of 1000 samples per class, with the random state set
+    for reproducibility. The function returns the resampled feature matrix and label vector suitable
     for training a machine learning model.
 
     """
 
     try:
         from imblearn.over_sampling import RandomOverSampler
     except ImportError:
-        raise RuntimeError('You have not installed imblearn, which is required to balance the datasets used for training the neural networks. If you use conda, run conda install -c conda-forge imbalanced-learn. If you use pip, run pip install -U imbalanced-learn.')
+        raise RuntimeError(
+            "You have not installed imblearn, which is required to balance the datasets used for training the neural networks. "
+            "If you use conda, run conda install -c conda-forge imbalanced-learn. If you use pip, run pip install -U imbalanced-learn."
+        )
 
-    oversample = RandomOverSampler(sampling_strategy='minority', random_state=42)
+    oversample = RandomOverSampler(sampling_strategy="minority", random_state=42)
 
     # Resample the dataset
     x_balanced, y_balanced = oversample.fit_resample(train_x, train_y)
 
     df_resampled = pd.DataFrame(x_balanced)
-    df_resampled['Mineral'] = y_balanced
+    df_resampled["Mineral"] = y_balanced
 
     df_balanced = pd.DataFrame()
-    for class_label in df_resampled['Mineral'].unique():
-        df_class = df_resampled[df_resampled['Mineral'] == class_label]
-        df_balanced = pd.concat([df_balanced, df_class.sample(n=n, replace = True, random_state=42)])
+    for class_label in df_resampled["Mineral"].unique():
+        df_class = df_resampled[df_resampled["Mineral"] == class_label]
+        df_balanced = pd.concat(
+            [df_balanced, df_class.sample(n=n, replace=True, random_state=42)]
+        )
 
     # Reset the index of the balanced dataframe
     df_balanced = df_balanced.reset_index(drop=True)
     train_x = df_balanced.iloc[:, :-1].to_numpy()
     train_y = df_balanced.iloc[:, -1].to_numpy()
 
     return train_x, train_y
 
 
 class VariationalLayer(nn.Module):
 
     """
-    
-    The VariationalLayer class implements a Bayesian approach to linear layers 
-    in neural networks, which allows for the incorporation 
-    of uncertainty in the weights and biases. This is achieved by modeling the 
-    parameters as distributions rather than point estimates. The layer utilizes 
+
+    The VariationalLayer class implements a Bayesian approach to linear layers
+    in neural networks, which allows for the incorporation
+    of uncertainty in the weights and biases. This is achieved by modeling the
+    parameters as distributions rather than point estimates. The layer utilizes
     variational inference to learn the parameters of these distributions.
 
     Parameters:
         in_features (int): The number of input features to the layer.
         out_features (int): The number of output features from the layer.
 
     Attributes:
         weight_mu (Parameter): The mean of the Gaussian distributions of the weights.
-        weight_rho (Parameter): The rho parameters (unconstrained) for the standard 
+        weight_rho (Parameter): The rho parameters (unconstrained) for the standard
                                 deviations of the Gaussian distributions of the weights.
         bias_mu (Parameter): The mean of the Gaussian distributions of the biases.
-        bias_rho (Parameter): The rho parameters (unconstrained) for the standard 
+        bias_rho (Parameter): The rho parameters (unconstrained) for the standard
                               deviations of the Gaussian distributions of the biases.
-        softplus (nn.Softplus): A Softplus activation function used for ensuring the 
+        softplus (nn.Softplus): A Softplus activation function used for ensuring the
                                 standard deviation is positive.
 
     Methods:
         reset_parameters(): Initializes the parameters based on the number of input features.
-        forward(input): Performs the forward pass using a sampled weight and bias according 
+        forward(input): Performs the forward pass using a sampled weight and bias according
                         to their respective distributions.
-        kl_divergence(): Computes the Kullback-Leibler divergence of the layer's 
-                         parameters, which can be used as a part of the loss function 
+        kl_divergence(): Computes the Kullback-Leibler divergence of the layer's
+                         parameters, which can be used as a part of the loss function
                          to regulate the learning of the distribution parameters.
 
-    The forward computation of this layer is equivalent to a standard linear layer 
-    with sampled weights and biases. The KL divergence method returns a value that 
-    quantifies the difference between the prior and variational distributions of the 
-    layer's parameters, which encourages the learning of plausible weights and biases 
+    The forward computation of this layer is equivalent to a standard linear layer
+    with sampled weights and biases. The KL divergence method returns a value that
+    quantifies the difference between the prior and variational distributions of the
+    layer's parameters, which encourages the learning of plausible weights and biases
     while controlling complexity.
 
     """
 
     def __init__(self, in_features, out_features):
-
         super(VariationalLayer, self).__init__()
         self.in_features = in_features
         self.out_features = out_features
-        
+
         self.weight_mu = nn.Parameter(torch.Tensor(out_features, in_features))
         self.weight_rho = nn.Parameter(torch.Tensor(out_features, in_features))
         self.bias_mu = nn.Parameter(torch.Tensor(out_features))
         self.bias_rho = nn.Parameter(torch.Tensor(out_features))
-        
+
         self.softplus = nn.Softplus()
         self.reset_parameters()
-        
-    def reset_parameters(self):
 
-        std = 1. / math.sqrt(self.weight_mu.size(1))
+    def reset_parameters(self):
+        std = 1.0 / math.sqrt(self.weight_mu.size(1))
         self.weight_mu.data.uniform_(-std, std)
         self.weight_rho.data.uniform_(-std, std)
         self.bias_mu.data.uniform_(-std, std)
         self.bias_rho.data.uniform_(-std, std)
-        
-    def forward(self, input):
 
+    def forward(self, input):
         weight_sigma = torch.log1p(torch.exp(self.weight_rho))
         bias_sigma = torch.log1p(torch.exp(self.bias_rho))
-        
-        weight_epsilon = torch.normal(mean=0., std=1., size=weight_sigma.size(), device=input.device)
-        bias_epsilon = torch.normal(mean=0., std=1., size=bias_sigma.size(), device=input.device)
-        
+
+        weight_epsilon = torch.normal(
+            mean=0.0, std=1.0, size=weight_sigma.size(), device=input.device
+        )
+        bias_epsilon = torch.normal(
+            mean=0.0, std=1.0, size=bias_sigma.size(), device=input.device
+        )
+
         weight_sample = self.weight_mu + weight_epsilon * weight_sigma
         bias_sample = self.bias_mu + bias_epsilon * bias_sigma
-        
+
         output = F.linear(input, weight_sample, bias_sample)
         return output
 
     def kl_divergence(self):
-
         weight_sigma = torch.log1p(torch.exp(self.weight_rho))
         bias_sigma = torch.log1p(torch.exp(self.bias_rho))
-        
-        kl_div = -0.5 * torch.sum(1 + torch.log(weight_sigma.pow(2)) - self.weight_mu.pow(2) - weight_sigma.pow(2))
-        kl_div += -0.5 * torch.sum(1 + torch.log(bias_sigma.pow(2)) - self.bias_mu.pow(2) - bias_sigma.pow(2))
+
+        kl_div = -0.5 * torch.sum(
+            1
+            + torch.log(weight_sigma.pow(2))
+            - self.weight_mu.pow(2)
+            - weight_sigma.pow(2)
+        )
+        kl_div += -0.5 * torch.sum(
+            1 + torch.log(bias_sigma.pow(2)) - self.bias_mu.pow(2) - bias_sigma.pow(2)
+        )
 
         return kl_div
 
 
 class MultiClassClassifier(nn.Module):
 
     """
-    A neural network module for multi-class classification tasks. It 
-    consists of a sequence of layers defined by the input dimensions, number 
-    of classes, dropout rate, and sizes of hidden layers. It can be 
-    customized with different numbers and sizes of hidden layers, as well as 
-    varying dropout rates to prevent overfitting. The final output layer is 
+    A neural network module for multi-class classification tasks. It
+    consists of a sequence of layers defined by the input dimensions, number
+    of classes, dropout rate, and sizes of hidden layers. It can be
+    customized with different numbers and sizes of hidden layers, as well as
+    varying dropout rates to prevent overfitting. The final output layer is
     designed for classification among a fixed number of classes.
 
     Parameters:
         input_dim (int): Dimensionality of the input features. Defaults to 10.
         classes (int): The number of output classes for classification. Defaults to 12.
         dropout_rate (float): The dropout rate applied after each hidden layer. Defaults to 0.1.
-        hidden_layer_sizes (list of int): The sizes of each hidden layer. Defaults to a single 
+        hidden_layer_sizes (list of int): The sizes of each hidden layer. Defaults to a single
                                           hidden layer with 8 units.
 
     Attributes:
         input_dim (int): Internal storage of the input dimensionality.
         classes (int): Internal storage of the number of classes.
         dropout_rate (float): Internal storage of the dropout rate.
         hls (list of int): Internal storage of the hidden layer sizes.
-        encode (nn.Sequential): The sequential container of layers making up the encoder part 
-                                of the classifier, including linear, batch normalization, 
-                                leaky ReLU, and dropout layers. 
+        encode (nn.Sequential): The sequential container of layers making up the encoder part
+                                of the classifier, including linear, batch normalization,
+                                leaky ReLU, and dropout layers.
 
     Methods:
         encoded(x): Encodes input `x` through the sequence of layers defined in `encode`.
         forward(x): Implements the forward pass of the network, returning raw scores for each class.
         predict(x): Provides class predictions for input `x` based on the scores from the forward pass.
 
-    The class utilizes a helper function `element` to create each hidden layer or the variational 
-    layer if it is the last one. The `weights_init` function is applied to initialize weights 
+    The class utilizes a helper function `element` to create each hidden layer or the variational
+    layer if it is the last one. The `weights_init` function is applied to initialize weights
     after the model is constructed.
 
     """
 
-    def __init__(self, input_dim=10, classes=12, dropout_rate=0.1, hidden_layer_sizes=[64, 32, 16]):
+    def __init__(
+        self,
+        input_dim=10,
+        classes=12,
+        dropout_rate=0.1,
+        hidden_layer_sizes=[64, 32, 16],
+    ):
         super(MultiClassClassifier, self).__init__()
         self.input_dim = input_dim
         self.classes = classes
         self.dropout_rate = dropout_rate
         self.hls = hidden_layer_sizes
 
         def element(in_channel, out_channel, is_last=False):
@@ -323,17 +364,21 @@
             else:
                 layers = [VariationalLayer(in_channel, out_channel)]
             return layers
 
         encoder = []
         for i, size in enumerate(self.hls):
             if i == 0:
-                encoder += element(self.input_dim, size, is_last=(i==len(self.hls)-1))
+                encoder += element(
+                    self.input_dim, size, is_last=(i == len(self.hls) - 1)
+                )
             else:
-                encoder += element(self.hls[i-1], size, is_last=(i==len(self.hls)-1))
+                encoder += element(
+                    self.hls[i - 1], size, is_last=(i == len(self.hls) - 1)
+                )
 
         encoder += [nn.Linear(size, self.classes)]  # Add this line
 
         self.encode = nn.Sequential(*encoder)
         self.apply(weights_init)
 
     def encoded(self, x):
@@ -348,20 +393,19 @@
         scores = self.forward(x)
         # Get predicted class indices
         class_indices = scores.argmax(dim=1)
         return class_indices
 
 
 def predict_class_prob_nn_train(model, input_data, n_iterations=250):
-
     """
-    
-    Computes the predicted class probabilities for the given input data using the model by 
-    performing multiple forward passes. The function operates in evaluation mode and does not 
-    track gradients. It returns the mean and standard deviation of the softmax probabilities 
+
+    Computes the predicted class probabilities for the given input data using the model by
+    performing multiple forward passes. The function operates in evaluation mode and does not
+    track gradients. It returns the mean and standard deviation of the softmax probabilities
     across all iterations, providing a measure of model uncertainty.
 
     Parameters:
         model (nn.Module): The model to be used for prediction, which should already be trained.
         input_data (Tensor): The input data to be passed to the model for prediction.
         n_iterations (int): The number of forward passes to perform for prediction. Defaults to 250.
 
@@ -372,162 +416,190 @@
     """
 
     model.eval()
     output_list = []
     for i in range(n_iterations):
         with torch.no_grad():
             output = model(input_data)
-            output_list.append(torch.nn.functional.softmax(output, dim=1).detach().cpu().numpy())
+            output_list.append(
+                torch.nn.functional.softmax(output, dim=1).detach().cpu().numpy()
+            )
 
     output_list = np.array(output_list)
-    
+
     # Calculate mean and standard deviation
     prediction_mean = output_list.mean(axis=0)
     prediction_std = output_list.std(axis=0)
 
     return prediction_mean, prediction_std
 
 
-def predict_class_prob_nn(df, n_iterations=250): 
-
+def predict_class_prob_nn(df, n_iterations=250):
     """
 
-    Predicts the class probabilities, corresponding mineral names, and the maximum 
-    probability for each class using a predefined MultiClassClassifier model. This 
-    function loads a pre-trained model and its optimizer state, normalizes input 
+    Predicts the class probabilities, corresponding mineral names, and the maximum
+    probability for each class using a predefined MultiClassClassifier model. This
+    function loads a pre-trained model and its optimizer state, normalizes input
     data, and performs multiple inference iterations to compute the prediction probabilities.
 
     Parameters:
         df (DataFrame): The input DataFrame containing the oxide composition data.
-        n_iterations (int): The number of inference iterations to average over for predictions. 
+        n_iterations (int): The number of inference iterations to average over for predictions.
 
     Returns:
-        df (DataFrame): The input DataFrame with columns predict_mineral (predicted mineral names) 
-        and predict_prob (maximum probability of predicted class). 
+        df (DataFrame): The input DataFrame with columns predict_mineral (predicted mineral names)
+        and predict_prob (maximum probability of predicted class).
         probability_matrix (ndarray): The matrix of class probabilities for each sample.
 
     """
 
-    lr = 5e-3 
-    wd = 1e-3 
+    lr = 5e-3
+    wd = 1e-3
     dr = 0.1
     hls = [64, 32, 16]
 
-    oxides = ['SiO2', 'TiO2', 'Al2O3', 'FeOt', 'MnO', 'MgO', 'CaO', 'Na2O', 'K2O', 'Cr2O3']
-    device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-
-    model = MultiClassClassifier(input_dim=len(oxides), dropout_rate=dr, hidden_layer_sizes=hls).to(device)
+    oxides = [
+        "SiO2",
+        "TiO2",
+        "Al2O3",
+        "FeOt",
+        "MnO",
+        "MgO",
+        "CaO",
+        "Na2O",
+        "K2O",
+        "Cr2O3",
+    ]
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+    model = MultiClassClassifier(
+        input_dim=len(oxides), dropout_rate=dr, hidden_layer_sizes=hls
+    ).to(device)
     optimizer = torch.optim.SGD(model.parameters(), lr=lr, weight_decay=wd)
     current_dir = os.path.dirname(__file__)
-    model_path = os.path.join(current_dir, 'nn_best_model.pt') 
+    model_path = os.path.join(current_dir, "nn_best_model.pt")
 
     load_model(model, optimizer, model_path)
 
     norm_wt = norm_data_nn(df)
     input_data = torch.Tensor(norm_wt).to(device)
 
     model.eval()
     output_list = []
     for i in range(n_iterations):
         with torch.no_grad():
             output = model(input_data)
-            output_list.append(torch.nn.functional.softmax(output, dim=1).detach().cpu().numpy())
+            output_list.append(
+                torch.nn.functional.softmax(output, dim=1).detach().cpu().numpy()
+            )
 
     output_list = np.array(output_list)
     probability_matrix = output_list.mean(axis=0)
     # predict_class = np.argmax(probability_matrix, axis=1)
     # predict_prob = np.max(probability_matrix, axis=1)
     # predict_mineral = class2mineral_nn(predict_class)
 
     top_two_indices = np.argsort(probability_matrix, axis=1)[:, -2:]
-    first_predict_prob = probability_matrix[np.arange(probability_matrix.shape[0]), top_two_indices[:, 1]]
-    second_predict_prob = probability_matrix[np.arange(probability_matrix.shape[0]), top_two_indices[:, 0]]
+    first_predict_prob = probability_matrix[
+        np.arange(probability_matrix.shape[0]), top_two_indices[:, 1]
+    ]
+    second_predict_prob = probability_matrix[
+        np.arange(probability_matrix.shape[0]), top_two_indices[:, 0]
+    ]
     first_predict_mineral = class2mineral_nn(top_two_indices[:, 1])
     second_predict_mineral = class2mineral_nn(top_two_indices[:, 0])
 
-    df['Predict_Mineral'] = first_predict_mineral
-    df['Predict_Probability'] = first_predict_prob
-    df['Second_Predict_Mineral'] = second_predict_mineral
-    df['Second_Predict_Probability'] = second_predict_prob
+    df["Predict_Mineral"] = first_predict_mineral
+    df["Predict_Probability"] = first_predict_prob
+    df["Second_Predict_Mineral"] = second_predict_mineral
+    df["Second_Predict_Probability"] = second_predict_prob
 
     return df, probability_matrix
 
 
-def unique_mapping_nn(pred_class): 
-
+def unique_mapping_nn(pred_class):
     """
-    Generates a mapping of unique class codes from given and predicted class labels, 
-    considering only the classes present in both input arrays. It loads a predefined 
-    category list and mapping, encodes the 'given_class' labels into categorical codes, 
-    and creates a subset mapping for the unique classes found. It also handles unknown 
+    Generates a mapping of unique class codes from given and predicted class labels,
+    considering only the classes present in both input arrays. It loads a predefined
+    category list and mapping, encodes the 'given_class' labels into categorical codes,
+    and creates a subset mapping for the unique classes found. It also handles unknown
     classes by assigning them a code of -1 and mapping the 'Unknown' label to them.
 
     Parameters:
         pred_class (array-like): The array of predicted class labels.
 
     Returns:
         unique (ndarray): Array of unique class codes found in both given and predicted classes.
-        valid_mapping (dict): Dictionary mapping class codes to their corresponding labels, 
+        valid_mapping (dict): Dictionary mapping class codes to their corresponding labels,
         including 'Unknown' for any class code of -1.
     """
 
     _, mapping = load_minclass_nn()
     unique = np.unique(pred_class)
     valid_mapping = {key: mapping[key] for key in unique}
     if -1 in unique:
-        valid_mapping[-1] = "Unknown" 
+        valid_mapping[-1] = "Unknown"
 
     return unique, valid_mapping
 
 
-def class2mineral_nn(pred_class): 
-
+def class2mineral_nn(pred_class):
     """
 
     Translates predicted class codes into mineral names using a mapping obtained from the
-    unique classes present in the 'pred_class' array. It utilizes the 'unique_mapping_nn' 
+    unique classes present in the 'pred_class' array. It utilizes the 'unique_mapping_nn'
     function to establish the relevant class-to-mineral name mapping.
 
     Parameters:
         pred_class (array-like): The array of predicted class codes to be translated into mineral names.
 
     Returns:
         pred_mineral (ndarray): An array of mineral names corresponding to the predicted class codes.
-        
+
     """
 
     _, valid_mapping = unique_mapping_nn(pred_class)
     pred_mineral = np.array([valid_mapping[x] for x in pred_class])
 
     return pred_mineral
 
 
 def confusion_matrix_df(given_min, pred_min):
-
     """
 
-    Constructs a confusion matrix as a pandas DataFrame for easy visualization and 
-    analysis. The function first finds the unique classes and maps them to their 
-    corresponding mineral names. Then, it uses these mappings to construct the 
+    Constructs a confusion matrix as a pandas DataFrame for easy visualization and
+    analysis. The function first finds the unique classes and maps them to their
+    corresponding mineral names. Then, it uses these mappings to construct the
     confusion matrix, which compares the given and predicted classes.
 
     Parameters:
         given_class (array-like): The true class labels.
         pred_class (array-like): The predicted class labels.
 
     Returns:
-        cm_df (DataFrame): A DataFrame representing the confusion matrix, with rows 
-                           and columns labeled by the unique mineral names found in 
+        cm_df (DataFrame): A DataFrame representing the confusion matrix, with rows
+                           and columns labeled by the unique mineral names found in
                            the given and predicted class arrays.
 
     """
 
-    minerals = ['Amphibole', 'Biotite', 'Clinopyroxene', 'Garnet', 'Ilmenite', 
-                'KFeldspar', 'Magnetite', 'Muscovite', 'Olivine', 'Orthopyroxene', 
-                'Plagioclase', 'Spinel']
+    minerals = [
+        "Amphibole",
+        "Biotite",
+        "Clinopyroxene",
+        "Garnet",
+        "Ilmenite",
+        "KFeldspar",
+        "Magnetite",
+        "Muscovite",
+        "Olivine",
+        "Orthopyroxene",
+        "Plagioclase",
+        "Spinel",
+    ]
 
     # Create a confusion matrix with labels as all possible minerals
     cm_matrix = confusion_matrix(given_min, pred_min, labels=minerals)
 
     # Create a DataFrame from the confusion matrix
     cm_df = pd.DataFrame(cm_matrix, index=minerals, columns=minerals)
 
@@ -546,21 +618,30 @@
 
     # min_cat, _ = load_minclass_nn()
     # cm_df = pd.DataFrame(cm_matrix, index=min_cat, columns=min_cat)
 
     return cm_df
 
 
-def train_nn(model, optimizer, train_loader, valid_loader, n_epoch, criterion, kl_weight_decay, kl_decay_epochs=750, patience=50):
-
-    """
-
-    Trains a neural network model using the provided data loaders, optimizer, and loss criterion. It incorporates KL divergence 
-    into the loss to enable learning in a variational framework, with the KL weight increasing each epoch until a maximum value 
-    is reached. The function includes an early stopping mechanism that terminates training if validation loss does not improve 
+def train_nn(
+    model,
+    optimizer,
+    train_loader,
+    valid_loader,
+    n_epoch,
+    criterion,
+    kl_weight_decay,
+    kl_decay_epochs=750,
+    patience=50,
+):
+    """
+
+    Trains a neural network model using the provided data loaders, optimizer, and loss criterion. It incorporates KL divergence
+    into the loss to enable learning in a variational framework, with the KL weight increasing each epoch until a maximum value
+    is reached. The function includes an early stopping mechanism that terminates training if validation loss does not improve
     for a specified number of consecutive epochs.
 
     Parameters:
         model (nn.Module): The neural network model to train.
         optimizer (Optimizer): The optimization algorithm used to update model weights.
         train_loader (DataLoader): The DataLoader containing the training data.
         valid_loader (DataLoader): The DataLoader containing the validation data.
@@ -576,19 +657,19 @@
         avg_train_loss (list): The list of average training losses per epoch.
         avg_valid_loss (list): The list of average validation losses per epoch.
         best_valid_loss (float): The best validation loss observed during training.
         best_model_state (dict): The state dictionary of the model at the point of the best validation loss.
 
     """
 
-    device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')    
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     avg_train_loss = []
     avg_valid_loss = []
-    best_valid_loss = float('inf')
+    best_valid_loss = float("inf")
     best_model_state = None
     patience_counter = 0
 
     kl_weight = 0.0  # Initial kl_weight
 
     for epoch in range(n_epoch):
         model.train()
@@ -597,30 +678,30 @@
         for i, (data, labels) in enumerate(train_loader):
             x = data.to(device)
             y = labels.to(device)
             train_output = model(x)
             loss = criterion(train_output, y)
 
             # Add KL divergence with weight decay
-            kl_div = 0.
+            kl_div = 0.0
             # kl_weight = min(kl_weight + (kl_weight_decay * (epoch // kl_decay_epochs)), 1)
             kl_weight_increment = kl_weight_decay / kl_decay_epochs
             kl_weight = min(kl_weight + kl_weight_increment, 1)
 
             for module in model.modules():
                 if isinstance(module, VariationalLayer):
                     kl_div += module.kl_divergence()
             loss += kl_weight * kl_div / len(train_loader.dataset)
 
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
             train_loss.append(loss.detach().item())
-        
+
         # Validation
         model.eval()
         valid_loss = []
         with torch.no_grad():
             for i, (data, labels) in enumerate(valid_loader):
                 x = data.to(device)
                 y = labels.to(device)
@@ -629,43 +710,55 @@
                 valid_loss.append(loss.detach().item())
 
         # Logging
         avg_train = sum(train_loss) / len(train_loss)
         avg_valid = sum(valid_loss) / len(valid_loss)
         avg_train_loss.append(avg_train)
         avg_valid_loss.append(avg_valid)
-        
+
         training_time = time.time() - t
- 
-        print(f'[{epoch+1:03}/{n_epoch:03}] train_loss: {avg_train:.6f}, valid_loss: {avg_valid:.6f}, time: {training_time:.2f} s')
+
+        print(
+            f"[{epoch+1:03}/{n_epoch:03}] train_loss: {avg_train:.6f}, valid_loss: {avg_valid:.6f}, time: {training_time:.2f} s"
+        )
 
         # Early stopping
         if avg_valid < best_valid_loss:
             best_valid_loss = avg_valid
             patience_counter = 0
-            best_model_state = copy.deepcopy(model.state_dict())  # Save the best model weights
+            best_model_state = copy.deepcopy(
+                model.state_dict()
+            )  # Save the best model weights
 
         else:
             patience_counter += 1
             if patience_counter >= patience:
-                print(f"Validation loss hasn't improved for {patience} epochs. Stopping early.")
+                print(
+                    f"Validation loss hasn't improved for {patience} epochs. Stopping early."
+                )
                 break
 
-    return train_output, valid_output, avg_train_loss, avg_valid_loss, best_valid_loss, best_model_state
+    return (
+        train_output,
+        valid_output,
+        avg_train_loss,
+        avg_valid_loss,
+        best_valid_loss,
+        best_model_state,
+    )
 
 
 def neuralnetwork(df, hls_list, kl_weight_decay_list, lr, wd, dr, ep, n, balanced):
-
     """
 
-    Trains a neural network with various configurations of hidden layer sizes and KL weight 
-    decay parameters to find the best model for classifying minerals based on their oxide 
-    composition. It normalizes input data, balances the dataset if required, initializes 
-    the model and optimizer, and performs training and validation. The best performing 
-    model's parameters are saved, along with training and validation losses, and prediction 
+    Trains a neural network with various configurations of hidden layer sizes and KL weight
+    decay parameters to find the best model for classifying minerals based on their oxide
+    composition. It normalizes input data, balances the dataset if required, initializes
+    the model and optimizer, and performs training and validation. The best performing
+    model's parameters are saved, along with training and validation losses, and prediction
     reports.
 
     Parameters:
         df (DataFrame): The input DataFrame with mineral composition data and labels.
         hls_list (list of list of int): List of configurations for hidden layer sizes.
         kl_weight_decay_list (list of float): List of KL weight decay values to try during training.
         lr (float): Learning rate for the optimizer.
@@ -673,125 +766,183 @@
         dr (float): Dropout rate for the model.
         ep (int): Number of epochs to train.
         n (float): Test size fraction or absolute number for splitting the dataset.
         balanced (bool): Whether to balance the dataset or not.
 
     Returns:
         best_model_state (dict): The state dictionary of the best performing model.
-        
+
     """
 
-    path_beg = os.getcwd() + '/'
-    output_dir = ["parametermatrix_neuralnetwork"] 
+    path_beg = os.getcwd() + "/"
+    output_dir = ["parametermatrix_neuralnetwork"]
     for ii in range(len(output_dir)):
         if not os.path.exists(path_beg + output_dir[ii]):
             os.makedirs(path_beg + output_dir[ii], exist_ok=True)
 
-    device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-    wt = df[['SiO2', 'TiO2', 'Al2O3', 'FeOt', 'MnO', 'MgO', 'CaO', 'Na2O', 'K2O', 'Cr2O3']].fillna(0)
+    wt = df[
+        ["SiO2", "TiO2", "Al2O3", "FeOt", "MnO", "MgO", "CaO", "Na2O", "K2O", "Cr2O3"]
+    ].fillna(0)
 
     ss = StandardScaler()
     array_norm = ss.fit_transform(wt)
 
-    code = pd.Categorical(df['Mineral']).codes
-    cat_lab = pd.Categorical(df['Mineral'])
+    code = pd.Categorical(df["Mineral"]).codes
+    cat_lab = pd.Categorical(df["Mineral"])
 
     # Split the dataset into train and test sets
-    train_x, valid_x, train_y, valid_y = train_test_split(array_norm, code, test_size=n, stratify=code, random_state=42)
+    train_x, valid_x, train_y, valid_y = train_test_split(
+        array_norm, code, test_size=n, stratify=code, random_state=42
+    )
 
-    if balanced == True: 
+    if balanced == True:
         train_x, train_y = balance(train_x, train_y)
 
     # Define datasets to be used with PyTorch - see autoencoder file for details
     feature_dataset = LabelDataset(train_x, train_y)
     valid_dataset = LabelDataset(valid_x, valid_y)
 
     mapping = dict(zip(code, cat_lab))
     sort_mapping = dict(sorted(mapping.items(), key=lambda item: item[0]))
 
     # Autoencoder params:
     lr = lr
-    wd = wd 
+    wd = wd
     dr = dr
     epochs = ep
     batch_size = 256
     input_size = len(feature_dataset.__getitem__(0)[0])
 
     best_hidden_layer_size = None
     best_kl_weight_decay = None
     best_model_state = None
-    best_valid_loss = float('inf')
+    best_valid_loss = float("inf")
 
     # Define data loaders
     feature_loader = DataLoader(feature_dataset, batch_size=batch_size, shuffle=True)
     valid_loader = DataLoader(valid_dataset, batch_size=batch_size, shuffle=True)
-    np.savez('parametermatrix_neuralnetwork/' + 'best_model_nn_features.npz', feature_loader=feature_loader, valid_loader=valid_loader)
+    np.savez(
+        "parametermatrix_neuralnetwork/" + "best_model_nn_features.npz",
+        feature_loader=feature_loader,
+        valid_loader=valid_loader,
+    )
 
     train_losses_dict = {}
     valid_losses_dict = {}
 
     for hls in hls_list:
         for kl_weight_decay in kl_weight_decay_list:
-
-            print(f"Training with KL weight decay: {kl_weight_decay} and hidden layer sizes: {hls}")
+            print(
+                f"Training with KL weight decay: {kl_weight_decay} and hidden layer sizes: {hls}"
+            )
 
             # Initialize model
-            model = MultiClassClassifier(input_dim=input_size, dropout_rate=dr, hidden_layer_sizes=hls).to(device)
+            model = MultiClassClassifier(
+                input_dim=input_size, dropout_rate=dr, hidden_layer_sizes=hls
+            ).to(device)
 
             # Define loss function and optimizer
             criterion = nn.CrossEntropyLoss()
             optimizer = torch.optim.SGD(model.parameters(), lr=lr, weight_decay=wd)
 
             # Train model and get the best test loss and model state
-            train_output, valid_output, avg_train_loss, avg_valid_loss, current_best_valid_loss, current_best_model_state = train_nn(model, optimizer, feature_loader, valid_loader, epochs, criterion, kl_weight_decay=kl_weight_decay)
+            (
+                train_output,
+                valid_output,
+                avg_train_loss,
+                avg_valid_loss,
+                current_best_valid_loss,
+                current_best_model_state,
+            ) = train_nn(
+                model,
+                optimizer,
+                feature_loader,
+                valid_loader,
+                epochs,
+                criterion,
+                kl_weight_decay=kl_weight_decay,
+            )
 
             if current_best_valid_loss < best_valid_loss:
                 best_valid_loss = current_best_valid_loss
                 best_kl_weight_decay = kl_weight_decay
                 best_hidden_layer_size = hls
                 best_model_state = current_best_model_state
 
             train_losses_dict[(kl_weight_decay, tuple(hls))] = avg_train_loss
             valid_losses_dict[(kl_weight_decay, tuple(hls))] = avg_valid_loss
 
     # Create a new model with the best model state
-    best_model = MultiClassClassifier(input_dim=input_size, dropout_rate=dr, hidden_layer_sizes=best_hidden_layer_size)
+    best_model = MultiClassClassifier(
+        input_dim=input_size, dropout_rate=dr, hidden_layer_sizes=best_hidden_layer_size
+    )
     best_model.load_state_dict(best_model_state)
     best_model.eval()
 
     # Perform predictions on the test dataset using the best model
     with torch.no_grad():
         valid_predictions = best_model(torch.Tensor(valid_x))
         train_predictions = best_model(torch.Tensor(train_x))
         valid_pred_y = valid_predictions.argmax(dim=1).cpu().numpy()
         train_pred_y = train_predictions.argmax(dim=1).cpu().numpy()
 
     # Calculate classification metrics for the test dataset
-    valid_report = classification_report(valid_y, valid_pred_y, target_names=list(sort_mapping.values()), zero_division=0, output_dict=True)
-    train_report = classification_report(train_y, train_pred_y, target_names=list(sort_mapping.values()), zero_division=0, output_dict=True) # output_dict=True
+    valid_report = classification_report(
+        valid_y,
+        valid_pred_y,
+        target_names=list(sort_mapping.values()),
+        zero_division=0,
+        output_dict=True,
+    )
+    train_report = classification_report(
+        train_y,
+        train_pred_y,
+        target_names=list(sort_mapping.values()),
+        zero_division=0,
+        output_dict=True,
+    )  # output_dict=True
 
     # Print the best kl_weight_decay value and test report
     print("Best kl_weight_decay:", best_kl_weight_decay)
     print("Best best_hidden_layer_size:", best_hidden_layer_size)
 
     # Save the best model and other relevant information
-    model_path = 'parametermatrix_neuralnetwork/best_model.pt'
+    model_path = "parametermatrix_neuralnetwork/best_model.pt"
     save_model_nn(optimizer, best_model_state, model_path)
 
-    train_pred_mean, train_pred_std = predict_class_prob_nn_train(model, feature_dataset.x)
-    valid_pred_mean, valid_pred_std = predict_class_prob_nn_train(model, valid_dataset.x)
+    train_pred_mean, train_pred_std = predict_class_prob_nn_train(
+        model, feature_dataset.x
+    )
+    valid_pred_mean, valid_pred_std = predict_class_prob_nn_train(
+        model, valid_dataset.x
+    )
 
     # Get the most probable classes
     train_pred_y = np.argmax(train_pred_mean, axis=1)
     valid_pred_y = np.argmax(valid_pred_mean, axis=1)
 
-    np.savez('parametermatrix_neuralnetwork/best_model_data.npz', best_hidden_layer_size=best_hidden_layer_size, best_kl_weight_decay=best_kl_weight_decay, 
-             valid_report=valid_report, train_report=train_report,
-             train_y=train_y, valid_y=valid_y, train_pred_y=train_pred_y, valid_pred_y=valid_pred_y, 
-             train_pred_mean=train_pred_mean, train_pred_std=train_pred_std, valid_pred_mean=valid_pred_mean, valid_pred_std=valid_pred_std)
+    np.savez(
+        "parametermatrix_neuralnetwork/best_model_data.npz",
+        best_hidden_layer_size=best_hidden_layer_size,
+        best_kl_weight_decay=best_kl_weight_decay,
+        valid_report=valid_report,
+        train_report=train_report,
+        train_y=train_y,
+        valid_y=valid_y,
+        train_pred_y=train_pred_y,
+        valid_pred_y=valid_pred_y,
+        train_pred_mean=train_pred_mean,
+        train_pred_std=train_pred_std,
+        valid_pred_mean=valid_pred_mean,
+        valid_pred_std=valid_pred_std,
+    )
 
     # Save the train and test losses
-    np.savez('parametermatrix_neuralnetwork/best_model_losses.npz', train_losses=train_losses_dict, valid_losses=valid_losses_dict)
+    np.savez(
+        "parametermatrix_neuralnetwork/best_model_losses.npz",
+        train_losses=train_losses_dict,
+        valid_losses=valid_losses_dict,
+    )
 
     return best_model_state
-
```

### Comparing `mineralML-0.0.0.5/src/mineralML/unsupervised.py` & `mineralML-0.0.0.6/src/mineralML/unsupervised.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,164 +4,209 @@
 import math
 import time
 import copy
 
 import numpy as np
 import pandas as pd
 
+from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import StandardScaler
 
 import torch
 import torch.nn as nn
 from torch.nn.modules.activation import LeakyReLU
 from torch.utils.data import DataLoader
+from scipy.special import softmax
 
-from hdbscan.flat import (HDBSCAN_flat, approximate_predict_flat)
+from hdbscan.flat import HDBSCAN_flat, approximate_predict_flat
 
 from matplotlib import pyplot as plt
 import matplotlib.colors as mcolors
 import matplotlib.cm as mcm
 
 from mineralML.core import *
 
-# %% 
+# %%
 
 
 def prep_df_ae(df):
-
     """
 
-    Prepares a DataFrame for analysis by performing data cleaning specific to mineralogical data. 
-    It filters the DataFrame for selected minerals, handles missing values, and separates the data 
+    Prepares a DataFrame for analysis by performing data cleaning specific to mineralogical data.
+    It filters the DataFrame for selected minerals, handles missing values, and separates the data
     into two DataFrames: one that includes specified minerals and another that excludes them.
-    The function defines a list of oxide column names and minerals to include and exclude. It drops 
-    rows where the specified oxides and 'Mineral' column have fewer than six non-NaN values. 
+    The function defines a list of oxide column names and minerals to include and exclude. It drops
+    rows where the specified oxides and 'Mineral' column have fewer than six non-NaN values.
 
     Parameters:
         df (DataFrame): The input DataFrame containing mineral composition data along with 'Mineral' column.
 
     Returns:
         df_in (DataFrame): A DataFrame with rows including only the specified minerals and 'NaN' filled with zero.
         df_ex (DataFrame): A DataFrame with rows excluding the specified minerals and 'NaN' filled with zero.
-    
+
     """
 
     if "FeO" in df.columns and "FeOt" not in df.columns:
-        raise ValueError("No 'FeOt' column found. You have a 'FeO' column. mineralML only recognizes 'FeOt' as a column. Please convert to FeOt.")
+        raise ValueError(
+            "No 'FeOt' column found. You have a 'FeO' column. mineralML only recognizes 'FeOt' as a column. Please convert to FeOt."
+        )
     if "Fe2O3" in df.columns and "FeOt" not in df.columns:
-        raise ValueError("No 'FeOt' column found. You have a 'Fe2O3' column. mineralML only recognizes 'FeOt' as a column. Please convert to FeOt.")
-
-    oxidesandmin = ['SiO2', 'TiO2', 'Al2O3', 'FeOt', 'MnO', 'MgO', 'CaO', 'Na2O', 'K2O', 'Cr2O3', 'Mineral']
-    include_minerals = ['Amphibole', 'Apatite', 'Biotite', 'Clinopyroxene', 'Garnet', 'Ilmenite', 
-                        'KFeldspar', 'Magnetite', 'Muscovite', 'Olivine', 'Orthopyroxene', 
-                        'Plagioclase', 'Quartz', 'Rutile', 'Spinel', 'Tourmaline', 'Zircon']
+        raise ValueError(
+            "No 'FeOt' column found. You have a 'Fe2O3' column. mineralML only recognizes 'FeOt' as a column. Please convert to FeOt."
+        )
+
+    oxidesandmin = [
+        "SiO2",
+        "TiO2",
+        "Al2O3",
+        "FeOt",
+        "MnO",
+        "MgO",
+        "CaO",
+        "Na2O",
+        "K2O",
+        "Cr2O3",
+        "Mineral",
+    ]
+    include_minerals = [
+        "Amphibole",
+        "Apatite",
+        "Biotite",
+        "Clinopyroxene",
+        "Garnet",
+        "Ilmenite",
+        "KFeldspar",
+        "Magnetite",
+        "Muscovite",
+        "Olivine",
+        "Orthopyroxene",
+        "Plagioclase",
+        "Quartz",
+        "Rutile",
+        "Spinel",
+        "Tourmaline",
+        "Zircon",
+    ]
     # df.dropna(subset=oxidesandmin, thresh=5, inplace=True)
-    df_in = df[df['Mineral'].isin(include_minerals)]
-    df_ex = df[~df['Mineral'].isin(include_minerals)]
+    df_in = df[df["Mineral"].isin(include_minerals)]
+    df_ex = df[~df["Mineral"].isin(include_minerals)]
 
     df_in = df_in[oxidesandmin].fillna(0)
 
     df_in = df_in.reset_index(drop=True)
     df_ex = df_ex.reset_index(drop=True)
 
     return df_in, df_ex
 
 
 def norm_data_ae(df):
-
     """
 
-    Normalizes the oxide composition data in the input DataFrame using a predefined StandardScaler. 
-    It ensures that the dataframe has been preprocessed accordingly before applying the transformation. 
-    The function expects that the scaler is already fitted and available for use as defined in the 
+    Normalizes the oxide composition data in the input DataFrame using a predefined StandardScaler.
+    It ensures that the dataframe has been preprocessed accordingly before applying the transformation.
+    The function expects that the scaler is already fitted and available for use as defined in the
     'load_scaler' function.
 
     Parameters:
         df (DataFrame): The input DataFrame containing the oxide composition data.
 
     Returns:
         array_x (ndarray): An array of the transformed oxide composition data.
 
     """
 
-    oxides = ['SiO2', 'TiO2', 'Al2O3', 'FeOt', 'MnO', 'MgO', 'CaO', 'Na2O', 'K2O', 'Cr2O3']
-    mean, std = load_scaler('scaler_ae.npz')
+    oxides = [
+        "SiO2",
+        "TiO2",
+        "Al2O3",
+        "FeOt",
+        "MnO",
+        "MgO",
+        "CaO",
+        "Na2O",
+        "K2O",
+        "Cr2O3",
+    ]
+    mean, std = load_scaler("scaler_ae.npz")
 
     if df[oxides].isnull().any().any():
         df, _ = prep_df_ae(df)
-    else: 
-        df = df 
+    else:
+        df = df
 
     scaled_df = df[oxides].copy()
 
-    for col in df[oxides].columns: 
+    for col in df[oxides].columns:
         scaled_df[col] = (df[col] - mean[col]) / std[col]
 
     array_x = scaled_df.to_numpy()
-    
-    return array_x
 
+    return array_x
 
-def feature_normalisation(feature, return_params = False, mean_norm = True):
 
+def feature_normalisation(feature, return_params=False, mean_norm=True):
     """
     Function to perform mean normalisation on the dataset passed to it.
-    
-    Parameters: 
+
+    Parameters:
         feature (numpy array): Features to be normalised.
         return_params (boolean, optional): Set to True if parameters used for mean normalisation
         are to be returned for each feature.
-                            
-    Returns: 
+
+    Returns:
         norm (numpy array): Mean normalised features.
         params (list of numpy arrays): Only returned if set to True above; list of parameters
         used for the mean normalisation as derived from the features (i.e., mean, min, and max).
     """
-    
+
     params = []
-    
+
     norm = np.zeros_like(feature)
-    
+
     if len(feature.shape) == 2:
         for i in range(feature.shape[1]):
             if mean_norm == True:
-                temp_mean = feature[:,i].mean()
+                temp_mean = feature[:, i].mean()
             elif mean_norm == False:
                 temp_mean = 0
             else:
                 raise ValueError("Mean_norm must be boolean")
-            norm[:,i] = (feature[:,i] - temp_mean) / (feature[:,i].max() - feature[:,i].min())
-            params.append(np.asarray([temp_mean,feature[:,i].min(),feature[:,i].max()]))
-    
+            norm[:, i] = (feature[:, i] - temp_mean) / (
+                feature[:, i].max() - feature[:, i].min()
+            )
+            params.append(
+                np.asarray([temp_mean, feature[:, i].min(), feature[:, i].max()])
+            )
+
     elif len(feature.shape) == 1:
         if mean_norm == True:
             temp_mean = feature[:].mean()
         elif mean_norm == False:
-                temp_mean = 0
+            temp_mean = 0
         else:
             raise ValueError("Mean_norm must be boolean")
         norm[:] = (feature[:] - temp_mean) / (feature.max() - feature.min())
-        params.append(np.asarray([temp_mean,feature[:].min(),feature[:].max()]))
-        
+        params.append(np.asarray([temp_mean, feature[:].min(), feature[:].max()]))
+
     else:
         raise ValueError("Feature array must be either 1D or 2D numpy array.")
-        
-    
+
     if return_params == True:
         return norm, params
     else:
         return norm
 
 
 class Autoencoder(nn.Module):
 
     """
 
-    A neural network module for dimensionality reduction and feature learning, 
-    implementing an autoencoder architecture. It compresses input data into a 
+    A neural network module for dimensionality reduction and feature learning,
+    implementing an autoencoder architecture. It compresses input data into a
     lower-dimensional latent space and then reconstructs it back.
 
     Parameters:
         input_dim (int): Dimension of the input data. Default: 10.
         latent_dim (int): Dimension of the latent space. Default: 2.
         hidden_layer_sizes (tuple of ints): Sizes of the hidden layers in the encoder
                                             and decoder. Default: (256, 64, 16).
@@ -174,15 +219,15 @@
     Methods:
         encoded(self, x): Encodes input data `x` to the latent space.
         decoded(self, x): Decodes data `x` from the latent space to the input space.
         forward(self, x): Defines the forward pass of the autoencoder.
 
     """
 
-    def __init__(self,input_dim = 10, latent_dim = 2, hidden_layer_sizes=(256, 64, 16)):
+    def __init__(self, input_dim=10, latent_dim=2, hidden_layer_sizes=(256, 64, 16)):
         super(Autoencoder, self).__init__()
         self.input_dim = input_dim
         self.latent_dim = latent_dim
         self.hls = hidden_layer_sizes
 
         def element(in_channel, out_channel):
             return [
@@ -195,44 +240,44 @@
         for i in range(len(self.hls) - 1):
             encoder += element(self.hls[i], self.hls[i + 1])
         encoder += [nn.Linear(self.hls[-1], latent_dim)]
 
         decoder = element(latent_dim, self.hls[-1])
         for i in range(len(self.hls) - 1, 0, -1):
             decoder += element(self.hls[i], self.hls[i - 1])
-        decoder += [nn.Linear(self.hls[0], self.input_dim)] # nn.Softmax()]
+        decoder += [nn.Linear(self.hls[0], self.input_dim)]  # nn.Softmax()]
 
         self.encode = nn.Sequential(*encoder)
         self.decode = nn.Sequential(*decoder)
 
         self.apply(weights_init)
 
     def encoded(self, x):
-        #encodes data to latent space
+        # encodes data to latent space
         return self.encode(x)
 
     def decoded(self, x):
-        #decodes latent space data to 'real' space
+        # decodes latent space data to 'real' space
         return self.decode(x)
 
     def forward(self, x):
         en = self.encoded(x)
         de = self.decoded(en)
         return de
 
 
 class Tanh_Autoencoder(nn.Module):
 
     """
 
-    A neural network module implementing an autoencoder with Tanh activation functions. 
-    This class is designed for dimensionality reduction and feature learning, 
+    A neural network module implementing an autoencoder with Tanh activation functions.
+    This class is designed for dimensionality reduction and feature learning,
     encoding input data into a lower-dimensional latent space and reconstructing it.
 
-    The architecture uses Tanh activation functions in each layer, which can provide 
+    The architecture uses Tanh activation functions in each layer, which can provide
     smoother gradients and potentially better convergence in some cases.
 
     Parameters:
         input_dim (int): Dimension of the input data. Default: 10.
         latent_dim (int): Dimension of the latent space. Default: 2.
         hidden_layer_sizes (tuple of ints): Sizes of the hidden layers in the encoder
                                             and decoder. Default: (256, 64, 16).
@@ -244,20 +289,20 @@
 
     Methods:
         encoded(self, x): Encodes input data `x` to the latent space.
         decoded(self, x): Decodes data `x` from the latent space back to the input space.
         forward(self, x): Defines the forward pass of the autoencoder.
 
     Note:
-        This autoencoder uses a Tanh activation function in each layer 
+        This autoencoder uses a Tanh activation function in each layer
         for both the encoder and the decoder.
 
     """
 
-    def __init__(self,input_dim = 10, latent_dim = 2, hidden_layer_sizes=(256, 64, 16)):
+    def __init__(self, input_dim=10, latent_dim=2, hidden_layer_sizes=(256, 64, 16)):
         super(Tanh_Autoencoder, self).__init__()
         self.input_dim = input_dim
         self.latent_dim = latent_dim
         self.hls = hidden_layer_sizes
 
         def element(in_channel, out_channel):
             return [
@@ -270,39 +315,47 @@
         for i in range(len(self.hls) - 1):
             encoder += element(self.hls[i], self.hls[i + 1])
         encoder += [nn.Linear(self.hls[-1], latent_dim)]
 
         decoder = element(latent_dim, self.hls[-1])
         for i in range(len(self.hls) - 1, 0, -1):
             decoder += element(self.hls[i], self.hls[i - 1])
-        decoder += [nn.Linear(self.hls[0], self.input_dim)] # nn.Softmax()]
+        decoder += [nn.Linear(self.hls[0], self.input_dim)]  # nn.Softmax()]
 
         self.encode = nn.Sequential(*encoder)
         self.decode = nn.Sequential(*decoder)
 
         self.apply(weights_init)
 
     def encoded(self, x):
-        #encodes data to latent space
+        # encodes data to latent space
         return self.encode(x)
 
     def decoded(self, x):
-        #decodes latent space data to 'real' space
+        # decodes latent space data to 'real' space
         return self.decode(x)
 
     def forward(self, x):
         en = self.encoded(x)
         de = self.decoded(en)
         return de
 
 
-def train(model, optimizer, train_loader, valid_loader, n_epoch, criterion, patience=10, min_delta=0.0005):
-    
+def train(
+    model,
+    optimizer,
+    train_loader,
+    valid_loader,
+    n_epoch,
+    criterion,
+    patience=10,
+    min_delta=0.0005,
+):
     """
-    
+
     Trains a given model using specified data loaders, optimizer, and loss criterion.
 
     The function performs training for a fixed number of epochs and evaluates the model
     on validation data at the end of each epoch. It also implements early stopping based
     on validation loss improvement.
 
     Parameters:
@@ -318,19 +371,19 @@
                                      Default: 0.0005.
 
     Returns:
         tuple: A tuple containing two lists: average training loss per epoch and average validation loss per epoch.
 
     """
 
-    device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')    
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     avg_train_loss = []
     avg_valid_loss = []
 
-    best_valid_loss = float('inf')
+    best_valid_loss = float("inf")
     patience_counter = 0
 
     for epoch in range(n_epoch):
         # Training
         model.train()
         t = time.time()
         train_loss = []
@@ -340,56 +393,59 @@
             loss = criterion(x_recon, x)
 
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
             train_loss.append(loss.detach().item())
-        
+
         # Testing
         model.eval()
         valid_loss = []
         for i, test in enumerate(valid_loader):
             x = test.to(device)
             x_recon = model(x)
             loss = criterion(x_recon, x)
             valid_loss.append(loss.detach().item())
-            
+
         # Logging
         avg_loss = sum(train_loss) / len(train_loss)
         avg_valid = sum(valid_loss) / len(valid_loss)
         avg_train_loss.append(avg_loss)
         avg_valid_loss.append(avg_valid)
 
         training_time = time.time() - t
-        
-        print(f'[{epoch+1:03}/{n_epoch:03}] train_loss: {avg_loss:.6f}, valid_loss: {avg_valid:.6f}, time: {training_time:.2f} s')
+
+        print(
+            f"[{epoch+1:03}/{n_epoch:03}] train_loss: {avg_loss:.6f}, valid_loss: {avg_valid:.6f}, time: {training_time:.2f} s"
+        )
 
         # Early stopping
         valid_loss_improvement = best_valid_loss - avg_valid
         if valid_loss_improvement > min_delta:
             best_valid_loss = avg_valid
             patience_counter = 0
         else:
             patience_counter += 1
             if patience_counter >= patience:
-                print(f"Test loss hasn't improved significantly for {patience} epochs. Stopping early.")
+                print(
+                    f"Test loss hasn't improved significantly for {patience} epochs. Stopping early."
+                )
                 break
 
     return avg_train_loss, avg_valid_loss
 
 
 def autoencode(df, name, AE_Model, hidden_layer_sizes, epochs):
-
     """
 
     Trains an autoencoder on a given dataset and visualizes the latent space representation.
 
-    This function preprocesses the dataset, splits it into training and validation sets, 
-    initializes an autoencoder model, and trains it. The latent space representation of the 
+    This function preprocesses the dataset, splits it into training and validation sets,
+    initializes an autoencoder model, and trains it. The latent space representation of the
     entire dataset is then visualized, and the model parameters are saved.
 
     Parameters:
         df (pd.DataFrame): Input dataset containing the features and mineral labels.
         name (str): Name to be used for saving outputs (plots, model parameters, etc.).
         AE_Model (nn.Module): Autoencoder model class to be instantiated.
         hidden_layer_sizes (tuple of ints): Sizes of the hidden layers in the autoencoder.
@@ -398,296 +454,372 @@
     Returns:
         np.ndarray: Latent space representation of the entire dataset.
 
     """
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-    oxides = ['SiO2', 'TiO2', 'Al2O3', 'FeOt', 'MnO', 'MgO', 'CaO', 'Na2O', 'K2O', 'Cr2O3']
+    oxides = [
+        "SiO2",
+        "TiO2",
+        "Al2O3",
+        "FeOt",
+        "MnO",
+        "MgO",
+        "CaO",
+        "Na2O",
+        "K2O",
+        "Cr2O3",
+    ]
 
-    wt = df[oxides].fillna(0)
+    # wt = df[oxides].fillna(0)
+    wt = df[oxides].fillna(1e-4)
     wt = wt.to_numpy()
 
-    #perform z-score normalisation
+    # perform z-score normalisation
     ss = StandardScaler()
     array_norm = ss.fit_transform(wt)
 
     # #split the dataset into train and test sets
-    train_data, valid_data = train_valid_split(array_norm, valid_size=0.1, stratify = df['Mineral'], random_state=42)
+    # train_data, valid_data = train_test_split(array_norm, test_size=0.1, stratify = df['Mineral'], random_state=42)
+    train_data, valid_data = train_test_split(
+        array_norm, test_size=0.2, stratify=df["Mineral"], random_state=42
+    )
 
-    #define datasets to be used with PyTorch - see autoencoder file for details
+    # define datasets to be used with PyTorch - see autoencoder file for details
     feature_dataset = FeatureDataset(train_data)
-    valid_dataset = FeatureDataset(valid_data)   
+    valid_dataset = FeatureDataset(valid_data)
 
-    #autoencoder params:
+    # autoencoder params:
     lr = 5e-4
-    wd = 0
+    wd = 0.005
     batch_size = 256
     epochs = epochs
     input_size = feature_dataset.__getitem__(0).size(0)
 
-    #define data loaders
-    feature_loader = DataLoader(feature_dataset, batch_size=batch_size,shuffle=True)
-    valid_loader = DataLoader(valid_dataset, batch_size=batch_size,shuffle=True)
-    np.savez('parametermatrix_autoencoder/' + name + '_features.npz', feature_loader = feature_loader, valid_loader = valid_loader)
-
-    #define model
-    model = AE_Model(input_dim=input_size, hidden_layer_sizes = hidden_layer_sizes).to(device)
+    # define data loaders
+    feature_loader = DataLoader(feature_dataset, batch_size=batch_size, shuffle=True)
+    valid_loader = DataLoader(valid_dataset, batch_size=batch_size, shuffle=True)
+    np.savez(
+        "parametermatrix_autoencoder/" + name + "_features.npz",
+        feature_loader=feature_loader,
+        valid_loader=valid_loader,
+    )
+
+    # define model
+    model = AE_Model(input_dim=input_size, hidden_layer_sizes=hidden_layer_sizes).to(
+        device
+    )
 
-    #use ADAM optimizer with mean squared error loss function
-    optimizer = torch.optim.Adam(model.parameters(), lr=lr, weight_decay=wd) 
+    # use ADAM optimizer with mean squared error loss function
+    optimizer = torch.optim.Adam(model.parameters(), lr=lr, weight_decay=wd)
     criterion = nn.MSELoss()
 
-    #train model using pre-defined function
-    train_loss, valid_loss = train(model, optimizer, feature_loader, valid_loader, epochs, criterion)
-    np.savez('parametermatrix_autoencoder/' + name + '_tanh_loss.npz', train_loss = train_loss, valid_loss = valid_loss)
-    
-    # fig, ax = plt.subplots(1, 2, figsize = (16, 8))
-    # ax = ax.flatten()
-    # ax[0].plot(np.linspace(1, len(train_loss), len(train_loss)), train_loss, '.-', label = 'Train Loss')
-    # ax[0].plot(np.linspace(1, len(train_loss), len(train_loss)), valid_loss, '.-', label = 'Test Loss')
-    # ax[0].set_xlabel("Epochs")
-    # ax[0].set_ylabel("Loss")
-    # ax[0].legend(prop={'size': 10})
+    # train model using pre-defined function
+    train_loss, valid_loss = train(
+        model, optimizer, feature_loader, valid_loader, epochs, criterion
+    )
+    np.savez(
+        "parametermatrix_autoencoder/" + name + "_tanh_loss.npz",
+        train_loss=train_loss,
+        valid_loss=valid_loss,
+    )
+
+    fig, ax = plt.subplots(1, 2, figsize=(16, 8))
+    ax = ax.flatten()
+    ax[0].plot(
+        np.linspace(1, len(train_loss), len(train_loss)),
+        train_loss,
+        ".-",
+        label="Train Loss",
+    )
+    ax[0].plot(
+        np.linspace(1, len(train_loss), len(train_loss)),
+        valid_loss,
+        ".-",
+        label="Test Loss",
+    )
+    ax[0].set_xlabel("Epochs")
+    ax[0].set_ylabel("Loss")
+    ax[0].legend(prop={"size": 10})
 
     # #transform entire dataset to latent space
-    # z = getLatent(model, array_norm)
+    z = getLatent(model, array_norm)
 
-    # phase = np.array(['Amphibole', 'Apatite', 'Biotite', 'Clinopyroxene', 
-    #     'Garnet', 'Ilmenite', 'KFeldspar', 'Magnetite', 'Muscovite', 'Olivine', 
+    # phase = np.array(['Amphibole', 'Apatite', 'Biotite', 'Clinopyroxene',
+    #     'Garnet', 'Ilmenite', 'KFeldspar', 'Magnetite', 'Muscovite', 'Olivine',
     #     'Orthopyroxene', 'Plagioclase', 'Quartz', 'Rutile', 'Spinel', 'Tourmaline',
-    #     'Zircon'])    
-    # phasez = range(1,len(phase))
-    # tab = plt.get_cmap('tab20')
-    # cNorm  = mcolors.Normalize(vmin=0, vmax=len(phase))
-    # scalarMap = mcm.ScalarMappable(norm=cNorm, cmap=tab)
-
-    # # plot latent representation
-    # for i in range(len(phase)):
-    #     indx = df['Mineral'] == phase[i]
-    #     ax[1].scatter(z[indx, 0], z[indx, 1], s=15, color=scalarMap.to_rgba(i), lw=1, label=phase[i], rasterized = True)
-    # ax[1].set_xlabel("Latent Variable 1")
-    # ax[1].set_ylabel("Latent Variable 2")
-    # ax[1].set_title(name + " Latent Space Representation")
-    # ax[1].legend(prop={'size': 8})
-    # plt.tight_layout()
-    # plt.savefig('parametermatrix_autoencoder/' + name + '_loss_latentspace.pdf',)
+    #     'Zircon'])
+
+    phase = np.array(
+        [
+            "Amphibole",
+            "Biotite",
+            "Clinopyroxene",
+            "Garnet",
+            "Ilmenite",
+            "KFeldspar",
+            "Magnetite",
+            "Muscovite",
+            "Olivine",
+            "Orthopyroxene",
+            "Plagioclase",
+            "Spinel",
+        ]
+    )
+
+    phasez = range(1, len(phase))
+    tab = plt.get_cmap("tab20")
+    cNorm = mcolors.Normalize(vmin=0, vmax=len(phase))
+    scalarMap = mcm.ScalarMappable(norm=cNorm, cmap=tab)
+
+    # plot latent representation
+    for i in range(len(phase)):
+        indx = df["Mineral"] == phase[i]
+        ax[1].scatter(
+            z[indx, 0],
+            z[indx, 1],
+            s=15,
+            color=scalarMap.to_rgba(i),
+            lw=1,
+            label=phase[i],
+            rasterized=True,
+        )
+    ax[1].set_xlabel("Latent Variable 1")
+    ax[1].set_ylabel("Latent Variable 2")
+    ax[1].set_title(name + " Latent Space Representation")
+    ax[1].legend(prop={"size": 8})
+    plt.tight_layout()
+    plt.savefig(
+        "parametermatrix_autoencoder/" + name + "_loss_latentspace.pdf",
+    )
 
     # save main model params
-    model_path = 'parametermatrix_autoencoder/' + name + "_tanh_params.pt"
+    model_path = "parametermatrix_autoencoder/" + name + "_tanh_params.pt"
     save_model_ae(model, optimizer, model_path)
 
     # save all other params
     conc_file = name + "_tanh.npz"
-    np.savez('parametermatrix_autoencoder/' + name + "_tanh.npz", batch_size = batch_size, epochs = epochs, lr = lr, wd = wd, input_size = input_size, 
-            conc_file = conc_file, z = z)
+    np.savez(
+        "parametermatrix_autoencoder/" + name + "_tanh.npz",
+        batch_size=batch_size,
+        epochs=epochs,
+        lr=lr,
+        wd=wd,
+        input_size=input_size,
+        conc_file=conc_file,
+        z=z,
+    )
 
-    return z 
+    return z
 
 
-def getLatent(model, dataset:np):
-
+def getLatent(model, dataset: np):
     """
 
-    Processes a given dataset through the encoder part of a trained model to obtain and return 
-    the latent space representations. The dataset is wrapped in a FeatureDataset and passed 
+    Processes a given dataset through the encoder part of a trained model to obtain and return
+    the latent space representations. The dataset is wrapped in a FeatureDataset and passed
     through the model in evaluation mode to generate latent vectors without computing gradients.
 
     Parameters:
         model (nn.Module): The trained model with an 'encoded' method that projects input to latent space.
         dataset (numpy.ndarray): The input data to be transformed into latent space representations.
 
     Returns:
         numpy.ndarray: An array of the latent space representations for the input dataset.
 
-    The function uses a DataLoader to batch process the dataset for efficiency and assumes the 
+    The function uses a DataLoader to batch process the dataset for efficiency and assumes the
     model has been moved to the appropriate device (CPU or GPU) before calling this function.
 
     """
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-    #transform real data to latent space using the trained model
-    latents=[]
+    # transform real data to latent space using the trained model
+    latents = []
     model.to(device)
 
     dataset_ = FeatureDataset(dataset)
-    loader = DataLoader(dataset_,batch_size=20,shuffle=False)
-    
+    loader = DataLoader(dataset_, batch_size=20, shuffle=False)
+
     model.eval()
     with torch.no_grad():
         for i, data in enumerate(loader):
             x = data.to(device)
             z = model.encoded(x)
             latents.append(z.detach().cpu().numpy())
-    
-    return np.concatenate(latents, axis=0)
 
+    return np.concatenate(latents, axis=0)
 
-def get_latent_space(df): 
 
+def get_latent_space(df):
     """
 
-    Loads a pre-trained autoencoder model and computes the latent space representations 
-    for the input dataframe. This function loads a model from a predefined path, normalizes 
-    the input data, and then uses the model to generate latent space representations for 
+    Loads a pre-trained autoencoder model and computes the latent space representations
+    for the input dataframe. This function loads a model from a predefined path, normalizes
+    the input data, and then uses the model to generate latent space representations for
     each data point.
 
     Parameters:
         df (pd.DataFrame): Input data frame to be processed by the autoencoder.
 
     Returns:
         pd.DataFrame: DataFrame containing the latent space representations.
 
     """
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     current_dir = os.path.dirname(__file__)
-    model_path = os.path.join(current_dir, 'ae_best_model.pt')
+    model_path = os.path.join(current_dir, "ae_best_model.pt")
     # model_path = os.path.join(current_dir, 'ae_best_model_noP_tanh.pt')
     model = Tanh_Autoencoder(input_dim=10, hidden_layer_sizes=(256, 64, 16)).to(device)
     optimizer = torch.optim.Adam(model.parameters(), lr=5e-4, weight_decay=0)
     load_model(model, optimizer, model_path)
 
     # # Set the model to evaluation mode
     # model.eval()
 
     norm_wt = norm_data_ae(df)
     z = getLatent(model, norm_wt)
-    z_df = pd.DataFrame(z, columns=['LV1', 'LV2'])
+    z_df = pd.DataFrame(z, columns=["LV1", "LV2"])
 
     return z_df
 
 
 def load_minclass_ae():
-
     """
 
     Loads the label dictionary for the autoencoder from a .npz file.
-    The file is expected to contain a dictionary under the 'label_dict' key. 
+    The file is expected to contain a dictionary under the 'label_dict' key.
     This function reads the dictionary and returns it.
 
     Returns:
         mapping (dict): A dictionary mapping integer codes to their corresponding
             class names.
 
     """
 
     current_dir = os.path.dirname(__file__)
-    filepath = os.path.join(current_dir, 'mineral_classes_ae.npz')
+    filepath = os.path.join(current_dir, "mineral_classes_ae.npz")
 
     with np.load(filepath, allow_pickle=True) as data:
-        mapping = data['mapping'].item()  # .item() is used to get the dictionary from numpy array
+        mapping = data[
+            "mapping"
+        ].item()  # .item() is used to get the dictionary from numpy array
 
     return mapping
 
 
-def load_clusterer(): 
-
+def load_clusterer():
     """
 
     Loads latent space data from a saved file, performs normalization, and applies clustering.
 
-    This function reads latent space representations from a saved .npz file, normalizes them, 
-    and then uses HDBSCAN to cluster the data. It returns the clusterer object and a DataFrame 
+    This function reads latent space representations from a saved .npz file, normalizes them,
+    and then uses HDBSCAN to cluster the data. It returns the clusterer object and a DataFrame
     containing the latent space data along with clustering results.
 
     Returns:
-        tuple: A tuple containing the HDBSCAN clusterer object and a DataFrame with latent variables, 
+        tuple: A tuple containing the HDBSCAN clusterer object and a DataFrame with latent variables,
                cluster labels, predicted minerals, and prediction probabilities.
 
     """
 
-
     current_dir = os.path.dirname(__file__)
-    filepath = os.path.join(current_dir, 'ae_tanh.npz')
-    z = np.load(filepath)['z']
+    filepath = os.path.join(current_dir, "ae_tanh.npz")
+    z = np.load(filepath)["z"]
 
-    array_train, params_train = feature_normalisation(z, return_params = True)
-    clusterer = HDBSCAN_flat(array_train, min_cluster_size=30, cluster_selection_epsilon=0.025, prediction_data=True)
+    array_train, params_train = feature_normalisation(z, return_params=True)
+    clusterer = HDBSCAN_flat(
+        array_train,
+        min_cluster_size=30,
+        cluster_selection_epsilon=0.025,
+        prediction_data=True,
+    )
     labels, probs = clusterer.labels_, clusterer.probabilities_
     minerals = class2mineral_ae(labels)
 
-    z_df = pd.DataFrame(z, columns=['LV1', 'LV2'])
-    z_df['Label'] = labels
-    z_df['Predict_Mineral'] = minerals
-    z_df['Predict_Probability'] = probs
+    z_df = pd.DataFrame(z, columns=["LV1", "LV2"])
+    z_df["Label"] = labels
+    z_df["Predict_Mineral"] = minerals
+    z_df["Predict_Probability"] = probs
 
     return clusterer, z_df
 
 
-def predict_class_prob_ae(df): 
-
+def predict_class_prob_ae(df):
     """
 
-    Predicts the class probabilities, corresponding mineral names, and the maximum 
-    probability for each class using a predefined Autoencoder model. This 
-    function loads a pre-trained model and its optimizer state, normalizes input 
+    Predicts the class probabilities, corresponding mineral names, and the maximum
+    probability for each class using a predefined Autoencoder model. This
+    function loads a pre-trained model and its optimizer state, normalizes input
     data, and performs multiple inference iterations to compute the prediction probabilities.
 
     Parameters:
         df (DataFrame): The input DataFrame containing the oxide composition data.
 
     Returns:
-        df (DataFrame): The input DataFrame with columns predict_mineral (predicted mineral names) 
-        and predict_prob (clustering probability of predicted class). 
+        df (DataFrame): The input DataFrame with columns predict_mineral (predicted mineral names)
+        and predict_prob (clustering probability of predicted class).
 
     """
 
     clusterer, z_df = load_clusterer()
 
     df_pred = df.copy()
 
     z_df = get_latent_space(df)
-    df_pred['LV1'] = z_df['LV1']
-    df_pred['LV2'] = z_df['LV2']
+    df_pred["LV1"] = z_df["LV1"]
+    df_pred["LV2"] = z_df["LV2"]
 
-    array_valid, params_valid = feature_normalisation(z_df.to_numpy(), return_params = True)
-    labels_valid, probs_valid = approximate_predict_flat(clusterer, array_valid, cluster_selection_epsilon=0.025)
+    array_valid, params_valid = feature_normalisation(
+        z_df.to_numpy(), return_params=True
+    )
+    labels_valid, probs_valid = approximate_predict_flat(
+        clusterer, array_valid, cluster_selection_epsilon=0.025
+    )
     predict_mineral = class2mineral_ae(labels_valid)
-    df_pred['Predict_Code'] = labels_valid
-    df_pred['Predict_Mineral'] = predict_mineral
-    df_pred['Predict_Probability'] = probs_valid
+    df_pred["Predict_Code"] = labels_valid
+    df_pred["Predict_Mineral"] = predict_mineral
+    df_pred["Predict_Probability"] = probs_valid
 
     return df_pred
 
 
-def unique_mapping_ae(pred_class): 
-
+def unique_mapping_ae(pred_class):
     """
-    Generates a mapping of unique class codes from given and predicted class labels, 
-    considering only the classes present in both input arrays. It loads a predefined 
-    category list and mapping, encodes the 'given_class' labels into categorical codes, 
-    and creates a subset mapping for the unique classes found. It also handles unknown 
+    Generates a mapping of unique class codes from given and predicted class labels,
+    considering only the classes present in both input arrays. It loads a predefined
+    category list and mapping, encodes the 'given_class' labels into categorical codes,
+    and creates a subset mapping for the unique classes found. It also handles unknown
     classes by assigning them a code of -1 and mapping the 'Unknown' label to them.
 
     Parameters:
         pred_class (array-like): The array of predicted class labels.
 
     Returns:
         unique (ndarray): Array of unique class codes found in both given and predicted classes.
-        valid_mapping (dict): Dictionary mapping class codes to their corresponding labels, 
+        valid_mapping (dict): Dictionary mapping class codes to their corresponding labels,
         including 'Unknown' for any class code of -1.
     """
 
     mapping = load_minclass_ae()
     unique = np.unique(pred_class)
     valid_mapping = {key: mapping[key] for key in unique}
     # if -1 in unique:
-    #     valid_mapping[-1] = "Outlier" 
+    #     valid_mapping[-1] = "Outlier"
 
     return unique, valid_mapping
 
 
-def class2mineral_ae(pred_class): 
-
+def class2mineral_ae(pred_class):
     """
     Translates predicted class codes into mineral names using a mapping obtained from the
-    unique classes present in the 'pred_class' array. It utilizes the 'unique_mapping_ae' 
+    unique classes present in the 'pred_class' array. It utilizes the 'unique_mapping_ae'
     function to establish the relevant class-to-mineral name mapping.
 
     Parameters:
         pred_class (array-like): The array of predicted class codes to be translated into mineral names.
 
     Returns:
         pred_mineral (ndarray): An array of mineral names corresponding to the predicted class codes.
@@ -696,66 +828,123 @@
     _, valid_mapping = unique_mapping_ae(pred_class)
     pred_mineral = np.array([valid_mapping[x] for x in pred_class])
 
     return pred_mineral
 
 
 def plot_latent_space(df_pred):
-
     """
 
     Plots the latent space representations of the training and validation datasets.
-    This function loads the latent space data using the `load_clusterer` function 
-    and visualizes it in a scatter plot. It compares the latent space representations 
-    of the training set with the predictions on the validation set, using different colors 
+    This function loads the latent space data using the `load_clusterer` function
+    and visualizes it in a scatter plot. It compares the latent space representations
+    of the training set with the predictions on the validation set, using different colors
     for each predicted mineral class.
 
     Parameters:
-        df_pred (pd.DataFrame): DataFrame containing latent space representations and predictions 
+        df_pred (pd.DataFrame): DataFrame containing latent space representations and predictions
                                 for the validation dataset.
 
     """
 
     clusterer, z_df = load_clusterer()
 
-    phase = np.array(['Amphibole', 'Apatite', 'Biotite', 'Clinopyroxene', 'Garnet', 
-        'Ilmenite', 'KFeldspar', 'Magnetite', 'Muscovite', 'Olivine', 'Orthopyroxene', 
-        'Plagioclase', 'Quartz', 'Rutile', 'Spinel', 'Tourmaline', 'Zircon'])    
-    cNorm  = mcolors.Normalize(vmin=0, vmax=len(phase))
-    scalarMap = mcm.ScalarMappable(norm=cNorm, cmap=plt.get_cmap('tab20'))
+    phase = np.array(
+        [
+            "Amphibole",
+            "Apatite",
+            "Biotite",
+            "Clinopyroxene",
+            "Garnet",
+            "Ilmenite",
+            "KFeldspar",
+            "Magnetite",
+            "Muscovite",
+            "Olivine",
+            "Orthopyroxene",
+            "Plagioclase",
+            "Quartz",
+            "Rutile",
+            "Spinel",
+            "Tourmaline",
+            "Zircon",
+        ]
+    )
+    cNorm = mcolors.Normalize(vmin=0, vmax=len(phase))
+    scalarMap = mcm.ScalarMappable(norm=cNorm, cmap=plt.get_cmap("tab20"))
 
-    fig, ax = plt.subplots(1, 2, figsize = (16, 8))
+    fig, ax = plt.subplots(1, 2, figsize=(16, 8))
     ax = ax.flatten()
     for i in range(len(phase)):
-        indx_z = z_df['Predict_Mineral'] == phase[i]
+        indx_z = z_df["Predict_Mineral"] == phase[i]
         if not z_df[indx_z].empty:
-            ax[0].scatter(z_df.LV1[indx_z], z_df.LV2[indx_z], marker='o', s=15, color=scalarMap.to_rgba(i), lw=0.1, ec='k', alpha=z_df.Predict_Probability[indx_z], label=phase[i], rasterized = True)
-        indx_pred = df_pred['Predict_Mineral'] == phase[i]
+            ax[0].scatter(
+                z_df.LV1[indx_z],
+                z_df.LV2[indx_z],
+                marker="o",
+                s=15,
+                color=scalarMap.to_rgba(i),
+                lw=0.1,
+                ec="k",
+                alpha=z_df.Predict_Probability[indx_z],
+                label=phase[i],
+                rasterized=True,
+            )
+        indx_pred = df_pred["Predict_Mineral"] == phase[i]
         if not df_pred[indx_pred].empty:
-            ax[1].scatter(df_pred.LV1[indx_pred], df_pred.LV2[indx_pred], marker='o', s=15, color=scalarMap.to_rgba(i), lw=0.1, ec='k', alpha=df_pred.Predict_Probability[indx_pred], label=phase[i], rasterized = True)
-    leg = ax[0].legend(prop={'size': 8}, loc = 'upper right', labelspacing = 0.4, handletextpad = 0.8, handlelength = 1.0, frameon=False)
-    for handle in leg.legendHandles: 
+            ax[1].scatter(
+                df_pred.LV1[indx_pred],
+                df_pred.LV2[indx_pred],
+                marker="o",
+                s=15,
+                color=scalarMap.to_rgba(i),
+                lw=0.1,
+                ec="k",
+                alpha=df_pred.Predict_Probability[indx_pred],
+                label=phase[i],
+                rasterized=True,
+            )
+    leg = ax[0].legend(
+        prop={"size": 8},
+        loc="upper right",
+        labelspacing=0.4,
+        handletextpad=0.8,
+        handlelength=1.0,
+        frameon=False,
+    )
+    for handle in leg.legendHandles:
         colors = handle.get_facecolor()
         # Set alpha value for face color
         colors[:, 3] = 1  # Set the alpha value of the RGBA color to 1
         handle.set_facecolor(colors)
 
         # If the handles also have edge colors, set their alpha values as well
         edge_colors = handle.get_edgecolor()
         edge_colors[:, 3] = 1
         handle.set_edgecolor(edge_colors)
-    ax[0].set_xlabel('Latent Variable 1')
-    ax[0].set_ylabel('Latent Variable 2')
+    ax[0].set_xlabel("Latent Variable 1")
+    ax[0].set_ylabel("Latent Variable 2")
     ax[0].set_xlim([-1.5, 2.0])
     ax[0].set_ylim([-2.5, 2.5])
-    ax[0].annotate("Training Latent Space", xy=(0.03, 0.94), xycoords="axes fraction", fontsize=20, weight='medium')
-    ax[0].tick_params(axis="x", direction='in', length=5, pad = 6.5) 
-    ax[0].tick_params(axis="y", direction='in', length=5, pad = 6.5)
-    ax[1].set_xlabel('Latent Variable 1')
-    ax[1].set_xlabel('Latent Variable 2')
+    ax[0].annotate(
+        "Training Latent Space",
+        xy=(0.03, 0.94),
+        xycoords="axes fraction",
+        fontsize=20,
+        weight="medium",
+    )
+    ax[0].tick_params(axis="x", direction="in", length=5, pad=6.5)
+    ax[0].tick_params(axis="y", direction="in", length=5, pad=6.5)
+    ax[1].set_xlabel("Latent Variable 1")
+    ax[1].set_xlabel("Latent Variable 2")
     ax[1].set_xlim([-1.5, 2.0])
     ax[1].set_ylim([-2.5, 2.5])
-    ax[1].annotate("Validation Latent Space", xy=(0.03, 0.94), xycoords="axes fraction", fontsize=20, weight='medium')
-    ax[1].tick_params(axis="x", direction='in', length=5, pad = 6.5) 
-    ax[1].tick_params(axis="y", direction='in', length=5, pad = 6.5)
+    ax[1].annotate(
+        "Validation Latent Space",
+        xy=(0.03, 0.94),
+        xycoords="axes fraction",
+        fontsize=20,
+        weight="medium",
+    )
+    ax[1].tick_params(axis="x", direction="in", length=5, pad=6.5)
+    ax[1].tick_params(axis="y", direction="in", length=5, pad=6.5)
     plt.tight_layout()
-
```

### Comparing `mineralML-0.0.0.5/src/mineralML.egg-info/PKG-INFO` & `mineralML-0.0.0.6/src/mineralML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mineralML
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: mineralML
 Home-page: https://github.com/sarahshi/mineralML
 Author: Sarah C. Shi
 Author-email: sarah.c.shi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,20 +16,20 @@
 # mineralML
 [![PyPI](https://badgen.net/pypi/v/mineralML)](https://pypi.org/project/mineralML/)
 [![Build Status](https://github.com/SarahShi/mineralML/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/mineralML/actions/workflows/main.yml)
 [![Documentation Status](https://readthedocs.org/projects/mineralml/badge/?version=latest)](https://mineralml.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/SarahShi/mineralML/branch/main/graph/badge.svg)](https://codecov.io/gh/SarahShi/mineralML/branch/main)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SarahShi/mineralML/blob/main/mineralML_colab.ipynb)
 [![Python 3.7](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 We present mineralML (mineral classification using Machine Learning) for classifying common igneous minerals based on oxide data collected by EPMA, with functions for calculating stoichiometries and crystallographic sites based on this classification. Utilizing this package allows for the identification of misclassified mineral phases and poor-quality data. We streamline data processing and cleaning to allow for the rapid transition to usable data, improving the utility of data curated in these databases and furthering computing and modeling capabilities. 
 
 ## Documentation
-Read the [documentation](https:/mineralML.readthedocs.io/en/latest/) for a run-through of the mineralML code. 
+Read the [documentation](https://mineralml.readthedocs.io/en/latest/?badge=latest) for a run-through of the mineralML code. 
 
 ## Run on the Cloud 
 If you do not have Python installed locally, run mineralML on [Google Colab](https://colab.research.google.com/github/SarahShi/mineralML/blob/main/mineralML_colab.ipynb). The Cloud-based version runs rapidly, with test cases of >10,000 microanalyses classified within 4 seconds. 
 
 ## Run and Install Locally
 Obtain a version of Python between 3.7 and 3.11 if you do not already have it installed. mineralML can be installed with one line. Open terminal and type the following:
```

### Comparing `mineralML-0.0.0.5/src/mineralML.egg-info/SOURCES.txt` & `mineralML-0.0.0.6/src/mineralML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

