# Comparing `tmp/batchfetch-1.1.0.tar.gz` & `tmp/batchfetch-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchfetch-1.1.0.tar", last modified: Fri May 10 17:57:02 2024, max compression
+gzip compressed data, was "batchfetch-1.1.1.tar", last modified: Wed May 15 15:26:01 2024, max compression
```

## Comparing `batchfetch-1.1.0.tar` & `batchfetch-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:57:02.147992 batchfetch-1.1.0/
--rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-10 17:56:54.000000 batchfetch-1.1.0/.gitignore
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-10 17:56:54.000000 batchfetch-1.1.0/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-10 17:57:02.147992 batchfetch-1.1.0/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-10 17:56:54.000000 batchfetch-1.1.0/README.md
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:57:02.144658 batchfetch-1.1.0/batchfetch/
--rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-10 17:56:54.000000 batchfetch-1.1.0/batchfetch/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     5437 2024-05-10 17:56:54.000000 batchfetch-1.1.0/batchfetch/batchfetch_base.py
--rw-r--r--   0 dev        (455) work      (1000)     9749 2024-05-10 17:56:54.000000 batchfetch-1.1.0/batchfetch/batchfetch_cli.py
--rw-r--r--   0 dev        (455) work      (1000)    13639 2024-05-10 17:56:54.000000 batchfetch-1.1.0/batchfetch/batchfetch_git.py
--rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-10 17:56:54.000000 batchfetch-1.1.0/batchfetch/helpers.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:57:02.147992 batchfetch-1.1.0/batchfetch.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-10 17:57:01.000000 batchfetch-1.1.0/batchfetch.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-10 17:57:02.000000 batchfetch-1.1.0/batchfetch.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-10 17:57:01.000000 batchfetch-1.1.0/batchfetch.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-10 17:57:01.000000 batchfetch-1.1.0/batchfetch.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-10 17:57:01.000000 batchfetch-1.1.0/batchfetch.egg-info/requires.txt
--rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-10 17:57:01.000000 batchfetch-1.1.0/batchfetch.egg-info/top_level.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-10 17:56:54.000000 batchfetch-1.1.0/run_tests.sh
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-10 17:57:02.147992 batchfetch-1.1.0/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-10 17:56:54.000000 batchfetch-1.1.0/setup.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:57:02.147992 batchfetch-1.1.0/tests/
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:57:02.147992 batchfetch-1.1.0/tests/data/
--rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-10 17:56:54.000000 batchfetch-1.1.0/tests/data/test-md5sum.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-10 17:56:54.000000 batchfetch-1.1.0/tests/data/test-run_simple.sh
--rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-10 17:56:54.000000 batchfetch-1.1.0/tests/test_helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/
+-rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-15 15:25:56.000000 batchfetch-1.1.1/.gitignore
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-15 15:25:56.000000 batchfetch-1.1.1/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-15 15:26:01.702767 batchfetch-1.1.1/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-15 15:25:56.000000 batchfetch-1.1.1/README.md
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/batchfetch/
+-rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     5951 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/batchfetch_base.py
+-rw-r--r--   0 dev        (455) work      (1000)     9753 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/batchfetch_cli.py
+-rw-r--r--   0 dev        (455) work      (1000)    13709 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/batchfetch_git.py
+-rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-15 15:25:56.000000 batchfetch-1.1.1/batchfetch/helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/batchfetch.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/requires.txt
+-rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-15 15:26:01.000000 batchfetch-1.1.1/batchfetch.egg-info/top_level.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-15 15:25:56.000000 batchfetch-1.1.1/run_tests.sh
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-15 15:26:01.702767 batchfetch-1.1.1/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-15 15:25:56.000000 batchfetch-1.1.1/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/tests/
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-15 15:26:01.702767 batchfetch-1.1.1/tests/data/
+-rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-15 15:25:56.000000 batchfetch-1.1.1/tests/data/test-md5sum.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-15 15:25:56.000000 batchfetch-1.1.1/tests/data/test-run_simple.sh
+-rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-15 15:25:56.000000 batchfetch-1.1.1/tests/test_helpers.py
```

### Comparing `batchfetch-1.1.0/.gitignore` & `batchfetch-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.0/LICENSE` & `batchfetch-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.0/PKG-INFO` & `batchfetch-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.1.0
+Version: 1.1.1
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `batchfetch-1.1.0/README.md` & `batchfetch-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.0/batchfetch/__init__.py` & `batchfetch-1.1.1/batchfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.0/batchfetch/batchfetch_base.py` & `batchfetch-1.1.1/batchfetch/batchfetch_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,85 +28,118 @@
 from .helpers import run_indent_str
 
 
 class BatchFetchError(Exception):
     """Exception raised by Downloader()."""
 
 
-class BatchFetchBase:
-    """Plugin downloader base class."""
-
-    def __init__(self, data: Dict[str, Any], options: Dict[str, Any]):
-        self.indent = 4
-        self.env = os.environ.copy()
+class DataAlreadyInitialized(Exception):
+    """Data already initialized."""
 
-        # Default
-        self.global_options_schema: Dict[Any, Any] = {
-            Optional("exec_before"): Or([str], str),
-            Optional("exec_after"): Or([str], str),
-        }
 
-        self.item_schema: Dict[Any, Any] = {
-            Optional("path"): str,
-            Optional("delete"): bool,
-
-            Optional("exec_before"): Or([str], str),
-            Optional("exec_after"): Or([str], str),
-        }
-
-        self.global_options_values: Dict[str, Any] = {
-            "exec_before": [],
-            "exec_after": [],
-        }
+class TaskBase:
+    def __init__(self, data: Dict[str, Any], options: Dict[str, Any]):
+        self.global_options_schema: Dict[Any, Any] = {}
+        self.global_options_values: Dict[str, Any] = {}
 
-        self.item_default_values: Dict[str, Any] = {
-            # Optional items
-            "delete": False,
-        }
+        self.task_schema: Dict[Any, Any] = {}
+        self.task_default_values: Dict[str, Any] = {}
 
         self._item_values = data
-        self._item_global_options = options
+        self._item_options = options
 
         # Variables
         self.values: Dict[str, Any] = {}
         self.options: Dict[str, Any] = {}
         self._values_initialized = False
 
     def _initialize_data(self):
         if self._values_initialized:
-            return
+            raise DataAlreadyInitialized
 
         # Options
         self.options = {}
-        self.options.update(deepcopy(self._item_global_options))
+        self.options.update(deepcopy(self.global_options_values))  # Default
+        self.options.update(deepcopy(self._item_options))
         schema = Schema(self.global_options_schema)
         schema.validate(self.options)
 
         # Data
         self.values = {}
-        self.values.update(deepcopy(self.item_default_values))
+        self.values.update(deepcopy(self.task_default_values))
         self.values.update(deepcopy(self._item_values))
-        # self.values.update(deepcopy(self._item_global_options))
-        schema = Schema(self.item_schema)
+        schema = Schema(self.task_schema)
         schema.validate(self.values)
 
         self.values["result"] = {
             "output": "",
             "error": False,
             "changed": False,
         }
 
-        self._values_initialized = True
+    def validate_schema(self):
+        self._initialize_data()
+
+    def __getitem__(self, key):
+        self._initialize_data()
+
+        if key in self.values:
+            return self.values[key]
+
+        if key in self.options:
+            return self.options[key]
+
+        if key in self.global_options_values:
+            return self.global_options_values[key]
+
+        raise KeyError(f"The item '{key}' was not found in '{self.values}")
+
+
+class BatchFetchBase(TaskBase):
+    """Plugin downloader base class."""
 
-        # Strip spaces
-        self.values = {
-            key: value.strip() if isinstance(value, str) else value
-            for key, value in self.values.items()
+    def __init__(self, data: Dict[str, Any], options: Dict[str, Any]):
+        super().__init__(data=data, options=options)
+        self.indent = 4
+        self.indent_spaces = " " * self.indent
+        self.env = os.environ.copy()
+
+        # Default
+        self.global_options_schema: Dict[Any, Any] = {
+            Optional("exec_before"): Or([str], str),
+            Optional("exec_after"): Or([str], str),
+        }
+
+        self.task_schema: Dict[Any, Any] = {
+            Optional("path"): str,
+            Optional("delete"): bool,
+
+            Optional("exec_before"): Or([str], str),
+            Optional("exec_after"): Or([str], str),
+        }
+
+        self.global_options_values: Dict[str, Any] = {
+            "exec_before": [],
+            "exec_after": [],
+        }
+
+        self.task_default_values: Dict[str, Any] = {
+            # Optional items
+            "delete": False,
         }
 
+    def _initialize_data(self):
+        try:
+            super()._initialize_data()
+        except DataAlreadyInitialized:
+            return
+
+        # Mark values as initialized
+        self._values_initialized = True
+
     def _run(self, *args, **kwargs):
         stdout = run_indent_str(*args, **kwargs)
 
         if not stdout.endswith("\n"):
             stdout += "\n"
         self.add_output(stdout)
 
@@ -127,31 +160,14 @@
         for post_exec in self["exec_after"]:
             if not post_exec:
                 continue
 
             self._run(post_exec, cwd=str(cwd), env=self.env,
                       spaces=self.indent)
 
-    def __getitem__(self, key):
-        self._initialize_data()
-
-        if key in self.values:
-            return self.values[key]
-
-        if key in self.options:
-            return self.options[key]
-
-        if key in self.global_options_values:
-            return self.global_options_values[key]
-
-        raise KeyError(f"The item '{key}' was not found in '{self.values}")
-
-    def validate_schema(self):
-        self._initialize_data()
-
     def is_changed(self) -> bool:
         self._initialize_data()
         return bool(self.values["result"]["changed"])
 
     def set_changed(self, changed: bool):
         self._initialize_data()
         self.values["result"]["changed"] = changed
```

