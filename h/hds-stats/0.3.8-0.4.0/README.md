# Comparing `tmp/hds-stats-0.3.8.tar.gz` & `tmp/hds_stats-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.3.8.tar", last modified: Fri Aug  4 13:48:39 2023, max compression
+gzip compressed data, was "hds_stats-0.4.0.tar", last modified: Tue May 14 21:44:31 2024, max compression
```

## Comparing `hds-stats-0.3.8.tar` & `hds_stats-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-08-04 13:48:39.488951 hds-stats-0.3.8/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.8/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-08-04 13:48:39.488693 hds-stats-0.3.8/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.8/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-08-04 13:48:39.486526 hds-stats-0.3.8/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.8/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     9519 2023-07-10 06:49:34.000000 hds-stats-0.3.8/hds_stats/ml.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11856 2023-07-10 06:45:02.000000 hds-stats-0.3.8/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27275 2023-08-04 13:47:41.000000 hds-stats-0.3.8/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-08-04 13:48:39.488285 hds-stats-0.3.8/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.8/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-08-04 13:48:39.489041 hds-stats-0.3.8/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-08-04 13:47:53.000000 hds-stats-0.3.8/setup.py
+drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-14 21:44:31.822028 hds_stats-0.4.0/
+-rw-------   0 seonghona   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds_stats-0.4.0/LICENSE
+-rw-r--r--   0 seonghona   (501) staff       (20)      829 2024-05-14 21:44:31.821457 hds_stats-0.4.0/PKG-INFO
+-rw-------   0 seonghona   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds_stats-0.4.0/README.md
+drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-14 21:44:31.818495 hds_stats-0.4.0/hds_stats/
+-rw-------   0 seonghona   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds_stats-0.4.0/hds_stats/__init__.py
+-rw-------   0 seonghona   (501) staff       (20)    10483 2024-05-14 03:26:39.000000 hds_stats-0.4.0/hds_stats/ml.py
+-rw-------   0 seonghona   (501) staff       (20)    13163 2024-05-14 03:26:38.000000 hds_stats-0.4.0/hds_stats/plot.py
+-rw-------   0 seonghona   (501) staff       (20)    28176 2024-05-14 03:26:38.000000 hds_stats-0.4.0/hds_stats/stat.py
+drwxr-xr-x   0 seonghona   (501) staff       (20)        0 2024-05-14 21:44:31.820936 hds_stats-0.4.0/hds_stats.egg-info/
+-rw-r--r--   0 seonghona   (501) staff       (20)      829 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/PKG-INFO
+-rw-------   0 seonghona   (501) staff       (20)      279 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/SOURCES.txt
+-rw-------   0 seonghona   (501) staff       (20)        1 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/dependency_links.txt
+-rw-------   0 seonghona   (501) staff       (20)       72 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/requires.txt
+-rw-------   0 seonghona   (501) staff       (20)       23 2024-05-14 21:44:31.000000 hds_stats-0.4.0/hds_stats.egg-info/top_level.txt
+-rw-------   0 seonghona   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds_stats-0.4.0/pyproject.toml
+-rw-r--r--   0 seonghona   (501) staff       (20)       38 2024-05-14 21:44:31.822156 hds_stats-0.4.0/setup.cfg
+-rw-------   0 seonghona   (501) staff       (20)     1210 2024-05-13 23:36:17.000000 hds_stats-0.4.0/setup.py
```

### Comparing `hds-stats-0.3.8/LICENSE` & `hds_stats-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.8/hds_stats/ml.py` & `hds_stats-0.4.0/hds_stats/ml.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     
     with open(file = f'{fileName}.dot', mode = 'rt') as file:
         graph = file.read()
         graph = graphviz.Source(source = graph, format = 'png')
         graph.render(filename = fileName)
     
     os.remove(f'{fileName}')
+    
     os.remove(f'{fileName}.dot')
 
 
 # 입력변수별 중요도 시각화
 def plot_feature_importance(model, pal = 'Spectral'):
     '''
     이 함수는 입력변수별 중요도로 막대 그래프를 그립니다.
@@ -70,49 +71,60 @@
     
     import numpy as np
     import pandas as pd
     import seaborn as sns
     import matplotlib.pyplot as plt
     
     if 'LGBM' in str(type(model)):
-        imp = pd.DataFrame(
+        fi = pd.DataFrame(
             data = model.feature_importances_, 
             index = model.feature_name_, 
-            columns = ['Imp']
+            columns = ['importance']
         )
     else:
-        imp = pd.DataFrame(
+        fi = pd.DataFrame(
             data = model.feature_importances_, 
             index = model.feature_names_in_, 
-            columns = ['Imp']
-        )
-    
-    imp = imp.sort_values(by = 'Imp', ascending = False)
-    imp = imp.reset_index()
+            columns = ['importance']
+        ) \
+        .sort_values(by = 'importance', ascending = False) \
+        .reset_index()
     
     sns.barplot(
-        data = imp, 
-        x = 'Imp', 
+        data = fi, 
+        x = 'importance', 
         y = 'index', 
-        palette = pal
+        hue = 'index', 
+        palette = pal, 
+        legend = True
     )
     
-    for index, row in imp.iterrows():
+    for i, r in fi.iterrows():
         plt.text(
-            x = row['Imp'], 
-            y = index, 
-            s = np.round(row['Imp'], 3), 
+            x = r['importance'] + 0.01, 
+            y = i, 
+            s = f"{r['importance']:.3f}", 
             ha = 'left', 
-            va = 'center'
+            va = 'center', 
+            fontsize = 8, 
+            fontweight = 'bold'
         )
     
-    plt.xlim(0, imp['Imp'].max() * 1.2)
-    plt.title(label = 'Feature Importances')
+    plt.xlim(0, fi['importance'].max() * 1.2)
+    
+    plt.title(label = 'Feature Importances', 
+              fontdict = {'fontweight': 'bold'})
+    
     plt.xlabel(xlabel = 'Feature Importances')
-    plt.ylabel(ylabel = 'Feature');
+    
+    plt.ylabel(ylabel = 'Feature')
+    
+    plt.legend(loc = 'lower right',
+               title = 'feat_imp', 
+               fontsize = 8);
 
 
 # 나무모형 가지치기 단계 그래프 시각화
 def plot_step(data, x = 'alpha', y = 'impurity', color = 'blue', xangle = None):
     '''
     이 함수는 나무모형 가지치기 결과로 단계 그래프를 그립니다.
     
