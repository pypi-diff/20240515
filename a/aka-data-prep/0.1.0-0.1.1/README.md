# Comparing `tmp/aka-data-prep-0.1.0.tar.gz` & `tmp/aka-data-prep-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka-data-prep-0.1.0.tar", last modified: Tue May 14 21:37:52 2024, max compression
+gzip compressed data, was "aka-data-prep-0.1.1.tar", last modified: Tue May 14 22:27:02 2024, max compression
```

## Comparing `aka-data-prep-0.1.0.tar` & `aka-data-prep-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/
--rw-rw-rw-   0        0        0      190 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/aka_data_prep/
--rw-rw-rw-   0        0        0      124 2024-05-14 20:45:06.000000 aka-data-prep-0.1.0/aka_data_prep/__init__.py
--rw-rw-rw-   0        0        0    28453 2024-05-14 21:33:14.000000 aka-data-prep-0.1.0/aka_data_prep/aka_data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/
--rw-rw-rw-   0        0        0      190 2024-05-14 21:37:52.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 21:37:52.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-14 21:37:52.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 21:37:52.000000 aka-data-prep-0.1.0/aka_data_prep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 21:37:54.000000 aka-data-prep-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-05-14 21:37:28.000000 aka-data-prep-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/
+-rw-rw-rw-   0        0        0      190 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/aka_data_prep/
+-rw-rw-rw-   0        0        0      124 2024-05-14 20:45:06.000000 aka-data-prep-0.1.1/aka_data_prep/__init__.py
+-rw-rw-rw-   0        0        0    28673 2024-05-14 22:19:40.000000 aka-data-prep-0.1.1/aka_data_prep/aka_data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/aka_data_prep.egg-info/
+-rw-rw-rw-   0        0        0      190 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/aka_data_prep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/aka_data_prep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/aka_data_prep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/aka_data_prep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/aka_data_prep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 22:27:04.000000 aka-data-prep-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-05-14 22:26:44.000000 aka-data-prep-0.1.1/setup.py
```

### Comparing `aka-data-prep-0.1.0/aka_data_prep/aka_data_prep.py` & `aka-data-prep-0.1.1/aka_data_prep/aka_data_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import numpy as np 
 import math
 import shap
 
  
 import plotly.express as px
 import plotly.graph_objects as go
+import plotly.figure_factory as ff
+
 from plotly.subplots import make_subplots
 
  
 from scipy import stats
 
 
 
@@ -333,17 +335,22 @@
     # Method to plot a box plot
 
     def plot_box(self,df,index_col_box = [0,-1]):   
         for i in [0,1]:
             if index_col_box[i]<0:
                 index_col_box[i] += df.shape[1]+1 
 
-        fig = px.box(df, y=df.max().sort_values()[max(0,index_col_box[0]-1):min(index_col_box[1],df.shape[1])].index) 
+        df_max = df.select_dtypes(exclude=['object']).max().sort_values()
+        fig = px.box(df, y=df_max[max(0,index_col_box[0]-1):min(index_col_box[1],df.shape[1])].index) 
         fig.update_layout(**self.update_layout_parameter) 
         fig.update_xaxes(**self.update_axes)
+        fig.update_layout(
+                title='Box Plot',
+                font=dict(size=self.fsize)
+            ) 
         return fig
 
     # Method to plot a heatmap
     def plot_heatmap(self, df, show_label=True):
         x_label = df.columns
         y_label = df.index
         if df.shape[1] > 0:
@@ -372,14 +379,34 @@
             fig.update_layout(**self.update_layout_parameter)
             fig.update_xaxes(**self.update_axes)
             fig.update_yaxes(**self.update_axes)
             return fig
         else:
             print("Empty list is provided.")
 
+
+
+    # Method to plot the correlation matrix
+    def Plot_Correlation_Matrix(self, df, height=900, width=1000):
+        cm = df.corr()
+
+        fig = px.imshow(cm, labels=dict(color="Correlation"), x=cm.columns, y=cm.index)
+
+        fig.update_layout(**self.update_layout_parameter)
+        fig.update_xaxes(**self.update_axes)
+        fig.update_layout(
+            height=height,
+            width=width
+        )
+        fig.update_layout(
+            title='Correlation Matrix',
+            font=dict(size=self.fsize)
+        )
+        return fig
+
     # Method to plot a scatter plot
     def Plot_scatter(self, df, corr_tmp, fig_size_row=390, fig_size_col=490, subplot_col=3):
         if len(corr_tmp) > 0:
             nrow = math.ceil(len(corr_tmp) / subplot_col)
             # Create subplots
             fig = make_subplots(
                 rows=nrow, cols=subplot_col,
@@ -502,16 +529,14 @@
         fig.update_yaxes(**self.update_axes) 
         fig.update_layout(title='Regression Summary',font=dict(size=self.fsize)) 
 
         return fig
 
 
 
-
-
     def plot_classification_report(self, y, y_predict, cmLabel, lab=1): 
         # Generate classification report
         report_str = classification_report(y, y_predict, target_names=cmLabel, output_dict=True) 
         colss = ['precision', 'recall', 'f1-score', 'support']
 
         # Convert to a DataFrame
         report_df = pd.DataFrame(report_str)
@@ -539,32 +564,14 @@
                 title='Correlation Matrix',
                 font=dict(size=self.fsize)
             ) 
 
         return fig 
 
 
-    # Method to plot the correlation matrix
-    def Plot_Correlation_Matrix(self, df, height=900, width=1000):
-        cm = df.corr()
-
-        fig = px.imshow(cm, labels=dict(color="Correlation"), x=cm.columns, y=cm.index)
-
-        fig.update_layout(**self.update_layout_parameter)
-        fig.update_xaxes(**self.update_axes)
-        fig.update_layout(
-            height=height,
-            width=width
-        )
-        fig.update_layout(
-            title='Correlation Matrix',
-            font=dict(size=self.fsize)
-        )
-        return fig
-
     # Method to plot a confusion matrix
     def plot_confusion_matrix(self, y, y_predict, feature_name, show_label=True):
         cm = confusion_matrix(y, y_predict)
         if show_label:
             fig = ff.create_annotated_heatmap(cm,
                                                x=feature_name[:cm.shape[1]],
                                                y=feature_name[:cm.shape[1]],
```

