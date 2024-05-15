# Comparing `tmp/adtoolbox-0.5.6.tar.gz` & `tmp/adtoolbox-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adtoolbox-0.5.6.tar", max compression
+gzip compressed data, was "adtoolbox-0.5.7.tar", max compression
```

## Comparing `adtoolbox-0.5.6.tar` & `adtoolbox-0.5.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      909 2024-05-08 21:28:31.763577 adtoolbox-0.5.6/README.md
--rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.6/adtoolbox/.DS_Store
--rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.6/adtoolbox/__init__.py
--rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.6/adtoolbox/__main__.py
--rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.6/adtoolbox/adm.py
--rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.6/adtoolbox/bio_struct.py
--rwxr-xr-x   0        0        0    29971 2024-05-08 22:45:44.491151 adtoolbox-0.5.6/adtoolbox/cli.py
--rw-r--r--   0        0        0    16518 2024-05-09 03:31:15.258155 adtoolbox-0.5.6/adtoolbox/configs.py
--rw-r--r--   0        0        0   108599 2024-05-09 03:33:26.323559 adtoolbox-0.5.6/adtoolbox/core.py
--rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.6/adtoolbox/metagenomics_report.py
--rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.6/adtoolbox/optimize.py
--rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.6/adtoolbox/pipeline.py
--rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.6/adtoolbox/pkg_data/.DS_Store
--rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.6/adtoolbox/pkg_data/Modified_ADM_Map.json
--rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.6/adtoolbox/pkg_data/Modified_ADM_Model.json
--rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.6/adtoolbox/pkg_data/README.md
--rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.5.6/adtoolbox/pkg_data/qiime_template_paired.txt
--rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.5.6/adtoolbox/pkg_data/qiime_template_single.txt
--rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.6/adtoolbox/pkg_data/slurm_template.txt
--rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.6/adtoolbox/stats.py
--rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.6/adtoolbox/tables.py
--rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.5.6/adtoolbox/utils.py
--rw-r--r--   0        0        0      748 2024-05-09 03:33:35.872104 adtoolbox-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     4338 2024-05-09 03:33:38.492417 adtoolbox-0.5.6/setup.py
--rw-r--r--   0        0        0     1882 2024-05-09 03:33:38.492620 adtoolbox-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      988 2024-05-09 04:21:15.185160 adtoolbox-0.5.7/README.md
+-rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.7/adtoolbox/.DS_Store
+-rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.7/adtoolbox/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.7/adtoolbox/__main__.py
+-rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.7/adtoolbox/adm.py
+-rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.7/adtoolbox/bio_struct.py
+-rwxr-xr-x   0        0        0    29971 2024-05-08 22:45:44.491151 adtoolbox-0.5.7/adtoolbox/cli.py
+-rw-r--r--   0        0        0    16613 2024-05-15 15:55:16.214048 adtoolbox-0.5.7/adtoolbox/configs.py
+-rw-r--r--   0        0        0   109451 2024-05-15 17:41:17.396046 adtoolbox-0.5.7/adtoolbox/core.py
+-rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.7/adtoolbox/metagenomics_report.py
+-rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.7/adtoolbox/optimize.py
+-rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.7/adtoolbox/pipeline.py
+-rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.7/adtoolbox/pkg_data/.DS_Store
+-rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.7/adtoolbox/pkg_data/Modified_ADM_Map.json
+-rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.7/adtoolbox/pkg_data/Modified_ADM_Model.json
+-rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.7/adtoolbox/pkg_data/README.md
+-rw-r--r--   0        0        0      864 2024-05-15 19:39:10.537774 adtoolbox-0.5.7/adtoolbox/pkg_data/qiime_template_paired.txt
+-rw-r--r--   0        0        0      920 2024-05-15 19:45:02.263654 adtoolbox-0.5.7/adtoolbox/pkg_data/qiime_template_single.txt
+-rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.7/adtoolbox/pkg_data/slurm_template.txt
+-rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.7/adtoolbox/stats.py
+-rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.7/adtoolbox/tables.py
+-rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.5.7/adtoolbox/utils.py
+-rw-r--r--   0        0        0      748 2024-05-15 19:52:55.322828 adtoolbox-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     4420 2024-05-15 19:53:04.395268 adtoolbox-0.5.7/setup.py
+-rw-r--r--   0        0        0     1961 2024-05-15 19:53:04.395592 adtoolbox-0.5.7/PKG-INFO
```

### Comparing `adtoolbox-0.5.6/README.md` & `adtoolbox-0.5.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,12 +8,14 @@
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)
 <a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 [![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)
 
+***NOTE***:Binder implementations don't offer escher map functionalities yet.
+
 ADToolbox comes with a detailed documentation website. You can access this website using the link below:
 
 ** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **
```

### Comparing `adtoolbox-0.5.6/adtoolbox/.DS_Store` & `adtoolbox-0.5.7/adtoolbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/__init__.py` & `adtoolbox-0.5.7/adtoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/adm.py` & `adtoolbox-0.5.7/adtoolbox/adm.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/bio_struct.py` & `adtoolbox-0.5.7/adtoolbox/bio_struct.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/cli.py` & `adtoolbox-0.5.7/adtoolbox/cli.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/configs.py` & `adtoolbox-0.5.7/adtoolbox/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 RXN_DB = os.path.join(Main_Dir, "Database", "Reaction_Metadata.csv")
 
 Seed_RXN_DB = os.path.join(Main_Dir, "Database", "reactions.json")
 Seed_COMPOUNDS_DB = os.path.join(Main_Dir, "Database", "compounds.json")
 
 ADTOOLBOX_CONTAINERS={
-	'docker_x86':"parsaghadermazi/adtoolbox:latest",
+	'docker_x86':"parsaghadermazi/adtoolbox:x86",
 	'docker_arm64':"parsaghadermazi/adtoolbox:arm64",
 	'singularity_x86':"docker://parsaghadermazi/adtoolbox:x86",
 	'singularity_arm64':"docker://parsaghadermazi/adtoolbox:arm64"}
 
 E_ADM_2_REMOTE={
 	"model_parameters":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_model_parameters.json",
 	"base_parameters":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_base_parameters.json",
@@ -79,15 +79,15 @@
                   "http://www.cazy.org/Polysaccharide-Lyases.html",
                   "http://www.cazy.org/Carbohydrate-Esterases.html"
                   		],
 	"amplicon2genome":{'Version': 'https://data.ace.uq.edu.au/public/gtdb/data/releases/latest/VERSION',
                'MD5SUM': 'https://data.ace.uq.edu.au/public/gtdb/data/releases/latest/MD5SUM',
                'FILE_DESCRIPTIONS': 'https://data.ace.uq.edu.au/public/gtdb/data/releases/latest/FILE_DESCRIPTIONS',
                'metadata_field_desc': 'https://data.ace.uq.edu.au/public/gtdb/data/releases/latest/auxillary_files/metadata_field_desc.tsv',
-               'bac120_ssu': 'https://data.ace.uq.edu.au/public/gtdb/data/releases/latest/genomic_files_all/ssu_all.tar.gz'
+               'bac120_ssu': 'https://data.ace.uq.edu.au/public/gtdb/data/releases/latest/genomic_files_all/ssu_all.fna.gz'
                },
 	
 	"seed_rxn_url":"https://github.com/modelSEED/modelSEEDDatabase/raw/master/Biochemistry/reactions.json",
  	"seed_compound_url":"https://github.com/ModelSEED/ModelSEEDDatabase/raw/master/Biochemistry/compounds.json",
 	
 }
 
