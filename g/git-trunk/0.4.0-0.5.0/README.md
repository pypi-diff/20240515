# Comparing `tmp/git_trunk-0.4.0.tar.gz` & `tmp/git_trunk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/git_trunk-0.4.0.tar", last modified: Tue Nov  3 11:01:01 2020, max compression
+gzip compressed data, was "dist/git_trunk-0.5.0.tar", last modified: Mon Mar  1 13:45:33 2021, max compression
```

## Comparing `git_trunk-0.4.0.tar` & `git_trunk-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 oerp      (1001) oerp      (1001)        0 2020-11-03 11:01:01.000000 git_trunk-0.4.0/
-drwxrwxr-x   0 oerp      (1001) oerp      (1001)        0 2020-11-03 11:01:01.000000 git_trunk-0.4.0/git_trunk/
--rw-rw-r--   0 oerp      (1001) oerp      (1001)     9228 2020-11-03 10:55:12.000000 git_trunk-0.4.0/git_trunk/git_trunk_config.py
--rw-rw-r--   0 oerp      (1001) oerp      (1001)       22 2020-11-03 10:55:12.000000 git_trunk-0.4.0/git_trunk/__init__.py
--rw-rw-r--   0 oerp      (1001) oerp      (1001)     4085 2020-11-03 10:55:12.000000 git_trunk-0.4.0/git_trunk/version.py
--rw-rw-r--   0 oerp      (1001) oerp      (1001)    24030 2020-11-03 10:55:12.000000 git_trunk-0.4.0/git_trunk/git_trunk_commands.py
--rw-rw-r--   0 oerp      (1001) oerp      (1001)    14257 2020-11-03 10:55:12.000000 git_trunk-0.4.0/git_trunk/git_trunk_base.py
--rw-rw-r--   0 oerp      (1001) oerp      (1001)    43540 2020-04-01 13:23:08.000000 git_trunk-0.4.0/LICENSE
--rw-rw-r--   0 oerp      (1001) oerp      (1001)      859 2020-04-01 13:23:08.000000 git_trunk-0.4.0/setup.py
--rw-rw-r--   0 oerp      (1001) oerp      (1001)     8836 2020-11-03 10:55:12.000000 git_trunk-0.4.0/README.rst
--rw-rw-r--   0 oerp      (1001) oerp      (1001)    10391 2020-11-03 11:01:01.000000 git_trunk-0.4.0/PKG-INFO
-drwxrwxr-x   0 oerp      (1001) oerp      (1001)        0 2020-11-03 11:01:01.000000 git_trunk-0.4.0/bin/
--rwxrwxr-x   0 oerp      (1001) oerp      (1001)    13851 2020-11-03 10:55:12.000000 git_trunk-0.4.0/bin/git-trunk
+drwxr-xr-x   0 silvija   (1000) silvija   (1000)        0 2021-03-01 13:45:33.000000 git_trunk-0.5.0/
+drwxr-xr-x   0 silvija   (1000) silvija   (1000)        0 2021-03-01 13:45:33.000000 git_trunk-0.5.0/bin/
+-rwxr-xr-x   0 silvija   (1000) silvija   (1000)    13851 2021-02-25 07:39:41.000000 git_trunk-0.5.0/bin/git-trunk
+-rw-r--r--   0 silvija   (1000) silvija   (1000)     8836 2021-02-25 07:39:41.000000 git_trunk-0.5.0/README.rst
+drwxr-xr-x   0 silvija   (1000) silvija   (1000)        0 2021-03-01 13:45:33.000000 git_trunk-0.5.0/git_trunk/
+-rw-r--r--   0 silvija   (1000) silvija   (1000)     9228 2021-02-25 07:39:41.000000 git_trunk-0.5.0/git_trunk/git_trunk_config.py
+-rw-r--r--   0 silvija   (1000) silvija   (1000)    24077 2021-03-01 13:42:07.000000 git_trunk-0.5.0/git_trunk/git_trunk_commands.py
+-rw-r--r--   0 silvija   (1000) silvija   (1000)    14257 2021-02-25 07:39:41.000000 git_trunk-0.5.0/git_trunk/git_trunk_base.py
+-rw-r--r--   0 silvija   (1000) silvija   (1000)       22 2021-03-01 13:42:07.000000 git_trunk-0.5.0/git_trunk/__init__.py
+-rw-r--r--   0 silvija   (1000) silvija   (1000)    10391 2021-03-01 13:45:33.000000 git_trunk-0.5.0/PKG-INFO
+-rw-r--r--   0 silvija   (1000) silvija   (1000)      838 2021-03-01 13:42:07.000000 git_trunk-0.5.0/setup.py
+-rw-r--r--   0 silvija   (1000) silvija   (1000)    43540 2020-05-07 12:33:26.000000 git_trunk-0.5.0/LICENSE
```

### Comparing `git_trunk-0.4.0/git_trunk/git_trunk_config.py` & `git_trunk-0.5.0/git_trunk/git_trunk_config.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.4.0/git_trunk/git_trunk_commands.py` & `git_trunk-0.5.0/git_trunk/git_trunk_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Git Trunk based workflow helper commands."""
 import re
 from collections import namedtuple
 from typing import Optional, Union
 import natsort
 from footil.path import chdir_tmp
 from footil.patterns import MethodCommand
+from footil import version as version_manager
 import git  # GitPython
 
 from . import git_trunk_base as gt_base
 from . import git_trunk_config as gt_config
-from . import version as version_manager
 
 EMPTY_VERSION = '0.0.0'  # default version when are no versions yet
 
 MethodData = namedtuple('MethodData', 'method args kwargs')
 # Set defaults for args and kwargs.
 MethodData.__new__.__defaults__ = ((), {})
 
@@ -265,29 +265,31 @@
                 trunk_branch_name,
                 trunk_tracking_data,
                 [
                     MethodData(
                         method=self.git_push,
                         args=(
                             trunk_tracking_data.remote,
-                            trunk_tracking_data.head)
+                            trunk_tracking_data.head,
                         )
+                    )
                 ]
             )
         if active_tracking_data:
             handle_tracking_data(
                 active_branch_name,
                 active_tracking_data,
                 [
                     MethodData(
                         method=self.git_delete_remote_branch,
                         args=(
                             active_tracking_data.remote,
-                            active_tracking_data.head)
+                            active_tracking_data.head,
                         )
+                    )
                 ]
             )
         force_delete = False
         if not self.is_release_branch(active_branch_name):
             self._merge_branch(active_branch_name)
         else:
             # Need to be explicit when deleting not merged branch.
@@ -545,15 +547,15 @@
         if include_squash_msg:
             # Include one extra commit, to also have message from commit
             # that will be left after squashing.
             return self._get_n_logs_body(squash_count + 1)
         return None
 
     def _amend_commit_for_squash(
-            self, message: Union[None, str] = None):
+            self, message: Union[None, str]=None):
         args = ['--amend']
         if message:
             args.extend(['-m', message])
         else:
             args.append('--no-edit')
         self.git.commit(*args)
```

### Comparing `git_trunk-0.4.0/git_trunk/git_trunk_base.py` & `git_trunk-0.5.0/git_trunk/git_trunk_base.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.4.0/LICENSE` & `git_trunk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_trunk-0.4.0/setup.py` & `git_trunk-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     name='git_trunk',
     version=__version__,
     packages=['git_trunk'],
     license='LGPLv3',
     url='https://github.com/focusate/git-trunk',
     description="Git Trunk based workflow",
     long_description=open('README.rst').read(),
-    install_requires=['footil>=0.19.0', 'gitpython', 'semver', 'natsort'],
+    install_requires=['footil>=0.24.0', 'gitpython'],
     scripts=['bin/git-trunk'],
     maintainer='Andrius Laukavičius',
     maintainer_email='dev@focusate.eu',
     python_requires='>=3.5',
     classifiers=[
         'Environment :: Other Environment',
         'Intended Audience :: Developers',
```

### Comparing `git_trunk-0.4.0/README.rst` & `git_trunk-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `git_trunk-0.4.0/PKG-INFO` & `git_trunk-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: git_trunk
-Version: 0.4.0
+Version: 0.5.0
 Summary: Git Trunk based workflow
 Home-page: https://github.com/focusate/git-trunk
 Author: Andrius Laukavičius
 Author-email: dev@focusate.eu
 License: LGPLv3
 Description: .. image:: https://travis-ci.com/focusate/git-trunk.svg?branch=master
             :target: https://travis-ci.com/focusate/git-trunk
```

### Comparing `git_trunk-0.4.0/bin/git-trunk` & `git_trunk-0.5.0/bin/git-trunk`

 * *Files identical despite different names*

