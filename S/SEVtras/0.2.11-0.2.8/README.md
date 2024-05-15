# Comparing `tmp/SEVtras-0.2.11.tar.gz` & `tmp/SEVtras-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SEVtras-0.2.11.tar", last modified: Wed May 15 11:29:45 2024, max compression
+gzip compressed data, was "dist/SEVtras-0.2.8.tar", last modified: Fri Dec  8 18:17:33 2023, max compression
```

## Comparing `SEVtras-0.2.11.tar` & `SEVtras-0.2.8.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxr-x   0 heruiqiao   (600) heruiqiao   (606)        0 2024-05-15 11:31:44.000000 SEVtras-0.2.11/
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)    35184 2023-12-03 14:29:52.000000 SEVtras-0.2.11/LICENSE
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)      233 2024-05-15 11:24:26.000000 SEVtras-0.2.11/MANIFEST.in
--rw-r--r--   0 heruiqiao   (600) heruiqiao   (606)     3226 2024-05-15 11:29:45.000000 SEVtras-0.2.11/PKG-INFO
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)     2357 2023-12-02 14:09:10.000000 SEVtras-0.2.11/README.md
-drwxrwxr-x   0 heruiqiao   (600) heruiqiao   (606)        0 2024-05-15 11:31:43.000000 SEVtras-0.2.11/SEVtras/
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)      289 2023-12-08 17:31:02.000000 SEVtras-0.2.11/SEVtras/__init__.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)     2213 2023-11-10 07:37:24.000000 SEVtras-0.2.11/SEVtras/_docs.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)      690 2022-11-10 06:50:04.000000 SEVtras-0.2.11/SEVtras/env.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)      171 2023-07-06 07:31:48.000000 SEVtras-0.2.11/SEVtras/evs.gmt
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)      166 2024-04-25 08:30:00.000000 SEVtras-0.2.11/SEVtras/evsM.gmt
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)    13652 2024-05-14 07:43:16.000000 SEVtras-0.2.11/SEVtras/functional.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)    13453 2023-07-06 07:31:22.000000 SEVtras-0.2.11/SEVtras/id_homo_rna_ev
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)     5878 2023-07-06 07:31:26.000000 SEVtras-0.2.11/SEVtras/id_mus_rna_ev
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)    10797 2024-05-14 07:44:20.000000 SEVtras-0.2.11/SEVtras/main.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)   170216 2023-12-08 14:45:46.000000 SEVtras-0.2.11/SEVtras/sc_pp.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)    38594 2023-12-08 05:25:24.000000 SEVtras-0.2.11/SEVtras/sc_readwrite.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)    28360 2023-12-03 02:08:58.000000 SEVtras-0.2.11/SEVtras/sc_utils.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)     9467 2024-04-24 07:50:04.000000 SEVtras-0.2.11/SEVtras/utils.py
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)       23 2024-05-15 11:29:18.000000 SEVtras-0.2.11/SEVtras/version.py
-drwxrwxr-x   0 heruiqiao   (600) heruiqiao   (606)        0 2024-05-15 11:31:43.000000 SEVtras-0.2.11/SEVtras.egg-info/
--rw-r--r--   0 heruiqiao   (600) heruiqiao   (606)     3226 2024-05-15 11:29:44.000000 SEVtras-0.2.11/SEVtras.egg-info/PKG-INFO
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)      643 2024-05-15 11:29:44.000000 SEVtras-0.2.11/SEVtras.egg-info/SOURCES.txt
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)        1 2024-05-15 11:29:44.000000 SEVtras-0.2.11/SEVtras.egg-info/dependency_links.txt
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)       57 2024-05-15 11:29:44.000000 SEVtras-0.2.11/SEVtras.egg-info/entry_points.txt
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)      109 2024-05-15 11:29:44.000000 SEVtras-0.2.11/SEVtras.egg-info/requires.txt
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)        8 2024-05-15 11:29:44.000000 SEVtras-0.2.11/SEVtras.egg-info/top_level.txt
-drwxrwxr-x   0 heruiqiao   (600) heruiqiao   (606)        0 2024-05-15 11:31:43.000000 SEVtras-0.2.11/docs/
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)   118473 2023-12-01 01:49:32.000000 SEVtras-0.2.11/docs/Part1.png
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)   273002 2023-12-01 07:25:46.000000 SEVtras-0.2.11/docs/Part2.png
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)   167774 2023-12-04 00:36:38.000000 SEVtras-0.2.11/docs/SEVtras_overview.png
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)       38 2024-05-15 11:29:45.000000 SEVtras-0.2.11/setup.cfg
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)     1390 2024-05-15 11:28:55.000000 SEVtras-0.2.11/setup.py
-drwxrwxr-x   0 heruiqiao   (600) heruiqiao   (606)        0 2024-05-15 11:31:44.000000 SEVtras-0.2.11/tests/
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)   148840 2023-12-08 16:19:22.000000 SEVtras-0.2.11/tests/sEV_SEVtras.h5ad
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)       22 2022-11-10 11:32:56.000000 SEVtras-0.2.11/tests/sample_file
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)  4271792 2022-11-10 14:39:04.000000 SEVtras-0.2.11/tests/test1.h5ad
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)  4296880 2023-12-03 13:30:14.000000 SEVtras-0.2.11/tests/test2.h5ad
--rw-rw-r--   0 heruiqiao   (600) heruiqiao   (606)  9978672 2023-12-03 04:31:02.000000 SEVtras-0.2.11/tests/test_cell.h5ad
+drwxr-xr-x   0 heruiqiao   (600) zhao       (541)        0 2023-12-08 18:17:40.000000 SEVtras-0.2.8/
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)    35184 2023-12-08 18:17:32.000000 SEVtras-0.2.8/LICENSE
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)      205 2023-12-08 18:17:32.000000 SEVtras-0.2.8/MANIFEST.in
+-rw-r--r--   0 heruiqiao   (600) zhao       (541)     3225 2023-12-08 18:17:33.000000 SEVtras-0.2.8/PKG-INFO
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)     2357 2023-12-08 18:17:32.000000 SEVtras-0.2.8/README.md
+drwxr-xr-x   0 heruiqiao   (600) zhao       (541)        0 2023-12-08 18:17:40.000000 SEVtras-0.2.8/SEVtras/
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)      289 2023-12-08 17:31:02.000000 SEVtras-0.2.8/SEVtras/__init__.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)     2213 2023-11-10 07:37:24.000000 SEVtras-0.2.8/SEVtras/_docs.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)      690 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras/env.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)      171 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras/evs.gmt
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)    13500 2023-12-04 00:35:54.000000 SEVtras-0.2.8/SEVtras/functional.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)    13453 2023-07-06 07:31:22.000000 SEVtras-0.2.8/SEVtras/id_homo_rna_ev
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)     5878 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras/id_mus_rna_ev
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)    10729 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras/main.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)   170216 2023-12-08 14:45:46.000000 SEVtras-0.2.8/SEVtras/sc_pp.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)    38594 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras/sc_readwrite.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)    28360 2023-12-03 02:08:58.000000 SEVtras-0.2.8/SEVtras/sc_utils.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)     9467 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras/utils.py
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)       22 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras/version.py
+drwxr-xr-x   0 heruiqiao   (600) zhao       (541)        0 2023-12-08 18:17:40.000000 SEVtras-0.2.8/SEVtras.egg-info/
+-rw-r--r--   0 heruiqiao   (600) zhao       (541)     3225 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras.egg-info/PKG-INFO
+-rw-r--r--   0 heruiqiao   (600) zhao       (541)      626 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras.egg-info/SOURCES.txt
+-rw-r--r--   0 heruiqiao   (600) zhao       (541)        1 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras.egg-info/dependency_links.txt
+-rw-r--r--   0 heruiqiao   (600) zhao       (541)       57 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras.egg-info/entry_points.txt
+-rw-r--r--   0 heruiqiao   (600) zhao       (541)      109 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras.egg-info/requires.txt
+-rw-r--r--   0 heruiqiao   (600) zhao       (541)        8 2023-12-08 18:17:32.000000 SEVtras-0.2.8/SEVtras.egg-info/top_level.txt
+drwxr-xr-x   0 heruiqiao   (600) zhao       (541)        0 2023-12-08 18:17:40.000000 SEVtras-0.2.8/docs/
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)   118473 2023-12-01 01:49:32.000000 SEVtras-0.2.8/docs/Part1.png
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)   273002 2023-12-01 07:25:46.000000 SEVtras-0.2.8/docs/Part2.png
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)   167774 2023-12-04 00:36:38.000000 SEVtras-0.2.8/docs/SEVtras_overview.png
+-rw-r--r--   0 heruiqiao   (600) zhao       (541)       38 2023-12-08 18:17:33.000000 SEVtras-0.2.8/setup.cfg
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)     1389 2023-12-08 17:32:20.000000 SEVtras-0.2.8/setup.py
+drwxr-xr-x   0 heruiqiao   (600) zhao       (541)        0 2023-12-08 18:17:40.000000 SEVtras-0.2.8/tests/
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)   148840 2023-12-08 18:17:32.000000 SEVtras-0.2.8/tests/sEV_SEVtras.h5ad
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)       22 2023-12-08 18:17:32.000000 SEVtras-0.2.8/tests/sample_file
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)  4271792 2022-11-10 14:39:04.000000 SEVtras-0.2.8/tests/test1.h5ad
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)  4296880 2023-12-03 13:30:14.000000 SEVtras-0.2.8/tests/test2.h5ad
+-rw-rw-r--   0 heruiqiao   (600) zhao       (541)  9978672 2023-12-03 04:31:02.000000 SEVtras-0.2.8/tests/test_cell.h5ad
```

### Comparing `SEVtras-0.2.11/LICENSE` & `SEVtras-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/PKG-INFO` & `SEVtras-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SEVtras
-Version: 0.2.11
+Version: 0.2.8
 Summary: sEV-containing droplet identification in scRNA-seq data
 Home-page: http://pypi.python.org/pypi/SEVtras/
 Author: Ruiqiao He
 Author-email: ruiqiaohe@gmail.com
 License: GPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `SEVtras-0.2.11/README.md` & `SEVtras-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras/_docs.py` & `SEVtras-0.2.8/SEVtras/_docs.py`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras/env.py` & `SEVtras-0.2.8/SEVtras/env.py`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras/functional.py` & `SEVtras-0.2.8/SEVtras/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import copy
 import sys
 import os
 import pickle
 # from pathlib import Path
 from os import path
 
-def source_biogenesis(adata_cell, species, OBScelltype='celltype', Xraw = True, normalW=True):
+def source_biogenesis(adata_cell, OBScelltype='celltype', Xraw = True, normalW=True):
     if Xraw:
         X_input = adata_cell.raw
     else:
         X_input = adata_cell
         
     if normalW:
         try:
@@ -26,18 +26,15 @@
             X_norm = scale(X_input.X, zero_center=True, max_value=None, copy=False)
     else:
         X_norm = X_input.X
     
     gsea_pval = []
     num_clusters = len(adata_cell.obs[OBScelltype].cat.categories)
 
-    if species == 'Homo':
-        gmt_path = path.join(path.dirname(__file__), 'evs.gmt')#Path(__file__).parent / 'evs.gmt'
-    elif species == 'Mus':
-        gmt_path = path.join(path.dirname(__file__), 'evsM.gmt')
+    gmt_path = path.join(path.dirname(__file__), 'evs.gmt')#Path(__file__).parent / 'evs.gmt'
 
     for i in range(num_clusters):
         i = adata_cell.obs[OBScelltype].cat.categories[i]
         gene_rank = pd.DataFrame({'exp': np.array(X_norm[adata_cell.obs[OBScelltype] == str(i), :].mean(axis=0))}, index = X_input.var_names)
 
         res = gp.prerank(rnk=gene_rank, gene_sets=gmt_path)
         terms = res.results.keys()
@@ -108,18 +105,18 @@
         neighbors(adata_combined)
         umap(adata_combined)        
 
         #raise ImportError("")Please install scanpy: `pip install scanpy`.
 
     return(adata_combined)
 
-def deconvolver(adata_ev, adata_cell, species, OBSsample='batch', OBScelltype='celltype', OBSev='sEV', OBSMpca='X_pca', cellN=10, Xraw = True, normalW=True):
+def deconvolver(adata_ev, adata_cell, OBSsample='batch', OBScelltype='celltype', OBSev='sEV', OBSMpca='X_pca', cellN=10, Xraw = True, normalW=True):
 
     adata_combined = preprocess_source(adata_ev, adata_cell, OBScelltype=OBScelltype, OBSev=OBSev, Xraw = Xraw)
-    gsea_pval_dat = source_biogenesis(adata_cell, species, OBScelltype=OBScelltype, Xraw = Xraw, normalW=normalW)
+    gsea_pval_dat = source_biogenesis(adata_cell, OBScelltype=OBScelltype, Xraw = Xraw, normalW=normalW)
     near_neighbor_dat = near_neighbor(adata_combined, OBSsample=OBSsample, OBSev=OBSev, OBScelltype=OBScelltype, OBSMpca=OBSMpca, cellN=cellN)
     
     near_neighbor_dat['times'] = ''
     near_neighbor_dat['type'] = ''
     for i in range(near_neighbor_dat.shape[0]):
         ## iteration for all ev
         tmp_times = near_neighbor_dat.iloc[i,2:12].value_counts(sort = True)
```