@@ -169,27 +181,33 @@
     n = len(x)
     xticks = range(1, n + 1)
     
     sns.lineplot(
         x = xticks, 
         y = x, 
         color = 'blue',
-        ls = '--', 
+        linestyle = '-', 
+        linewidth = 1, 
         marker = 'o'
     )
     
     plt.axhline(
         y = 1, 
         color = 'red', 
-        linestyle = '--'
+        linestyle = '--', 
+        linewidth = 0.5
     )
     
     plt.xticks(ticks = xticks)
-    plt.title(label = 'Scree Plot')
+    
+    plt.title(label = 'Scree Plot', 
+              fontdict = {'fontweight': 'bold'})
+    
     plt.xlabel(xlabel = 'Number of PC')
+    
     plt.ylabel(ylabel = 'Variance');
     
 
 # 주성분 분석 행렬도 시각화
 def plot_biplot(score, coefs, x = 1, y = 2, zoom = 1):
     '''
     이 함수는 주성분 분석 결과를 받아 스크리 도표를 그립니다.
@@ -205,64 +223,73 @@
         그래프 외에 반환하는 객체는 없습니다.
     '''
     
     import seaborn as sns
     import matplotlib.pyplot as plt
     
     xs = score.iloc[:, x-1]
+    
     ys = score.iloc[:, y-1]
     
     sns.scatterplot(
         x = xs, 
         y = ys, 
         fc = 'silver',
         ec = 'black',
         s = 15, 
         alpha = 0.2
     )
     
     plt.axvline(
         x = 0, 
         color = '0.5', 
-        linestyle = '--'
+        linestyle = '--', 
+        linewidth = 0.5
     )
     
     plt.axhline(
         y = 0, 
         color = '0.5', 
-        linestyle = '--'
+        linestyle = '--', 
+        linewidth = 0.5
     )
     
     n = score.shape[1]
+    
     for i in range(n):
         plt.arrow(
             x = 0, 
             y = 0, 
             dx = coefs.iloc[i, x-1] * zoom, 
             dy = coefs.iloc[i, y-1] * zoom, 
             color = 'red',
-            lw = 0.5,
+            linewidth = 0.5,
             alpha = 0.5
         )
         
         plt.text(
             x = coefs.iloc[i, x-1] * (zoom + 0.5), 
             y = coefs.iloc[i, y-1] * (zoom + 0.5), 
             s = coefs.index[i], 
             color = 'darkred', 
             ha = 'center', 
             va = 'center', 
-            fontsize = 8
+            fontsize = 8, 
+            fontweight = 'bold'
         )
     
     # plt.xlim(-1, 1)
     # plt.ylim(-1, 1)
     # plt.grid()
-    plt.title(label = 'Biplot with PC1 and PC2')
+    
+    plt.title(label = 'Biplot with PC1 and PC2', 
+              fontdict = {'fontweight': 'bold'})
+    
     plt.xlabel(xlabel = 'PC{}'.format(x))
+    
     plt.ylabel(ylabel = 'PC{}'.format(y));
 
 
 # k-평균 군집분석 WSS 단계 그래프 시각화
 def plot_wcss(X, k = 3):
     '''
     이 함수는 군집별 편차 제곱합으로 선 그래프를 그립니다.
@@ -276,25 +303,36 @@
     '''
     
     from sklearn.cluster import KMeans
     import seaborn as sns
     import matplotlib.pyplot as plt
     
     ks = range(1, k + 1)
+    
     result = []
+    
     for k in ks:
         model = KMeans(n_clusters = k, random_state = 0)
         model.fit(X = X)
         wcss = model.inertia_
         result.append(wcss)
     
-    sns.lineplot(x = ks, y = result, marker = 'o')
+    sns.lineplot(x = ks, 
+                 y = result, 
+                 marker = 'o', 
+                 linestyle = '-', 
+                 linewidth = 1)
+    
     plt.xticks(ticks = ks)
-    plt.title(label = 'Elbow Method')
+    
+    plt.title(label = 'Elbow Method', 
+              fontdict = {'fontweight': 'bold'})
+    
     plt.xlabel(xlabel = 'Number of clusters')
