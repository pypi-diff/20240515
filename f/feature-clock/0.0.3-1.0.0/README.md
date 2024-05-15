# Comparing `tmp/feature_clock-0.0.3.tar.gz` & `tmp/feature_clock-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_clock-0.0.3.tar", last modified: Wed Apr 10 00:57:57 2024, max compression
+gzip compressed data, was "feature_clock-1.0.0.tar", last modified: Wed May 15 15:55:55 2024, max compression
```

## Comparing `feature_clock-0.0.3.tar` & `feature_clock-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,27 @@
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.822473 feature_clock-0.0.3/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    11356 2024-03-27 01:55:39.000000 feature_clock-0.0.3/LICENSE
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3205 2024-04-10 00:57:57.822250 feature_clock-0.0.3/PKG-INFO
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      897 2024-04-07 19:03:08.000000 feature_clock-0.0.3/README.md
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1924 2024-04-10 00:56:54.000000 feature_clock-0.0.3/pyproject.toml
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       38 2024-04-10 00:57:57.822519 feature_clock-0.0.3/setup.cfg
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.815426 feature_clock-0.0.3/src/
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.816784 feature_clock-0.0.3/src/feature_clock/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        0 2024-02-16 15:04:27.000000 feature_clock-0.0.3/src/feature_clock/__init__.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1265 2024-03-27 01:35:12.000000 feature_clock-0.0.3/src/feature_clock/graph.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    47421 2024-04-10 00:41:31.000000 feature_clock-0.0.3/src/feature_clock/plot.py
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.821914 feature_clock-0.0.3/src/feature_clock.egg-info/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3205 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/PKG-INFO
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      605 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/SOURCES.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        1 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/dependency_links.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      799 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/requires.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       14 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/top_level.txt
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.821173 feature_clock-0.0.3/test/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     9874 2024-04-07 23:09:41.000000 feature_clock-0.0.3/test/test_bankrupcy.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12360 2024-04-07 23:09:42.000000 feature_clock-0.0.3/test/test_cancer.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5899 2024-04-07 23:09:45.000000 feature_clock-0.0.3/test/test_gaussians.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5574 2024-04-07 23:10:02.000000 feature_clock-0.0.3/test/test_gene_expr.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    22299 2024-04-07 23:10:04.000000 feature_clock-0.0.3/test/test_iris.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12881 2024-04-10 00:52:12.000000 feature_clock-0.0.3/test/test_melody.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    27733 2024-04-09 23:58:30.000000 feature_clock-0.0.3/test/test_neftel.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    13901 2024-04-10 00:10:01.000000 feature_clock-0.0.3/test/test_pima.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12620 2024-04-07 23:10:00.000000 feature_clock-0.0.3/test/test_pima_autoencoder.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8103 2024-04-10 00:02:31.000000 feature_clock-0.0.3/test/test_pima_nn.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8329 2024-04-10 00:05:40.000000 feature_clock-0.0.3/test/test_pima_nn_2out.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5574 2024-04-07 23:09:49.000000 feature_clock-0.0.3/test/test_real_data.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    41830 2024-04-09 20:49:21.000000 feature_clock-0.0.3/test/test_support.py
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.950626 feature_clock-1.0.0/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    11356 2024-03-27 01:55:39.000000 feature_clock-1.0.0/LICENSE
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5623 2024-05-15 15:55:55.950407 feature_clock-1.0.0/PKG-INFO
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3019 2024-05-15 15:24:57.000000 feature_clock-1.0.0/README.md
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     2190 2024-05-15 15:55:44.000000 feature_clock-1.0.0/pyproject.toml
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       38 2024-05-15 15:55:55.950673 feature_clock-1.0.0/setup.cfg
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.944155 feature_clock-1.0.0/src/
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.945310 feature_clock-1.0.0/src/feature_clock/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        0 2024-02-16 15:04:27.000000 feature_clock-1.0.0/src/feature_clock/__init__.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1298 2024-05-15 15:33:23.000000 feature_clock-1.0.0/src/feature_clock/graph.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    51437 2024-05-15 15:33:17.000000 feature_clock-1.0.0/src/feature_clock/plot.py
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.950092 feature_clock-1.0.0/src/feature_clock.egg-info/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5623 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/PKG-INFO
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      513 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        1 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      799 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/requires.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       14 2024-05-15 15:55:55.000000 feature_clock-1.0.0/src/feature_clock.egg-info/top_level.txt
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-05-15 15:55:55.949343 feature_clock-1.0.0/test/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    13015 2024-05-15 15:36:34.000000 feature_clock-1.0.0/test/test_cancer.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    15674 2024-05-15 15:33:01.000000 feature_clock-1.0.0/test/test_iris.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    15838 2024-05-15 15:33:30.000000 feature_clock-1.0.0/test/test_melody.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    28749 2024-05-15 15:34:13.000000 feature_clock-1.0.0/test/test_neftel.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    16859 2024-05-15 15:33:57.000000 feature_clock-1.0.0/test/test_pima.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    13372 2024-05-15 15:32:18.000000 feature_clock-1.0.0/test/test_pima_autoencoder.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8460 2024-05-15 15:32:41.000000 feature_clock-1.0.0/test/test_pima_nn.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8620 2024-05-15 15:32:43.000000 feature_clock-1.0.0/test/test_pima_nn_2out.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    48933 2024-05-15 15:33:49.000000 feature_clock-1.0.0/test/test_support.py
```

### Comparing `feature_clock-0.0.3/LICENSE` & `feature_clock-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feature_clock-0.0.3/pyproject.toml` & `feature_clock-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "feature_clock"
-version = "0.0.3"
+version = "1.0.0"
 authors = [
   { name="Olga Ovcharenko", email="ovcharenko.folga@gmail.com" },
 ]
 description = "Feature Clock, provides visualizations that eliminate the need for multiple plots to inspect the influence of original variables in the latent space. Feature Clock enhances the explainability and compactness of visualizations of embedded data."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
@@ -60,9 +60,12 @@
     "tqdm==4.66.2",
     "tzdata==2024.1",
     "umap-learn==0.5.5",
     "wrapt==1.16.0"
 ]
 
 [project.urls]
-Homepage = "https://github.com/OlgaOvcharenko/feature_clock_visualization"
+Homepage = "https://pypi.org/project/feature-clock/"
+Repository = "https://github.com/OlgaOvcharenko/feature_clock_visualization"
+Documentation = "https://github.com/OlgaOvcharenko/feature_clock_visualization/blob/main/tutorials/docs.md"
+Tutorial = "https://github.com/OlgaOvcharenko/feature_clock_visualization/blob/main/tutorials/iris.md"
 Issues = "https://github.com/OlgaOvcharenko/feature_clock_visualization/issues"
```

### Comparing `feature_clock-0.0.3/src/feature_clock/graph.py` & `feature_clock-1.0.0/src/feature_clock/graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 import sys
- 
- 
-class Graph():
+
+
+class Graph:
     def __init__(self, vertices):
         self.V = vertices
         self.graph = [[0 for column in range(vertices)]
                       for row in range(vertices)]
- 
+
     def printMST(self, parent):
         print("Edge \tWeight")
         for i in range(1, self.V):
             print(parent[i], "-", i, "\t", self.graph[i][parent[i]])
- 
+
     def minKey(self, key, mstSet):
         min = sys.maxsize
- 
+
         for v in range(self.V):
             if key[v] < min and mstSet[v] == False:
                 min = key[v]
                 min_index = v
- 
+
         return min_index
- 
+
     def primMST(self):
         key = [sys.maxsize] * self.V
-        parent = [None] * self.V  
+        parent = [None] * self.V
         key[0] = 0
         mstSet = [False] * self.V
- 
-        parent[0] = -1 
- 
+
+        parent[0] = -1
+
         for cout in range(self.V):
             u = self.minKey(key, mstSet)
- 
+
             mstSet[u] = True
             for v in range(self.V):
-                if self.graph[u][v] > 0 and mstSet[v] == False \
-                and key[v] > self.graph[u][v]:
+                if (
+                    self.graph[u][v] > 0
+                    and mstSet[v] == False
+                    and key[v] > self.graph[u][v]
+                ):
                     key[v] = self.graph[u][v]
                     parent[v] = u
- 
+
         res = []
         for i in range(1, self.V):
             res.append([parent[i], i, self.graph[i][parent[i]]])
-            
+
         return res
-
```

### Comparing `feature_clock-0.0.3/src/feature_clock/plot.py` & `feature_clock-1.0.0/src/feature_clock/plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     ):
         self.is_projected = False
 
         self.high_dim_data = high_dim_data
         self.observations = observations
         low_dim_data = np.array(low_dim_data)
         cluster_labels = np.array(cluster_labels)
-        self.low_dim_data = pd.DataFrame(low_dim_data, columns=["emb1", "emb2"])
+        self.low_dim_data = pd.DataFrame(
+            low_dim_data, columns=["emb1", "emb2"])
 
         if cluster_labels is not None:
             self.cluster_labels = cluster_labels
         elif self.low_dim_data is not None:
             self.cluster_labels = self._compute_HDBSCAN_hulls()
         else:
             self.cluster_labels = None
@@ -135,16 +136,17 @@
         )
         y_new = point[1] * math.cos(math.radians(angle)) - point[0] * math.sin(
             math.radians(angle)
         )
         return [x_new, y_new]
 
     def _project_line(
-        self, data, angle: float, point_a: list = [0, 0], point_b: list = [1, 1]
-    ):
+        self, data, angle: float, point_a: list = [
+            0, 0], point_b: list = [
+            1, 1]):
         line = Line.from_points(point_a=point_a, point_b=point_b)
 
         projected_points = []
         for i in range(data.shape[0]):
             point = (data["emb1"][i], data["emb2"][i])
             new_point = line.project_point(point)
             new_point = self._rotate(new_point, angle)
@@ -180,24 +182,29 @@
                 point_a=[0, 0],
                 point_b=self._get_slope_from_angle(angle),
             )
             for angle in self.angles
         ]
         self.projections = np.array(projections).T
 
-    def _get_importance(self, X, y, significance: float = 0.05, univar: bool = False):
+    def _get_importance(
+            self,
+            X,
+            y,
+            significance: float = 0.05,
+            univar: bool = False):
         coefs, pvals, is_significant, std_x, std_y = [], [], [], [], []
-        
+
         remove_cols = []
         for j in range(X.shape[1]):
-            val1 = X[0, j] 
+            val1 = X[0, j]
             for i in range(X.shape[0]):
                 if X[i, j] != val1:
                     break
-                if i == X.shape[0]-1 and X[i, j] == val1:
+                if i == X.shape[0] - 1 and X[i, j] == val1:
                     remove_cols.append(j)
         for k in remove_cols:
             X = np.delete(X, k, 1)
 
         for i in range(y.shape[1]):
             if univar:
                 coefs_a, pvals_a, is_significant_a = [], [], []
@@ -211,25 +218,26 @@
                 std_x.append(np.ones((len(coefs_a),)))
                 std_y.append(np.ones((len(coefs_a),)))
                 pvals.append(pvals_a)
                 is_significant.append(is_significant_a)
 
             else:
                 # lm = sm.OLS(y[:, i], X).fit()
+                # .fit_regularized("sqrt_lasso", refir=True, L1_wt=0.5)
                 lm = sm.OLS(y[:, i], np.c_[np.ones(X.shape[0]), X]).fit()
-                
+
                 coefs_tmp = lm.params[1:]
                 pvals_tmp = lm.pvalues[1:]
                 x_std_tmp = X.std(axis=0)
-                
+
                 for k in remove_cols:
                     coefs_tmp = np.insert(coefs_tmp, k, 0)
                     pvals_tmp = np.insert(pvals_tmp, k, 0)
                     x_std_tmp = np.insert(x_std_tmp, k, 1)
-                    
+
                 coefs.append(np.array(coefs_tmp))
 
                 pval = np.array(pvals_tmp)
                 pvals.append(pval)
                 is_significant.append(pval <= significance)
 
                 std_x.append(np.array(x_std_tmp))
@@ -238,60 +246,66 @@
         return (
             np.array(coefs),
             np.array(pvals),
             np.array(is_significant),
             np.array(std_x),
             np.array(std_y),
         )
-    
+
     def _logit_pvalue(self, model, x):
