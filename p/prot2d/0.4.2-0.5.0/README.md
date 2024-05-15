# Comparing `tmp/prot2d-0.4.2.tar.gz` & `tmp/prot2d-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prot2d-0.4.2.tar", max compression
+gzip compressed data, was "prot2d-0.5.0.tar", max compression
```

## Comparing `prot2d-0.4.2.tar` & `prot2d-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     2830 2024-03-11 14:55:09.953172 prot2d-0.4.2/README.md
--rw-r--r--   0        0        0    38642 2024-03-14 16:48:28.479752 prot2d-0.4.2/prot2d/Classes.py
--rw-r--r--   0        0        0    11522 2024-03-14 16:41:58.326432 prot2d-0.4.2/prot2d/Graphical.py
--rw-r--r--   0        0        0    22210 2024-03-14 16:39:56.433246 prot2d-0.4.2/prot2d/Main_functions.py
--rw-r--r--   0        0        0   198175 2024-03-11 14:19:46.187184 prot2d-0.4.2/prot2d/SF_database/db_info.tsv
--rw-r--r--   0        0        0   388233 2024-01-17 17:40:25.978712 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db
--rw-r--r--   0        0        0        4 2024-01-17 17:40:25.979909 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db.dbtype
--rw-r--r--   0        0        0    41444 2024-01-17 17:40:25.980824 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db.index
--rw-r--r--   0        0        0    74749 2024-01-17 17:40:25.982474 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db.lookup
--rw-r--r--   0        0        0    61944 2024-01-17 17:40:25.983909 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db.source
--rw-r--r--   0        0        0  2354412 2024-01-17 17:40:25.988589 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ca
--rw-r--r--   0        0        0        4 2024-01-17 17:40:25.990266 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ca.dbtype
--rw-r--r--   0        0        0    45535 2024-01-17 17:40:25.991883 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ca.index
--rw-r--r--   0        0        0    51922 2024-01-17 17:40:25.994073 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_h
--rw-r--r--   0        0        0        4 2024-01-17 17:40:25.994761 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_h.dbtype
--rw-r--r--   0        0        0    37255 2024-01-17 17:40:25.995461 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_h.index
--rw-r--r--   0        0        0   388233 2024-01-17 17:40:25.997857 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ss
--rw-r--r--   0        0        0        4 2024-01-17 17:40:25.998587 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ss.dbtype
--rw-r--r--   0        0        0    41444 2024-01-17 17:40:25.999446 prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ss.index
--rw-r--r--   0        0        0    11087 2024-03-14 16:37:51.547921 prot2d-0.4.2/prot2d/Structure_Database.py
--rw-r--r--   0        0        0      322 2024-02-01 15:51:36.214821 prot2d-0.4.2/prot2d/__init__.py
--rw-r--r--   0        0        0      840 2024-03-14 16:42:39.792664 prot2d-0.4.2/prot2d/cli.py
--rw-r--r--   0        0        0    18000 2024-03-11 14:56:28.840350 prot2d-0.4.2/prot2d/main.py
--rw-r--r--   0        0        0     8706 2024-03-14 16:37:03.856707 prot2d-0.4.2/prot2d/utils.py
--rw-r--r--   0        0        0     1138 2024-03-14 16:48:19.626337 prot2d-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 prot2d-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2830 2024-03-11 14:55:09.953172 prot2d-0.5.0/README.md
+-rw-r--r--   0        0        0    38642 2024-03-14 16:48:28.479752 prot2d-0.5.0/prot2d/Classes.py
+-rw-r--r--   0        0        0    11522 2024-03-14 16:41:58.326432 prot2d-0.5.0/prot2d/Graphical.py
+-rw-r--r--   0        0        0    22210 2024-03-14 16:39:56.433246 prot2d-0.5.0/prot2d/Main_functions.py
+-rw-r--r--   0        0        0   198175 2024-05-15 10:24:46.817604 prot2d-0.5.0/prot2d/SF_database/db_info.tsv
+-rw-r--r--   0        0        0   388233 2024-01-17 17:40:25.978712 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db
+-rw-r--r--   0        0        0        4 2024-01-17 17:40:25.979909 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db.dbtype
+-rw-r--r--   0        0        0    41444 2024-01-17 17:40:25.980824 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db.index
+-rw-r--r--   0        0        0    74749 2024-01-17 17:40:25.982474 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db.lookup
+-rw-r--r--   0        0        0    61944 2024-01-17 17:40:25.983909 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db.source
+-rw-r--r--   0        0        0  2354412 2024-01-17 17:40:25.988589 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ca
+-rw-r--r--   0        0        0        4 2024-01-17 17:40:25.990266 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ca.dbtype
+-rw-r--r--   0        0        0    45535 2024-01-17 17:40:25.991883 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ca.index
+-rw-r--r--   0        0        0    51922 2024-01-17 17:40:25.994073 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_h
+-rw-r--r--   0        0        0        4 2024-01-17 17:40:25.994761 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_h.dbtype
+-rw-r--r--   0        0        0    37255 2024-01-17 17:40:25.995461 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_h.index
+-rw-r--r--   0        0        0   388233 2024-01-17 17:40:25.997857 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ss
+-rw-r--r--   0        0        0        4 2024-01-17 17:40:25.998587 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ss.dbtype
+-rw-r--r--   0        0        0    41444 2024-01-17 17:40:25.999446 prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ss.index
+-rw-r--r--   0        0        0    13086 2024-05-15 10:27:29.303592 prot2d-0.5.0/prot2d/Structure_Database.py
+-rw-r--r--   0        0        0      322 2024-02-01 15:51:36.214821 prot2d-0.5.0/prot2d/__init__.py
+-rw-r--r--   0        0        0      840 2024-03-14 16:42:39.792664 prot2d-0.5.0/prot2d/cli.py
+-rw-r--r--   0        0        0    18904 2024-05-15 10:27:33.402252 prot2d-0.5.0/prot2d/main.py
+-rw-r--r--   0        0        0     8706 2024-03-14 16:37:03.856707 prot2d-0.5.0/prot2d/utils.py
+-rw-r--r--   0        0        0     1167 2024-05-15 10:28:39.614377 prot2d-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 prot2d-0.5.0/PKG-INFO
```

### Comparing `prot2d-0.4.2/README.md` & `prot2d-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/Classes.py` & `prot2d-0.5.0/prot2d/Classes.py`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/Graphical.py` & `prot2d-0.5.0/prot2d/Graphical.py`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/Main_functions.py` & `prot2d-0.5.0/prot2d/Main_functions.py`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/db_info.tsv` & `prot2d-0.5.0/prot2d/SF_database/db_info.tsv`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,8 @@
-SF	representative	average_score	family_size	rotation_matrix	rotation_type
+ID	representative	average_score	family_size	rotation_matrix	rotation_type
 3001498	7K1S_C_115_736	0.771823076923077	13	(1, 0, 0, 0, 1, 0, 0, 0, 1)	automatic
 3000778	1O8R_A_1_94		1	(1, 0, 0, 0, 1, 0, 0, 0, 1)	automatic
 3002813	4CPC_E_82_224	1.0	2	(1, 0, 0, 0, 1, 0, 0, 0, 1)	automatic
 3002679	4N9N_A_604_716	0.77195	2	(1, 0, 0, 0, 1, 0, 0, 0, 1)	automatic
 3000912	4HEI_B_1_91	0.8342857142857143	7	(1, 0, 0, 0, 1, 0, 0, 0, 1)	automatic
 3001008	3FT9_A_2_95	0.9306666666666666	3	(1, 0, 0, 0, 1, 0, 0, 0, 1)	automatic
 3001834	1QZX_A_1_84	0.781190909090909	14	(1, 0, 0, 0, 1, 0, 0, 0, 1)	automatic