### Comparing `SEVtras-0.2.11/SEVtras/id_homo_rna_ev` & `SEVtras-0.2.8/SEVtras/id_homo_rna_ev`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras/id_mus_rna_ev` & `SEVtras-0.2.8/SEVtras/id_mus_rna_ev`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras/main.py` & `SEVtras-0.2.8/SEVtras/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
             each_adata = str(input_path) + '/' + str(sample)
         else:
             each_adata = sample
 
         adata = read_adata(each_adata, get_only=get_only, dir_origin=dir_origin)
         adata = filter_adata(adata)
         sample = sample.replace(".", "_")
-        sample = sample.replace("/", "_")
         name_list.append(sample)
 
         iteration_list = ev_list_s
         inter_gene = []
         pth = 0.005
         flag = 1
         inter_out_p = pd.DataFrame(list(range(0, adata.obs.shape[0])))
@@ -174,22 +173,22 @@
 
     ## Aggregation
     if len_sample > 1:
         sEV_aggregator(out_path, name_list, max_M, score_t, threads, search_UMI)
 
     return('Recognization done!')
 
-def ESAI_calculator(adata_ev_path, adata_cell_path, out_path, species='Homo', OBSsample='batch', OBScelltype='celltype', OBSev='sEV', OBSMpca='X_pca', cellN=10, Xraw = True, normalW=True, plot_cmp='SEV_builtin', save_plot_prefix='', OBSMumap='X_umap',size=10):
+def ESAI_calculator(adata_ev_path, adata_cell_path, out_path, OBSsample='batch', OBScelltype='celltype', OBSev='sEV', OBSMpca='X_pca', cellN=10, Xraw = True, normalW=True, plot_cmp='SEV_builtin', save_plot_prefix='', OBSMumap='X_umap',size=10):
     if not os.path.exists(out_path):
         os.makedirs(out_path)
 
     adata_ev = read_adata(adata_ev_path, get_only=False)
     adata_cell = read_adata(adata_cell_path, get_only=False)
     from .functional import deconvolver, ESAI_celltype, plot_SEVumap, plot_ESAIumap
