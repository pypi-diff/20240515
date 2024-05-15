# Comparing `tmp/CTG_Utils-1.1.2.tar.gz` & `tmp/CTG_Utils-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTG_Utils-1.1.2.tar", last modified: Mon May 13 07:54:24 2024, max compression
+gzip compressed data, was "CTG_Utils-1.1.3.tar", last modified: Tue May 14 14:57:18 2024, max compression
```

## Comparing `CTG_Utils-1.1.2.tar` & `CTG_Utils-1.1.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:54:24.633921 CTG_Utils-1.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-13 07:54:24.585146 CTG_Utils-1.1.2/CTG_Utils/
-drwxrwxrwx   0        0        0        0 2024-05-13 07:54:24.601106 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/
--rw-rw-rw-   0        0        0     6530 2024-05-12 12:12:01.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTGClasses.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:54:24.609084 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/
--rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
--rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
--rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
--rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
--rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
--rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
--rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
--rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
--rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
--rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_config.py
--rw-rw-rw-   0        0        0    19138 2024-05-13 07:46:15.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_effectif.py
--rw-rw-rw-   0        0        0    11461 2024-05-12 12:33:31.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_plot.py
--rw-rw-rw-   0        0        0    15877 2024-05-12 15:37:19.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_synthese.py
--rw-rw-rw-   0        0        0     4645 2024-05-10 17:35:42.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_utility.py
--rw-rw-rw-   0        0        0      191 2024-05-12 12:09:52.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_Func/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:54:24.632892 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/
--rw-rw-rw-   0        0        0    16023 2024-05-13 07:39:52.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/GUI_Globals.py
--rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageDivers.py
--rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageEffectif.py
--rw-rw-rw-   0        0        0    11622 2024-05-12 11:11:49.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageSorties.py
--rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageSynthese.py
--rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageTendance.py
--rw-rw-rw-   0        0        0    30344 2024-05-10 07:03:45.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/Page_Classes.py
--rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/Useful_Classes.py
--rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/Useful_Functions.py
--rw-rw-rw-   0        0        0      198 2024-05-10 17:28:54.000000 CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:54:24.593128 CTG_Utils-1.1.2/CTG_Utils.egg-info/
--rw-rw-rw-   0        0        0      681 2024-05-13 07:54:23.000000 CTG_Utils-1.1.2/CTG_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2024-05-13 07:54:23.000000 CTG_Utils-1.1.2/CTG_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:54:23.000000 CTG_Utils-1.1.2/CTG_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-13 07:54:23.000000 CTG_Utils-1.1.2/CTG_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-05-13 07:54:23.000000 CTG_Utils-1.1.2/CTG_Utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.2/LICENSE
--rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      681 2024-05-13 07:54:24.633921 CTG_Utils-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 07:54:24.633921 CTG_Utils-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1367 2024-05-13 07:51:44.000000 CTG_Utils-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:57:18.778475 CTG_Utils-1.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-14 14:57:18.667249 CTG_Utils-1.1.3/CTG_Utils/
+drwxrwxrwx   0        0        0        0 2024-05-14 14:57:18.715122 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/
+-rw-rw-rw-   0        0        0     6861 2024-05-14 14:48:11.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTGClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:57:18.733073 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/
+-rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
+-rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
+-rw-rw-rw-   0        0        0     1355 2024-05-14 14:24:59.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
+-rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
+-rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
+-rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
+-rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
+-rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
+-rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
+-rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
+-rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_config.py
+-rw-rw-rw-   0        0        0    19138 2024-05-13 07:46:15.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_effectif.py
+-rw-rw-rw-   0        0        0    11461 2024-05-12 12:33:31.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_plot.py
+-rw-rw-rw-   0        0        0    15877 2024-05-12 15:37:19.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_synthese.py
+-rw-rw-rw-   0        0        0     4645 2024-05-10 17:35:42.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_utility.py
+-rw-rw-rw-   0        0        0      191 2024-05-12 12:09:52.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_Func/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:57:18.774485 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/
+-rw-rw-rw-   0        0        0    16064 2024-05-14 08:52:29.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/GUI_Globals.py
+-rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageDivers.py
+-rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageEffectif.py
+-rw-rw-rw-   0        0        0    11622 2024-05-12 11:11:49.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageSorties.py
+-rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageSynthese.py
+-rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageTendance.py
+-rw-rw-rw-   0        0        0    32691 2024-05-14 14:19:21.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/Page_Classes.py
+-rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/Useful_Classes.py
+-rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/Useful_Functions.py
+-rw-rw-rw-   0        0        0      198 2024-05-10 17:28:54.000000 CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:57:18.701158 CTG_Utils-1.1.3/CTG_Utils.egg-info/
+-rw-rw-rw-   0        0        0      681 2024-05-14 14:57:17.000000 CTG_Utils-1.1.3/CTG_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1256 2024-05-14 14:57:17.000000 CTG_Utils-1.1.3/CTG_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 14:57:17.000000 CTG_Utils-1.1.3/CTG_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-14 14:57:17.000000 CTG_Utils-1.1.3/CTG_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-14 14:57:17.000000 CTG_Utils-1.1.3/CTG_Utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      681 2024-05-14 14:57:18.777479 CTG_Utils-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 14:57:18.778475 CTG_Utils-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2024-05-14 14:56:27.000000 CTG_Utils-1.1.3/setup.py
```

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTGClasses.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTGClasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,22 +49,25 @@
         dist = 2 * rad * asin(sqrt(sin((phi2 - phi1) / 2) ** 2
                                  + cos(phi1) * cos(phi2) * sin((lon2 - lon1) / 2) ** 2))
         return np.round(dist,1)
     
     def stat(self):
     
         # Standard library imports
+        from pathlib import Path
         from tkinter import messagebox
         
         # Internal imports
         from CTG_Utils.CTG_Func.CTG_utility import read_correction_effectifs
 
         da = self.effectif.groupby('Sexe')['Age'].agg(['count','median','max','min'])
         res = self.effectif['Age'].agg(['count','median','max','min']).tolist()
         stat = []
+        stat.append(f"Année : {self.year}")
+        stat.append(" ")
         nbr_membres = round(res[0],0)
         stat.append(f"Nombre d'adhérents : {nbr_membres}")
         nbr_femmes = da.loc['F','count']
         stat.append(f"Nombre de femmes : {nbr_femmes} ({round(100*nbr_femmes/nbr_membres,1)} %)")
         nbr_hommes = da.loc['M','count']
         stat.append(f"Nombre d'hommes : {nbr_hommes} ({round(100*nbr_hommes/nbr_membres,1)} %)")
         stat.append(' ')
@@ -112,14 +115,19 @@
         self.effectif = self.effectif.rename(columns={'\n\t\t\t\tAbonnements':'Abonnements'})
         nbr_abonnements = len(self.effectif.query('Abonnements == "Oui"'))
         stat.append(f"Nombre d'abonnés à la revue FFCT : {nbr_abonnements} ({round(100*nbr_abonnements/nbr_membres)} %)")
         
         stat ='\n'.join(stat)
         messagebox.showinfo(f'Statistique {self.year}',stat)
         
+        path_info_effectif = self.ctg_path / Path(str(self.year)) / Path('STATISTIQUES')/Path(f'info_effectif_{self.year}.txt')
+        with open(path_info_effectif,'w') as f:
+            f.write(stat)
+        
+        
     def plot_histo(self):
     
         # Third party imports
         import matplotlib.pyplot as plt
         import pandas as pd
         
         fig, ax = plt.subplots(figsize=(10,10))
```

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_effectif.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_effectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_plot.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_plot.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_synthese.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_synthese.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_Func/CTG_utility.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_Func/CTG_utility.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/GUI_Globals.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/GUI_Globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,15 @@
 # Setting label for each gui page
 PAGES_LABELS = {'PageEffectif': "Analyse des effectifs",
                 'PageSorties' : "Analyse des sorties",
                 'PageSynthese': "Synthèse des sorties et effectifs",
                 'PageTendance': "Analyse de l'évolution temporelle des pratiques ",
                 'PageTendance': "Analyse tendancielle",
                 'PageDivers'  : "Autres analyses",
+                'PageHelp'    : "Aide",
                }
 
 
 ########################## Cover Page (BiblioMeter launching Page) ##########################
 
 # Titre de la page
 TEXT_TITLE                  = "- CTG_Meter -\nInitialisation de l'analyse"