```

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db.index` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db.index`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db.lookup` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db.lookup`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db.source` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db.source`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ca` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ca`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ca.index` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ca.index`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_h` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_h`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_h.index` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_h.index`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ss` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ss`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/SF_database/foldseek_db/db_ss.index` & `prot2d-0.5.0/prot2d/SF_database/foldseek_db/db_ss.index`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/Structure_Database.py` & `prot2d-0.5.0/prot2d/Structure_Database.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,95 @@
 import numpy as np
 import subprocess
 import pandas as pd
 import importlib.resources as pkg_resources
+import csv
 
 
 #SCOP_summary = '/Users/constantincarl/Uni/BachelorThesis/prot2D/database/SCOP_SF_summary.txt'
 class Structure_Database:
     # the obj is created using at least foldseek_executable path and tmp_Dir from the user.
     # db information and data is saved in the package structure itself (default relative paths)
     # --> the data base can be acce
     def __init__(self,foldseek_executable,tmp_dir):
         self.foldseek_executable = foldseek_executable
         self.tmp_dir = tmp_dir
-        self.package_data_dir_path = 'prot2d.SF_database'
-        self.SCOP_SF_db_info_tsv = self.load_package_file(self.package_data_dir_path,'db_info.tsv') #SCOP SF info tsv
-        self.foldseek_SCOP_db= self.load_package_file(self.package_data_dir_path+'.foldseek_db','db') #SCOP SF database dir
+        self.presetSCOPdb = 'prot2d.SF_database'
+        self.SCOP_SF_db_info_tsv = self.load_package_file(self.presetSCOPdb,'db_info.tsv') #SCOP SF info tsv
+        self.foldseek_SCOP_db= self.load_package_file(self.presetSCOPdb+'.foldseek_db','db') #SCOP SF database dir
         