+    
     plt.ylabel(ylabel = 'Within Cluster Sum of Squares');
 
 
 # k-평균 군집분석 실루엣 지수 시각화
 def plot_silhouette(X, k = 3):
     '''
     이 함수는 군집별 실루엣 지수로 선 그래프를 그립니다.
@@ -309,24 +347,35 @@
     
     from sklearn.cluster import KMeans
     from sklearn.metrics import silhouette_score
     import seaborn as sns
     import matplotlib.pyplot as plt
     
     ks = range(1, k + 1)
+    
     result = [0]
+    
     for k in ks:
         if k == 1: continue
         model = KMeans(n_clusters = k, random_state = 0)
         model.fit(X = X)
         cluster = model.predict(X = X)
         silwidth = silhouette_score(X = X, labels = cluster)
         result.append(silwidth)
     
-    sns.lineplot(x = ks, y = result, marker = 'o')
+    sns.lineplot(x = ks, 
+                 y = result, 
+                 marker = 'o', 
+                 linestyle = '-', 
+                 linewidth = 1)
+    
     plt.xticks(ticks = ks)
-    plt.title(label = 'Silhouette Width')
+    
+    plt.title(label = 'Silhouette Width', 
+              fontdict = {'fontweight': 'bold'})
+    
     plt.xlabel(xlabel = 'Number of clusters')
+    
     plt.ylabel(ylabel = 'Silhouette Width Average');
 
 
 ## End of Document
```

### Comparing `hds-stats-0.3.8/hds_stats/plot.py` & `hds_stats-0.4.0/hds_stats/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,48 +16,62 @@
     '''
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
     
-    avg = data.groupby(x)[y].mean().reset_index()
+    avg = data.groupby(by = x)[y].mean()
     
     sns.boxplot(
         data = data, 
         x = x, 
         y = y, 
-        order = avg[x], 
+        hue = x, 
+        order = avg.index, 
         palette = pal, 
         flierprops = {
             'marker': 'o', 
             'markersize': 3, 
             'markerfacecolor': 'pink',
             'markeredgecolor': 'red', 
             'markeredgewidth': 0.2
-        }
-    )
-    
-    sns.scatterplot(
-        data = avg, 
-        x = avg.index, 
-        y = y, 
-        color = 'red', 
-        s = 30, 
-        edgecolor = 'black', 
+        }, 
+        linecolor = '0.5',
         linewidth = 0.5
     )
     
+    # sns.scatterplot(
+    #     data = avg, 
+    #     x = avg.index, 
+    #     y = avg[y], 
+    #     color = 'red', 
+    #     s = 30, 
+    #     edgecolor = 'black', 
+    #     linewidth = 0.5
+    # )
+    
     plt.axhline(
         y = data[y].mean(), 
         color = 'red', 
+        linewidth = 0.5, 
         linestyle = '--'
     )
     
-    plt.title(label = f'{x} 범주별 {y}의 평균 비교');
+    for i, v in enumerate(avg):
+        plt.text(x = i, 
+                 y = v, 
+                 s = f'{v:,.2f}', 
+                 ha = 'center', 
+                 va = 'center',
+                 fontsize = 6, 
+                 fontweight = 'bold')
+    
+    plt.title(label = f'{x} 범주별 {y}의 평균 비교', 
+              fontdict = {'fontweight': 'bold'});
 
 
 # 두 연속형 변수로 산점도를 그리는 함수
 def scatter(data, x: str, y: str, color: str = '0.3') -> None:
     '''
     이 함수는 두 연속형 변수의 산점도를 그립니다.
     
@@ -79,15 +93,16 @@
     sns.scatterplot(
         data = data, 
         x = x, 
         y = y, 
         color = color
     )
     
-    plt.title(label = f'{x}와(과) {y}의 관계');
+    plt.title(label = f'{x}와(과) {y}의 관계', 
+              fontdict = {'fontweight': 'bold'});
 
 
 # 두 연속형 변수로 산점도와 회귀직선을 그리는 함수
 def regline(data, x: str, y: str, color: str = '0.3', size: int = 15) -> None:
     '''
     이 함수는 두 연속형 변수의 산점도에 회귀직선을 그립니다.
     
@@ -109,29 +124,31 @@
         
     sns.regplot(
         data = data, 
         x = x, 
         y = y, 
         ci = None, 
         scatter_kws = {
-            'color': color, 
+            'facecolor': color, 
             'edgecolor': '1', 
             's': size, 
-            'linewidth': 0.5
+            'alpha': 0.2
         },
         line_kws = {
             'color': 'red', 
             'linewidth': 1.5
         }
     )
     
     # x_min = data[x].min()
     # x_max = data[x].max()
     # plt.xlim(x_min * 0.9, x_max * 1.1)