@@ -196,15 +196,15 @@
 			warnings.warn(f"The ADM parameters are not in the same directory!")
 
 class Metagenomics:
 	"""	
 	An instance of this class will hold all the configuration information for core.Metagenomics functionalities.
 	"""
 	### Here we have some class variables that are used in the class
-	gtdb_dir="ssu_all_*.fna"
+	gtdb_dir="ssu_all*.fna"
 	def __init__(self, 
             amplicon2genome_k=10,
             vsearch_similarity=0.97,
             genomes_base_dir=os.path.join(Main_Dir,"Genomes"),
             align_to_gtdb_outputs_dir=os.path.join(Main_Dir,"Genomes"),
             amplicon2genome_db=Database().amplicon_to_genome_db,
             qiime_outputs_dir=os.path.join(Main_Dir,'Metagenomics_Data','QIIME_Outputs'),
@@ -220,14 +220,15 @@
             e_value=10**-5,
             qiime2_docker_image="quay.io/qiime2/core:2022.2",
             qiime2_singularity_image="docker://quay.io/qiime2/core:2022.2",
             qiime2_paired_end_bash_str=os.path.join(PKG_DATA,"qiime_template_paired.txt"),
             qiime2_single_end_bash_str=os.path.join(PKG_DATA,"qiime_template_single.txt"),
 			qiime_classifier_db=Database().qiime_classifier_db,
 			adm_mapping=Database().adm_microbial_groups_mapping,
+			qiime2_p_trunc_len:tuple[int,int]=("250","250"),
              ):
 		self.k = amplicon2genome_k
 		self.vsearch_similarity = vsearch_similarity
 		self.align_to_gtdb_outputs_dir = align_to_gtdb_outputs_dir
 		self.amplicon2genome_db = amplicon2genome_db
 		self.qiime_outputs_dir = qiime_outputs_dir
 		self.protein_db=Database().protein_db