```

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageDivers.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageDivers.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageEffectif.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageEffectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageSorties.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageSorties.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageSynthese.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageSynthese.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/PageTendance.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/PageTendance.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/Page_Classes.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/Page_Classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         # 3rd party imports
         from screeninfo import get_monitors
         
         # Local imports
         from CTG_Utils.CTG_GUI.Useful_Functions import window_properties
         import CTG_Utils.CTG_GUI.GUI_Globals as gg
         
+        ctg_path_default = Path.home() /Path('CTG/SORTIES')
+        
         # Setting the link with "tk.Tk"
         tk.Tk.__init__(master)
 
   
         # Identifying tk window of init class   
         _ = get_monitors() # OBLIGATOIRE        
         master.attributes("-topmost", True)
@@ -45,15 +47,16 @@
         win_width_px  = sizes_tuple[0]
         win_height_px = sizes_tuple[1]
         
         master.geometry(f"{win_width_px}x{win_height_px}")
         master.resizable(False, False)           
         
         # Defining pages classes and pages list
-        AppMain.pages = ( PageDivers,
+        AppMain.pages = ( PageHelp,
+                          PageDivers,
                           PageTendance,
                           PageSynthese,
                           PageEffectif,
                           PageSorties,                     
                          )
         AppMain.pages_ordered_list = [x.__name__ for x in AppMain.pages][::-1]
         
@@ -67,16 +70,15 @@
         AppMain.width_sf_min  = min(AppMain.width_sf_mm, AppMain.width_sf_px)
                  
         
         ######################################## Title and copyright and application initialization                       
         PageTitle(master)    
         AuthorCopyright(master)
         InitApp(master)
-        SetLaunchButton(master, "CTG", r"c:\users\franc\CTG")
-        #InitApp(master)        
+        SetLaunchButton(master, "CTG", ctg_path_default)        
                               
         
     ################################ Class init - end ################################
     
 class InitApp(tk.Tk):
 
     def __init__(self,master):
@@ -227,15 +229,15 @@
                 # Setting corpi_val value to empty string
                 corpi_val.set("")                                       
                 
         def _update_page():
             from pathlib import Path
 
             institute_select = 'CTG'
-            inst_default_bmf = Path.home() / Path('CTG') 
+            inst_default_bmf = Path.home() / Path('CTG/SORTIES') 
             
             # Managing working folder (bmf stands for "BiblioMeter_Files") 
             _set_bmf_widget_param(institute_select, inst_default_bmf)
             
             # Managing corpus list
             corpi_val = _set_corpi_widgets_param(inst_default_bmf)            
                 # Setting and displating corpuses list initial values
@@ -552,15 +554,66 @@
         create_divers_analysis(self, master, page_name, institute, ctg_path)
         
         setcontrollerbutton = SetControllerButton(master, container_button,page_name)
         
         settitleclass = SetTitltleClass(self,page_name,institute)
         
         quitapp = QuitApp(self, master, container_button)
+
+class PageHelp(tk.Frame):
+    '''PAGE 5 'Analyse des corpus'.
+    '''
+    def __init__(self, container_frame, master, container_button, institute, ctg_path):
+    
+        # Standard library import imports
+        from pathlib import Path
+        
+        # Internal imports
+        import CTG_Utils.CTG_GUI.GUI_Globals as gg
+        from CTG_Utils.CTG_GUI.Useful_Functions import mm_to_px
+        from CTG_Utils.CTG_GUI.Useful_Functions import place_after
+        from CTG_Utils.CTG_GUI.Useful_Functions import place_bellow
+        
+        if_analysis_x_pos_px     = mm_to_px(10 * AppMain.width_sf_mm,  gg.PPI)
+        if_analysis_y_pos_px     = mm_to_px(10 * AppMain.height_sf_mm, gg.PPI)  
+        
+        super().__init__(container_frame)
+
+        page_name  = self.__class__.__name__
+        
+        help_box = tk.Text(self,
+                           width=90,
+                           height=30,
+                           highlightthickness=1, 
+                           foreground="black",
+                           insertbackground="black",
+                           font=("Helvetica", 8))
+                           
+        help_box.place(x = if_analysis_x_pos_px, y = if_analysis_y_pos_px)
+        
+        tex_scroll_y = tk.Scrollbar(self,orient=tk.VERTICAL,)
+        tex_scroll_y.config(command=help_box.yview, )
+        help_box["yscrollcommand"] = tex_scroll_y.set
+        place_after(help_box, tex_scroll_y, dx = 5, dy = 0)
+        
+        #tex_scroll_x = tk.Scrollbar(orient=tk.HORIZONTAL,)
+        #tex_scroll_x.config(command=help_box.xview, )
+        #help_box["yscrollcommand"] = tex_scroll_x.set
+        #place_bellow(help_box, tex_scroll_x, dx = 0, dy = 5)
+        
+        path_help = Path(__file__).parent.parent / Path('CTG_Func') / Path('CTG_RefFiles') / Path( 'help.txt')
+        with open(path_help,'r',encoding="utf-8")as file_text:
+            help_content =  file_text.read() 
+        help_box.insert(tk.END,help_content)         
+        
+        setcontrollerbutton = SetControllerButton(master, container_button,page_name)
+        
+        #settitleclass = SetTitltleClass(self,page_name,institute)
         
+        quitapp = QuitApp(self, master, container_button)        
         
 class SetControllerButton(tk.Tk):
 
     def __init__(self, master, container_button,page_name):
         # Standard library imports
         from tkinter import font as tkFont
```

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/Useful_Classes.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/Useful_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils/CTG_GUI/Useful_Functions.py` & `CTG_Utils-1.1.3/CTG_Utils/CTG_GUI/Useful_Functions.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/CTG_Utils.egg-info/PKG-INFO` & `CTG_Utils-1.1.3/CTG_Utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG-Utils
-Version: 1.1.2
+Version: 1.1.3
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.2/CTG_Utils.egg-info/SOURCES.txt` & `CTG_Utils-1.1.3/CTG_Utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 CTG_Utils/CTG_Func/CTG_effectif.py
 CTG_Utils/CTG_Func/CTG_plot.py
 CTG_Utils/CTG_Func/CTG_synthese.py
 CTG_Utils/CTG_Func/CTG_utility.py
 CTG_Utils/CTG_Func/__init__.py
 CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
 CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
+CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
 CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
 CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
 CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
 CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
 CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
 CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
 CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
```

### Comparing `CTG_Utils-1.1.2/LICENSE` & `CTG_Utils-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.2/PKG-INFO` & `CTG_Utils-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG_Utils
-Version: 1.1.2
+Version: 1.1.3
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.2/setup.py` & `CTG_Utils-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 install_requires = open(path.join(this_directory, 'requirements.txt'), encoding='utf-8').read().strip().split('\n') 
 
 # This setup is suitable for "python setup.py develop".
 
 setup(name='CTG_Utils',
-      version='1.1.2',
+      version='1.1.3',
       description='A toolbox for ctg statistics analysis',
       long_description=long_description,
       long_description_content_type='text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
```