-    plt.title(label = f'{x}와(과) {y}의 관계');
+    
+    plt.title(label = f'{x}와(과) {y}의 관계', 
+              fontdict = {'fontweight': 'bold'});
 
 
 # 범주형 변수의 빈도수로 막대 그래프를 그리는 함수
 def bar_freq(data, x: str, color: str = None, pal: list = None) -> None:
     '''
     이 함수는 범주형 변수의 빈도수를 내림차순 정렬한 막대 그래프를 그립니다.
     
@@ -147,37 +164,44 @@
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
     
     grp = data[x].value_counts()
+    
     v_max = grp.values.max()
+    
     space = np.ceil(v_max * 0.01)
     
     sns.countplot(
         data = data, 
         x = x, 
+        hue = x, 
         order = grp.index, 
         color = color, 
         palette = pal
     )
     
     for i, v in enumerate(grp):
         plt.text(
             x = i, 
             y = v + space, 
             s = v, 
             ha = 'center', 
             va = 'bottom', 
-            c = 'black'
+            c = 'black', 
+            fontsize = 8, 
+            fontweight = 'bold'
         )
     
     plt.ylim(0, v_max * 1.2)
-    plt.title(label = '목표변수의 범주별 빈도수 비교');
+    
+    plt.title(label = '목표변수의 범주별 빈도수 비교', 
+              fontdict = {'fontweight': 'bold'});
 
 
 # 범주형 변수를 소그룹으로 나누고 빈도수로 펼친 막대 그래프를 그리는 함수
 def bar_dodge_freq(data, x: str, group: str, pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 빈도수로 펼친 막대 그래프를 그립니다.
     
@@ -193,15 +217,17 @@
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
     
     grp = data.groupby(by = [x, group]).count().iloc[:, 0]
+    
     v_max = grp.values.max()
+    
     space = np.ceil(v_max * 0.01)
     
     sns.countplot(
         data = data, 
         x = x, 
         hue = group, 
         order = grp.index.levels[0], 
@@ -215,20 +241,27 @@
         else:
             i = (i-1)/2 + 0.2
         plt.text(
             x = i, 
             y = v + space, 
             s = v, 
             ha = 'center', 
-            va = 'bottom'
+            va = 'bottom', 
+            fontsize = 8, 
+            fontweight = 'bold'
         )
     
     plt.ylim(0, v_max * 1.2)
-    plt.title(label = f'{x}의 범주별 {group}의 빈도수 비교')
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
+    
+    plt.title(label = f'{x}의 범주별 {group}의 빈도수 비교', 
+              fontdict = {'fontweight': 'bold'})
+    
+    plt.legend(loc = 'center left', 
+               bbox_to_anchor = (1, 0.5), 
+               fontsize = 8);
 
 
 # 범주형 변수를 소그룹으로 나누고 빈도수로 쌓은 막대 그래프를 그리는 함수
 def bar_stack_freq(data, x: str, group: str, kind: str = 'bar', pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 빈도수로 쌓은 막대 그래프를 그립니다.
     
@@ -245,27 +278,32 @@
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
     
     p = data[group].unique().size
+    
     pv = pd.pivot_table(
         data = data, 
         index = x, 
         columns = group, 
         aggfunc = 'count'
     )
     
     pv = pv.iloc[:, 0:p].sort_index()
+    
     pv.columns = pv.columns.droplevel(level = 0)
+    
     pv.columns.name = None
+    
     pv = pv.reset_index()
     
     cols = pv.columns[1:]
+    
     cumsum = pv[cols].cumsum(axis = 1)
     
     if type(pal) == list:
         pal = sns.set_palette(sns.color_palette(pal))
     
     pv.plot(
         x = x, 
@@ -282,29 +320,35 @@
             for i, (v1, v2) in enumerate(zip(cumsum[col], pv[col])):
                 plt.text(
                     x = i, 
                     y = v1 - v2/2, 
                     s = v2, 
                     ha = 'center', 
                     va = 'center', 
-                    c = 'black'
+                    c = 'black', 
+                    fontsize = 8, 
+                    fontweight = 'bold'
                 );
     elif kind == 'barh':
         for col in cols:
             for i, (v1, v2) in enumerate(zip(cumsum[col], pv[col])):
                 plt.text(
                     x = v1 - v2/2, 
                     y = i, 
                     s = v2, 
                     ha = 'center', 
                     va = 'center', 
-                    c = 'black'
+                    c = 'black', 
+                    fontsize = 8, 
+                    fontweight = 'bold'
                 )
 
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
+    plt.legend(loc = 'center left', 
+               bbox_to_anchor = (1, 0.5), 
+               fontsize = 8);
 
 
 # 범주형 변수를 소그룹으로 나누고 상대도수로 쌓은 막대 그래프를 그리는 함수
 def bar_stack_prop(data, x: str, group: str, kind: str = 'bar', pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 상대도수로 쌓은 막대 그래프를 그립니다.
     
@@ -321,29 +365,36 @@
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
     
     p = data[group].unique().size
+    
     pv = pd.pivot_table(
         data = data, 
         index = x, 
         columns = group, 
         aggfunc = 'count'
     )
     
     pv = pv.iloc[:, 0:p].sort_index()
+    
     pv.columns = pv.columns.droplevel(level = 0)
+    
     pv.columns.name = None
+    
     pv = pv.reset_index()
     
     cols = pv.columns[1:]
+    
     rowsum = pv[cols].apply(func = sum, axis = 1)
+    
     pv[cols] = pv[cols].div(rowsum, 0) * 100
+    
     cumsum = pv[cols].cumsum(axis = 1)
     
     if type(pal) == list:
         pal = sns.set_palette(sns.color_palette(pal))
         
     pv.plot(
         x = x, 
@@ -362,26 +413,32 @@
                 v3 = f'{np.round(v2, 1)}%'
                 plt.text(
                     x = i, 
                     y = v1 - v2/2, 
                     s = v3, 
                     ha = 'center', 
                     va = 'center', 
-                    c = 'black'
+                    c = 'black', 
+                    fontsize = 8, 
+                    fontweight = 'bold'
                 );
     elif kind == 'barh':
         for col in cols:
             for i, (v1, v2) in enumerate(zip(cumsum[col], pv[col])):
                 v3 = f'{np.round(v2, 1)}%'
                 plt.text(
                     x = v1 - v2/2, 
                     y = i, 
                     s = v3, 
                     ha = 'center', 
                     va = 'center', 
-                    c = 'black'
+                    c = 'black', 
+                    fontsize = 8, 
+                    fontweight = 'bold'
                 )
     
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
+    plt.legend(loc = 'center left', 
+               bbox_to_anchor = (1, 0.5), 
+               fontsize = 8);
 
 
 ## End of Document
```

### Comparing `hds-stats-0.3.8/hds_stats/stat.py` & `hds_stats-0.4.0/hds_stats/stat.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     매개변수:
         y: 목표변수 벡터를 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         X: 입력변수 행렬을 pd.DataFrame 또는 2차원 np.ndarray로 지정합니다.
     
     반환:
         다중선형 회귀모형을 적합한 모형을 반환합니다.
     '''
