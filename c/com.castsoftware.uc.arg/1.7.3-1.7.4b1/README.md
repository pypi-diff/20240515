# Comparing `tmp/com_castsoftware_uc_arg-1.7.3.tar.gz` & `tmp/com_castsoftware_uc_arg-1.7.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com_castsoftware_uc_arg-1.7.3.tar", last modified: Thu Apr 18 19:40:44 2024, max compression
+gzip compressed data, was "com_castsoftware_uc_arg-1.7.4b1.tar", last modified: Wed May 15 21:23:03 2024, max compression
```

## Comparing `com_castsoftware_uc_arg-1.7.3.tar` & `com_castsoftware_uc_arg-1.7.4b1.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 19:40:44.635631 com_castsoftware_uc_arg-1.7.3/
--rw-rw-rw-   0        0        0      943 2024-04-18 19:40:44.590190 com_castsoftware_uc_arg-1.7.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 19:40:44.353321 com_castsoftware_uc_arg-1.7.3/cast_arg/
--rw-rw-rw-   0        0        0     1429 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/Effort.csv
--rw-rw-rw-   0        0        0        0 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/__init__.py
--rw-rw-rw-   0        0        0     8669 2024-02-14 14:50:20.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/actionPlan.py
--rw-rw-rw-   0        0        0      338 2023-12-20 18:51:05.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/apikey_test.py
--rw-rw-rw-   0        0        0     1004 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/cause.json
--rw-rw-rw-   0        0        0     7689 2024-02-05 21:42:15.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/config.py
--rw-rw-rw-   0        0        0    28200 2024-04-18 19:37:06.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/convert.py
--rw-rw-rw-   0        0        0      624 2023-08-25 16:17:25.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/keycloak_test.py
--rw-rw-rw-   0        0        0     1042 2024-02-05 15:11:37.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/main.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:40:44.496418 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/
--rw-rw-rw-   0        0        0        0 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/__init__.py
--rw-rw-rw-   0        0        0     6344 2023-11-28 18:25:50.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_benchmark.py
--rw-rw-rw-   0        0        0     4985 2024-04-12 21:15:49.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_cloud.py
--rw-rw-rw-   0        0        0     4567 2024-02-08 21:15:16.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_greenIt.py
--rw-rw-rw-   0        0        0     2344 2024-04-13 15:52:11.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_report.py
--rw-rw-rw-   0        0        0    11293 2024-04-15 19:53:46.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_summary.py
--rw-rw-rw-   0        0        0     3191 2023-12-27 13:33:57.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_grades.py
--rw-rw-rw-   0        0        0     1084 2024-01-05 20:20:49.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_overview.py
--rw-rw-rw-   0        0        0      890 2024-02-07 20:58:01.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_report.py
--rw-rw-rw-   0        0        0     4593 2024-03-15 19:02:18.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_sizing.py
--rw-rw-rw-   0        0        0     1780 2024-02-21 18:47:01.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_strengh_improvement.py
--rw-rw-rw-   0        0        0     3582 2024-03-15 20:51:57.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_tech_detail_table.py
--rw-rw-rw-   0        0        0     9012 2024-02-14 21:54:47.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/powerpoint.py
--rw-rw-rw-   0        0        0    34636 2024-02-20 19:28:49.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/restCall.py
--rw-rw-rw-   0        0        0     7182 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/stats.py
--rw-rw-rw-   0        0        0    14091 2024-01-28 17:19:54.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/test copy.py
--rw-rw-rw-   0        0        0    11974 2024-01-29 19:02:47.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:40:44.578467 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/
--rw-rw-rw-   0        0        0      943 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      919 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      817 2024-04-18 19:39:27.000000 com_castsoftware_uc_arg-1.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 19:40:44.635631 com_castsoftware_uc_arg-1.7.3/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:23:03.115862 com_castsoftware_uc_arg-1.7.4b1/
+-rw-rw-rw-   0        0        0     2328 2024-05-15 21:23:03.101658 com_castsoftware_uc_arg-1.7.4b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 21:23:02.822434 com_castsoftware_uc_arg-1.7.4b1/cast_arg/
+-rw-rw-rw-   0        0        0     1429 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/Effort.csv
+-rw-rw-rw-   0        0        0        0 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/__init__.py
+-rw-rw-rw-   0        0        0     8669 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/actionPlan.py
+-rw-rw-rw-   0        0        0     1004 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/cause.json
+-rw-rw-rw-   0        0        0     7689 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/config.py
+-rw-rw-rw-   0        0        0    28583 2024-05-07 15:10:56.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/convert.py
+-rw-rw-rw-   0        0        0     1105 2024-04-29 21:58:10.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:23:02.974808 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/
+-rw-rw-rw-   0        0        0        0 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_benchmark.py
+-rw-rw-rw-   0        0        0     5044 2024-05-09 16:55:39.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_cloud.py
+-rw-rw-rw-   0        0        0     4567 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_greenIt.py
+-rw-rw-rw-   0        0        0     2344 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_report.py
+-rw-rw-rw-   0        0        0    11296 2024-05-07 18:27:33.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_summary.py
+-rw-rw-rw-   0        0        0     3191 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_grades.py
+-rw-rw-rw-   0        0        0     1084 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_overview.py
+-rw-rw-rw-   0        0        0      890 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_report.py
+-rw-rw-rw-   0        0        0     4593 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_sizing.py
+-rw-rw-rw-   0        0        0     1780 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_strengh_improvement.py
+-rw-rw-rw-   0        0        0     3582 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_tech_detail_table.py
+-rw-rw-rw-   0        0        0     8800 2024-05-07 15:30:59.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/powerpoint.py
+-rw-rw-rw-   0        0        0    34636 2024-04-24 18:49:23.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/restCall.py
+-rw-rw-rw-   0        0        0     7182 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/cast_arg/stats.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:23:03.091066 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/
+-rw-rw-rw-   0        0        0     2328 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 21:23:02.000000 com_castsoftware_uc_arg-1.7.4b1/com.castsoftware.uc.arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      819 2024-05-15 21:22:26.000000 com_castsoftware_uc_arg-1.7.4b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 21:23:03.115862 com_castsoftware_uc_arg-1.7.4b1/setup.cfg
+-rw-rw-rw-   0        0        0      422 2024-04-24 15:47:20.000000 com_castsoftware_uc_arg-1.7.4b1/setup.py
```

### Comparing `com_castsoftware_uc_arg-1.7.3/PKG-INFO` & `com_castsoftware_uc_arg-1.7.4b1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1
-Name: com.castsoftware.uc.arg
-Version: 1.7.3
-Summary: Assessment Report Generator (ARG)
-Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
-Author-email: Nevin Kaplan <n.kaplan@castsoftware.com>, DD Assessment Team <Team.ddassessments@castsoftware.com>
-Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
-Project-URL: documentation, https://github.com/CAST-Extend/com.castsoftware.uc.arg/wiki
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: python-pptx==0.6.19
-Requires-Dist: com.castsoftware.uc.python.common>=1.1.11
-Requires-Dist: IPython
-Requires-Dist: requests
-Requires-Dist: Jinja2
-Requires-Dist: setuptools
-Requires-Dist: inflect
+[project]
+name='com.castsoftware.uc.arg'
+description="Assessment Report Generator (ARG)"
+version='1.7.4b1' #prod version
+authors= [
+    {name="Nevin Kaplan",email="n.kaplan@castsoftware.com"},
+    {name="DD Assessment Team",email="Team.ddassessments@castsoftware.com"}
+]
+readme="README.md"
+dependencies = ['pandas', 'python-pptx==0.6.19', 'com.castsoftware.uc.python.common>=1.1.12', 'IPython', 'requests', 'Jinja2','setuptools','inflect']
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: OS Independent",
+]
+requires-python = ">=3.6"
+[project.urls]
+Homepage = "https://github.com/CAST-Extend/com.castsoftware.uc.arg"
+documentation="https://github.com/CAST-Extend/com.castsoftware.uc.arg/wiki"
```

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/Effort.csv` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/Effort.csv`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/actionPlan.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/actionPlan.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/cause.json` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/cause.json`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/config.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/config.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/convert.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from cast_arg.stats import OssStats,AIPStats,LicenseStats
 
 
 
 from cast_common.mri import MRI
 from cast_common.logger import Logger,DEBUG, INFO, WARN
-from cast_common.util import find_nth, no_dups, list_to_text,format_table
+from cast_common.util import find_nth, no_dups, list_to_text,create_folder,yes_no_input
 from cast_arg.powerpoint import PowerPoint
 from cast_common.highlight import Highlight
 
 from copy import deepcopy
 
 from pandas import DataFrame
 from pptx import Presentation
@@ -57,19 +57,24 @@
 
     day_rate=1600
 
     def __init__(self, config:Config):
         super().__init__("generate",config.logging_generate)
         self._config = config
 
+        self._ppt = PowerPoint(config)
         out = abspath(f"{config.output}/Project {config.project} - Tech DD Findings.pptx")
         self.out=out
         self.info(f'Generating {out}')
-
-        self._ppt = PowerPoint(config)
+        if not exists(dirname(out)):
+            if yes_no_input(f'{dirname(out)} does not exist, create it now'):
+                create_folder(dirname(out))
+            else:
+                self.info('Aborting report generation')
+                return
 
         # TODO: Handle cases where on HL data is needed and not AIP.
         self.hl_pages = []
         if config.aip_active:
             self.info("Collecting AIP Data")
             try:
                 self._aip_data = AipData(config,log_level=config.logging_aip)
@@ -105,21 +110,26 @@
 
         if app_cnt == 1: 
             s = self._ppt.get_shape_by_name('port_level_slide')
             pass
             #self._ppt.delete_slide
         else:
             self._ppt.duplicate_slides(app_cnt)
+            self._ppt.save()
+            # exit()
+            
             self._ppt.copy_block("each_app",["app"],app_cnt)
             # self._ppt.save()
             # return 
 
         self._ppt.replace_text("{app_per_page}","",tbd_for_blanks=False)
 
-        self.expand_tables(config,['project_overview'])
+        if self._config.aip_active:
+            self.expand_tables(config,['project_overview'])
+
         self.replace_all_text()
 
     def expand_tables(self,config:Config,table_names:list):
         app_cnt = len(config.application)
         for tbl_name in table_names:
             try:
                 table = self._ppt.get_shape_by_name(tbl_name)
```

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/main.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,9 +17,12 @@
     print('Copyright (c) 2023 CAST Software Inc.')
     print('If you need assistance, please contact oneclick@castsoftware.com')
 
     parser = ArgumentParser(description='Assessment Report Generation Tool')
     parser.add_argument('-c','--config', required=True, help='Configuration properties file')
     args = parser.parse_args()
     config=Config(args.config)