@@ -250,15 +251,16 @@
 			self.gtdb_dir_fasta=None
 		self.genome_alignment_script=genome_alignment_script	
 		self.adtoolbox_singularity=adtoolbox_singularity
 		self.adtoolbox_docker=adtoolbox_docker
 		self.rsync_download_dir=rsync_download_dir
 		self.genomes_base_dir=genomes_base_dir
 		self.adm_mapping=adm_mapping
-
+		self.qiime2_p_trunc_len=qiime2_p_trunc_len
+		
 class Documentation:
     def __init__(self,
                  readme=os.path.join(PKG_DATA,"README.md")):
         self.readme = readme
 
 class Utils:
 	"""
```

### Comparing `adtoolbox-0.5.6/adtoolbox/core.py` & `adtoolbox-0.5.7/adtoolbox/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from bs4 import BeautifulSoup
 from datetime import datetime
 from pathlib import Path
 from collections import Counter
 from collections import namedtuple
 import pathlib
 import asyncio
-import tarfile
+import gzip
 import configs
 from rich.progress import track,Progress
 import rich
 from adtoolbox import Main_Dir
 from typing import Iterable
 from typing import Union
 from dataclasses import dataclass
@@ -1395,16 +1395,17 @@
                     block_size = 1024
                     with Progress() as progress:
                         task1 = progress.add_task("Downloading " + keys, total=total_size)
                         with open(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1]), 'wb') as f:
                             for data in r.iter_content(block_size):
                                 progress.update(task1, advance=len(data))
                                 f.write(data)
-                with tarfile.open(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1])) as f_in:
-                    f_in.extractall(self.config.amplicon_to_genome_db)
+                with gzip.open(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1]),"r") as f_in:
+                    with open(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1].replace(".gz","")),"wb") as f_out:
+                        f_out.write(f_in.read())
 
                 
                 os.remove(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1]))
         else:
             for keys in ['Version', 'MD5SUM', 'FILE_DESCRIPTIONS']:
                 with requests.get(url[keys], allow_redirects=True, stream=False) as r:
                     with open(os.path.join(self.config.amplicon_to_genome_db, keys), 'wb') as f:
@@ -1412,16 +1413,17 @@
             with requests.get(url['metadata_field_desc'], allow_redirects=True, stream=False) as r:
                 with open(os.path.join(self.config.amplicon_to_genome_db, 'metadata_field_desc.tsv'), 'wb') as f:
                     f.write(r.content)
             for keys in [ 'bac120_ssu']:
                 with requests.get(url[keys], allow_redirects=True, stream=False) as r:
                     with open(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1]), 'wb') as f:
                         f.write(r.content)
-                with tarfile.open(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1])) as f_in:
-                    f_in.extractall(self.config.amplicon_to_genome_db)
+                with gzip.open(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1]),"r") as f_in:
+                    with open(os.path.join(self.config.amplicon_to_genome_db, url[keys].split("/")[-1].replace(".gz","")),"wb") as f_out:
+                        f_out.write(f_in.read())
         if verbose:
             rich.print("[bold green]Downloaded all the required files for Amplicon to Genome functionality.[/bold green]")
                     
                         
 
             
     def download_all_databases(self,verbose:bool=True)->None:
@@ -1601,15 +1603,15 @@
                         ' --db '+ gtdb_dir_fasta +
                         ' --id ' +str(self.config.vsearch_similarity) +
                         ' --threads '+str(self.config.vsearch_threads)+
                         ' --alnout '+ alignment_dir +
                         ' --top_hits_only'+'\n')
         
         if container=="docker":
-            bash_script='docker run'
+            bash_script='docker run '
             for dir in dirs:
                 bash_script+=('-v '+dir+':'+dir+' ')
             
             bash_script += (self.config.adtoolbox_docker+' vsearch --top_hits_only --blast6out '+
                         match_table+
                         ' --usearch_global '+ query +
                         ' --db '+ gtdb_dir_fasta +
@@ -1686,15 +1688,15 @@
             
         genome_dir=pathlib.Path(output_dir)
             
         if container=="None":
             bash_script+=('rsync -avz --progress '+base_ncbi_dir+specific_ncbi_dir+' '+str(genome_dir))
             
         if container=="docker":
-            bash_script+=('docker run -it -v '+str(genome_dir.parent)+':'+str(genome_dir.parent)+ f' {self.config.adtoolbox_docker} rsync -avz --progress '+' '+base_ncbi_dir+specific_ncbi_dir+' '+str(genome_dir))
+            bash_script+=('docker run -v '+str(genome_dir.parent)+':'+str(genome_dir.parent)+ f' {self.config.adtoolbox_docker} rsync -avz --progress '+' '+base_ncbi_dir+specific_ncbi_dir+' '+str(genome_dir))
             
         if container=="singularity":
             bash_script+=('singularity exec -B '+str(genome_dir.parent)+':'+str(genome_dir.parent)+ f' {self.config.adtoolbox_singularity} rsync -avz --progress '+' '+base_ncbi_dir+specific_ncbi_dir+' '+str(genome_dir))
         
         return bash_script,
     
     def async_genome_downloader(self,identifiers:Iterable[str],batch_size:float=10,container:str="None"):
@@ -1705,43 +1707,44 @@
         await asyncio.gather(*[self._genome_dl_coro(identifier=i,semaphore=semaphore,container=container) for i in identifiers])
         
     async def _genome_dl_coro(self,identifier:str,semaphore:asyncio.Semaphore,container:str="None")->None:
         async with semaphore:
             await asyncio.create_subprocess_exec(*self.download_genome(identifier=identifier,container=container).split(" "))
     
     def extract_genome_info(self,
+                            base_dir:str,
                             endpattern:str="genomic.fna.gz",
                             filters:dict={
                                           "INCLUDE":[],
                                           "EXCLUDE":["cds","rna"],
                                             })->dict[str,str]:
         """This function extracts the genome information from the genomes base directory. The output
         is a dictionary where the keys are the genome IDs and the values are the paths to the genome files.
         
         Required Configs:
