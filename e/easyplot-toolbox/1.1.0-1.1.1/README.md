# Comparing `tmp/easyplot_toolbox-1.1.0.tar.gz` & `tmp/easyplot_toolbox-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyplot_toolbox-1.1.0.tar", max compression
+gzip compressed data, was "easyplot_toolbox-1.1.1.tar", max compression
```

## Comparing `easyplot_toolbox-1.1.0.tar` & `easyplot_toolbox-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       23 2024-04-28 20:37:03.067281 easyplot_toolbox-1.1.0/easyplot_toolbox/__init__.py
--rw-r--r--   0        0        0    43826 2024-04-29 00:02:13.718962 easyplot_toolbox-1.1.0/easyplot_toolbox/easyplot.py
--rw-r--r--   0        0        0     1115 2024-04-23 00:44:35.527423 easyplot_toolbox-1.1.0/license.md
--rw-r--r--   0        0        0      531 2024-04-29 00:13:22.106376 easyplot_toolbox-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      997 2024-04-29 00:17:20.509228 easyplot_toolbox-1.1.0/readme2.md
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 easyplot_toolbox-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-28 20:37:03.067281 easyplot_toolbox-1.1.1/easyplot_toolbox/__init__.py
+-rw-r--r--   0        0        0    49060 2024-05-15 00:28:28.387863 easyplot_toolbox-1.1.1/easyplot_toolbox/easyplot.py
+-rw-r--r--   0        0        0     1115 2024-04-23 00:44:35.527423 easyplot_toolbox-1.1.1/license.md
+-rw-r--r--   0        0        0      535 2024-05-15 00:20:38.591219 easyplot_toolbox-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1170 2024-05-15 00:45:35.515142 easyplot_toolbox-1.1.1/readme-pypi.md
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 easyplot_toolbox-1.1.1/PKG-INFO
```

### Comparing `easyplot_toolbox-1.1.0/easyplot_toolbox/easyplot.py` & `easyplot_toolbox-1.1.1/easyplot_toolbox/easyplot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""easyplot tools for data visualization"""
 import matplotlib.pyplot as plt
 import seaborn as sns
 import numpy as np
 from matplotlib.lines import Line2D
 import squarify
 import pandas as pd
 import joypy
@@ -62,51 +63,51 @@
 
 
 def histogram_chart(**kwargs):
     """
     This function shows a Boxplot and Histogram in a single chart.
 
     Args:
-        plot_setup (Dictionary): Setup chart Dictionary with the following keys:
+        plot_setup (Dictionary): Settings of chart (Dictionary with the following keys):
             name (String): Path + name figure (key required in plot_setup)
             width (Float): figure width in SI units (key required in plot_setup)
             height (Float): figure height in SI units (key required in plot_setup)
             extension (String): File extension (key required in plot_setup)
-            dots per inch (Integer): The resolution in dots per inch (key required in plot_setup)
-            x axis label (String): x axis label (key required in plot_setup)
-            x axis size (Integer): x axis size (key required in plot_setup)
-            y axis label (String): y axis label (key required in plot_setup)
-            y axis size (Integer): y axis size (key required in plot_setup)
-            axises color (String): Axises color (key required in plot_setup)
-            labels size (Integer): Labels size (key required in plot_setup)
-            labels color (String): Labels color (key required in plot_setup)
-            chart color (String): Chart color (key required in plot_setup)
+            dots_per_inch (Integer): The resolution in dots per inch (key required in plot_setup)
+            x_axis_label (String): x axis label (key required in plot_setup)
+            x_axis_size (Integer): x axis size (key required in plot_setup)
+            y_axis_label (String): y axis label (key required in plot_setup)
+            y_axis_size (Integer): y axis size (key required in plot_setup)
+            axises_color (String): Axises color (key required in plot_setup)
+            labels_size (Integer): Labels size (key required in plot_setup)
+            labels_color (String): Labels color (key required in plot_setup)
+            chart_color (String): Chart color (key required in plot_setup)
             bins (Integer): Range representing the width of a single bar (key required in plot_setup)
         dataset (List or array): Dataset
             
     Returns:
         None
     """
 
     # Setup
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
-    x_axis_label = plot_setup['x axis label']
-    x_axis_size = plot_setup['x axis size']
-    y_axis_label = plot_setup['y axis label']
-    y_axis_size = plot_setup['y axis size']
-    axises_color = plot_setup['axises color']
-    labels_size = plot_setup['labels size']     
-    labels_color = plot_setup['labels color']
-    chart_color = plot_setup['chart color']
+    x_axis_label = plot_setup['x_axis_label']
+    x_axis_size = plot_setup['x_axis_size']
+    y_axis_label = plot_setup['y_axis_label']
+    y_axis_size = plot_setup['y_axis_size']
+    axises_color = plot_setup['axises_color']
+    labels_size = plot_setup['labels_size']     
+    labels_color = plot_setup['labels_color']
+    chart_color = plot_setup['chart_color']
     bins = int(plot_setup['bins']) 
     # kDE = plot_setup['kDE']
-    dots_per_inch = plot_setup['dots per inch'] 
+    dots_per_inch = plot_setup['dots_per_inch'] 
     extension = plot_setup['extension']
     
     # Dataset
     data = kwargs.get('dataset')
  
     # Plot
     [w, h] = convert_si_to_inches_in_chart_size(w, h)
@@ -127,50 +128,50 @@
     plt.grid()
     sns.despine(ax=ax_hist)
     sns.despine(ax=ax_box, left=True)
     plt.tight_layout()
 
     # Save figure
     save_chart_in_folder(name, extension, dots_per_inch)
-    
+
     # Show figure
     plt.show()
 
 
 def line_chart(**kwargs):
     """
     This function shows a multiple lines in single chart.
 
     Args:
-        plot_setup (Dictionary): Setup chart Dictionary with the following keys:
+        plot_setup (Dictionary): Settings of chart (Dictionary with the following keys):
             name (String): Path + name figure (key required in plot_setup)
             width (Float): figure width in SI units (key required in plot_setup)
             height (Float): figure height in SI units (key required in plot_setup)
             extension (String): File extension (key required in plot_setup)
             dots_per_inch (Integer): The resolution in dots per inch (key required in plot_setup)
             marker (List): List of markers. See <a href="https://matplotlib.org/stable/gallery/lines_bars_and_markers/marker_reference.html#sphx-glr-gallery-lines-bars-and-markers-marker-reference-py" target="_blank">gallery</a> (key required in plot_setup)
-            marker size (List): List of marker sizes (key required in plot_setup)
-            line width (List): List of line widths (key required in plot_setup)
-            line style (List): List of line styles. See <a href="https://matplotlib.org/stable/gallery/lines_bars_and_markers/linestyles.html" target="_blank">gallery</a> (key required in plot_setup) 
-            y axis label (String): y axis label (key required in plot_setup)
-            x axis label (String): x axis label (key required in plot_setup)
-            labels size (Integer): Labels size (key required in plot_setup)
-            labels color (String): Labels color (key required in plot_setup)
-            x axis size (Integer): x axis size (key required in plot_setup)
-            y axis size (Integer): y axis size (key required in plot_setup)
-            axises color (String): Axises color (key required in plot_setup)
-            x limit (List): x axis limits (key required in plot_setup)
-            y limit (List): y axis limits (key required in plot_setup)
-            chart color (List): List of chart colors (key required in plot_setup)
-            on grid? (Boolean): Grid on or off (key required in plot_setup)
-            y log (Boolean): y log scale (key required in plot_setup)
-            x log (Boolean): x log scale (key required in plot_setup)
+            marker_size (List): List of marker sizes (key required in plot_setup)
+            line_width (List): List of line widths (key required in plot_setup)
+            line_style (List): List of line styles. See <a href="https://matplotlib.org/stable/gallery/lines_bars_and_markers/linestyles.html" target="_blank">gallery</a> (key required in plot_setup) 
+            x_axis_label (String): x axis label (key required in plot_setup)
+            x_axis_size (Integer): x axis size (key required in plot_setup)
+            y_axis_label (String): y axis label (key required in plot_setup)
+            y_axis_size (Integer): y axis size (key required in plot_setup)
+            axises_color (String): Axises color (key required in plot_setup)
+            labels_size (Integer): Labels size (key required in plot_setup)
+            labels_color (String): Labels color (key required in plot_setup)
+            chart_color (List): List of chart_colors (key required in plot_setup)
+            x_limit (List): x axis limits (key required in plot_setup)
+            y_limit (List): y axis limits (key required in plot_setup)
+            on_grid (Boolean): Grid on or off (key required in plot_setup)
+            y_log (Boolean): y log scale (key required in plot_setup)
+            x_log (Boolean): x log scale (key required in plot_setup)
             legend (List): List of legends (key required in plot_setup)
-            legend location (String): Legend location (key required in plot_setup)
-            size legend (Integer): Legend size (key required in plot_setup)
+            legend_location (String): Legend location (key required in plot_setup)
+            size_legend (Integer): Legend size (key required in plot_setup)
         dataset (Dictionary): Dataset with the following
             x0 (List or array): x axis values for the first line (key required in dataset)
             y0 (List or array): y axis values for the first line (key required in dataset)
             x1 (List or array): x axis values for the second line (key required in dataset)
             y1 (List or array): y axis values for the second line (key required in dataset)
             xn (List or array): x axis values for the n-th line (key required in dataset)
             yn (List or array): y axis values for the n-th line (key required in dataset)
@@ -182,35 +183,35 @@
     # Chart setup
     plot_setup = kwargs.get('plot_setup')
     plot_setup = keys_to_lower(plot_setup)
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
     extension = plot_setup['extension']
-    dots_per_inch = plot_setup['dots per inch']
+    dots_per_inch = plot_setup['dots_per_inch']
     marker = plot_setup['marker']
-    marker_size = plot_setup['marker size']
-    line_width = plot_setup['line width']
-    line_style = plot_setup['line style']
-    y_axis_label = plot_setup['y axis label']
-    x_axis_label = plot_setup['x axis label']
-    labels_size = plot_setup['labels size']
-    labels_color = plot_setup['labels color']
-    x_axis_size = plot_setup['x axis size']
-    y_axis_size = plot_setup['y axis size']
-    axises_color = plot_setup['axises color']
-    x_limit = plot_setup['x limit']
-    y_limit = plot_setup['y limit']
-    colors = plot_setup['chart color']
-    grid = plot_setup['on grid?']
-    y_log_scale = plot_setup['y log']
-    x_log_scale = plot_setup['x log']
+    marker_size = plot_setup['marker_size']
+    line_width = plot_setup['line_width']
+    line_style = plot_setup['line_style']
+    y_axis_label = plot_setup['y_axis_label']
+    x_axis_label = plot_setup['x_axis_label']
+    labels_size = plot_setup['labels_size']
+    labels_color = plot_setup['labels_color']
+    x_axis_size = plot_setup['x_axis_size']
+    y_axis_size = plot_setup['y_axis_size']
+    axises_color = plot_setup['axises_color']
+    x_limit = plot_setup['x_limit']
+    y_limit = plot_setup['y_limit']
+    colors = plot_setup['chart_color']
+    grid = plot_setup['on_grid']
+    y_log_scale = plot_setup['y_log']
+    x_log_scale = plot_setup['x_log']
     legend = plot_setup['legend']