-    import statsmodels.api as sa
+    import statsmodels.api as sma
     
-    model = sa.OLS(endog = y, exog = X)
+    model = sma.OLS(endog = y, exog = X)
     
     return model.fit()
 
 
 # 다중선형 회귀모형 변수선택법 중 전진선택법
 def forward_selection(y, X):
     '''
@@ -35,20 +35,23 @@
     import pandas as pd
     import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
     Xvars = list(set(X.columns))
+    
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ 1'
+    
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
     
     selected = []
+    
     while Xvars:
         Xvar_aic = []
         for Xvar in Xvars:
             formula = f'{y.name} ~ {" + ".join(selected + [Xvar])} + 1'
             aic = smf.ols(formula = formula, data = dat).fit().aic
             aic = np.round(a = aic, decimals = 4)
             Xvar_aic.append((aic, Xvar))
@@ -60,14 +63,15 @@
             Xvars.remove(best_Xvar)
             selected.append(best_Xvar)
             curr_aic = new_aic
         else:
             break
     
     formula = f'{y.name} ~ {" + ".join(selected)} + 1'
+    
     model = smf.ols(formula = formula, data = dat).fit()
     
     return model
 
 
 # 다중선형 회귀모형 변수선택법 중 후진소거법
 def backward_selection(y, X):
@@ -86,20 +90,23 @@
     import pandas as pd
     import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
     Xvars = list(set(X.columns))
+    
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ {" + ".join(list(Xvars))}'
+    
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
     
     selected = []
+    
     while Xvars:
         Xvar_aic = []
         for Xvar in Xvars:
             sub = dat.drop(labels = selected + [Xvar], axis = 1).copy()
             sub_Xvars = set(sub.columns) - set([y.name])
             formula = f'{y.name} ~ {" + ".join(list(sub_Xvars))} + 1'
             aic = smf.ols(formula = formula, data = sub).fit().aic
@@ -113,17 +120,19 @@
             Xvars.remove(best_Xvar)
             selected.append(best_Xvar)
             curr_aic = new_aic
         else:
             break
     
     dat = dat.drop(labels = selected, axis = 1)
+    
     dat_Xvars = set(dat.columns) - set([y.name])
     
     formula = f'{y.name} ~ {" + ".join(list(dat_Xvars))} + 1'
+    
     model = smf.ols(formula = formula, data = dat).fit()
     
     return model
 
 
 # 다중선형 회귀모형 변수선택법 중 단계적방법
 def stepwise_selection(y, X):
@@ -142,20 +151,23 @@
     import pandas as pd
     import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
     Xvars = list(set(X.columns))
+    
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ 1'
+    
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
     
     selected = []
+    
     while Xvars:
         Xvar_aic = []
         for Xvar in Xvars:
             formula = f'{y.name} ~ {" + ".join(selected + [Xvar])} + 1'
             aic = smf.ols(formula = formula, data = dat).fit().aic
             aic = np.round(a = aic, decimals = 4)
             Xvar_aic.append((aic, 'add', Xvar))
@@ -167,28 +179,30 @@
                 sub_Xvars = set(sub.columns) - set([y.name])
                 formula = f'{y.name} ~ {" + ".join(list(sub_Xvars))} + 1'
                 aic = smf.ols(formula = formula, data = sub).fit().aic
                 aic = np.round(a = aic, decimals = 4)
                 Xvar_aic.append((aic, 'sub', Xvar))
         
         Xvar_aic.sort(reverse = True)
+        
         new_aic, how, best_Xvar = Xvar_aic.pop()
         
         if curr_aic > new_aic and how == 'add':
             Xvars.remove(best_Xvar)
             selected.append(best_Xvar)
             curr_aic = new_aic
         elif curr_aic > new_aic and how == 'sub':
             Xvars.append(best_Xvar)
             selected.remove(best_Xvar)
             curr_aic = new_aic
         elif curr_aic <= new_aic:
             break
     
     formula = f'{y.name} ~ {" + ".join(selected)} + 1'
+    
     model = smf.ols(formula = formula, data = dat).fit()
     
     return model
 
 
 # 다중선형 회귀모형 변수선택법
 def stepwise(y, X, direction = 'both'):
@@ -230,50 +244,56 @@
         네 가지 그래프 외에 반환하는 객체는 없습니다.
     '''
     import numpy as np
     import pandas as pd
     import seaborn as sns
     import matplotlib.pyplot as plt
     from scipy import stats
