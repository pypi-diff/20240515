# Comparing `tmp/uqtils-0.3.0.tar.gz` & `tmp/uqtils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uqtils-0.3.0.tar", last modified: Tue Feb 20 01:05:40 2024, max compression
+gzip compressed data, was "uqtils-0.3.1.tar", last modified: Tue May 14 22:32:18 2024, max compression
```

## Comparing `uqtils-0.3.0.tar` & `uqtils-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35149 2024-02-20 01:05:24.997918 uqtils-0.3.0/LICENSE
--rw-r--r--   0        0        0     1366 2024-02-20 01:05:24.997918 uqtils-0.3.0/docs/README.md
--rw-r--r--   0        0        0     1699 2024-02-20 01:05:40.237955 uqtils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      387 2024-02-20 01:05:24.997918 uqtils-0.3.0/src/uqtils/__init__.py
--rw-r--r--   0        0        0     1888 2024-02-20 01:05:24.997918 uqtils-0.3.0/src/uqtils/example.py
--rw-r--r--   0        0        0     4685 2024-02-20 01:05:25.001918 uqtils-0.3.0/src/uqtils/grad.py
--rw-r--r--   0        0        0    12584 2024-02-20 01:05:25.001918 uqtils-0.3.0/src/uqtils/mcmc.py
--rw-r--r--   0        0        0    13314 2024-02-20 01:05:25.001918 uqtils-0.3.0/src/uqtils/plots.py
--rw-r--r--   0        0        0    10930 2024-02-20 01:05:25.001918 uqtils-0.3.0/src/uqtils/sobol.py
--rw-r--r--   0        0        0      771 2024-02-20 01:05:25.001918 uqtils-0.3.0/src/uqtils/uq_types.py
--rw-r--r--   0        0        0        0 2024-02-20 01:05:25.001918 uqtils-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      364 2024-02-20 01:05:25.001918 uqtils-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1892 2024-02-20 01:05:25.001918 uqtils-0.3.0/tests/test_grad.py
--rw-r--r--   0        0        0     1540 2024-02-20 01:05:25.001918 uqtils-0.3.0/tests/test_mcmc.py
--rw-r--r--   0        0        0      722 2024-02-20 01:05:25.001918 uqtils-0.3.0/tests/test_plots.py
--rw-r--r--   0        0        0    42798 1970-01-01 00:00:00.000000 uqtils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-14 22:32:05.628152 uqtils-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1366 2024-05-14 22:32:05.628152 uqtils-0.3.1/docs/README.md
+-rw-r--r--   0        0        0     1699 2024-05-14 22:32:18.400324 uqtils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      387 2024-05-14 22:32:05.628152 uqtils-0.3.1/src/uqtils/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-14 22:32:05.628152 uqtils-0.3.1/src/uqtils/default.mplstyle
+-rw-r--r--   0        0        0     1888 2024-05-14 22:32:05.628152 uqtils-0.3.1/src/uqtils/example.py
+-rw-r--r--   0        0        0     4685 2024-05-14 22:32:05.628152 uqtils-0.3.1/src/uqtils/grad.py
+-rw-r--r--   0        0        0    12584 2024-05-14 22:32:05.632152 uqtils-0.3.1/src/uqtils/mcmc.py
+-rw-r--r--   0        0        0    14184 2024-05-14 22:32:05.632152 uqtils-0.3.1/src/uqtils/plots.py
+-rw-r--r--   0        0        0    10930 2024-05-14 22:32:05.632152 uqtils-0.3.1/src/uqtils/sobol.py
+-rw-r--r--   0        0        0      771 2024-05-14 22:32:05.632152 uqtils-0.3.1/src/uqtils/uq_types.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:32:05.632152 uqtils-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      364 2024-05-14 22:32:05.632152 uqtils-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1892 2024-05-14 22:32:05.632152 uqtils-0.3.1/tests/test_grad.py
+-rw-r--r--   0        0        0     1540 2024-05-14 22:32:05.632152 uqtils-0.3.1/tests/test_mcmc.py
+-rw-r--r--   0        0        0      722 2024-05-14 22:32:05.632152 uqtils-0.3.1/tests/test_plots.py
+-rw-r--r--   0        0        0    42798 1970-01-01 00:00:00.000000 uqtils-0.3.1/PKG-INFO
```

### Comparing `uqtils-0.3.0/LICENSE` & `uqtils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/docs/README.md` & `uqtils-0.3.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/pyproject.toml` & `uqtils-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Topic :: Scientific/Engineering :: Physics",
     "Intended Audience :: Science/Research",
 ]
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Repository = "https://github.com/eckelsjd/uqtils.git"
 Documentation = "https://eckelsjd.github.io/uqtils/"
