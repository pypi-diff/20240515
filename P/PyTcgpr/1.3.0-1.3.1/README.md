# Comparing `tmp/PyTcgpr-1.3.0.tar.gz` & `tmp/PyTcgpr-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTcgpr-1.3.0.tar", last modified: Tue Dec 26 11:54:58 2023, max compression
+gzip compressed data, was "PyTcgpr-1.3.1.tar", last modified: Wed May 15 10:05:43 2024, max compression
```

## Comparing `PyTcgpr-1.3.0.tar` & `PyTcgpr-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-12-26 11:54:58.022365 PyTcgpr-1.3.0/
--rw-r--r--   0 jacob      (501) staff       (20)     1243 2023-12-26 11:54:58.022163 PyTcgpr-1.3.0/PKG-INFO
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-12-26 11:54:58.020627 PyTcgpr-1.3.0/PyTcgpr/
--rw-rw-rw-   0 jacob      (501) staff       (20)    12546 2023-12-26 11:46:29.000000 PyTcgpr-1.3.0/PyTcgpr/TCGPR.py
--rw-r--r--   0 jacob      (501) staff       (20)     1154 2023-07-17 01:51:15.000000 PyTcgpr-1.3.0/PyTcgpr/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-12-26 11:54:58.021669 PyTcgpr-1.3.0/PyTcgpr/data/
--rw-rw-rw-   0 jacob      (501) staff       (20)    21836 2023-12-26 11:41:32.000000 PyTcgpr-1.3.0/PyTcgpr/data/DatasetPartition.py
--rw-rw-rw-   0 jacob      (501) staff       (20)    17680 2023-12-26 11:42:12.000000 PyTcgpr-1.3.0/PyTcgpr/data/OutliersIdentification.py
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.3.0/PyTcgpr/data/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-12-26 11:54:58.021930 PyTcgpr-1.3.0/PyTcgpr/feature/
--rw-rw-rw-   0 jacob      (501) staff       (20)    24282 2023-12-26 11:46:33.000000 PyTcgpr-1.3.0/PyTcgpr/feature/FeaturesSelection.py
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.3.0/PyTcgpr/feature/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-12-26 11:54:58.021242 PyTcgpr-1.3.0/PyTcgpr.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1243 2023-12-26 11:54:57.000000 PyTcgpr-1.3.0/PyTcgpr.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      371 2023-12-26 11:54:57.000000 PyTcgpr-1.3.0/PyTcgpr.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-12-26 11:54:57.000000 PyTcgpr-1.3.0/PyTcgpr.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       21 2023-12-26 11:54:57.000000 PyTcgpr-1.3.0/PyTcgpr.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        8 2023-12-26 11:54:57.000000 PyTcgpr-1.3.0/PyTcgpr.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)      550 2023-12-26 11:54:50.000000 PyTcgpr-1.3.0/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-12-26 11:54:58.022405 PyTcgpr-1.3.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1404 2023-12-26 11:47:43.000000 PyTcgpr-1.3.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-15 10:05:43.547663 PyTcgpr-1.3.1/
+-rw-r--r--   0 jacob      (501) staff       (20)     1243 2024-05-15 10:05:43.547429 PyTcgpr-1.3.1/PKG-INFO
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-15 10:05:43.545877 PyTcgpr-1.3.1/PyTcgpr/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    12554 2024-05-15 10:03:57.000000 PyTcgpr-1.3.1/PyTcgpr/TCGPR.py
+-rw-r--r--   0 jacob      (501) staff       (20)      351 2024-05-15 10:04:19.000000 PyTcgpr-1.3.1/PyTcgpr/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-15 10:05:43.546931 PyTcgpr-1.3.1/PyTcgpr/data/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    21836 2023-12-26 11:41:32.000000 PyTcgpr-1.3.1/PyTcgpr/data/DatasetPartition.py
+-rw-rw-rw-   0 jacob      (501) staff       (20)    17680 2023-12-26 11:42:12.000000 PyTcgpr-1.3.1/PyTcgpr/data/OutliersIdentification.py
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.3.1/PyTcgpr/data/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-15 10:05:43.547193 PyTcgpr-1.3.1/PyTcgpr/feature/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    24282 2023-12-26 11:46:33.000000 PyTcgpr-1.3.1/PyTcgpr/feature/FeaturesSelection.py
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.3.1/PyTcgpr/feature/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-15 10:05:43.546507 PyTcgpr-1.3.1/PyTcgpr.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1243 2024-05-15 10:05:43.000000 PyTcgpr-1.3.1/PyTcgpr.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      371 2024-05-15 10:05:43.000000 PyTcgpr-1.3.1/PyTcgpr.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2024-05-15 10:05:43.000000 PyTcgpr-1.3.1/PyTcgpr.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       21 2024-05-15 10:05:43.000000 PyTcgpr-1.3.1/PyTcgpr.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        8 2024-05-15 10:05:43.000000 PyTcgpr-1.3.1/PyTcgpr.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)      550 2023-12-26 11:54:50.000000 PyTcgpr-1.3.1/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2024-05-15 10:05:43.547706 PyTcgpr-1.3.1/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1404 2024-05-15 10:05:10.000000 PyTcgpr-1.3.1/setup.py
```

### Comparing `PyTcgpr-1.3.0/PKG-INFO` & `PyTcgpr-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTcgpr
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.
 Home-page: https://github.com/Bin-Cao/TCGPR
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: 17734910905@163.com
 License: MIT License