-    import statsmodels.api as sm
+    import statsmodels.api as sma
     
     plt.figure(figsize = (10, 10), dpi = 100)
     
     # 선형성 가정
     # 잔차로 lowess(locally weighted linear regression) 회귀선을 산점도에 추가
     ax1 = plt.subplot(2, 2, 1)
+    
     sns.regplot(
         x = model.fittedvalues, 
         y = model.resid, 
         lowess = True, 
         scatter_kws = dict(
             color = '0.8',
             ec = '0.3', 
             s = 15
         ),
         line_kws = dict(
             color = 'red', 
-            lw = 1
+            linewidth = 1
         ), 
         ax = ax1
     )
+    
     plt.axhline(
         y = 0, 
         color = '0.5', 
-        lw = 1, 
-        ls = '--'
+        linestyle = '--', 
+        linewidth = 1
     )
+    
     plt.title(
         label = 'Residuals vs Fitted', 
-        fontdict = dict(size = 14)
+        fontdict = dict(size = 14, 
+                        fontweight = 'bold')
     )
+    
     plt.xlabel(
         xlabel = 'Fitted values', 
         fontdict = dict(size = 12)
     )
+    
     plt.ylabel(
         ylabel = 'Residuals', 
         fontdict = dict(size = 12)
     )
     
     # 정규성 가정 확인
     ax2 = plt.subplot(2, 2, 2)
@@ -290,74 +310,90 @@
         y = y, 
         color = '0.8', 
         ec = '0.3', 
         size = 2, 
         legend = False, 
         ax = ax2
     )
+    
     plt.plot(
         [-4, 4], 
         [-4, 4], 
         color = '0.5', 
-        lw = 1, 
-        ls = '--'
+        linestyle = '--', 
+        linewidth = 1
     )
+    
     plt.title(
         label = 'Normal Q-Q', 
-        fontdict = dict(size = 14)
+        fontdict = dict(size = 14, 
+                        fontweight = 'bold')
     )
+    
     plt.xlabel(
         xlabel = 'Theoretical Quantiles', 
         fontdict = dict(size = 12)
     )
+    
     plt.ylabel(
         ylabel = 'Standardized residuals', 
         fontdict = dict(size = 12)
     )
     
     # 등분산성 가정 확인
     ax3 = plt.subplot(2, 2, 3)
+    
     sns.regplot(
         x = model.fittedvalues, 
         y = np.sqrt(stdres.abs()), 
         lowess = True,
         scatter_kws = dict(
             color = '0.8', 
             ec = '0.3', 
             s = 15
         ),
         line_kws = dict(
             color = 'red', 
-            lw = 1
+            linewidth = 1
         ), 
         ax = ax3
     )
+    
     plt.title(
         label = 'Scale-Location', 
-        fontdict = dict(size = 14)
+        fontdict = dict(size = 14, 
+                        fontweight = 'bold')
     )
+    
     plt.xlabel(
         xlabel = 'Fitted values', 
         fontdict = dict(size = 12)
     )
+    
     plt.ylabel(
         ylabel = 'Sqrt of Standardized residuals', 
         fontdict = dict(size = 12)
     )
 
     # 쿡의 거리(이상치 탐지)
     ax4 = plt.subplot(2, 2, 4)
