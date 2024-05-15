# Comparing `tmp/computenest-cli-1.2.7.tar.gz` & `tmp/computenest-cli-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computenest-cli-1.2.7.tar", last modified: Wed Apr  3 03:29:30 2024, max compression
+gzip compressed data, was "computenest-cli-1.2.8.tar", last modified: Wed May 15 09:44:46 2024, max compression
```

## Comparing `computenest-cli-1.2.7.tar` & `computenest-cli-1.2.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.038373 computenest-cli-1.2.7/
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1916 2024-04-03 03:29:30.037793 computenest-cli-1.2.7/PKG-INFO
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1669 2024-03-08 01:57:25.000000 computenest-cli-1.2.7/README.md
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.017685 computenest-cli-1.2.7/computenest_cli.egg-info/
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1916 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/PKG-INFO
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1116 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/SOURCES.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)        1 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/dependency_links.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)       61 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/entry_points.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)      230 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/requires.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)       15 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/top_level.txt
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.018772 computenest-cli-1.2.7/computenestcli/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/__init__.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.022084 computenest-cli-1.2.7/computenestcli/client/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/__init__.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      418 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/base.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      785 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/computenest.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      525 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/ecs.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      525 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/oos.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.026754 computenest-cli-1.2.7/computenestcli/common/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/__init__.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1753 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/constant.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      146 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/context.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      236 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/credentials.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      670 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/decorator.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     2102 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/util.py
--rwxr-xr-x   0 xuhaoran   (502) staff       (20)     4130 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/main.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.031852 computenest-cli-1.2.7/computenestcli/processor/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/__init__.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)    17199 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/artifact.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     4448 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/check.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     6753 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/image.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     2197 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/jinja2.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)    20467 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/service.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.036727 computenest-cli-1.2.7/computenestcli/service/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/__init__.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     8354 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/artifact.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      606 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/base.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1002 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/credentials.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     2903 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/file.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     3253 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/image.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     5508 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/supplier.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)       38 2024-04-03 03:29:30.038510 computenest-cli-1.2.7/setup.cfg
--rw-r--r--   0 xuhaoran   (502) staff       (20)      783 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/setup.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-05-15 09:44:46.116656 computenest-cli-1.2.8/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1916 2024-05-15 09:44:46.115725 computenest-cli-1.2.8/PKG-INFO
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1669 2024-03-08 01:57:25.000000 computenest-cli-1.2.8/README.md
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-05-15 09:44:46.030504 computenest-cli-1.2.8/computenest_cli.egg-info/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1916 2024-05-15 09:44:45.000000 computenest-cli-1.2.8/computenest_cli.egg-info/PKG-INFO
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1116 2024-05-15 09:44:45.000000 computenest-cli-1.2.8/computenest_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        1 2024-05-15 09:44:45.000000 computenest-cli-1.2.8/computenest_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 xuhaoran   (502) staff       (20)       61 2024-05-15 09:44:45.000000 computenest-cli-1.2.8/computenest_cli.egg-info/entry_points.txt
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      230 2024-05-15 09:44:45.000000 computenest-cli-1.2.8/computenest_cli.egg-info/requires.txt
+-rw-r--r--   0 xuhaoran   (502) staff       (20)       15 2024-05-15 09:44:45.000000 computenest-cli-1.2.8/computenest_cli.egg-info/top_level.txt
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-05-15 09:44:46.031998 computenest-cli-1.2.8/computenestcli/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/__init__.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-05-15 09:44:46.036711 computenest-cli-1.2.8/computenestcli/client/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/client/__init__.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      418 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/client/base.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      785 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/client/computenest.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      525 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/client/ecs.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      525 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/client/oos.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-05-15 09:44:46.043075 computenest-cli-1.2.8/computenestcli/common/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/common/__init__.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1753 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/common/constant.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      146 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/common/context.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      236 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/common/credentials.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      670 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/common/decorator.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     2102 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/common/util.py
+-rwxr-xr-x   0 xuhaoran   (502) staff       (20)     4130 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/main.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-05-15 09:44:46.101695 computenest-cli-1.2.8/computenestcli/processor/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/processor/__init__.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)    17199 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/processor/artifact.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     4448 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/processor/check.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     6753 2024-04-24 03:43:20.000000 computenest-cli-1.2.8/computenestcli/processor/image.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     2197 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/processor/jinja2.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)    20713 2024-05-15 06:14:25.000000 computenest-cli-1.2.8/computenestcli/processor/service.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-05-15 09:44:46.113887 computenest-cli-1.2.8/computenestcli/service/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/service/__init__.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     8354 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/service/artifact.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      606 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/service/base.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1002 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/service/credentials.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     2903 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/service/file.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     3253 2024-04-03 03:28:56.000000 computenest-cli-1.2.8/computenestcli/service/image.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     5599 2024-05-15 04:43:25.000000 computenest-cli-1.2.8/computenestcli/service/supplier.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)       38 2024-05-15 09:44:46.116902 computenest-cli-1.2.8/setup.cfg
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      783 2024-05-15 09:44:21.000000 computenest-cli-1.2.8/setup.py
```

### Comparing `computenest-cli-1.2.7/PKG-INFO` & `computenest-cli-1.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computenest-cli
-Version: 1.2.7
+Version: 1.2.8
 Summary: A command line interface for running the compute nest project
 Home-page: 
 Author: Chuan Lin
 Author-email: zhaoshuaibo.zsb@alibaba-inc.com
 Description-Content-Type: text/markdown
 
 # ComputeNest-CLI