### Comparing `batchfetch-1.1.0/batchfetch/batchfetch_cli.py` & `batchfetch-1.1.1/batchfetch/batchfetch_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self._plugin_add("git", BatchFetchGit)
 
     def _plugin_add(self, keyword: str, batchfetch_class: Any):
         batchfetch_instance = batchfetch_class(data={},
                                                options={})
         batchfetch_instance.validate_schema()
 
-        self.batchfetch_schemas[keyword] = batchfetch_instance.item_schema
+        self.batchfetch_schemas[keyword] = batchfetch_instance.task_schema
         self.batchfetch_classes[keyword] = batchfetch_class
         self.cfg_schema = {
             Optional("options"):
                 batchfetch_instance.global_options_schema,  # type: ignore
             Optional("tasks"): [
                 Or(*list(self.batchfetch_schemas.values()))
             ]
@@ -101,15 +101,15 @@
         try:
             schema.validate(data)
         except SchemaError as err:
             print(f"Schema error: {err}.", file=sys.stderr)
             sys.exit(1)
 
         self.cfg = {
-            "options": {"clone_args": []},
+            "options": {"git_clone_args": []},
             "tasks": [],
         }
 
         if "options" in data:
             self.cfg["options"].update(data["options"])
 
         self._loads_tasks(data)
```

### Comparing `batchfetch-1.1.0/batchfetch/batchfetch_git.py` & `batchfetch-1.1.1/batchfetch/batchfetch_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,39 +38,39 @@
 
 class BatchFetchGit(BatchFetchBase):
     """Clone or update a Git repository."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.env["GIT_TERMINAL_PROMPT"] = "0"
-        self.indent_spaces = " " * self.indent
+        self.env["GIT_PAGER"] = ""
         self.main_key = "git"
 
         # Schema
-        self.item_schema.update({
+        self.task_schema.update({
             # Local options
             self.main_key: str,
             Optional("reference"): str,
 
             # Same as global options
-            Optional("clone_args"): [str],
+            Optional("git_clone_args"): [str],
             Optional("git_pull"): bool,
         })
 
         self.global_options_schema.update({
             # Global options
-            Optional("clone_args"): [str],
+            Optional("git_clone_args"): [str],
             Optional("git_pull"): bool,
         })
 
         # Data
-        self.global_options_values.update({"clone_args": [],
+        self.global_options_values.update({"git_clone_args": [],
                                            "git_pull": True})
 
-        self.item_default_values.update({
+        self.task_default_values.update({
             self.main_key: "",
             "reference": "",
             "delete": False,
         })
 
         self.git_local_dir = Path(self["path"])
         self.current_branch = None
@@ -187,15 +187,15 @@
         elif self.git_local_dir.is_dir():
             shutil.rmtree(str(self.git_local_dir))
             self.add_output(self.indent_spaces +
                             f"[INFO] Deleted: '{self.git_local_dir}'")
             self.set_changed(True)
 
     def _repo_clone(self):
-        git_clone_args = self["clone_args"]
+        git_clone_args = self["git_clone_args"]
         git_clone_args += ["--recurse-submodules"]
 
         cmd = ["git", "clone"] + git_clone_args + \
             [self[self.main_key], str(self.git_local_dir)]
         self._run(cmd, env=self.env)
         self.set_changed(True)
 
@@ -250,15 +250,15 @@
         # Fetch
         cmd = ["git", "fetch", "origin"]
         self._run(cmd, cwd=str(self.git_local_dir), env=self.env)
 
         # Merge
         real_branch = self._git_is_local_branch("HEAD")
         if real_branch:
-           # TODO: only merge when difference from upstream
+            # TODO: only merge when difference from upstream
             commit_ref_head = self._git_ref(cwd=self.git_local_dir)
             self._run(["git", "merge", "--ff-only"],
                       cwd=str(self.git_local_dir), env=self.env)
             git_ref_after_merge = self._git_ref(cwd=self.git_local_dir)
             if commit_ref_head != git_ref_after_merge:
                 git_merge = True
                 self.set_changed(True)
@@ -311,17 +311,18 @@
                 env=self.env,
                 cwd=self.git_local_dir,
             )
 
             # Also check the commit reference in case
             # branch is a commit reference instead of a tag
             try:
-                git_ref_branch = self._git_tags(self["reference"])[0]
+                git_ref_branch = self._git_tags(self["reference"] +
+                                                "^{commit}")[0]
             except GitReferenceDoesNotExist as err:
-                raise BatchFetchError(f"The branch '{self['branch']}' "
+                raise BatchFetchError(f"The branch '{self['reference']}' "
                                       "does not exist.") from err
 
             if git_ref_after_merge != git_ref_branch and \
                     self["reference"] not in git_tags:
                 # Update the branch
                 self._run(["git", "checkout"] + [self["reference"]],
                           cwd=str(self.git_local_dir), env=self.env)
```

### Comparing `batchfetch-1.1.0/batchfetch/helpers.py` & `batchfetch-1.1.1/batchfetch/helpers.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.0/batchfetch.egg-info/PKG-INFO` & `batchfetch-1.1.1/batchfetch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.1.0
+Version: 1.1.1
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `batchfetch-1.1.0/run_tests.sh` & `batchfetch-1.1.1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `batchfetch-1.1.0/setup.py` & `batchfetch-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="batchfetch",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     description="Efficiently clone and pull multiple Git repositories.",
     license="GPLv3",
     long_description=((Path(__file__).parent.resolve().joinpath("README.md"))
                       .read_text(encoding="utf-8")),
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/batchfetch",
```

### Comparing `batchfetch-1.1.0/tests/test_helpers.py` & `batchfetch-1.1.1/tests/test_helpers.py`

 * *Files identical despite different names*

