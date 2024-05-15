# Comparing `tmp/lupin-grognard-2.0.0.tar.gz` & `tmp/lupin_grognard-2.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-grognard-2.0.0.tar", last modified: Fri Mar 22 08:47:41 2024, max compression
+gzip compressed data, was "lupin_grognard-2.1.0.dev0.tar", last modified: Wed May 15 08:09:05 2024, max compression
```

## Comparing `lupin-grognard-2.0.0.tar` & `lupin_grognard-2.1.0.dev0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.269213 lupin-grognard-2.0.0/
--rw-rw-rw-   0        0        0     1091 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/LICENCE
--rw-rw-rw-   0        0        0       36 2023-06-22 08:55:16.000000 lupin-grognard-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      797 2024-03-22 08:47:41.269213 lupin-grognard-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-06-22 08:55:16.000000 lupin-grognard-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.224306 lupin-grognard-2.0.0/lupin_grognard/
--rw-rw-rw-   0        0        0       23 2024-03-22 08:47:41.000000 lupin-grognard-2.0.0/lupin_grognard/__init__.py
--rw-rw-rw-   0        0        0       77 2023-06-23 08:25:25.000000 lupin-grognard-2.0.0/lupin_grognard/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.246835 lupin-grognard-2.0.0/lupin_grognard/core/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/__init__.py
--rw-rw-rw-   0        0        0     3346 2023-11-21 08:43:53.000000 lupin-grognard-2.0.0/lupin_grognard/core/check.py
--rw-rw-rw-   0        0        0      912 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/cmd.py
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.251834 lupin-grognard-2.0.0/lupin_grognard/core/commit/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/commit/__init__.py
--rw-rw-rw-   0        0        0    12803 2024-02-11 17:59:08.000000 lupin-grognard-2.0.0/lupin_grognard/core/commit/commit.py
--rw-rw-rw-   0        0        0     2573 2023-09-27 14:18:43.000000 lupin-grognard-2.0.0/lupin_grognard/core/commit/commit_error.py
--rw-rw-rw-   0        0        0     5247 2023-11-02 11:42:50.000000 lupin-grognard-2.0.0/lupin_grognard/core/commit/commit_reporter.py
--rw-rw-rw-   0        0        0    12639 2024-03-22 08:46:06.000000 lupin-grognard-2.0.0/lupin_grognard/core/commit/commit_validator.py
--rw-rw-rw-   0        0        0     1546 2024-02-02 13:10:44.000000 lupin-grognard-2.0.0/lupin_grognard/core/config.py
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.255870 lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/__init__.py
--rw-rw-rw-   0        0        0    11902 2024-02-11 17:59:08.000000 lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/changelog.py
--rw-rw-rw-   0        0        0     2209 2024-02-11 17:34:35.000000 lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/jinja_generator.py
--rw-rw-rw-   0        0        0     5474 2024-03-22 08:46:06.000000 lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/reviewlog.py
--rw-rw-rw-   0        0        0     1540 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/ros2_docs.py
--rw-rw-rw-   0        0        0     4663 2024-02-06 11:27:05.000000 lupin-grognard-2.0.0/lupin_grognard/core/git.py
--rw-rw-rw-   0        0        0      205 2024-02-06 11:27:05.000000 lupin-grognard-2.0.0/lupin_grognard/core/gitlab.py
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.257871 lupin-grognard-2.0.0/lupin_grognard/core/tools/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/tools/__init__.py
--rw-rw-rw-   0        0        0      216 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/tools/log_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.259870 lupin-grognard-2.0.0/lupin_grognard/core/tools/ros2/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/tools/ros2/__init__.py
--rw-rw-rw-   0        0        0     2654 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/tools/ros2/interfaces.py
--rw-rw-rw-   0        0        0     2644 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/tools/ros2/package.py
--rw-rw-rw-   0        0        0    35591 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/core/tools/ros2/parser.py
--rw-rw-rw-   0        0        0     5290 2024-02-06 14:49:34.000000 lupin-grognard-2.0.0/lupin_grognard/core/tools/utils.py
--rw-rw-rw-   0        0        0     7929 2024-02-06 14:49:34.000000 lupin-grognard-2.0.0/lupin_grognard/run.py
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.267216 lupin-grognard-2.0.0/lupin_grognard/templates/
--rw-rw-rw-   0        0        0     2690 2024-02-05 10:11:09.000000 lupin-grognard-2.0.0/lupin_grognard/templates/changelog.j2
--rw-rw-rw-   0        0        0     5865 2024-02-12 14:19:43.000000 lupin-grognard-2.0.0/lupin_grognard/templates/reviewlog.j2
--rw-rw-rw-   0        0        0      454 2023-06-22 08:55:15.000000 lupin-grognard-2.0.0/lupin_grognard/templates/rosapi.j2
-drwxrwxrwx   0        0        0        0 2024-03-22 08:47:41.268215 lupin-grognard-2.0.0/lupin_grognard.egg-info/
--rw-rw-rw-   0        0        0      797 2024-03-22 08:47:41.000000 lupin-grognard-2.0.0/lupin_grognard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2024-03-22 08:47:41.000000 lupin-grognard-2.0.0/lupin_grognard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 08:47:41.000000 lupin-grognard-2.0.0/lupin_grognard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-22 08:47:41.000000 lupin-grognard-2.0.0/lupin_grognard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 13:19:47.000000 lupin-grognard-2.0.0/lupin_grognard.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      135 2024-03-22 08:47:41.000000 lupin-grognard-2.0.0/lupin_grognard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-22 08:47:41.000000 lupin-grognard-2.0.0/lupin_grognard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      935 2024-03-22 08:47:41.271213 lupin-grognard-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      171 2023-06-23 08:22:50.000000 lupin-grognard-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.895522 lupin_grognard-2.1.0.dev0/
+-rw-rw-rw-   0        0        0     1091 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/LICENCE
+-rw-rw-rw-   0        0        0       36 2023-06-22 08:55:16.000000 lupin_grognard-2.1.0.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0      802 2024-05-15 08:09:05.895522 lupin_grognard-2.1.0.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-06-22 08:55:16.000000 lupin_grognard-2.1.0.dev0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.775738 lupin_grognard-2.1.0.dev0/lupin_grognard/
+-rw-rw-rw-   0        0        0       28 2024-05-15 08:09:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/__init__.py
+-rw-rw-rw-   0        0        0       77 2023-06-23 08:25:25.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.800536 lupin_grognard-2.1.0.dev0/lupin_grognard/core/
+-rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/__init__.py
+-rw-rw-rw-   0        0        0     3346 2023-11-21 08:43:53.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/check.py
+-rw-rw-rw-   0        0        0      912 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.806057 lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/
+-rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/__init__.py
+-rw-rw-rw-   0        0        0    12886 2024-05-15 07:50:28.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/commit.py
+-rw-rw-rw-   0        0        0     2573 2023-09-27 14:18:43.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/commit_error.py
+-rw-rw-rw-   0        0        0     5247 2023-11-02 11:42:50.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/commit_reporter.py
+-rw-rw-rw-   0        0        0    13235 2024-05-14 09:28:14.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/commit_validator.py
+-rw-rw-rw-   0        0        0     1865 2024-05-14 09:28:14.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/config.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.863320 lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/__init__.py
+-rw-rw-rw-   0        0        0    13139 2024-05-14 09:28:14.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/changelog.py
+-rw-rw-rw-   0        0        0     2209 2024-02-11 17:34:35.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/jinja_generator.py
+-rw-rw-rw-   0        0        0     5474 2024-05-14 21:38:52.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/reviewlog.py
+-rw-rw-rw-   0        0        0     1540 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/ros2_docs.py
+-rw-rw-rw-   0        0        0     4663 2024-02-06 11:27:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/git.py
+-rw-rw-rw-   0        0        0      205 2024-02-06 11:27:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/gitlab.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.866830 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/__init__.py
+-rw-rw-rw-   0        0        0      216 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/log_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.869831 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/ros2/
+-rw-rw-rw-   0        0        0        0 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/ros2/__init__.py
+-rw-rw-rw-   0        0        0     2654 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/ros2/interfaces.py
+-rw-rw-rw-   0        0        0     2644 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/ros2/package.py
+-rw-rw-rw-   0        0        0    35591 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/ros2/parser.py
+-rw-rw-rw-   0        0        0     5322 2024-05-14 20:32:17.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/utils.py
+-rw-rw-rw-   0        0        0     7961 2024-05-14 09:28:14.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/run.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.893515 lupin_grognard-2.1.0.dev0/lupin_grognard/templates/
+-rw-rw-rw-   0        0        0     3200 2024-05-14 09:28:14.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/templates/changelog.j2
+-rw-rw-rw-   0        0        0     5947 2024-05-15 07:50:28.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/templates/reviewlog.j2
+-rw-rw-rw-   0        0        0      454 2023-06-22 08:55:15.000000 lupin_grognard-2.1.0.dev0/lupin_grognard/templates/rosapi.j2
+drwxrwxrwx   0        0        0        0 2024-05-15 08:09:05.895522 lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/
+-rw-rw-rw-   0        0        0      802 2024-05-15 08:09:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1412 2024-05-15 08:09:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 08:09:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-15 08:09:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 13:19:47.000000 lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      135 2024-05-15 08:09:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 08:09:05.000000 lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      940 2024-05-15 08:09:05.898045 lupin_grognard-2.1.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      171 2023-06-23 08:22:50.000000 lupin_grognard-2.1.0.dev0/setup.py
```

### Comparing `lupin-grognard-2.0.0/LICENCE` & `lupin_grognard-2.1.0.dev0/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/PKG-INFO` & `lupin_grognard-2.1.0.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-grognard
-Version: 2.0.0
+Version: 2.1.0.dev0
 Summary: Lupin linter tool
 License: MIT License
 Keywords: cli,linter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/check.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/check.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/cmd.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/cmd.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/commit/commit.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from lupin_grognard.core.config import (
     INITIAL_COMMIT,
     MAJOR_COMMIT_TYPES,
     PATTERN,
 )
 from lupin_grognard.core.git import Git