```

### Comparing `computenest-cli-1.2.7/README.md` & `computenest-cli-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenest_cli.egg-info/PKG-INFO` & `computenest-cli-1.2.8/computenest_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computenest-cli
-Version: 1.2.7
+Version: 1.2.8
 Summary: A command line interface for running the compute nest project
 Home-page: 
 Author: Chuan Lin
 Author-email: zhaoshuaibo.zsb@alibaba-inc.com
 Description-Content-Type: text/markdown
 
 # ComputeNest-CLI
```

### Comparing `computenest-cli-1.2.7/computenest_cli.egg-info/SOURCES.txt` & `computenest-cli-1.2.8/computenest_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/client/computenest.py` & `computenest-cli-1.2.8/computenestcli/client/computenest.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/client/ecs.py` & `computenest-cli-1.2.8/computenestcli/client/ecs.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/client/oos.py` & `computenest-cli-1.2.8/computenestcli/client/oos.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/common/constant.py` & `computenest-cli-1.2.8/computenestcli/common/constant.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/common/decorator.py` & `computenest-cli-1.2.8/computenestcli/common/decorator.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/common/util.py` & `computenest-cli-1.2.8/computenestcli/common/util.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/main.py` & `computenest-cli-1.2.8/computenestcli/main.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/processor/artifact.py` & `computenest-cli-1.2.8/computenestcli/processor/artifact.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/processor/check.py` & `computenest-cli-1.2.8/computenestcli/processor/check.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/processor/image.py` & `computenest-cli-1.2.8/computenestcli/processor/image.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/processor/jinja2.py` & `computenest-cli-1.2.8/computenestcli/processor/jinja2.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/processor/service.py` & `computenest-cli-1.2.8/computenestcli/processor/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,19 +190,20 @@
         if len(data_list.body.services) == 0:
             if icon:
                 service_config[constant.SERVICE_INFO][constant.IMAGE] = icon
             else:
                 # 将服务logo的本地路径替换成Url
                 service_config[constant.SERVICE_INFO][constant.IMAGE] = self._replace_file_path_with_url(image_path)
             # 将模版文件的本地路径替换成url
-            for template in deploy_metadata_config.get(constant.TEMPLATE_CONFIGS):
-                # 将相对路径替换成绝对路径
-                if template.get(constant.URL):
-                    template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
-                    template[constant.URL] = self._replace_file_path_with_url(template_path)
+            if deploy_metadata_config.get(constant.TEMPLATE_CONFIGS):
+                for template in deploy_metadata_config.get(constant.TEMPLATE_CONFIGS):
+                    # 将相对路径替换成绝对路径
+                    if template.get(constant.URL):
+                        template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
+                        template[constant.URL] = self._replace_file_path_with_url(template_path)
             # 将SupplierDeployMetadata的路径做替换
             if constant.SUPPLIER_DEPLOY_METADATA in deploy_metadata_config:
                 supplier_deploy_metadata = deploy_metadata_config.get(constant.SUPPLIER_DEPLOY_METADATA)
                 if constant.SUPPLIER_TEMPLATE_CONFIGS in supplier_deploy_metadata:
                     for supplier_template_config in supplier_deploy_metadata.get(constant.SUPPLIER_TEMPLATE_CONFIGS):
                         template_path = os.path.join(os.path.dirname(file_path),
                                                      supplier_template_config.get(constant.URL))