-    celltype_e_number, adata_evS, adata_com = deconvolver(adata_ev, adata_cell, species, OBSsample, OBScelltype, OBSev, OBSMpca, cellN, Xraw, normalW)
+    celltype_e_number, adata_evS, adata_com = deconvolver(adata_ev, adata_cell, OBSsample, OBScelltype, OBSev, OBSMpca, cellN, Xraw, normalW)
     ##ESAI for sample
     sample_ESAI = (adata_com[adata_com.obs[OBScelltype]==OBSev,].obs[OBSsample].value_counts() / adata_com[adata_com.obs[OBScelltype]!=OBSev,].obs[OBSsample].value_counts()).fillna(0)
 
     ev_activity_dat_pivot = ESAI_celltype(adata_evS, adata_cell, OBSsample, OBScelltype)
 
     out_path = str(out_path)
     if out_path.endswith('/'):
```

### Comparing `SEVtras-0.2.11/SEVtras/sc_pp.py` & `SEVtras-0.2.8/SEVtras/sc_pp.py`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras/sc_readwrite.py` & `SEVtras-0.2.8/SEVtras/sc_readwrite.py`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras/sc_utils.py` & `SEVtras-0.2.8/SEVtras/sc_utils.py`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras/utils.py` & `SEVtras-0.2.8/SEVtras/utils.py`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/SEVtras.egg-info/PKG-INFO` & `SEVtras-0.2.8/SEVtras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SEVtras
-Version: 0.2.11
+Version: 0.2.8
 Summary: sEV-containing droplet identification in scRNA-seq data
 Home-page: http://pypi.python.org/pypi/SEVtras/
 Author: Ruiqiao He
 Author-email: ruiqiaohe@gmail.com
 License: GPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `SEVtras-0.2.11/SEVtras.egg-info/SOURCES.txt` & `SEVtras-0.2.8/SEVtras.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 setup.py
 SEVtras/__init__.py
 SEVtras/_docs.py
 SEVtras/env.py
 SEVtras/evs.gmt
-SEVtras/evsM.gmt
 SEVtras/functional.py
 SEVtras/id_homo_rna_ev
 SEVtras/id_mus_rna_ev
 SEVtras/main.py
 SEVtras/sc_pp.py
 SEVtras/sc_readwrite.py
 SEVtras/sc_utils.py
```