-    GeneratePPT(config)._ppt.save()
+    try:
+        GeneratePPT(config)._ppt.save()
+    except Exception as ex:
+        print (ex)
```

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_benchmark.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_benchmark.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_cloud.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_cloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,20 @@
             # self.ppt.replace_text(f'{{{self.tag_prefix}_hl_cloud_total_boosters}}',round(metrics['boosters']*100,1),slide=self.slide)
             self.get_cloud_totals(data)
                 
             # update the techology chart
             agr = data[['Technology','NB Roadblocks']].groupby('Technology').aggregate('sum').reindex()
             self.ppt.update_chart(f'{self.tag_prefix}_CloudTechPieChart',agr)
 
-            data = data.drop(columns=['Files'])
+            data = data.drop(columns=['Files']).sort_values(['Rule Types','NB Roadblocks','Technology'])
             self.ppt.update_table(f'{self.tag_prefix}_CloudDetailTable',data,app,include_index=False)  
             pass      
         except Exception as ex:
             ex_type, ex_value, ex_traceback = exc_info()
-            self.log.error(f'{ex_type.__name__}: {ex_value} while in {__class__}')
+            self.log.warning(f'{ex_type.__name__}: {ex_value} while in {__class__}')
             status = False
 
         return status
 
     def get_data(self,app:str):
         df = self.get_cloud_detail(app)
         df = df.rename(columns={'technology':'Technology',
```

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_greenIt.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_greenIt.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_report.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_report.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_summary.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/hl_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             pass
 
         text = {
             'quality':{'high':'high','medium':'moderate','low':'low-level'},
             'improvement':{'high':'no immediate action required','medium':'room for improvement','low':'ample opportunity for improvement'},
             'maintain':{'high':'highly maintainable','medium':'maintainable but needs improvement','low':'is not maintainable'},
 
-            'quality_alt_1':{'high':'well','medium':'fair','low':'bad'},
+            'quality_alt_1':{'high':'well','medium':'fair','low':'poorly'},
             'quality_alt_2':{'high':'impressive','medium':'fair','low':'poor'},
             'quality_alt_3':{'high':'stands out','medium':'average','low':'in need of improvement'},
             'maturity':{'high':'high','medium':'medium','low':'low'},
             'effort':{'high':'minimal','medium':'medium','low':'considerable'},
             'risk':{'high':'low amount of','medium':'average','low':'very high'}
         }
 