+        self.flexUSERdb = 'prot2d.flexUSER_database'
+        self.USER_db_info_tsv = self.load_package_file(self.flexUSERdb,'db_info.tsv') #SCOP SF info tsv
+        self.foldseek_USER_db= self.load_package_file(self.flexUSERdb+'.foldseek_db','db') #SCOP SF database dir
+
     def load_package_file(self,package_data_dir,filename):
         with pkg_resources.path(package_data_dir,filename) as path:
             return path
     
+    def create_USER_PDB_foldseek_index(self,pdb_dir):
+        # create foldseek index out of user_pdbs 
+        command = [self.foldseek_executable,'createdb',pdb_dir,self.foldseek_USER_db]
+        subprocess.run(command)
+        # TODO: important: delete not working pdbs from db_info table --> else errors
+
+    def check_create_USERdb_info_table(self,name_id_mapping, db_info_table):
+        id_name_dict = {}
+        # Check uniqueness of IDs and names
+        with open(name_id_mapping, "r") as file:
+            reader = csv.DictReader(file)
+            for row in reader:
+                if row["ID"] in id_name_dict:
+                    print(f"Duplicate ID found: {row['ID']}")
+                    return None
+                if row["NAME"] in id_name_dict.values():
+                    print(f"Duplicate NAME found: {row['NAME']}")
+                    return None
+                id_name_dict[row["ID"]] = row["NAME"]
+        # create db_info_table with rotation matrix init
+        with open(db_info_table, "w") as file:
+            file.write("ID\trepresentative\trotation_matrix\trotation_type\n")
+            for id, representative in id_name_dict.items():
+                line = f"{id}\t{representative}\t(1, 0, 0, 0, 1, 0, 0, 0, 1)\tautomatic\n"
+                file.write(line)
+        print("Database info TSV was created successfully.")
+        return db_info_table
+
     def create_fixed_tmp_db(self,sf_number):
         #not used !
         db  = pd.read_csv(self.SCOP_SF_db_info_tsv, sep='\t')
         if sf_number not in db['SF'].values:
                 print(f"{sf_number} is not a valid SCOP SF number")
                 return False
         else:
             filtered_row = db.loc[db['SF'] == sf_number]
             representative = filtered_row['representative']
 