### Comparing `SEVtras-0.2.11/docs/Part1.png` & `SEVtras-0.2.8/docs/Part1.png`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/docs/Part2.png` & `SEVtras-0.2.8/docs/Part2.png`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/docs/SEVtras_overview.png` & `SEVtras-0.2.8/docs/SEVtras_overview.png`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/setup.py` & `SEVtras-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='SEVtras',
-    version='0.2.11',
+    version='0.2.8',
     author='Ruiqiao He',
     author_email='ruiqiaohe@gmail.com',
     packages=['SEVtras'],
     license="GPL",
     url='http://pypi.python.org/pypi/SEVtras/',
     description='sEV-containing droplet identification in scRNA-seq data',
     long_description=open('README.md').read(),
```

### Comparing `SEVtras-0.2.11/tests/sEV_SEVtras.h5ad` & `SEVtras-0.2.8/tests/sEV_SEVtras.h5ad`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/tests/test1.h5ad` & `SEVtras-0.2.8/tests/test1.h5ad`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/tests/test2.h5ad` & `SEVtras-0.2.8/tests/test2.h5ad`

 * *Files identical despite different names*

### Comparing `SEVtras-0.2.11/tests/test_cell.h5ad` & `SEVtras-0.2.8/tests/test_cell.h5ad`

 * *Files identical despite different names*