-    loc_legend = plot_setup['legend location']
-    size_legend = plot_setup['size legend']
+    loc_legend = plot_setup['legend_location']
+    size_legend = plot_setup['size_legend']
 
     # Dataset
     dataset = kwargs.get('dataset')
     data = keys_to_lower(dataset)
     x_dataset = []
     y_dataset = []
     number_of_plots = int(len(data) / 2)
@@ -293,60 +294,60 @@
 
     Args:
         plot_setup (Dictionary): Setup chart Dictionary with the following keys:
             name (String): Path + name figure (key required in plot_setup)
             width (Float): Figure width in SI units (key required in plot_setup)
             height (Float): Figure height in SI units (key required in plot_setup)
             extension (String): File extension (key required in plot_setup)
-            dots per inch (Integer): The resolution in dots per inch (key required in plot_setup)
-            marker size (List): List of marker sizes (key required in plot_setup)
+            dots_per_inch (Integer): The resolution in dots per inch (key required in plot_setup)
+            marker_size (List): List of marker sizes (key required in plot_setup)
             color map (String or List): String for color map values or list of colors in scatterplot. See <a href="https://matplotlib.org/stable/gallery/color/colormap_reference.html" target="_blank">gallery</a> (key required in plot_setup)
-            y axis label (String): y axis label (key required in plot_setup)
-            x axis label (String): x axis label (key required in plot_setup)
-            labels size (Integer): Labels size (key required in plot_setup)
-            labels color (String): Labels color (key required in plot_setup)
-            x axis size (Integer): x axis size (key required in plot_setup)
-            y axis size (Integer): y axis size (key required in plot_setup)
-            axises color (String): Axises color (key required in plot_setup)
-            on grid? (Boolean): Grid on or off (key required in plot_setup)
-            y log (Boolean): y log scale (key required in plot_setup)
-            x log (Boolean): x log scale (key required in plot_setup)
+            y_axis_label (String): y axis label (key required in plot_setup)
+            y_axis_size (Integer): y axis size (key required in plot_setup)
+            x_axis_label (String): x axis label (key required in plot_setup)
+            x_axis_size (Integer): x axis size (key required in plot_setup)
+            labels_size (Integer): Labels size (key required in plot_setup)
+            labels_color (String): Labels color (key required in plot_setup)
+            axises_color (String): Axises color (key required in plot_setup)
+            on_grid (Boolean): Grid on or off (key required in plot_setup)
+            y_log (Boolean): y log scale (key required in plot_setup)
+            x_log (Boolean): x log scale (key required in plot_setup)
             legend (List): List of legends (key required in plot_setup)
-            legend location (String): Legend location (key required in plot_setup)
-            size legend (Integer): Legend size (key required in plot_setup)
+            legend_location (String): Legend location (key required in plot_setup)
+            size_legend (Integer): Legend size (key required in plot_setup)
         dataset (Dictionary): Dataset. Add key 'colorbar' for colorbar in scatterplot
             x0 (List or array): x axis values for the first line (key required in dataset)
             y0 (List or array): y axis values for the first line (key required in dataset)
             x1 (List or array): x axis values for the second line (key required in dataset)
             y1 (List or array): y axis values for the second line (key required in dataset)
             xn (List or array): x axis values for the n-th line (key required in dataset)
             yn (List or array): y axis values for the n-th line (key required in dataset)
-            
+            colorbar (List): List of colorbar values (key required in dataset when colorbar is used. If not, it is not necessary)
     Returns:
         None
     """
 
     # Setup
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
-    marker_size = plot_setup['marker size']
+    marker_size = plot_setup['marker_size']
     color_map = plot_setup['color map']
-    y_axis_label = plot_setup['y axis label']
-    y_axis_size = plot_setup['y axis size']
-    x_axis_label = plot_setup['x axis label']
-    x_axis_size = plot_setup['x axis size']
-    labels_size = plot_setup['labels size']  
-    labels_color = plot_setup['labels color']
-    axises_color = plot_setup['axises color']
-    grid = plot_setup['on grid?']
-    y_log_scale = plot_setup['y log']
-    x_log_scale = plot_setup['x log']
-    dots_per_inch = plot_setup['dots per inch']
+    y_axis_label = plot_setup['y_axis_label']
+    y_axis_size = plot_setup['y_axis_size']
+    x_axis_label = plot_setup['x_axis_label']
+    x_axis_size = plot_setup['x_axis_size']
+    labels_size = plot_setup['labels_size']  
+    labels_color = plot_setup['labels_color']
+    axises_color = plot_setup['axises_color']
+    grid = plot_setup['on_grid']
+    y_log_scale = plot_setup['y_log']
+    x_log_scale = plot_setup['x_log']
+    dots_per_inch = plot_setup['dots_per_inch']
     extension = plot_setup['extension']
 
     # Dataset
     data = kwargs.get('dataset')
 
     # Plot
     w, h = convert_si_to_inches_in_chart_size(w, h)
@@ -354,16 +355,16 @@
     
     if isinstance(color_map, str):
         az = ax.scatter(data['x0'], data['y0'], c=data['colorbar'], marker='o', s=marker_size, cmap=color_map)
         cbar = fig.colorbar(az)
         cbar.ax.tick_params(labelsize=y_axis_size)
     else:
         legend = plot_setup['legend']
-        loc_legend = plot_setup['legend location']
-        size_legend = plot_setup['size legend']
+        loc_legend = plot_setup['legend_location']
+        size_legend = plot_setup['size_legend']
         x_dataset = []
         y_dataset = []
         number_of_plots = int(len(data) / 2)
         for I in range(number_of_plots):
             x_column_name = f'x{I}'
             y_column_name = f'y{I}'
             x_dataset.append(data[x_column_name])
@@ -412,25 +413,25 @@
 
     Args:
         plot_setup (Dictionary): Setup chart Dictionary with the following keys:
             name (String): Path + name figure (key required in plot_setup)
             width (Float): Figure width in SI units (key required in plot_setup)
             height (Float): Figure height in SI units (key required in plot_setup)
             extension (String): File extension (key required in plot_setup)
-            dots per inch (Integer): The resolution in dots per inch (key required in plot_setup)
-            y axis label (String): y axis label (key required in plot_setup)
-            x axis label (String): x axis label (key required in plot_setup)
-            labels size (Integer): Labels size (key required in plot_setup)
-            labels color (String): Labels color (key required in plot_setup)
-            x axis size (Integer): x axis size (key required in plot_setup)
-            y axis size (Integer): y axis size (key required in plot_setup)
-            axises color (String): Axises color (key required in plot_setup)
-            on grid? (Boolean): Grid on or off (key required in plot_setup)
-            y log (Boolean): y log scale (key required in plot_setup)
-            x log (Boolean): x log scale (key required in plot_setup)
+            dots_per_inch (Integer): The resolution in dots per inch (key required in plot_setup)
+            y_axis_label (String): y axis label (key required in plot_setup)
+            x_axis_label (String): x axis label (key required in plot_setup)
+            labels_size (Integer): Labels size (key required in plot_setup)
+            labels_color (String): Labels color (key required in plot_setup)
+            x_axis_size (Integer): x axis size (key required in plot_setup)
+            y_axis_size (Integer): y axis size (key required in plot_setup)
+            axises_color (String): Axises color (key required in plot_setup)
+            on_grid (Boolean): Grid on or off (key required in plot_setup)
+            y_log (Boolean): y log scale (key required in plot_setup)
+            x_log (Boolean): x log scale (key required in plot_setup)
             colors (List): List of colors for the bars (key required in plot_setup)
             bar width (Float): Width of each bar (key required in plot_setup)
             opacity (Float): Opacity of the bars (key required in plot_setup)
   
     Returns:
         None
     """