-    def get_matching_SF_U_T_fixed_region(self,input_pdb, min_prob,fixed_sf_number = None):
+    def get_matching_SF_U_T_fixed_region(self,input_pdb, min_prob,fixed_sf_number = None, use_flex_USER_db=False):
+        db = self.foldseek_SCOP_db if not use_flex_USER_db else self.foldseek_USER_db 
+        db_info = self.SCOP_SF_db_info_tsv if not use_flex_USER_db else self.USER_db_info_tsv
+        #TODO: change naming from sf to id...
+        #TODO: check if user db is correctly set for usage (db info file available...?!)
         try:
             filename = input_pdb.split('/')[-1]  # Gets the filename with extension
             filename_without_ext = '.'.join(filename.split('.')[:-1])
             result_file = self.tmp_dir+'/'+filename_without_ext+'_foldseek_result'
             print_file = self.tmp_dir+'/'+filename_without_ext+'foldseek_printOut'
-            command = [self.foldseek_executable,'easy-search', input_pdb,self.foldseek_SCOP_db,result_file , self.tmp_dir,'--format-output', 'query,target,qstart,qend,tstart,tend,tseq,prob,alntmscore,u,t,lddtfull,qaln,taln']
+            command = [self.foldseek_executable,'easy-search', input_pdb,db,result_file , self.tmp_dir,'--format-output', 'query,target,qstart,qend,tstart,tend,tseq,prob,alntmscore,u,t,lddtfull,qaln,taln']
             print("### foldseek start ### ")
             with open(print_file, 'w') as output_file:
                 subprocess.run(command,stdout=output_file, stderr=output_file)
 
             column_names = ['query', 'target', 'qstart', 'qend', 'tstart', 'tend', 'tseq', 'prob', 'alntmscore', 'u', 't','lddtfull','qaln','taln']
             df = pd.read_csv(result_file, sep='\t', names=column_names)
             if len(df) ==0:
                 print("No matching SF found")
                 return None,None,None,None,None,None,None
             if fixed_sf_number!=None:
                 try:
-                    fam_info  = pd.read_csv(self.SCOP_SF_db_info_tsv, sep='\t')
+                    fam_info  = pd.read_csv(db_info, sep='\t')
                     if fixed_sf_number not in fam_info['SF'].values:
                         raise ValueError(f"Error: {fixed_sf_number} is not a valid SCOP SF number")
                     sf_row = fam_info.loc[fam_info['SF'] == fixed_sf_number]
                     fixed_representative_name = sf_row['representative'].iloc[0]
                     try:
                         matched_row = df[df['target'] == fixed_representative_name+".pdb"].iloc[0]
                         print(f"Using fixed SF: {fixed_sf_number} (representative: {fixed_representative_name})")
@@ -93,41 +130,42 @@
                     new_lddtfull.append(0)
                 elif q_char != '-' and t_char != '-':
                     #alignment residue with existing lddt
                     new_lddtfull.append(lddtfull[lddt_index])
                     lddt_index += 1
 
             ## read in SCOP_db summary file ##
-            df = pd.read_csv(self.SCOP_SF_db_info_tsv, sep='\t')
+            df = pd.read_csv(db_info, sep='\t')
             df.replace({'None': None, 'nan': None}, inplace=True)
 
             specific_row = df.loc[df['representative'] == best_SF_representative]
             if not df['representative'].eq(best_SF_representative).any():
                 print("db error !!!!! (representative in db not in summary file)")
                 return None,None,None,None,None,None,None
-            SF = specific_row['SF'].iloc[0]
+            ID = specific_row['ID'].iloc[0]
             fixed_rot_matrix_string = specific_row['rotation_matrix'].iloc[0]
             
             fixed_rot =string_matrix_to_numpy(fixed_rot_matrix_string)
             u_matrix = np.array([float(num) for num in u.split(',')]).reshape(3, 3)
             t_vector = np.array([float(num) for num in t.split(',')])
-            print("\n################# foldseek result")
+            
+            print(f"\n################# foldseek result  (user_db: {use_flex_USER_db})")
             print("--- Rotating by inital SF FoldSeek alignment + fixed family rotation ---")
             print(f"input: {filename_without_ext}")
-            print(f"SF: {SF} (prob: {matched_row['prob']})")
+            print(f"ID: {ID} (prob: {matched_row['prob']})")
             print(f"representative: {best_SF_representative}")
             print("#################\n")
             