-        """ Calculate z-scores for scikit-learn LogisticRegression.
+        """Calculate z-scores for scikit-learn LogisticRegression.
         parameters:
             model: fitted sklearn.linear_model.LogisticRegression with intercept and large C
             x:     matrix on which the model was fit
         This function uses asymtptics for maximum likelihood estimates.
         """
         p = model.predict_proba(x)
         n = len(p)
         m = len(model.coef_[0]) + 1
         coefs = np.concatenate([model.intercept_, model.coef_[0]])
-        x_full = np.matrix(np.insert(np.array(x), 0, 1, axis = 1))
+        x_full = np.matrix(np.insert(np.array(x), 0, 1, axis=1))
         ans = np.zeros((m, m))
         for i in range(n):
-            ans = ans + np.dot(np.transpose(x_full[i, :]), x_full[i, :]) * p[i,1] * p[i, 0]
+            ans = (ans +
+                   np.dot(np.transpose(x_full[i, :]), x_full[i, :]) *
+                   p[i, 1] *
+                   p[i, 0])
         vcov = np.linalg.inv(np.matrix(ans))
         se = np.sqrt(np.diag(vcov))
-        t =  coefs/se  
+        t = coefs / se
         p = (1 - norm.cdf(abs(t))) * 2
         return p
 
-
-    def _get_importance_between(self, X, mst, significance: float = 0.05, univar: bool = False):
+    def _get_importance_between(
+        self, X, mst, significance: float = 0.05, univar: bool = False
+    ):
         coefs, pvals, is_significant, std_x, std_y = [], [], [], [], []
 
         for val in mst:
-            ix = np.logical_or((self.cluster_labels == val[0]), (self.cluster_labels == val[1]))
+            ix = np.logical_or(
+                (self.cluster_labels == val[0]),
+                (self.cluster_labels == val[1]))
             X_i = X[ix]
-            y = self.cluster_labels[np.logical_or((self.cluster_labels == val[0]), (self.cluster_labels == val[1]))]
-            lm = LogisticRegressionCV(cv=5, fit_intercept=True, penalty="l2").fit(X_i, y)
+            y = self.cluster_labels[np.logical_or(
+                (self.cluster_labels == val[0]), (self.cluster_labels == val[1]))]
+            lm = LogisticRegressionCV(
+                cv=5,
+                fit_intercept=True,
+                penalty="l2").fit(
+                X_i,
+                y)
 
             pval = np.array(self._logit_pvalue(lm, X_i)[1:])
             coefs.append(np.array(lm.coef_[0]))
             pvals.append(pval)
             is_significant.append(pval <= significance)
 
             std_x.append(X_i.std(axis=0))
             std_y.append(y.std())
 
-            # for i, val in enumerate(self.observations):
-            #     print(val)
-            #     print(lm.coef_[0][i])
-            #     print(pval[i])
-            #     print(pval[i] <= significance)
-
         return (
             np.array(coefs),
             np.array(pvals),
             np.array(is_significant),
             np.array(std_x),
             np.array(std_y),
         )
@@ -322,23 +336,55 @@
             if np.isnan(coefs).any():
                 coefs = np.nan_to_num(coefs)
                 warnings.warn(
                     "NaNs were introduced after standartizing coefficients and were replaced by 0."
                 )
 
         if biggest_arrow:
-            is_significant = np.logical_or(is_significant[0], is_significant[1])
             coefs_points = [[x, y] for x, y in zip(coefs[0], coefs[1])]
-            coefs_new = np.array(
-                [math.sqrt((x * x) + (y * y)) for x, y in zip(coefs[0], coefs[1])]
-            )
+            coefs_new = np.array([math.sqrt((x * x) + (y * y))
+                                  for x, y in zip(coefs[0], coefs[1])])
+
+            # is_significant = np.logical_or(is_significant[0], is_significant[1])
+            is_significant_tmp = np.zeros(is_significant[0].shape)
+            for i in range(is_significant[0].shape[0]):
+                if is_significant[0][i] or is_significant[1][i]:
+                    is_significant_tmp[i] = True
+                else:
+                    print("\nBoth False values.")
+
+                    # Project and rotate
+                    angle = math.degrees(math.atan(coefs[1][i] / coefs[0][i]))
+                    proj_tmp = self._project_line(
+                        self.low_dim_data,
+                        angle,
+                        point_a=[0, 0],
+                        point_b=coefs_points[i],
+                    )
+
+                    # Predict
+                    coefs_tmp, p_val_tmp, is_s_tmp, _, _ = self._get_importance(
+                        self.high_dim_data.to_numpy(),
+                        np.array([proj_tmp]).T,
+                        univar=univar_importance,
+                        significance=feature_significance,
+                    )
+                    print(coefs_tmp[0][i])
+                    print(coefs_new[i])
+                    print(is_s_tmp[0][i])
+                    print(p_val_tmp[0][i])
+
+                    is_significant_tmp[i] = is_s_tmp[0][i]
+            is_significant = np.array(is_significant_tmp)
 
             if plot_top_k != 0:
                 min_ix = list(
-                    np.argsort(np.abs(coefs_new) * is_significant)[0 : len(coefs_new) - plot_top_k]
+                    np.argsort(np.abs(coefs_new) * is_significant)[
+                        0: len(coefs_new) - plot_top_k
+                    ]
                 )  # FISME * is_significant
 
                 is_significant[min_ix] = False
 
             coefs = coefs_new
 
             arrows, arrow_labels = self._plot_central(
@@ -357,15 +403,15 @@
                 points=coefs_points,
             )
 
         else:
             if plot_top_k != 0:
                 min_ix = list(
                     np.argsort(np.max(np.abs(coefs * is_significant), axis=0))[
-                        0 : coefs.shape[1] - plot_top_k
+                        0: coefs.shape[1] - plot_top_k
                     ]
                 )
                 is_significant[:, min_ix] = False
 
             arrows, arrow_labels = self._plot_central(
                 ax,
                 self.low_dim_data,
@@ -448,25 +494,33 @@
                     )
                 )
                 labels_all.append(lbl)
 
         return arrows, labels_all
 
     def _add_circle_contributions(
-        self, ax, coefs_scaled, is_significant, labels, x_center, y_center, arrow_width
-    ):
+            self,
+            ax,
+            coefs_scaled,
+            is_significant,
+            labels,
+            x_center,
+            y_center,
+            arrow_width):
         arrows, labels_all = [], []
         for a, c, s in zip(self.angles, coefs_scaled, is_significant):
             a = math.radians(a)
 
             # Plot contributions
             ind = abs(c).argsort(axis=None)[::-1]
-            x_add_coefs, y_add_coefs = math.cos(a) * c[ind], math.sin(a) * c[ind]
+            x_add_coefs, y_add_coefs = math.cos(
+                a) * c[ind], math.sin(a) * c[ind]
 
-            for is_s, x_c, y_c, i in zip(s[ind], x_add_coefs, y_add_coefs, ind):
+            for is_s, x_c, y_c, i in zip(
+                    s[ind], x_add_coefs, y_add_coefs, ind):
                 # if is_s: does not make sense since we want to see circles
                 col = self.colors[self.observations[i]]
                 lbl = labels[i]
                 arrows.append(
                     ax.arrow(
                         x_center,
                         y_center,
@@ -479,16 +533,23 @@
                     )
                 )
                 labels_all.append(lbl)
 
         return arrows, labels_all
 
     def _make_circles(
-        self, ax, num_circles, annotate, x_center, y_center, radius, c_max, c_min
-    ):
+            self,
+            ax,
+            num_circles,
+            annotate,
+            x_center,
+            y_center,
+            radius,
+            c_max,
+            c_min):
         for i in list(range(1, num_circles))[::-1]:
             radius_circle = round(i * annotate, 1)
             if i == num_circles - 1:
                 circle = patches.Circle(
                     (x_center, y_center),
                     radius=radius_circle,
                     edgecolor="gray",
@@ -534,15 +595,15 @@
         x_center,
         y_center,
         radius,
         c_min,
         c_max,
         ann_sign=[1, 1],
         clock_label="",
-        clock_label_angle=270
+        clock_label_angle=270,
     ):
         for i in list(range(1, num_circles))[::-1]:
             radius_circle = round(i * annotate, 1)
             if i == num_circles - 1:
                 circle = patches.Circle(
                     (x_center, y_center),
                     radius=radius_circle,
@@ -563,15 +624,15 @@
                 ax.annotate(
                     clock_label,
                     xy=(x_ann, y_ann),
                     ha="center",
                     color="gray",
                     path_effects=[pe.withStroke(linewidth=2, foreground="white")],
                     fontsize=7,
-                    zorder=20
+                    zorder=20,
                 )
             else:
                 circle = patches.Circle(
                     (x_center, y_center),
                     radius=radius_circle,
                     edgecolor="gray",
                     linewidth=1,
@@ -615,20 +676,25 @@
         points: list = [],
     ):
         alpha = 0.1
 
         if plot_scatter:
             # Scatter plot
             ax.scatter(
-                data["emb1"], data["emb2"], color="gray", s=1, alpha=alpha, zorder=0
-            )
+                data["emb1"],
+                data["emb2"],
+                color="gray",
+                s=1,
+                alpha=alpha,
+                zorder=0)
 
         # Add circles lines
         x_center, y_center = self._get_center(data)
-        x_center, y_center = x_center + move_circle[0], y_center + move_circle[1]
+        x_center, y_center = x_center + \
+            move_circle[0], y_center + move_circle[1]
         radius = np.abs(coefs).max() * scale_circle
         c_min, c_max = self._get_cmin_cmax(coefs=coefs)
         num_circles = math.floor(radius / annotate) + 1
         coefs_scaled = coefs * (radius / max(abs(c_max), abs(c_min)))
         self._add_circles_lines(
             ax, num_circles, annotate, angles_shift, x_center, y_center
         )
@@ -643,15 +709,16 @@
                 labels,
                 x_center,
                 y_center,
                 arrow_width,
             )
         else:
             if len(points) != len(labels):
-                raise Exception(f"Points for biggest arrow method are not computed.")
+                raise Exception(
+                    f"Points for biggest arrow method are not computed.")
 
             tmp_points = []
             counts = np.zeros((4,))
             for point in points:
                 new_x = point[0] * (radius / max(abs(c_max), abs(c_min)))
                 new_y = point[1] * (radius / max(abs(c_max), abs(c_min)))
                 tmp_points.append([new_x, new_y])
@@ -697,33 +764,43 @@
             c_min,
             c_max,
             ann_sign=ann_sign,
         )
         return arrows, arrow_labels
 
     def _draw_clusters(self, ax, data, alpha):
-        print(data["cluster"].unique())
+        # print(data["cluster"].unique())
         for i in data["cluster"].unique():
             if i >= 0:
                 points = data[data["cluster"] == i]
                 if points.shape[0] > 2:
                     hull = ConvexHull(points[["emb1", "emb2"]].to_numpy())
                     vert = np.append(hull.vertices, hull.vertices[0])
 
                     a, b = points["emb1"].iloc[vert], points["emb2"].iloc[vert]
                     ax.plot(a, b, "--", c="gray", alpha=alpha)
                     ax.fill(a, b, alpha=alpha, c="gray")
 
-    def _get_plot(self, ax, data, draw_hulls: bool = True, plot_scatter: bool = True):
+    def _get_plot(
+            self,
+            ax,
+            data,
+            draw_hulls: bool = True,
+            plot_scatter: bool = True):
         alpha = 0.1
         print(draw_hulls)
         if draw_hulls:
             self._draw_clusters(ax, data, alpha)
         if plot_scatter:
-            ax.scatter(data["emb1"], data["emb2"], color="gray", s=2, alpha=alpha)
+            ax.scatter(
+                data["emb1"],
+                data["emb2"],
+                color="gray",
+                s=2,
+                alpha=alpha)
 
     def _plot_small(
         self,
         ax,
         data,
         angles_shift,
         angles,
@@ -733,15 +810,15 @@
         biggest_arrow: bool = True,
         scale_circle: float = 1.0,
         annotate: float = 0.2,
         move_circle: list = [0, 0],
         arrow_width: float = 0.01,
         points: list = [],
         clock_label: str = "",
-        clocks_label_angle: float = 270
+        clocks_label_angle: float = 270,
     ):
         x_center, y_center = self._get_center(data)
 
         x_center += move_circle[0]
         y_center += move_circle[1]
 
         radius = np.abs(coefs).max() * scale_circle
@@ -760,17 +837,19 @@
 
         if not biggest_arrow:
             for a, c, s in zip(angles, coefs_scaled, is_significant):
                 a = math.radians(a)
 
                 # Plot contributions
                 ind = abs(c).argsort(axis=None)[::-1]
-                x_add_coefs, y_add_coefs = math.cos(a) * c[ind], math.sin(a) * c[ind]
+                x_add_coefs, y_add_coefs = math.cos(
+                    a) * c[ind], math.sin(a) * c[ind]
 
-                for is_s, x_c, y_c, i in zip(s[ind], x_add_coefs, y_add_coefs, ind):
+                for is_s, x_c, y_c, i in zip(
+                        s[ind], x_add_coefs, y_add_coefs, ind):
                     if is_s:
                         col = self.colors[self.observations[i]]
                         lbl = labels[i]
                         arrows.append(
                             ax.arrow(
                                 x_center,
                                 y_center,
@@ -781,15 +860,16 @@
                                 label=lbl,
                                 zorder=15,
                             )
                         )
 
         else:
             if len(points) != len(labels):
-                raise Exception(f"Points for biggest arrow method are not computed.")
+                raise Exception(
+                    f"Points for biggest arrow method are not computed.")
 
             ix_col_by_len = np.argsort(coefs_scaled)[::-1]
             tmp_points = []
             counts = np.zeros((4,))
             for point in points:
                 new_x = point[0] * (radius / max(abs(c_max), abs(c_min)))
                 new_y = point[1] * (radius / max(abs(c_max), abs(c_min)))
@@ -840,15 +920,15 @@
             x_center,
             y_center,
             radius,
             c_min,
             c_max,
             ann_sign=ann_sign,
             clock_label=clock_label,
-            clock_label_angle=clocks_label_angle
+            clock_label_angle=clocks_label_angle,
         )
 
         return arrows, labels_all
 
     def _plot_small_clock(
         self,
         ax,
@@ -860,19 +940,20 @@
         move_circle,
         annotate,
         arrow_width,
         plot_scatter,
         plot_hulls,
         plot_top_k,
         clocks_labels,
-        clocks_labels_angles
+        clocks_labels_angles,
     ):
         dist_clusters = self.low_dim_data["cluster"].unique()
         dist_clusters.sort()
-        dist_clusters = dist_clusters[1:] if dist_clusters[0] == -1 else dist_clusters
+        dist_clusters = dist_clusters[1:] if dist_clusters[0] == - \
+            1 else dist_clusters
 
         self._get_plot(ax, self.low_dim_data, plot_hulls, plot_scatter)
 
         all_coeffs, all_is_significant, all_points, all_std_x, all_std_y = (
             [],
             [],
             [],
@@ -881,49 +962,79 @@
         )
         arrows_dict = {}
         for cl in dist_clusters:
             ind = (self.low_dim_data["cluster"] == cl).values.reshape(
                 (self.low_dim_data.shape[0], 1)
             )
 
-
             data_cl = self.low_dim_data[ind]
             new_data_cl = self.high_dim_data[ind]
             projections_cl = self.projections[ind[:, 0], :]
 
             coefs, _, is_significant, std_x, std_y = self._get_importance(
                 new_data_cl.to_numpy(),
                 projections_cl,
                 univar=univar_importance,
                 significance=feature_significance,
             )
 
             if biggest_arrow:
-                is_significant = np.logical_or(is_significant[0], is_significant[1])
+                # is_significant = np.logical_or(is_significant[0], is_significant[1])
                 coefs_points = [[x, y] for x, y in zip(coefs[0], coefs[1])]
-                coefs_new = np.array(
-                    [math.sqrt((x * x) + (y * y)) for x, y in zip(coefs[0], coefs[1])]
-                )
+                coefs_new = np.array([math.sqrt((x * x) + (y * y))
+                                      for x, y in zip(coefs[0], coefs[1])])
+
+                is_significant_tmp = np.zeros(is_significant[0].shape)
+                for i in range(is_significant[0].shape[0]):
+                    if is_significant[0][i] == is_significant[1][i]:
+                        is_significant_tmp[i] = is_significant[0][i]
+                    else:
+                        # Project and rotate
+                        angle = math.degrees(
+                            math.atan(coefs[1][i] / coefs[0][i]))
+                        proj_tmp = self._project_line(
+                            self.low_dim_data,
+                            angle,
+                            point_a=[0, 0],
+                            point_b=coefs_points[i],
+                        )
+
+                        # Predict
+                        coefs_tmp, _, is_s_tmp, _, _ = self._get_importance(
+                            self.high_dim_data.to_numpy(),
+                            np.array([proj_tmp]).T,
+                            univar=univar_importance,
+                            significance=feature_significance,
+                        )
+
+                        is_significant_tmp[i] = is_s_tmp[0][i]
+                is_significant = np.array(is_significant_tmp)
 
                 if plot_top_k != 0:
                     min_ix = list(
-                        np.argsort(np.abs(coefs_new))[0 : len(coefs_new) - plot_top_k]
-                    )
+                        np.argsort(
+                            np.abs(coefs_new))[
+                            0: len(coefs_new) -
+                            plot_top_k])
                     is_significant[min_ix] = False
 
                 coefs = coefs_new * is_significant
                 all_points.append(coefs_points)
 
             else:
                 if plot_top_k != 0:
                     min_ix = list(
-                        np.argsort(np.max(np.abs(coefs * is_significant), axis=0))[
-                            0 : coefs.shape[1] - plot_top_k
-                        ]
-                    )
+                        np.argsort(
+                            np.max(
+                                np.abs(
+                                    coefs *
+                                    is_significant),
+                                axis=0))[
+                            0: coefs.shape[1] -
+                            plot_top_k])
                     is_significant[:, min_ix] = False
 
             all_coeffs.append(coefs)
             all_is_significant.append(is_significant)
             all_std_x.append(std_x)
             all_std_y.append(std_y)
 
@@ -962,16 +1073,24 @@
                     self.observations,
                     scale_circle=scale,
                     annotate=a,
                     biggest_arrow=biggest_arrow,
                     move_circle=move_circle[i],
                     arrow_width=arrow_width,
                     points=all_points[i] if len(all_points) > 0 else [],
-                    clock_label=clocks_labels[i] if len(clocks_labels) == len(dist_clusters) else "",
-                    clocks_label_angle=clocks_labels_angles[i] if len(clocks_labels_angles) == len(dist_clusters) else 270
+                    clock_label=(
+                        clocks_labels[i]
+                        if len(clocks_labels) == len(dist_clusters)
+                        else ""
+                    ),
+                    clocks_label_angle=(
+                        clocks_labels_angles[i]
+                        if len(clocks_labels_angles) == len(dist_clusters)
+                        else 270
+                    ),
                 )
 
                 for arrow, lbl in zip(arrows, arrow_labels):
                     if arrows_dict.get(lbl) is None:
                         arrows_dict[lbl] = arrow
 
             else:
@@ -998,15 +1117,17 @@
             adj_matrix.append(adj_row)
         return adj_matrix
 
     def _build_MST(self, n_clusters, adj_matrix):
         grapf_cl = Graph(n_clusters)
         grapf_cl.graph = adj_matrix
         mst = grapf_cl.primMST()
-        print(f"MST constructed for the inter-cluster clock ([[node1, node2, distance], ...]): \n {mst}")
+        print(
+            f"MST constructed for the Inter-group clock ([[node1, node2, distance], ...]): \n {mst}"
+        )
         return mst
 
     def _get_angle_to_x(self, points_a, points_b):
         m1 = (points_a[1] - points_b[1]) / (points_a[0] - points_b[0])
         y = min(points_a[1], points_b[1])
         m2 = (y - y) / (points_a[0] - points_b[0])
         return math.atan((m1 - m2) / (1 + (m1 * m2)))
@@ -1023,23 +1144,27 @@
         scale_circle,
         move_circle,
         annotate,
         arrow_width,
         plot_scatter,
         plot_hulls,
         clocks_labels,
-        clocks_labels_angles
+        clocks_labels_angles,
     ):
         alpha = 0.1
 
         # Scatter plot
         if plot_scatter:
             ax.scatter(
-                data["emb1"], data["emb2"], color="gray", s=2, alpha=alpha, zorder=0
-            )
+                data["emb1"],
+                data["emb2"],
+                color="gray",
+                s=2,
+                alpha=alpha,
+                zorder=0)
 
         if plot_hulls:
             self._draw_clusters(ax, data, alpha)
 
         # Add lines and clock
         clock_centers = []
         coefs_scaled = copy.deepcopy(coefs)
@@ -1047,32 +1172,48 @@
             p_a, p_b = cl_means[val[0]], cl_means[val[1]]
 
             # Add clock
             x_center, y_center = (
                 np.mean((p_a[0], p_b[0])) + move_circle[i][0],
                 np.mean((p_a[1], p_b[1])) + move_circle[i][1],
             )
-            
+
             clock_centers.append([x_center, y_center])
 
             radius = (math.dist(p_a, p_b) / 2) * scale_circle[i]
             c_min, c_max = self._get_cmin_cmax(coefs=coefs[i])
             num_circles = math.floor(radius / annotate[i]) + 1
             self._add_circles_lines(
                 ax, num_circles, annotate[i], 90, x_center, y_center
             )
 
             # num_circles - one circle per annotation
             self._add_circles(
-                ax, num_circles, annotate[i], x_center, y_center, radius, c_min, c_max, 
-                clock_label=f"{clocks_labels[val[0]]} "+ u"\u21FE" f" {clocks_labels[val[1]]}" if len(clocks_labels) > 1 else f"{val[0]}"+ u"\u21FE" f"{val[1]}",
-                clock_label_angle=clocks_labels_angles[i] if len(clocks_labels_angles) == len(mst) else 270
+                ax,
+                num_circles,
+                annotate[i],
+                x_center,
+                y_center,
+                radius,
+                c_min,
+                c_max,
+                clock_label=(
+                    f"{clocks_labels[val[0]]} " + "\u21FE" f" {clocks_labels[val[1]]}"
+                    if len(clocks_labels) > 1
+                    else f"{val[0]}" + "\u21FE" f"{val[1]}"
+                ),
+                clock_label_angle=(
+                    clocks_labels_angles[i]
+                    if len(clocks_labels_angles) == len(mst)
+                    else 270
+                ),
             )
 
-            coefs_scaled[i] = coefs_scaled[i] * (radius / max(abs(c_max), abs(c_min)))
+            coefs_scaled[i] = coefs_scaled[i] * \
+                (radius / max(abs(c_max), abs(c_min)))
 
             if val[0] > val[1] and p_a[0] < p_b[0]:
                 coefs_scaled[i] = coefs_scaled[i] * (-1)
             elif val[0] < val[1] and p_a[0] > p_b[0]:
                 coefs_scaled[i] = coefs_scaled[i] * (-1)
 
         # Add arrows
@@ -1117,19 +1258,20 @@
         move_circle,
         annotate,
         arrow_width,
         plot_scatter,
         plot_hulls,
         plot_top_k,
         clocks_labels,
-        clocks_labels_angles
+        clocks_labels_angles,
     ):
         dist_clusters = self.low_dim_data["cluster"].unique()
         dist_clusters.sort()
-        dist_clusters = dist_clusters[1:] if dist_clusters[0] == -1 else dist_clusters
+        dist_clusters = dist_clusters[1:] if dist_clusters[0] == - \
+            1 else dist_clusters
 
         cl_means = self._get_cluster_centers(dist_clusters)
         adj_matrix = self._build_adj_matrix(cl_means)
         mst = self._build_MST(len(dist_clusters), adj_matrix)
 
         mst_proj, angles = [], []
         for val in mst:
@@ -1144,24 +1286,24 @@
             mst,
             univar=univar_importance,
             significance=feature_significance,
         )
 
         if plot_top_k != 0:
             # print(coefs)
-            min_ix = np.argsort(np.abs(coefs) * is_significant, axis=1)[:, 0 : len(coefs) - plot_top_k-1]
+            min_ix = np.argsort(np.abs(coefs) * is_significant, axis=1)[
+                :, 0: len(coefs) - plot_top_k - 1
+            ]
             # print(min_ix)
             for i in range(is_significant.shape[0]):
                 for j in range(is_significant.shape[1]):
                     if j in min_ix[i]:
                         is_significant[i, j] = False
         if is_significant.sum() == 0:
-            warnings.warn(
-                    "no significant features."
-                )
+            warnings.warn("no significant features.")
             return [], []
 
         if standartize_coef:
             coefs = coefs / std_x
             if np.isnan(coefs).any():
                 coefs = np.nan_to_num(coefs)
                 warnings.warn(
@@ -1182,30 +1324,30 @@
             scale_circle,
             move_circle,
             annotate,
             arrow_width,
             plot_scatter,
             plot_hulls,
             clocks_labels,
-            clocks_labels_angles
+            clocks_labels_angles,
         )
 
         return arrows, labels
 
     def get_num_clusters(self):
         return self.low_dim_data["cluster"].nunique()
 
     def plot_global_clock(
         self,
         ax: matplotlib.axis.Axis,
         standartize_data: bool = True,
         standartize_coef: bool = True,
         biggest_arrow_method: bool = True,
         angle_shift: int = 5,
-        univar_importance: bool = True,
+        univar_importance: bool = False,
         feature_significance: float = 0.05,
         scale_circle: float = 1,
         move_circle: list = [0, 0],
         annotate: float = 0.6,
         arrow_width: float = 0.1,
         plot_scatter: bool = True,
         plot_top_k: int = 0,
@@ -1247,15 +1389,15 @@
     def plot_local_clocks(
         self,
         ax: matplotlib.axis.Axis,
         standartize_data: bool = True,
         standartize_coef: bool = True,
         biggest_arrow_method: bool = True,
         angle_shift: int = 5,
-        univar_importance: bool = True,
+        univar_importance: bool = False,
         feature_significance: float = 0.05,
         scale_circles: list = [],
         move_circles: list = [],
         annotates: list = [],
         arrow_width: float = 0.1,
         plot_scatter: bool = True,
         plot_hulls: bool = True,
@@ -1270,15 +1412,16 @@
 
             if biggest_arrow_method:
                 self._create_biggest_projections()
             else:
                 self._create_angles_projections(angle_shift=angle_shift)
 
         n_clusters = self.low_dim_data["cluster"].nunique()
-        if n_clusters != len(scale_circles) != len(move_circles) != len(annotates):
+        if n_clusters != len(scale_circles) != len(
+                move_circles) != len(annotates):
             raise Exception(
                 f"Length of annotates, move_circles, scale_circles should be equal number of clusters {n_clusters}."
             )
 
         if len(scale_circles) == len(move_circles) == len(annotates) == 0:
             for _ in range(n_clusters):
                 scale_circles.append(1)
@@ -1305,15 +1448,15 @@
             move_circle=move_circles,
             annotate=annotates,
             arrow_width=arrow_width,
             plot_scatter=plot_scatter,
             plot_hulls=plot_hulls,
             plot_top_k=plot_top_k,
             clocks_labels=clocks_labels,
-            clocks_labels_angles=clocks_labels_angles
+            clocks_labels_angles=clocks_labels_angles,
         )
         return arrows_all, arrow_labels_all
 
     def plot_between_clock(
         self,
         ax: matplotlib.axis.Axis,
         standartize_data: bool = True,
@@ -1345,15 +1488,16 @@
 
         if plot_top_k > self.high_dim_data.shape[1]:
             raise Exception(
                 f"Invalid value for plot_top_k: {plot_top_k} (0 - plot all, ncol > k > 0). plot_top_k greater than umber of columns."
             )
 
         n_clusters = self.low_dim_data["cluster"].nunique() - 1
-        if n_clusters != len(scale_circles) != len(move_circles) != len(annotates):
+        if n_clusters != len(scale_circles) != len(
+                move_circles) != len(annotates):
             raise Exception(
                 f"Length of annotates, move_circles, scale_circles should be equal number of edges {n_clusters}."
             )
 
         if len(scale_circles) == len(move_circles) == len(annotates) == 0:
             for _ in range(n_clusters):
                 scale_circles.append(1)
@@ -1369,11 +1513,11 @@
             move_circle=move_circles,
             annotate=annotates,
             arrow_width=arrow_width,
             plot_scatter=plot_scatter,
             plot_hulls=plot_hulls,
             plot_top_k=plot_top_k,
             clocks_labels=clocks_labels,
-            clocks_labels_angles = clocks_labels_angles
+            clocks_labels_angles=clocks_labels_angles,
         )
 
         return arrows, labels
```

### Comparing `feature_clock-0.0.3/src/feature_clock.egg-info/requires.txt` & `feature_clock-1.0.0/src/feature_clock.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `feature_clock-0.0.3/test/test_cancer.py` & `feature_clock-1.0.0/test/test_iris.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,376 +1,558 @@
-from matplotlib import pyplot as plt
+import math
+from matplotlib import cm, gridspec, pyplot as plt
+import matplotlib
 import numpy as np
 import pandas as pd
 from sklearn.discriminant_analysis import StandardScaler
 from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
+from sklearn import decomposition  # decomposition.PCA
+from sklearn import manifold
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
-from sklearn import preprocessing
 
-def make_legend_arrow(legend, orig_handle,
-                      xdescent, ydescent,
-                      width, height, fontsize):
-    p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
-    return p
 
+def make_legend_arrow(legend, orig_handle, xdescent, ydescent, width, height, fontsize):
+    p = mpatches.FancyArrow(
+        0, 0.5 * height, width, 0, length_includes_head=True, head_width=0.75 * height
+    )
+    return p
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
-def setup_cancer_data(method="tsne", drop_labels=True):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/Cancer_Data.csv"
+def setup_iris_data(method="tsne", drop_labels=True):
+    file_name = "feature_clock_visualization/data/Iris.csv"
     X = read_data(file_name)
+    X.rename(
+        columns={
+            "SepalLengthCm": "SepalLength",
+            "SepalWidthCm": "SepalWidth",
+            "PetalLengthCm": "PetalLength",
+            "PetalWidthCm": "PetalWidth",
+        },
+        inplace=True,
+    )
+
+    X.drop(columns={"Id"}, inplace=True)
 
-    X.drop(columns=["id"], inplace=True)
     X = X.dropna()
-    X.diagnosis = X.diagnosis.map({'M': 0, 'B': 1})
-    
-    labels = X["diagnosis"]
+    # X = pd.concat([X[X["Species"] == "Iris-setosa"][0:49], X[X["Species"] == "Iris-versicolor"], X[X["Species"] == "Iris-virginica"]], ignore_index=True)
+    # pd. factorize(X["Species"])[0]
+    X["Species"] = X.Species.map(
+        {"Iris-setosa": 0, "Iris-versicolor": 1, "Iris-virginica": 2}
+    ).to_numpy()
+
+    for col in X.columns:
+        if col != "Species":
+            X[col] = (X[col] - X[col].mean()) / X[col].std()
+
+            Q1 = X[col].quantile(0.25)
+            Q3 = X[col].quantile(0.77)
+            IQR = Q3 - Q1
+            X = X[~((X[col] < (Q1 - 1.5 * IQR)) | (X[col] > (Q3 + 1.5 * IQR)))]
+
+    print(X.Species.value_counts())
+
+    labels = X["Species"]
     if drop_labels:
-        X.drop(columns=["diagnosis"], inplace=True)
+        X.drop(columns=["Species"], inplace=True)
     obs = list(X.columns)
-    
-    for col in X.columns:
-        X[col] = (X[col] - X[col].mean()) / X[col].std()
-    
+
     # compute umap
     if method == "umap":
-        reducer = umap.UMAP(min_dist=0.2, n_neighbors=30, random_state=42)
+        reducer = umap.UMAP(random_state=42)
         if not drop_labels:
-            K = X.drop(columns=["diagnosis"], inplace=False)
+            K = X.drop(columns=["Species"], inplace=False)
             standard_embedding = reducer.fit_transform(K)
         else:
             standard_embedding = reducer.fit_transform(X)
 
     elif method == "tsne":
-        raise NotImplementedError()
+        tsne = manifold.TSNE(
+            n_components=2,
+            learning_rate="auto",
+            random_state=42,
+            n_iter=1000,
+            perplexity=17,
+        )
+        standard_embedding = tsne.fit_transform(X)
 
     elif method == "phate":
         raise NotImplementedError()
-    
+
+    elif method == "pca":
+        pca = decomposition.PCA(n_components=2)
+        standard_embedding = pca.fit_transform(X)
+
+        return X, obs, standard_embedding, labels, pca.components_
+
     # get clusters
-    # clusters = HDBSCAN(min_samples=12).fit_predict(X)
-    clusters = KMeans(n_clusters=2, n_init="auto", max_iter=1000, random_state=42).fit_predict(X)
+    clusters = HDBSCAN(min_samples=12).fit_predict(X)
+    # clusters = KMeans(n_clusters=3, n_init="auto", max_iter=1000).fit_predict(X)
+
+    for i in range(standard_embedding.shape[1]):
+        standard_embedding[:, i] = (
+            standard_embedding[:, i] - standard_embedding[:, i].mean()
+        ) / standard_embedding[:, i].std()
 
     return X, obs, standard_embedding, labels, clusters
 
 
-def test_between_all_3():
-    colors = [
-        'tab:pink', 'darkorchid', 'tab:green', 'cornflowerblue', 'mediumslateblue', 'crimson', 
-        'tab:blue', 'tab:olive', 'coral', 'black', 'blueviolet', 'brown', 
-        'darkgoldenrod', 'tab:orange', 'darkgreen', 'darkgrey', 'darkkhaki', 'darkmagenta', 
-        'cadetblue', 'chartreuse', 'tab:purple', 'tab:cyan', 'tab:red', 'tab:brown', 'darkblue', 
-        'darkolivegreen', 'darkorange', 'lawngreen', 'darkred', "orangered"]
+def print_iris_all():
+    X_new, obs, standard_embedding, labels, clusters = setup_iris_data(
+        method="tsne", drop_labels=True
+    )
+    dpi = 1000
+    # fig_size = (2.375, 2.375)
+    fig_size = (3.2325, 2.9)
+    fig, axi = plt.subplots(
+        2,
+        2,
+        num=None,
+        figsize=fig_size,
+        dpi=dpi,
+        facecolor="w",
+        edgecolor="k",
+    )
+    for i, o in enumerate(obs):
+        if o == "Species":
+            break
+
+        im = axi[i % 2, i // 2].scatter(
+            standard_embedding[:, 0],
+            standard_embedding[:, 1],
+            marker=".",
+            s=5,
+            c=X_new[o],
+            cmap="jet",
+        )
+        axi[i % 2, i // 2].set_yticks([])
+        axi[i % 2, i // 2].set_xticks([])
+        axi[i % 2, i // 2].yaxis.set_label_coords(x=-0.01, y=0.5)
+        axi[i % 2, i // 2].xaxis.set_label_coords(x=0.5, y=-0.02)
+        axi[i % 2, i // 2].set_title(o, size=8, pad=-14)
 
-    X_new, obs, standard_embedding, labels, clusters = setup_cancer_data(method="umap")
+    axi[1, 0].set_ylabel("t-SNE2", size=8)
+    axi[1, 0].set_xlabel("t-SNE1", size=8)
 
-    fig, axi = plt.subplots(1, 3, figsize=(7.125-0.66, 2.375))
+    plt.subplots_adjust(
+        left=0.05,
+        right=0.98,
+        top=0.95,
+        bottom=0.05,  # wspace=0.21, hspace=0.33
+    )
+    cbar = fig.colorbar(im, ax=axi.ravel().tolist(), pad=0.1)
+    cbar.ax.tick_params(labelsize=7)
+    # for ax in axi:
+    #     for a in ax:
+    #         a.axis('off')
+    # axi[1][2].set_visible(False)
+    plt.savefig("plots/paper/iris/plot_irisAll.pdf")
+
+
+def test_between_all():
+    X_new, obs, standard_embedding, labels, clusters = setup_iris_data(method="tsne")
+
+    fig, ax = plt.subplots(1, figsize=(3.2325, 3.2325))
     plt.tight_layout()
 
-    sc = axi[0].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
-    
-    legend1 = axi[0].legend(
-        handles = sc.legend_elements()[0],
+    sc = ax.scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="tab10",
+        alpha=0.5,
+        zorder=0,
+        s=3,
+    )
+
+    legend1 = ax.legend(
+        handles=sc.legend_elements()[0],
         loc="upper center",
         # bbox_to_anchor=(0.0, 0.0),
         fontsize=7,
         ncol=3,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.1,
-        labels=["Malignant", "Benign"])
-    
-    axi[0].add_artist(legend1)
+        labels=["Setosa", "Versicolor", "Virginica"],
+    )
+    ax.add_artist(legend1)
+
+    plot_inst = NonLinearClock(
+        X_new, obs, standard_embedding, labels, method="tsne", cluster_labels=clusters
+    )
+    arrows, arrow_labels = plot_inst.plot_global_clock(
+        standartize_data=False,
+        standartize_coef=True,
+        biggest_arrow_method=True,
+        univar_importance=False,
+        ax=ax,
+        scale_circle=5,
+        move_circle=[-8.0, 0],
+        annotate=2.5,
+        arrow_width=0.3,
+    )
+
+    ax.legend(
+        arrows,
+        arrow_labels,
+        loc="lower center",
+        bbox_to_anchor=(0.5, 1.0),
+        fontsize=7,
+        ncol=3,
+        markerscale=0.6,
+        handlelength=1.3,
+        columnspacing=0.8,
+        handletextpad=0.1,
+    )
+
+    ax.set_yticks([])
+    ax.set_xticks([])
+    ax.set_ylabel("t-SNE2", size=8)
+    ax.set_xlabel("t-SNE1", size=8)
+    # ax.set_title("Iris dataset", size=8)
+    ax.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax.xaxis.set_label_coords(x=0.5, y=-0.02)
+    plt.subplots_adjust(
+        left=0.05,
+        right=0.95,
+        top=0.92,
+        bottom=0.05,  # wspace=0.21, hspace=0.33
+    )
+    plt.savefig("plots/paper/iris/iris_global.pdf")
+
 
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters, color_scheme=colors)
+def test_between_all_3():
+    X_new, obs, standard_embedding, labels, clusters = setup_iris_data(method="umap")
+
+    fig, axi = plt.subplots(1, 3, figsize=(7.125 - 0.66, 2.375))
+    plt.tight_layout()
+    plot_inst = NonLinearClock(
+        X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=axi[0],
         scale_circle=1.2,
         move_circle=[0, 0],
         annotate=1.0,
-        arrow_width=0.1,
-        plot_scatter=False,
-        plot_top_k=5
+        arrow_width=0.08,
     )
 
     axi[0].set_yticks([])
     axi[0].set_xticks([])
     axi[0].set_ylabel("UMAP2", size=8)
     axi[0].set_xlabel("UMAP1", size=8)
-    axi[0].set_title("Global clock", size=8)
+    axi[0].set_title("Diabetis", size=8)
     axi[0].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[0].xaxis.set_label_coords(x=0.5, y=-0.02)
     plt.subplots_adjust(
         left=0.05,
         right=0.95,
         top=0.79,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
+    plt.savefig("plots/paper/iris/iris_global.pdf")
 
     # Local
-    arrows1, arrow_labels1 = plot_inst.plot_local_clocks(
+    # fig, ax = plt.subplots(1, figsize=(3.33, 3.33))
+    arrows, arrow_labels = plot_inst.plot_local_clocks(
         standartize_data=True,
         standartize_coef=True,
-        biggest_arrow_method=False,
+        biggest_arrow_method=True,
         univar_importance=False,
         ax=axi[1],
-        scale_circles=[0.5, 0.5],
-        move_circles=[[-0.4, 0], [0.5, 0]],
-        annotates=[50.0, 50.0],
+        scale_circles=[3, 1, 0.5],
+        move_circles=[[0, 0], [0, 0], [0, 0]],
+        annotates=[1.0, 1.0, 0.8],
         arrow_width=0.08,
-        plot_top_k=5,
-        plot_hulls=True,
-        plot_scatter=False
     )
 
-    sc2 = axi[1].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
-    
-    legend2 = axi[1].legend(
-        handles = sc2.legend_elements()[0],
-        loc="upper center",
-        # bbox_to_anchor=(0.0, 0.0),
-        fontsize=7,
-        ncol=3,
-        markerscale=0.6,
-        handlelength=1.5,
-        columnspacing=0.8,
-        handletextpad=0.1,
-        labels=["Malignant", "Benign"])
-    
-    axi[1].add_artist(legend2)
-
     axi[1].set_yticks([])
     axi[1].set_xticks([])
     axi[1].set_ylabel("UMAP2", size=8)
     axi[1].set_xlabel("UMAP1", size=8)
-    axi[1].set_title("Local clock", size=8)
+    axi[1].set_title("Diabetis", size=8)
     axi[1].yaxis.set_label_coords(x=-0.01, y=0.5)
-    axi[1].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     # Between
-    sc3 = axi[2].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
-    
-    legend3 = axi[2].legend(
-        handles = sc3.legend_elements()[0],
-        loc="upper center",
-        # bbox_to_anchor=(0.0, 0.0),
-        fontsize=7,
-        ncol=3,
-        markerscale=0.6,
-        handlelength=1.5,
-        columnspacing=0.8,
-        handletextpad=0.1,
-        labels=["Malignant", "Benign"])
-    
-    axi[2].add_artist(legend3)
-    
-    arrows2, arrow_labels2 = plot_inst.plot_between_clock(
-        standartize_data=False,
+    _, _ = plot_inst.plot_between_clock(
+        standartize_data=True,
         standartize_coef=True,
-        univar_importance=False,
+        univar_importance=True,
         ax=axi[2],
         scale_circles=[1.25],
         move_circles=[[0, 0]],
         annotates=[1.1],
         arrow_width=0.08,
-        plot_top_k=5,
-        plot_scatter=False
     )
-
-    arrows_dict = {}
-    for i, val in enumerate(arrow_labels):
-        arrows_dict[val] = arrows[i]
-    for i, val in enumerate(arrow_labels1):
-        arrows_dict[val] = arrows1[i]
-    for i, val in enumerate(arrow_labels2):
-        arrows_dict[val] = arrows2[i]
-
     axi[2].legend(
-        list(arrows_dict.values()),
-        list(arrows_dict.keys()),
+        arrows,
+        arrow_labels,
         loc="lower center",
         bbox_to_anchor=(-0.84, 1.12),
         fontsize=7,
-        ncol=5,
+        ncol=8,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
     )
 
     axi[2].set_yticks([])
     axi[2].set_xticks([])
     axi[2].set_ylabel("UMAP2", size=8)
     axi[2].set_xlabel("UMAP1", size=8)
-    axi[2].set_title("Inter-cluster clock", size=8)
+    axi[2].set_title("Diabetis", size=8)
     axi[2].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[2].xaxis.set_label_coords(x=0.5, y=-0.02)
-
     plt.subplots_adjust(
-        left=0.03,
-        right=0.99,
-        top=0.75,
+        left=0.05,
+        right=0.95,
+        top=0.79,
         bottom=0.07,  # wspace=0.21, hspace=0.33
     )
-    plt.savefig("plots/paper/cancer/cancer_3.pdf")
+    plt.savefig("plots/paper/iris/iris_3.pdf")
 
 
-def test_between_all_3():
-    colors = [
-        'tab:pink', 'darkorchid', 'tab:green', 'cornflowerblue', 'mediumslateblue', 'crimson', 
-        'tab:blue', 'tab:olive', 'coral', 'black', 'blueviolet', 'brown', 
-        'darkgoldenrod', 'tab:orange', 'darkgreen', 'darkgrey', 'darkkhaki', 'darkmagenta', 
-        'cadetblue', 'chartreuse', 'tab:purple', 'tab:cyan', 'tab:red', 'tab:brown', 'darkblue', 
-        'darkolivegreen', 'darkorange', 'lawngreen', 'darkred', "orangered"]
+def test_pca_all_3():
+    dpi = 1000
+    fig_size = ((7.125 - 0.17) / 2, ((7.125 - 0.17) / 2.8) / 1.618)
 
-    X_new, obs, standard_embedding, labels, clusters = setup_cancer_data(method="umap")
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=dpi,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=3, nrows=1, figure=fig, left=0.04, right=0.99, top=0.72, bottom=0.08
+    )
+    ax1 = fig.add_subplot(spec2[0])
+    ax3 = fig.add_subplot(spec2[2])
 
-    fig, axi = plt.subplots(1, 3, figsize=((7.125-0.17), ((7.125-0.17)/1.8)/1.618))
-    plt.tight_layout()
+    spec23 = gridspec.GridSpecFromSubplotSpec(2, 2, subplot_spec=spec2[1], wspace=0.05)
+    ax21 = fig.add_subplot(spec23[0, 0])
+    ax22 = fig.add_subplot(spec23[0, 1])
+    ax23 = fig.add_subplot(spec23[1, 0])
+    ax24 = fig.add_subplot(spec23[1, 1])
 
-    sc = axi[0].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
+    df = pd.read_csv("feature_clock_visualization/data/Iris.csv")
+    # df = df.groupby('Species', group_keys=False).apply(lambda x: x.sample(2000, random_state=42, replace=True))
+    labels = df.Species.map(
+        {"Iris-setosa": 0, "Iris-versicolor": 1, "Iris-virginica": 2}
+    ).to_numpy()
 
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=labels, color_scheme=colors)
-    arrows, arrow_labels = plot_inst.plot_global_clock(
-        standartize_data=False,
-        standartize_coef=True,
-        biggest_arrow_method=True,
-        univar_importance=True,
-        ax=axi[0],
-        scale_circle=1.2,
-        move_circle=[0, 0],
-        annotate=1.0,
-        arrow_width=0.1,
-        plot_scatter=False,
-        plot_top_k=5
+    df.rename(
+        columns={
+            "SepalLengthCm": "SepalLength",
+            "SepalWidthCm": "SepalWidth",
+            "PetalLengthCm": "PetalLength",
+            "PetalWidthCm": "PetalWidth",
+        },
+        inplace=True,
     )
 
-    axi[0].set_yticks([])
-    axi[0].set_xticks([])
-    axi[0].set_ylabel("UMAP2", size=8)
-    axi[0].set_xlabel("UMAP1", size=8)
-    axi[0].set_title("Global clock", size=8)
-    axi[0].yaxis.set_label_coords(x=-0.01, y=0.5)
-    axi[0].xaxis.set_label_coords(x=0.5, y=-0.02)
-    plt.subplots_adjust(
-        left=0.05,
-        right=0.95,
-        top=0.79,
-        bottom=0.05,  # wspace=0.21, hspace=0.33
+    df.drop(columns={"Id"}, inplace=True)
+    df = df.dropna()
+
+    X = df.drop("Species", axis=1).to_numpy()
+
+    scaler = StandardScaler()
+    X = scaler.fit_transform(X)
+
+    pca = decomposition.PCA(n_components=2)
+    pcaT = pca.fit_transform(X)
+
+    C = pca.components_
+
+    colormap = plt.cm.Dark2  # or any other colormap
+    normalize = matplotlib.colors.Normalize(vmin=-1, vmax=3)
+
+    sc = ax1.scatter(
+        pcaT[:, 0],
+        pcaT[:, 1],
+        marker=".",
+        c=labels,
+        cmap=colormap,
+        norm=normalize,
+        alpha=0.2,
+        zorder=0,
     )
 
-    # Local
-    arrows1, arrow_labels1 = plot_inst.plot_local_clocks(
+    colors = ["tab:cyan", "tab:red", "tab:blue", "tab:pink"]
+    labels = ["SepalLen", "SepalWid", "PetalLen", "PetalWid"]
+
+    arrows_dict = {}
+    for i in range(0, 4):
+        arrows_dict[labels[i][0:8]] = ax1.arrow(
+            -1,
+            0.5,
+            (C[0][i]) * 2,
+            (C[1][i]) * 2,
+            color=colors[i],
+            width=0.06,
+            label=labels[i],
+        )
+
+    ax1.set_yticks([])
+    ax1.set_xticks([])
+    ax1.set_ylabel("PC2", size=8)
+    ax1.set_xlabel("PC1", size=8)
+    ax1.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax1.xaxis.set_label_coords(x=0.5, y=-0.02)
+
+    # second plot
+    X_new, obs, standard_embedding, labels, clusters = setup_iris_data(
+        method="tsne", drop_labels=True
+    )
+    standard_embedding[:, 0], standard_embedding[:, 1] = (
+        1 * standard_embedding[:, 0],
+        1 * standard_embedding[:, 1],
+    )
+    for (i, o), axi in zip(enumerate(obs), [ax21, ax22, ax23, ax24]):
+        if o == "Species":
+            break
+
+        im = axi.scatter(
+            standard_embedding[:, 0],
+            standard_embedding[:, 1],
+            marker=".",
+            s=1,
+            c=X_new[o],
+            cmap=cm.coolwarm,
+            alpha=0.8,
+        )
+        axi.set_yticks([])
+        axi.set_xticks([])
+        axi.yaxis.set_label_coords(x=-0.01, y=0.5)
+        axi.xaxis.set_label_coords(x=0.5, y=-0.02)
+        axi.set_title(o[0:3] + o[5:8], size=5, pad=-14)
+
+    ax21.set_ylabel("t-SNE2", size=8)
+    ax23.set_xlabel("t-SNE1", size=8)
+
+    ax21.yaxis.set_label_coords(0, -0.15)
+    ax23.xaxis.set_label_coords(1.1, -0.04)
+
+    cbar = fig.colorbar(
+        im, ax=[ax21, ax22, ax23, ax24], pad=0.02, ticks=[-1, 0, 1], aspect=40
+    )
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
+    cbar.outline.set_visible(False)
+
+    # third plot
+    ax3.set_yticks([])
+    ax3.set_xticks([])
+    ax3.set_ylabel("t-SNE2", size=8)
+    ax3.set_xlabel("t-SNE1", size=8)
+    ax3.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax3.xaxis.set_label_coords(x=0.5, y=-0.02)
+
+    X_new, obs, standard_embedding, labels, clusters = setup_iris_data(
+        method="tsne", drop_labels=True
+    )
+    standard_embedding[:, 0], standard_embedding[:, 1] = (
+        1 * standard_embedding[:, 0],
+        1 * standard_embedding[:, 1],
+    )
+
+    sc = ax3.scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap=colormap,
+        norm=normalize,
+        alpha=0.2,
+        zorder=0,
+        edgecolors="face",
+    )
+
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="umap",
+        cluster_labels=labels,
+        color_scheme=colors,
+    )
+    _, _ = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
-        ax=axi[1],
-        scale_circles=[1, 1],
-        move_circles=[[-0.4, 0], [0.5, 0]],
-        annotates=[40, 40],
-        arrow_width=0.08,
-        plot_top_k=5,
-        plot_hulls=True,
-        plot_scatter=False
+        ax=ax3,
+        scale_circle=1.5,
+        move_circle=[-0.3, 0.0],
+        annotate=0.5,
+        arrow_width=0.05,
+        # annotate=4.5,
+        # arrow_width=0.5,
+        plot_scatter=False,
     )
 
-    sc2 = axi[1].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
-
-    axi[1].set_yticks([])
-    axi[1].set_xticks([])
-    axi[1].set_ylabel("UMAP2", size=8)
-    axi[1].set_xlabel("UMAP1", size=8)
-    axi[1].set_title("Local clock", size=8)
-    axi[1].yaxis.set_label_coords(x=-0.01, y=0.5)
-    axi[1].xaxis.set_label_coords(x=0.5, y=-0.02)
-
-    # Between
-    sc3 = axi[2].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
-    
-    arrows2, arrow_labels2 = plot_inst.plot_between_clock(
-        standartize_data=True,
-        standartize_coef=True,
-        univar_importance=False,
-        ax=axi[2],
-        scale_circles=[1.25],
-        move_circles=[[0, 0]],
-        annotates=[1.1],
-        arrow_width=0.08,
-        plot_top_k=5,
-        plot_scatter=False
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 2
+        + [list(arrows_dict.values())[0]]
+        + [sc.legend_elements()[0][0]]
+        + [list(arrows_dict.values())[1]]
+        + [sc.legend_elements()[0][1]]
+        + [list(arrows_dict.values())[2]]
+        + [sc.legend_elements()[0][2]]
+        + [list(arrows_dict.values())[3]]
+    )
+
+    labels = (
+        ["Factors:", "Labels:"]
+        + [list(arrows_dict.keys())[0]]
+        + ["Setosa"]
+        + [list(arrows_dict.keys())[1]]
+        + ["Versicolor"]
+        + [list(arrows_dict.keys())[2]]
+        + ["Virginica"]
+        + [list(arrows_dict.keys())[3]]
     )
 
-    arrows_dict = {}
-    for i, val in enumerate(arrow_labels):
-        arrows_dict[val] = arrows[i]
-    for i, val in enumerate(arrow_labels1):
-        arrows_dict[val] = arrows1[i]
-    for i, val in enumerate(arrow_labels2):
-        arrows_dict[val] = arrows2[i]
-
-    
-    hatches = [plt.plot([],marker="", ls="")[0]]*3 + \
-        list(arrows_dict.values())[0:2] + [sc.legend_elements()[0][0]] + \
-        list(arrows_dict.values())[2:4] + [sc.legend_elements()[0][1]] + \
-        list(arrows_dict.values())[4:6] + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[6:8] + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[8:]  + [plt.plot([],marker="", ls="")[0]]
-    
-    labels = ["Factors:", " ","Labels:"] + \
-        list(arrows_dict.keys())[0:2] + ["Malignant"] + \
-        list(arrows_dict.keys())[2:4] + ["Benign"] + \
-        list(arrows_dict.keys())[4:6] + [" "] + \
-        list(arrows_dict.keys())[6:8] + [" "] + \
-        list(arrows_dict.keys())[8:]  + [" "]
-    
-    leg = axi[2].legend(
+    leg = ax22.legend(
         hatches,
         labels,
         loc="lower center",
-        bbox_to_anchor=(-0.84, 1.12),
+        bbox_to_anchor=(0.25, 1.1),
         fontsize=7,
-        ncol=6,
+        ncol=5,
         markerscale=0.6,
-        handlelength=1.5,
+        handlelength=1.0,
         columnspacing=0.8,
-        handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handletextpad=0.3,
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
+    for lh in leg.legendHandles:
+        lh.set_alpha(1)
 
-    axi[2].set_yticks([])
-    axi[2].set_xticks([])
-    axi[2].set_ylabel("UMAP2", size=8)
-    axi[2].set_xlabel("UMAP1", size=8)
-    axi[2].set_title("Inter-cluster clock", size=8)
-    axi[2].yaxis.set_label_coords(x=-0.01, y=0.5)
-    axi[2].xaxis.set_label_coords(x=0.5, y=-0.02)
+    plt.savefig("plots/paper/iris/plot_biplot.pdf")
 
-    plt.subplots_adjust(
-        left=0.02,
-        right=0.99,
-        top=0.7,
-        bottom=0.06,  # wspace=0.21, hspace=0.33
-    )
-    plt.savefig("plots/paper/cancer/cancer_3.pdf")
-
-# print_cancer_all()
-test_between_all_3()
-# teaser()
-# import matplotlib.colors as mcolors
-# print(list(mcolors.TABLEAU_COLORS.keys()))
-# print(list(mcolors.CSS4_COLORS.keys()))
+
+# print_iris_all()
+test_between_all()
+test_pca_all_3()
```

### Comparing `feature_clock-0.0.3/test/test_melody.py` & `feature_clock-1.0.0/test/test_melody.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,83 @@
-from matplotlib import cm, pyplot as plt
+from matplotlib import cm, gridspec, pyplot as plt
 import matplotlib
 import numpy as np
 import pandas as pd
 from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
-def make_legend_arrow(legend, orig_handle,
-                      xdescent, ydescent,
-                      width, height, fontsize):
-    p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
+
+def make_legend_arrow(legend, orig_handle, xdescent, ydescent, width, height, fontsize):
+    p = mpatches.FancyArrow(
+        0, 0.5 * height, width, 0, length_includes_head=True, head_width=0.75 * height
+    )
     return p
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_melody_data(method="tsne", drop_labels=True):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/melody.csv"
+    file_name = "feature_clock_visualization/data/melody.csv"
     X = read_data(file_name)
     # X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     # X.drop(columns=["Genre"], inplace=True)
     X["Genre"], _ = pd.factorize(X["Genre"])
     X = X.dropna()
 
-    X.rename(columns={
-        'LyricalContect':'Lyrical contect', 
-        'ReleasedYear':'Year of release', 
-        'NumInstruments':'Num of instruments',
-        'SongLength':'Song length'
-    }, inplace=True)
+    X.rename(
+        columns={
+            "LyricalContent": "Lyrical Content",
+            "ReleasedYear": "Year of Release",
+            "NumInstruments": "Num of Instruments",
+            "SongLength": "Song Length",
+        },
+        inplace=True,
+    )
 
+    for col in X.columns:
+        X[col] = (X[col] - X[col].mean()) / X[col].std()
 
     labels = X["Popularity"]
     if drop_labels:
         X.drop(columns=["Popularity"], inplace=True)
     obs = list(X.columns)
 
-    for col in X.columns:
-        X[col] = (X[col] - X[col].mean()) / X[col].std()
-    
     # compute umap
     if method == "umap":
         reducer = umap.UMAP(random_state=42)
         if not drop_labels:
             K = X.drop(columns=["Popularity"], inplace=False)
             standard_embedding = reducer.fit_transform(K)
         else:
             standard_embedding = reducer.fit_transform(X)
 
     elif method == "tsne":
         raise NotImplementedError()
 
     elif method == "phate":
         raise NotImplementedError()
-    
+
     # get clusters
-    clusters = HDBSCAN(min_samples=10, min_cluster_size=30).fit_predict(X)
-    # clusters = KMeans(n_clusters=2).fit_predict(X)
+    # clusters = HDBSCAN(min_samples=10, min_cluster_size=30).fit_predict(X)
+    clusters = labels > 0.5
+    print(clusters)
 
     return X, obs, standard_embedding, labels, clusters
 
+
 def print_melody_all():
-    X_new, obs, standard_embedding, labels, clusters = setup_melody_data(method="umap", drop_labels=False)
+    X_new, obs, standard_embedding, labels, clusters = setup_melody_data(
+        method="umap", drop_labels=False
+    )
     dpi = 1000
     # fig_size = (2.375, 2.375)
     fig_size = (3.2325, 2.9)
     fig, axi = plt.subplots(
         3,
         3,
         num=None,
@@ -100,37 +107,39 @@
     plt.subplots_adjust(
         left=0.05,
         right=1,
         top=0.95,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     cbar = fig.colorbar(im, ax=axi.ravel().tolist(), pad=0.1)
-    cbar.ax.tick_params(labelsize=7) 
+    cbar.ax.tick_params(labelsize=7)
     # for ax in axi:
     #     for a in ax:
-    #         a.axis('off') 
+    #         a.axis('off')
     plt.savefig("plots/paper/melody/plot_melodyAll_teaser.pdf")
 
 
 def test_between_all():
     X_new, obs, standard_embedding, labels, clusters = setup_melody_data(method="umap")
 
     fig, ax = plt.subplots(1, figsize=(3.33, 2.8))
     plt.tight_layout()
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters)
+    plot_inst = NonLinearClock(
+        X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax,
         scale_circle=1,
         move_circle=[0, 0],
         annotate=0.6,
-        arrow_width=1.5
+        arrow_width=1.5,
     )
     ax.legend(
         arrows,
         arrow_labels,
         loc="lower center",
         bbox_to_anchor=(0.5, 1.07),
         fontsize=7,
@@ -165,26 +174,14 @@
         univar_importance=False,
         ax=ax,
         scale_circles=[3, 0.5, 0.5],
         move_circles=[[0, 0], [0, 0], [0, 0]],
         annotates=[0.5, 0.5, 0.5],
         arrow_width=0.05,
     )
-    # ax.legend(
-    #     arrows,
-    #     arrow_labels,
-    #     loc="lower center",
-    #     bbox_to_anchor=(0.5, 1.07),
-    #     fontsize=7,
-    #     ncol=4,
-    #     markerscale=0.6,
-    #     handlelength=1.5,
-    #     columnspacing=0.8,
-    #     handletextpad=0.5,
-    # )
 
     ax.set_yticks([])
     ax.set_xticks([])
     ax.set_ylabel("UMAP2", size=8)
     ax.set_xlabel("UMAP1", size=8)
     ax.set_title("Melody popularity", size=8)
     ax.yaxis.set_label_coords(x=-0.01, y=0.5)
@@ -238,84 +235,164 @@
     plt.savefig("plots/paper/melody/melody_between.pdf")
 
 
 def test_between_all_3():
     X_new, obs, standard_embedding, labels, clusters = setup_melody_data(method="umap")
 
     colors = [
-        'tab:pink', 'tab:green', 'tab:blue', 'tab:red', 'tab:orange',
-        'tab:purple', 'tab:cyan', 'tab:olive', 'tab:brown']
+        "tab:pink",
+        "tab:green",
+        "tab:blue",
+        "tab:red",
+        "tab:orange",
+        "tab:purple",
+        "tab:cyan",
+        "tab:olive",
+        "tab:brown",
+    ]
 
-    fig, axi = plt.subplots(1, 3, figsize=((7.125-0.17), ((7.125-0.17)/1.8)/1.618))
-    plt.tight_layout()
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters, color_scheme=colors)
-    # print(plot_inst.get_num_clusters())
+    fig_size = ((7.125 - 0.17), ((7.125 - 0.17) / 1.8) / 1.618)
 
-    sc0 = axi[0].scatter(
-        standard_embedding[:, 0],
-        standard_embedding[:, 1],
-        marker=".",
-        c=labels,
-        cmap=cm.coolwarm,
-        alpha=0.05,
-        s=30
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=1000,
+        facecolor="w",
+        edgecolor="k",
     )
-    
+    spec2 = gridspec.GridSpec(
+        ncols=4,
+        nrows=1,
+        figure=fig,
+        left=0.02,
+        right=1,
+        top=0.77,
+        bottom=0.06,
+        wspace=0.15,
+    )
+    ax1 = fig.add_subplot(spec2[0])
+    ax2 = fig.add_subplot(spec2[1])
+    ax3 = fig.add_subplot(spec2[2])
+    axi = [ax1, ax2, ax3]
+
+    spec23 = gridspec.GridSpecFromSubplotSpec(3, 3, subplot_spec=spec2[3], wspace=0.05)
+    ax4_11 = fig.add_subplot(spec23[0, 0])
+    ax4_12 = fig.add_subplot(spec23[0, 1])
+    ax4_13 = fig.add_subplot(spec23[0, 2])
+    ax4_21 = fig.add_subplot(spec23[1, 0])
+    ax4_22 = fig.add_subplot(spec23[1, 1])
+    ax4_23 = fig.add_subplot(spec23[1, 2])
+    ax4_32 = fig.add_subplot(spec23[2, 1])
+
+    # Local
+    scs = []
+    for val, i in zip([-1, 0, 1], [0, 2, 8]):
+        if val == -1:
+            sc = axi[0].scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color="gray",
+                alpha=0.1,
+                s=30,
+            )
+            sc = axi[1].scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color="gray",
+                alpha=0.1,
+                s=30,
+            )
+            axi[2].scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color="gray",
+                alpha=0.1,
+                s=30,
+            )
+
+        else:
+            sc = axi[0].scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color=matplotlib.colormaps["Paired"].colors[i],
+                alpha=0.3,
+                s=30,
+            )
+
+            sc = axi[1].scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color=matplotlib.colormaps["Paired"].colors[i],
+                alpha=0.3,
+                s=30,
+            )
+
+            axi[2].scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color=matplotlib.colormaps["Paired"].colors[i],
+                alpha=0.3,
+                s=30,
+            )
+
+        scs.append(sc)
+
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters,
+        color_scheme=colors,
+    )
+
     arrows1, arrow_labels1 = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=axi[0],
         scale_circle=2.5,
         move_circle=[0, 0],
         annotate=1.5,
         arrow_width=0.2,
-        plot_scatter=False
+        plot_scatter=False,
     )
 
     axi[0].set_yticks([])
     axi[0].set_xticks([])
     axi[0].set_ylabel("UMAP2", size=8)
     axi[0].set_xlabel("UMAP1", size=8)
     axi[0].set_title("Global clock", size=8)
     axi[0].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[0].xaxis.set_label_coords(x=0.5, y=-0.02)
 
-    # Local
-    scs = []
-    for val, i in zip([-1, 0, 1], [0, 2, 4]):
-        if val == -1:
-            sc = axi[1].scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                            color="gray", alpha=0.1, s=30)
-            axi[2].scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                       color="gray", alpha=0.1, s=30)
-            
-        else:
-            sc = axi[1].scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                                color=matplotlib.colormaps["Paired"].colors[i], alpha=0.3, s=30)
-            
-            axi[2].scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                        color=matplotlib.colormaps["Paired"].colors[i], alpha=0.3, s=30)
-        
-        scs.append(sc)
-
     arrows2, arrow_labels2 = plot_inst.plot_local_clocks(
         standartize_data=False,
         standartize_coef=False,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=axi[1],
-        scale_circles=[1, 1,],
-        move_circles=[[2, -0.6], [-0.5, 0.5]],
-        annotates=[1, 1,1],
+        scale_circles=[
+            1.5,
+            1.3,
+        ],
+        move_circles=[[1.5, 1], [-1, -1]],
+        annotates=[1, 1, 1],
         arrow_width=0.15,
-        clocks_labels=["0", "1"],
+        clocks_labels=["Unpopular", "Popular"],
         plot_scatter=False,
-        plot_hulls=False
+        plot_hulls=False,
     )
 
     axi[1].set_yticks([])
     axi[1].set_xticks([])
     axi[1].set_ylabel("UMAP2", size=8)
     axi[1].set_xlabel("UMAP1", size=8)
     axi[1].set_title("Local clock", size=8)
@@ -323,87 +400,150 @@
     axi[1].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     arrows3, arrow_labels3 = plot_inst.plot_between_clock(
         standartize_data=False,
         standartize_coef=True,
         univar_importance=True,
         ax=axi[2],
-        scale_circles=[1,],
+        scale_circles=[
+            2,
+        ],
         move_circles=[[0, 0]],
-        annotates=[1.0,],
+        annotates=[
+            1.0,
+        ],
         arrow_width=0.15,
         plot_scatter=False,
-        plot_hulls=False
+        plot_hulls=False,
+        clocks_labels=["Unpopular", "Popular"],
     )
 
     arrows_dict = {}
     for i, val in enumerate(arrow_labels3):
         arrows_dict[val] = arrows3[i]
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
     for i, val in enumerate(arrow_labels2):
         arrows_dict[val] = arrows2[i]
 
-    hatches = [plt.plot([],marker="", ls="")[0]] + list(arrows_dict.values())
+    hatches = [plt.plot([], marker="", ls="")[0]] + list(arrows_dict.values())
     labels = ["Factors:"] + list(arrows_dict.keys())
 
-    hatches = [plt.plot([],marker="", ls="")[0]]*2 + \
-        [list(arrows_dict.values())[0]] + [scs[1]] + \
-        [list(arrows_dict.values())[1]] + [scs[2]] + \
-        [list(arrows_dict.values())[2]] + [scs[0]] + \
-        [list(arrows_dict.values())[3]] + [plt.plot([],marker="", ls="")[0]] + \
-        [list(arrows_dict.values())[4]] + [plt.plot([],marker="", ls="")[0]] + \
-        [list(arrows_dict.values())[5]] + [plt.plot([],marker="", ls="")[0]] 
-
-    labels = ["Factors:", "Labels:"] + \
-        [list(arrows_dict.keys())[0]] + ["0"] + \
-        [list(arrows_dict.keys())[1]] + ["1"] + \
-        [list(arrows_dict.keys())[2]] + ["No class"] + \
-        [list(arrows_dict.keys())[3]] + [""] + \
-        [list(arrows_dict.keys())[4]] + [""] + \
-        [list(arrows_dict.keys())[5]] + [""] 
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 2
+        + [list(arrows_dict.values())[0]]
+        + [scs[1]]
+        + [list(arrows_dict.values())[1]]
+        + [scs[2]]
+        + [list(arrows_dict.values())[2]]
+        + [plt.plot([], marker="", ls="")[0]]
+        + [list(arrows_dict.values())[3]]
+        + [plt.plot([], marker="", ls="")[0]]
+        + [list(arrows_dict.values())[4]]
+        + [plt.plot([], marker="", ls="")[0]]
+        + [list(arrows_dict.values())[5]]
+        + [plt.plot([], marker="", ls="")[0]]
+    )
+
+    labels = (
+        ["Factors:", "Labels:"]
+        + [list(arrows_dict.keys())[0]]
+        + ["Unpopular"]
+        + [list(arrows_dict.keys())[1]]
+        + ["Popular"]
+        + [list(arrows_dict.keys())[2]]
+        + [""]
+        + [list(arrows_dict.keys())[3]]
+        + [""]
+        + [list(arrows_dict.keys())[4]]
+        + [""]
+        + [list(arrows_dict.keys())[5]]
+        + [""]
+    )
 
     leg = axi[2].legend(
         hatches,
         labels,
         loc="lower center",
-        bbox_to_anchor=(-0.7, 1.12),
+        bbox_to_anchor=(-0.13, 1.1),
         fontsize=7,
         ncol=7,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
-    for lh in leg.legendHandles: 
+    for lh in leg.legendHandles:
         lh.set_alpha(1)
 
     axi[2].set_yticks([])
     axi[2].set_xticks([])
     axi[2].set_ylabel("UMAP2", size=8)
     axi[2].set_xlabel("UMAP1", size=8)
-    axi[2].set_title("Inter-cluster clock", size=8)
+    axi[2].set_title("Inter-group clock", size=8)
     axi[2].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[2].xaxis.set_label_coords(x=0.5, y=-0.02)
 
-    cbar = fig.colorbar(sc0, ax=axi[0]) # ticks=[100, 50, 0]
-    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
-    cbar.solids.set(alpha=1)
-    cbar.outline.set_visible(False)
-
-    plt.subplots_adjust(
-        left=0.02,
-        right=0.99,
-        top=0.75,
-        bottom=0.06,  
-        wspace=0.18
+    # cbar = fig.colorbar(sc0, ax=axi[0], pad=0.02, aspect=40) # ticks=[100, 50, 0]
+    # cbar.ax.tick_params(labelsize=5, length=0.8, pad=0.2, grid_linewidth=0.08) #labelrotation=90,
+    # cbar.solids.set(alpha=1)
+    # cbar.set_label('Song popularity', size=6, rotation=270, labelpad=8)
+    # cbar.outline.set_visible(False)
+
+    X_new, obs, standard_embedding, labels, clusters = setup_melody_data(
+        method="umap", drop_labels=False
     )
+
+    for (i, o), axi in zip(
+        enumerate(obs), [ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_32]
+    ):
+        im = axi.scatter(
+            standard_embedding[:, 0],
+            standard_embedding[:, 1],
+            marker=".",
+            s=1.3,
+            c=X_new[o],
+            cmap=cm.coolwarm,
+            # vmin=0, vmax=1
+        )
+        axi.set_yticks([])
+        axi.set_xticks([])
+        # axi.yaxis.set_label_coords(x=-0.01, y=0.5)
+        # axi.xaxis.set_label_coords(x=0.5, y=-0.02)
+
+        if o == "Song Length":
+            o = "Song Len."
+        elif o == "Num of Instruments":
+            o = "Num Inst."
+        elif o == "Lyrical Content":
+            o = "Lyrical C."
+        elif o == "Year of Release":
+            o = "Rel. Year"
+        axi.set_title(o, size=5, pad=-14)
+
+    ax4_21.set_ylabel("UMAP2", size=8)
+    ax4_32.set_xlabel("UMAP1", size=8)
+
+    ax4_21.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax4_32.xaxis.set_label_coords(x=0.55, y=-0.07)
+
+    cbar = fig.colorbar(
+        im,
+        ax=[ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_32],
+        pad=0.02,
+        aspect=40,
+    )
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
+    cbar.outline.set_visible(False)
     plt.savefig("plots/paper/melody/melody_3.pdf")
 
 
 # print_melody_all()
 test_between_all_3()
-# teaser()
```

### Comparing `feature_clock-0.0.3/test/test_neftel.py` & `feature_clock-1.0.0/test/test_neftel.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,41 @@
 from src.feature_clock.plot import NonLinearClock
 import scanpy.external as sce
 import phate
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 from hdbscan import HDBSCAN
 
-def make_legend_arrow(legend, orig_handle,
-                      xdescent, ydescent,
-                      width, height, fontsize):
-    p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
+
+def make_legend_arrow(
+        legend,
+        orig_handle,
+        xdescent,
+        ydescent,
+        width,
+        height,
+        fontsize):
+    p = mpatches.FancyArrow(
+        0,
+        0.5 *
+        height,
+        width,
+        0,
+        length_includes_head=True,
+        head_width=0.75 *
+        height)
     return p
 
 
 def read_data(path):
     return sp.read_h5ad(path)
 
 
 def setup_neftel_data(method="tsne"):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/neftel_malignant.h5ad"
+    file_name = "feature_clock_visualization/data/neftel_malignant.h5ad"
     X = read_data(file_name)
 
     obs = [
         "MESlike2",
         "MESlike1",
         "AClike",
         "OPClike",
@@ -34,15 +48,16 @@
         "G1S",
         "G2M",
         "genes_expressed",
     ]
 
     new_data = X.obs[obs].dropna()
     for col in new_data.columns:
-        new_data[col] = (new_data[col] - new_data[col].mean()) / new_data[col].std()
+        new_data[col] = (new_data[col] - new_data[col].mean()
+                         ) / new_data[col].std()
 
     X_new = sp.AnnData(new_data)
 
     # compute umap
     sp.pp.neighbors(X_new)
     if method == "umap":
         sp.tl.umap(X_new, min_dist=2)
@@ -67,16 +82,17 @@
     npc = np.stack((X_new.X[:, 4], X_new.X[:, 5]))
     ac, opc = X_new.X[:, 2], X_new.X[:, 3]
     mes_max = np.max(mes, axis=0)
     npc_max = np.max(npc, axis=0)
     res_vect = np.stack((ac, opc, mes_max, npc_max))
     res_labels = np.max(res_vect, axis=0)
 
-    clusters = HDBSCAN(min_samples=10, min_cluster_size=30).fit_predict(new_data)
-
+    clusters = HDBSCAN(
+        min_samples=10,
+        min_cluster_size=30).fit_predict(new_data)
 
     return new_data, obs, standard_embedding, res_labels, clusters
 
 
 def test_umap():
     X_new, obs, standard_embedding, labels = setup_neftel_data(method="umap")
 
@@ -136,15 +152,15 @@
     plt.subplots_adjust(
         left=0.05,
         right=1,
         top=0.95,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     cbar = fig.colorbar(im, ax=axi.ravel().tolist(), pad=0.1)
-    cbar.ax.tick_params(labelsize=7) 
+    cbar.ax.tick_params(labelsize=7)
     plt.savefig("plots/paper/neftel/plot_neftelAll.pdf")
 
 
 def test_between_all():
     X_new, obs, standard_embedding, labels = setup_neftel_data(method="umap")
 
     fig, ax = plt.subplots(1, figsize=(3.33, 3.33))
@@ -265,30 +281,31 @@
         left=0.05,
         right=0.95,
         top=0.79,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_between.pdf")
 
+
 def test_all_in_row():
     X_new, obs, standard_embedding, labels = setup_neftel_data(method="umap")
 
-    fig, axi = plt.subplots(1, 3, figsize=(7.125-0.66, 2.375))
+    fig, axi = plt.subplots(1, 3, figsize=(7.125 - 0.66, 2.375))
     plt.tight_layout()
     plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, "UMAP")
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=axi[0],
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.6,
-        arrow_width=0.05
+        arrow_width=0.05,
     )
 
     axi[0].set_yticks([])
     axi[0].set_xticks([])
     axi[0].set_ylabel("UMAP2", size=8)
     axi[0].set_xlabel("UMAP1", size=8)
     axi[0].set_title("Global clock", size=8)
@@ -301,15 +318,15 @@
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=axi[1],
         scale_circles=[1, 0.4, 0.25],
         move_circles=[[-0.2, 0], [0.4, 0.3], [-0.1, -0.4]],
         annotates=[0.5, 0.5, 0.3],
-        arrow_width=0.05
+        arrow_width=0.05,
     )
 
     axi[1].set_yticks([])
     axi[1].set_xticks([])
     axi[1].set_ylabel("UMAP2", size=8)
     axi[1].set_xlabel("UMAP1", size=8)
     axi[1].set_title("Local clock", size=8)
@@ -321,15 +338,15 @@
         standartize_data=True,
         standartize_coef=True,
         univar_importance=True,
         ax=axi[2],
         scale_circles=[1, 1.5],
         move_circles=[[0, 0], [0.7, 0]],
         annotates=[0.3, 0.2],
-        arrow_width=0.05
+        arrow_width=0.05,
     )
     axi[2].legend(
         arrows,
         arrow_labels,
         loc="lower center",
         bbox_to_anchor=(-0.84, 1.12),
         fontsize=7,
@@ -340,44 +357,43 @@
         handletextpad=0.5,
     )
 
     axi[2].set_yticks([])
     axi[2].set_xticks([])
     axi[2].set_ylabel("UMAP2", size=8)
     axi[2].set_xlabel("UMAP1", size=8)
-    axi[2].set_title("Inter-cluster clock", size=8)
+    axi[2].set_title("Inter-group clock", size=8)
     axi[2].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[2].xaxis.set_label_coords(x=0.5, y=-0.02)
     plt.subplots_adjust(
         left=0.05,
         right=0.95,
         top=0.79,
         bottom=0.07,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_3.pdf")
 
 
-
 def test_experiment1():
     X_new, obs, standard_embedding, labels = setup_neftel_data(method="umap")
 
-    fig, ax = plt.subplots(1, figsize=(3.4775/2, 3.4775/2))
+    fig, ax = plt.subplots(1, figsize=(3.4775 / 2, 3.4775 / 2))
     plt.tight_layout()
     plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, "UMAP")
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=False,
         univar_importance=True,
         ax=ax,
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.9,
         arrow_width=0.03,
-        angle_shift=5
+        angle_shift=5,
     )
 
     ax.set_yticks([])
     ax.set_xticks([])
     ax.set_ylabel("UMAP2", size=8)
     ax.set_xlabel("UMAP1", size=8)
     # ax.set_title("Malignant cells", size=8)
@@ -387,28 +403,28 @@
         left=0.08,
         right=0.98,
         top=0.95,
         bottom=0.08,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_all_only_clock.pdf")
 
-    fig, ax = plt.subplots(1, figsize=(3.4775/2, 3.4775/2))
+    fig, ax = plt.subplots(1, figsize=(3.4775 / 2, 3.4775 / 2))
     plt.tight_layout()
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=ax,
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.9,
-        arrow_width=0.05
+        arrow_width=0.05,
     )
-    
+
     ax.set_yticks([])
     ax.set_xticks([])
     ax.set_ylabel("UMAP2", size=8)
     ax.set_xlabel("UMAP1", size=8)
     # ax.set_title("Malignant cells", size=8)
     ax.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax.xaxis.set_label_coords(x=0.5, y=-0.02)
@@ -418,30 +434,31 @@
         top=0.95,
         bottom=0.08,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_biggest_only_clock.pdf")
 
 
 def test_experiment2():
-    X_new, obs, standard_embedding, labels, _ = setup_neftel_data(method="umap")
+    X_new, obs, standard_embedding, labels, _ = setup_neftel_data(
+        method="umap")
 
-    fig, ax = plt.subplots(1, figsize=(3.4775/2, 3.4775/2))
+    fig, ax = plt.subplots(1, figsize=(3.4775 / 2, 3.4775 / 2))
     plt.tight_layout()
     plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, "UMAP")
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=False,
         univar_importance=True,
         ax=ax,
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.9,
         arrow_width=0.01,
-        angle_shift=1
+        angle_shift=1,
     )
 
     ax.set_yticks([])
     ax.set_xticks([])
     ax.set_ylabel("UMAP2", size=8)
     ax.set_xlabel("UMAP1", size=8)
     # ax.set_title("Malignant cells", size=8)
@@ -450,28 +467,28 @@
     plt.subplots_adjust(
         left=0.08,
         right=0.98,
         top=0.95,
         bottom=0.08,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_all_1_degree.pdf")
-    
-    fig, ax = plt.subplots(1, figsize=(3.4775/2, 3.4775/2))
+
+    fig, ax = plt.subplots(1, figsize=(3.4775 / 2, 3.4775 / 2))
     plt.tight_layout()
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=False,
         univar_importance=True,
         ax=ax,
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.9,
         arrow_width=0.01,
-        angle_shift=5
+        angle_shift=5,
     )
 
     ax.set_yticks([])
     ax.set_xticks([])
     ax.set_ylabel("UMAP2", size=8)
     ax.set_xlabel("UMAP1", size=8)
     # ax.set_title("Malignant cells", size=8)
@@ -481,26 +498,25 @@
         left=0.08,
         right=0.98,
         top=0.95,
         bottom=0.08,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_all_5_degree.pdf")
 
-    
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=False,
         univar_importance=True,
         ax=ax,
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.9,
         arrow_width=0.01,
-        angle_shift=15
+        angle_shift=15,
     )
 
     ax.set_yticks([])
     ax.set_xticks([])
     ax.set_ylabel("UMAP2", size=8)
     ax.set_xlabel("UMAP1", size=8)
     # ax.set_title("Malignant cells", size=8)
@@ -512,52 +528,67 @@
         top=0.95,
         bottom=0.08,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_all_15_degree.pdf")
 
 
 def test_all_4_in_row():
-    X_new, obs, standard_embedding, labels, _ = setup_neftel_data(method="umap")
+    X_new, obs, standard_embedding, labels, _ = setup_neftel_data(
+        method="umap")
 
     # fig, axi = plt.subplots(1, 3, figsize=(7.125-0.66, 2.375))
     # plt.tight_layout()
 
     dpi = 1000
-    fig_size = ((7.125-0.17), ((7.125-0.17)/1.8)/1.618)
+    fig_size = ((7.125 - 0.17), ((7.125 - 0.17) / 1.8) / 1.618)
 
-    fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=dpi, facecolor="w",edgecolor="k",)
-    spec2 = gridspec.GridSpec(ncols=4, nrows=1, figure=fig, 
-                     left=0.02, right=1, top=0.82, bottom=0.06, wspace=0.15)
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=dpi,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=4,
+        nrows=1,
+        figure=fig,
+        left=0.02,
+        right=1,
+        top=0.82,
+        bottom=0.06,
+        wspace=0.15,
+    )
     ax1 = fig.add_subplot(spec2[0])
     ax2 = fig.add_subplot(spec2[1])
     ax3 = fig.add_subplot(spec2[2])
 
-    spec23 = gridspec.GridSpecFromSubplotSpec(3, 3, subplot_spec=spec2[3], wspace=0.05)
+    spec23 = gridspec.GridSpecFromSubplotSpec(
+        3, 3, subplot_spec=spec2[3], wspace=0.05)
     ax4_11 = fig.add_subplot(spec23[0, 0])
     ax4_12 = fig.add_subplot(spec23[0, 1])
     ax4_13 = fig.add_subplot(spec23[0, 2])
     ax4_21 = fig.add_subplot(spec23[1, 0])
     ax4_22 = fig.add_subplot(spec23[1, 1])
     ax4_23 = fig.add_subplot(spec23[1, 2])
     ax4_31 = fig.add_subplot(spec23[2, 0])
     ax4_32 = fig.add_subplot(spec23[2, 1])
     ax4_33 = fig.add_subplot(spec23[2, 2])
 
-
     plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, "UMAP")
     arrows1, arrow_labels1 = plot_inst.plot_global_clock(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=ax1,
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.6,
-        arrow_width=0.05
+        arrow_width=0.05,
     )
 
     ax1.set_yticks([])
     ax1.set_xticks([])
     ax1.set_ylabel("UMAP2", size=8)
     ax1.set_xlabel("UMAP1", size=8)
     ax1.set_title("Global clock", size=8)
@@ -570,15 +601,15 @@
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=ax2,
         scale_circles=[1.5, 0.9],
         move_circles=[[-0.6, 0.1], [0.6, -0.2]],
         annotates=[0.5, 0.5],
-        arrow_width=0.05
+        arrow_width=0.05,
     )
 
     ax2.set_yticks([])
     ax2.set_xticks([])
     ax2.set_ylabel("UMAP2", size=8)
     ax2.set_xlabel("UMAP1", size=8)
     ax2.set_title("Local clock", size=8)
@@ -590,150 +621,216 @@
         standartize_data=True,
         standartize_coef=True,
         univar_importance=True,
         ax=ax3,
         scale_circles=[1.5, 1.5],
         move_circles=[[0, 0], [0.7, 0]],
         annotates=[0.4, 0.2],
-        arrow_width=0.05
+        arrow_width=0.05,
     )
 
     arrows_dict = {}
     for i, val in enumerate(arrow_labels3):
         arrows_dict[val] = arrows3[i]
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
     for i, val in enumerate(arrow_labels2):
         arrows_dict[val] = arrows2[i]
-    
-    hatches = [plt.plot([],marker="", ls="")[0]] + list(arrows_dict.values())
+
+    hatches = [plt.plot([], marker="", ls="")[0]] + list(arrows_dict.values())
     labels = ["Factors:"] + list(arrows_dict.keys())
 
     leg = ax3.legend(
         hatches,
         labels,
         loc="lower center",
         bbox_to_anchor=(-0.13, 1.1),
         fontsize=7,
         ncol=10,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     ax3.set_yticks([])
     ax3.set_xticks([])
     ax3.set_ylabel("UMAP2", size=8)
     ax3.set_xlabel("UMAP1", size=8)
-    ax3.set_title("Inter-cluster clock", size=8)
+    ax3.set_title("Inter-group clock", size=8)
     ax3.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax3.xaxis.set_label_coords(x=0.5, y=-0.02)
 
     X_new, obs, standard_embedding, labels = setup_neftel_data(method="umap")
-    
-    for (i, o), axi in zip(enumerate(obs), [ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33]):
+
+    for (i, o), axi in zip(
+        enumerate(obs),
+        [ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33],
+    ):
         im = axi.scatter(
             standard_embedding[:, 0],
             standard_embedding[:, 1],
             marker=".",
             s=1.3,
             c=X_new[o],
             cmap="Spectral",
             # vmin=0, vmax=1
         )
         axi.set_yticks([])
         axi.set_xticks([])
         # axi.yaxis.set_label_coords(x=-0.01, y=0.5)
         # axi.xaxis.set_label_coords(x=0.5, y=-0.02)
-        
+
         if o == "genes_expressed":
             o = "genes_exp."
         axi.set_title(o, size=5, pad=-14)
 
     ax4_21.set_ylabel("UMAP2", size=8)
     ax4_32.set_xlabel("UMAP1", size=8)
 
     ax4_21.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax4_32.xaxis.set_label_coords(x=0.55, y=-0.07)
 
-    cbar = fig.colorbar(im, ax=[ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33], 
-                        pad=0.02, aspect=40)
-    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
+    cbar = fig.colorbar(
+        im,
+        ax=[ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33],
+        pad=0.02,
+        aspect=40,
+    )
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
     cbar.outline.set_visible(False)
 
     plt.savefig("plots/paper/neftel/neftel_3.pdf")
 
 
 def test_all_4_in_row_hdbscan():
-    X_new, obs, standard_embedding, labels, clusters = setup_neftel_data(method="umap")
-
-    # fig, axi = plt.subplots(1, 3, figsize=(7.125-0.66, 2.375))
-    # plt.tight_layout()
+    X_new, obs, standard_embedding, labels, clusters = setup_neftel_data(
+        method="umap")
 
     dpi = 1000
-    fig_size = ((7.125-0.17), ((7.125-0.17)/1.8)/1.618)
+    fig_size = ((7.125 - 0.17), ((7.125 - 0.17) / 1.8) / 1.618)
 
-    fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=dpi, facecolor="w",edgecolor="k",)
-    spec2 = gridspec.GridSpec(ncols=4, nrows=1, figure=fig, 
-                     left=0.02, right=1, top=0.77, bottom=0.06, wspace=0.15)
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=dpi,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=4,
+        nrows=1,
+        figure=fig,
+        left=0.02,
+        right=1,
+        top=0.77,
+        bottom=0.06,
+        wspace=0.15,
+    )
     ax1 = fig.add_subplot(spec2[0])
     ax2 = fig.add_subplot(spec2[1])
     ax3 = fig.add_subplot(spec2[2])
 
-    spec23 = gridspec.GridSpecFromSubplotSpec(3, 3, subplot_spec=spec2[3], wspace=0.05)
+    spec23 = gridspec.GridSpecFromSubplotSpec(
+        3, 3, subplot_spec=spec2[3], wspace=0.05)
     ax4_11 = fig.add_subplot(spec23[0, 0])
     ax4_12 = fig.add_subplot(spec23[0, 1])
     ax4_13 = fig.add_subplot(spec23[0, 2])
     ax4_21 = fig.add_subplot(spec23[1, 0])
     ax4_22 = fig.add_subplot(spec23[1, 1])
     ax4_23 = fig.add_subplot(spec23[1, 2])
     ax4_31 = fig.add_subplot(spec23[2, 0])
     ax4_32 = fig.add_subplot(spec23[2, 1])
     ax4_33 = fig.add_subplot(spec23[2, 2])
 
     scs = []
-    for val, i in zip([-1, 0, 1], [0, 2, 4]):
+    for val, i in zip([-1, 0, 1], [0, 2, 8]):
         if val == -1:
-            sc = ax1.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                            color="gray", alpha=0.1, s=30)
-            ax2.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                            color="gray", alpha=0.1, s=30)
-            ax3.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                       color="gray", alpha=0.1, s=30)
-            
+            sc = ax1.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color="gray",
+                alpha=0.1,
+                s=30,
+            )
+            ax2.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color="gray",
+                alpha=0.1,
+                s=30,
+            )
+            ax3.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color="gray",
+                alpha=0.1,
+                s=30,
+            )
+
         else:
-            sc = ax1.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                                color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=30)
-            
-            ax2.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                        color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=30)
-            ax3.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                       color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=30)
-        
+            sc = ax1.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color=matplotlib.colormaps["Paired"].colors[i],
+                alpha=0.2,
+                s=30,
+            )
+
+            ax2.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color=matplotlib.colormaps["Paired"].colors[i],
+                alpha=0.2,
+                s=30,
+            )
+            ax3.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color=matplotlib.colormaps["Paired"].colors[i],
+                alpha=0.2,
+                s=30,
+            )
+
         scs.append(sc)
 
     print(clusters)
 
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters)
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters)
     arrows1, arrow_labels1 = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=ax1,
         scale_circle=1.5,
         move_circle=[0, 0],
         annotate=5.5,
         arrow_width=0.5,
-        plot_scatter=False
+        plot_scatter=False,
     )
 
     ax1.set_yticks([])
     ax1.set_xticks([])
     ax1.set_ylabel("UMAP2", size=8)
     ax1.set_xlabel("UMAP1", size=8)
     ax1.set_title("Global clock", size=8)
@@ -745,20 +842,20 @@
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=ax2,
         scale_circles=[0.3, 0.4],
         clocks_labels=["0", "1"],
-        clocks_labels_angles = [45, 270],
+        clocks_labels_angles=[45, 270],
         move_circles=[[0, 0], [0, 0]],
         annotates=[5, 3],
         arrow_width=0.45,
         plot_hulls=False,
-        plot_scatter=False
+        plot_scatter=False,
     )
 
     ax2.set_yticks([])
     ax2.set_xticks([])
     ax2.set_ylabel("UMAP2", size=8)
     ax2.set_xlabel("UMAP1", size=8)
     ax2.set_title("Local clock", size=8)
@@ -772,106 +869,139 @@
         univar_importance=True,
         ax=ax3,
         scale_circles=[1, 1],
         move_circles=[[0, 0], [0.0, 0]],
         annotates=[5],
         arrow_width=0.5,
         plot_hulls=False,
-        plot_scatter=False
+        plot_scatter=False,
     )
 
     arrows_dict = {}
     for i, val in enumerate(arrow_labels3):
         arrows_dict[val] = arrows3[i]
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
     for i, val in enumerate(arrow_labels2):
         arrows_dict[val] = arrows2[i]
-    
-    hatches = [plt.plot([],marker="", ls="")[0]]*2 + \
-        [list(arrows_dict.values())[0]] + [scs[1]] + \
-        [list(arrows_dict.values())[1]] + [scs[2]] + \
-        [list(arrows_dict.values())[2]] + [scs[0]] + \
-        [list(arrows_dict.values())[3]] + [plt.plot([],marker="", ls="")[0]] + \
-        [list(arrows_dict.values())[4]] + [plt.plot([],marker="", ls="")[0]] + \
-        [list(arrows_dict.values())[5]] + [plt.plot([],marker="", ls="")[0]] + \
-        [list(arrows_dict.values())[6]] + [plt.plot([],marker="", ls="")[0]] + \
-        [list(arrows_dict.values())[7]] + [plt.plot([],marker="", ls="")[0]] + \
-        [list(arrows_dict.values())[8]] + [plt.plot([],marker="", ls="")[0]]
-
-    labels = ["Factors:", "Labels:"] + \
-        [list(arrows_dict.keys())[0]] + ["0"] + \
-        [list(arrows_dict.keys())[1]] + ["1"] + \
-        [list(arrows_dict.keys())[2]] + ["No class"] + \
-        [list(arrows_dict.keys())[3]] + [""] + \
-        [list(arrows_dict.keys())[4]] + [""] + \
-        [list(arrows_dict.keys())[5]] + [""] + \
-        [list(arrows_dict.keys())[6]] + [""] + \
-        [list(arrows_dict.keys())[7]] + [""] + \
-        [list(arrows_dict.keys())[8]] + [""]
+
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 2
+        + [list(arrows_dict.values())[0]]
+        + [scs[1]]
+        + [list(arrows_dict.values())[1]]
+        + [scs[2]]
+        + [list(arrows_dict.values())[2]]
+        + [scs[0]]
+        + [list(arrows_dict.values())[3]]
+        + [plt.plot([], marker="", ls="")[0]]
+        + [list(arrows_dict.values())[4]]
+        + [plt.plot([], marker="", ls="")[0]]
+        + [list(arrows_dict.values())[5]]
+        + [plt.plot([], marker="", ls="")[0]]
+        + [list(arrows_dict.values())[6]]
+        + [plt.plot([], marker="", ls="")[0]]
+        + [list(arrows_dict.values())[7]]
+        + [plt.plot([], marker="", ls="")[0]]
+        + [list(arrows_dict.values())[8]]
+        + [plt.plot([], marker="", ls="")[0]]
+    )
+
+    labels = (
+        ["Factors:", "Labels:"]
+        + [list(arrows_dict.keys())[0]]
+        + ["0"]
+        + [list(arrows_dict.keys())[1]]
+        + ["1"]
+        + [list(arrows_dict.keys())[2]]
+        + ["No class"]
+        + [list(arrows_dict.keys())[3]]
+        + [""]
+        + [list(arrows_dict.keys())[4]]
+        + [""]
+        + [list(arrows_dict.keys())[5]]
+        + [""]
+        + [list(arrows_dict.keys())[6]]
+        + [""]
+        + [list(arrows_dict.keys())[7]]
+        + [""]
+        + [list(arrows_dict.keys())[8]]
+        + [""]
+    )
 
     leg = ax3.legend(
         hatches,
         labels,
         loc="lower center",
         bbox_to_anchor=(-0.13, 1.1),
         fontsize=7,
         ncol=10,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
-    for lh in leg.legendHandles: 
+    for lh in leg.legendHandles:
         lh.set_alpha(1)
 
     ax3.set_yticks([])
     ax3.set_xticks([])
     ax3.set_ylabel("UMAP2", size=8)
     ax3.set_xlabel("UMAP1", size=8)
-    ax3.set_title("Inter-cluster clock", size=8)
+    ax3.set_title("Inter-group clock", size=8)
     ax3.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax3.xaxis.set_label_coords(x=0.5, y=-0.02)
 
-    X_new, obs, standard_embedding, labels, clusters = setup_neftel_data(method="umap")
-    
-    for (i, o), axi in zip(enumerate(obs), [ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33]):
+    X_new, obs, standard_embedding, labels, clusters = setup_neftel_data(
+        method="umap")
+
+    for (i, o), axi in zip(
+        enumerate(obs),
+        [ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33],
+    ):
         im = axi.scatter(
             standard_embedding[:, 0],
             standard_embedding[:, 1],
             marker=".",
             s=1.3,
             c=X_new[o],
             cmap=cm.coolwarm,
             # vmin=0, vmax=1
         )
         axi.set_yticks([])
         axi.set_xticks([])
         # axi.yaxis.set_label_coords(x=-0.01, y=0.5)
         # axi.xaxis.set_label_coords(x=0.5, y=-0.02)
-        
+
         if o == "genes_expressed":
             o = "genes_exp."
         axi.set_title(o, size=5, pad=-14)
 
     ax4_21.set_ylabel("UMAP2", size=8)
     ax4_32.set_xlabel("UMAP1", size=8)
 
     ax4_21.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax4_32.xaxis.set_label_coords(x=0.55, y=-0.07)
 
-    cbar = fig.colorbar(im, ax=[ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33], 
-                        pad=0.02, aspect=40)
-    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
+    cbar = fig.colorbar(
+        im,
+        ax=[ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33],
+        pad=0.02,
+        aspect=40,
+    )
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
     cbar.outline.set_visible(False)
 
     plt.savefig("plots/paper/neftel/neftel_3.pdf")
 
 
 # test_between_all()
-test_all_4_in_row_hdbscan()
 # print_neftel_all()
-# test_experiment2()
+test_all_4_in_row_hdbscan()
```

### Comparing `feature_clock-0.0.3/test/test_pima.py` & `feature_clock-1.0.0/test/test_pima.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,45 @@
-from matplotlib import pyplot as plt
+from matplotlib import cm, gridspec, pyplot as plt
 from matplotlib.legend_handler import HandlerPatch
 import numpy as np
 import pandas as pd
 from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
-def make_legend_arrow(legend, orig_handle,
-                      xdescent, ydescent,
-                      width, height, fontsize):
-    p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
-    return p
 
+def make_legend_arrow(
+        legend,
+        orig_handle,
+        xdescent,
+        ydescent,
+        width,
+        height,
+        fontsize):
+    p = mpatches.FancyArrow(
+        0,
+        0.5 *
+        height,
+        width,
+        0,
+        length_includes_head=True,
+        head_width=0.75 *
+        height)
+    return p
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_pima_data(method="tsne", drop_labels=True):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/diabetes.csv"
+    file_name = "feature_clock_visualization/data/diabetes.csv"
     X = read_data(file_name)
     X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     X = X.dropna()
 
     labels = X["Outcome"]
     if drop_labels:
         X.drop(columns=["Outcome"], inplace=True)
@@ -45,36 +58,49 @@
             standard_embedding = reducer.fit_transform(X)
 
     elif method == "tsne":
         raise NotImplementedError()
 
     elif method == "phate":
         raise NotImplementedError()
-    
+
     # get clusters
     clusters = HDBSCAN(min_samples=12).fit_predict(X)
     # clusters = KMeans(n_clusters=3, n_init="auto", max_iter=1000).fit_predict(X)
 
     return X, obs, standard_embedding, labels, clusters
 
+
 def print_pima_all():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap", drop_labels=False)
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="umap", drop_labels=False
+    )
     dpi = 1000
     # fig_size = (2.375, 2.375)
     fig_size = (3.2325, 2.9)
     fig, axi = plt.subplots(
         3,
         3,
         num=None,
         figsize=fig_size,
         dpi=dpi,
         facecolor="w",
         edgecolor="k",
     )
-    names = {'SkinThickness': 'a', 'Insulin': 'd', 'BMI': 'g', 'Age': 'b', 'Pregnancies': 'e', "Pedigree": "h", 'BloodPressure': 'c', 'Glucose': 'f', "Outcome": "i"}
+    names = {
+        "SkinThickness": "a",
+        "Insulin": "d",
+        "BMI": "g",
+        "Age": "b",
+        "Pregnancies": "e",
+        "Pedigree": "h",
+        "BloodPressure": "c",
+        "Glucose": "f",
+        "Outcome": "i",
+    }
     for i, o in enumerate(list(names.keys())):
         im = axi[i % 3, i // 3].scatter(
             standard_embedding[:, 0],
             standard_embedding[:, 1],
             marker=".",
             s=1.3,
             c=X_new[o],
@@ -92,37 +118,44 @@
     plt.subplots_adjust(
         left=0.05,
         right=1,
         top=0.95,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     # cbar = fig.colorbar(im, ax=axi.ravel().tolist(), pad=0.1)
-    # cbar.ax.tick_params(labelsize=7) 
+    # cbar.ax.tick_params(labelsize=7)
     for ax in axi:
         for a in ax:
-            a.axis('off') 
+            a.axis("off")
     plt.savefig("plots/paper/pima/plot_pimaAll_teaser.pdf")
 
 
 def test_between_all():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="umap")
 
     fig, ax = plt.subplots(1, figsize=(3.33, 2.8))
     plt.tight_layout()
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters)
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters)
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax,
         scale_circle=1,
         move_circle=[0, 0],
         annotate=0.6,
-        arrow_width=1.5
+        arrow_width=1.5,
     )
     ax.legend(
         arrows,
         arrow_labels,
         loc="lower center",
         bbox_to_anchor=(0.5, 1.07),
         fontsize=7,
@@ -227,24 +260,86 @@
         top=0.79,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/pima/pima_between.pdf")
 
 
 def test_between_all_3():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="umap")
     colors = [
-        'tab:pink', 'tab:green', 'tab:blue', 'tab:orange',
-        'tab:purple', 'tab:cyan', 'tab:red', 'tab:brown', 'tab:olive']
+        "tab:pink",
+        "tab:green",
+        "tab:blue",
+        "tab:orange",
+        "tab:purple",
+        "tab:cyan",
+        "tab:red",
+        "tab:brown",
+        "tab:olive",
+    ]
 
-    fig, axi = plt.subplots(1, 3, figsize=((7.125-0.17), ((7.125-0.17)/1.8)/1.618))
-    plt.tight_layout()
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=labels, color_scheme=colors)
-    
-    sc = axi[0].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
+    dpi = 1000
+    fig_size = ((7.125 - 0.17), ((7.125 - 0.17) / 1.8) / 1.618)
+
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=dpi,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=4,
+        nrows=1,
+        figure=fig,
+        left=0.02,
+        right=1,
+        top=0.77,
+        bottom=0.06,
+        wspace=0.15,
+    )
+    ax1 = fig.add_subplot(spec2[0])
+    ax2 = fig.add_subplot(spec2[1])
+    ax3 = fig.add_subplot(spec2[2])
+
+    spec23 = gridspec.GridSpecFromSubplotSpec(
+        3, 3, subplot_spec=spec2[3], wspace=0.05, hspace=0.05
+    )
+    ax4_11 = fig.add_subplot(spec23[0, 0])
+    ax4_12 = fig.add_subplot(spec23[0, 1])
+    ax4_13 = fig.add_subplot(spec23[0, 2])
+    ax4_21 = fig.add_subplot(spec23[1, 0])
+    ax4_22 = fig.add_subplot(spec23[1, 1])
+    ax4_23 = fig.add_subplot(spec23[1, 2])
+    ax4_31 = fig.add_subplot(spec23[2, 0])
+    ax4_32 = fig.add_subplot(spec23[2, 1])
+    ax4_33 = fig.add_subplot(spec23[2, 2])
+
+    axi = [ax1, ax2, ax3]
+
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=labels,
+        color_scheme=colors,
+    )
+
+    sc = axi[0].scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="Accent",
+        zorder=0,
+        alpha=0.2,
+    )
     # legend1 = axi[0].legend(
     #     handles = sc.legend_elements()[0],
     #     loc="upper center",
     #     # bbox_to_anchor=(0.0, 0.0),
     #     fontsize=7,
     #     ncol=3,
     #     markerscale=0.6,
@@ -260,52 +355,68 @@
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=axi[0],
         scale_circle=2.5,
         move_circle=[0, 0],
         annotate=1.0,
-        arrow_width=0.08
+        arrow_width=0.08,
     )
     axi[0].set_yticks([])
     axi[0].set_xticks([])
     axi[0].set_ylabel("UMAP2", size=8)
     axi[0].set_xlabel("UMAP1", size=8)
     axi[0].set_title("Global clock", size=8)
     axi[0].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[0].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     # Local
-    sc = axi[1].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
+    sc = axi[1].scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="Accent",
+        zorder=0,
+        alpha=0.2,
+    )
 
     arrows2, arrow_labels2 = plot_inst.plot_local_clocks(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=axi[1],
         scale_circles=[1.5, 1.5],
         move_circles=[[-2.2, 0], [2.5, 0]],
         annotates=[0.9, 0.9],
         clocks_labels=["Healthy", "Diabetes"],
         arrow_width=0.08,
         plot_scatter=False,
-        plot_hulls=False
+        plot_hulls=False,
     )
 
     axi[1].set_yticks([])
     axi[1].set_xticks([])
     axi[1].set_ylabel("UMAP2", size=8)
     axi[1].set_xlabel("UMAP1", size=8)
     axi[1].set_title("Local clock", size=8)
     axi[1].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[1].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     # Between
-    sc = axi[2].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
+    sc = axi[2].scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="Accent",
+        zorder=0,
+        alpha=0.2,
+    )
 
     arrows3, arrow_labels3 = plot_inst.plot_between_clock(
         standartize_data=True,
         standartize_coef=True,
         univar_importance=False,
         ax=axi[2],
         scale_circles=[4],
@@ -320,125 +431,186 @@
     arrows_dict = {}
     for i, val in enumerate(arrow_labels3):
         arrows_dict[val] = arrows3[i]
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
     for i, val in enumerate(arrow_labels2):
         arrows_dict[val] = arrows2[i]
-    
+
     # hatches = [plt.plot([],marker="", ls="")[0]]*2 + list(arrows_dict.values()) + sc.legend_elements()[0]
     # labels = ["Factors:", "Labels:"] + list(arrows_dict.keys()) + ["Healthy", "Diabetis"]
 
-    hatches = [plt.plot([],marker="", ls="")[0]]*2 + \
-        [list(arrows_dict.values())[0]] + [sc.legend_elements()[0][0]] + \
-        [list(arrows_dict.values())[1]] + [sc.legend_elements()[0][1]] + \
-        list(arrows_dict.values())[2:]
-    
-    labels = ["Factors:", "Labels:"] + [list(arrows_dict.keys())[0]] + ["Healthy"] + \
-        [list(arrows_dict.keys())[1]] + ["Diabetes"] + \
-        list(arrows_dict.keys())[2:]
-
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 2
+        + [list(arrows_dict.values())[0]]
+        + [sc.legend_elements()[0][0]]
+        + [list(arrows_dict.values())[1]]
+        + [sc.legend_elements()[0][1]]
+        + list(arrows_dict.values())[2:]
+    )
+
+    labels = (
+        ["Factors:", "Labels:"]
+        + [list(arrows_dict.keys())[0]]
+        + ["Healthy"]
+        + [list(arrows_dict.keys())[1]]
+        + ["Diabetes"]
+        + list(arrows_dict.keys())[2:]
+    )
 
-    leg = axi[1].legend(
+    leg = axi[2].legend(
         hatches,
         labels,
         loc="lower center",
-        bbox_to_anchor=(0.5, 1.12),
+        bbox_to_anchor=(-0.13, 1.1),
         fontsize=7,
         ncol=9,
         markerscale=0.6,
         handlelength=1.3,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
-        # markerfirst=False 
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
+        # markerfirst=False
     )
-    for lh in leg.legendHandles: 
+    for lh in leg.legendHandles:
         lh.set_alpha(1)
 
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     axi[2].set_yticks([])
     axi[2].set_xticks([])
     axi[2].set_ylabel("UMAP2", size=8)
     axi[2].set_xlabel("UMAP1", size=8)
-    axi[2].set_title("Inter-cluster clock", size=8)
+    axi[2].set_title("Inter-group clock", size=8)
     axi[2].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[2].xaxis.set_label_coords(x=0.5, y=-0.02)
-    plt.subplots_adjust(
-        left=0.02,
-        right=0.98,
-        top=0.75,
-        bottom=0.06,  
-        wspace=0.1, 
-        # hspace=0.1
+
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="umap", drop_labels=False
     )
+
+    for (i, o), axi in zip(
+        enumerate(obs),
+        [ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33],
+    ):
+        im = axi.scatter(
+            standard_embedding[:, 0],
+            standard_embedding[:, 1],
+            marker=".",
+            s=1.3,
+            c=X_new[o],
+            cmap=cm.coolwarm,
+            # vmin=0, vmax=1
+        )
+        axi.set_yticks([])
+        axi.set_xticks([])
+        # axi.yaxis.set_label_coords(x=-0.01, y=0.5)
+        # axi.xaxis.set_label_coords(x=0.5, y=-0.02)
+
+        axi.set_aspect("equal")
+        print(axi.get_ylim())
+        axi.set_ylim((axi.get_ylim()[0] - 2, axi.get_ylim()[1] + 2))
+
+        if o == "Outcome":
+            o = "Labels"
+        elif o == "BloodPressure":
+            o = "BloodPr."
+        axi.set_title(o, size=5, pad=-14)
+
+    ax4_21.set_ylabel("UMAP2", size=8)
+    ax4_32.set_xlabel("UMAP1", size=8)
+
+    ax4_21.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax4_32.xaxis.set_label_coords(x=0.55, y=-0.07)
+
+    cbar = fig.colorbar(
+        im,
+        ax=[ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33],
+        pad=0.02,
+        aspect=40,
+        ticks=[1.0, 0.5, 0.0, -0.5],
+    )
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
+    cbar.outline.set_visible(False)
+
     plt.savefig("plots/paper/pima/pima_3.pdf")
 
 
 def teaser():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="umap")
 
-    fig, axi = plt.subplots(1, 1, figsize=(2.375, 2.375))
+    fig, axi = plt.subplots(1, 1, figsize=(1, 1))
     plt.tight_layout()
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters)
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters)
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=axi,
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.8,
         arrow_width=0.08,
+        plot_scatter=False,
     )
 
     axi.set_yticks([])
     axi.set_xticks([])
     # axi[1].set_ylabel("UMAP2", size=8)
     # axi[1].set_xlabel("UMAP1", size=8)
     # axi[1].set_title("Diabetis", size=8)
     # axi[1].yaxis.set_label_coords(x=-0.01, y=0.5)
     # axi[1].xaxis.set_label_coords(x=0.5, y=-0.02)
 
-    
     names_dict = {}
     letters = ["a", "b", "c", "d", "e", "f", "g", "h", "i"]
     for a, l in zip(arrow_labels, letters):
         names_dict[a] = l
     print(names_dict)
-    leg = axi.legend(
-        arrows,
-        letters,
-        loc="lower center",
-        bbox_to_anchor=(0.5, 0.88),
-        fontsize=7,
-        ncol=8,
-        markerscale=0.6,
-        handlelength=1.5,
-        columnspacing=0.8,
-        handletextpad=0.5,
-       handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
-    )
+    # leg = axi.legend(
+    #     arrows,
+    #     letters,
+    #     loc="lower center",
+    #     bbox_to_anchor=(0.5, 0.88),
+    #     fontsize=7,
+    #     ncol=8,
+    #     markerscale=0.6,
+    #     handlelength=1.5,
+    #     columnspacing=0.8,
+    #     handletextpad=0.5,
+    #    handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+    # )
 
     # axi[0].set_yticks([])
     # axi[0].set_xticks([])
     # axi[0].set_ylabel("UMAP2", size=8)
     # axi[0].set_xlabel("UMAP1", size=8)
     # axi[0].set_title("Diabetis", size=8)
     # axi[0].yaxis.set_label_coords(x=-0.01, y=0.5)
     # axi[0].xaxis.set_label_coords(x=0.5, y=-0.02)
-    axi.axis('off')
+    axi.axis("off")
     plt.subplots_adjust(
         left=0.01,
         right=0.99,
         top=0.98,
         bottom=0.01,  # wspace=0.21, hspace=0.33
     )
-    plt.savefig("plots/paper/pima/pima_general_clock.pdf")
+    plt.savefig("plots/paper/pima/pima_only_clock.pdf")
+
 
 # print_pima_all()
 test_between_all_3()
 # teaser()
```

### Comparing `feature_clock-0.0.3/test/test_pima_autoencoder.py` & `feature_clock-1.0.0/test/test_pima_autoencoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
-def make_legend_arrow(legend, orig_handle,
-                      xdescent, ydescent,
-                      width, height, fontsize):
-    p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
+
+def make_legend_arrow(legend, orig_handle, xdescent, ydescent, width, height, fontsize):
+    p = mpatches.FancyArrow(
+        0, 0.5 * height, width, 0, length_includes_head=True, head_width=0.75 * height
+    )
     return p
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
-def setup_pima_data(method="tsne", drop_labels=True, file: str=""):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/diabetes.csv"
+def setup_pima_data(method="tsne", drop_labels=True, file: str = ""):
+    file_name = "feature_clock_visualization/data/diabetes.csv"
     X = read_data(file_name)
     X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     X = X.dropna()
 
     labels = X["Outcome"]
     if drop_labels:
         X.drop(columns=["Outcome"], inplace=True)
     obs = list(X.columns)
 
     for col in X.columns:
         X[col] = (X[col] - X[col].mean()) / X[col].std()
-    
+
     file_name2 = file
     Y = read_data(file_name2)
     Y.drop(columns=["target"], inplace=True)
     print(Y.shape)
 
     Y = np.array(Y)
 
@@ -48,30 +49,34 @@
         standard_embedding = reducer.fit_transform(Y)
 
     elif method == "tsne":
         raise NotImplementedError()
 
     elif method == "phate":
         raise NotImplementedError()
-    
+
     for i in range(standard_embedding.shape[1]):
-        standard_embedding[:, i] = (standard_embedding[:, i] - standard_embedding[:, i].mean()) / standard_embedding[:, i].std()
-    
+        standard_embedding[:, i] = (
+            standard_embedding[:, i] - standard_embedding[:, i].mean()
+        ) / standard_embedding[:, i].std()
 
     standard_embedding[:, 0] = 3 * standard_embedding[:, 0]
     standard_embedding[:, 1] = 1 * standard_embedding[:, 1]
 
     # get clusters
     clusters = HDBSCAN(min_samples=12).fit_predict(X)
     # clusters = KMeans(n_clusters=3, n_init="auto", max_iter=1000).fit_predict(X)
 
     return X, obs, standard_embedding, labels, clusters
 
+
 def print_pima_all(file, dataset_i):
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="none", drop_labels=False, file=file)
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="none", drop_labels=False, file=file
+    )
     dpi = 1000
     # fig_size = (2.375, 2.375)
     fig_size = (3.2325, 2.9)
     fig, axi = plt.subplots(
         3,
         3,
         num=None,
@@ -93,119 +98,184 @@
         axi[i % 3, i // 3].set_xticks([])
         axi[i % 3, i // 3].yaxis.set_label_coords(x=-0.01, y=0.5)
         axi[i % 3, i // 3].xaxis.set_label_coords(x=0.5, y=-0.02)
         axi[i % 3, i // 3].set_title(o, size=8, pad=-14)
 
     axi[1, 0].set_ylabel("UMAP2", size=8)
     axi[2, 1].set_xlabel("UMAP1", size=8)
-    
+
     plt.subplots_adjust(
         left=0.05,
         right=0.95,
         top=0.95,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     cbar = fig.colorbar(im, ax=axi.ravel().tolist(), pad=0.1)
-    cbar.ax.tick_params(labelsize=7) 
+    cbar.ax.tick_params(labelsize=7)
     # for ax in axi:
     #     for a in ax:
-    #         a.axis('off') 
+    #         a.axis('off')
     plt.savefig(f"plots/paper/pima_network/plot_pimaAll_nn_{dataset_i}.pdf")
 
 
 def test_between_all_2():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/emb_6.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="",
+        file="feature_clock_visualization/data/emb_6.csv",
+    )
 
-    fig_size = ((7.125-0.17)/2, ((7.125-0.17)/2.5)/1.618)
+    fig_size = ((7.125 - 0.17) / 2, ((7.125 - 0.17) / 2.5) / 1.618)
 
-    fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=1000, facecolor="w",edgecolor="k",)
-    spec2 = gridspec.GridSpec(ncols=2, nrows=1, figure=fig, 
-                     left=0.04, right=1.04, top=0.565, bottom=0.07)
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=1000,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=2, nrows=1, figure=fig, left=0.04, right=1.04, top=0.565, bottom=0.07
+    )
     ax1 = fig.add_subplot(spec2[0])
 
-    spec23 = gridspec.GridSpecFromSubplotSpec(3, 3, subplot_spec=spec2[1], wspace=0.05, hspace=0.33)
+    spec23 = gridspec.GridSpecFromSubplotSpec(
+        3, 3, subplot_spec=spec2[1], wspace=0.05, hspace=0.33
+    )
     ax2_11 = fig.add_subplot(spec23[0, 0])
     ax2_12 = fig.add_subplot(spec23[0, 1])
     ax2_13 = fig.add_subplot(spec23[0, 2])
     ax2_21 = fig.add_subplot(spec23[1, 0])
     ax2_22 = fig.add_subplot(spec23[1, 1])
     ax2_23 = fig.add_subplot(spec23[1, 2])
     ax2_31 = fig.add_subplot(spec23[2, 0])
     ax2_32 = fig.add_subplot(spec23[2, 1])
     ax2_33 = fig.add_subplot(spec23[2, 2])
 
     plt.tight_layout()
 
-    sc = ax1.scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
+    sc = ax1.scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="Accent",
+        zorder=0,
+        alpha=0.2,
+    )
 
     colors = [
-        'tab:pink', 'tab:green', 'tab:blue', 'tab:olive', 'tab:orange',
-        'tab:purple', 'tab:cyan', 'tab:red', 'tab:brown']
-    
+        "tab:pink",
+        "tab:green",
+        "tab:blue",
+        "tab:olive",
+        "tab:orange",
+        "tab:purple",
+        "tab:cyan",
+        "tab:red",
+        "tab:brown",
+    ]
+
     plot_inst = NonLinearClock(
-        X_new, obs, standard_embedding, labels, method="UMAP", 
-        cluster_labels=clusters, color_scheme=colors)
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters,
+        color_scheme=colors,
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax1,
         scale_circle=3,
         move_circle=[0, 2],
         annotate=2.5,
-        arrow_width=0.1
+        arrow_width=0.1,
     )
 
-    hatches = [plt.plot([],marker="", ls="")[0]]*4 + arrows[0:3] + \
-        [sc.legend_elements()[0][0]] + arrows[3:6] + \
-        [sc.legend_elements()[0][1]] + arrows[6:] + [plt.plot([],marker="", ls="")[0]]*2
-    labels = ["Factors:", " ", " ", "Labels: "] + arrow_labels[0:3] + \
-        ["Healthy"] + arrow_labels[3:6] + \
-        ["Diabetes"] + arrow_labels[6:] + [" ", " "]
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 4
+        + arrows[0:3]
+        + [sc.legend_elements()[0][0]]
+        + arrows[3:6]
+        + [sc.legend_elements()[0][1]]
+        + arrows[6:]
+        + [plt.plot([], marker="", ls="")[0]] * 2
+    )
+    labels = (
+        ["Factors:", " ", " ", "Labels: "]
+        + arrow_labels[0:3]
+        + ["Healthy"]
+        + arrow_labels[3:6]
+        + ["Diabetes"]
+        + arrow_labels[6:]
+        + [" ", " "]
+    )
     leg = ax1.legend(
-        hatches, labels,
+        hatches,
+        labels,
         loc="lower center",
         bbox_to_anchor=(1.02, 1.09),
         fontsize=7,
         ncol=4,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
 
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     ax1.set_yticks([])
     ax1.set_xticks([])
     ax1.set_ylabel("Dim2", size=8)
     ax1.set_xlabel("Dim1", size=8)
     # ax1.set_title("Second hidden layer", size=8)
     ax1.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax1.xaxis.set_label_coords(x=0.5, y=-0.02)
 
-
     # second plot
-    axis_array = [ax2_11, ax2_12, ax2_13, ax2_21, ax2_22, ax2_23, ax2_31, ax2_32, ax2_33]
-
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/emb_6.csv")
-    standard_embedding[:,0], standard_embedding[:,1] = 1 * standard_embedding[:,0], 7 * standard_embedding[:,1]
+    axis_array = [
+        ax2_11,
+        ax2_12,
+        ax2_13,
+        ax2_21,
+        ax2_22,
+        ax2_23,
+        ax2_31,
+        ax2_32,
+        ax2_33,
+    ]
+
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="",
+        drop_labels=False,
+        file="feature_clock_visualization/data/emb_6.csv",
+    )
+    standard_embedding[:, 0], standard_embedding[:, 1] = (
+        1 * standard_embedding[:, 0],
+        7 * standard_embedding[:, 1],
+    )
     for (i, o), axi in zip(enumerate(obs), axis_array):
         im = axi.scatter(
             standard_embedding[:, 0],
             standard_embedding[:, 1],
             marker=".",
             s=1,
             c=X_new[o],
             cmap="jet",
-            alpha=0.7
+            alpha=0.7,
         )
         axi.set_yticks([])
         axi.set_xticks([])
         axi.yaxis.set_label_coords(x=-0.01, y=0.5)
         axi.xaxis.set_label_coords(x=0.5, y=-0.02)
         if o == "SkinThickness":
             o = "SkinThick."
@@ -218,114 +288,179 @@
     ax2_21.set_ylabel("Dim2", size=8)
     ax2_32.set_xlabel("Dim1", size=8)
 
     ax2_21.yaxis.set_label_coords(0, 0.5)
     ax2_32.xaxis.set_label_coords(0.5, -0.07)
 
     cbar = fig.colorbar(im, ax=axis_array, pad=0.02, ticks=[-1, 0, 1], aspect=40)
-    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
     cbar.outline.set_visible(False)
 
     plt.savefig("plots/paper/pima_network/pima_global_autoencoder.pdf")
 
 
-
 def test_between_all_new():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/emb_1_e-5.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="",
+        file="feature_clock_visualization/data/emb_1_e-5.csv",
+    )
 
-    fig_size = ((7.125-0.17)/2, ((7.125-0.17)/2.5)/1.618)
+    fig_size = ((7.125 - 0.17) / 2, ((7.125 - 0.17) / 2.5) / 1.618)
 
-    fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=1000, facecolor="w",edgecolor="k",)
-    spec2 = gridspec.GridSpec(ncols=2, nrows=1, figure=fig, 
-                     left=0.04, right=1.04, top=0.565, bottom=0.07)
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=1000,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=2, nrows=1, figure=fig, left=0.04, right=1.04, top=0.565, bottom=0.07
+    )
     ax1 = fig.add_subplot(spec2[0])
 
-    spec23 = gridspec.GridSpecFromSubplotSpec(3, 3, subplot_spec=spec2[1], wspace=0.05, hspace=0.33)
+    spec23 = gridspec.GridSpecFromSubplotSpec(
+        3, 3, subplot_spec=spec2[1], wspace=0.05, hspace=0.33
+    )
     ax2_11 = fig.add_subplot(spec23[0, 0])
     ax2_12 = fig.add_subplot(spec23[0, 1])
     ax2_13 = fig.add_subplot(spec23[0, 2])
     ax2_21 = fig.add_subplot(spec23[1, 0])
     ax2_22 = fig.add_subplot(spec23[1, 1])
     ax2_23 = fig.add_subplot(spec23[1, 2])
     ax2_31 = fig.add_subplot(spec23[2, 0])
     ax2_32 = fig.add_subplot(spec23[2, 1])
     ax2_33 = fig.add_subplot(spec23[2, 2])
 
     plt.tight_layout()
 
-    sc = ax1.scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
+    sc = ax1.scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="Accent",
+        zorder=0,
+        alpha=0.2,
+    )
 
     colors = [
-        'tab:pink', 'tab:green', 'tab:blue', 'tab:orange',
-        'tab:purple', 'tab:cyan', 'tab:red', 'tab:brown']
-    
+        "tab:pink",
+        "tab:green",
+        "tab:blue",
+        "tab:orange",
+        "tab:purple",
+        "tab:cyan",
+        "tab:red",
+        "tab:brown",
+    ]
+
     plot_inst = NonLinearClock(
-        X_new, obs, standard_embedding, labels, method="UMAP", 
-        cluster_labels=clusters, color_scheme=colors)
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters,
+        color_scheme=colors,
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax1,
         scale_circle=4,
         move_circle=[7, 1],
         annotate=1.8,
-        arrow_width=0.1
+        arrow_width=0.1,
     )
 
-    hatches = [plt.plot([],marker="", ls="")[0]]*4 + arrows[0:3] + \
-        [sc.legend_elements()[0][0]] + arrows[3:6] + \
-        [sc.legend_elements()[0][1]] + arrows[6:] + [plt.plot([],marker="", ls="")[0]]*2
-    labels = ["Factors:", " ", " ", "Labels: "] + arrow_labels[0:3] + \
-        ["Healthy"] + arrow_labels[3:6] + \
-        ["Diabetes"] + arrow_labels[6:] + [" ", " "]
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 4
+        + arrows[0:3]
+        + [sc.legend_elements()[0][0]]
+        + arrows[3:6]
+        + [sc.legend_elements()[0][1]]
+        + arrows[6:]
+        + [plt.plot([], marker="", ls="")[0]] * 2
+    )
+    labels = (
+        ["Factors:", " ", " ", "Labels: "]
+        + arrow_labels[0:3]
+        + ["Healthy"]
+        + arrow_labels[3:6]
+        + ["Diabetes"]
+        + arrow_labels[6:]
+        + [" ", " "]
+    )
     leg = ax1.legend(
-        hatches, labels,
+        hatches,
+        labels,
         loc="lower center",
         bbox_to_anchor=(1.02, 1.09),
         fontsize=7,
         ncol=4,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
 
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     ax1.set_yticks([])
     ax1.set_xticks([])
     ax1.set_ylabel("Dim2", size=8)
     ax1.set_xlabel("Dim1", size=8)
     # ax1.set_title("Second hidden layer", size=8)
     ax1.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax1.xaxis.set_label_coords(x=0.5, y=-0.02)
 
-
     # second plot
-    axis_array = [ax2_11, ax2_12, ax2_13, ax2_21, ax2_22, ax2_23, ax2_31, ax2_32, ax2_33]
-
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/emb_1_e-5.csv")
-    standard_embedding[:,0], standard_embedding[:,1] = 1 * standard_embedding[:,0], 7 * standard_embedding[:,1]
+    axis_array = [
+        ax2_11,
+        ax2_12,
+        ax2_13,
+        ax2_21,
+        ax2_22,
+        ax2_23,
+        ax2_31,
+        ax2_32,
+        ax2_33,
+    ]
+
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="",
+        drop_labels=False,
+        file="feature_clock_visualization/data/emb_1_e-5.csv",
+    )
+    standard_embedding[:, 0], standard_embedding[:, 1] = (
+        1 * standard_embedding[:, 0],
+        7 * standard_embedding[:, 1],
+    )
     for (i, o), axi in zip(enumerate(obs), axis_array):
         if o == "Species":
             break
 
         im = axi.scatter(
             standard_embedding[:, 0],
             standard_embedding[:, 1],
             marker=".",
             s=1,
             c=X_new[o],
             cmap="jet",
-            alpha=0.7
+            alpha=0.7,
         )
         axi.set_yticks([])
         axi.set_xticks([])
         axi.yaxis.set_label_coords(x=-0.01, y=0.5)
         axi.xaxis.set_label_coords(x=0.5, y=-0.02)
         if o == "SkinThickness":
             o = "SkinThick."
@@ -338,14 +473,17 @@
     ax2_21.set_ylabel("Dim2", size=8)
     ax2_32.set_xlabel("Dim1", size=8)
 
     ax2_21.yaxis.set_label_coords(0, 0.5)
     ax2_32.xaxis.set_label_coords(0.5, -0.07)
 
     cbar = fig.colorbar(im, ax=axis_array, pad=0.02, ticks=[-1, 0, 1], aspect=40)
-    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
     cbar.outline.set_visible(False)
 
     plt.savefig("plots/paper/pima_network/pima_global_autoencoder_new.pdf")
 
+
 # test_between_all_2()
 test_between_all_new()
```

### Comparing `feature_clock-0.0.3/test/test_pima_nn.py` & `feature_clock-1.0.0/test/test_pima_nn.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
-def make_legend_arrow(legend, orig_handle,
-                      xdescent, ydescent,
-                      width, height, fontsize):
-    p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
-    return p
-
 
+def make_legend_arrow(legend, orig_handle, xdescent, ydescent, width, height, fontsize):
+    p = mpatches.FancyArrow(
+        0, 0.5 * height, width, 0, length_includes_head=True, head_width=0.75 * height
+    )
+    return p
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
-def setup_pima_data(method="tsne", drop_labels=True, file: str=""):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/diabetes.csv"
+def setup_pima_data(method="tsne", drop_labels=True, file: str = ""):
+    file_name = "feature_clock_visualization/data/diabetes.csv"
     X = read_data(file_name)
     X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     X = X.dropna()
 
     labels = X["Outcome"]
     if drop_labels:
         X.drop(columns=["Outcome"], inplace=True)
@@ -45,23 +44,26 @@
         standard_embedding = reducer.fit_transform(Y)
 
     elif method == "tsne":
         raise NotImplementedError()
 
     elif method == "phate":
         raise NotImplementedError()
-    
+
     # get clusters
     clusters = HDBSCAN(min_samples=12).fit_predict(X)
     # clusters = KMeans(n_clusters=3, n_init="auto", max_iter=1000).fit_predict(X)
 
     return X, obs, standard_embedding, labels, clusters
 
+
 def print_pima_all(file, dataset_i):
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap", drop_labels=False, file=file)
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="umap", drop_labels=False, file=file
+    )
     dpi = 1000
     # fig_size = (2.375, 2.375)
     fig_size = (3.2325, 2.9)
     fig, axi = plt.subplots(
         3,
         3,
         num=None,
@@ -83,69 +85,112 @@
         axi[i % 3, i // 3].set_xticks([])
         axi[i % 3, i // 3].yaxis.set_label_coords(x=-0.01, y=0.5)
         axi[i % 3, i // 3].xaxis.set_label_coords(x=0.5, y=-0.02)
         axi[i % 3, i // 3].set_title(o, size=8, pad=-14)
 
     axi[1, 0].set_ylabel("UMAP2", size=8)
     axi[2, 1].set_xlabel("UMAP1", size=8)
-    
+
     plt.subplots_adjust(
         left=0.05,
         right=0.95,
         top=0.95,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     cbar = fig.colorbar(im, ax=axi.ravel().tolist(), pad=0.1)
-    cbar.ax.tick_params(labelsize=7) 
+    cbar.ax.tick_params(labelsize=7)
     # for ax in axi:
     #     for a in ax:
-    #         a.axis('off') 
+    #         a.axis('off')
     plt.savefig(f"plots/paper/pima_network/plot_pimaAll_nn_{dataset_i}.pdf")
 
 
 def test_between_all_1():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap", file="/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_1.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="umap",
+        file="feature_clock_visualization/data/latent_space_1.csv",
+    )
 
-    fig, ax = plt.subplots(1, figsize=(3.2325, 3.2325)) #(2.375, 2.375)
+    fig, ax = plt.subplots(1, figsize=(3.2325, 3.2325))  # (2.375, 2.375)
     plt.tight_layout()
 
-    sc = ax.scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
+    sc = ax.scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="Accent",
+        zorder=0,
+        alpha=0.3,
+    )
     colors = [
-        'tab:pink', 'tab:green', 'tab:blue', 'tab:olive', 'tab:orange',
-        'tab:purple', 'tab:cyan', 'tab:red', 'tab:brown']
-    
+        "tab:pink",
+        "tab:green",
+        "tab:blue",
+        "tab:olive",
+        "tab:orange",
+        "tab:purple",
+        "tab:cyan",
+        "tab:red",
+        "tab:brown",
+    ]
+
     plot_inst = NonLinearClock(
-        X_new, obs, standard_embedding, labels, 
-        method="UMAP", cluster_labels=clusters, color_scheme=colors)
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters,
+        color_scheme=colors,
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax,
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.6,
         arrow_width=0.1,
     )
 
-    hatches = [plt.plot([],marker="", ls="")[0]]*4 + arrows[0:3] + [sc.legend_elements()[0][0]] + arrows[3:6] + [sc.legend_elements()[0][1]] + arrows[6:] + [plt.plot([],marker="", ls="")[0]]*2
-    labels = ["Factors:", " ", "", "Labels: "] + arrow_labels[0:3] + ["No diabetes"] + arrow_labels[3:6] + ["Diabetes"] + arrow_labels[6:] + [" ", " "]
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 4
+        + arrows[0:3]
+        + [sc.legend_elements()[0][0]]
+        + arrows[3:6]
+        + [sc.legend_elements()[0][1]]
+        + arrows[6:]
+        + [plt.plot([], marker="", ls="")[0]] * 2
+    )
+    labels = (
+        ["Factors:", " ", "", "Labels: "]
+        + arrow_labels[0:3]
+        + ["No diabetes"]
+        + arrow_labels[3:6]
+        + ["Diabetes"]
+        + arrow_labels[6:]
+        + [" ", " "]
+    )
     leg = ax.legend(
         hatches,
         labels,
         loc="lower center",
         bbox_to_anchor=(0.5, 1.09),
         fontsize=7,
         ncol=4,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
 
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     ax.set_yticks([])
@@ -159,54 +204,95 @@
         left=0.05,
         right=0.96,
         top=0.73,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/pima_network/pima_global_nn_1.pdf")
 
+
 def test_between_all_2():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="umap",
+        file="feature_clock_visualization/data/latent_space_2.csv",
+    )
 
-    fig, ax = plt.subplots(1, figsize=(3.2325, 3.2325)) #(2.375, 2.375)
+    fig, ax = plt.subplots(1, figsize=(3.2325, 3.2325))  # (2.375, 2.375)
     plt.tight_layout()
 
-    sc = ax.scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
+    sc = ax.scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="Accent",
+        zorder=0,
+        alpha=0.3,
+    )
 
     colors = [
-        'tab:pink', 'tab:green', 'tab:blue', 'tab:olive', 'tab:orange',
-        'tab:purple', 'tab:cyan', 'tab:red', 'tab:brown']
-    
+        "tab:pink",
+        "tab:green",
+        "tab:blue",
+        "tab:olive",
+        "tab:orange",
+        "tab:purple",
+        "tab:cyan",
+        "tab:red",
+        "tab:brown",
+    ]
+
     plot_inst = NonLinearClock(
-        X_new, obs, standard_embedding, labels, method="UMAP", 
-        cluster_labels=clusters, color_scheme=colors)
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters,
+        color_scheme=colors,
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax,
         scale_circle=3,
         move_circle=[0, 0],
         annotate=0.9,
-        arrow_width=0.1
+        arrow_width=0.1,
     )
 
-    hatches = [plt.plot([],marker="", ls="")[0]]*3 + arrows[0:2] + [sc.legend_elements()[0][0]] + arrows[2:] + [sc.legend_elements()[0][1]]
-    labels = ["Factors:", " ", "Labels: "] + arrow_labels[0:2] + ["No diabetes"] + arrow_labels[2:] + ["Diabetes"]
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 3
+        + arrows[0:2]
+        + [sc.legend_elements()[0][0]]
+        + arrows[2:]
+        + [sc.legend_elements()[0][1]]
+    )
+    labels = (
+        ["Factors:", " ", "Labels: "]
+        + arrow_labels[0:2]
+        + ["No diabetes"]
+        + arrow_labels[2:]
+        + ["Diabetes"]
+    )
     leg = ax.legend(
-        hatches, labels,
+        hatches,
+        labels,
         loc="lower center",
         bbox_to_anchor=(0.5, 1.09),
         fontsize=7,
         ncol=3,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
 
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     ax.set_yticks([])
@@ -221,11 +307,11 @@
         right=0.99,
         top=0.77,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/pima_network/pima_global_nn_2.pdf")
 
 
-# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_1.csv", 1)
+# print_pima_all("feature_clock_visualization/data/latent_space_1.csv", 1)
 test_between_all_1()
-# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2.csv", 2)
-test_between_all_2()
+# print_pima_all("feature_clock_visualization/data/latent_space_2.csv", 2)
+test_between_all_2()
```

### Comparing `feature_clock-0.0.3/test/test_pima_nn_2out.py` & `feature_clock-1.0.0/test/test_pima_nn_2out.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,41 +4,40 @@
 from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
-def make_legend_arrow(legend, orig_handle,
-                      xdescent, ydescent,
-                      width, height, fontsize):
-    p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
-    return p
-
 
+def make_legend_arrow(legend, orig_handle, xdescent, ydescent, width, height, fontsize):
+    p = mpatches.FancyArrow(
+        0, 0.5 * height, width, 0, length_includes_head=True, head_width=0.75 * height
+    )
+    return p
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
-def setup_pima_data(method="tsne", drop_labels=True, file: str=""):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/diabetes.csv"
+def setup_pima_data(method="tsne", drop_labels=True, file: str = ""):
+    file_name = "feature_clock_visualization/data/diabetes.csv"
     X = read_data(file_name)
     X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     X = X.dropna()
 
     labels = X["Outcome"]
     if drop_labels:
         X.drop(columns=["Outcome"], inplace=True)
     obs = list(X.columns)
 
     for col in X.columns:
         X[col] = (X[col] - X[col].mean()) / X[col].std()
-    
+
     file_name2 = file
     Y = read_data(file_name2)
     Y.drop(columns=["target"], inplace=True)
     print(Y.shape)
 
     Y = np.array(Y)
 
@@ -52,38 +51,43 @@
         standard_embedding = reducer.fit_transform(Y)
 
     elif method == "tsne":
         raise NotImplementedError()
 
     elif method == "phate":
         raise NotImplementedError()
-    
+
     # for i in range(standard_embedding.shape[1]):
     #     standard_embedding[:, i] = (standard_embedding[:, i] - standard_embedding[:, i].mean()) / standard_embedding[:, i].std()
-    
+
     # get clusters
     clusters = HDBSCAN(min_samples=12).fit_predict(X)
     # clusters = KMeans(n_clusters=3, n_init="auto", max_iter=1000).fit_predict(X)
 
     return X, obs, standard_embedding, labels, clusters
 
+
 def print_pima_all(file, dataset_i):
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="none", drop_labels=False, file=file)
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="none", drop_labels=False, file=file
+    )
     dpi = 1000
     # fig_size = (2.375, 2.375)
     fig_size = (3.2325, 2.9)
     fig, axi = plt.subplots(
         3,
         3,
         num=None,
         figsize=fig_size,
         dpi=dpi,
         facecolor="w",
         edgecolor="k",
     )
+
+    axs = []
     for i, o in enumerate(obs):
         im = axi[i % 3, i // 3].scatter(
             standard_embedding[:, 0],
             standard_embedding[:, 1],
             marker=".",
             s=1.3,
             c=X_new[o],
@@ -93,124 +97,190 @@
         axi[i % 3, i // 3].set_xticks([])
         axi[i % 3, i // 3].yaxis.set_label_coords(x=-0.01, y=0.5)
         axi[i % 3, i // 3].xaxis.set_label_coords(x=0.5, y=-0.02)
         axi[i % 3, i // 3].set_title(o, size=8, pad=-14)
 
     axi[1, 0].set_ylabel("UMAP2", size=8)
     axi[2, 1].set_xlabel("UMAP1", size=8)
-    
+
     plt.subplots_adjust(
         left=0.05,
         right=0.95,
         top=0.95,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     cbar = fig.colorbar(im, ax=axi.ravel().tolist(), pad=0.1)
-    cbar.ax.tick_params(labelsize=7) 
+    cbar.ax.tick_params(labelsize=7)
     # for ax in axi:
     #     for a in ax:
-    #         a.axis('off') 
+    #         a.axis('off')
     plt.savefig(f"plots/paper/pima_network/plot_pimaAll_nn_{dataset_i}.pdf")
 
 
 def test_between_all_2():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2_2out.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="",
+        file="feature_clock_visualization/data/latent_space_2_2out.csv",
+    )
 
-    fig_size = ((7.125-0.17)/2, ((7.125-0.17)/2.5)/1.618)
+    fig_size = ((7.125 - 0.17) / 2, ((7.125 - 0.17) / 2.5) / 1.618)
 
-    fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=1000, facecolor="w",edgecolor="k",)
-    spec2 = gridspec.GridSpec(ncols=2, nrows=1, figure=fig, 
-                     left=0.04, right=1.04, top=0.565, bottom=0.07)
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=1000,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=2, nrows=1, figure=fig, left=0.04, right=1.04, top=0.565, bottom=0.07
+    )
     ax1 = fig.add_subplot(spec2[0])
 
-    spec23 = gridspec.GridSpecFromSubplotSpec(3, 3, subplot_spec=spec2[1], wspace=0.05, hspace=0.33)
+    spec23 = gridspec.GridSpecFromSubplotSpec(
+        3, 3, subplot_spec=spec2[1], wspace=0.05, hspace=0.33
+    )
     ax2_11 = fig.add_subplot(spec23[0, 0])
     ax2_12 = fig.add_subplot(spec23[0, 1])
     ax2_13 = fig.add_subplot(spec23[0, 2])
     ax2_21 = fig.add_subplot(spec23[1, 0])
     ax2_22 = fig.add_subplot(spec23[1, 1])
     ax2_23 = fig.add_subplot(spec23[1, 2])
     ax2_31 = fig.add_subplot(spec23[2, 0])
     ax2_32 = fig.add_subplot(spec23[2, 1])
     ax2_33 = fig.add_subplot(spec23[2, 2])
 
     plt.tight_layout()
 
-    sc = ax1.scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
+    sc = ax1.scatter(
+        standard_embedding[:, 0],
+        standard_embedding[:, 1],
+        marker=".",
+        c=labels,
+        cmap="Accent",
+        zorder=0,
+        alpha=0.2,
+    )
 
     colors = [
-        'tab:pink', 'tab:green', 'tab:blue', 'tab:olive', 'tab:orange',
-        'tab:purple', 'tab:cyan', 'tab:red', 'tab:brown']
-    
+        "tab:pink",
+        "tab:green",
+        "tab:blue",
+        "tab:olive",
+        "tab:orange",
+        "tab:purple",
+        "tab:cyan",
+        "tab:red",
+        "tab:brown",
+    ]
+
     plot_inst = NonLinearClock(
-        X_new, obs, standard_embedding, labels, method="UMAP", 
-        cluster_labels=clusters, color_scheme=colors)
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=clusters,
+        color_scheme=colors,
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax1,
         scale_circle=2,
         move_circle=[0, 2],
         annotate=2.0,
-        arrow_width=0.15
+        arrow_width=0.15,
     )
 
-    hatches = [plt.plot([],marker="", ls="")[0]]*4 + arrows[0:3] + \
-        [sc.legend_elements()[0][0]] + arrows[3:6] + \
-        [sc.legend_elements()[0][1]] + arrows[6:] + [plt.plot([],marker="", ls="")[0]]*2
-    labels = ["Factors:", " ", " ", "Labels: "] + arrow_labels[0:3] + \
-        ["Healthy"] + arrow_labels[3:6] + \
-        ["Diabetes"] + arrow_labels[6:] + [" ", " "]
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 4
+        + arrows[0:3]
+        + [sc.legend_elements()[0][0]]
+        + arrows[3:6]
+        + [sc.legend_elements()[0][1]]
+        + arrows[6:]
+        + [plt.plot([], marker="", ls="")[0]] * 2
+    )
+    labels = (
+        ["Factors:", " ", " ", "Labels: "]
+        + arrow_labels[0:3]
+        + ["Healthy"]
+        + arrow_labels[3:6]
+        + ["Diabetes"]
+        + arrow_labels[6:]
+        + [" ", " "]
+    )
     leg = ax1.legend(
-        hatches, labels,
+        hatches,
+        labels,
         loc="lower center",
         bbox_to_anchor=(1.02, 1.09),
         fontsize=7,
         ncol=4,
         markerscale=0.6,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
 
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
-    for lh in leg.legendHandles: 
+    for lh in leg.legendHandles:
         lh.set_alpha(1)
 
     ax1.set_yticks([])
     ax1.set_xticks([])
     ax1.set_ylabel("Dim2", size=8)
     ax1.set_xlabel("Dim1", size=8)
     # ax1.set_title("Second hidden layer", size=8)
     ax1.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax1.xaxis.set_label_coords(x=0.5, y=-0.02)
 
-
     # second plot
-    axis_array = [ax2_11, ax2_12, ax2_13, ax2_21, ax2_22, ax2_23, ax2_31, ax2_32, ax2_33]
-
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2_2out.csv")
-    standard_embedding[:,0], standard_embedding[:,1] = 1 * standard_embedding[:,0], 7 * standard_embedding[:,1]
+    axis_array = [
+        ax2_11,
+        ax2_12,
+        ax2_13,
+        ax2_21,
+        ax2_22,
+        ax2_23,
+        ax2_31,
+        ax2_32,
+        ax2_33,
+    ]
+
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(
+        method="",
+        drop_labels=False,
+        file="feature_clock_visualization/data/latent_space_2_2out.csv",
+    )
+    standard_embedding[:, 0], standard_embedding[:, 1] = (
+        1 * standard_embedding[:, 0],
+        1 * standard_embedding[:, 1],
+    )
+    ims = []
     for (i, o), axi in zip(enumerate(obs), axis_array):
         if o == "Species":
             break
 
         im = axi.scatter(
             standard_embedding[:, 0],
             standard_embedding[:, 1],
             marker=".",
             s=1,
             c=X_new[o],
             cmap="jet",
-            alpha=0.7
+            alpha=0.7,
         )
         axi.set_yticks([])
         axi.set_xticks([])
         axi.yaxis.set_label_coords(x=-0.01, y=0.5)
         axi.xaxis.set_label_coords(x=0.5, y=-0.02)
         if o == "SkinThickness":
             o = "SkinThick."
@@ -223,17 +293,17 @@
     ax2_21.set_ylabel("Dim2", size=8)
     ax2_32.set_xlabel("Dim1", size=8)
 
     ax2_21.yaxis.set_label_coords(0, 0.5)
     ax2_32.xaxis.set_label_coords(0.5, -0.07)
 
     cbar = fig.colorbar(im, ax=axis_array, pad=0.02, ticks=[-1, 0, 1], aspect=40)
-    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
     cbar.outline.set_visible(False)
 
-
-
     plt.savefig("plots/paper/pima_network/pima_global_nn_last_2out.pdf")
 
 
-# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2.csv", 2)
+# print_pima_all("feature_clock_visualization/data/latent_space_2.csv", 2)
 test_between_all_2()
```

### Comparing `feature_clock-0.0.3/test/test_support.py` & `feature_clock-1.0.0/test/test_support.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,194 +9,401 @@
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 import matplotlib.colors as mcolors
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 from sklearn import manifold, preprocessing
 
-def make_legend_arrow(legend, orig_handle,
-                      xdescent, ydescent,
-                      width, height, fontsize):
-    p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
-    return p
 
+def make_legend_arrow(
+        legend,
+        orig_handle,
+        xdescent,
+        ydescent,
+        width,
+        height,
+        fontsize):
+    p = mpatches.FancyArrow(
+        0,
+        0.5 *
+        height,
+        width,
+        0,
+        length_includes_head=True,
+        head_width=0.75 *
+        height)
+    return p
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_support_data(method="tsne", drop_labels=True):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/support2.csv"
+    file_name = "feature_clock_visualization/data/support2.csv"
     X = read_data(file_name)
     X.drop(columns=["id"], inplace=True)
 
-    X.drop(columns=["death", "sfdm2", "d.time", "surv2m", "surv6m"], inplace=True)
+    X.drop(
+        columns=[
+            "death",
+            "sfdm2",
+            "d.time",
+            "surv2m",
+            "surv6m"],
+        inplace=True)
 
     for c in X.columns:
-        if c in ['sex', 'dzgroup', 'dzclass', 'income', 'race', 'ca', 'dnr']:
+        if c in ["sex", "dzgroup", "dzclass", "income", "race", "ca", "dnr"]:
             X[c] = X[c].fillna(X[c].mode())
-        elif c == 'sfdm2':
+        elif c == "sfdm2":
             pass
-        else: 
+        else:
             X[c] = X[c].fillna(X[c].mean())
 
-    for c in ['sex', 'dzgroup', 'dzclass', 'income', 'race', 'ca', 'dnr']:
+    for c in ["sex", "dzgroup", "dzclass", "income", "race", "ca", "dnr"]:
         X[c], _ = pd.factorize(X[c])
-    
+
     # X['sfdm2'] = X['sfdm2'].map({"no(M2 and SIP pres)": 0, "adl>=4 (>=5 if sur)": 1, "SIP>=30": 2, "Coma or Intub": 4, "<2 mo. follow-up": 3})
     # X = X[X.sfdm2 != 4]
     X = X.dropna(subset=["hospdead"])
-    
+
     labels = X["hospdead"]
 
     if drop_labels:
         X.drop(columns=["hospdead"], inplace=True)
-    
-    X.rename(columns={
-        'dzclass':'Disease', 
-        'avtisst':'Avg. TISS score', 
-        'aps':'APACHE3 score', 
-        'totcst':'Cost/charges ratio', 
-        'diabetes':'Diabetes', 
-        'dementia':'Dementia', 
-        'adls':'ADL family', 
-        'adlp':'ADL patient', 
-        'bili':'Bilirubin', 
-        'slos':'Days in study', 
-        'prg2m':'2 month survival', 
-        'totmcst': 'Micro cost',
-        'scoma':'Coma score',
-        'sps':'Physiology score',
-        'hday':'Study enter',
-        'dnr':'Rescuscitate order',
-        'charges':'Charges',
-        'age': 'Age'
-    }, inplace=True)
-    
+
+    X.rename(
+        columns={
+            "dzclass": "Disease",
+            "avtisst": "Avg. TISS score",
+            "aps": "APACHE3 score",
+            "totcst": "Cost/charges ratio",
+            "diabetes": "Diabetes",
+            "dementia": "Dementia",
+            "adls": "ADL family",
+            "adlp": "ADL patient",
+            "bili": "Bilirubin",
+            "slos": "Days in study",
+            "prg2m": "2 month survival",
+            "totmcst": "Micro cost",
+            "scoma": "Coma score",
+            "sps": "Physiology score",
+            "hday": "Study enter",
+            "dnr": "Resuscitate order",
+            "charges": "Charges",
+            "age": "Age",
+            "dnrday": "DNR order day",
+        },
+        inplace=True,
+    )
+
     obs = list(X.columns)
 
     # X.drop(columns=["diabetes", "ca", "bun", "glucose", "sex"], inplace=True)
     obs = list(X.columns)
 
     for col in X.columns:
         X[col] = (X[col] - X[col].mean()) / X[col].std()
-    
+        # print([X[col].min(), X[col].max()])
+
     # compute umap
     if method == "umap":
         reducer = umap.UMAP(min_dist=0.2, n_neighbors=30, random_state=42)
         if not drop_labels:
             K = X.drop(columns=["hospdead"], inplace=False)
             standard_embedding = reducer.fit_transform(K)
         else:
             standard_embedding = reducer.fit_transform(X)
 
     elif method == "tsne":
-        tsne = manifold.TSNE(n_components = 2, random_state=42, perplexity=50, learning_rate='auto')
+        tsne = manifold.TSNE(
+            n_components=2,
+            random_state=42,
+            perplexity=50,
+            learning_rate="auto")
         standard_embedding = tsne.fit_transform(X)
 
     elif method == "phate":
         raise NotImplementedError()
-    
+
     standard_embedding = np.array(standard_embedding)
     labels = np.array(labels)
     for i in range(standard_embedding.shape[1]):
-        standard_embedding[:, i] = (standard_embedding[:, i] - standard_embedding[:, i].mean()) / standard_embedding[:, i].std()
-    
+        standard_embedding[:, i] = (
+            standard_embedding[:, i] - standard_embedding[:, i].mean()
+        ) / standard_embedding[:, i].std()
+
     # get clusters
     clusters = HDBSCAN(min_samples=12).fit_predict(X)
     # clusters = KMeans(n_clusters=2, n_init="auto", max_iter=1000, random_state=42).fit_predict(X)
-    
+
     return X, obs, standard_embedding, labels, clusters
 
 
 def test_between_all_3_5():
-    colors = ['aliceblue', 'antiquewhite', 'aqua', 'aquamarine', 'azure', 'beige', 'bisque', 'black', 
-              'blanchedalmond', 'blue', 'blueviolet', 'brown', 'burlywood', 'cadetblue', 'chartreuse', 
-              'chocolate', 'coral', 'cornflowerblue', 'cornsilk', 'crimson', 'cyan', 'darkblue', 
-              'darkcyan', 'darkgoldenrod', 'darkgray', 'darkgreen', 'darkgrey', 'darkkhaki', 
-              'darkmagenta', 'darkolivegreen', 'darkorange', 'darkorchid', 'darkred', 'darksalmon', 
-              'darkseagreen', 'darkslateblue', 'darkslategray', 'darkslategrey', 'darkturquoise', 
-              'darkviolet', 'deeppink', 'deepskyblue', 'dimgray', 'dimgrey', 'dodgerblue', 'firebrick', 
-              'floralwhite', 'forestgreen', 'fuchsia', 'gainsboro', 'ghostwhite', 'gold', 'goldenrod', 'gray', 
-              'green', 'greenyellow', 'grey', 'honeydew', 'hotpink', 'indianred', 'indigo', 'ivory', 
-              'khaki', 'lavender', 'lavenderblush', 'lawngreen', 'lemonchiffon', 'lightblue', 'lightcoral', 
-              'lightcyan', 'lightgoldenrodyellow', 'lightgray', 'lightgreen', 'lightgrey', 'lightpink', 
-              'lightsalmon', 'lightseagreen', 'lightskyblue', 'lightslategray', 'lightslategrey', 
-              'lightsteelblue', 'lightyellow', 'lime', 'limegreen', 'linen', 'magenta', 'maroon', 
-              'mediumaquamarine', 'mediumblue', 'mediumorchid', 'mediumpurple', 'mediumseagreen', 
-              'mediumslateblue', 'mediumspringgreen', 'mediumturquoise', 'mediumvioletred', 'midnightblue', 
-              'mintcream', 'mistyrose', 'moccasin', 'navajowhite', 'navy', 'oldlace', 'olive', 'olivedrab', 
-              'orange', 'orangered', 'orchid', 'palegoldenrod', 'palegreen', 'paleturquoise', 'palevioletred', 
-              'papayawhip', 'peachpuff', 'peru', 'pink', 'plum', 'powderblue', 'purple', 'rebeccapurple', 'red', 
-              'rosybrown', 'royalblue', 'saddlebrown', 'salmon', 'sandybrown', 'seagreen', 'seashell', 'sienna', 
-              'silver', 'skyblue', 'slateblue', 'slategray', 'slategrey', 'snow', 'springgreen', 'steelblue', 
-              'tan', 'teal', 'thistle', 'tomato', 'turquoise', 'violet', 'wheat', 'white', 'whitesmoke', 'yellow', 
-              'yellowgreen']
+    colors = [
+        "aliceblue",
+        "antiquewhite",
+        "aqua",
+        "aquamarine",
+        "azure",
+        "beige",
+        "bisque",
+        "black",
+        "blanchedalmond",
+        "blue",
+        "blueviolet",
+        "brown",
+        "burlywood",
+        "cadetblue",
+        "chartreuse",
+        "chocolate",
+        "coral",
+        "cornflowerblue",
+        "cornsilk",
+        "crimson",
+        "cyan",
+        "darkblue",
+        "darkcyan",
+        "darkgoldenrod",
+        "darkgray",
+        "darkgreen",
+        "darkgrey",
+        "darkkhaki",
+        "darkmagenta",
+        "darkolivegreen",
+        "darkorange",
+        "darkorchid",
+        "darkred",
+        "darksalmon",
+        "darkseagreen",
+        "darkslateblue",
+        "darkslategray",
+        "darkslategrey",
+        "darkturquoise",
+        "darkviolet",
+        "deeppink",
+        "deepskyblue",
+        "dimgray",
+        "dimgrey",
+        "dodgerblue",
+        "firebrick",
+        "floralwhite",
+        "forestgreen",
+        "fuchsia",
+        "gainsboro",
+        "ghostwhite",
+        "gold",
+        "goldenrod",
+        "gray",
+        "green",
+        "greenyellow",
+        "grey",
+        "honeydew",
+        "hotpink",
+        "indianred",
+        "indigo",
+        "ivory",
+        "khaki",
+        "lavender",
+        "lavenderblush",
+        "lawngreen",
+        "lemonchiffon",
+        "lightblue",
+        "lightcoral",
+        "lightcyan",
+        "lightgoldenrodyellow",
+        "lightgray",
+        "lightgreen",
+        "lightgrey",
+        "lightpink",
+        "lightsalmon",
+        "lightseagreen",
+        "lightskyblue",
+        "lightslategray",
+        "lightslategrey",
+        "lightsteelblue",
+        "lightyellow",
+        "lime",
+        "limegreen",
+        "linen",
+        "magenta",
+        "maroon",
+        "mediumaquamarine",
+        "mediumblue",
+        "mediumorchid",
+        "mediumpurple",
+        "mediumseagreen",
+        "mediumslateblue",
+        "mediumspringgreen",
+        "mediumturquoise",
+        "mediumvioletred",
+        "midnightblue",
+        "mintcream",
+        "mistyrose",
+        "moccasin",
+        "navajowhite",
+        "navy",
+        "oldlace",
+        "olive",
+        "olivedrab",
+        "orange",
+        "orangered",
+        "orchid",
+        "palegoldenrod",
+        "palegreen",
+        "paleturquoise",
+        "palevioletred",
+        "papayawhip",
+        "peachpuff",
+        "peru",
+        "pink",
+        "plum",
+        "powderblue",
+        "purple",
+        "rebeccapurple",
+        "red",
+        "rosybrown",
+        "royalblue",
+        "saddlebrown",
+        "salmon",
+        "sandybrown",
+        "seagreen",
+        "seashell",
+        "sienna",
+        "silver",
+        "skyblue",
+        "slateblue",
+        "slategray",
+        "slategrey",
+        "snow",
+        "springgreen",
+        "steelblue",
+        "tan",
+        "teal",
+        "thistle",
+        "tomato",
+        "turquoise",
+        "violet",
+        "wheat",
+        "white",
+        "whitesmoke",
+        "yellow",
+        "yellowgreen",
+    ]
     # tab20 = [
-    #     '#1f77b4', '#aec7e8', 
-    #     '#ff7f0e', '#ffbb78', 
-    #     '#2ca02c', '#98df8a', 
-    #     '#d62728', '#ff9896', 
-    #     '#9467bd', '#c5b0d5', 
-    #     '#8c564b', '#c49c94', 
-    #     '#e377c2', '#f7b6d2', 
-    #     '#7f7f7f', '#c7c7c7', 
-    #     '#bcbd22', '#dbdb8d', 
+    #     '#1f77b4', '#aec7e8',
+    #     '#ff7f0e', '#ffbb78',
+    #     '#2ca02c', '#98df8a',
+    #     '#d62728', '#ff9896',
+    #     '#9467bd', '#c5b0d5',
+    #     '#8c564b', '#c49c94',
+    #     '#e377c2', '#f7b6d2',
+    #     '#7f7f7f', '#c7c7c7',
+    #     '#bcbd22', '#dbdb8d',
     #     '#17becf', '#9edae5']
 
     tab20 = [
-        '#1f77b4', 
-        '#ff7f0e', 
-        '#d62728', '#ff9896', 
-        '#9467bd', 'navy', 
-        '#8c564b', 'dimgray', 
-        '#e377c2', 'darkolivegreen', 
-        '#bcbd22', 
-        '#17becf', "chartreuse"]
+        "#1f77b4",
+        "#ff7f0e",
+        "#d62728",
+        "#ff9896",
+        "#9467bd",
+        "navy",
+        "#8c564b",
+        "dimgray",
+        "#e377c2",
+        "darkolivegreen",
+        "#bcbd22",
+        "#17becf",
+        "chartreuse",
+    ]
 
-    
-    X_new, obs, standard_embedding, labels, clusters = setup_support_data(method="tsne")
+    X_new, obs, standard_embedding, labels, clusters = setup_support_data(
+        method="tsne")
 
     i = 0
-    for k in range(len(obs)): 
-        if obs[k] in ['surv2m', 'surv6m', 'avtisst', 'dzclass', 'aps', 'death', 'sps', 'dnr', 'adlsc', 'prg6m', 'prg2m', 'd.time', 'num.co']:
+    for k in range(len(obs)):
+        if obs[k] in [
+            "surv2m",
+            "surv6m",
+            "avtisst",
+            "dzclass",
+            "aps",
+            "death",
+            "sps",
+            "dnr",
+            "adlsc",
+            "prg6m",
+            "prg2m",
+            "d.time",
+            "num.co",
+        ]:
             colors[k] = tab20[i]
-            if  obs[k] == "surv6m":
+            if obs[k] == "surv6m":
                 colors[k] = "darkred"
-            if  obs[k] == "num.co":
+            if obs[k] == "num.co":
                 colors[k] = "orangered"
             if obs[k] == "adlsc":
                 colors[k] = "peru"
             i += 1
-    
-    fig, axi = plt.subplots(1, 3, figsize=((7.125-0.17), ((7.125-0.17)/1.8)/1.618))
+
+    fig, axi = plt.subplots(
+        1, 3, figsize=((7.125 - 0.17), ((7.125 - 0.17) / 1.8) / 1.618)
+    )
     plt.tight_layout()
 
     scs = []
     # for val, i in zip([0, 1, 2, 3], [0, 5, 2, 1]):
     for val, i in zip([0, 3, 1, 2], [0, 2, 5, 1]):
-        sc = axi[0].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', color=matplotlib.colormaps["Accent"].colors[i], alpha=0.3)
+        sc = axi[0].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Accent"].colors[i],
+            alpha=0.3,
+        )
         scs.append(sc)
-        axi[1].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', color=matplotlib.colormaps["Accent"].colors[i], alpha=0.3)
-        axi[2].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', color=matplotlib.colormaps["Accent"].colors[i], alpha=0.3)
+        axi[1].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Accent"].colors[i],
+            alpha=0.3,
+        )
+        axi[2].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Accent"].colors[i],
+            alpha=0.3,
+        )
 
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=labels, color_scheme=colors)
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=labels,
+        color_scheme=colors,
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=False,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=axi[0],
         scale_circle=3,
         move_circle=[0, 0],
         annotate=0.8,
         arrow_width=0.1,
         plot_scatter=False,
-        plot_top_k=5
+        plot_top_k=5,
     )
 
     axi[0].set_yticks([])
     axi[0].set_xticks([])
     axi[0].set_ylabel("t-SNE2", size=8)
     axi[0].set_xlabel("t-SNE1", size=8)
     axi[0].set_title("Global clock", size=8)
@@ -219,216 +426,418 @@
         scale_circles=[2.2, 2, 2.5, 0.2],
         # move_circles=[[-1.5, 0.3], [0, 1.5], [2.3, -1], [-0.8, -0.2]],
         move_circles=[[-1.8, 0.3], [-0.8, 0], [2.5, -0.8], [-0.0, 0]],
         annotates=[0.4, 0.4, 0.4, 0.4],
         arrow_width=0.08,
         plot_top_k=5,
         plot_hulls=False,
-        plot_scatter=False
+        plot_scatter=False,
     )
 
     # sc2 = axi[1].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
 
     axi[1].set_yticks([])
     axi[1].set_xticks([])
     axi[1].set_ylabel("t-SNE2", size=8)
     axi[1].set_xlabel("t-SNE1", size=8)
     axi[1].set_title("Local clock", size=8)
     axi[1].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[1].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     # Between
     # sc3 = axi[2].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
-    
+
     arrows2, arrow_labels2 = plot_inst.plot_between_clock(
         standartize_data=True,
         standartize_coef=False,
         univar_importance=False,
         ax=axi[2],
         scale_circles=[6, 10, 0],
         # move_circles=[[1.8, 1.1], [0.1, -0.8], [0.0, 0.0]],
         move_circles=[[0.7, -1.5], [0.4, 1.3], [0, 0]],
         annotates=[0.5, 0.5, 0.5],
         arrow_width=0.08,
         plot_top_k=5,
         plot_scatter=False,
-        plot_hulls=False
+        plot_hulls=False,
     )
 
     arrows_dict = {}
     for i, val in enumerate(arrow_labels):
         arrows_dict[val] = arrows[i]
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
     for i, val in enumerate(arrow_labels2):
         arrows_dict[val] = arrows2[i]
 
     print(len(list(arrows_dict.keys())))
-    
-    hatches = [plt.plot([],marker="", ls="")[0]]*3 + \
-        list(arrows_dict.values())[0:2]   + [scs[0]] + \
-        list(arrows_dict.values())[2:4]   + [scs[3]] + \
-        list(arrows_dict.values())[4:6]   + [scs[1]] + \
-        list(arrows_dict.values())[6:8]   + [scs[2]] + \
-        list(arrows_dict.values())[8:10]  + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[10:12] + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[12:14] + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[14:]   + [plt.plot([],marker="", ls="")[0]]
-    
-    labels = ["Factors:", " ", "Labels (Disability):"] + \
-        list(arrows_dict.keys())[0:2]   + ["Level 1"] + \
-        list(arrows_dict.keys())[2:4]   + ["Level 2"] + \
-        list(arrows_dict.keys())[4:6]   + ["Level 3"] + \
-        list(arrows_dict.keys())[6:8]   + ["Level 4"] + \
-        list(arrows_dict.keys())[8:10]  + [" "] + \
-        list(arrows_dict.keys())[10:12] + [" "] + \
-        list(arrows_dict.keys())[12:14] + [" "] + \
-        list(arrows_dict.keys())[14:]   + [" "]
 
-    
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 3
+        + list(arrows_dict.values())[0:2]
+        + [scs[0]]
+        + list(arrows_dict.values())[2:4]
+        + [scs[3]]
+        + list(arrows_dict.values())[4:6]
+        + [scs[1]]
+        + list(arrows_dict.values())[6:8]
+        + [scs[2]]
+        + list(arrows_dict.values())[8:10]
+        + [plt.plot([], marker="", ls="")[0]]
+        + list(arrows_dict.values())[10:12]
+        + [plt.plot([], marker="", ls="")[0]]
+        + list(arrows_dict.values())[12:14]
+        + [plt.plot([], marker="", ls="")[0]]
+        + list(arrows_dict.values())[14:]
+        + [plt.plot([], marker="", ls="")[0]]
+    )
+
+    labels = (
+        ["Factors:", " ", "Labels (Disability):"]
+        + list(arrows_dict.keys())[0:2]
+        + ["Level 1"]
+        + list(arrows_dict.keys())[2:4]
+        + ["Level 2"]
+        + list(arrows_dict.keys())[4:6]
+        + ["Level 3"]
+        + list(arrows_dict.keys())[6:8]
+        + ["Level 4"]
+        + list(arrows_dict.keys())[8:10]
+        + [" "]
+        + list(arrows_dict.keys())[10:12]
+        + [" "]
+        + list(arrows_dict.keys())[12:14]
+        + [" "]
+        + list(arrows_dict.keys())[14:]
+        + [" "]
+    )
+
     leg = axi[2].legend(
         hatches,
         labels,
         loc="lower center",
         bbox_to_anchor=(-0.84, 1.12),
         fontsize=7,
         ncol=9,
         markerscale=1,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     axi[2].set_yticks([])
     axi[2].set_xticks([])
     axi[2].set_ylabel("t-SNE2", size=8)
     axi[2].set_xlabel("t-SNE1", size=8)
-    axi[2].set_title("Inter-cluster clock", size=8)
+    axi[2].set_title("Inter-group clock", size=8)
     axi[2].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[2].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     plt.subplots_adjust(
         left=0.02,
         right=0.99,
         top=0.7,
         bottom=0.06,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/support/support_3.pdf")
 
 
 def test_between_all_3():
-    colors = ['aliceblue', 'antiquewhite', 'aqua', 'aquamarine', 'azure', 'beige', 'bisque', 'black', 
-              'blanchedalmond', 'blue', 'blueviolet', 'brown', 'burlywood', 'cadetblue', 'chartreuse', 
-              'chocolate', 'coral', 'cornflowerblue', 'cornsilk', 'crimson', 'cyan', 'darkblue', 
-              'darkcyan', 'darkgoldenrod', 'darkgray', 'darkgreen', 'darkgrey', 'darkkhaki', 
-              'darkmagenta', 'darkolivegreen', 'darkorange', 'darkorchid', 'darkred', 'darksalmon', 
-              'darkseagreen', 'darkslateblue', 'darkslategray', 'darkslategrey', 'darkturquoise', 
-              'darkviolet', 'deeppink', 'deepskyblue', 'dimgray', 'dimgrey', 'dodgerblue', 'firebrick', 
-              'floralwhite', 'forestgreen', 'fuchsia', 'gainsboro', 'ghostwhite', 'gold', 'goldenrod', 'gray', 
-              'green', 'greenyellow', 'grey', 'honeydew', 'hotpink', 'indianred', 'indigo', 'ivory', 
-              'khaki', 'lavender', 'lavenderblush', 'lawngreen', 'lemonchiffon', 'lightblue', 'lightcoral', 
-              'lightcyan', 'lightgoldenrodyellow', 'lightgray', 'lightgreen', 'lightgrey', 'lightpink', 
-              'lightsalmon', 'lightseagreen', 'lightskyblue', 'lightslategray', 'lightslategrey', 
-              'lightsteelblue', 'lightyellow', 'lime', 'limegreen', 'linen', 'magenta', 'maroon', 
-              'mediumaquamarine', 'mediumblue', 'mediumorchid', 'mediumpurple', 'mediumseagreen', 
-              'mediumslateblue', 'mediumspringgreen', 'mediumturquoise', 'mediumvioletred', 'midnightblue', 
-              'mintcream', 'mistyrose', 'moccasin', 'navajowhite', 'navy', 'oldlace', 'olive', 'olivedrab', 
-              'orange', 'orangered', 'orchid', 'palegoldenrod', 'palegreen', 'paleturquoise', 'palevioletred', 
-              'papayawhip', 'peachpuff', 'peru', 'pink', 'plum', 'powderblue', 'purple', 'rebeccapurple', 'red', 
-              'rosybrown', 'royalblue', 'saddlebrown', 'salmon', 'sandybrown', 'seagreen', 'seashell', 'sienna', 
-              'silver', 'skyblue', 'slateblue', 'slategray', 'slategrey', 'snow', 'springgreen', 'steelblue', 
-              'tan', 'teal', 'thistle', 'tomato', 'turquoise', 'violet', 'wheat', 'white', 'whitesmoke', 'yellow', 
-              'yellowgreen']
+    colors = [
+        "aliceblue",
+        "antiquewhite",
+        "aqua",
+        "aquamarine",
+        "azure",
+        "beige",
+        "bisque",
+        "black",
+        "blanchedalmond",
+        "blue",
+        "blueviolet",
+        "brown",
+        "burlywood",
+        "cadetblue",
+        "chartreuse",
+        "chocolate",
+        "coral",
+        "cornflowerblue",
+        "cornsilk",
+        "crimson",
+        "cyan",
+        "darkblue",
+        "darkcyan",
+        "darkgoldenrod",
+        "darkgray",
+        "darkgreen",
+        "darkgrey",
+        "darkkhaki",
+        "darkmagenta",
+        "darkolivegreen",
+        "darkorange",
+        "darkorchid",
+        "darkred",
+        "darksalmon",
+        "darkseagreen",
+        "darkslateblue",
+        "darkslategray",
+        "darkslategrey",
+        "darkturquoise",
+        "darkviolet",
+        "deeppink",
+        "deepskyblue",
+        "dimgray",
+        "dimgrey",
+        "dodgerblue",
+        "firebrick",
+        "floralwhite",
+        "forestgreen",
+        "fuchsia",
+        "gainsboro",
+        "ghostwhite",
+        "gold",
+        "goldenrod",
+        "gray",
+        "green",
+        "greenyellow",
+        "grey",
+        "honeydew",
+        "hotpink",
+        "indianred",
+        "indigo",
+        "ivory",
+        "khaki",
+        "lavender",
+        "lavenderblush",
+        "lawngreen",
+        "lemonchiffon",
+        "lightblue",
+        "lightcoral",
+        "lightcyan",
+        "lightgoldenrodyellow",
+        "lightgray",
+        "lightgreen",
+        "lightgrey",
+        "lightpink",
+        "lightsalmon",
+        "lightseagreen",
+        "lightskyblue",
+        "lightslategray",
+        "lightslategrey",
+        "lightsteelblue",
+        "lightyellow",
+        "lime",
+        "limegreen",
+        "linen",
+        "magenta",
+        "maroon",
+        "mediumaquamarine",
+        "mediumblue",
+        "mediumorchid",
+        "mediumpurple",
+        "mediumseagreen",
+        "mediumslateblue",
+        "mediumspringgreen",
+        "mediumturquoise",
+        "mediumvioletred",
+        "midnightblue",
+        "mintcream",
+        "mistyrose",
+        "moccasin",
+        "navajowhite",
+        "navy",
+        "oldlace",
+        "olive",
+        "olivedrab",
+        "orange",
+        "orangered",
+        "orchid",
+        "palegoldenrod",
+        "palegreen",
+        "paleturquoise",
+        "palevioletred",
+        "papayawhip",
+        "peachpuff",
+        "peru",
+        "pink",
+        "plum",
+        "powderblue",
+        "purple",
+        "rebeccapurple",
+        "red",
+        "rosybrown",
+        "royalblue",
+        "saddlebrown",
+        "salmon",
+        "sandybrown",
+        "seagreen",
+        "seashell",
+        "sienna",
+        "silver",
+        "skyblue",
+        "slateblue",
+        "slategray",
+        "slategrey",
+        "snow",
+        "springgreen",
+        "steelblue",
+        "tan",
+        "teal",
+        "thistle",
+        "tomato",
+        "turquoise",
+        "violet",
+        "wheat",
+        "white",
+        "whitesmoke",
+        "yellow",
+        "yellowgreen",
+    ]
     # tab20 = [
-    #     '#1f77b4', '#aec7e8', 
-    #     '#ff7f0e', '#ffbb78', 
-    #     '#2ca02c', '#98df8a', 
-    #     '#d62728', '#ff9896', 
-    #     '#9467bd', '#c5b0d5', 
-    #     '#8c564b', '#c49c94', 
-    #     '#e377c2', '#f7b6d2', 
-    #     '#7f7f7f', '#c7c7c7', 
-    #     '#bcbd22', '#dbdb8d', 
+    #     '#1f77b4', '#aec7e8',
+    #     '#ff7f0e', '#ffbb78',
+    #     '#2ca02c', '#98df8a',
+    #     '#d62728', '#ff9896',
+    #     '#9467bd', '#c5b0d5',
+    #     '#8c564b', '#c49c94',
+    #     '#e377c2', '#f7b6d2',
+    #     '#7f7f7f', '#c7c7c7',
+    #     '#bcbd22', '#dbdb8d',
     #     '#17becf', '#9edae5']
 
     tab20 = [
-        '#1f77b4', 
-        '#bcbd22',  
-        '#9467bd',
-        '#8c564b', 
-        '#e377c2', 'orangered', 
-        '#d62728', "darkolivegreen",
-        '#17becf', "navy"]
+        "#1f77b4",
+        "#bcbd22",
+        "#9467bd",
+        "#8c564b",
+        "#e377c2",
+        "orangered",
+        "#d62728",
+        "darkolivegreen",
+        "#17becf",
+        "navy",
+    ]
 
-    
-    X_new, obs, standard_embedding, labels, clusters = setup_support_data(method="tsne")
+    X_new, obs, standard_embedding, labels, clusters = setup_support_data(
+        method="tsne")
 
     i = 0
-    for k in range(len(obs)): 
-        if obs[k] in ['Disease', 'Avg. TISS score', 
-                      'APACHE3 score', 'Cost/charges ratio', 
-                      'Diabetes', 'Dementia', 
-                      'ADL family', 'ADL patient', 
-                      'Bilirubin', 'Coma score', 
-                      'Physiology score', '2 month survival', 
-                      'Study enter', 'Micro cost']:
-            
-            if obs[k] == 'APACHE3 score':
+    for k in range(len(obs)):
+        if obs[k] in [
+            "Disease",
+            "Avg. TISS score",
+            "APACHE3 score",
+            "Cost/charges ratio",
+            "Diabetes",
+            "Dementia",
+            "ADL family",
+            "ADL patient",
+            "Bilirubin",
+            "Coma score",
+            "Physiology score",
+            "2 month survival",
+            "Study enter",
+            "Micro cost",
+        ]:
+
+            if obs[k] == "APACHE3 score":
                 colors[k] = "purple"
-            elif obs[k] == 'Study enter':
+            elif obs[k] == "Study enter":
                 colors[k] = "peru"
-            elif obs[k] == 'Physiology score':
+            elif obs[k] == "Physiology score":
                 colors[k] = "dimgray"
-            elif obs[k] == 'Cost/charges ratio':
+            elif obs[k] == "Cost/charges ratio":
                 colors[k] = "#ff7f0e"
             else:
                 colors[k] = tab20[i]
                 i += 1
 
-    fig = plt.figure(constrained_layout=True, figsize=((7.125-0.17), ((7.125-0.17)/1.65)/1.618), dpi=1000, facecolor="w",edgecolor="k",)
-    spec2 = gridspec.GridSpec(ncols=4, nrows=1, figure=fig, 
-                     left=0.02, right=0.99, top=0.67, bottom=0.06)
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=((7.125 - 0.17), ((7.125 - 0.17) / 1.65) / 1.618),
+        dpi=1000,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=4,
+        nrows=1,
+        figure=fig,
+        left=0.02,
+        right=0.99,
+        top=0.67,
+        bottom=0.06)
     ax1 = fig.add_subplot(spec2[0])
     ax3 = fig.add_subplot(spec2[2])
     ax4 = fig.add_subplot(spec2[3])
     axi = [ax1, ax3, ax4]
 
-    spec23 = gridspec.GridSpecFromSubplotSpec(2, 2, subplot_spec=spec2[1], hspace=0.18, wspace=0.05)# wspace=-0.5, hspace=-0.9)
+    spec23 = gridspec.GridSpecFromSubplotSpec(
+        2, 2, subplot_spec=spec2[1], hspace=0.18, wspace=0.05
+    )  # wspace=-0.5, hspace=-0.9)
     ax21 = fig.add_subplot(spec23[0, 0])
     ax22 = fig.add_subplot(spec23[0, 1])
     ax23 = fig.add_subplot(spec23[1, 0])
     ax24 = fig.add_subplot(spec23[1, 1])
 
     scs = []
-    for val, i in zip([0, 1], [2, 4]):
-        sc = axi[0].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', 
-                            color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=15)
+    for val, i in zip([0, 1], [2, 8]):
+        sc = axi[0].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Paired"].colors[i],
+            alpha=0.2,
+            s=15,
+        )
         scs.append(sc)
-        axi[1].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', 
-                       color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=15)
-        axi[2].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', 
-                       color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=15)
+        axi[1].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Paired"].colors[i],
+            alpha=0.2,
+            s=15,
+        )
+        axi[2].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Paired"].colors[i],
+            alpha=0.2,
+            s=15,
+        )
 
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=labels, color_scheme=colors)
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=labels,
+        color_scheme=colors,
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=False,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=axi[0],
         scale_circle=2,
         move_circle=[0, 0],
         annotate=0.8,
         arrow_width=0.1,
         plot_scatter=False,
-        plot_top_k=4
+        plot_top_k=4,
     )
 
     axi[0].set_yticks([])
     axi[0].set_xticks([])
     axi[0].set_ylabel("t-SNE2", size=8)
     axi[0].set_xlabel("t-SNE1", size=8)
     axi[0].set_title("Global clock", size=8)
@@ -441,20 +850,20 @@
         standartize_coef=False,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=axi[1],
         scale_circles=[1.5, 1.5],
         move_circles=[[-0.3, 0.5], [0.0, -0.5]],
         clocks_labels=["Survival", "Death"],
-        clocks_labels_angles = [45, 90],
+        clocks_labels_angles=[45, 90],
         annotates=[0.3, 0.3],
         arrow_width=0.08,
         plot_top_k=4,
         plot_hulls=False,
-        plot_scatter=False
+        plot_scatter=False,
     )
 
     axi[1].set_yticks([])
     axi[1].set_xticks([])
     axi[1].set_ylabel("t-SNE2", size=8)
     axi[1].set_xlabel("t-SNE1", size=8)
     axi[1].set_title("Local clock", size=8)
@@ -467,192 +876,404 @@
         standartize_coef=False,
         univar_importance=False,
         ax=axi[2],
         scale_circles=[2],
         move_circles=[[0, 0]],
         annotates=[0.5],
         clocks_labels=["Survival", "Death"],
-        clocks_labels_angles = [270],
+        clocks_labels_angles=[90],
         arrow_width=0.08,
         plot_top_k=4,
         plot_scatter=False,
-        plot_hulls=False
+        plot_hulls=False,
     )
 
     arrows_dict = {}
     for i, val in enumerate(arrow_labels):
         arrows_dict[val] = arrows[i]
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
     for i, val in enumerate(arrow_labels2):
         arrows_dict[val] = arrows2[i]
 
     print(len(list(arrows_dict.keys())))
     print((list(arrows_dict.keys())))
-    
-    hatches = [plt.plot([],marker="", ls="")[0]]*4 + \
-        list(arrows_dict.values())[0:3]  + [scs[0]] + \
-        list(arrows_dict.values())[3:6]  + [scs[1]] + \
-        list(arrows_dict.values())[6:9]  + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[9:12] + [plt.plot([],marker="", ls="")[0]]
-    labels = ["Factors:", " ", " ", "Labels (Death in hospital):"] + \
-        list(arrows_dict.keys())[0:3]  + ["Survival"] + \
-        list(arrows_dict.keys())[3:6]  + ["Death"] + \
-        list(arrows_dict.keys())[6:9]  + [""] + \
-        list(arrows_dict.keys())[9:12] + [""]
+
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 4
+        + list(arrows_dict.values())[0:3]
+        + [scs[0]]
+        + list(arrows_dict.values())[3:6]
+        + [scs[1]]
+        + list(arrows_dict.values())[6:9]
+        + [plt.plot([], marker="", ls="")[0]]
+        + list(arrows_dict.values())[9:12]
+        + [plt.plot([], marker="", ls="")[0]]
+    )
+    labels = (
+        ["Factors:", " ", " ", "Labels (Death in hospital):"]
+        + list(arrows_dict.keys())[0:3]
+        + ["Survival"]
+        + list(arrows_dict.keys())[3:6]
+        + ["Death"]
+        + list(arrows_dict.keys())[6:9]
+        + [""]
+        + list(arrows_dict.keys())[9:12]
+        + [""]
+    )
     leg = axi[2].legend(
         hatches,
         labels,
         loc="lower center",
         bbox_to_anchor=(-1.29, 1.12),
         fontsize=7,
         ncol=5,
         markerscale=1,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
-    for lh in leg.legendHandles: 
+    for lh in leg.legendHandles:
         lh.set_alpha(1)
 
     axi[2].set_yticks([])
     axi[2].set_xticks([])
     axi[2].set_ylabel("t-SNE2", size=8)
     axi[2].set_xlabel("t-SNE1", size=8)
-    axi[2].set_title("Inter-cluster clock", size=8)
+    axi[2].set_title("Inter-group clock", size=8)
     axi[2].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[2].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     # fourth plot
-    X_new, obs, standard_embedding, labels, clusters = setup_support_data(method="tsne", drop_labels=True)
+    X_new, obs, standard_embedding, labels, clusters = setup_support_data(
+        method="tsne", drop_labels=True
+    )
+
+    standard_embedding[:, 0], standard_embedding[:, 1] = (
+        5 * standard_embedding[:, 0],
+        1 * standard_embedding[:, 1],
+    )
+    for (
+        i, o), axi_i in zip(
+        enumerate(arrow_labels), [
+            ax21, ax22, ax23, ax24]):
+        if i == 0:
+            im = axi_i.scatter(
+                standard_embedding[:, 0],
+                standard_embedding[:, 1],
+                marker=".",
+                s=1,
+                c=X_new[o],
+                cmap=cm.coolwarm,
+                alpha=0.8,
+            )
+        else:
+            axi_i.scatter(
+                standard_embedding[:, 0],
+                standard_embedding[:, 1],
+                marker=".",
+                s=1,
+                c=X_new[o],
+                cmap=cm.coolwarm,
+                alpha=0.8,
+            )
 
-    standard_embedding[:,0], standard_embedding[:,1] = 5 * standard_embedding[:,0], 1 * standard_embedding[:,1]
-    for (i, o), axi_i in zip(enumerate(arrow_labels), [ax21, ax22, ax23, ax24]):
-        im = axi_i.scatter(
-            standard_embedding[:, 0],
-            standard_embedding[:, 1],
-            marker=".",
-            s=1,
-            c=X_new[o],
-            cmap=cm.coolwarm,
-            alpha=0.8
-        )
         axi_i.set_yticks([])
         axi_i.set_xticks([])
 
         names = {
-            'Disease':'Disease', 
-            'Avg. TISS score':'Avg. TISS', 
-            'APACHE3 score':'APACHE3', 
-            'Cost/charges ratio':'Cost/charges'
+            "Disease": "Disease",
+            "Avg. TISS score": "Avg. TISS",
+            "APACHE3 score": "APACHE3",
+            "Cost/charges ratio": "Cost/charges",
         }
 
         axi_i.set_title(names[o], size=7, pad=-14)
 
     ax21.set_ylabel("t-SNE2", size=8)
     ax23.set_xlabel("t-SNE1", size=8)
 
     ax21.yaxis.set_label_coords(0, -0.1)
     ax23.xaxis.set_label_coords(1.1, -0.04)
 
     cbar = fig.colorbar(im, ax=[ax21, ax22, ax23, ax24], pad=0.03, aspect=40)
-    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
     cbar.outline.set_visible(False)
 
     plt.savefig("plots/paper/support/support_3.pdf")
 
 
 def test_between_all_3_5():
-    colors = ['aliceblue', 'antiquewhite', 'aqua', 'aquamarine', 'azure', 'beige', 'bisque', 'black', 
-              'blanchedalmond', 'blue', 'blueviolet', 'brown', 'burlywood', 'cadetblue', 'chartreuse', 
-              'chocolate', 'coral', 'cornflowerblue', 'cornsilk', 'crimson', 'cyan', 'darkblue', 
-              'darkcyan', 'darkgoldenrod', 'darkgray', 'darkgreen', 'darkgrey', 'darkkhaki', 
-              'darkmagenta', 'darkolivegreen', 'darkorange', 'darkorchid', 'darkred', 'darksalmon', 
-              'darkseagreen', 'darkslateblue', 'darkslategray', 'darkslategrey', 'darkturquoise', 
-              'darkviolet', 'deeppink', 'deepskyblue', 'dimgray', 'dimgrey', 'dodgerblue', 'firebrick', 
-              'floralwhite', 'forestgreen', 'fuchsia', 'gainsboro', 'ghostwhite', 'gold', 'goldenrod', 'gray', 
-              'green', 'greenyellow', 'grey', 'honeydew', 'hotpink', 'indianred', 'indigo', 'ivory', 
-              'khaki', 'lavender', 'lavenderblush', 'lawngreen', 'lemonchiffon', 'lightblue', 'lightcoral', 
-              'lightcyan', 'lightgoldenrodyellow', 'lightgray', 'lightgreen', 'lightgrey', 'lightpink', 
-              'lightsalmon', 'lightseagreen', 'lightskyblue', 'lightslategray', 'lightslategrey', 
-              'lightsteelblue', 'lightyellow', 'lime', 'limegreen', 'linen', 'magenta', 'maroon', 
-              'mediumaquamarine', 'mediumblue', 'mediumorchid', 'mediumpurple', 'mediumseagreen', 
-              'mediumslateblue', 'mediumspringgreen', 'mediumturquoise', 'mediumvioletred', 'midnightblue', 
-              'mintcream', 'mistyrose', 'moccasin', 'navajowhite', 'navy', 'oldlace', 'olive', 'olivedrab', 
-              'orange', 'orangered', 'orchid', 'palegoldenrod', 'palegreen', 'paleturquoise', 'palevioletred', 
-              'papayawhip', 'peachpuff', 'peru', 'pink', 'plum', 'powderblue', 'purple', 'rebeccapurple', 'red', 
-              'rosybrown', 'royalblue', 'saddlebrown', 'salmon', 'sandybrown', 'seagreen', 'seashell', 'sienna', 
-              'silver', 'skyblue', 'slateblue', 'slategray', 'slategrey', 'snow', 'springgreen', 'steelblue', 
-              'tan', 'teal', 'thistle', 'tomato', 'turquoise', 'violet', 'wheat', 'white', 'whitesmoke', 'yellow', 
-              'yellowgreen']
+    colors = [
+        "aliceblue",
+        "antiquewhite",
+        "aqua",
+        "aquamarine",
+        "azure",
+        "beige",
+        "bisque",
+        "black",
+        "blanchedalmond",
+        "blue",
+        "blueviolet",
+        "brown",
+        "burlywood",
+        "cadetblue",
+        "chartreuse",
+        "chocolate",
+        "coral",
+        "cornflowerblue",
+        "cornsilk",
+        "crimson",
+        "cyan",
+        "darkblue",
+        "darkcyan",
+        "darkgoldenrod",
+        "darkgray",
+        "darkgreen",
+        "darkgrey",
+        "darkkhaki",
+        "darkmagenta",
+        "darkolivegreen",
+        "darkorange",
+        "darkorchid",
+        "darkred",
+        "darksalmon",
+        "darkseagreen",
+        "darkslateblue",
+        "darkslategray",
+        "darkslategrey",
+        "darkturquoise",
+        "darkviolet",
+        "deeppink",
+        "deepskyblue",
+        "dimgray",
+        "dimgrey",
+        "dodgerblue",
+        "firebrick",
+        "floralwhite",
+        "forestgreen",
+        "fuchsia",
+        "gainsboro",
+        "ghostwhite",
+        "gold",
+        "goldenrod",
+        "gray",
+        "green",
+        "greenyellow",
+        "grey",
+        "honeydew",
+        "hotpink",
+        "indianred",
+        "indigo",
+        "ivory",
+        "khaki",
+        "lavender",
+        "lavenderblush",
+        "lawngreen",
+        "lemonchiffon",
+        "lightblue",
+        "lightcoral",
+        "lightcyan",
+        "lightgoldenrodyellow",
+        "lightgray",
+        "lightgreen",
+        "lightgrey",
+        "lightpink",
+        "lightsalmon",
+        "lightseagreen",
+        "lightskyblue",
+        "lightslategray",
+        "lightslategrey",
+        "lightsteelblue",
+        "lightyellow",
+        "lime",
+        "limegreen",
+        "linen",
+        "magenta",
+        "maroon",
+        "mediumaquamarine",
+        "mediumblue",
+        "mediumorchid",
+        "mediumpurple",
+        "mediumseagreen",
+        "mediumslateblue",
+        "mediumspringgreen",
+        "mediumturquoise",
+        "mediumvioletred",
+        "midnightblue",
+        "mintcream",
+        "mistyrose",
+        "moccasin",
+        "navajowhite",
+        "navy",
+        "oldlace",
+        "olive",
+        "olivedrab",
+        "orange",
+        "orangered",
+        "orchid",
+        "palegoldenrod",
+        "palegreen",
+        "paleturquoise",
+        "palevioletred",
+        "papayawhip",
+        "peachpuff",
+        "peru",
+        "pink",
+        "plum",
+        "powderblue",
+        "purple",
+        "rebeccapurple",
+        "red",
+        "rosybrown",
+        "royalblue",
+        "saddlebrown",
+        "salmon",
+        "sandybrown",
+        "seagreen",
+        "seashell",
+        "sienna",
+        "silver",
+        "skyblue",
+        "slateblue",
+        "slategray",
+        "slategrey",
+        "snow",
+        "springgreen",
+        "steelblue",
+        "tan",
+        "teal",
+        "thistle",
+        "tomato",
+        "turquoise",
+        "violet",
+        "wheat",
+        "white",
+        "whitesmoke",
+        "yellow",
+        "yellowgreen",
+    ]
     # tab20 = [
-    #     '#1f77b4', '#aec7e8', 
-    #     '#ff7f0e', '#ffbb78', 
-    #     '#2ca02c', '#98df8a', 
-    #     '#d62728', '#ff9896', 
-    #     '#9467bd', '#c5b0d5', 
-    #     '#8c564b', '#c49c94', 
-    #     '#e377c2', '#f7b6d2', 
-    #     '#7f7f7f', '#c7c7c7', 
-    #     '#bcbd22', '#dbdb8d', 
+    #     '#1f77b4', '#aec7e8',
+    #     '#ff7f0e', '#ffbb78',
+    #     '#2ca02c', '#98df8a',
+    #     '#d62728', '#ff9896',
+    #     '#9467bd', '#c5b0d5',
+    #     '#8c564b', '#c49c94',
+    #     '#e377c2', '#f7b6d2',
+    #     '#7f7f7f', '#c7c7c7',
+    #     '#bcbd22', '#dbdb8d',
     #     '#17becf', '#9edae5']
 
     tab20 = [
-        '#1f77b4', 
-        '#ff7f0e', 
-        '#d62728', '#ff9896', 
-        '#9467bd', 'navy', 
-        '#8c564b', 'dimgray', 
-        '#e377c2', 'darkolivegreen', 
-        '#bcbd22', 
-        '#17becf', "chartreuse"]
+        "#1f77b4",
+        "#ff7f0e",
+        "#d62728",
+        "#ff9896",
+        "#9467bd",
+        "navy",
+        "#8c564b",
+        "dimgray",
+        "#e377c2",
+        "darkolivegreen",
+        "#bcbd22",
+        "#17becf",
+        "chartreuse",
+    ]
 
-    
-    X_new, obs, standard_embedding, labels, clusters = setup_support_data(method="tsne")
+    X_new, obs, standard_embedding, labels, clusters = setup_support_data(
+        method="tsne")
 
     i = 0
-    for k in range(len(obs)): 
-        if obs[k] in ['surv2m', 'surv6m', 'avtisst', 'dzclass', 'aps', 'death', 'sps', 'dnr', 'adlsc', 'prg6m', 'prg2m', 'd.time', 'num.co']:
+    for k in range(len(obs)):
+        if obs[k] in [
+            "surv2m",
+            "surv6m",
+            "avtisst",
+            "dzclass",
+            "aps",
+            "death",
+            "sps",
+            "dnr",
+            "adlsc",
+            "prg6m",
+            "prg2m",
+            "d.time",
+            "num.co",
+        ]:
             colors[k] = tab20[i]
-            if  obs[k] == "surv6m":
+            if obs[k] == "surv6m":
                 colors[k] = "darkred"
-            if  obs[k] == "num.co":
+            if obs[k] == "num.co":
                 colors[k] = "orangered"
             if obs[k] == "adlsc":
                 colors[k] = "peru"
             i += 1
-    
-    fig, axi = plt.subplots(1, 3, figsize=((7.125-0.17), ((7.125-0.17)/1.8)/1.618))
+
+    fig, axi = plt.subplots(
+        1, 3, figsize=((7.125 - 0.17), ((7.125 - 0.17) / 1.8) / 1.618)
+    )
     plt.tight_layout()
 
     scs = []
     # for val, i in zip([0, 1, 2, 3], [0, 5, 2, 1]):
     for val, i in zip([0, 3, 1, 2], [0, 2, 5, 1]):
-        sc = axi[0].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', color=matplotlib.colormaps["Accent"].colors[i], alpha=0.3)
+        sc = axi[0].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Accent"].colors[i],
+            alpha=0.3,
+        )
         scs.append(sc)
-        axi[1].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', color=matplotlib.colormaps["Accent"].colors[i], alpha=0.3)
-        axi[2].scatter(standard_embedding[labels == val,0], standard_embedding[labels == val,1], marker= '.', color=matplotlib.colormaps["Accent"].colors[i], alpha=0.3)
+        axi[1].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Accent"].colors[i],
+            alpha=0.3,
+        )
+        axi[2].scatter(
+            standard_embedding[labels == val, 0],
+            standard_embedding[labels == val, 1],
+            marker=".",
+            color=matplotlib.colormaps["Accent"].colors[i],
+            alpha=0.3,
+        )
 
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=labels, color_scheme=colors)
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        labels,
+        method="UMAP",
+        cluster_labels=labels,
+        color_scheme=colors,
+    )
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=False,
         standartize_coef=False,
         biggest_arrow_method=True,
         univar_importance=True,
         ax=axi[0],
         scale_circle=3,
         move_circle=[0, 0],
         annotate=0.8,
         arrow_width=0.1,
         plot_scatter=False,
-        plot_top_k=5
+        plot_top_k=5,
     )
 
     axi[0].set_yticks([])
     axi[0].set_xticks([])
     axi[0].set_ylabel("t-SNE2", size=8)
     axi[0].set_xlabel("t-SNE1", size=8)
     axi[0].set_title("Global clock", size=8)
@@ -675,97 +1296,117 @@
         scale_circles=[2.2, 2, 2.5, 0.2],
         # move_circles=[[-1.5, 0.3], [0, 1.5], [2.3, -1], [-0.8, -0.2]],
         move_circles=[[-1.8, 0.3], [-0.8, 0], [2.5, -0.8], [-0.0, 0]],
         annotates=[0.4, 0.4, 0.4, 0.4],
         arrow_width=0.08,
         plot_top_k=5,
         plot_hulls=False,
-        plot_scatter=False
+        plot_scatter=False,
     )
 
     # sc2 = axi[1].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
 
     axi[1].set_yticks([])
     axi[1].set_xticks([])
     axi[1].set_ylabel("t-SNE2", size=8)
     axi[1].set_xlabel("t-SNE1", size=8)
     axi[1].set_title("Local clock", size=8)
     axi[1].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[1].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     # Between
     # sc3 = axi[2].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
-    
+
     arrows2, arrow_labels2 = plot_inst.plot_between_clock(
         standartize_data=True,
         standartize_coef=False,
         univar_importance=False,
         ax=axi[2],
         scale_circles=[6, 10, 0],
         # move_circles=[[1.8, 1.1], [0.1, -0.8], [0.0, 0.0]],
         move_circles=[[0.7, -1.5], [0.4, 1.3], [0, 0]],
         annotates=[0.5, 0.5, 0.5],
         arrow_width=0.08,
         plot_top_k=5,
         plot_scatter=False,
-        plot_hulls=False
+        plot_hulls=False,
     )
 
     axi[2].set_yticks([])
     axi[2].set_xticks([])
     axi[2].set_ylabel("t-SNE2", size=8)
     axi[2].set_xlabel("t-SNE1", size=8)
-    axi[2].set_title("Inter-cluster clock", size=8)
+    axi[2].set_title("Inter-group clock", size=8)
     axi[2].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[2].xaxis.set_label_coords(x=0.5, y=-0.02)
 
-
     arrows_dict = {}
     for i, val in enumerate(arrow_labels):
         arrows_dict[val] = arrows[i]
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
     for i, val in enumerate(arrow_labels2):
         arrows_dict[val] = arrows2[i]
 
     print(len(list(arrows_dict.keys())))
-    
-    hatches = [plt.plot([],marker="", ls="")[0]]*3 + \
-        list(arrows_dict.values())[0:2]   + [scs[0]] + \
-        list(arrows_dict.values())[2:4]   + [scs[3]] + \
-        list(arrows_dict.values())[4:6]   + [scs[1]] + \
-        list(arrows_dict.values())[6:8]   + [scs[2]] + \
-        list(arrows_dict.values())[8:10]  + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[10:12] + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[12:14] + [plt.plot([],marker="", ls="")[0]] + \
-        list(arrows_dict.values())[14:]   + [plt.plot([],marker="", ls="")[0]]
-    
-    labels = ["Factors:", " ", "Labels (Disability):"] + \
-        list(arrows_dict.keys())[0:2]   + ["Level 1"] + \
-        list(arrows_dict.keys())[2:4]   + ["Level 2"] + \
-        list(arrows_dict.keys())[4:6]   + ["Level 3"] + \
-        list(arrows_dict.keys())[6:8]   + ["Level 4"] + \
-        list(arrows_dict.keys())[8:10]  + [" "] + \
-        list(arrows_dict.keys())[10:12] + [" "] + \
-        list(arrows_dict.keys())[12:14] + [" "] + \
-        list(arrows_dict.keys())[14:]   + [" "]
 
-    
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 3
+        + list(arrows_dict.values())[0:2]
+        + [scs[0]]
+        + list(arrows_dict.values())[2:4]
+        + [scs[3]]
+        + list(arrows_dict.values())[4:6]
+        + [scs[1]]
+        + list(arrows_dict.values())[6:8]
+        + [scs[2]]
+        + list(arrows_dict.values())[8:10]
+        + [plt.plot([], marker="", ls="")[0]]
+        + list(arrows_dict.values())[10:12]
+        + [plt.plot([], marker="", ls="")[0]]
+        + list(arrows_dict.values())[12:14]
+        + [plt.plot([], marker="", ls="")[0]]
+        + list(arrows_dict.values())[14:]
+        + [plt.plot([], marker="", ls="")[0]]
+    )
+
+    labels = (
+        ["Factors:", " ", "Labels (Disability):"]
+        + list(arrows_dict.keys())[0:2]
+        + ["Level 1"]
+        + list(arrows_dict.keys())[2:4]
+        + ["Level 2"]
+        + list(arrows_dict.keys())[4:6]
+        + ["Level 3"]
+        + list(arrows_dict.keys())[6:8]
+        + ["Level 4"]
+        + list(arrows_dict.keys())[8:10]
+        + [" "]
+        + list(arrows_dict.keys())[10:12]
+        + [" "]
+        + list(arrows_dict.keys())[12:14]
+        + [" "]
+        + list(arrows_dict.keys())[14:]
+        + [" "]
+    )
+
     leg = axi[2].legend(
         hatches,
         labels,
         loc="lower center",
         bbox_to_anchor=(-0.84, 1.12),
         fontsize=7,
         ncol=9,
         markerscale=1,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     plt.subplots_adjust(
         left=0.02,
@@ -773,127 +1414,317 @@
         top=0.7,
         bottom=0.06,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/support/support_3.pdf")
 
 
 def test_local_hdbscan():
-    colors = ['aliceblue', 'antiquewhite', 'aqua', 'aquamarine', 'azure', 'beige', 'bisque', 'black', 
-              'blanchedalmond', 'blue', 'blueviolet', 'brown', 'burlywood', 'cadetblue', 'chartreuse', 
-              'chocolate', 'coral', 'cornflowerblue', 'cornsilk', 'crimson', 'cyan', 'darkblue', 
-              'darkcyan', 'darkgoldenrod', 'darkgray', 'darkgreen', 'darkgrey', 'darkkhaki', 
-              'darkmagenta', 'darkolivegreen', 'darkorange', 'darkorchid', 'darkred', 'darksalmon', 
-              'darkseagreen', 'darkslateblue', 'darkslategray', 'darkslategrey', 'darkturquoise', 
-              'darkviolet', 'deeppink', 'deepskyblue', 'dimgray', 'dimgrey', 'dodgerblue', 'firebrick', 
-              'floralwhite', 'forestgreen', 'fuchsia', 'gainsboro', 'ghostwhite', 'gold', 'goldenrod', 'gray', 
-              'green', 'greenyellow', 'grey', 'honeydew', 'hotpink', 'indianred', 'indigo', 'ivory', 
-              'khaki', 'lavender', 'lavenderblush', 'lawngreen', 'lemonchiffon', 'lightblue', 'lightcoral', 
-              'lightcyan', 'lightgoldenrodyellow', 'lightgray', 'lightgreen', 'lightgrey', 'lightpink', 
-              'lightsalmon', 'lightseagreen', 'lightskyblue', 'lightslategray', 'lightslategrey', 
-              'lightsteelblue', 'lightyellow', 'lime', 'limegreen', 'linen', 'magenta', 'maroon', 
-              'mediumaquamarine', 'mediumblue', 'mediumorchid', 'mediumpurple', 'mediumseagreen', 
-              'mediumslateblue', 'mediumspringgreen', 'mediumturquoise', 'mediumvioletred', 'midnightblue', 
-              'mintcream', 'mistyrose', 'moccasin', 'navajowhite', 'navy', 'oldlace', 'olive', 'olivedrab', 
-              'orange', 'orangered', 'orchid', 'palegoldenrod', 'palegreen', 'paleturquoise', 'palevioletred', 
-              'papayawhip', 'peachpuff', 'peru', 'pink', 'plum', 'powderblue', 'purple', 'rebeccapurple', 'red', 
-              'rosybrown', 'royalblue', 'saddlebrown', 'salmon', 'sandybrown', 'seagreen', 'seashell', 'sienna', 
-              'silver', 'skyblue', 'slateblue', 'slategray', 'slategrey', 'snow', 'springgreen', 'steelblue', 
-              'tan', 'teal', 'thistle', 'tomato', 'turquoise', 'violet', 'wheat', 'white', 'whitesmoke', 'yellow', 
-              'yellowgreen']
-    
+    colors = [
+        "aliceblue",
+        "antiquewhite",
+        "aqua",
+        "aquamarine",
+        "azure",
+        "beige",
+        "bisque",
+        "black",
+        "blanchedalmond",
+        "blue",
+        "blueviolet",
+        "brown",
+        "burlywood",
+        "cadetblue",
+        "chartreuse",
+        "chocolate",
+        "coral",
+        "cornflowerblue",
+        "cornsilk",
+        "crimson",
+        "cyan",
+        "darkblue",
+        "darkcyan",
+        "darkgoldenrod",
+        "darkgray",
+        "darkgreen",
+        "darkgrey",
+        "darkkhaki",
+        "darkmagenta",
+        "darkolivegreen",
+        "darkorange",
+        "darkorchid",
+        "darkred",
+        "darksalmon",
+        "darkseagreen",
+        "darkslateblue",
+        "darkslategray",
+        "darkslategrey",
+        "darkturquoise",
+        "darkviolet",
+        "deeppink",
+        "deepskyblue",
+        "dimgray",
+        "dimgrey",
+        "dodgerblue",
+        "firebrick",
+        "floralwhite",
+        "forestgreen",
+        "fuchsia",
+        "gainsboro",
+        "ghostwhite",
+        "gold",
+        "goldenrod",
+        "gray",
+        "green",
+        "greenyellow",
+        "grey",
+        "honeydew",
+        "hotpink",
+        "indianred",
+        "indigo",
+        "ivory",
+        "khaki",
+        "lavender",
+        "lavenderblush",
+        "lawngreen",
+        "lemonchiffon",
+        "lightblue",
+        "lightcoral",
+        "lightcyan",
+        "lightgoldenrodyellow",
+        "lightgray",
+        "lightgreen",
+        "lightgrey",
+        "lightpink",
+        "lightsalmon",
+        "lightseagreen",
+        "lightskyblue",
+        "lightslategray",
+        "lightslategrey",
+        "lightsteelblue",
+        "lightyellow",
+        "lime",
+        "limegreen",
+        "linen",
+        "magenta",
+        "maroon",
+        "mediumaquamarine",
+        "mediumblue",
+        "mediumorchid",
+        "mediumpurple",
+        "mediumseagreen",
+        "mediumslateblue",
+        "mediumspringgreen",
+        "mediumturquoise",
+        "mediumvioletred",
+        "midnightblue",
+        "mintcream",
+        "mistyrose",
+        "moccasin",
+        "navajowhite",
+        "navy",
+        "oldlace",
+        "olive",
+        "olivedrab",
+        "orange",
+        "orangered",
+        "orchid",
+        "palegoldenrod",
+        "palegreen",
+        "paleturquoise",
+        "palevioletred",
+        "papayawhip",
+        "peachpuff",
+        "peru",
+        "pink",
+        "plum",
+        "powderblue",
+        "purple",
+        "rebeccapurple",
+        "red",
+        "rosybrown",
+        "royalblue",
+        "saddlebrown",
+        "salmon",
+        "sandybrown",
+        "seagreen",
+        "seashell",
+        "sienna",
+        "silver",
+        "skyblue",
+        "slateblue",
+        "slategray",
+        "slategrey",
+        "snow",
+        "springgreen",
+        "steelblue",
+        "tan",
+        "teal",
+        "thistle",
+        "tomato",
+        "turquoise",
+        "violet",
+        "wheat",
+        "white",
+        "whitesmoke",
+        "yellow",
+        "yellowgreen",
+    ]
+
     tab20 = [
-        '#1f77b4', 
-        '#bcbd22',  
-        '#9467bd',
-        '#8c564b', 
-        '#e377c2', 'orangered', 
-        '#d62728', "darkolivegreen",
-        '#17becf', "navy"]
-    
-    color_dict = {"Disease":"#1f77b4",
-    "Coma score":"#bcbd22",
-    "Micro cost":"#9467bd",
-    "Avg. TISS score":"#8c564b",
-    "Diabetes":"#e377c2",
-    "Dementia":"orangered",
-    "2 month survival":"#d62728",
-    "Bilirubin":"darkolivegreen",
-    "ADL patient":"#17becf",
-    "ADL family":"navy"}
-    
-    X_new, obs, standard_embedding, labels, clusters = setup_support_data(method="tsne")
+        "#1f77b4",
+        "#bcbd22",
+        "#9467bd",
+        "#8c564b",
+        "#e377c2",
+        "orangered",
+        "#d62728",
+        "darkolivegreen",
+        "#17becf",
+        "navy",
+    ]
+
+    color_dict = {
+        "Disease": "#1f77b4",
+        "Coma score": "#bcbd22",
+        "Micro cost": "#9467bd",
+        "Avg. TISS score": "#8c564b",
+        "Diabetes": "#e377c2",
+        "Dementia": "orangered",
+        "2 month survival": "#d62728",
+        "Bilirubin": "darkolivegreen",
+        "ADL patient": "#17becf",
+        "ADL family": "navy",
+    }
+
+    X_new, obs, standard_embedding, labels, clusters = setup_support_data(
+        method="tsne")
 
     i = 0
-    for k in range(len(obs)): 
-        if obs[k] in ['Disease', 'Avg. TISS score', 
-                      'APACHE3 score', 'Cost/charges ratio', 
-                      'Diabetes', 'Dementia', 
-                      'ADL family', 'ADL patient', 
-                      'Bilirubin', 'Coma score', 
-                      'Physiology score', '2 month survival', 
-                      'Study enter', 'Micro cost']:
-            
-            if obs[k] == 'APACHE3 score':
+    for k in range(len(obs)):
+        if obs[k] in [
+            "Disease",
+            "Avg. TISS score",
+            "APACHE3 score",
+            "Cost/charges ratio",
+            "Diabetes",
+            "Dementia",
+            "ADL family",
+            "ADL patient",
+            "Bilirubin",
+            "Coma score",
+            "Physiology score",
+            "2 month survival",
+            "Study enter",
+            "Micro cost",
+        ]:
+
+            if obs[k] == "APACHE3 score":
                 colors[k] = "purple"
-            elif obs[k] == 'Study enter':
+            elif obs[k] == "Study enter":
                 colors[k] = "peru"
-            elif obs[k] == 'Physiology score':
+            elif obs[k] == "Physiology score":
                 colors[k] = "dimgray"
-            elif obs[k] == 'Cost/charges ratio':
+            elif obs[k] == "Cost/charges ratio":
                 colors[k] = "#ff7f0e"
             else:
                 colors[k] = tab20[i]
                 i += 1
-    fig_size = ((7.125-0.17)/2, ((7.125-0.17)/2.3)/1.618)
-    fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=1000, facecolor="w",edgecolor="k",)
-    spec2 = gridspec.GridSpec(ncols=3, nrows=1, figure=fig, 
-                     left=0.04, right=0.99, top=0.63, bottom=0.06)
+    fig_size = ((7.125 - 0.17) / 2, ((7.125 - 0.17) / 2.3) / 1.618)
+    fig = plt.figure(
+        constrained_layout=True,
+        figsize=fig_size,
+        dpi=1000,
+        facecolor="w",
+        edgecolor="k",
+    )
+    spec2 = gridspec.GridSpec(
+        ncols=3,
+        nrows=1,
+        figure=fig,
+        left=0.04,
+        right=0.99,
+        top=0.63,
+        bottom=0.06)
     ax1 = fig.add_subplot(spec2[0])
     ax2 = fig.add_subplot(spec2[1])
 
-    spec23 = gridspec.GridSpecFromSubplotSpec(2, 3, subplot_spec=spec2[2], hspace=0.25, wspace=0.08)# wspace=-0.5, hspace=-0.9)
+    spec23 = gridspec.GridSpecFromSubplotSpec(
+        2, 3, subplot_spec=spec2[2], hspace=0.25, wspace=0.08
+    )  # wspace=-0.5, hspace=-0.9)
     ax11 = fig.add_subplot(spec23[0, 0])
     ax12 = fig.add_subplot(spec23[0, 1])
     ax13 = fig.add_subplot(spec23[0, 2])
     ax21 = fig.add_subplot(spec23[1, 0])
     ax23 = fig.add_subplot(spec23[1, 1])
     ax22 = fig.add_subplot(spec23[1, 2])
 
     scs = []
     for val, i in zip([-1, 0, 1], [-1, 0, 6]):
         if val == -1:
-            sc = ax1.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                            color="gray", alpha=0.2, s=13)
-            sc = ax2.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                            color="gray", alpha=0.2, s=13)
+            sc = ax1.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color="gray",
+                alpha=0.2,
+                s=13,
+            )
+            sc = ax2.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color="gray",
+                alpha=0.2,
+                s=13,
+            )
         else:
-            sc = ax1.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                            color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=13)
-            sc = ax2.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
-                            color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=13)
+            sc = ax1.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color=matplotlib.colormaps["Paired"].colors[i],
+                alpha=0.2,
+                s=13,
+            )
+            sc = ax2.scatter(
+                standard_embedding[clusters == val, 0],
+                standard_embedding[clusters == val, 1],
+                marker=".",
+                color=matplotlib.colormaps["Paired"].colors[i],
+                alpha=0.2,
+                s=13,
+            )
         scs.append(sc)
 
-    plot_inst = NonLinearClock(X_new, obs, standard_embedding, clusters, method="UMAP", cluster_labels=clusters, color_scheme=colors)
+    plot_inst = NonLinearClock(
+        X_new,
+        obs,
+        standard_embedding,
+        clusters,
+        method="UMAP",
+        cluster_labels=clusters,
+        color_scheme=colors,
+    )
 
     # Local
     arrows1, arrow_labels1 = plot_inst.plot_local_clocks(
         standartize_data=False,
         standartize_coef=False,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax1,
         scale_circles=[2.5, 15],
         move_circles=[[0, 0], [0, 0]],
-        clocks_labels = ["0", "1"],
-        clocks_labels_angles = [45, 315],
+        clocks_labels=["0", "1"],
+        clocks_labels_angles=[45, 315],
         annotates=[0.5, 0.5],
         arrow_width=0.08,
         plot_top_k=4,
         plot_hulls=False,
-        plot_scatter=False
+        plot_scatter=False,
     )
 
     ax1.set_yticks([])
     ax1.set_xticks([])
     ax1.set_ylabel("t-SNE2", size=8)
     ax1.set_xlabel("t-SNE1", size=8)
     ax1.set_title("Local clock", size=8)
@@ -906,24 +1737,24 @@
         standartize_coef=False,
         univar_importance=False,
         ax=ax2,
         scale_circles=[1],
         move_circles=[[0, 0]],
         annotates=[0.5],
         arrow_width=0.08,
-        plot_top_k=5,
+        plot_top_k=4,
         plot_scatter=False,
-        plot_hulls=False
+        plot_hulls=False,
     )
-    
+
     ax2.set_yticks([])
     ax2.set_xticks([])
     ax2.set_ylabel("t-SNE2", size=8)
     ax2.set_xlabel("t-SNE1", size=8)
-    ax2.set_title("Inter-cluster clock", size=8)
+    ax2.set_title("Inter-group clock", size=8)
     ax2.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax2.xaxis.set_label_coords(x=0.5, y=-0.02)
 
     arrows_dict = {}
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
     for i, val in enumerate(arrow_labels2):
@@ -936,79 +1767,116 @@
     dict_vals[-1] = tmp
     tmp = dict_keys[-2]
     dict_keys[-2] = dict_keys[-1]
     dict_keys[-1] = tmp
 
     print(dict_keys)
     print(len(dict_keys))
-    
-    hatches = [plt.plot([],marker="", ls="")[0]]*3 + \
-        dict_vals[0:2]  + [scs[1]] + \
-        dict_vals[2:4]  + [scs[2]] + \
-        dict_vals[4:6]  + [scs[0]]
-    
-    labels = ["Factors:", " ", "Labels:"] + \
-        dict_keys[0:2] + ["0"] + \
-        dict_keys[2:4] + ["1"] + \
-        dict_keys[4:6] + ["No class"] 
-        
+
+    hatches = (
+        [plt.plot([], marker="", ls="")[0]] * 3
+        + dict_vals[0:2]
+        + [scs[1]]
+        + dict_vals[2:4]
+        + [scs[2]]
+        + dict_vals[4:6]
+        + [scs[0]]
+    )
+
+    labels = (
+        ["Factors:", " ", "Labels:"]
+        + dict_keys[0:2]
+        + ["0"]
+        + dict_keys[2:4]
+        + ["1"]
+        + dict_keys[4:6]
+        + ["No class"]
+    )
+
     leg = ax12.legend(
         hatches,
         labels,
         loc="lower center",
         bbox_to_anchor=(-3.9, 1.35),
         fontsize=7,
         ncol=4,
         markerscale=1,
         handlelength=1.5,
         columnspacing=0.8,
         handletextpad=0.5,
-        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+        handler_map={
+            mpatches.FancyArrow: HandlerPatch(patch_func=make_legend_arrow),
+        },
     )
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
-    for lh in leg.legendHandles: 
+    for lh in leg.legendHandles:
         lh.set_alpha(1)
 
-
     # fourth plot
-    standard_embedding[:,0], standard_embedding[:,1] = 20 * standard_embedding[:,0], 1 * standard_embedding[:,1]
-    for (i, o), axi_i in zip(enumerate(dict_keys), [ax11, ax12, ax13, ax21, ax22, ax23]):
-        im = axi_i.scatter(
-            standard_embedding[:, 0],
-            standard_embedding[:, 1],
-            marker=".",
-            s=1,
-            c=X_new[o],
-            cmap=cm.coolwarm,
-            alpha=0.8
-        )
+    standard_embedding[:, 0], standard_embedding[:, 1] = (
+        20 * standard_embedding[:, 0],
+        1 * standard_embedding[:, 1],
+    )
+    for (i, o), axi_i in zip(
+        enumerate(dict_keys), [ax11, ax12, ax13, ax21, ax22, ax23]
+    ):
+        if i == 0:
+            im = axi_i.scatter(
+                standard_embedding[:, 0],
+                standard_embedding[:, 1],
+                marker=".",
+                s=1,
+                c=X_new[o],
+                cmap=cm.coolwarm,
+                alpha=0.8,
+            )
+        else:
+            axi_i.scatter(
+                standard_embedding[:, 0],
+                standard_embedding[:, 1],
+                marker=".",
+                s=1,
+                c=X_new[o],
+                cmap=cm.coolwarm,
+                alpha=0.8,
+            )
+
         axi_i.set_yticks([])
         axi_i.set_xticks([])
 
         names = {
-            'Disease':'Dis.', 
-            'ADL family':'ADL f.', 
-            'ADL patient':'ADL p.', 
-            'Dementia':'Dem.',
-            'Diabetes':'Diab.',
-            'Charges': 'Charges',
-            'Study enter':'St. e.'
+            "Disease": "Dis.",
+            "ADL family": "ADL f.",
+            "ADL patient": "ADL p.",
+            "Dementia": "Dem.",
+            "Diabetes": "Diab.",
+            "Charges": "Charges",
+            "Study enter": "St. e.",
         }
 
         axi_i.set_title(names[o], size=5, pad=-14)
 
     ax21.set_ylabel("t-SNE2", size=8)
     ax22.set_xlabel("t-SNE1", size=8)
 
     ax21.yaxis.set_label_coords(0, 1.15)
     ax22.xaxis.set_label_coords(-0.5, -0.04)
 
-    cbar = fig.colorbar(im, ax=[ax11, ax12, ax13, ax21, ax22, ax23], pad=0.03, aspect=40)
-    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
+    # ticks=[0, 5, 10, 15])
+    cbar = fig.colorbar(
+        im,
+        ax=[ax11, ax12, ax13, ax21, ax22, ax23],
+        pad=0.03,
+        aspect=40,
+    )
+    cbar.ax.tick_params(
+        labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1
+    )  # labelrotation=90,
     cbar.outline.set_visible(False)
 
     plt.savefig("plots/paper/support/support_local_hdbscan.pdf")
 
-# test_between_all_3()
+
+test_between_all_3()
 test_local_hdbscan()
```

