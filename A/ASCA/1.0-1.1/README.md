# Comparing `tmp/ASCA-1.0.tar.gz` & `tmp/ASCA-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCA-1.0.tar", last modified: Tue Dec  6 09:35:57 2022, max compression
+gzip compressed data, was "ASCA-1.1.tar", last modified: Wed May 15 15:52:40 2024, max compression
```

## Comparing `ASCA-1.0.tar` & `ASCA-1.1.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-12-06 09:35:57.340902 ASCA-1.0/
-drwxrwxrwx   0        0        0        0 2022-12-06 09:35:57.321905 ASCA-1.0/ASCA/
--rw-rw-rw-   0        0        0    15344 2022-12-06 09:21:21.000000 ASCA-1.0/ASCA/ASCA.py
--rw-rw-rw-   0        0        0        0 2022-06-26 12:56:39.000000 ASCA-1.0/ASCA/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 09:35:57.338902 ASCA-1.0/ASCA.egg-info/
--rw-rw-rw-   0        0        0     4227 2022-12-06 09:35:57.000000 ASCA-1.0/ASCA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2022-12-06 09:35:57.000000 ASCA-1.0/ASCA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-06 09:35:57.000000 ASCA-1.0/ASCA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-12-06 09:35:57.000000 ASCA-1.0/ASCA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-12-06 09:35:57.000000 ASCA-1.0/ASCA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1326 2022-12-06 09:33:45.000000 ASCA-1.0/LICENSE
--rw-rw-rw-   0        0        0     4227 2022-12-06 09:35:57.340902 ASCA-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3465 2022-12-06 09:33:45.000000 ASCA-1.0/README.md
--rw-rw-rw-   0        0        0       86 2022-12-06 09:35:57.342903 ASCA-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1385 2022-12-06 09:06:39.000000 ASCA-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:52:40.556137 ASCA-1.1/
+-rw-rw-rw-   0        0        0     1712 2022-03-03 12:05:02.000000 ASCA-1.1/.gitignore
+-rw-rw-rw-   0        0        0      214 2022-03-03 12:05:02.000000 ASCA-1.1/.travis.yml
+drwxrwxrwx   0        0        0        0 2024-05-15 15:52:40.500140 ASCA-1.1/ASCA/
+-rw-rw-rw-   0        0        0    15440 2024-05-15 15:49:52.000000 ASCA-1.1/ASCA/ASCA.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:49:52.000000 ASCA-1.1/ASCA/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:52:40.535139 ASCA-1.1/ASCA.egg-info/
+-rw-rw-rw-   0        0        0     4279 2024-05-15 15:52:39.000000 ASCA-1.1/ASCA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-15 15:52:40.000000 ASCA-1.1/ASCA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:52:39.000000 ASCA-1.1/ASCA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-15 15:52:39.000000 ASCA-1.1/ASCA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 15:52:39.000000 ASCA-1.1/ASCA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      306 2024-05-15 15:49:52.000000 ASCA-1.1/CITATION.cff
+-rw-rw-rw-   0        0        0     1326 2022-12-06 09:33:45.000000 ASCA-1.1/LICENSE
+-rw-rw-rw-   0        0        0     4279 2024-05-15 15:52:40.555156 ASCA-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3465 2022-12-06 09:33:45.000000 ASCA-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 15:52:40.551137 ASCA-1.1/examples/
+-rw-rw-rw-   0        0        0    98170 2024-05-15 15:49:52.000000 ASCA-1.1/examples/ASCA_Example.ipynb
+-rw-rw-rw-   0        0        0       30 2022-12-06 09:07:38.000000 ASCA-1.1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-05-15 15:52:40.560143 ASCA-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1385 2024-05-15 15:50:33.000000 ASCA-1.1/setup.py
```

### Comparing `ASCA-1.0/ASCA/ASCA.py` & `ASCA-1.1/ASCA/ASCA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from sklearn.base import TransformerMixin, RegressorMixin, BaseEstimator
 import matplotlib.pyplot as plt
 from matplotlib.markers import MarkerStyle
 import matplotlib.cm as cm
 from scipy.spatial import ConvexHull
 import math