```

### Comparing `uqtils-0.3.0/src/uqtils/example.py` & `uqtils-0.3.1/src/uqtils/example.py`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/src/uqtils/grad.py` & `uqtils-0.3.1/src/uqtils/grad.py`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/src/uqtils/mcmc.py` & `uqtils-0.3.1/src/uqtils/mcmc.py`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/src/uqtils/plots.py` & `uqtils-0.3.1/src/uqtils/plots.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,33 +18,37 @@
 
 from .uq_types import Array
 from .mcmc import normal_sample
 
 __all__ = ['ax_default', 'plot_slice', 'ndscatter']
 
 
-def ax_default(ax: plt.Axes, xlabel='', ylabel='', legend=False, cmap='tab10'):
-    """Nice default formatting for plotting X-Y data.
+def ax_default(ax: plt.Axes, xlabel='', ylabel='', legend=None, cmap='tab10'):
+    """Nice default plt formatting for plotting X-Y data.
 
     :param ax: the axes to apply these settings to
     :param xlabel: the xlabel to set for `ax`
     :param ylabel: the ylabel to set for `ax`
-    :param legend: whether to show a legend
+    :param legend: will display a legend if bool(legend) is truthy, can pass a dict of legend kwargs here (optional)
     :param cmap: colormap to use for cycling
     """
-    plt.rcParams["axes.prop_cycle"] = _get_cycle(cmap)
-    plt.rc('xtick', labelsize='small')
-    plt.rc('ytick', labelsize='small')
+    default_leg = {'fancybox': True, 'facecolor': 'white', 'framealpha': 1, 'loc': 'best', 'edgecolor': 'k'}
+    leg_use = legend if isinstance(legend, dict) else default_leg
+    for key, val in default_leg.items():
+        if key not in leg_use:
+            leg_use[key] = val
+
+    ax.set_prop_cycle(_get_cycle(cmap))
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     ax.tick_params(axis='both', which='both', direction='in')
+    ax.grid(visible=True)
     if legend:
-        leg = ax.legend(fancybox=True, facecolor='white', framealpha=1)
-        frame = leg.get_frame()
-        frame.set_edgecolor('k')
+        leg = ax.legend(**leg_use)
+        return leg
 
 
 def _get_cycle(cmap: str | matplotlib.colors.Colormap, num_colors: int = None):
     """Get a color cycler for plotting.
 
     :param cmap: a string specifier of a matplotlib colormap (or a colormap instance)
     :param num_colors: the number of colors to cycle through
@@ -151,47 +155,54 @@
     fig.set_size_inches(3 * len(x_idx), 3 * len(y_idx))
     fig.tight_layout()
 
     return fig, axs
 
 
 def ndscatter(samples: np.ndarray, labels: list[str] = None, tick_fmts: list[str] = None,
-              plot: Literal['scatter', 'kde', 'hist'] = 'scatter', cmap='viridis', bins=20, z: np.ndarray = None,
-              cb_label=None, cb_norm='linear', subplot_size=3, cov_overlay=None):
+              plot1d: Literal['kde', 'hist'] = None, plot2d: Literal['scatter', 'kde', 'hist', 'hex'] = 'scatter',
+              cmap='viridis', bins=20, cmin=0, z: np.ndarray = None, cb_label=None, cb_norm='linear',
+              subplot_size=3, cov_overlay=None):
     """Triangle scatter plots of n-dimensional samples.
 
     !!! Warning
         Best for `dim < 10`. You can shrink the `subplot_size` to assist graphics loading time.
 
     :param samples: `(N, dim)` samples to plot
     :param labels: list of axis labels of length `dim`
     :param tick_fmts: list of str.format() specifiers for ticks, e.g `['{x: ^10.2f}', ...]`, of length `dim`
-    :param plot: 'hist' for 2d hist plot, 'kde' for kernel density estimation, or 'scatter' (default)
+    :param plot1d: 'hist' or 'kde' for 1d marginals, defaults to plot2d if None
+    :param plot2d: 'hist' for 2d hist plot, 'kde' for kernel density estimation, 'hex', or 'scatter' (default)
     :param cmap: the matplotlib string specifier of a colormap
     :param bins: number of bins in each dimension for histogram marginals
+    :param cmin: the minimum bin count below which the bins are not displayed
     :param z: `(N,)` a performance metric corresponding to `samples`, used to color code the scatter plot if provided
     :param cb_label: label for color bar (if `z` is provided)
     :param cb_norm: `str` or `plt.colors.Normalize`, normalization method for plotting `z` on scatter plot
     :param subplot_size: size in inches of a single 2d marginal subplot
     :param cov_overlay: `(ndim, ndim)` a covariance matrix to overlay as a Gaussian kde over the samples
     :returns fig, axs: the `plt` Figure and Axes objects, (returns an additional `cb_fig, cb_ax` if `z` is specified)
     """
     N, dim = samples.shape
     x_min = np.min(samples, axis=0)
     x_max = np.max(samples, axis=0)
     if labels is None:
         labels = [f"x{i}" for i in range(dim)]
     if z is None:
-        z = np.zeros(N)
+        z = plt.get_cmap(cmap)(0)
     if cb_label is None:
         cb_label = 'Performance metric'
 
     def tick_format_func(value, pos):
         if np.isclose(value, 0):
             return f'{value:.2f}'
+        if abs(value) > 1000:
+            return f'{value:.2E}'
+        if abs(value) > 100:
+            return f'{int(value):d}'
         if abs(value) > 1:
             return f'{value:.2f}'
         if abs(value) > 0.01:
             return f'{value:.4f}'
         if abs(value) < 0.01:
             return f'{value:.2E}'
     default_ticks = FuncFormatter(tick_format_func)
@@ -229,43 +240,48 @@
 
     # Plot marginals
     for i in range(dim):
         for j in range(dim):
             ax = axs[i, j]
             if i == j:                      # 1d marginals (on diagonal)
                 c = plt.get_cmap(cmap)(0)
+                plot = plot1d if plot1d is not None else plot2d
                 if plot == 'kde':
                     kernel = st.gaussian_kde(samples[:, i])
                     x = np.linspace(x_min[i], x_max[i], 500)
                     ax.fill_between(x, y1=kernel(x), y2=0, lw=0, alpha=0.3, facecolor=c)
                     ax.plot(x, kernel(x), ls='-', c=c, lw=1.5)
                 else:
                     ax.hist(samples[:, i], edgecolor='black', color=c, density=True, alpha=0.5,
                             linewidth=1.2, bins=bins)
                 if cov_overlay is not None:
                     kernel = st.gaussian_kde(x_overlay[:, i])
                     x = np.linspace(x_min[i], x_max[i], 500)
                     ax.fill_between(x, y1=kernel(x), y2=0, lw=0, alpha=0.5, facecolor=[0.5, 0.5, 0.5])
                     ax.plot(x, kernel(x), ls='-', c='k', lw=1.5, alpha=0.5)
+                bottom, top = ax.get_ylim()
+                ax.set_ylim([0, top])
             if j < i:                       # 2d marginals (lower triangle)
                 ax.set_xlim([x_min[j], x_max[j]])
                 ax.set_ylim([x_min[i], x_max[i]])
-                if plot == 'scatter':
+                if plot2d == 'scatter':
                     sc = ax.scatter(samples[:, j], samples[:, i], s=1.5, c=z, cmap=cmap, norm=cb_norm)
-                elif plot == 'hist':
-                    ax.hist2d(samples[:, j], samples[:, i], bins=bins, density=True, cmap=cmap)
-                elif plot == 'kde':
+                elif plot2d == 'hist':
+                    ax.hist2d(samples[:, j], samples[:, i], bins=bins, cmap=cmap, cmin=cmin)
+                elif plot2d == 'kde':
                     kernel = st.gaussian_kde(samples[:, [j, i]].T)
-                    xg, yg = np.meshgrid(np.linspace(x_min[j], x_max[j], 50), np.linspace(x_min[i], x_max[i], 50))
+                    xg, yg = np.meshgrid(np.linspace(x_min[j], x_max[j], 40), np.linspace(x_min[i], x_max[i], 40))
                     x = np.vstack([xg.ravel(), yg.ravel()])
                     zg = np.reshape(kernel(x), xg.shape)
                     cs = ax.contourf(xg, yg, zg, 5, cmap=cmap, alpha=0.9, extend='both')
                     cs.cmap.set_under('white')
                     cs.changed()
                     ax.contour(xg, yg, zg, 5, colors=[(0.5, 0.5, 0.5)], linewidths=1.2)
+                elif plot2d == 'hex':
+                    ax.hexbin(samples[:, j], samples[:, i], gridsize=bins, cmap=cmap, mincnt=cmin)
                 else:
                     raise NotImplementedError('This plot type is not known. plot=["hist", "kde", "scatter"]')
 
                 if cov_overlay is not None:
                     kernel = st.gaussian_kde(x_overlay[:, [j, i]].T)
                     xg, yg = np.meshgrid(np.linspace(x_min[j], x_max[j], 40), np.linspace(x_min[i], x_max[i], 40))
                     x = np.vstack([xg.ravel(), yg.ravel()])
@@ -273,15 +289,15 @@
                     ax.contourf(xg, yg, zg, 4, cmap='Greys', alpha=0.4)
                     ax.contour(xg, yg, zg, 4, colors='k', linewidths=1.5, alpha=0.6)
 
     fig.set_size_inches(subplot_size * dim, subplot_size * dim)
     fig.tight_layout()
 
     # Plot colorbar in standalone figure
-    if np.max(z) > 0 and plot == 'scatter':
+    if np.max(z) > 0 and plot2d == 'scatter':
         cb_fig, cb_ax = plt.subplots(figsize=(1.5, 6))
         cb_fig.subplots_adjust(right=0.7)
         cb_fig.colorbar(sc, cax=cb_ax, orientation='vertical', label=cb_label)
         cb_fig.tight_layout()
         return fig, axs, cb_fig, cb_ax
 
     return fig, axs
```

### Comparing `uqtils-0.3.0/src/uqtils/sobol.py` & `uqtils-0.3.1/src/uqtils/sobol.py`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/src/uqtils/uq_types.py` & `uqtils-0.3.1/src/uqtils/uq_types.py`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/tests/test_grad.py` & `uqtils-0.3.1/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/tests/test_mcmc.py` & `uqtils-0.3.1/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/tests/test_plots.py` & `uqtils-0.3.1/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `uqtils-0.3.0/PKG-INFO` & `uqtils-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: uqtils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Assorted utilities for uncertainty quantification and scientific computing.
-Keywords: Uncertainty quantification Bayesian
+Keywords: Uncertainty quantification,Bayesian
 Author-Email: Joshua Eckels <eckelsjd@umich.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