-            return SF,prob,u_matrix,t_vector,fixed_rot,(q_start,q_end),new_lddtfull
+            return ID,prob,u_matrix,t_vector,fixed_rot,(q_start,q_end),new_lddtfull
         except Exception as e:
             print(e)
             return None,None,None,None,None,None,None
 
-    def initial_and_fixed_Sf_rot_region(self,input_pdb,drop_family_prob,fixed_sf):
-        sf,prob,u,t,fixed_rot,aligned_region,lddtfull = self.get_matching_SF_U_T_fixed_region(input_pdb,drop_family_prob,fixed_sf)
+    def initial_and_fixed_Sf_rot_region(self,input_pdb,drop_family_prob,fixed_sf, flex_USER_db):
+        sf,prob,u,t,fixed_rot,aligned_region,lddtfull = self.get_matching_SF_U_T_fixed_region(input_pdb,drop_family_prob,fixed_sf,flex_USER_db)
         if sf == None:
             return None,None,None,None,None
         U_inv,T_inv = invert_UT(u,t)
 
         filename = input_pdb.split('/')[-1]  # Gets the filename with extension
         filename_without_ext = '.'.join(filename.split('.')[:-1])
         sf_aligned_rot_pdb = self.tmp_dir+'/'+filename_without_ext+f'_sf-{sf}_aligned_rot.pdb'
