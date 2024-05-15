# Comparing `tmp/pulumi_eks-2.4.0a1715281916.tar.gz` & `tmp/pulumi_eks-2.4.0a1715729375.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_eks-2.4.0a1715281916.tar", last modified: Thu May  9 19:17:49 2024, max compression
+gzip compressed data, was "pulumi_eks-2.4.0a1715729375.tar", last modified: Tue May 14 23:34:03 2024, max compression
```

## Comparing `pulumi_eks-2.4.0a1715281916.tar` & `pulumi_eks-2.4.0a1715729375.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:17:49.295372 pulumi_eks-2.4.0a1715281916/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-09 19:17:49.295372 pulumi_eks-2.4.0a1715281916/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:17:49.291372 pulumi_eks-2.4.0a1715281916/pulumi_eks/
--rw-------   0 runner    (1001) docker     (127)     1150 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/__init__.py
--rw-------   0 runner    (1001) docker     (127)    88001 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9222 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/_utilities.py
--rw-------   0 runner    (1001) docker     (127)    95529 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/cluster.py
--rw-------   0 runner    (1001) docker     (127)     4860 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/cluster_creation_role_provider.py
--rw-------   0 runner    (1001) docker     (127)    30218 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/managed_node_group.py
--rw-------   0 runner    (1001) docker     (127)    46243 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/node_group.py
--rw-------   0 runner    (1001) docker     (127)     8405 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/node_group_security_group.py
--rw-------   0 runner    (1001) docker     (127)    49155 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/node_group_v2.py
--rw-------   0 runner    (1001) docker     (127)    40852 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2715 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/provider.py
--rw-------   0 runner    (1001) docker     (127)       40 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/py.typed
--rw-------   0 runner    (1001) docker     (127)    39043 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks/vpc_cni.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:17:49.295372 pulumi_eks-2.4.0a1715281916/pulumi_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-09 19:17:49.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-09 19:17:49.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 19:17:49.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-09 19:17:49.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 19:17:49.000000 pulumi_eks-2.4.0a1715281916/pulumi_eks.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      720 2024-05-09 19:17:39.000000 pulumi_eks-2.4.0a1715281916/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 19:17:49.295372 pulumi_eks-2.4.0a1715281916/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/pulumi_eks/
+-rw-------   0 runner    (1001) docker     (127)     1150 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    88001 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9222 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/_utilities.py
+-rw-------   0 runner    (1001) docker     (127)    95529 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/cluster.py
+-rw-------   0 runner    (1001) docker     (127)     4860 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/cluster_creation_role_provider.py
+-rw-------   0 runner    (1001) docker     (127)    30218 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/managed_node_group.py
+-rw-------   0 runner    (1001) docker     (127)    46243 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group.py
+-rw-------   0 runner    (1001) docker     (127)     8405 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group_security_group.py
+-rw-------   0 runner    (1001) docker     (127)    49155 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group_v2.py
+-rw-------   0 runner    (1001) docker     (127)    40852 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2715 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/provider.py
+-rw-------   0 runner    (1001) docker     (127)       40 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/py.typed
+-rw-------   0 runner    (1001) docker     (127)    39043 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks/vpc_cni.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 23:34:02.000000 pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      720 2024-05-14 23:33:53.000000 pulumi_eks-2.4.0a1715729375/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:34:02.997788 pulumi_eks-2.4.0a1715729375/setup.cfg
```

### Comparing `pulumi_eks-2.4.0a1715281916/PKG-INFO` & `pulumi_eks-2.4.0a1715729375/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 2.4.0a1715281916
+Version: 2.4.0a1715729375
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Keywords: pulumi,aws,eks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715281916 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715729375 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. License: Apache-2.0 Project-
 URL: Homepage, https://pulumi.com Project-URL: Repository, https://github.com/
 pulumi/pulumi-eks Keywords: pulumi,aws,eks Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Requires-Dist: parver>=0.2.1 Requires-Dist:
 pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0 Requires-Dist:
 pulumi-kubernetes<5.0.0,>=4.0.0 Requires-Dist: semver>=2.8.1 [![Build Status]
 (https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)]
```

### Comparing `pulumi_eks-2.4.0a1715281916/README.md` & `pulumi_eks-2.4.0a1715729375/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/__init__.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/_inputs.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/_utilities.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/cluster.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/cluster_creation_role_provider.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/cluster_creation_role_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/managed_node_group.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/managed_node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/node_group.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/node_group_security_group.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/node_group_v2.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/node_group_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/outputs.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/provider.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks/vpc_cni.py` & `pulumi_eks-2.4.0a1715729375/pulumi_eks/vpc_cni.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks.egg-info/PKG-INFO` & `pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 2.4.0a1715281916
+Version: 2.4.0a1715729375
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Keywords: pulumi,aws,eks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715281916 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715729375 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. License: Apache-2.0 Project-
 URL: Homepage, https://pulumi.com Project-URL: Repository, https://github.com/
 pulumi/pulumi-eks Keywords: pulumi,aws,eks Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Requires-Dist: parver>=0.2.1 Requires-Dist:
 pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0 Requires-Dist:
 pulumi-kubernetes<5.0.0,>=4.0.0 Requires-Dist: semver>=2.8.1 [![Build Status]
 (https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)]
```

### Comparing `pulumi_eks-2.4.0a1715281916/pulumi_eks.egg-info/SOURCES.txt` & `pulumi_eks-2.4.0a1715729375/pulumi_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715281916/pyproject.toml` & `pulumi_eks-2.4.0a1715729375/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_eks"
   description = "Pulumi Amazon Web Services (AWS) EKS Components."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-aws>=6.0.0,<7.0.0", "pulumi-kubernetes>=4.0.0,<5.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aws", "eks"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1715281916"
+  version = "2.4.0a1715729375"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-eks"
 
 [build-system]
```