@@ -439,26 +440,26 @@
     dataset = kwargs.get('dataset')
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
     bar_width = plot_setup['bar width']
     opacity = plot_setup['opacity']
-    y_axis_label = plot_setup['y axis label']
-    x_axis_label = plot_setup['x axis label']
-    x_axis_size = plot_setup['x axis size']
-    y_axis_size = plot_setup['y axis size']
-    axises_color = plot_setup['axises color']
-    labels_size = plot_setup['labels size']
-    labels_color = plot_setup['labels color']
+    y_axis_label = plot_setup['y_axis_label']
+    x_axis_label = plot_setup['x_axis_label']
+    x_axis_size = plot_setup['x_axis_size']
+    y_axis_size = plot_setup['y_axis_size']
+    axises_color = plot_setup['axises_color']
+    labels_size = plot_setup['labels_size']
+    labels_color = plot_setup['labels_color']
     colors = plot_setup['colors']
-    grid = plot_setup['on grid?']  
-    y_log_scale = plot_setup['y log']
+    grid = plot_setup['on_grid']  
+    y_log_scale = plot_setup['y_log']
     extension = plot_setup['extension']
-    dots_per_inch = plot_setup['dots per inch']
+    dots_per_inch = plot_setup['dots_per_inch']
     
     # data
     data = dataset['dataset']
     data_names = list(data.columns)
     data_names = [i.upper() for i in data_names]
     data.columns = data_names
     x = list(data['X'])
@@ -514,16 +515,16 @@
         plot_setup (Dictionary): Setup chart Dictionary with the following keys:
             name (String): Path + name figure (key required in plot_setup)
             width (Float): Figure width in SI units (key required in plot_setup)
             height (Float): Figure height in SI units (key required in plot_setup)
             text color (String): Color of the text extensions (key required in plot_setup)
             text font size (Integer): Font size of the text extensions (key required in plot_setup)
             colors (List): List of colors for the pie slices (key required in plot_setup)
-            size legend (Integer): Font size of the legend (key required in plot_setup)
-            dots per inch (Integer): The resolution in dots per inch (key required in plot_setup)
+            size_legend (Integer): Font size of the legend (key required in plot_setup)
+            dots_per_inch (Integer): The resolution in dots per inch (key required in plot_setup)
             extension (String): File extension (key required in plot_setup)
                 
     Returns:
         None
     """
 
     # Setup
@@ -531,16 +532,16 @@
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
     textension_color = plot_setup['text color']
     textension_font_size = plot_setup['text font size']
     colors = plot_setup['colors']
-    legend_size = plot_setup['size legend']
-    dots_per_inch = plot_setup['dots per inch']
+    legend_size = plot_setup['size_legend']
+    dots_per_inch = plot_setup['dots_per_inch']
     extension = plot_setup['extension']
     
     # dataset
     data = dataset['dataset']
     data_names = list(data.columns)
     data_names = [i.upper() for i in data_names]
     data.columns = data_names
@@ -574,15 +575,15 @@
             height (float): Figure height in SI units (key required in plot_setup)
             text size (integer): Font size of the radar divisions (key required in plot_setup)
             div color (string): Color of the radar divisions (key required in plot_setup)
             radar color (list): List of colors for the radar lines and areas (key required in plot_setup)
             opacity (float): Opacity of the radar areas (key required in plot_setup)
             background (string): Color of the polar background (key required in plot_setup)
             legend size (integer): Font size of the legend (key required in plot_setup)
-            dots per inch (integer): The resolution in dots per inch (key required in plot_setup)
+            dots_per_inch (integer): The resolution in dots per inch (key required in plot_setup)
             extension (string): File extension (key required in plot_setup)
             
     Returns:
         None
     """
     # Setup
     dataset = kwargs.get('dataset')
@@ -592,15 +593,15 @@
     height = plot_setup['height']
     radar_div_size = plot_setup['text size']
     radar_div_color = plot_setup['div color']
     radar_color = plot_setup['radar color']
     opacity = plot_setup['opacity']
     polar_color = plot_setup['background']
     size_legend = plot_setup['legend size']
