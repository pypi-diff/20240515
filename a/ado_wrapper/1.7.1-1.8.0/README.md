# Comparing `tmp/ado_wrapper-1.7.1.tar.gz` & `tmp/ado_wrapper-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.7.1.tar", max compression
+gzip compressed data, was "ado_wrapper-1.8.0.tar", max compression
```

## Comparing `ado_wrapper-1.7.1.tar` & `ado_wrapper-1.8.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.7.1/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.7.1/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.7.1/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.7.1/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.7.1/ado_wrapper/client.py
--rw-r--r--   0        0        0    21892 2024-05-07 18:26:17.266989 ado_wrapper-1.7.1/ado_wrapper/dumps.py
--rw-r--r--   0        0        0     3537 2024-05-06 10:01:09.344505 ado_wrapper-1.7.1/ado_wrapper/generate_docs.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.7.1/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.7.1/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.7.1/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.7.1/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3791 2024-05-06 09:59:23.335964 ado_wrapper-1.7.1/ado_wrapper/resources/agent_pools.py
--rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.7.1/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.7.1/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.7.1/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.7.1/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.7.1/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.7.1/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15678 2024-05-07 19:06:41.212391 ado_wrapper-1.7.1/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.7.1/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.7.1/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.7.1/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10768 2024-05-07 11:42:12.821826 ado_wrapper-1.7.1/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0    10723 2024-05-06 10:05:11.748381 ado_wrapper-1.7.1/ado_wrapper/resources/repo_user_permission.py
--rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.7.1/ado_wrapper/resources/searches.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.7.1/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.7.1/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.7.1/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.7.1/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.7.1/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.7.1/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.7.1/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-05-07 19:07:19.557317 ado_wrapper-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.8.0/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.8.0/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.8.0/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.8.0/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.8.0/ado_wrapper/client.py
+-rw-r--r--   0        0        0    21892 2024-05-07 18:26:17.266989 ado_wrapper-1.8.0/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3537 2024-05-06 10:01:09.344505 ado_wrapper-1.8.0/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.8.0/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.8.0/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.8.0/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.8.0/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.8.0/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.8.0/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.8.0/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3791 2024-05-06 09:59:23.335964 ado_wrapper-1.8.0/ado_wrapper/resources/agent_pools.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.8.0/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.8.0/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.8.0/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.8.0/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.8.0/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.8.0/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15678 2024-05-07 19:06:41.212391 ado_wrapper-1.8.0/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.8.0/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.8.0/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.8.0/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10768 2024-05-07 11:42:12.821826 ado_wrapper-1.8.0/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0    12422 2024-05-15 10:22:38.436043 ado_wrapper-1.8.0/ado_wrapper/resources/repo_user_permission.py
+-rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.8.0/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.8.0/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.8.0/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.8.0/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.8.0/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.8.0/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.8.0/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.8.0/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-05-15 10:21:32.826937 ado_wrapper-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.8.0/PKG-INFO
```

### Comparing `ado_wrapper-1.7.1/LICENSE` & `ado_wrapper-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/README.md` & `ado_wrapper-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/__main__.py` & `ado_wrapper-1.8.0/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/client.py` & `ado_wrapper-1.8.0/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/dumps.py` & `ado_wrapper-1.8.0/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/generate_docs.py` & `ado_wrapper-1.8.0/ado_wrapper/generate_docs.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.8.0/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.8.0/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.8.0/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/agent_pools.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/agent_pools.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/branches.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/builds.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/commits.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/environment.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/groups.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/merge_policies.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/projects.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/releases.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/repo.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/repo_user_permission.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/repo_user_permission.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,21 +86,44 @@
             json=PAYLOAD,
         ).json()["dataProviders"]["ms.vss-admin-web.security-view-permissions-data-provider"]
         if request is None:
             raise ResourceNotFound("Couldn't find perms for that repo, descriptor combo.")
         return [UserPermission.from_request_payload(x) for x in request["subjectPermissions"]]
 
     @classmethod
