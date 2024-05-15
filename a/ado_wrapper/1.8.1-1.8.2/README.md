# Comparing `tmp/ado_wrapper-1.8.1.tar.gz` & `tmp/ado_wrapper-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.8.1.tar", max compression
+gzip compressed data, was "ado_wrapper-1.8.2.tar", max compression
```

## Comparing `ado_wrapper-1.8.1.tar` & `ado_wrapper-1.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.8.1/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.8.1/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.8.1/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.8.1/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.8.1/ado_wrapper/client.py
--rw-r--r--   0        0        0    21892 2024-05-07 18:26:17.266989 ado_wrapper-1.8.1/ado_wrapper/dumps.py
--rw-r--r--   0        0        0     3537 2024-05-06 10:01:09.344505 ado_wrapper-1.8.1/ado_wrapper/generate_docs.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.8.1/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.8.1/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.8.1/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.8.1/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.8.1/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.8.1/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.8.1/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3791 2024-05-06 09:59:23.335964 ado_wrapper-1.8.1/ado_wrapper/resources/agent_pools.py
--rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.8.1/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.8.1/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.8.1/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.8.1/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.8.1/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.8.1/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15678 2024-05-07 19:06:41.212391 ado_wrapper-1.8.1/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.8.1/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.8.1/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.8.1/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10768 2024-05-07 11:42:12.821826 ado_wrapper-1.8.1/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0    12706 2024-05-15 10:28:55.220198 ado_wrapper-1.8.1/ado_wrapper/resources/repo_user_permission.py
--rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.8.1/ado_wrapper/resources/searches.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.8.1/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.8.1/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.8.1/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.8.1/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.8.1/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.8.1/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.8.1/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-05-15 10:29:05.012537 ado_wrapper-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.8.2/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.8.2/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.8.2/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.8.2/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.8.2/ado_wrapper/client.py
+-rw-r--r--   0        0        0    21892 2024-05-07 18:26:17.266989 ado_wrapper-1.8.2/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3537 2024-05-06 10:01:09.344505 ado_wrapper-1.8.2/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.8.2/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.8.2/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.8.2/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.8.2/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.8.2/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.8.2/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.8.2/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3791 2024-05-06 09:59:23.335964 ado_wrapper-1.8.2/ado_wrapper/resources/agent_pools.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.8.2/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3520 2024-05-15 12:17:11.865100 ado_wrapper-1.8.2/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.8.2/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.8.2/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.8.2/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.8.2/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15678 2024-05-07 19:06:41.212391 ado_wrapper-1.8.2/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.8.2/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.8.2/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.8.2/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10768 2024-05-07 11:42:12.821826 ado_wrapper-1.8.2/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0    12706 2024-05-15 10:28:55.220198 ado_wrapper-1.8.2/ado_wrapper/resources/repo_user_permission.py
+-rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.8.2/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.8.2/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.8.2/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.8.2/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.8.2/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.8.2/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.8.2/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.8.2/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-05-15 12:18:39.170587 ado_wrapper-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.8.2/PKG-INFO
```

### Comparing `ado_wrapper-1.8.1/LICENSE` & `ado_wrapper-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/README.md` & `ado_wrapper-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/__main__.py` & `ado_wrapper-1.8.2/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/client.py` & `ado_wrapper-1.8.2/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/dumps.py` & `ado_wrapper-1.8.2/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/generate_docs.py` & `ado_wrapper-1.8.2/ado_wrapper/generate_docs.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.8.2/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.8.2/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.8.2/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/agent_pools.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/agent_pools.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/branches.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/branches.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Literal
 
 from ado_wrapper.state_managed_abc import StateManagedResource
+from ado_wrapper.resources.users import Member 
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 BranchEditableAttribute = Literal["name"]
 
 
@@ -15,23 +16,25 @@
 class Branch(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/refs?view=azure-devops-rest-7.1
     This isn't entirely what I wanted, you can't branch without a commit, so I need to add a commit method to this class
     And overall, just use commits if you can.
     """
 
     branch_id: str = field(metadata={"is_id_field": True})
-    name: str = field(metadata={"editable": True})  # Maybe more?
+    name: str = field(metadata={"editable": True})
     repo_id: str = field(repr=False)
+    creator: Member = field(repr=False)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, str | dict[str, str]]) -> Branch:
         return cls(
-            data["objectId"],  # type: ignore[arg-type]
+            data["objectId"],
             data["name"].removeprefix("refs/heads/"),  # type: ignore[union-attr]
             data["url"].split("/")[-2],  # type: ignore[union-attr]
+            Member.from_request_payload(data["creator"]),  # type: ignore[union-attr]
         )
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, repo_id: str, branch_id: str) -> Branch:  # type: ignore[override]
         for branch in cls.get_all_by_repo(ado_client, repo_id):
             if branch.branch_id == branch_id:
                 return branch
```

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/builds.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/commits.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/environment.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/groups.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/merge_policies.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/projects.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/releases.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/repo.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/repo_user_permission.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/repo_user_permission.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/searches.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/searches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/teams.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/users.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.8.2/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.8.2/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/state_manager.py` & `ado_wrapper-1.8.2/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/ado_wrapper/utils.py` & `ado_wrapper-1.8.2/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.1/pyproject.toml` & `ado_wrapper-1.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.8.1"
+version = "1.8.2"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.8.1/PKG-INFO` & `ado_wrapper-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.8.1
+Version: 1.8.2
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