-from lupin_grognard.core.tools.log_utils import info
+from lupin_grognard.core.tools.log_utils import info, warn
 
 
 class GitLabMergeRequestDetails:
     def __init__(self):
         self.associated_closed_issue: Optional[str] = None
         self.associated_approvers: Optional[str] = None
         self.associated_approvers_date: Optional[str] = None
@@ -82,21 +82,22 @@
         body = body.rstrip("\n")
 
         return [
             self._remove_markdown_list_markers(message) for message in body.split("\n")
         ]
 
     @property
-    def closes_issues(self) -> List | None:
+    def closes_issues(self) -> List | str:
         """Returns the list of issues closed by the commit"""
         if self.body:
             for line in self.body:
                 if line.startswith("Closes #"):  # Closes #465, #190 and #400
                     return re.findall(r"#(\d+)", line)  # ['465', '190', '400']
-        return None
+        warn(f"Could not find the issue closed by the commit '{self.title}'")
+        return "0"
 
     @property
     def approvers(self) -> List[str]:
         approvers = []
         if self.body:
             for line in self.body:
                 if line.startswith("Approved-by: "):
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/commit/commit_error.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/commit_error.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/commit/commit_reporter.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/commit_reporter.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/commit/commit_validator.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/commit/commit_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from lupin_grognard.core.commit.commit_reporter import CommitReporter
 from lupin_grognard.core.config import (
     COMMIT_TYPE_MUST_HAVE_SCOPE,
     COMMIT_TYPE_MUST_NOT_HAVE_SCOPE,
     COMMIT_WITH_SCOPE,
     INITIAL_COMMIT,
     IMPACT_TAG,
+    JAMA_FIXDEFECT_REGEX,
     JAMA_REGEX,
     JAMA_TAG,
     MAIN_BRANCHES_LIST,
     MAX_COMMIT_DESCR_LINES,
     MIN_COMMIT_DESCR_LENTH,
     PATTERN,
     TITLE_FAILED,
@@ -230,29 +231,31 @@
                 invalid_jama_refs.append(jama_ref)
             elif jama_ref in unique_jama_refs and jama_ref not in duplicate_jama_refs:
                 duplicate_jama_refs.append(jama_ref)
             else:
                 unique_jama_refs.add(jama_ref)
         return duplicate_jama_refs, invalid_jama_refs
 
-    def _validate_commit_message(self, commit_msg: str, type: str, scope: str) -> bool:
+    def _validate_commit_message(
+        self, commit_msg: str, c_type: str, scope: str
+    ) -> bool:
         if self._is_special_commit(commit_msg=commit_msg):
             return True
 
-        match type:
+        match c_type:
             case None:
                 self.reporter.display_invalid_title_report(error_message=TITLE_FAILED)
                 return False
-            case match_type if (match_type := type) in COMMIT_WITH_SCOPE:
+            case match_type if (match_type := c_type) in COMMIT_WITH_SCOPE:
                 return self._validate_commit_message_for_specific_type(
-                    scope=scope, type=match_type
+                    scope=scope, c_type=match_type
                 )
             case _:
                 return self._validate_commit_message_for_generic_type(
-                    type=type, scope=scope
+                    c_type=c_type, scope=scope
                 )
 
     def _is_conventional_commit_body_valid(self, message: str) -> bool:
         """Checks if the line in the body of a commit message starts with a conventional commit"""
         return bool(re.match(PATTERN, message))
 
     def _is_commit_body_line_length_valid(self, message: str) -> bool:
@@ -294,30 +297,45 @@
         """Find MR approvers that are also authors of the commit(s) associated with the MR."""
         rejected_user_emails = []
         for author in self.mr_details.associated_commits_authors:
             if author in self.approvers_mail:
                 rejected_user_emails.append(author)
         return rejected_user_emails
 
-    def _validate_commit_message_for_specific_type(self, scope: str, type: str) -> bool:
+    def _validate_commit_message_for_specific_type(
+        self, scope: str, c_type: str
+    ) -> bool:
         """
         Validates the scope for a COMMIT_WITH_SCOPE list.
+
+        Args:
+            scope (str): The scope of the commit message
+            c_type (str): The commit type
+
+        Returns:
+            bool: True if the commit message is valid, False otherwise
         """
-        if scope is None or scope not in ["(add)", "(change)", "(remove)"]:
+        if c_type == "fixdefect":
+            if scope is None or not re.match(JAMA_FIXDEFECT_REGEX, scope):
+                self.reporter.display_invalid_title_report(
+                    error_message=COMMIT_TYPE_MUST_HAVE_SCOPE[c_type]
+                )
+                return False
+        elif scope is None or scope not in ["(add)", "(change)", "(remove)"]:
             self.reporter.display_invalid_title_report(
-                error_message=COMMIT_TYPE_MUST_HAVE_SCOPE.format(type=type)
+                error_message=COMMIT_TYPE_MUST_HAVE_SCOPE["other"].format(c_type=c_type)
             )
             return False
         return True
 
     def _remove_punctuation_around_words(self, words: List[str]) -> List[str]:
         """Removes punctuation around words"""
         return [word.strip(string.punctuation) for word in words if word != ""]
 
-    def _validate_commit_message_for_generic_type(self, type, scope: str) -> bool:
+    def _validate_commit_message_for_generic_type(self, c_type, scope: str) -> bool:
         """Validates other commit types do not contain a scope"""
         if scope is None:
             return True
         else:
-            error_message = COMMIT_TYPE_MUST_NOT_HAVE_SCOPE.format(type, type)
+            error_message = COMMIT_TYPE_MUST_NOT_HAVE_SCOPE.format(c_type, c_type)
             self.reporter.display_invalid_title_report(error_message=error_message)
             return False
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/config.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,33 +24,41 @@
 )
 
 MERGE_FAILED = "Commit merges should have at least one approver."
 
 EMOJI_CHECK = ":check_mark_button:"
 EMOJI_CROSS = ":cross_mark:"
 