-            config.genomes_base_dir: The path to the base directory where the genomes are saved.
-            ---------
+            None
+        ---------
         Args:
-            genome_info (dict[str,str]): A dictionary containing the genome information.
+            base_dir (str): The path to the base directory where the genomes are saved.
             endpattern (str, optional): The end pattern of the genome files. Defaults to "genomic.fna.gz".
             filters (dict, optional): The filters to be applied to the genome files. This filter must be a 
             dictionary with two keys: INCLUDE and EXCLUDE. The values of these keys must be lists of strings.
             Defaults to {"INCLUDE":[],"EXCLUDE":["cds","rna"]}. This defult is compatible with the genomes downloaded
             from NCBI i.e. only change this if you are providing your own genomes with different file name conventions.
         Returns:
             dict[str,str]: A dictionary containing the address of the genomes that are downloaded or to be downloaded.
         """
-        base_dir = pathlib.Path(self.config.genomes_base_dir)
+        base_dir = pathlib.Path(base_dir)
         genome_info = {}
         for genome_dir in base_dir.iterdir():
             if genome_dir.is_dir():
                 candids=list(genome_dir.rglob(f'*{endpattern}'))
                 for candid in candids:
                     if all([i in candid.name for i in filters["INCLUDE"]]) and all([i not in candid.name for i in filters["EXCLUDE"]]):
-                        genome_info[genome_dir.name]=str(candid.absolute())           
+                        genome_info[candid.name.replace("_genomic.fna.gz","")]=str(candid.absolute())           
         return genome_info
      
     def align_genome_to_protein_db(
             self,
             address:str,
             outdir:str,
             name:str,
@@ -1751,26 +1754,24 @@
         This is a function that will align a genome to the Protein Database of the ADToolbox using mmseqs2.
         If you want to save the scripts, set save to True. Note that the alignment tables will be saved in any case.
         Note that this function uses mmseqs2 to align the genomes to the protein database. So, to run this function without
         any container you need to have mmseqs2 installed on your system. However, if you want to run this function with a container,
         you need to have the container installed on your system. You may select from "None", "docker", "singularity".
 
         Requires:
-            config.genome_alignment_output: The path to the directory where the alignment results will be saved.
-            ---------
-            config.protein_db: The path to the ADToolbox protein database in fasta.
+            config.protein_db: The address of the protein database of the ADToolbox.
             ---------
             config.adtoolbox_docker: The name of the docker image to be used by ADToolbox (Only if using Docker as container).
             ---------
             config.adtoolbox_singularity: The name of the singularity image to be used by ADToolbox (Only if using Singularity as container).
             ---------
         Args:
-            address (str): The address of the genome fasta file. The file must be in fasta format.
-            run (bool, optional): Whether to run the alignment. Defaults to True.
-            save (bool, optional): Whether to save the alignment scripts. Defaults to True.
+            address (str): The address of the genome to be aligned.
+            outdir (str): The output directory where the alignment files will be saved.
+            name (str): The name of the genome.
             container (str, optional): The container to use. Defaults to "None". You may select from "None", "docker", "singularity".
 
         Returns:
             str: A dictionary containing the alignment files.
             str: The bash script that is used to align the genomes or to be used to align the genomes.
         """
  