```

### Comparing `prot2d-0.4.2/prot2d/cli.py` & `prot2d-0.5.0/prot2d/cli.py`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/prot2d/main.py` & `prot2d-0.5.0/prot2d/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,25 @@
 
     - returns nothing but changes the db entry of the given SF_number. 
     """
     db= Structure_Database(None,None)
     rot_matrix = transform_pymol_out_to_UT(pymol_output)[0]
     db.set_manual_SF_rotation(SF_number, rot_matrix)
 
-def create_2DSVG_from_pdb(pdb_file:str, result_dir:str, tmp_dir:str, family_vis:bool=True, fam_aligned_splitting:bool = True, drop_family_prob:float = 0.5,foldseek_executable:str=None,fixed_sf:int=None,fam_info:bool=True ,domain_splitted:bool=False, domain_annotation_file:str=None, domain_hull:bool=True, visualisation_type:str ="normal", 
+def create_USERflex_db(pdb_dir, name_id_mapping_csv, foldseek_executable):
+        structure_database_obj = Structure_Database(foldseek_executable,None)
+        # create user-specified databse for comparing input proteins to. needs
+        # needs pdb_dir and matching name -> id list for tsv info
+        info_check = structure_database_obj.check_create_USERdb_info_table(name_id_mapping_csv,structure_database_obj.USER_db_info_tsv)
+        if info_check == None:
+            print("USER-database creation error: name_id mapping !")
+            return
+        structure_database_obj.create_USER_PDB_foldseek_index(pdb_dir)
+
+def create_2DSVG_from_pdb(pdb_file:str, result_dir:str, tmp_dir:str, family_vis:bool=True, fam_aligned_splitting:bool = True, drop_family_prob:float = 0.5,foldseek_executable:str=None,user_db:bool=False,fixed_sf:int=None,fam_info:bool=True ,domain_splitted:bool=False, domain_annotation_file:str=None, domain_hull:bool=True, visualisation_type:str ="normal", 
                     cysteins:bool=True, as_annotation:bool=False, mark_endings:bool=True, simple_helix:bool=True, show_lddt_col:bool=False,show_lddt_text:bool=False, find_best_rot_step:int = 30, simple_coil_avg:int=10, chain_info:bool=True):
     """
     Main method of the package for creating 2D visualisations of a protein in form of a SVG file. The user can decide between different visualisation options.
     
     Args:\n\n
 
     - pdb_file (str): Path to pdb file the visualisation file is generated on. (Required)\n
@@ -149,15 +159,16 @@
     - fam_aligned_splitting (bool): If True, the protein is split into SF-aligned (is rotated based on this segment) and not-aligned parts. THey are connected with a dashed line. Default is True.\n
     - drop_family_prob (float): Allows the program to drop a chosen SF if the FoldSeek probability is smaller than given cut-off. In this case the protein rotation is determined using the implemented "find_best_view_angle" method. Default is 0.5. \n
     - show_lddt_col (bool): LDDT scores from FoldSeek alignment to best matching SF is shown per residue as colorscale (magenta). Default is False. \n
     - show_lddt_text (bool): LDDT scores from FoldSeek alignment to best matching SF is shown per residue. Default is False. \n
     - foldseek_executable (str): Path to foldseek executable (will be used for family alignment).\n
     - fixed_sf (int): Fixed SCOP superamily accession number that will be used for the protein (/ for every domain in the protein) (to distant SFs cannot be used for aligning)\n
     - fam_info (bool): If True, adds assigned Superfamily number and corresponding foldseek probability to the drawing. Default is True.\n
-
+    - user_db (bool): If True, prot2d uses the user-created database for protein matching. The user-db must be created before with the "create_USERflex_db" function. Default is False for simple usage with SCOP superfamily database\n4
+    
     - domain_splitted (bool): If True, protein is split into domains using the provided domain annotation file. Can be used in combination with family_vis which is then applied on each domain seperatly. Default is False.\n
     - domain_annotation_file (str): Path to the domain annotation file. Required if domain_splitted is True.\n
     - domain_hull (bool): If True sourounds domains with smoothed convex hull colored based on the secondary structure composition (R,G,B) <-> (helix,sheet,coil). Default is True\n
 
     - visualisation_type (string): "only-path", "normal", or "simple-coil". Default is "normal".\n
     - cysteins (bool): If True, includes calculated cystein bonds in the visualisation. Default is True.\n
     - as_annotation (bool): If True, includes AS-annotation. Default is False.\n
@@ -209,15 +220,15 @@
         ############## 2) Get rotation of protein (family-vis / best rotation) ##############
         dom_proteins = []
         matched_sfs = []
         probs = []
         for dom_file in domain_files:
             print(f"\n### \"{dom_file}\" ###\n")
             if family_vis:
-                sf,prob,sf_aligned_pdb_file, aligned_region,lddtfull = structure_database_obj.initial_and_fixed_Sf_rot_region(dom_file,drop_family_prob,fixed_sf=fixed_sf)
+                sf,prob,sf_aligned_pdb_file, aligned_region,lddtfull = structure_database_obj.initial_and_fixed_Sf_rot_region(dom_file,drop_family_prob,fixed_sf=fixed_sf, flex_USER_db=user_db)
                 if sf_aligned_pdb_file== None:
                     #no mathcing sf (with higher than min prob found) --> do normal vis
                     print("\033[91m"+ "No maching SF (with higher prob than min prob) found. Normal roation algo will be used!"+"\033[0m" )
                     add_header_to_pdb(dom_file)
                     dom_prot = Protein()
                     dom_prot.chain = chain_id
                     pdb_element = dom_prot.parse_pdb(dom_file)
```

### Comparing `prot2d-0.4.2/prot2d/utils.py` & `prot2d-0.5.0/prot2d/utils.py`

 * *Files identical despite different names*

### Comparing `prot2d-0.4.2/pyproject.toml` & `prot2d-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "prot2d"
-version = "0.4.2"
+version = "0.5.0"
 description = "Python package for creating simplified 2D protein visualisations. Specialised on showing differences and similaritys between proteins from the same protein family."
 authors = ["constantincarl <ge37goy@mytum.de>"]
 readme = "README.md"
 
-include = ["prot2d/SF_database/*"]
+include = ["prot2d/SF_database/*","prot2d/flexUSER_database/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 biopython = "^1.81"
 networkx = "^3.2"
 svgwrite = "^1.4.3"
 shapely = "^2.0.2"
```

### Comparing `prot2d-0.4.2/PKG-INFO` & `prot2d-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prot2d
-Version: 0.4.2
+Version: 0.5.0
 Summary: Python package for creating simplified 2D protein visualisations. Specialised on showing differences and similaritys between proteins from the same protein family.
 Author: constantincarl
 Author-email: ge37goy@mytum.de
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