+import itertools
 class ASCA(BaseEstimator):
     def __init__(self):
         self.__name__='ASCA'
         
         #Default
         self.factors=None
         self.interactions=None
@@ -128,38 +129,39 @@
         
         #Calculate Effects
         X_effect=[]        
         for effect in range(F.shape[1]):
           X_effect.append(np.zeros_like(Xm))
           for f in factor_set:
               select=F[:,effect]==f
-              select_mat=np.where([select,select],Xm.T,zero.T).T
+              select_mat=np.where([select]*Xm.T.shape[0],Xm.T,zero.T).T
               select_avg=np.sum(select_mat,axis=0)/(sum(select)+np.finfo(float).eps) #average avoiding empty entry
               select_mat[select_mat.nonzero()]=1 #set all as 1
               X_effect[effect]=X_effect[effect]+select_mat*select_avg
         
         #Sum the effects
         Total_effect=[]
         for Xe in X_effect:
             if len(Total_effect)==0:
                 Total_effect=Xe
             else:
                 Total_effect=Total_effect+Xe    
         
         #Calculate Interactions
         X_interact=[]
+
+        combination_factor_set=list(itertools.combinations(list(factor_set), F.shape[0]))
         for inter in range(len(interactions)):
           X_interact.append(np.zeros_like(Xm))
-          for f1 in factor_set:
-            for f2 in factor_set:
-              select=np.sum(F==[f1,f2],axis=1)==2
-              select_mat=np.where([select,select],Xm.T,zero.T).T
-              select_avg=np.sum(select_mat,axis=0)/(sum(select)+np.finfo(float).eps) #average avoiding empty entry
-              select_mat[select_mat.nonzero()]=1 #set all as 1
-              X_interact[inter]=X_interact[inter]+select_mat*select_avg-select_mat*Total_effect
+          for ff in combination_factor_set:
+            select=np.sum(F==list(ff),axis=1)==F.shape[0]
+            select_mat=np.where([select]*Xm.T.shape[0],Xm.T,zero.T).T
+            select_avg=np.sum(select_mat,axis=0)/(sum(select)+np.finfo(float).eps) #average avoiding empty entry
+            select_mat[select_mat.nonzero()]=1 #set all as 1
+            X_interact[inter]=X_interact[inter]+select_mat*select_avg-select_mat*Total_effect
               
         #Sum the Interactions
         Total_interact=[]
         for Xi in X_interact:
             if len(Total_interact)==0:
                 Total_interact=Xi
             else:
@@ -225,15 +227,15 @@
             x = np.arange(len(labels))
             width = 0.2
             my_cmap=list(plt.get_cmap("Set1").colors)
             rects1 = ax[1].bar(x - width/2-0.01, first_loading, width, label='First Loading',color=my_cmap[0])
             rects2 = ax[1].bar(x + width/2+0.01, second_loading, width, label='Second Loading',color=my_cmap[1])
             ax[1].hlines(y=0, xmin=0- width-0.05, xmax=len(labels)-1 + width+0.01*5, linewidth=0.5,linestyles='--', color='black')
             ax[1].set_ylabel('Value')
-            ax[1].set_title('Loading for Interaction '+ str(ii+1))
+            ax[1].set_title('Loading for Factor '+ str(ii+1))
             ax[1].set_xticks(x, labels)
             ax[1].legend()
             plt.tight_layout()
             plt.show()
         
     def plot_factors(self):
         for ii in range(len(self.factors_scores)):
@@ -359,15 +361,15 @@
     F=np.asarray(F)
     interactions = [[0, 1]]
 
     ASCA=ASCA()
     ASCA.fit(X,F,interactions)
     ASCA.plot_factors()
     ASCA.plot_interactions()