-    dots_per_inch = plot_setup['dots per inch']
+    dots_per_inch = plot_setup['dots_per_inch']
     extension = plot_setup['extension']
     
     # Data
     data = dataset['dataset']
     data_names = list(data.columns)
     data_names = [i.lower() for i in data_names]
     data.columns = data_names
@@ -658,17 +659,17 @@
 
     Args:
         plot_setup (dictionary): Setup chart dictionary with the following keys:
             name (string): Path + name figure (key required in plot_setup)
             width (float): Figure width in SI units (key required in plot_setup)
             height (float): Figure height in SI units (key required in plot_setup)
             extension (string): File extension (key required in plot_setup)
-            dots per inch (integer): The resolution in dots per inch (key required in plot_setup)
+            dots_per_inch (integer): The resolution in dots per inch (key required in plot_setup)
             mask (boolean): Whether to use a mask for the upper triangle (key required in plot_setup)
-            line widths (float): Width of the lines between cells (key required in plot_setup)
+            line_widths (float): Width of the lines between cells (key required in plot_setup)
             color map (string or list): Color map for the heatmap (key required in plot_setup)
             line color (string): Color of the lines between cells (key required in plot_setup)
             annot (boolean): Whether to annotate each cell with the correlation value (key required in plot_setup)
             annot size font (integer): Font size of the annotations (key required in plot_setup)
             
     Returns:
         None
@@ -677,17 +678,17 @@
     # Setup
     dataset = kwargs.get('dataset')
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
     extension = plot_setup['extension']
-    dots_per_inch = plot_setup['dots per inch']
+    dots_per_inch = plot_setup['dots_per_inch']
     escada = plot_setup['mask']
-    line_widths = plot_setup['line widths']
+    line_widths = plot_setup['line_widths']
     color_map =  plot_setup['color map']
     line_color = plot_setup['line color']
     annot =  plot_setup['annot']
     annot_size_font = plot_setup['annot size font']
     annot_font_weight = 'bold'
 
     # Dataset
@@ -717,15 +718,15 @@
     This function creates a treemap chart.
 
     Args:
         plot_setup (dictionary): Setup chart dictionary with the following keys:
             name (string): Path + name figure (key required in plot_setup)
             width (float): Figure width in SI units (key required in plot_setup)
             height (float): Figure height in SI units (key required in plot_setup)
-            dots per inch (integer): The resolution in dots per inch (key required in plot_setup)
+            dots_per_inch (integer): The resolution in dots per inch (key required in plot_setup)
             extension (string): File extension (key required in plot_setup)
             colors (list): List of colors for the treemap (key required in plot_setup)
             labels (list): List of labels for the treemap (key required in plot_setup)
             label size (integer): Font size of the labels (key required in plot_setup)
             
     Returns:
         None
@@ -733,15 +734,15 @@
 
     # Setup
     dataset = kwargs.get('dataset')
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     width = plot_setup['width']
     height = plot_setup['height']
-    dots_per_inch = plot_setup['dots per inch']
+    dots_per_inch = plot_setup['dots_per_inch']
     extension = plot_setup['extension']
     colors = plot_setup['colors']
     labels = plot_setup['labels']
     label_size = plot_setup['label size']
 
     # Dataset and other information
     values = dataset['dataset']['values']
@@ -770,18 +771,18 @@
 
     # Setup
     dataset = kwargs.get('dataset')
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     width = plot_setup['width']
     height = plot_setup['height']
-    x_axis_size = plot_setup['x axis size']
+    x_axis_size = plot_setup['x_axis_size']
     x_axis_color = plot_setup['X axIS color']
     OVERLAP = 0
-    dots_per_inch = plot_setup['dots per inch']
+    dots_per_inch = plot_setup['dots_per_inch']
     extension = plot_setup['extension']
     
     # dataset
     data = dataset['dataset']
     data_nameS = List(data.columns)
     data_nameS = [i.upper() for i in data_nameS]
     data.columns = data_nameS
@@ -804,32 +805,32 @@
     # Setup
     dataset = kwargs.get('dataset')
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
     extension = plot_setup['extension']
-    dots_per_inch = plot_setup['dots per inch']
+    dots_per_inch = plot_setup['dots_per_inch']
     marker = plot_setup['marker']
-    marker_size = plot_setup['marker size']
-    line_width = plot_setup['line width']
-    line_style = plot_setup['line style']
+    marker_size = plot_setup['marker_size']
+    line_width = plot_setup['line_width']
+    line_style = plot_setup['line_style']
     Y0_axIS_LABEL = plot_setup['Y0 axIS LABEL']
     Y1_axIS_LABEL = plot_setup['Y1 axIS LABEL']
-    x_axis_label = plot_setup['x axis label']
-    labels_size = plot_setup['labels size']     
-    x_axis_size = plot_setup['x axis size']
-    y_axis_size = plot_setup['y axis size']
-    colors = plot_setup['chart color']
-    grid = plot_setup['on grid?']
-    y_log_scale = plot_setup['y log']
-    x_log_scale = plot_setup['x log']
+    x_axis_label = plot_setup['x_axis_label']
+    labels_size = plot_setup['labels_size']     
+    x_axis_size = plot_setup['x_axis_size']
+    y_axis_size = plot_setup['y_axis_size']
+    colors = plot_setup['chart_color']
+    grid = plot_setup['on_grid']
+    y_log_scale = plot_setup['y_log']
+    x_log_scale = plot_setup['x_log']
     legend = plot_setup['legend']
-    loc_legend = plot_setup['legend location']
-    size_legend = plot_setup['size legend']
+    loc_legend = plot_setup['legend_location']
+    size_legend = plot_setup['size_legend']
     
     # dataset and others information
     data = dataset['dataset']
     data_nameS = List(data.columns)
     data_nameS = [i.upper() for i in data_nameS]
     data.columns = data_nameS
     X = List(data['X'])