@@ -227,15 +228,16 @@
                 if result_image:
                     image_url = image_url_existed
                 else:
                     image_url = self._replace_file_path_with_url(image_path)
                 service_config[constant.SERVICE_INFO][constant.IMAGE] = image_url
 
             service_deploy_metadata = json.loads(self._get_template_url_data(service_name))
-            if service_deploy_metadata and service_deploy_metadata.get(constant.TEMPLATE_CONFIGS):
+            if service_deploy_metadata and service_deploy_metadata.get(constant.TEMPLATE_CONFIGS) and \
+                    service_config.get(constant.DEPLOY_METADATA).get(constant.TEMPLATE_CONFIGS):
                 name_url_mapping = {template[constant.NAME]: template[constant.URL] for template in
                                     service_deploy_metadata.get(constant.TEMPLATE_CONFIGS)}
                 # 检查模版文件是否重复，重复则不再上传，直接使用原有Url
                 for template in service_config[constant.DEPLOY_METADATA][constant.TEMPLATE_CONFIGS]:
                     if template[constant.NAME] in name_url_mapping:
                         # 将相对路径替换成绝对路径
                         template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
@@ -245,15 +247,15 @@
                             template[constant.URL] = name_url_mapping.get(template[constant.NAME])
                         else:
                             template[constant.URL] = self._replace_file_path_with_url(template_path)
                     else:
                         if template.get(constant.URL):
                             template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
                             template[constant.URL] = self._replace_file_path_with_url(template_path)
-            else:
+            elif deploy_metadata_config.get(constant.TEMPLATE_CONFIGS):
                 for template in deploy_metadata_config.get(constant.TEMPLATE_CONFIGS):
                     # 将相对路径替换成绝对路径
                     if template.get(constant.URL):
                         template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
                         template[constant.URL] = self._replace_file_path_with_url(template_path)
 
             # 将SupplierDeployMetadata的路径做替换
```

### Comparing `computenest-cli-1.2.7/computenestcli/service/artifact.py` & `computenest-cli-1.2.8/computenestcli/service/artifact.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/service/base.py` & `computenest-cli-1.2.8/computenestcli/service/base.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/service/credentials.py` & `computenest-cli-1.2.8/computenestcli/service/credentials.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/service/file.py` & `computenest-cli-1.2.8/computenestcli/service/file.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/service/image.py` & `computenest-cli-1.2.8/computenestcli/service/image.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.2.7/computenestcli/service/supplier.py` & `computenest-cli-1.2.8/computenestcli/service/supplier.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,18 @@
         if operation_metadata is None:
             operation_metadata = '{}'
         else:
             operation_metadata = json.dumps(operation_metadata)
 
         version_name = Util.add_timestamp_to_version_name(service_data.get(constant.VERSION_NAME))
         deploy_metadata = service_data.get(constant.DEPLOY_METADATA)
-        for template in deploy_metadata.get(constant.TEMPLATE_CONFIGS):
-            template[constant.PREDEFINED_PARAMETERS] = template.get(constant.PREDEFINED_PARAMETERS) or []
-            template[constant.HIDDEN_PARAMETER_KEYS] = template.get(constant.HIDDEN_PARAMETER_KEYS) or []
+        if deploy_metadata and deploy_metadata.get(constant.TEMPLATE_CONFIGS):
+            for template in deploy_metadata.get(constant.TEMPLATE_CONFIGS):
+                template[constant.PREDEFINED_PARAMETERS] = template.get(constant.PREDEFINED_PARAMETERS) or []
+                template[constant.HIDDEN_PARAMETER_KEYS] = template.get(constant.HIDDEN_PARAMETER_KEYS) or []
         json_data = json.dumps(deploy_meta_data)
         service_info_init = compute_nest_supplier_20210521_models.UpdateServiceRequestServiceInfo(
             name=service_info.get(constant.NAME),
             image=service_info.get(constant.IMAGE),
             short_description=service_info.get(constant.SHORT_DESCRIPTION),
             locale=service_info.get(constant.LOCALE)
         )
```

### Comparing `computenest-cli-1.2.7/setup.py` & `computenest-cli-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
 
 setup(
     name='computenest-cli',
-    version='1.2.7',
+    version='1.2.8',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'computenest-cli = computenestcli.main:main'
         ]
     },
     install_requires=requirements,
```