-COMMIT_TYPE_MUST_HAVE_SCOPE = (
-    "Commits of type '{type}' must be of the form '{type}(add)', "
-    "'{type}(change)' or '{type}(remove)'"
-)
+COMMIT_TYPE_MUST_HAVE_SCOPE = {
+    "fixdefect": (
+        "The defect being fixed must be given in argument with the syntax 'fixdefect(JAMA-xxx)' "
+        "where 'xxx' is the ID of the associated item in JAMA"
+    ),
+    "other": (
+        "Commits of type '{c_type}' must be of the form '{c_type}(add)', "
+        "'{c_type}(change)' or '{c_type}(remove)'"
+    ),
+}
 
 COMMIT_TYPE_MUST_NOT_HAVE_SCOPE = (
     "Commits of type '{}' must not specify a scope but simply use the form '{}'"
 )
 
 PATTERN = (
     r"(?s)"  # To explictly make . match new line
-    r"(build|bump|ci|deps|docs|enabler|feat|fixbug|refactor|test)"  # type
+    r"(build|bump|ci|deps|docs|enabler|feat|fixbug|fixdefect|refactor|test)"  # type
     r"(\(\S+\))?!?:"  # scope
     r"( [^\n\r]+)"  # subject
     r"((\n\n.*)|(\s*))?$"
 )
 