```

### Comparing `PyTcgpr-1.3.0/PyTcgpr/TCGPR.py` & `PyTcgpr-1.3.1/PyTcgpr/TCGPR.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Guangzhou Municipal Key Laboratory of Materials Informatics, Advanced Materials Thrust,
     Hong Kong University of Science and Technology (Guangzhou), Guangzhou 511400, Guangdong, China
 
     ==================================================================
     Please feel free to open issues in the Github :
     https://github.com/Bin-Cao/TCGPR
     or 
-    contact Mr.Bin Cao (bcao@shu.edu.cn)
+    contact Mr.Bin Cao (binjacobcao@gmail.com)
     in case of any problems/comments/suggestions in using the code. 
     ==================================================================
 
     Parameters
     ----------
     :param defined in TCGPR
     ==================================================================
@@ -249,15 +249,15 @@
             if ratio == None:
                 ratio = 0.0
             DataOutI(filePath=filePath, sampling_cap=sampling_cap, measure=measure,ratio=ratio, up_search = up_search,target = target, weight=weight,exploit_coef=exploit_coef,
                 CV=CV,alpha=alpha, n_restarts_optimizer=n_restarts_optimizer,normalize_y=normalize_y, exploit_model = exploit_model)
             print('The Outliers has been deleted !')
             print('='*100)
 
-    if Mission == 'FEATURE':
+    elif Mission == 'FEATURE':
         if up_search == None:
             up_search = 10
         if ratio == None:
             ratio = -0.1
         print('Execution of TCGPR : Feature Selection Module')
         Feature(filePath=filePath, initial_set_cap=initial_set_cap, sampling_cap=sampling_cap, measure=measure,ratio=ratio, up_search = up_search, target = target,weight=weight, exploit_coef=exploit_coef,
             CV=CV,alpha=alpha, n_restarts_optimizer=n_restarts_optimizer,normalize_y=normalize_y, exploit_model = exploit_model)
```

### Comparing `PyTcgpr-1.3.0/PyTcgpr/data/DatasetPartition.py` & `PyTcgpr-1.3.1/PyTcgpr/data/DatasetPartition.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.3.0/PyTcgpr/data/OutliersIdentification.py` & `PyTcgpr-1.3.1/PyTcgpr/data/OutliersIdentification.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.3.0/PyTcgpr/feature/FeaturesSelection.py` & `PyTcgpr-1.3.1/PyTcgpr/feature/FeaturesSelection.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.3.0/PyTcgpr.egg-info/PKG-INFO` & `PyTcgpr-1.3.1/PyTcgpr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTcgpr
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.
 Home-page: https://github.com/Bin-Cao/TCGPR
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: 17734910905@163.com
 License: MIT License
```

### Comparing `PyTcgpr-1.3.0/README.md` & `PyTcgpr-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.3.0/setup.py` & `PyTcgpr-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='PyTcgpr',  # 包名
-    version='1.3.0',  # 版本
+    version='1.3.1',  # 版本
     description="Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='17734910905@163.com',  # 维护者邮件
```