@@ -882,29 +883,29 @@
 
     # Setup
     dataset = kwargs.get('dataset')
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
-    marker_size = plot_setup['marker size']
+    marker_size = plot_setup['marker_size']
     color_map = plot_setup['SCATTER color']
     line_color = plot_setup['line color']
     ORDER = plot_setup['ORDER'] 
-    y_axis_label = plot_setup['y axis label']
-    y_axis_size = plot_setup['y axis size']
-    x_axis_label = plot_setup['x axis label']
-    x_axis_size = plot_setup['x axis size']
-    labels_size = plot_setup['labels size']  
-    labels_color = plot_setup['labels color']
-    axises_color = plot_setup['axises color']
-    grid = plot_setup['on grid?']
-    y_log_scale = plot_setup['y log']
-    x_log_scale = plot_setup['x log']
-    dots_per_inch = plot_setup['dots per inch']
+    y_axis_label = plot_setup['y_axis_label']
+    y_axis_size = plot_setup['y_axis_size']
+    x_axis_label = plot_setup['x_axis_label']
+    x_axis_size = plot_setup['x_axis_size']
+    labels_size = plot_setup['labels_size']  
+    labels_color = plot_setup['labels_color']
+    axises_color = plot_setup['axises_color']
+    grid = plot_setup['on_grid']
+    y_log_scale = plot_setup['y_log']
+    x_log_scale = plot_setup['x_log']
+    dots_per_inch = plot_setup['dots_per_inch']
     extension = plot_setup['extension']
 
     # data
     data = dataset['dataset']
     data_nameS = List(data.columns)
     data_nameS = [i.upper() for i in data_nameS]
     data.columns = data_nameS
@@ -933,111 +934,204 @@
     if grid == True:
         ax.grid(color = 'grey', linestyle = '-', linewidth = 1, alpha = 0.20)
     
     # Save figure
     save_chart_in_folder(name, extension, dots_per_inch)
 
 
-def scatter_line_plot(dataset, plot_setup): 
+def scatter_line_chart(**kwargs):
     """
-    This function shows a scatter and line chart.
+    This function shows a multiple lines and scatter points in single chart.
 
     Args:
         plot_setup (Dictionary): Setup chart Dictionary with the following keys:
             name (String): Path + name figure (key required in plot_setup)
-            width (Float): Figure width in SI units (key required in plot_setup)
-            height (Float): Figure height in SI units (key required in plot_setup)
+            width (Float): figure width in SI units (key required in plot_setup)
+            height (Float): figure height in SI units (key required in plot_setup)
             extension (String): File extension (key required in plot_setup)
-            dots per inch (Integer): The resolution in dots per inch (key required in plot_setup)
-            marker size (List): List of marker sizes (key required in plot_setup)
-            color map (String or List): Color map for the scatter plot (key required in plot_setup)
-            y axis label (String): y axis label (key required in plot_setup)
-            x axis label (String): x axis label (key required in plot_setup)
-            labels size (Integer): Labels size (key required in plot_setup)
-            labels color (String): Labels color (key required in plot_setup)
-            x axis size (Integer): x axis size (key required in plot_setup)
-            y axis size (Integer): y axis size (key required in plot_setup)
-            axises color (String): Axises color (key required in plot_setup)
-            on grid? (Boolean): Grid on or off (key required in plot_setup)
-            y log (Boolean): y log scale (key required in plot_setup)
-            x log (Boolean): x log scale (key required in plot_setup)
-            
+            dots_per_inch (Integer): The resolution in dots per inch (key required in plot_setup)
+            marker (List): List of markers. See <a href="https://matplotlib.org/stable/gallery/lines_bars_and_markers/marker_reference.html#sphx-glr-gallery-lines-bars-and-markers-marker-reference-py" target="_blank">gallery</a> (key required in plot_setup)
+            marker_size (List): List of marker sizes (key required in plot_setup)
+            line_width (List): List of line widths (key required in plot_setup)
+            line_style (List): List of line styles. See <a href="https://matplotlib.org/stable/gallery/lines_bars_and_markers/linestyles.html" target="_blank">gallery</a> (key required in plot_setup) 
+            x_axis_label (String): x axis label (key required in plot_setup)
+            x_axis_size (Integer): x axis size (key required in plot_setup)
+            y_axis_label (String): y axis label (key required in plot_setup)
+            y_axis_size (Integer): y axis size (key required in plot_setup)
+            axises_color (String): Axises color (key required in plot_setup)
+            labels_size (Integer): Labels size (key required in plot_setup)
+            labels_color (String): Labels color (key required in plot_setup)
+            chart_color (List): List of chart_colors (key required in plot_setup)
+            x_limit (List): x axis limits (key required in plot_setup)
+            y_limit (List): y axis limits (key required in plot_setup)
+            on_grid (Boolean): Grid on or off (key required in plot_setup)
+            y_log (Boolean): y log scale (key required in plot_setup)
+            x_log (Boolean): x log scale (key required in plot_setup)
+            legend line (List): List of legends (key required in plot_setup)
+            legend scatter (List): List of legends (key required in plot_setup)
+            legend_location (String): Legend location (key required in plot_setup)
+            size_legend (Integer): Legend size (key required in plot_setup)
+        dataset_line (Dictionary): Dataset with the following
+            x0 (List or array): x axis values for the first line (key required in dataset)
+            y0 (List or array): y axis values for the first line (key required in dataset)
+            x1 (List or array): x axis values for the second line (key required in dataset)
+            y1 (List or array): y axis values for the second line (key required in dataset)
+            xn (List or array): x axis values for the n-th line (key required in dataset)
+            yn (List or array): y axis values for the n-th line (key required in dataset)
+        dataset_sc (Dictionary): Dataset with the following
+            x0 (List or array): x axis values for the first line (key required in dataset)
+            y0 (List or array): y axis values for the first line (key required in dataset)
+            x1 (List or array): x axis values for the second line (key required in dataset)
+            y1 (List or array): y axis values for the second line (key required in dataset)
+            xn (List or array): x axis values for the n-th line (key required in dataset)
+            yn (List or array): y axis values for the n-th line (key required in dataset)
+
     Returns:
         None
     """
 