@@ -1781,15 +1782,15 @@
                 address + " " + \
                 self.config.protein_db + " " + \
                 alignment_file+ ' tmp --format-mode 4 '+"\n\n"
         
         if container=="docker":
             bash_script = ""
             alignment_file=os.path.join(outdir,"Alignment_Results_mmseq_"+name+".tsv")
-            bash_script +="docker run -it "+ \
+            bash_script +="docker run "+ \
             " -v "+address+":"+address+ \
             " -v "+self.config.protein_db+":"+self.config.protein_db+ \
             " -v "+outdir+":"+outdir+ \
             f" {self.config.adtoolbox_docker}  mmseqs easy-search " + \
                 address + " " + \
                 self.config.protein_db + " " + \
                 alignment_file+' tmpfiles --format-mode 4 '+"\n\n"
@@ -2030,15 +2031,16 @@
     def run_qiime2_from_sra(self,
                             read_1:str,
                             read_2:str|None,
                             sample_name:str|None=None,
                             manifest_dir:str|None=None,
                             workings_dir:str|None=None,
                             save_manifest:bool=True,
-                            container:str='None') -> tuple[str,str]:
+                            container:str='None',
+                            **kwargs) -> tuple[str,str]:
         """
         This method uses the input fastq files to run qiime2. The method uses the qiime2 template scripts that are provided in pkg_data module.
         The method also creates a manifest file for qiime2. The manifest file is created based on the input fastq files.
         Required Configs:
             config.qiime2_single_end_bash_str: The path to the qiime2 bash script for single end reads.
             ---------
             config.qiime2_paired_end_bash_str: The path to the qiime2 bash script for paired end reads.
@@ -2092,19 +2094,32 @@
   
         if paired_end:
             with open(self.config.qiime2_paired_end_bash_str,"r") as f:
                 qiime2_bash_str=f.read()
         else:
             with open(self.config.qiime2_single_end_bash_str,"r") as f:
                 qiime2_bash_str=f.read()
+        if kwargs.get("p_trunc_len",None) is not None:
+            if not paired_end:
+                qiime2_bash_str=qiime2_bash_str.replace("<p-trunc-len>",str(kwargs.get("p_trunc_len")[0]))
+            else:
+                qiime2_bash_str=qiime2_bash_str.replace("<p-trunc-len-f>",str(kwargs.get("p_trunc_len")[0]))
+                qiime2_bash_str=qiime2_bash_str.replace("<p-trunc-len-r>",str(kwargs.get("p_trunc_len")[1]))
+        else:
+            if not paired_end:
+                qiime2_bash_str=qiime2_bash_str.replace("<p-trunc-len>",self.config.qiime2_p_trunc_len[0])
+            else:
+                qiime2_bash_str=qiime2_bash_str.replace("<p-trunc-len-f>",self.config.qiime2_p_trunc_len[0])
+                qiime2_bash_str=qiime2_bash_str.replace("<p-trunc-len-r>",self.config.qiime2_p_trunc_len[1])
  
         if container=="None":
             qiime2_bash_str=qiime2_bash_str.replace("<manifest>",str(manifest_dir))
             qiime2_bash_str=qiime2_bash_str.replace("<qiime2_work_dir>",str(workings_dir))
             qiime2_bash_str=qiime2_bash_str.replace("<classifier>",str(self.config.qiime_classifier_db))
+            
         
         elif container=="docker":
             qiime2_bash_str=qiime2_bash_str.splitlines()
             for idx,line in enumerate(qiime2_bash_str):
                 line=line.lstrip()
                 if line.startswith("qiime") or line.startswith("biom"):
                     if not paired_end:
```

### Comparing `adtoolbox-0.5.6/adtoolbox/metagenomics_report.py` & `adtoolbox-0.5.7/adtoolbox/metagenomics_report.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/optimize.py` & `adtoolbox-0.5.7/adtoolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/pipeline.py` & `adtoolbox-0.5.7/adtoolbox/pipeline.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/pkg_data/.DS_Store` & `adtoolbox-0.5.7/adtoolbox/pkg_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/pkg_data/Modified_ADM_Map.json` & `adtoolbox-0.5.7/adtoolbox/pkg_data/Modified_ADM_Map.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/pkg_data/Modified_ADM_Model.json` & `adtoolbox-0.5.7/adtoolbox/pkg_data/Modified_ADM_Model.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/pkg_data/README.md` & `adtoolbox-0.5.7/adtoolbox/pkg_data/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/pkg_data/qiime_template_paired.txt` & `adtoolbox-0.5.7/adtoolbox/pkg_data/qiime_template_single.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-#!/bin/bash 
+#!/bin/bash
 qiime tools import \
---type 'SampleData[PairedEndSequencesWithQuality]' \
+--type 'SampleData[SequencesWithQuality]' \
 --input-path <manifest> \
---output-path <qiime2_work_dir>/demux-paired-end.qza \
---input-format PairedEndFastqManifestPhred33V2
-qiime dada2 denoise-paired \
---i-demultiplexed-seqs <qiime2_work_dir>/demux-paired-end.qza \
---p-trunc-len-f 150 \
---p-trunc-len-r 150 \
+--output-path <qiime2_work_dir>/demux-single-end.qza \
+--input-format SingleEndFastqManifestPhred33V2
+qiime dada2 denoise-single \
+--i-demultiplexed-seqs <qiime2_work_dir>/demux-single-end.qza \
+--p-trunc-len <p-trunc-len> \
 --p-n-threads 0 \
 --o-representative-sequences <qiime2_work_dir>/rep-seqs.qza \
 --o-table <qiime2_work_dir>/feature-table.qza \
 --o-denoising-stats <qiime2_work_dir>/stats.qza
 
-qiime feature-classifier classify-sklearn \
---i-classifier <classifier> \
---i-reads <qiime2_work_dir>/rep-seqs.qza \
---p-n-jobs 4 \
---o-classification <qiime2_work_dir>/taxonomy.qza
 
 qiime tools export \
 --input-path  <qiime2_work_dir>/feature-table.qza \
 --output-path  <qiime2_work_dir>
+
 qiime tools export \
 --input-path  <qiime2_work_dir>/rep-seqs.qza \
 --output-path  <qiime2_work_dir>/
+
 qiime tools export \
 --input-path  <qiime2_work_dir>/taxonomy.qza \
 --output-path  <qiime2_work_dir>/
 
+
 biom convert --to-tsv -i <qiime2_work_dir>/feature-table.biom -o <qiime2_work_dir>/feature-table.tsv
```

### Comparing `adtoolbox-0.5.6/adtoolbox/pkg_data/qiime_template_single.txt` & `adtoolbox-0.5.7/adtoolbox/pkg_data/qiime_template_paired.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-#!/bin/bash
+#!/bin/bash 
 qiime tools import \
---type 'SampleData[SequencesWithQuality]' \
+--type 'SampleData[PairedEndSequencesWithQuality]' \
 --input-path <manifest> \
---output-path <qiime2_work_dir>/demux-single-end.qza \
---input-format SingleEndFastqManifestPhred33V2
-qiime dada2 denoise-single \
---i-demultiplexed-seqs <qiime2_work_dir>/demux-single-end.qza \
---p-trunc-len 0 \
+--output-path <qiime2_work_dir>/demux-paired-end.qza \
+--input-format PairedEndFastqManifestPhred33V2
+
+qiime dada2 denoise-paired \
+--i-demultiplexed-seqs <qiime2_work_dir>/demux-paired-end.qza \
+--p-trunc-len-f <p-trunc-len-f> \
+--p-trunc-len-r <p-trunc-len-r> \
 --p-n-threads 0 \
 --o-representative-sequences <qiime2_work_dir>/rep-seqs.qza \
 --o-table <qiime2_work_dir>/feature-table.qza \
 --o-denoising-stats <qiime2_work_dir>/stats.qza
 
-qiime feature-classifier classify-sklearn \
---i-classifier <classifier> \
---i-reads <qiime2_work_dir>/rep-seqs.qza \
---p-n-jobs 4 \
---o-classification <qiime2_work_dir>/taxonomy.qza
-
 qiime tools export \
 --input-path  <qiime2_work_dir>/feature-table.qza \
 --output-path  <qiime2_work_dir>
-
 qiime tools export \
 --input-path  <qiime2_work_dir>/rep-seqs.qza \
 --output-path  <qiime2_work_dir>/
 
-qiime tools export \
---input-path  <qiime2_work_dir>/taxonomy.qza \
---output-path  <qiime2_work_dir>/
-
 
 biom convert --to-tsv -i <qiime2_work_dir>/feature-table.biom -o <qiime2_work_dir>/feature-table.tsv
```

### Comparing `adtoolbox-0.5.6/adtoolbox/stats.py` & `adtoolbox-0.5.7/adtoolbox/stats.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/tables.py` & `adtoolbox-0.5.7/adtoolbox/tables.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/adtoolbox/utils.py` & `adtoolbox-0.5.7/adtoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.6/pyproject.toml` & `adtoolbox-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adtoolbox"
-version = "0.5.6"
+version = "0.5.7"
 description = "A tool for modeling and optimization of anaerobic digestion process."
 authors = ["ParsaGhadermazi <54489047+ParsaGhadermazi@users.noreply.github.com>"]
 readme= "README.md"
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 bs4 = "^0.0.1"
 dash = "^2.4.1"
```

### Comparing `adtoolbox-0.5.6/setup.py` & `adtoolbox-0.5.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,17 +72,17 @@
  'sympy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ADToolbox = adtoolbox.__main__:main']}
 
 setup_kwargs = {
     'name': 'adtoolbox',
-    'version': '0.5.6',
+    'version': '0.5.7',
     'description': 'A tool for modeling and optimization of anaerobic digestion process.',
-    'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder or Colab:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">\n  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n[![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
+    'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder or Colab:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">\n  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n[![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)\n\n***NOTE***:Binder implementations don\'t offer escher map functionalities yet.\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
     'author': 'ParsaGhadermazi',
     'author_email': '54489047+ParsaGhadermazi@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `adtoolbox-0.5.6/PKG-INFO` & `adtoolbox-0.5.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adtoolbox
-Version: 0.5.6
+Version: 0.5.7
 Summary: A tool for modeling and optimization of anaerobic digestion process.
 Author: ParsaGhadermazi
 Author-email: 54489047+ParsaGhadermazi@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -33,13 +33,15 @@
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)
 <a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 [![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)
 
+***NOTE***:Binder implementations don't offer escher map functionalities yet.
+
 ADToolbox comes with a detailed documentation website. You can access this website using the link below:
 
 ** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **
```