-MAJOR_COMMIT_TYPES = ["enabler", "feat", "fixbug", "refactor"]
+MAJOR_COMMIT_TYPES = ["enabler", "feat", "fixbug", "fixdefect", "refactor"]
 
-COMMIT_WITH_SCOPE = ["deps", "feat"]
+COMMIT_WITH_SCOPE = ["deps", "feat", "fixdefect"]
 
 JAMA_REGEX = r"SmlPrep-SUBSR-\d+"
 
+JAMA_FIXDEFECT_REGEX = r"\(JAMA-[a-zA-Z0-9-]+\)"
+
 JAMA_TAG = "JAMA:"
 
 IMPACT_TAG = "IMPACT:"
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/changelog.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/changelog.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,14 +150,16 @@
         self, commits: List[str], commit: Commit, issue_number: str
     ) -> None:
         """Append title without type and scope for feat and fixbug commit type,
         append title for other commit type. Append description if any
         and append issue number and url if issue number is found"""
         if commit.type == "feat" or commit.type == "fixbug":
             commit_title = commit.title_without_type_scope
+        elif commit.type == "fixdefect":
+            commit_title = self._format_fixdefect_title(commit=commit)
         else:
             commit_title = commit.title
 
         description, jama_ref = self._separate_jama_ref(commit=commit)
 
         if not issue_number:
             commits.append(
@@ -175,22 +177,53 @@
                     "description": description,
                     **({"jama_ref": jama_ref} if jama_ref else {}),
                     "gitlab_issue_id": issue_number,
                     "gitlab_issue_url": url,
                 }
             )
 
+    def _format_fixdefect_title(self, commit: Commit) -> str:
+        """Format fixdefect title with the associated jama reference"""
+        return (
+            "**"
+            + commit.scope.replace("(", "").replace(")", "")
+            + "**"
+            + ": "
+            + commit.title_without_type_scope
+        )
+
     def _classify_commits_by_type_and_scope(
         self, commits: List[Commit]
     ) -> Dict[str, Union[Dict[str, List[str]], List[str]]]:
         """Classify commits by type and scope and exclude merge commits"""