-    #ASCA.plot_factors_biplot()
+    ASCA.plot_factors_biplot()
     #print(ASCA.factors_scores)
     #print(ASCA.factors_loadings)
     #print(ASCA.factors_projected)
     #ang=math.radians(90)
     #A=np.asarray([[math.cos(ang),-math.sin(ang)],[math.sin(ang),math.cos(ang)]])
     #print([ f@A for f  in ASCA.factors_loadings])
     '''
```

### Comparing `ASCA-1.0/ASCA.egg-info/PKG-INFO` & `ASCA-1.1/ASCA.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: ASCA
-Version: 1.0
+Version: 1.1
 Summary: ASCA: ANOVA-simultaneous component analysis
-Home-page: UNKNOWN
 Author: Sin Yong Teng
 Author-email: tsyet12@gmail.com
 License: BSD 2-Clause
 Keywords: Design of Experiments,Chemometrics,Artificial Intelligence
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: sklearn
+Requires-Dist: numpy
 
 # ASCA: ANOVA-Simultaneous Component Analysis in Python
 
 
 <!-- TABLE OF CONTENTS -->
 ## Table of Contents
 
@@ -132,9 +134,7 @@
 Smilde, Age K., et al. "ANOVA-simultaneous component analysis (ASCA): a new tool for analyzing designed metabolomics data." Bioinformatics 21.13 (2005): 3043-3048.
 
 Jansen, Jeroen J., et al. "ASCA: analysis of multivariate data obtained from an experimental design." Journal of Chemometrics: A Journal of the Chemometrics Society 19.9 (2005): 469-481.
 
 
 ## Acknowledgements
 The research contribution from S.Y. Teng is supported by the European Union's Horizon Europe Research and Innovation Program, under Marie Skłodowska-Curie Actions grant agreement no. 101064585 (MoCEGS).
-
-
```

### Comparing `ASCA-1.0/LICENSE` & `ASCA-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ASCA-1.0/PKG-INFO` & `ASCA-1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: ASCA
-Version: 1.0
+Version: 1.1
 Summary: ASCA: ANOVA-simultaneous component analysis
-Home-page: UNKNOWN
 Author: Sin Yong Teng
 Author-email: tsyet12@gmail.com
 License: BSD 2-Clause
 Keywords: Design of Experiments,Chemometrics,Artificial Intelligence
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: sklearn
+Requires-Dist: numpy
 
 # ASCA: ANOVA-Simultaneous Component Analysis in Python
 
 
 <!-- TABLE OF CONTENTS -->
 ## Table of Contents
 
@@ -132,9 +134,7 @@
 Smilde, Age K., et al. "ANOVA-simultaneous component analysis (ASCA): a new tool for analyzing designed metabolomics data." Bioinformatics 21.13 (2005): 3043-3048.
 
 Jansen, Jeroen J., et al. "ASCA: analysis of multivariate data obtained from an experimental design." Journal of Chemometrics: A Journal of the Chemometrics Society 19.9 (2005): 469-481.
 
 
 ## Acknowledgements
 The research contribution from S.Y. Teng is supported by the European Union's Horizon Europe Research and Innovation Program, under Marie Skłodowska-Curie Actions grant agreement no. 101064585 (MoCEGS).
-
-
```

### Comparing `ASCA-1.0/README.md` & `ASCA-1.1/README.md`

 * *Files identical despite different names*

### Comparing `ASCA-1.0/setup.py` & `ASCA-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = [] 
 if os.path.isfile(requirementPath):
     with open(requirementPath) as f:
         install_requires = f.read().splitlines()
 
 
 setup(name='ASCA', 
-version='1.0', 
+version='1.1', 
 license='BSD 2-Clause',
 description="ASCA: ANOVA-simultaneous component analysis",
 author='Sin Yong Teng',
 long_description=long_description,
 long_description_content_type="text/markdown",
 author_email='tsyet12@gmail.com',
 keywords = ['Design of Experiments','Chemometrics','Artificial Intelligence'],
```