@@ -143,16 +143,16 @@
                         cmpnt_df['component']=df['component']
                         if not cmpnt_df.empty:
                             total_cmpnts_df = concat([cmpnt_df,total_cmpnts_df])
                             eff = ceil(len(cmpnt_df['component'].unique())/2)
                         cnt = len(df['cve'].unique())
                         total_cves += cnt
 
-                    self.replace_text(f'{key}_cve_total',cnt)
-                    self.replace_text(f'{key}_cve_effort',eff)
+                    self.replace_text(f'{key}_oss_total',cnt)
+                    self.replace_text(f'{key}_oss_effort',eff)
                     pass
     
                 self.replace_text('cve_total',total_cves)
                 total_eff = 0
                 if not total_cmpnts_df.empty:
                     total_eff = ceil(len(total_cmpnts_df['component'].unique())/2)
                     self.replace_text(f'{key}_total_cve_effort',total_eff)
```

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_grades.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_grades.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_overview.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_overview.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_report.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_report.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_sizing.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_sizing.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_strengh_improvement.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_strengh_improvement.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_tech_detail_table.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/pages/mri_tech_detail_table.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/powerpoint.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/powerpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 from cast_common.powerpoint import PowerPoint as common_ppt
+from cast_common.util import yes_no_input
 from cast_common.logger import INFO
 from cast_arg.config import Config
 from pptx.chart.data import CategoryChartData
 from pandas import Series,DataFrame
 from os.path import abspath
 
 __author__ = "Nevin Kaplan"
 __email__ = "n.kaplan@castsoftware.com"
 __copyright__ = "Copyright 2022, CAST Software"
 
-def yes_no_response(msg:str) -> bool:
-    while answer := input (f'{msg},  [Y or N]?'):
-        if answer.upper() == 'Y':
-            return True
-        elif answer.upper() == 'N':
-            return False
-        else:
-            continue
-
 def numeric_response(msg:str,value:int,max_rows) -> int:
     msg_str=msg
     while True:
         first = True
         answer = input(f'{msg_str}: ')
         if len(answer)==0:
             answer = f'{value}'
@@ -56,15 +48,15 @@
     def save(self):
         while True:
             try:
                 self._prs.save(self._out)
                 self.log.info(f'{self._out} saved.')
                 return 
             except PermissionError as pe: 
-                if not yes_no_response(f'Error writing {self._out} powerpoint document, Retry'):
+                if not yes_no_input(f'Error writing {self._out} powerpoint document, Retry'):
                     return 
             except Exception as ex:
                 self.log.error(f'General Exception while saving PowerPoint document: {ex}')
                 raise ex
 
 
     def update_table(self,name,data:DataFrame, app:str,
```

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/restCall.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/restCall.py`

 * *Files identical despite different names*

### Comparing `com_castsoftware_uc_arg-1.7.3/cast_arg/stats.py` & `com_castsoftware_uc_arg-1.7.4b1/cast_arg/stats.py`

 * *Files identical despite different names*