-        commits_feat_add, commits_feat_change, commits_feat_remove = [], [], []
-        commits_fixbug, commits_other, commits_unspecified = [], [], []
+        (
+            commits_fixdefect,
+            commits_feat_add,
+            commits_feat_change,
+            commits_feat_remove,
+            commits_fixbug,
+            commits_other,
+            commits_unspecified,
+        ) = (
+            [],
+            [],
+            [],
+            [],
+            [],
+            [],
+            [],
+        )
         for commit in commits:
             match (commit.type, commit.scope):
+                case ("fixdefect", commit.scope):
+                    self._append_title_and_description_with_matched_issue(
+                        commits=commits_fixdefect,
+                        commit=commit,
+                        issue_number=commit.mr_details.associated_closed_issue,
+                    )
                 case ("feat", "(add)"):
                     self._append_title_and_description_with_matched_issue(
                         commits=commits_feat_add,
                         commit=commit,
                         issue_number=commit.mr_details.associated_closed_issue,
                     )
                 case ("feat", "(change)"):
@@ -221,32 +254,36 @@
                     if not commit.is_gitlab_merge_commit():
                         self._append_title_and_description_with_matched_issue(
                             commits=commits_unspecified,
                             commit=commit,
                             issue_number=commit.mr_details.associated_closed_issue,
                         )
         return self._create_commit_dict(
+            commits_fixdefect=commits_fixdefect,
             commits_feat_add=commits_feat_add,
             commits_feat_change=commits_feat_change,
             commits_feat_remove=commits_feat_remove,
             commits_fixbug=commits_fixbug,
             commits_other=commits_other,
             commits_unspecified=commits_unspecified,
         )
 
     def _create_commit_dict(
         self,
+        commits_fixdefect: List[str],
         commits_feat_add: List[str],
         commits_feat_change: List[str],
         commits_feat_remove: List[str],
         commits_fixbug: List[str],
         commits_other: List[str],
         commits_unspecified: List[str],
     ) -> Dict[str, Union[Dict[str, List[str]], List[str]]]:
         result = {}
+        if commits_fixdefect:
+            result["fixdefect"] = commits_fixdefect
         if commits_feat_add or commits_feat_change or commits_feat_remove:
             result["feature"] = {}
             if commits_feat_add:
                 result["feature"]["added"] = commits_feat_add
             if commits_feat_change:
                 result["feature"]["changed"] = commits_feat_change
             if commits_feat_remove:
@@ -260,14 +297,15 @@
         return result
 
     def _display_number_of_commits_found_for_changelog(
         self, versioned_commits: List[Dict[str, List[str]]]
     ) -> None:
         total = 0
         for v in versioned_commits:
+            total += len(v.get("commits", {}).get("fixdefect", []))
             total += len(v.get("commits", {}).get("feature", {}).get("added", []))
             total += len(v.get("commits", {}).get("feature", {}).get("changed", []))
             total += len(v.get("commits", {}).get("feature", {}).get("removed", []))
             total += len(v.get("commits", {}).get("fixbug", []))
             total += len(v.get("commits", {}).get("other", []))
             total += len(v.get("commits", {}).get("unspecified", []))
         info(msg=f"Found {total} commits")
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/jinja_generator.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/jinja_generator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/reviewlog.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/reviewlog.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/doc_generator/ros2_docs.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/doc_generator/ros2_docs.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/git.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/git.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/tools/ros2/interfaces.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/ros2/interfaces.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/tools/ros2/package.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/ros2/package.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/tools/ros2/parser.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/ros2/parser.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/lupin_grognard/core/tools/utils.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/core/tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         "bump",
         "ci",
         "deps(add|change|remove)",
         "docs",
         "enabler",
         "feat(add|change|remove)",
         "fixbug",