-    sm.graphics.influence_plot(
+    
+    fig = sma.graphics.influence_plot(
         results = model, 
         criterion = 'cooks', 
         size = 24, 
         plot_alpha = 0.2, 
         ax = ax4
     )
     
+    for text in ax4.texts:
+        text.set_fontsize(8)
+        text.set_ha('center')
+        text.set_va('center')
+    
     plt.tight_layout();
 
 
 # 쿡의 거리
 def cooks_distance(model):
     '''
     이 함수는 다중선형 회귀모형의 훈련셋으로 관측값별 쿡의 거리를 계산합니다.
@@ -367,14 +403,15 @@
     
     반환:
         훈련셋의 관측값별 쿡의 거리를 반환합니다.
     '''
     from statsmodels.stats.outliers_influence import OLSInfluence
     
     cd, _ = OLSInfluence(results = model).cooks_distance
+    
     cd = cd.sort_values(ascending = False)
     
     return cd
 
 
 # 햇 매트릭스
 def hat_matrix(X):
@@ -387,16 +424,19 @@
     반환:
         훈련셋의 햇 매트릭스를 반환합니다.
     '''
     import numpy as np
     import pandas as pd
     
     X = np.array(object = X)
+    
     XtX = np.matmul(X.transpose(), X)
+    
     XtX_inv = np.linalg.inv(XtX)
+    
     result = np.matmul(np.matmul(X, XtX_inv), X.transpose())
     
     return result
 
 
 # 레버리지(hat value) 계산
 def leverage(X):
@@ -409,16 +449,19 @@
     반환:
         훈련셋의 관측값별 Leverage를 반환합니다.
     '''
     import numpy as np
     import pandas as pd
     
     n = X.shape[0]
+    
     hatMat = hat_matrix(X = X)
+    
     X['Leverage'] = np.array([hatMat[i][i] for i in range(n)])
+    
     X = X.iloc[:, -1].sort_values(ascending = False)
     
     return X
 
 
 # 표준화 잔차 계산
 def std_Resid(model):
@@ -430,14 +473,15 @@
     
     반환:
         훈련셋의 관측값별 표준화 잔차를 반환합니다.
     '''
     from scipy import stats
     
     stdres = stats.zscore(a = model.resid)
+    
     locs = stdres.abs().sort_values(ascending = False)
     
     return stdres[locs.index]
 
 
 # 선형 회귀모형의 영향점 계산
 def augment(model):
@@ -485,17 +529,17 @@
         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         선형 회귀모형의 잔차 등분산성 검정 결과를 반환합니다.
     '''
     import numpy as np
     import pandas as pd
-    import statsmodels.api as sm
+    import statsmodels.api as sma
     
-    test = sm.stats.het_breuschpagan(
+    test = sma.stats.het_breuschpagan(
         resid = model.resid, 
         exog_het = model.model.exog
     )
     
     result = pd.DataFrame(
         data = test, 
         index = ['Statistic', 'P-Value', 'F-Value', 'F P-Value']
@@ -516,16 +560,19 @@
         입력변수 행렬의 열별 분산팽창지수를 반환합니다.
     '''
     import numpy as np
     import pandas as pd
     import statsmodels.stats.outliers_influence as oi
     
     func = oi.variance_inflation_factor
+    
     ncol = len(model.model.exog_names)
+    
     vifs = [func(exog = model.model.exog, exog_idx = i) for i in range(1, ncol)]
+    
     result = pd.DataFrame(data = vifs, index = model.model.exog_names[1:]).T
     
     return result
 
 
 # 회귀모형의 회귀계수
 def coefs(model):
@@ -573,14 +620,15 @@
     
     model_type = str(type(model.model))
     
     X = pd.DataFrame(
         data = model.model.exog, 
         columns = model.model.exog_names
     )
+    
     if 'OLS' in model_type:
         y = model.model.endog
         result = model.params * (X.std() / y.std())
     elif 'GLM' in model_type:
         y = 1
         result = model.params * (X.std() / 1)
     
@@ -599,46 +647,44 @@
     반환:
         회귀모형의 다양한 성능 지표를 데이터프레임으로 반환합니다.
         실제값과 추정값이 음수일 때 RMSLE는 결측값으로 채웁니다.
     '''
     import numpy as np
     import pandas as pd
     from sklearn.metrics import mean_squared_error
+    from sklearn.metrics import root_mean_squared_error
     from sklearn.metrics import mean_squared_log_error
+    from sklearn.metrics import root_mean_squared_log_error
     from sklearn.metrics import mean_absolute_error
     from sklearn.metrics import mean_absolute_percentage_error
     
     MSE = mean_squared_error(
         y_true = y_true, 
-        y_pred = y_pred, 
-        squared = True
+        y_pred = y_pred
     )
     
-    RMSE = mean_squared_error(
+    RMSE = root_mean_squared_error(
         y_true = y_true, 
-        y_pred = y_pred, 
-        squared = False
+        y_pred = y_pred
     )
     
     minus_count = pd.Series(data = y_pred).lt(0).sum()
     
     if minus_count > 0:
         MSLE = None
         RMSLE = None
     else:
         MSLE = mean_squared_log_error(
             y_true = y_true, 
-            y_pred = y_pred, 
-            squared = True
+            y_pred = y_pred
         )
         
-        RMSLE = mean_squared_log_error(
+        RMSLE = root_mean_squared_log_error(
             y_true = y_true, 
-            y_pred = y_pred, 
-            squared = False
+            y_pred = y_pred
         )
     
     MAE = mean_absolute_error(
         y_true = y_true, 
         y_pred = y_pred
     )
     
@@ -664,17 +710,17 @@
         y: 목표변수 벡터를 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         X: 입력변수 행렬을 pd.DataFrame 또는 2차원 np.ndarray로 지정합니다.
         family: 목표변수의 확률분포를 지정합니다.
     
     반환:
         다중선형 회귀모형을 적합한 모형을 반환합니다.
     '''
-    import statsmodels.api as sa
+    import statsmodels.api as sma
     
-    model = sa.GLM(endog = y, exog = X, family = sa.families.Binomial())
+    model = sma.GLM(endog = y, exog = X, family = sma.families.Binomial())
     
     return model.fit()
 
 
 # 분류모형의 ROC 곡선 시각화 및 AUC 계산
 def roc_curve(
     y_true, 
@@ -719,28 +765,34 @@
     auc_ = auc(x = fpr, y = tpr)
     
     plt.plot(
         fpr, 
         tpr, 
         color = color, 
         label = f'AUC = {auc_:.4f}', 
-        lw = 1.0
+        linewidth = 1.0
     )
     
     plt.plot(
         [0, 1], 
         [0, 1], 
         color = 'k', 
-        linestyle = '--'
+        linestyle = '--', 
+        linewidth = 0.5
     )
     
-    plt.title(label = 'ROC Curve')
+    plt.title(label = 'ROC Curve', 
+              fontdict = {'fontweight': 'bold'})
+    
     plt.xlabel(xlabel = 'FPR')
+    
     plt.ylabel(ylabel = 'TPR')
-    plt.legend(loc = 'lower right');
+    
+    plt.legend(loc = 'lower right', 
+               fontsize = 8);
 
 
 # 분류모형의 RP 곡선 시각화 및 AP 계산
 def pr_curve(
     y_true, 
     y_prob, 
     pos = None, 
@@ -778,18 +830,23 @@
         y_true = trReal, 
         y_pred = trProb, 
         pos_label = pos, 
         # name = name, 
         color = color
     )
     
-    plt.title(label = 'PR Curve')
+    plt.title(label = 'PR Curve', 
+              fontdict = {'fontweight': 'bold'})
+    
     plt.xlabel(xlabel = 'Recall')
+    
     plt.ylabel(ylabel = 'Precision')
-    plt.legend(loc = 'best');
+    
+    plt.legend(loc = 'best', 
+               fontsize = 8);
 
 
 # 분류모형의 성능 지표(Confusion Matrix, F1 Score)
 def clfmetrics(y_true, y_pred):
     '''
     이 함수는 분류모형의 다양한 성능 지표를 계산합니다.
     
@@ -800,26 +857,31 @@
     반환:
         분류모형의 다양한 성능 지표를 출력합니다.
     '''
     import pandas as pd
     from sklearn.metrics import classification_report
     
     print('▶ Confusion Matrix')
+    
     cfm = pd.crosstab(
         index = y_pred, 
         columns = y_true, 
         margins = True
     )
+    
     cfm.index.name = 'Pred'
+    
     cfm.columns.name = 'Real'
+    
     display(cfm)
     
     print()
     
     print('▶ Classification Report')
+    
     print(
         classification_report(
             y_true = y_true, 
             y_pred = y_pred, 
             digits = 4
         )
     )
@@ -881,16 +943,17 @@
     result['Optimal'] = result['Sensitivity'] + result['Specificity']
     
     # TPR and FPR for ROC Curve.
     result['TPR'] = result['Sensitivity']
     result['FPR'] = 1 - result['Specificity']
     
     # Set Column name.
-    cols = ['Cutoff', 'Sensitivity', 'Specificity', 'Optimal', 'Precision', \
-            'TPR', 'FPR', 'MCC']
+    cols = ['Cutoff', 'Sensitivity', 'Specificity', 'Optimal', \
+            'Precision', 'TPR', 'FPR', 'MCC']
+    
     result = result[cols]
     
     return result
 
 
 # 최적의 분리 기준점 시각화
 def EpiROC(y_true, y_prob):
@@ -912,44 +975,49 @@
     # Draw ROC curve
     sns.lineplot(
         data = obj, 
         x = 'FPR', 
         y = 'TPR', 
         color = 'black'
     )
-    plt.title(label = '최적의 분리 기준점 탐색')
+    
+    plt.title(label = '최적의 분리 기준점 탐색', 
+              fontdict = {'fontweight': 'bold'})
     
     # Draw diagonal line
     plt.plot(
         [0, 1], 
         [0, 1], 
         color = '0.5', 
-        ls = '--'
+        linestyle = '--', 
+        linewidth = 0.5
     )
     
     # Add the Optimal Point
     opt = obj.iloc[[obj['Optimal'].argmax()]]
+    
     sns.scatterplot(
         data = opt, 
         x = 'FPR', 
         y = 'TPR', 
         color = 'red'
     )
     
     # Add tangent line
     optX = opt['FPR'].iloc[0]
     optY = opt['TPR'].iloc[0]
     
     b = optY - optX
+    
     plt.plot(
         [0, 1-b], 
         [b, 1], 
         color = 'red', 
-        lw = 0.5, 
-        ls = '-.'
+        linestyle = '-.', 
+        linewidth = 0.5
     )
     
     # Add text
     plt.text(
         x = opt['FPR'].values[0] - 0.01, 
         y = opt['TPR'].values[0] + 0.01, 
         s = f"Cutoff = {opt['Cutoff'].round(2).values[0]}",
```

### Comparing `hds-stats-0.3.8/setup.py` & `hds_stats-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.3.8',
+    version = '0.4.0',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
-    description = 'Useful functions for Statistics and Machine Learning',
+    description = 'Useful functions for EDA, Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     
     url = 'https://github.com/HelloDataScience/hds-stats',
     project_urls = {
         'Bug Tracker': 'https://github.com/HelloDataScience/hds-stats/issues',
     },
@@ -25,15 +25,15 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     
     python_requires = '>=3.9',
     packages = find_packages(),
     package_dir = {'hds_stats': 'hds_stats'},
-    py_modules = ['plot', 'stat'],
+    py_modules = ['plot', 'stat', 'ml'],
     install_requires = [
         'numpy', 
         'pandas', 
         'scipy', 
         'seaborn', 
         'matplotlib', 
         'statsmodels',
```