-    # Setup
+    # Chart setup
+    plot_setup = kwargs.get('plot_setup')
+    plot_setup = keys_to_lower(plot_setup)
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
-    marker_size = plot_setup['marker size']
-    color_map = plot_setup['color_map color']
-    y_axis_label = plot_setup['y axis label']
-    y_axis_size = plot_setup['y axis size']
-    x_axis_label = plot_setup['x axis label']
-    x_axis_size = plot_setup['x axis size']
-    labels_size = plot_setup['labels size']  
-    labels_color = plot_setup['labels color']
-    line_color = plot_setup['line color']
-    axises_color = plot_setup['axises color']
-    grid = plot_setup['on grid?']
-    y_log_scale = plot_setup['y log']
-    x_log_scale = plot_setup['x log']
-    dpi = plot_setup['dots per inch']
     extension = plot_setup['extension']
+    dots_per_inch = plot_setup['dots_per_inch']
+    marker = plot_setup['marker line']
+    marker_size = plot_setup['marker size line']
+    marker_size_scatter = plot_setup['marker size scatter']
+    line_width = plot_setup['line_width']
+    line_style = plot_setup['line_style']
+    y_axis_label = plot_setup['y_axis_label']
+    x_axis_label = plot_setup['x_axis_label']
+    labels_size = plot_setup['labels_size']
+    labels_color = plot_setup['labels_color']
+    x_axis_size = plot_setup['x_axis_size']
+    y_axis_size = plot_setup['y_axis_size']
+    axises_color = plot_setup['axises_color']
+    x_limit = plot_setup['x_limit']
+    y_limit = plot_setup['y_limit']
+    colors = plot_setup['chart_color line']
+    color_map = plot_setup['color map']
+    grid = plot_setup['on_grid']
+    y_log_scale = plot_setup['y_log']
+    x_log_scale = plot_setup['x_log']
+    legend = plot_setup['legend line']
+    legend_sc = plot_setup['legend scatter']
+    loc_legend = plot_setup['legend_location']
+    size_legend = plot_setup['size_legend']
 
-    # Data
-    X = dataset['X']
-    Y = dataset['Y']
-    Z = dataset['Z']
-
-    LX = dataset['LX']
-    LY1 = dataset['LY1']
-    LY2 = dataset['LY2']   
-
+    # Dataset
+    dataset = kwargs.get('dataset_line')
+    data = keys_to_lower(dataset)
+    dataset_sc = kwargs.get('dataset_sc')
+    data_sc = keys_to_lower(dataset_sc)
+    x_dataset = []
+    y_dataset = []
+    number_of_plots = int(len(data) / 2)
+    for I in range(number_of_plots):
+        x_column_name = f'x{I}'
+        y_column_name = f'y{I}'
+        x_dataset.append(data[x_column_name])
+        y_dataset.append(data[y_column_name])
+    x_dataset_sc = []
+    y_dataset_sc = []
+    number_of_plots_sc = int(len(data_sc) / 2)
+    for I in range(number_of_plots_sc):
+        x_column_name = f'x{I}'
+        y_column_name = f'y{I}'
+        x_dataset_sc.append(data_sc[x_column_name])
+        y_dataset_sc.append(data_sc[y_column_name])
     # Plot
-    # w, h = convert_si_to_inches(w, h)
     w, h = convert_si_to_inches_in_chart_size(w, h)
-    fig, ax = plt.subplots(1, 1, figsize=(w, h), sharex=True)
-    if color_map == False:
-        im = ax.scatter(X, Y, marker='o', s=marker_size)
+    _, ax = plt.subplots(1, 1, figsize = (w, h), sharex=True)
+    for k in range(number_of_plots):
+        if len(legend) == 1:
+            if legend[0] is None:
+                ax.plot(x_dataset[k],
+                        y_dataset[k],
+                        marker=marker[k],
+                        linestyle=line_style[k],
+                        linewidth=line_width[k],
+                        markersize=marker_size[k],
+                        color=colors[k])
+            else:
+                ax.plot(x_dataset[k],
+                        y_dataset[k],
+                        marker=marker[k],
+                        linestyle=line_style[k],
+                        linewidth=line_width[k],
+                        markersize=marker_size[k],
+                        color=colors[k],
+                        label=legend[k])
+        else:
+            ax.plot(x_dataset[k],
+                    y_dataset[k],
+                    marker=marker[k],
+                    linestyle=line_style[k],
+                    linewidth=line_width[k],
+                    markersize=marker_size[k],
+                    color=colors[k],
+                    label=legend[k])
+    for k in range(number_of_plots_sc):
+        if len(color_map) == 1:
+            ax.scatter(x_dataset_sc[k], y_dataset_sc[k], marker='o', s=marker_size_scatter, c=color_map[0], label=legend_sc[0])
+        else:
+            ax.scatter(x_dataset_sc[k], y_dataset_sc[k], marker='o', s=marker_size_scatter, c=color_map[k], label=legend_sc[k])
+    if len(legend) == 1:
+        if legend[0] is None:
+            pass
+        else:
+            plt.legend(loc=loc_legend,
+                    prop={'size': size_legend})
     else:
-        im = ax.scatter(X, Y, c=Z, marker='o', s=marker_size , cmap=color_map)
-    
-    ax.plot(LX, LY1, color=line_color)
-    ax.tick_params(axis='y', labelcolor=line_color)
-
-    ax1 = ax.twinx()
-
-    ax1.plot(LX, [0, 50, 75, 100], line_color)
-    ax1.tick_params(axis='y', labelcolor=line_color)
-    
-    colorbar = plt.colorbar(im)
+        plt.legend(loc=loc_legend,
+                prop={'size': size_legend})
+    if x_limit is not None:
+        plt.xlim(x_limit[0], x_limit[1])
+    if y_limit is not None:
+        plt.ylim(y_limit[0], y_limit[1])
     if y_log_scale:
         ax.semilogy()
     if x_log_scale:
         ax.semilogx()
     font = {'fontname': 'DejaVu Sans',
-                'color':  labels_color,
-                'weight': 'normal',
-                'size': labels_size}
+            'color':  labels_color,
+            'weight': 'normal',
+            'size': labels_size}
     ax.set_ylabel(y_axis_label, fontdict=font)
-    ax.set_xlabel(x_axis_label, fontdict=font)  
-    ax.tick_params(axis='x', labelsize=x_axis_size, colors=axises_color, labelrotation=0, direction='out', which='both', length=10)
+    ax.set_xlabel(x_axis_label, fontdict=font)
+    ax.tick_params(axis='x', labelsize=x_axis_size, colors=axises_color)
     ax.tick_params(axis='y', labelsize=y_axis_size, colors=axises_color)
-    if grid == True:
+    if grid is True:
         ax.grid(color='grey', linestyle='-.', linewidth=1, alpha=0.20)
-    save_chart_in_folder(name, extension, dpi)
+    if len(legend) == 1:
+        if legend[0] is None:
+            pass
+        else:
+            plt.legend(loc=loc_legend,
+                       prop={'size': size_legend})
+    else:
+        plt.legend(loc=loc_legend,
+                   prop={'size': size_legend})
+    plt.tight_layout()
+
+    # Save figure
+    save_chart_in_folder(name, extension, dots_per_inch)
+
+    # Show figure
+    plt.show()
 
 
 def contour_chart(dataset, plot_setup):    
     
     # Setup
     name = plot_setup['name']
-    dots_per_inch = plot_setup['dots per inch']
+    dots_per_inch = plot_setup['dots_per_inch']
     extension = plot_setup['extension']
     TITLE = plot_setup['TITLE']
     LEVELS = plot_setup['LEVELS']
     
     # data
     X = dataset['X']
     Y = dataset['Y']
```

### Comparing `easyplot_toolbox-1.1.0/license.md` & `easyplot_toolbox-1.1.1/license.md`

 * *Files identical despite different names*

### Comparing `easyplot_toolbox-1.1.0/pyproject.toml` & `easyplot_toolbox-1.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "easyplot-toolbox"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = ["wmpjrufg <wanderlei_junior@ufcat.edu.br>", "nerodrakar <luiz_rezio@discente.ufcat.edu.br>"]
-readme = "readme2.md"
+readme = "readme-pypi.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 matplotlib = "^3.8.4"
 pandas = "^2.2.2"
 seaborn = "^0.13.2"
 joypy = "^0.2.6"
```

### Comparing `easyplot_toolbox-1.1.0/readme2.md` & `easyplot_toolbox-1.1.1/readme-pypi.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Easyplot toolbox
 EasyplotPy is a software being developed by the research group headed by professor Wanderlei Malaquias Pereira Junior in Faculty of Engineering at Federal University of Catalão (UFCAT). EasyplotPy algorithm provide an easy workflow to assemble charts and save figures. The framework was developed in Python language.
 
 # Version
+
+### 1.1.1
+
+_feat:_  
+  
+_improvement:_   
+
+_bug:_   
+
+_doc:_  
+- new documentation (histogram_chart);  
+- new documentation (line_chart);  
+
+_config:_ 
+
 ### 1.1.0
 
 _feat:_  
   
 _improvement:_  
 - scatter_chart new plot   
 
@@ -14,15 +29,16 @@
 _doc:_  
 - line_chart new doc  
 - histogram_chart new doc  
 - scatter_chart new doc   
 
 _config:_   
 
-### 1.0.0
+
+### 1.0.0  
 
 _feat:_
 - histogram_chart: This function shows a boxplot and histogram in a single chart.  
 - scatter_chart: This function shows a scatter plot in single chart.
 - scatter_line_plot: This function shows a scatter and line chart.
 
 _improvement:
```

### Comparing `easyplot_toolbox-1.1.0/PKG-INFO` & `easyplot_toolbox-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyplot-toolbox
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 Author: wmpjrufg
 Author-email: wanderlei_junior@ufcat.edu.br
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,14 +18,29 @@
 Requires-Dist: squarify (>=0.4.3,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Easyplot toolbox
 EasyplotPy is a software being developed by the research group headed by professor Wanderlei Malaquias Pereira Junior in Faculty of Engineering at Federal University of Catalão (UFCAT). EasyplotPy algorithm provide an easy workflow to assemble charts and save figures. The framework was developed in Python language.
 
 # Version
+
+### 1.1.1
+
+_feat:_  
+  
+_improvement:_   
+
+_bug:_   
+
+_doc:_  
+- new documentation (histogram_chart);  
+- new documentation (line_chart);  
+
+_config:_ 
+
 ### 1.1.0
 
 _feat:_  
   
 _improvement:_  
 - scatter_chart new plot   
 
@@ -34,15 +49,16 @@
 _doc:_  
 - line_chart new doc  
 - histogram_chart new doc  
 - scatter_chart new doc   
 
 _config:_   
 
-### 1.0.0
+
+### 1.0.0  
 
 _feat:_
 - histogram_chart: This function shows a boxplot and histogram in a single chart.  
 - scatter_chart: This function shows a scatter plot in single chart.
 - scatter_line_plot: This function shows a scatter and line chart.
 
 _improvement:
```

