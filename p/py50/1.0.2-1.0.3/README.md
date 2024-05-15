# Comparing `tmp/py50-1.0.2.tar.gz` & `tmp/py50-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py50-1.0.2.tar", max compression
+gzip compressed data, was "py50-1.0.3.tar", max compression
```

## Comparing `py50-1.0.2.tar` & `py50-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.2/LICENSE
--rw-r--r--   0        0        0     4542 2024-04-29 03:50:21.000706 py50-1.0.2/README_pypi.md
--rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.2/py50/.DS_Store
--rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.2/py50/__init__.py
--rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.2/py50/calculator.py
--rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.2/py50/plot_settings.py
--rw-r--r--   0        0        0    43460 2024-04-30 01:26:56.191290 py50-1.0.2/py50/plotcurve.py
--rw-r--r--   0        0        0    88711 2024-04-29 03:02:08.739556 py50-1.0.2/py50/stats.py
--rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.2/py50/utils.py
--rw-r--r--   0        0        0      591 2024-04-30 05:53:58.551879 py50-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 py50-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4542 2024-05-15 04:09:24.427854 py50-1.0.3/README_pypi.md
+-rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.3/py50/.DS_Store
+-rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.3/py50/__init__.py
+-rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.3/py50/calculator.py
+-rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.3/py50/plot_settings.py
+-rw-r--r--   0        0        0    43460 2024-04-30 01:26:56.191290 py50-1.0.3/py50/plotcurve.py
+-rw-r--r--   0        0        0    92545 2024-05-15 02:13:49.689769 py50-1.0.3/py50/stats.py
+-rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.3/py50/utils.py
+-rw-r--r--   0        0        0      591 2024-05-15 04:11:36.936202 py50-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 py50-1.0.3/PKG-INFO
```

### Comparing `py50-1.0.2/LICENSE` & `py50-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py50-1.0.2/README_pypi.md` & `py50-1.0.3/README_pypi.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # py50: Generate Dose-Response Curves
 
