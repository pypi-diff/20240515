# Comparing `tmp/dask_databricks-0.3.0.tar.gz` & `tmp/dask_databricks-0.3.1.tar.gz`

## Comparing `dask_databricks-0.3.0.tar` & `dask_databricks-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/dask_databricks/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/dask_databricks/_version.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/dask_databricks/cli.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/dask_databricks/databrickscluster.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/dask_databricks/tests/test_databricks.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/.gitignore
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/LICENSE
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/README.md
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 dask_databricks-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/_version.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/cli.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/databrickscluster.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/dask_databricks/tests/test_databricks.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/README.md
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 dask_databricks-0.3.1/PKG-INFO
```

### Comparing `dask_databricks-0.3.0/.pre-commit-config.yaml` & `dask_databricks-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/.github/workflows/release.yaml` & `dask_databricks-0.3.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/.github/workflows/test.yaml` & `dask_databricks-0.3.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/dask_databricks/__init__.py` & `dask_databricks-0.3.1/dask_databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/dask_databricks/cli.py` & `dask_databricks-0.3.1/dask_databricks/cli.py`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/dask_databricks/databrickscluster.py` & `dask_databricks-0.3.1/dask_databricks/databrickscluster.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,13 +43,14 @@
         self.scheduler_comm = rpc(f"{self.spark_local_ip}:8786")
         await super()._start()
 
     @property
     def dashboard_link(self):
         cluster_id = spark.conf.get("spark.databricks.clusterUsageTags.clusterId")
         org_id = spark.conf.get("spark.databricks.clusterUsageTags.orgId")
-        return f"https://dbc-dp-{org_id}.cloud.databricks.com/driver-proxy/o/{org_id}/{cluster_id}/8087/status"
+        workspace_url = spark.conf.get("spark.databricks.workspaceUrl")
+        return f"https://{workspace_url}/driver-proxy/o/{org_id}/{cluster_id}/8087/status"
 
 
 def get_client():
     """Get a Dask client connected to a Databricks cluster."""
     return DatabricksCluster().get_client()
```

### Comparing `dask_databricks-0.3.0/dask_databricks/tests/test_databricks.py` & `dask_databricks-0.3.1/dask_databricks/tests/test_databricks.py`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/.gitignore` & `dask_databricks-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/LICENSE` & `dask_databricks-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/README.md` & `dask_databricks-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/pyproject.toml` & `dask_databricks-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_databricks-0.3.0/PKG-INFO` & `dask_databricks-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dask-databricks
-Version: 0.3.0
+Version: 0.3.1
 Project-URL: Documentation, https://github.com/dask-contrib/dask-databricks#readme
 Project-URL: Issues, https://github.com/dask-contrib/dask-databricks/issues
 Project-URL: Source, https://github.com/dask-contrib/dask-databricks
 Author-email: Jacob Tomlinson <jacob@tomlinson.email>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

