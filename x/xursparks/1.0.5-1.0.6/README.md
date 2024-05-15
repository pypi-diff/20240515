# Comparing `tmp/xursparks-1.0.5.tar.gz` & `tmp/xursparks-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xursparks-1.0.5.tar", last modified: Mon May  6 03:24:34 2024, max compression
+gzip compressed data, was "xursparks-1.0.6.tar", last modified: Wed May 15 01:15:49 2024, max compression
```

## Comparing `xursparks-1.0.5.tar` & `xursparks-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-06 03:24:34.406768 xursparks-1.0.5/
--rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-05-06 03:24:34.406768 xursparks-1.0.5/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)     5345 2024-04-03 04:21:12.000000 xursparks-1.0.5/README.md
--rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.5/pyproject.toml
--rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-06 03:24:34.406768 xursparks-1.0.5/setup.cfg
--rw-rw-r--   0 doods     (1000) doods     (1000)      779 2024-05-06 02:43:55.000000 xursparks-1.0.5/setup.py
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-06 03:24:34.406768 xursparks-1.0.5/xursparks/
--rw-rw-r--   0 doods     (1000) doods     (1000)    34868 2024-05-06 01:38:42.000000 xursparks-1.0.5/xursparks/__init__.py
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-06 03:24:34.406768 xursparks-1.0.5/xursparks.egg-info/
--rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-05-06 03:24:34.000000 xursparks-1.0.5/xursparks.egg-info/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)      219 2024-05-06 03:24:34.000000 xursparks-1.0.5/xursparks.egg-info/SOURCES.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-06 03:24:34.000000 xursparks-1.0.5/xursparks.egg-info/dependency_links.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)       46 2024-05-06 03:24:34.000000 xursparks-1.0.5/xursparks.egg-info/requires.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)       10 2024-05-06 03:24:34.000000 xursparks-1.0.5/xursparks.egg-info/top_level.txt
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-15 01:15:49.481511 xursparks-1.0.6/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7792 2024-05-15 01:15:49.481511 xursparks-1.0.6/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7278 2024-05-15 00:58:02.000000 xursparks-1.0.6/README.md
+-rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.6/pyproject.toml
+-rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-15 01:15:49.481511 xursparks-1.0.6/setup.cfg
+-rw-rw-r--   0 doods     (1000) doods     (1000)      840 2024-05-15 01:15:44.000000 xursparks-1.0.6/setup.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-15 01:15:49.481511 xursparks-1.0.6/xursparks/
+-rw-rw-r--   0 doods     (1000) doods     (1000)    36126 2024-05-15 01:05:33.000000 xursparks-1.0.6/xursparks/__init__.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-15 01:15:49.481511 xursparks-1.0.6/xursparks.egg-info/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7792 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)      219 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/SOURCES.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/dependency_links.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)       66 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/requires.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)       10 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/top_level.txt
```

### Comparing `xursparks-1.0.5/setup.py` & `xursparks-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xursparks',
-    version='1.0.5',
+    version='1.0.6',
     packages=['xursparks'],
+    python_requires=">=3.10",
     install_requires=[
         'requests',
         'pandas',
         'pyspark',
         'boto3',
         'ydata-profiling',
+        'xurpas_data_quality',
     ],
     author='Randell Gabriel Santos',
     author_email='randellsantos@gmail.com',
-    description='Encapsulating Apache Spark for easy usage',
+    description='Encapsulating Apache Spark for Easy Usage',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dev-doods687/xursparks',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
```

### Comparing `xursparks-1.0.5/xursparks/__init__.py` & `xursparks-1.0.6/xursparks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from dateutil.relativedelta import relativedelta
 from datetime import date as dt, timedelta
 from urllib.parse import quote
 from email.mime.base import MIMEBase
 from email import encoders
+from xurpas_data_quality import DataReport
 
 def initialize(args):
 	#initialize global variables
 	global jobArguments
 	global customJobArgs
 	global targetTableDataset
 	global writeDate
@@ -912,29 +913,62 @@
 			for obj in page['Contents']:
 				s3.put_object_acl(ACL=permission, Bucket=bucket_name, Key=obj['Key'])
 				print(f"Permissions updated for {obj['Key']}")
 
 def generateDataProfiling():
 	df = targetTableDataset.toPandas()
 	title = f'{targetTable.get("database_name")}_{targetTable.get("table_name")}'
-	profile = ProfileReport(df, title=f'{title}')
 	filePath = f'{os.path.dirname(__file__)}/{targetTable.get("database_name")}_{targetTable.get("table_name")}.html'
+	profile = ProfileReport(df, title=f'{title}')
 	profile.to_file(f'{filePath}')
 	# read the HTML file
 	with open(filePath, 'r') as f:
 		html_content = f.read()
 	recipients = auditOptions.get("recipients")
 	if(optionalParams.get("audit.recipients") != None and len(optionalParams.get("audit.recipients")) > 0):
 		recipients = f'{recipients},optionalParams.get("audit.recipients")'
 	emailRecipients = recipients.split(",")
 	files = [filePath]
 	rename = [f'{title}.html']
 	sendEmail(subject=f'Data Profile[{title}]-{processDate}', message='Hi', from_email=auditOptions.get("sender"), 
 		to_email=emailRecipients, files=files, rename=rename)
 
+def generateDataQualityReport(**kwargs):
+	title = kwargs.get("dq_title")
+	filePath = kwargs.get("dq_file_path")
+	df = kwargs.get("dq_df")
+	message = kwargs.get("dq_message")
+
+	if(title == None):
+		title = f'{targetTable.get("database_name")}_{targetTable.get("table_name")}'
+	if(filePath == None):
+		filePath = f'{os.path.dirname(__file__)}/{targetTable.get("database_name")}_{targetTable.get("table_name")}.html'
+	if(df == None):
+		df = targetTableDataset.toPandas()
+	if(message == None):
+		message = 'Hi'
+	
+	# integration with XAIL DQ reporting library
+	report = DataReport(df=df,
+		report_name=title, 
+		file_path=f'{filePath}')
+	report.to_file()
+
+	# read the HTML file
+	with open(filePath, 'r') as f:
+		html_content = f.read()
+	recipients = auditOptions.get("recipients")
+	if(optionalParams.get("audit.recipients") != None and len(optionalParams.get("audit.recipients")) > 0):
+		recipients = f'{recipients},optionalParams.get("audit.recipients")'
+	emailRecipients = recipients.split(",")
+	files = [filePath]
+	rename = [f'{title}.html']
+	sendEmail(subject=f'Data Profile[{title}]-{processDate}', message={message}, from_email=auditOptions.get("sender"), 
+		to_email=emailRecipients, files=files, rename=rename)
+
 def createHiveTable():
 	hive_database = targetTable.get("database_name")
 	hive_table = targetTable.get("table_name")
 	partition_column = targetTable.get("partition_name").lower()
 	partition_value = processDate.strftime(targetTable.get("partition_date_format"))
 	hdfs_path = generateWritePath()
```