-![Static Badge](https://img.shields.io/badge/py50_v1.0.0-13406E)
+![Static Badge](https://img.shields.io/badge/py50_v1.0.3-13406E)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py50)
 [![Documentation Status](https://readthedocs.org/projects/py50/badge/?version=latest)](https://py50.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![DOI](https://zenodo.org/badge/716929963.svg)](https://zenodo.org/doi/10.5281/zenodo.10183912)
 [![Streamlit](https://img.shields.io/badge/Streamlit-1.29.0-FF4B4B.svg?style=flat&logo=Streamlit&logoColor=white)](https://py50-app.streamlit.app)
```

### Comparing `py50-1.0.2/py50/.DS_Store` & `py50-1.0.3/py50/.DS_Store`

 * *Files identical despite different names*

### Comparing `py50-1.0.2/py50/calculator.py` & `py50-1.0.3/py50/calculator.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.2/py50/plot_settings.py` & `py50-1.0.3/py50/plot_settings.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.2/py50/plotcurve.py` & `py50-1.0.3/py50/plotcurve.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.2/py50/stats.py` & `py50-1.0.3/py50/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         Test data normality of dataset.
 
         :param value_col: String
             Name of column containing the dependent variable.
         :param group_col: String
             Name of columnName of column containing the grouping variable.
         :param method: String
-            Normality test. ‘shapiro’ (default). Additional tests can be found with [pingouin.normality()](https://pingouin-stats.org/build/html/generated/pingouin.normality.html)
+            Normality test. ‘shapiro’ (default). Additional tests can be found with
+            [pingouin.normality()](https://pingouin-stats.org/build/html/generated/pingouin.normality.html)
         :param kwargs: optional
             Other options available with pingouin.normality()
         :return: Pandas.DataFrame
         """
 
         result_df = pg.normality(
             data=self.data, dv=value_col, group=group_col, method=method, **kwargs
@@ -72,15 +73,16 @@
         Test for data variance.
 
         :param value_col: String
             Name of column containing the dependent variable.
         :param group_col: String
             Name of columnName of column containing the grouping variable.
         :param method: String
-            Statistical test. ‘levene’ (default). Additional tests can be found with [pingouin.homoscedasticity()](https://pingouin-stats.org/build/html/generated/pingouin.homoscedasticity.html#pingouin.homoscedasticity)
+            Statistical test. ‘levene’ (default). Additional tests can be found with
+            [pingouin.homoscedasticity()](https://pingouin-stats.org/build/html/generated/pingouin.homoscedasticity.html#pingouin.homoscedasticity)
         :param kwargs: optional
             Other options available with pingouin.homoscedasticity()
         :return: Pandas.DataFrame
         """
 
         result_df = pg.homoscedasticity(
             data=self.data, dv=value_col, group=group_col, method=method, **kwargs
@@ -95,16 +97,17 @@
         """
         One-way and N-way ANOVA.
 
         :param value_col: String
             Name of column containing the dependent variable.
         :param group_col: String or list of strings
             Name of columnName of column containing the grouping variable.
-        :param kwarts: optional
-            Other options available with [pingouin.anova()](https://pingouin-stats.org/build/html/generated/pingouin.anova.html)
+        :param kwargs: optional
+            Other options available with
+            [pingouin.anova()](https://pingouin-stats.org/build/html/generated/pingouin.anova.html)
         :return: Pandas.DataFrame
         """
 
         result_df = pg.anova(data=self.data, dv=value_col, between=group_col, **kwargs)
 
         # Add significance asterisk
         pvalue = [utils.star_value(value) for value in result_df["p-unc"]]
@@ -191,15 +194,16 @@
         :param group_col: String
             Name of column containing the between factor.
         :param within_subject_col: String
             Name of column containing the within-subject factor (repeated measurements).
         :param subject_col:
             Name of column containing the between-subject identifier.
         :param kwargs: optional
-            Other options available with [pingouin.mixed_anova()](https://pingouin-stats.org/build/html/generated/pingouin.mixed_anova.html)
+            Other options available with
+            [pingouin.mixed_anova()](https://pingouin-stats.org/build/html/generated/pingouin.mixed_anova.html)
         :return: Pandas.DataFrame
         """
 
         result_df = pg.mixed_anova(
             data=self.data,
             dv=value_col,
             between=group_col,
@@ -219,15 +223,16 @@
         Pairwise Tukey post-hoc test.
 
         :param value_col: String
             Name of column containing the dependent variable.
         :param group_col: String
             Name of columnName of column containing the between factor.
         :param effsize: String or None
-            Effect size. Additional methods can be found with [pingouin.pairwise_tukey()](https://pingouin-stats.org/build/html/generated/pingouin.pairwise_tukey.html)
+            Effect size. Additional methods can be found with
+            [pingouin.pairwise_tukey()](https://pingouin-stats.org/build/html/generated/pingouin.pairwise_tukey.html)
         :return: Pandas.DataFrame
         """
 
         result_df = pg.pairwise_tukey(
             data=self.data, dv=value_col, between=group_col, effsize=effsize
         )
 
@@ -242,15 +247,16 @@
         Pairwise Games-Howell post-hoc test
 
         :param value_col: String
             Name of column containing the dependent variable.
         :param group_col: String
             Name of columnName of column containing the between factor.
         :param effsize: String or None
-            Effect size. Additional methods can be found with [pingouin.pairwise_gameshowell()](https://pingouin-stats.org/build/html/generated/pingouin.pairwise_gameshowell.html)
+            Effect size. Additional methods can be found with
+            [pingouin.pairwise_gameshowell()](https://pingouin-stats.org/build/html/generated/pingouin.pairwise_gameshowell.html)
         :return: Pandas.DataFrame
         """
 
         result_df = pg.pairwise_gameshowell(
             data=self.data, dv=value_col, between=group_col, effsize=effsize
         )
 
@@ -281,15 +287,16 @@
             Column containing group name.
         :param subgroup_col: String
             Column containing subgroup name.
         :param alternative: String
             Defines the alternative hypothesis, or tail of the test. Must be one of “two-sided”. Must be one of
             “two-sided” (default), “greater” or “less”.
         :param kwargs: Optional
-            Other options available with [pingouin.wilcoxon()](https://pingouin-stats.org/build/html/generated/pingouin.wilcoxon.html)
+            Other options available with
+            [pingouin.wilcoxon()](https://pingouin-stats.org/build/html/generated/pingouin.wilcoxon.html)
         :return: Pandas.DataFrame
         """
 
         # ignore Wilcoxon warnings
         warnings.filterwarnings(
             "ignore",
             message="Exact p-value calculation does not work if there are zeros.*",
@@ -568,15 +575,15 @@
         Calculate Kruskal-Wallis H-test for independent samples.
 
         :param value_col: String
             Name of column containing the dependent variable.
         :param group_col: String
             Name of column containing the between factor.
         :param detailed: Boolean
-            Ouput additional details from Kruskal-Wallis H-test.
+            Output additional details from Kruskal-Wallis H-test.
         :return: Pandas.DataFrame
         """
 
         result_df = pg.kruskal(
             data=self.data, dv=value_col, between=group_col, detailed=detailed
         )
 
@@ -869,14 +876,15 @@
         value_col=None,
         group_order=None,
         subgroup_col=None,
         subject_col=None,
         within_subject_col=None,
         pairs=None,
         pvalue_label=None,
+        hide_ns=False,
         palette=None,
         orient="v",
         loc="inside",
         whis=1.5,  # boxplot whiskers
         return_df=None,
         **kwargs,
     ):
@@ -898,14 +906,16 @@
             Name of the column containing the subject column.
         :param within_subject_col: String
             Name of the column containing the within subject column.
         :param pairs: List
             A list containing specific pairings for annotation on the plot.
         :param pvalue_label: List.
             A list containing specific pvalue labels. This order must match the length of pairs list.
+        :param hide_ns: bool
+            Automatically hide groups with no significance from plot.
         :param palette: String or List.
             Color palette used for the plot. Can be given as common color name or in hex code.
         :param orient: String
             Orientation of the plot. Only "v" and "h" are for vertical and horizontal, respectively, is supported
         :param loc: String
             Set location of annotations. Only "inside" or "outside" are supported.
         :param whis: Int
@@ -949,14 +959,27 @@
             annotate_kwargs["line_offset_to_group"] = line_offset_to_group
             annotate_kwargs["line_offset"] = line_offset
 
         # Set order for groups on plot
         if group_order:
             group_order = group_order
 
+        # If set to True, only show plots with significance
+        if hide_ns is True:
+            # Filter n.s. from pvalue and pairs
+            hidden_sigfig_data = [
+                (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
+            ]
+
+            # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
+            pvalue, pairs = zip(*hidden_sigfig_data)
+            # # to trouble shoot
+            # print(pvalue)
+            # print(pairs)
+
         # set orientation for plot and Annotator
         orient = orient.lower()
         if orient == "v":
             ax = sns.boxplot(
                 data=self.data,
                 x=group_col,
                 y=value_col,
@@ -1043,24 +1066,25 @@
         value_col=None,
         group_order=None,
         subgroup_col=None,
         subject_col=None,
         within_subject_col=None,
         pairs=None,
         pvalue_label=None,
+        hide_ns=False,
         palette=None,
         orient="v",
         loc="inside",
         errorbar="sd",
         capsize=0.1,
         return_df=None,
         **kwargs,
     ):
         """
-        Draw a boxplot from the input DataFrame.
+        Draw a barplot from the input DataFrame.
 
         :param test: String
             Name of test for calculations. Names must match the test names from the py50.Stats()
         :param group_col: String
             Name of column containing groups. This should be the between depending on the selected test.
         :param value_col: String
             Name of the column containing the values. This is the dependent variable.
@@ -1073,14 +1097,16 @@
             Name of the column containing the subject column.
         :param within_subject_col: String
             Name of the column containing the within subject column.
         :param pairs: List
             A list containing specific pairings for annotation on the plot.
         :param pvalue_label: List.
             A list containing specific pvalue labels. This order must match the length of pairs list.
+        :param hide_ns: bool
+            Automatically hide groups with no significance from plot.
         :param palette: String or List.
             Color palette used for the plot. Can be given as common color name or in hex code.
         :param orient: String
             Orientation of the plot. Only "v" and "h" are for vertical and horizontal, respectively, is supported
         :param loc: String
             Set location of annotations. Only "inside" or "outside" are supported.
         :param errorbar: String
@@ -1124,14 +1150,27 @@
             annotate_kwargs["line_offset_to_group"] = line_offset_to_group
             annotate_kwargs["line_offset"] = line_offset
 
         # Set order for groups on plot
         if group_order:
             group_order = group_order
 
+        # If set to True, only show plots with significance
+        if hide_ns is True:
+            # Filter n.s. from pvalue and pairs
+            hidden_sigfig_data = [
+                (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
+            ]
+
+            # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
+            pvalue, pairs = zip(*hidden_sigfig_data)
+            # # to trouble shoot
+            # print(pvalue)
+            # print(pairs)
+
         # set orientation for plot and Annotator
         orient = orient.lower()
         if orient == "v":
             ax = sns.barplot(
                 data=self.data,
                 x=group_col,
                 y=value_col,
@@ -1220,22 +1259,23 @@
         value_col=None,
         group_order=None,
         subgroup_col=None,
         subject_col=None,
         within_subject_col=None,
         pairs=None,
         pvalue_label=None,
+        hide_ns=False,
         palette=None,
         orient="v",
         loc="inside",
         return_df=None,
         **kwargs,
     ):
         """
-        Draw a boxplot from the input DataFrame.
+        Draw a biolinplot from the input DataFrame.
 
         :param test: String
             Name of test for calculations. Names must match the test names from the py50.Stats()
         :param group_col: String
             Name of column containing groups. This should be the between depending on the selected test.
         :param value_col: String
             Name of the column containing the values. This is the dependent variable.
@@ -1248,14 +1288,16 @@
             Name of the column containing the subject column.
         :param within_subject_col: String
             Name of the column containing the within subject column.
         :param pairs: List
             A list containing specific pairings for annotation on the plot.
         :param pvalue_label: List.
             A list containing specific pvalue labels. This order must match the length of pairs list.
+        :param hide_ns: bool
+            Automatically hide groups with no significance from plot.
         :param palette: String or List.
             Color palette used for the plot. Can be given as common color name or in hex code.
         :param orient: String
             Orientation of the plot. Only "v" and "h" are for vertical and horizontal, respectively, is supported
         :param loc: String
             Set location of annotations. Only "inside" or "outside" are supported.
         :param return_df: Boolean
@@ -1297,14 +1339,27 @@
             annotate_kwargs["line_offset_to_group"] = line_offset_to_group
             annotate_kwargs["line_offset"] = line_offset
 
         # Set order for groups on plot
         if group_order:
             group_order = group_order
 
+        # If set to True, only show plots with significance
+        if hide_ns is True:
+            # Filter n.s. from pvalue and pairs
+            hidden_sigfig_data = [
+                (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
+            ]
+
+            # Unzip the hidden_sigfig_data and separate into pvalue and pairs
+            pvalue, pairs = zip(*hidden_sigfig_data)
+            # # to trouble shoot
+            # print(pvalue)
+            # print(pairs)
+
         # set orientation for plot and Annotator
         orient = orient.lower()
         if orient == "v":
             ax = sns.violinplot(
                 data=self.data,
                 x=group_col,
                 y=value_col,
@@ -1375,36 +1430,37 @@
             plt.title(kwargs["title"])
         if "title" and "fontsize" in kwargs:
             plt.title(kwargs["title"], fontsize=kwargs["fontsize"])
 
         # Return DataFrame AND figure
         if return_df:
             return stat_df, annotator
-
-        return annotator
+        else:
+            return annotator
 
     def swarmplot(
         self,
         test=None,
         group_col=None,
         value_col=None,
         group_order=None,
         subgroup_col=None,
         subject_col=None,
         within_subject_col=None,
         pairs=None,
         pvalue_label=None,
+        hide_ns=False,
         palette=None,
         orient="v",
         loc="inside",
         return_df=None,
         **kwargs,
     ):
         """
-        Draw a boxplot from the input DataFrame.
+        Draw a swarmplot from the input DataFrame.
 
         :param test: String
             Name of test for calculations. Names must match the test names from the py50.Stats()
         :param group_col: String
             Name of column containing groups. This should be the between depending on the selected test.
         :param value_col: String
             Name of the column containing the values. This is the dependent variable.
@@ -1417,14 +1473,16 @@
             Name of the column containing the subject column.
         :param within_subject_col: String
             Name of the column containing the within subject column.
         :param pairs: List
             A list containing specific pairings for annotation on the plot.
         :param pvalue_label: List.
             A list containing specific pvalue labels. This order must match the length of pairs list.
+        :param hide_ns: bool
+            Automatically hide groups with no significance from plot.
         :param palette: String or List.
             Color palette used for the plot. Can be given as common color name or in hex code.
         :param orient: String
             Orientation of the plot. Only "v" and "h" are for vertical and horizontal, respectively, is supported
         :param loc: String
             Set location of annotations. Only "inside" or "outside" are supported.
         :param return_df: Boolean
@@ -1469,14 +1527,27 @@
             annotate_kwargs["line_offset_to_group"] = line_offset_to_group
             annotate_kwargs["line_offset"] = line_offset
 
         # Set order for groups on plot
         if group_order:
             group_order = group_order
 
+        # If set to True, only show plots with significance
+        if hide_ns is True:
+            # Filter n.s. from pvalue and pairs
+            hidden_sigfig_data = [
+                (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
+            ]
+
+            # Unzip the hidden_sigfig_data and separate into pvalue and pairs
+            pvalue, pairs = zip(*hidden_sigfig_data)
+            # # to trouble shoot
+            # print(pvalue)
+            # print(pairs)
+
         # To color code plots:
         subgroup_col_plot = None
         if subgroup_col is None:
             subgroup_col_plot = group_col
 
         # set orientation for plot and Annotator
         orient = orient.lower()
@@ -1547,15 +1618,15 @@
         # Make sure the pairs and pvalue lists match
         if len(pairs) != len(pvalue):
             raise Exception("pairs and pvalue_order length does not match!")
         else:
             annotator.set_custom_annotations(pvalue)
             annotator.annotate(**annotate_kwargs)
 
-        # Turn off legend by default. Can be assessed outside using hte plt.legend()
+        # Turn off legend by default. Can be assessed outside using the plt.legend()
         plt.legend().set_visible(False)
 
         # Adjust title and title fontsize from kwargs
         if "title" in kwargs:
             plt.title(kwargs["title"])
         if "title" and "fontsize" in kwargs:
             plt.title(kwargs["title"], fontsize=kwargs["fontsize"])
@@ -1573,22 +1644,23 @@
         value_col=None,
         group_order=None,
         subgroup_col=None,
         subject_col=None,
         within_subject_col=None,
         pairs=None,
         pvalue_label=None,
+        hide_ns=False,
         palette=None,
         orient="v",
         loc="inside",
         return_df=None,
         **kwargs,
     ):
         """
-        Draw a boxplot from the input DataFrame.
+        Draw a stripplot from the input DataFrame.
 
         :param test: String
             Name of test for calculations. Names must match the test names from the py50.Stats()
         :param group_col: String
             Name of column containing groups. This should be the between depending on the selected test.
         :param value_col: String
             Name of the column containing the values. This is the dependent variable.
@@ -1601,14 +1673,16 @@
             Name of the column containing the subject column.
         :param within_subject_col: String
             Name of the column containing the within subject column.
         :param pairs: List
             A list containing specific pairings for annotation on the plot.
         :param pvalue_label: List.
             A list containing specific pvalue labels. This order must match the length of pairs list.
+        :param hide_ns: bool
+            Automatically hide groups with no significance from plot.
         :param palette: String or List.
             Color palette used for the plot. Can be given as common color name or in hex code.
         :param orient: String
             Orientation of the plot. Only "v" and "h" are for vertical and horizontal, respectively, is supported
         :param loc: String
             Set location of annotations. Only "inside" or "outside" are supported.
         :param return_df: Boolean
@@ -1653,14 +1727,27 @@
             annotate_kwargs["line_offset_to_group"] = line_offset_to_group
             annotate_kwargs["line_offset"] = line_offset
 
         # Set order for groups on plot
         if group_order:
             group_order = group_order
 
+        # If set to True, only show plots with significance
+        if hide_ns is True:
+            # Filter n.s. from pvalue and pairs
+            hidden_sigfig_data = [
+                (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
+            ]
+
+            # Unzip the hidden_sigfig_data and separate into pvalue and pairs
+            pvalue, pairs = zip(*hidden_sigfig_data)
+            # # to trouble shoot
+            # print(pvalue)
+            # print(pairs)
+
         # To color code plots:
         subgroup_col_plot = None
         if subgroup_col is None:
             subgroup_col_plot = group_col
 
         # set orientation for plot and Annotator
         orient = orient.lower()
@@ -1757,22 +1844,23 @@
         value_col=None,
         group_order=None,
         subgroup_col=None,
         subject_col=None,
         within_subject_col=None,
         pairs=None,
         pvalue_label=None,
+        hide_ns=False,
         palette=None,
         orient="v",
         loc="inside",
         return_df=None,
         **kwargs,
     ):
         """
-        Draw a boxplot from the input DataFrame.
+        Draw a boxenplot from the input DataFrame.
 
         :param test: String
             Name of test for calculations. Names must match the test names from the py50.Stats()
         :param group_col: String
             Name of column containing groups. This should be the between depending on the selected test.
         :param value_col: String
             Name of the column containing the values. This is the dependent variable.
@@ -1785,14 +1873,16 @@
             Name of the column containing the subject column.
         :param within_subject_col: String
             Name of the column containing the within subject column.
         :param pairs: List
             A list containing specific pairings for annotation on the plot.
         :param pvalue_label: List.
             A list containing specific pvalue labels. This order must match the length of pairs list.
+        :param hide_ns: bool
+            Automatically hide groups with no significance from plot.
         :param palette: String or List.
             Color palette used for the plot. Can be given as common color name or in hex code.
         :param orient: String
             Orientation of the plot. Only "v" and "h" are for vertical and horizontal, respectively, is supported
         :param loc: String
             Set location of annotations. Only "inside" or "outside" are supported.
         :param return_df: Boolean
@@ -1834,14 +1924,27 @@
             annotate_kwargs["line_offset_to_group"] = line_offset_to_group
             annotate_kwargs["line_offset"] = line_offset
 
         # Set order for groups on plot
         if group_order:
             group_order = group_order
 
+        # If set to True, only show plots with significance
+        if hide_ns is True:
+            # Filter n.s. from pvalue and pairs
+            hidden_sigfig_data = [
+                (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
+            ]
+
+            # Unzip the hidden_sigfig_data and separate into pvalue and pairs
+            pvalue, pairs = zip(*hidden_sigfig_data)
+            # # to trouble shoot
+            # print(pvalue)
+            # print(pairs)
+
         # set orientation for plot and Annotator
         orient = orient.lower()
         if orient == "v":
             ax = sns.boxenplot(
                 data=self.data,
                 x=group_col,
                 y=value_col,
@@ -1940,15 +2043,15 @@
         loc="inside",
         ci="sd",
         capsize=0.1,
         return_df=None,
         **kwargs,
     ):
         """
-        Draw a boxplot from the input DataFrame.
+        Draw a lineplot from the input DataFrame.
 
         :param test: String
             Name of test for calculations. Names must match the test names from the py50.Stats()
         :param group_col: String
             Name of column containing groups. This should be the between depending on the selected test.
         :param value_col: String
             Name of the column containing the values. This is the dependent variable.
```

### Comparing `py50-1.0.2/py50/utils.py` & `py50-1.0.3/py50/utils.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.2/pyproject.toml` & `py50-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py50"
-version = "1.0.2"
+version = "1.0.3"
 description = "Generate Dose-Response Curves"
 documentation = "https://py50.readthedocs.io/en/latest/"
 authors = ["Tony Eight Lin <tonyelin@tmu.edu.tw>"]
 license = "GPL-3.0"
 readme = "README_pypi.md"
 packages = [{ include = "py50"}]
```

### Comparing `py50-1.0.2/PKG-INFO` & `py50-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py50
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generate Dose-Response Curves
 License: GPL-3.0
 Author: Tony Eight Lin
 Author-email: tonyelin@tmu.edu.tw
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 Requires-Dist: seaborn (<0.12.0)
 Requires-Dist: statannotations (>=0.6.0)
 Project-URL: Documentation, https://py50.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # py50: Generate Dose-Response Curves
 
-![Static Badge](https://img.shields.io/badge/py50_v1.0.0-13406E)
+![Static Badge](https://img.shields.io/badge/py50_v1.0.3-13406E)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py50)
 [![Documentation Status](https://readthedocs.org/projects/py50/badge/?version=latest)](https://py50.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![DOI](https://zenodo.org/badge/716929963.svg)](https://zenodo.org/doi/10.5281/zenodo.10183912)
 [![Streamlit](https://img.shields.io/badge/Streamlit-1.29.0-FF4B4B.svg?style=flat&logo=Streamlit&logoColor=white)](https://py50-app.streamlit.app)
```