-    def set_by_subject_email(cls, ado_client: AdoClient, repo_id: str, subject_email: str, action: ActionType,
+    def set_by_group_descriptor(cls, ado_client: AdoClient, repo_id: str, group_descriptor: str, action: ActionType, permission: PermissionType) -> None:  # fmt: skip
+        requires_initialisation(ado_client)
+        IDENTITY_PAYLOAD = {"contributionIds": ["ms.vss-admin-web.security-view-permissions-data-provider"], "dataProviderContext": {"properties": {
+            "subjectDescriptor": group_descriptor, "permissionSetId": PERMISSION_SET_ID,
+            "permissionSetToken": f"repoV2/{ado_client.ado_project_id}/{repo_id}",
+        }}}
+        request = ado_client.session.post(
+            f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=7.0-preview.1",
+            json=IDENTITY_PAYLOAD,
+        ).json()
+        identity_descriptor = request["dataProviders"]["ms.vss-admin-web.security-view-permissions-data-provider"]["identityDescriptor"]
+        # ====
+        PAYLOAD = {"token": f"repoV2/{ado_client.ado_project_id}/{repo_id}", "merge": True, "accessControlEntries": [
+            {"descriptor": identity_descriptor,
+             "allow": flag_mapping[permission] if action == "Allow" else 0, "deny": flag_mapping[permission] if action == "Deny" else 0,
+        }]}  # fmt: skip
+        request = ado_client.session.post(
+            f"https://dev.azure.com/{ado_client.ado_org}/_apis/AccessControlEntries/{PERMISSION_SET_ID}",
+            json=PAYLOAD,
+        )
+        assert request.status_code == 200
+
+    @classmethod
+    def set_by_user_email(cls, ado_client: AdoClient, repo_id: str, email: str, action: ActionType,
                              permission: PermissionType, domain_container_id: str = "") -> None:  # fmt: skip
         requires_initialisation(ado_client)
         if not domain_container_id:
-            domain_container_id = AdoUser.get_by_email(ado_client, subject_email).domain_container_id
-        PAYLOAD = {"token": f"repoV2/{ado_client.ado_project_id}/{repo_id}", "merge": True, "accessControlEntries":[
-            {"descriptor": f"Microsoft.IdentityModel.Claims.ClaimsIdentity;{domain_container_id}\\{subject_email}",
+            domain_container_id = AdoUser.get_by_email(ado_client, email).domain_container_id
+        PAYLOAD = {"token": f"repoV2/{ado_client.ado_project_id}/{repo_id}", "merge": True, "accessControlEntries": [
+            {"descriptor": f"Microsoft.IdentityModel.Claims.ClaimsIdentity;{domain_container_id}\\{email}",
              "allow": flag_mapping[permission] if action == "Allow" else 0, "deny": flag_mapping[permission] if action == "Deny" else 0,
         }]}  # fmt: skip
         request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/AccessControlEntries/{PERMISSION_SET_ID}",
             json=PAYLOAD,
         )
         assert request.status_code == 200
@@ -158,38 +181,42 @@
         }
 
     @staticmethod
     def get_by_subject_descriptor(ado_client: AdoClient, repo_id: str, subject_descriptor: str) -> list[UserPermission]:
         return UserPermission.get_by_subject_descriptor(ado_client, subject_descriptor, repo_id)
 
     @classmethod
-    def get_by_subject_email(cls, ado_client: AdoClient, repo_id: str, subject_email: str) -> list[UserPermission]:
+    def get_by_user_email(cls, ado_client: AdoClient, repo_id: str, subject_email: str) -> list[UserPermission]:
         descriptor = AdoUser.get_by_email(ado_client, subject_email).descriptor_id
         return cls.get_by_subject_descriptor(ado_client, repo_id, descriptor)
 
     @staticmethod
-    def set_by_subject_email(ado_client: AdoClient, repo_id: str, subject_email: str, action: ActionType,
+    def set_by_group_descriptor(ado_client: AdoClient, repo_id: str, group_descriptor: str, action: ActionType, permission: PermissionType) -> None:  # fmt: skip
+        return UserPermission.set_by_group_descriptor(ado_client, repo_id, group_descriptor, action, permission)
+
+    @staticmethod
+    def set_by_user_email(ado_client: AdoClient, repo_id: str, email: str, action: ActionType,
                              permission: PermissionType, domain_container_id: str = "") -> None:  # fmt: skip
-        return UserPermission.set_by_subject_email(ado_client, repo_id, subject_email, action, permission, domain_container_id)
+        return UserPermission.set_by_user_email(ado_client, repo_id, email, action, permission, domain_container_id)
 
     @classmethod
-    def set_by_subject_email_batch(cls, ado_client: AdoClient, repo_id: str, subject_email: str,
+    def set_by_user_email_batch(cls, ado_client: AdoClient, repo_id: str, subject_email: str,
                                    mapping: dict[PermissionType, ActionType], domain_container_id: str = "") -> None:  # fmt: skip
-        """Does a batch job of updating permissions, updating all permissions for one subject (user or group)"""
+        """Does a batch job of updating permissions, updating all permissions for each user"""
         if not domain_container_id:
             domain_container_id = AdoUser.get_by_email(ado_client, subject_email).domain_container_id
         for permission, action in mapping.items():
-            cls.set_by_subject_email(ado_client, repo_id, subject_email, action, permission, domain_container_id)
+            cls.set_by_user_email(ado_client, repo_id, subject_email, action, permission, domain_container_id)
 
     @classmethod
     def set_all_permissions_for_repo(cls, ado_client: AdoClient, repo_id: str, mapping: dict[str, dict[PermissionType, ActionType]]) -> None:  # fmt: skip
         """Takes a mapping of <user_email>: {permission_name: Allow | Deny | Not set}}"""
         domain_container_id = AdoUser.get_by_email(ado_client, list(mapping.keys())[0]).domain_container_id
         for email, permission_pairs in mapping.items():
-            cls.set_by_subject_email_batch(ado_client, repo_id, email, permission_pairs, domain_container_id)
+            cls.set_by_user_email_batch(ado_client, repo_id, email, permission_pairs, domain_container_id)
 
     @classmethod
     def remove_perm(cls, ado_client: AdoClient, repo_id: str, subject_email: str, domain_container_id: str = "") -> None:
         return UserPermission.remove_perm(ado_client, repo_id, subject_email, domain_container_id)
 
     @staticmethod
     def display_output(permissions: list[UserPermission]) -> str:
```

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/searches.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/searches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/teams.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/users.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.8.0/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.8.0/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/state_manager.py` & `ado_wrapper-1.8.0/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/ado_wrapper/utils.py` & `ado_wrapper-1.8.0/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.7.1/pyproject.toml` & `ado_wrapper-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.7.1"
+version = "1.8.0"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.7.1/PKG-INFO` & `ado_wrapper-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.7.1
+Version: 1.8.0
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