+        "fixdefect(JAMA-xxx)",
         "refactor",
         "test",
     ]
     print("Supported commit types: " + ", ".join(commit_type))
     print(
         "Only one commit of a major type is allowed per merge branch: "
         f'{", ".join(MAJOR_COMMIT_TYPES[:-1])}, or {MAJOR_COMMIT_TYPES[-1]}.'
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard/run.py` & `lupin_grognard-2.1.0.dev0/lupin_grognard/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,16 @@
     ),
     no_approvers: bool = typer.Option(
         False, "--no-approvers", "-na", help="ignore approver check"
     ),
 ):
     """
     Supported commit types: build, bump, ci, deps(add|change|remove), docs, enabler,
-    feat(add|change|remove), fixbug, refactor, test.
-    Only one major commit types allowed per branch: "enabler", "feat", "fixbug" or "refactor".
+    feat(add|change|remove), fixbug, fixdefect(JAMA-xxx), refactor, test.
+    Only one major commit types allowed per branch: "enabler", "feat", "fixbug", fixdefect or "refactor".
 
     Check every commit message since the last "merge request" in any of the branches in the
     main_branches_list : "main", "master", "dev", "develop", "development"
 
     - With --all option :
     grog check-commits [--all or -a] to check all commits from initial commit.
     This option is automatically set if current branch is a main one.
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard/templates/changelog.j2` & `lupin_grognard-2.1.0.dev0/lupin_grognard/templates/changelog.j2`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,32 @@
 
 {% for item in version_details %}
 ---
 ## [{{ item.version }}]{% if item.date %} ({{ item.date }}){% endif %}
 
 {% for type in item.commits %}
 
+{% if type == 'fixdefect' %}
+### Defects
+
+{% for commit in item.commits.fixdefect %}
+{%- if commit.gitlab_issue_id %}
+- {{ commit.title }} [#{{ commit.gitlab_issue_id }}]({{ commit.gitlab_issue_url }}){% if commit.jama_ref %}`{{ commit.jama_ref }}`{% endif %}
+
+{% else %}
+- {{ commit.title }}{% if commit.jama_ref %}`{{ commit.jama_ref }}`{% endif %}
+
+{% endif %}
+{% if commit.description %}
+{% for line in commit.description %}
+  - {{ line }}
+{% endfor %}
+{% endif %}
+{% endfor %}
+{% endif %}
 {% if type == 'feature' %}
 ### Features
 
 {% for scope in item.commits.feature %}
 #### {{ scope|capitalize }}
 
 {% for commit in item.commits.feature[scope] -%}
@@ -67,15 +85,14 @@
 {% if commit.description %}
 {% for line in commit.description %}
   - {{ line }}
 {% endfor %}
 {% endif %}
 {% endfor %}
 {% endif %}
-
 {% if type == 'unspecified' %}
 ### Unspecified
 
 {% for commit in item.commits.unspecified %}
 {%- if commit.gitlab_issue_id %}
 - {{ commit.title }} [#{{ commit.gitlab_issue_id }}]({{ commit.gitlab_issue_url }}){% if commit.jama_ref %}`{{ commit.jama_ref }}`{% endif %}
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard/templates/reviewlog.j2` & `lupin_grognard-2.1.0.dev0/lupin_grognard/templates/reviewlog.j2`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,17 @@
             </tr>
           </thead>
           <tbody>
             {% for commit in item.commits %}
             <tr>
               <td>
                 {{ commit.commit_hash }}<br>
+                {% if commit.gitlab_issue_id != "0" %}
                 Issue <a href="{{ project_url }}/-/issues/{{ commit.gitlab_issue_id }}">#{{ commit.gitlab_issue_id }}</a>
+                {% endif %}
               </td>
               <td>
                 {% if "`" in commit.title %}
                   {% set title_words = commit.title.split() %}
                   {% for word in title_words %}
                       {% if '`' in word %}
                           <samp>{{ word.replace('`', '')|e }}</samp>
@@ -150,15 +152,15 @@
             </tr>
             {% endfor %}
           </tbody>
         </table>
         {% endfor %}
       </div>
       <div>
-        <h2>List of participants</h2>
+        <h2>List of reviewers</h2>
         <table class="second-table">
           <thead>
             <tr>
               <th scope="col">Name</th>
               <th scope="col">Role</th>
               <th scope="col">Signature</th>
               <th scope="col">Date</th>
```

#### html2text {}

```diff
@@ -13,22 +13,22 @@
                        { word.replace('`',
                        '')|e }} {% else %} {
                        { word|e }} {% endif %}
                        {% if not loop.last %}
                        {% endif %} {% endfor %}
                        {% else %} {                                    * {% if
                        { commit.title }} {%                              commit.approvers %}
-                       endif %} {% if               * {                  {% for approver in
-{{ commit.commit_hash  commit.description %}          {                  commit.approvers %}
-}}                         * {% for line in           commit.autor     * {{ approver }}
-Issue _#_{                     commit.description       }}               * {% endfor %}
-_{                            %}                     * {                * {
-_c_o_m_m_i_t_._g_i_t_l_a_b___i_s_s_u_e___i_d     * {% if "`" in line        {                  {
-_}_}                           %} {% set                commit.date        commit.approver_date
-                             line_words =             }}                 }}
+{{ commit.commit_hash  endif %} {% if               * {                  {% for approver in
+}}                     commit.description %}          {                  commit.approvers %}
+{% if                      * {% for line in           commit.autor     * {{ approver }}
+commit.gitlab_issue_id       commit.description       }}               * {% endfor %}
+!= "0" %} Issue _#_{           %}                     * {                * {
+_{                          * {% if "`" in line        {                  {
+_c_o_m_m_i_t_._g_i_t_l_a_b___i_s_s_u_e___i_d       %} {% set                commit.date        commit.approver_date
+_}_} {% endif %}               line_words =             }}                 }}
                              line.split() %} {%                    {% else %} Not found {%
                              for word in                           endif %}
                              line_words %} {%
                              if '`' in word %}
                              {{ word.replace
                              ('`', '')|e }} {%
                              else %} {{ word|e
@@ -37,10 +37,10 @@
                              %} {% endif %} {%
                              endfor %} {% else
                              %} {{ line }} {%
                              endif %}
                            * {% endfor %}
                        {% endif %}
 {% endfor %}
-********** LLiisstt ooff ppaarrttiicciippaannttss **********
+********** LLiisstt ooff rreevviieewweerrss **********
 NNaammee              RRoollee SSiiggnnaattuurree DDaattee
 {{ participant }}
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard.egg-info/PKG-INFO` & `lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-grognard
-Version: 2.0.0
+Version: 2.1.0.dev0
 Summary: Lupin linter tool
 License: MIT License
 Keywords: cli,linter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-grognard-2.0.0/lupin_grognard.egg-info/SOURCES.txt` & `lupin_grognard-2.1.0.dev0/lupin_grognard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0/setup.cfg` & `lupin_grognard-2.1.0.dev0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d67 726f 676e 6172   = lupin-grognar
-00000020: 640d 0a76 6572 7369 6f6e 203d 2032 2e30  d..version = 2.0
-00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
-00000040: 3d20 4c75 7069 6e20 6c69 6e74 6572 2074  = Lupin linter t
-00000050: 6f6f 6c0d 0a6c 6f6e 675f 6465 7363 7269  ool..long_descri
-00000060: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-00000070: 4144 4d45 2e6d 640d 0a6b 6579 776f 7264  ADME.md..keyword
-00000080: 7320 3d20 636c 692c 206c 696e 7465 720d  s = cli, linter.
-00000090: 0a6c 6963 656e 7365 203d 204d 4954 204c  .license = MIT L
-000000a0: 6963 656e 7365 0d0a 636c 6173 7369 6669  icense..classifi
-000000b0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000000c0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
-000000d0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
-000000e0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000000f0: 496e 666f 726d 6174 696f 6e20 5465 6368  Information Tech
-00000100: 6e6f 6c6f 6779 0d0a 0954 6f70 6963 203a  nology...Topic :
-00000110: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000120: 6f70 6d65 6e74 203a 3a20 5175 616c 6974  opment :: Qualit
-00000130: 7920 4173 7375 7261 6e63 650d 0a09 5072  y Assurance...Pr
-00000140: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000160: 332e 3130 0d0a 094c 6963 656e 7365 203a  3.10...License :
-00000170: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000180: 3a20 4d49 5420 4c69 6365 6e73 650d 0a0d  : MIT License...
-00000190: 0a5b 6f70 7469 6f6e 735d 0d0a 7a69 705f  .[options]..zip_
-000001a0: 7361 6665 203d 2046 616c 7365 0d0a 696e  safe = False..in
-000001b0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-000001c0: 7461 203d 2054 7275 650d 0a70 6163 6b61  ta = True..packa
-000001d0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-000001e0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000001f0: 3d33 2e31 300d 0a69 6e73 7461 6c6c 5f72  =3.10..install_r
-00000200: 6571 7569 7265 7320 3d20 0d0a 0974 7970  equires = ...typ
-00000210: 6572 5b61 6c6c 5d3d 3d30 2e36 2e31 0d0a  er[all]==0.6.1..
-00000220: 0970 7974 686f 6e2d 646f 7465 6e76 3d3d  .python-dotenv==
-00000230: 302e 3231 2e30 0d0a 0965 6d6f 6a69 3d3d  0.21.0...emoji==
-00000240: 322e 322e 300d 0a09 4a69 6e6a 6132 3d3d  2.2.0...Jinja2==
-00000250: 332e 312e 320d 0a09 636d 616b 656c 616e  3.1.2...cmakelan
-00000260: 673d 3d30 2e36 2e31 330d 0a09 5079 5941  g==0.6.13...PyYA
-00000270: 4d4c 3d3d 362e 302e 310d 0a0d 0a5b 6f70  ML==6.0.1....[op
-00000280: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
-00000290: 7569 7265 5d0d 0a74 6573 7420 3d20 0d0a  uire]..test = ..
-000002a0: 0970 7974 6573 743d 3d37 2e31 2e33 0d0a  .pytest==7.1.3..
-000002b0: 0966 6c61 6b65 383d 3d35 2e30 2e34 0d0a  .flake8==5.0.4..
-000002c0: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
-000002d0: 5f70 6f69 6e74 735d 0d0a 636f 6e73 6f6c  _points]..consol
-000002e0: 655f 7363 7269 7074 7320 3d20 0d0a 0967  e_scripts = ...g
-000002f0: 726f 6720 3d20 6c75 7069 6e5f 6772 6f67  rog = lupin_grog
-00000300: 6e61 7264 2e72 756e 3a63 6c69 0d0a 0d0a  nard.run:cli....
-00000310: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000320: 5f64 6174 615d 0d0a 2a20 3d20 2a2e 636c  _data]..* = *.cl
-00000330: 616e 672d 666f 726d 6174 0d0a 0d0a 5b6f  ang-format....[o
-00000340: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000350: 6669 6e64 5d0d 0a65 7863 6c75 6465 203d  find]..exclude =
-00000360: 200d 0a09 6c75 7069 6e5f 6772 6f67 6e61   ...lupin_grogna
-00000370: 7264 2e74 6573 7473 2a0d 0a0d 0a5b 6567  rd.tests*....[eg
-00000380: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000390: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000003a0: 3d20 300d 0a0d 0a                        = 0....
+00000020: 640d 0a76 6572 7369 6f6e 203d 2032 2e31  d..version = 2.1
+00000030: 2e30 2e64 6576 300d 0a64 6573 6372 6970  .0.dev0..descrip
+00000040: 7469 6f6e 203d 204c 7570 696e 206c 696e  tion = Lupin lin
+00000050: 7465 7220 746f 6f6c 0d0a 6c6f 6e67 5f64  ter tool..long_d
+00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6b65  e: README.md..ke
+00000080: 7977 6f72 6473 203d 2063 6c69 2c20 6c69  ywords = cli, li
+00000090: 6e74 6572 0d0a 6c69 6365 6e73 6520 3d20  nter..license = 
+000000a0: 4d49 5420 4c69 6365 6e73 650d 0a63 6c61  MIT License..cla
+000000b0: 7373 6966 6965 7273 203d 200d 0a09 4465  ssifiers = ...De
+000000c0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+000000d0: 203a 3a20 3320 2d20 416c 7068 610d 0a09   :: 3 - Alpha...
+000000e0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+000000f0: 6520 3a3a 2049 6e66 6f72 6d61 7469 6f6e  e :: Information
+00000100: 2054 6563 686e 6f6c 6f67 790d 0a09 546f   Technology...To
+00000110: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000120: 4465 7665 6c6f 706d 656e 7420 3a3a 2051  Development :: Q
+00000130: 7561 6c69 7479 2041 7373 7572 616e 6365  uality Assurance
+00000140: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000150: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000160: 6e20 3a3a 2033 2e31 300d 0a09 4c69 6365  n :: 3.10...Lice
+00000170: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000180: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000190: 7365 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  se....[options].
+000001a0: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
+000001b0: 650d 0a69 6e63 6c75 6465 5f70 6163 6b61  e..include_packa
+000001c0: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
+000001d0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+000001e0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+000001f0: 7320 3d20 3e3d 332e 3130 0d0a 696e 7374  s = >=3.10..inst
+00000200: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000210: 0a09 7479 7065 725b 616c 6c5d 3d3d 302e  ..typer[all]==0.
+00000220: 362e 310d 0a09 7079 7468 6f6e 2d64 6f74  6.1...python-dot
+00000230: 656e 763d 3d30 2e32 312e 300d 0a09 656d  env==0.21.0...em
+00000240: 6f6a 693d 3d32 2e32 2e30 0d0a 094a 696e  oji==2.2.0...Jin
+00000250: 6a61 323d 3d33 2e31 2e32 0d0a 0963 6d61  ja2==3.1.2...cma
+00000260: 6b65 6c61 6e67 3d3d 302e 362e 3133 0d0a  kelang==0.6.13..
+00000270: 0950 7959 414d 4c3d 3d36 2e30 2e31 0d0a  .PyYAML==6.0.1..
+00000280: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
+00000290: 735f 7265 7175 6972 655d 0d0a 7465 7374  s_require]..test
+000002a0: 203d 200d 0a09 7079 7465 7374 3d3d 372e   = ...pytest==7.
+000002b0: 312e 330d 0a09 666c 616b 6538 3d3d 352e  1.3...flake8==5.
+000002c0: 302e 340d 0a0d 0a5b 6f70 7469 6f6e 732e  0.4....[options.
+000002d0: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+000002e0: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+000002f0: 200d 0a09 6772 6f67 203d 206c 7570 696e   ...grog = lupin
+00000300: 5f67 726f 676e 6172 642e 7275 6e3a 636c  _grognard.run:cl
+00000310: 690d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  i....[options.pa
+00000320: 636b 6167 655f 6461 7461 5d0d 0a2a 203d  ckage_data]..* =
+00000330: 202a 2e63 6c61 6e67 2d66 6f72 6d61 740d   *.clang-format.
+00000340: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000350: 6167 6573 2e66 696e 645d 0d0a 6578 636c  ages.find]..excl
+00000360: 7564 6520 3d20 0d0a 096c 7570 696e 5f67  ude = ...lupin_g
+00000370: 726f 676e 6172 642e 7465 7374 732a 0d0a  rognard.tests*..
+00000380: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000390: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000003a0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

