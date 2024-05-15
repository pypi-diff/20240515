# Comparing `tmp/aedev_git_repo_manager-0.3.78.tar.gz` & `tmp/aedev_git_repo_manager-0.3.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aedev_git_repo_manager-0.3.78.tar", last modified: Sat May  4 14:51:17 2024, max compression
+gzip compressed data, was "aedev_git_repo_manager-0.3.79.tar", last modified: Tue May 14 17:04:56 2024, max compression
```

## Comparing `aedev_git_repo_manager-0.3.78.tar` & `aedev_git_repo_manager-0.3.79.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 14:51:17.507407 aedev_git_repo_manager-0.3.78/
--rw-rw-rw-   0 root         (0) root         (0)    35002 2024-05-04 14:51:06.000000 aedev_git_repo_manager-0.3.78/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     6549 2024-05-04 14:51:17.507407 aedev_git_repo_manager-0.3.78/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-05-04 14:51:06.000000 aedev_git_repo_manager-0.3.78/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 14:51:17.500089 aedev_git_repo_manager-0.3.78/aedev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 14:51:17.501919 aedev_git_repo_manager-0.3.78/aedev/git_repo_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1879 2024-05-04 14:51:06.000000 aedev_git_repo_manager-0.3.78/aedev/git_repo_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   188569 2024-05-04 14:51:06.000000 aedev_git_repo_manager-0.3.78/aedev/git_repo_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 14:51:17.503748 aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6549 2024-05-04 14:51:17.000000 aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-04 14:51:17.000000 aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-04 14:51:17.000000 aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2024-05-04 14:51:17.000000 aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      543 2024-05-04 14:51:17.000000 aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-04 14:51:17.000000 aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-04 14:51:17.000000 aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-04 14:51:17.507407 aedev_git_repo_manager-0.3.78/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-05-04 14:51:06.000000 aedev_git_repo_manager-0.3.78/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 14:51:17.503748 aedev_git_repo_manager-0.3.78/tests/
--rw-rw-rw-   0 root         (0) root         (0)   157998 2024-05-04 14:51:06.000000 aedev_git_repo_manager-0.3.78/tests/test_git_repo_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:04:56.363640 aedev_git_repo_manager-0.3.79/
+-rw-rw-rw-   0 root         (0) root         (0)    35002 2024-05-14 17:04:43.000000 aedev_git_repo_manager-0.3.79/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-05-14 17:04:56.363640 aedev_git_repo_manager-0.3.79/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-05-14 17:04:43.000000 aedev_git_repo_manager-0.3.79/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:04:56.355640 aedev_git_repo_manager-0.3.79/aedev/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:04:56.357640 aedev_git_repo_manager-0.3.79/aedev/git_repo_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2024-05-14 17:04:43.000000 aedev_git_repo_manager-0.3.79/aedev/git_repo_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   198634 2024-05-14 17:04:43.000000 aedev_git_repo_manager-0.3.79/aedev/git_repo_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:04:56.360640 aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-05-14 17:04:56.000000 aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-14 17:04:56.000000 aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 17:04:56.000000 aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-14 17:04:56.000000 aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      543 2024-05-14 17:04:56.000000 aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-14 17:04:56.000000 aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 17:04:56.000000 aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 17:04:56.363640 aedev_git_repo_manager-0.3.79/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-05-14 17:04:43.000000 aedev_git_repo_manager-0.3.79/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:04:56.359640 aedev_git_repo_manager-0.3.79/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   158050 2024-05-14 17:04:43.000000 aedev_git_repo_manager-0.3.79/tests/test_git_repo_manager.py
```

### Comparing `aedev_git_repo_manager-0.3.78/LICENSE.md` & `aedev_git_repo_manager-0.3.79/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.78/PKG-INFO` & `aedev_git_repo_manager-0.3.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.78
+Version: 0.3.79
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -72,25 +72,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.78
+# git_repo_manager 0.3.79
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.77?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.77)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.78?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.78)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.78.
+>aedev_git_repo_manager package 0.3.79.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.78/README.md` & `aedev_git_repo_manager-0.3.79/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.78
+# git_repo_manager 0.3.79
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.77?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.77)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.78?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.78)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.78.
+>aedev_git_repo_manager package 0.3.79.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.78/aedev/git_repo_manager/__init__.py` & `aedev_git_repo_manager-0.3.79/aedev/git_repo_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 
 in conjunction with the template projects of the `aedev` namespace (like e.g. :mod:`aedev.tpl_project`) any common
 portions file (even the ``setup.py`` file) can be created/maintained as a template in a single place, and then
 requested and updated individually for each portion project.
 """
 
 
-__version__ = '0.3.78'
+__version__ = '0.3.79'
```

### Comparing `aedev_git_repo_manager-0.3.78/aedev/git_repo_manager/__main__.py` & `aedev_git_repo_manager-0.3.79/aedev/git_repo_manager/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 from collections import OrderedDict
 from contextlib import contextmanager
 from difflib import context_diff, diff_bytes, ndiff, unified_diff
 from functools import wraps
 from traceback import format_exc
 from typing import (
     Any, Callable, Collection, Dict, Iterable, Iterator, List, Optional, OrderedDict as OrderedDictType,
-    Sequence, Set, Tuple, Union, cast)
+    Sequence, Set, TYPE_CHECKING, Tuple, Union, cast)
 
 from dotenv import find_dotenv, load_dotenv
 
-from github import Github
+from github import Github, Auth, GithubException
+from github.AuthenticatedUser import AuthenticatedUser
+from github.Repository import Repository
+
 from gitlab import Gitlab, GitlabCreateError, GitlabError, GitlabHttpError
 from gitlab.const import MAINTAINER_ACCESS
-from gitlab.v4.objects import Group, Project, ProjectManager, User, UserProjectManager
+from gitlab.v4.objects import Group, Project, User
 
 from packaging.version import Version
 from PIL import Image
 
 import ae.base                                                                          # type: ignore # for patching
 from ae.base import (
     PY_EXT, PY_INIT, TEMPLATES_FOLDER, UNSET, UnsetType,
@@ -134,14 +137,16 @@
 RegisteredTemplateProject = Dict[str, str]                  #: registered template project info (tpl_projects item)
 RegisteredTemplates = Dict[str, RegisteredTemplateProject]
 
 # PdvVarType = List[RegisteredTemplateProject]; mypy does not recognize PevType: Union[PevType, Dict[str, PdvVarType]]
 PdvType = Dict[str, Any]                                    #: project development variables type
 ChildrenType = OrderedDictType[str, PdvType]                #: children pdv of a project parent or a namespace root
 
+RepoType = Union[Repository, Project]                       #: repo host libs repo object (PyGithub, python-gitlab)
+
 
 # --------------- global variables - most of them are constant after app initialization/startup -----------------------
 
 
 REGISTERED_ACTIONS: RegisteredActions = {}                  #: implemented actions registered via :func:`_action` deco
 
 _RCS: Dict[str, Callable] = {}
@@ -1564,14 +1569,18 @@
         _exit_error(9, "missing package name (specify via the --project or --path option)")
 
     project_type = project_type or pdv_str(pdv, 'project_type')
     namespace_name = _get_namespace(pdv, project_type)
     if namespace_name and not project_name.startswith(namespace_name + '_'):
         project_name = namespace_name + '_' + project_name
 
+    project_path = pdv_str(pdv, 'project_path')
+    _chk_if(9, project_name == os.path.basename(project_path),
+            f"project path '{project_path}' does not end with project name '{project_name}'")
+
     return project_name
 
 
 def _get_renamed_path_package(pdv: PdvType, namespace_name: str, project_type: str) -> Tuple[str, str]:
     _parent_path, project_path, project_name = _get_path_package(pdv, project_type=project_type)
     import_name = namespace_name + '.' + project_name[len(namespace_name) + 1:] if namespace_name else project_name
     old_ns_name = pdv_str(pdv, 'namespace_name')
@@ -1778,25 +1787,23 @@
 def _git_project_version(pdv: PdvType, increment_part: int = 3) -> str:
     """ determine latest or the next free package git repository version or the project specified via the pdv argument.
 
     :param pdv:                 project dev vars to identify the package.
     :param increment_part:      part of the version number to be incremented (1=mayor, 2=minor/namespace, 3=patch).
                                 pass zero/0 to return the latest published package version.
     :return:                    latest published repository package version as string
-                                or "0.0.1" if project never published a version tag to remotes/origin
-                                or empty string on error.
+                                or the first version (increment_version(NULL_VERSION, increment_part) or "0.0.1")
+                                if project never published a version tag to remotes/origin
+                                or an empty string on error.
     """
     if _git_fetch(pdv):
         return ""
 
     version_tags = _git_tag_list(pdv)
-    if not version_tags[-1]:
-        return "0.0.1"
-
-    return increment_version(version_tags[-1][1:], increment_part=increment_part)
+    return increment_version(version_tags[-1][1:] if version_tags[-1] else NULL_VERSION, increment_part=increment_part)
 
 
 def _git_push(pdv: PdvType, *branches_and_tags: str, exit_on_error: bool = True, extra_args: Iterable[str] = ()) -> int:
     """ push portion in the current working directory to the specified branch. """
     protocol = pdv_str(pdv, 'REPO_HOST_PROTOCOL')
     domain = _get_host_domain(pdv)
     project_name = _get_prj_name(pdv)
@@ -2400,48 +2407,256 @@
 
 # --------------- git remote repo connection --------------------------------------------------------------------------
 
 class RemoteHost:
     """ base class registering subclasses as remote host repo class in :data:`REGISTERED_HOSTS_CLASS_NAMES`. """
     name_prefix: str = 'repo'       # config variable name prefix
 
+    create_branch: Callable
+    release_project: Callable
+    repo_obj: Callable
+    request_merge: Callable
+
     def __init_subclass__(cls, **kwargs):
         """ register remote host class name; called on declaration of a subclass of :class:`RemoteHost`. """
         # global REGISTERED_HOSTS_CLASS_NAMES
         REGISTERED_HOSTS_CLASS_NAMES[camel_to_snake(cls.__name__)[1:].replace('_', '.').lower()] = cls.__name__
         super().__init_subclass__(**kwargs)
 
+    def _repo_merge_src_dst_fork_branch(self, ini_pdv: PdvType) -> Tuple[RepoType, RepoType, bool, str]:
+        branch = _get_branch(ini_pdv)
+        domain = _get_host_domain(ini_pdv)
+        group_name = _get_host_group(ini_pdv, domain)
+        project_name = _get_prj_name(ini_pdv)
+
+        remotes = _git_remotes(ini_pdv)
+        forked = 'upstream' in remotes
+        if forked:
+            owner_name = remotes['upstream'].split('/')[-2]
+            _chk_if(64, owner_name == group_name, f"upstream/owner-group mismatch: '{owner_name}' != '{group_name}'")
+            user_name = _get_host_user_name(ini_pdv, domain)
+        else:
+            user_name = group_name
+        origin_user = remotes.get('origin', "/").split('/')[-2]
+        _chk_if(64, origin_user == user_name, f"origin/user mismatch: '{origin_user}' != '{user_name}'")
+
+        # target_project_id/project_id is the upstream and source_project_id is the origin/fork
+        msg = "repository '{name}' not found on remote host server " + self.__class__.__name__
+        src = self.repo_obj(65, f"source/origin/fork {msg}", f"{user_name}/{project_name}")
+        tgt = self.repo_obj(66, f"target/upstream/forked {msg}", f"{group_name}/{project_name}")
+
+        return src, tgt, forked, branch
+
+    def _release_project(self, ini_pdv: PdvType, version_tag: str):
+        errors = _git_fetch(ini_pdv)
+        _chk_if(84, not bool(errors), f"git fetch errors:{_pp(errors)}" + _hint(
+            self.release_project, " later to retry if server is currently unavailable, or check remote configuration"))
+
+        # switch back to local MAIN_BRANCH and then merge-in the release-branch&-tag from remotes/origin/MAIN_BRANCH
+        _git_checkout(ini_pdv, branch=MAIN_BRANCH)
+        _git_merge(ini_pdv, f"origin/{MAIN_BRANCH}")
+
+        if version_tag == 'LATEST':
+            pkg_version = _git_project_version(ini_pdv, increment_part=0)
+            version_tag = f"v{pkg_version}"
+        else:
+            _chk_if(85, version_tag[0] == "v" and version_tag.count(".") == 2, f"version '{version_tag}' format error")
+            pkg_version = version_tag[1:]
+        _chk_if(85, _git_tag_in_branch(ini_pdv, version_tag),
+                f"push version tag {version_tag} has first to be merged into origin/{MAIN_BRANCH}" + _hint(
+                    self.request_merge, " to request to merge your branch."))
+
+        msg = f"updated local {MAIN_BRANCH} branch"
+        if pdv_str(ini_pdv, 'pip_name'):  # create release*ver branch only for projects available in PyPi via pip
+            release_branch = f"release{pkg_version}"
+            _chk_if(85, not _git_tag_in_branch(ini_pdv, release_branch),
+                    f"release branch {release_branch} already exists in origin/{MAIN_BRANCH}")
+            cae.dpo(f"   -- creating branch '{release_branch}' for tag '{version_tag}' at remotes/origin")
+            prj_id = f"{_get_host_group(ini_pdv, _get_host_domain(ini_pdv))}/{pdv_str(ini_pdv, 'project_name')}"
+            self.create_branch(prj_id, release_branch, version_tag)
+            msg += f" and released {pkg_version} onto new protected release branch {release_branch}"
+
+        cae.po(f" ==== {msg} of {pdv_str(ini_pdv, 'project_desc')}")
+
 
 class GithubCom(RemoteHost):
     """ remote connection and actions on remote repo in gitHub.com. """
     connection: Github                  #: connection to GitHub host
 
     def connect(self, ini_pdv: PdvType) -> bool:
         """ connect to gitHub.com remote host.
 
         :param ini_pdv:         project dev vars (host_token).
         :return:                True on successful authentication else False.
         """
         try:
-            self.connection = Github(pdv_val(ini_pdv, 'repo_token'))
+            self.connection = Github(auth=Auth.Token(pdv_val(ini_pdv, 'repo_token')))
         except (Exception, ) as ex:
-            cae.po(f"****  Github connection exception: {ex}")
+            cae.po(f"****  Github authentication exception: {ex}")
             return False
         return True
 
+    def create_branch(self, group_repo: str, branch_name: str, tag_name: str):
+        """ create new remote branch onto/from tag name.
+
+        :param group_repo:      string with owner-user-name/repo-name of the repository, e.g. "UserName/RepositoryName".
+        :param branch_name:     name of the branch to create.
+        :param tag_name:        name of the tag/ref to create branch from.
+        """
+        prj = self.repo_obj(95, "project {name} not found", group_repo)
+        try:
+            git_tag = prj.get_git_tag(tag_name)     # https://gist.github.com/ursulacj/36ade01fa6bd5011ea31f3f6b572834e
+            prj.create_git_ref(f'refs/heads/{branch_name}', git_tag.sha)
+        except (GithubException, Exception):
+            _exit_error(86, f"error creating branch '{branch_name}' for tag '{tag_name}': {format_exc()}")
+
+        # protect branch until GitHub Api supports wildcards in initial push (see comments in self.init_new_repo())
+        self._protect_branches(prj, [branch_name])
+
+    def init_new_repo(self, group_repo: str, project_desc: str):
+        """ config new project repo.
+
+        :param group_repo:      project owner user and repository names in the format "user-name/repo-name".
+        :param project_desc:    project description.
+        """
+        project_repo = self.repo_obj(78, "repository '{name}' to initialize not found", group_repo)
+        cae.vpo(f"    - setting remote project properties of new repository '{group_repo}'")
+        project_repo.edit(default_branch=MAIN_BRANCH, description=project_desc, visibility='public')
+
+        branch_masks = [MAIN_BRANCH]      # , 'release*']
+        self._protect_branches(project_repo, branch_masks)
+        # the GitHub REST api does still not allow to create a branch protection with a wildcard (for release*)
+        # .. see https://github.com/orgs/community/discussions/24703
+        # current workaround is to protect individual release branch in the release_project action
+
+        cae.po(f"   == initialized project and created {len(branch_masks)} protected branch(es): {branch_masks}")
+
+    def repo_obj(self, err_code: int, err_msg: str, group_repo: str) -> Repository:
+        """ convert user repo names to a repository instance of the remote api.
+
+        :param err_code:        error code, pass 0 to not quit if project not found.
+        :param err_msg:         error message to display on error with optional {name} to be automatically substituted
+                                with the project name from the :paramref:`~repo_obj.group_repo_names` argument.
+        :param group_repo:      string with owner-user-name/repo-name of the repository, e.g. "UserName/RepositoryName".
+        :return:                python-github repository if found, else return None if err_code is zero else quit.
+        """
+        try:
+            # search for repo projects: repos = list(self.connection.search_repositories(query="user:AndiEcker"))
+            return self.connection.get_repo(group_repo)
+        except (GithubException, Exception) as gh_ex:
+            if err_code:
+                _exit_error(err_code, err_msg.format(name=group_repo))
+            elif _debug_or_verbose():
+                cae.po(f"   * repository '{group_repo}' not found on connected remote server (exception: {gh_ex})")
+            return cast(Repository, None)
+
+    @staticmethod
+    def _protect_branches(project_repo: Repository, branch_masks: List[str]):
+        for branch_mask in branch_masks:
+            # see also GitHub WebUI docs: https://docs.github.com/de/rest/branches/branch-protection and
+            # https://docs.github.com/de/repositories/configuring-branches-and-merges-in-your-repository/...
+            # ...managing-protected-branches/managing-a-branch-protection-rule
+            # example: https://github.com/txqueuelen/reposettings/blob/master/reposettings.py
+            # .. done with powerscript: https://medium.com/objectsharp/...
+            # ...adding-branch-protection-to-your-repo-with-the-github-rest-api-and-powershell-67ee19425e40
+            branch_obj = project_repo.get_branch(branch_mask)
+            cae.vpo(f"    - protecting branch {branch_mask}")
+            branch_obj.edit_protection(strict=True)
+
     # ----------- remote action methods ----------------------------------------------------------------------------
 
-    # @_action(PARENT_PRJ, arg_names=(('fork-repo-remote-url', ), ))
-    @_action(PARENT_PRJ, *ANY_PRJ_TYPE, shortcut='fork')
-    def fork_project(self, ini_pdv: PdvType):
-        """ create/renew fork of a remote repo specified via the ``package`` option, into our user/group namespace. """
-        # group_name = _get_host_group(ini_pdv, domain)
-        # parent_path, _project_path, project_name = _get_path_package(ini_pdv)
-        # prj = self.connection.get_repo(fork_repo_remote_url)
-        # self.connection.get_user().create_fork(prj)
+    @_action(PARENT_PRJ, *ANY_PRJ_TYPE, arg_names=(('forked-user-slash-repo', ), ), shortcut='fork')
+    def fork_project(self, ini_pdv: PdvType, forked_usr_repo: str):
+        """ create/renew fork of a remote repo specified via the 1st argument, into our user/group namespace. """
+        domain = _get_host_domain(ini_pdv)
+        _chk_if(20, domain == 'github.com', f"invalid repo host domain '{domain}'! add option --domain=github.com")
+
+        prj = self.repo_obj(20, "repository {name} to fork not found", forked_usr_repo)
+        cast(AuthenticatedUser, self.connection.get_user()).create_fork(prj)
+
+        cae.po(f" ==== forked {pdv_str(ini_pdv, 'project_desc')} on {domain}")
+
+    @_action(arg_names=((), ('branch-name', ), ), shortcut='push')
+    def push_project(self, ini_pdv: PdvType, branch_name: str = ''):
+        """ push current/specified branch of project/package to remote host domain, version-tagged if release is True.
+
+        :param ini_pdv:             project dev vars.
+        :param branch_name:         optional branch name to push (alternatively specified by the ``branch`` command line
+                                    option).
+        """
+        group_name = _get_host_group(ini_pdv, _get_host_domain(ini_pdv))
+        project_name = _get_prj_name(ini_pdv)
+
+        changed = _git_uncommitted(ini_pdv)
+        _chk_if(76, not changed, f"{project_name} has {len(changed)} uncommitted files: {changed}")
+
+        new_repo = False
+        push_refs = []
+        if not self.repo_obj(0, "", f"{group_name}/{project_name}"):
+            usr_obj = cast(AuthenticatedUser, self.connection.get_user())
+            usr_obj.create_repo(project_name)   # if not then git push throws error "Repository not found"
+            new_repo = True
+            push_refs.append(MAIN_BRANCH)
+
+        branch_name = branch_name or _get_branch(ini_pdv)
+        if branch_name and branch_name not in push_refs:
+            push_refs.append(branch_name)
+
+        pkg_version = _git_project_version(ini_pdv, increment_part=cae.get_option('versionIncrementPart'))
+        file_version = pdv_str(ini_pdv, 'project_version')
+        _chk_if(77, pkg_version == file_version, f"version mismatch: local={file_version} remote={pkg_version}")
+        if Version(pkg_version) > Version(file_version):     # and cae.get_option('force')
+            replace_file_version(pdv_str(ini_pdv, 'version_file'), new_version=pkg_version)
+            _write_commit_message(ini_pdv, pkg_version=pkg_version,
+                                  title=f"late commit of forced push version correction {file_version}->{pkg_version}")
+            _git_add(ini_pdv)
+            _git_commit(ini_pdv)
+            ini_pdv['project_version'] = pkg_version
+        else:
+            pkg_version = file_version
+        tag = f"v{pkg_version}"
+        _git_tag_add(ini_pdv, tag)
+        push_refs.append(tag)
+
+        _git_push(ini_pdv, *push_refs, extra_args=("--set-upstream", ))
+
+        if new_repo:    # branch protection rules have to be created after branch creation done by git push
+            self.init_new_repo(f"{group_name}/{project_name}", pdv_str(ini_pdv, 'project_desc'))
+
+        cae.po(f" ==== pushed {' '.join(push_refs)} branches/tags to remote project {project_name}")
+
+    @_action(arg_names=(("version-tag", ), ('LATEST', )), shortcut='release')
+    def release_project(self, ini_pdv: PdvType, version_tag: str):
+        """ update local MAIN_BRANCH from origin and if pip_name is set then also release the latest/specified version.
+
+        :param ini_pdv:         project dev vars.
+        :param version_tag:     push version tag in the format ``v<version-number>`` to release or ``LATEST`` to use
+                                the version tag of the latest git repository version.
+        """
+        self._release_project(ini_pdv, version_tag)
+
+    @_action(shortcut='request')
+    def request_merge(self, ini_pdv: PdvType):
+        """ request merge of the origin=fork repository into the main branch at remote/upstream=forked. """
+        # see https://docs.github.com/de/rest/pulls/pulls?apiVersion=2022-11-28#create-a-pull-request
+        src_prj, tgt_prj, forked, branch = self._repo_merge_src_dst_fork_branch(ini_pdv)
+
+        commit_msg_title, commit_msg_body = read_file(_check_commit_msg_file(ini_pdv)).split(os.linesep, maxsplit=1)
+        merge_req = tgt_prj.create_pull(base=MAIN_BRANCH, head=branch, title=commit_msg_title, body=commit_msg_body)
+        if _debug_or_verbose():
+            diff_url = merge_req.diff_url
+            cae.po(f"    . merge request diffs available at: {diff_url}")
+
+        action = "requested merge"
+        if not forked:
+            _wait()  # wait for created un-forked/direct maintainer merge request (with --force --user=group_name)
+            tgt_prj.merge(base=MAIN_BRANCH, head=branch, commit_message=commit_msg_title + os.linesep + commit_msg_body)
+            action = "auto-merged un-forked and forced merge request"
+
+        cae.po(f" ==== {action} of branch {branch} from fork/origin ({src_prj.id}) into upstream ({tgt_prj.id})")
 
 
 class GitlabCom(RemoteHost):
     """ remote connection and actions on gitlab.com. """
     connection: Gitlab                  #: connection to Gitlab host
 
     def connect(self, ini_pdv: PdvType) -> bool:
@@ -2457,76 +2672,80 @@
                 self.connection.enable_debug()
             self.connection.auth()          # authenticate and create user attribute
         except (Exception, ) as ex:
             cae.po(f"****  Gitlab connection exception: {ex}")
             return False
         return True
 
-    def create_project(self, ini_pdv: PdvType):
+    def create_branch(self, group_repo: str, branch_name: str, tag_name: str):
+        """ create new remote branch onto/from tag name.
+
+        :param group_repo:      string with owner-user-name/repo-name of the repository, e.g. "UserName/RepositoryName".
+        :param branch_name:     name of the branch to create.
+        :param tag_name:        name of the tag/ref to create branch from.
+        """
+        cae.dpo(f"   -- creating branch '{branch_name}' for tag '{tag_name}' at remotes/origin")
+        prj = self.repo_obj(95, "group/project {name} not found", group_repo)
+        try:
+            prj.branches.create({'branch': branch_name, 'ref': tag_name})
+        except (GitlabHttpError, GitlabCreateError, GitlabError, Exception):
+            _exit_error(86, f"error '{format_exc()}' creating branch '{branch_name}' for tag '{tag_name}'")
+
+    def init_new_repo(self, ini_pdv: PdvType):
         """ create group/user project specified in ini_pdv or quit with error if group/user not found.
 
         :param ini_pdv:         project dev vars.
         """
         owner_obj = self.project_owner(ini_pdv)
         project_name = _get_prj_name(ini_pdv)
         project_properties = {
             'name': project_name,
             'description': pdv_str(ini_pdv, 'project_desc'),
             'default_branch': MAIN_BRANCH,
             'visibility': 'public',
         }
-        owner_projects: Union[ProjectManager, UserProjectManager]
         if isinstance(owner_obj, User):
             project_properties['user_id'] = owner_obj.id
-            owner_projects = owner_obj.projects
         else:
             project_properties['namespace_id'] = owner_obj.id
-            owner_projects = self.connection.projects
         cae.vpo(f"    - remote project properties of new package {project_name}: {PPF(project_properties)}")
 
-        project = cast(Project, owner_projects.create(project_properties))
+        # using UserProtectManager|owner_obj.projects.create() for user projects results in 403 Forbidden error
+        project = cast(Project, self.connection.projects.create(project_properties))
         cae.po(f"   == created new project for user/group '{owner_obj.name}'; attributes: {PPF(project.attributes)}")
 
         _wait()
 
         for branch_mask in (MAIN_BRANCH, 'release*'):
             protected_branch_properties = {'name': branch_mask,
                                            'merge_access_level': MAINTAINER_ACCESS,
                                            'push_access_level': MAINTAINER_ACCESS}
             cae.vpo(f"    - {branch_mask} protected branch properties: {protected_branch_properties}")
             project.protectedbranches.create(protected_branch_properties)
         cae.po(f"   == created 2 protected branches: '{MAIN_BRANCH}', 'release*'")
 
-    def project_from_name(self, err_code: int, err_msg: str, project_name: str, owned: bool = True) -> Project:
+    def repo_obj(self, err_code: int, err_msg: str, group_repo: str) -> Project:
         """ convert group/project_name or an endswith-fragment of it to a Project instance of the remote repo api.
 
         :param err_code:        error code, pass 0 to not quit if project not found.
         :param err_msg:         error message to display on error with optional {name} to be automatically substituted
-                                with the project name from the :paramref:`~project_from_name.project_name` argument.
-        :param project_name:    package-name, group/package-name or group/package-endswith-fragment to search for.
-        :param owned:           if True then the 2nd/fallback fragment/list search is limited to owned repos (quicker).
-                                pass False to search in all repos for the specified group/project-name fragment.
+                                with the project name from the :paramref:`~repo_obj.group_repo` argument.
+        :param group_repo:      group/project-name to search for.
         :return:                python-gitlab project instance if found, else return None if err_code is zero else quit.
         """
         try:
             # Projects.get() raises GitLabError (404 project not found) on an exact project name if there are other
             # project names starting with the same string. Projects.list() will then return the project as last item.
-            return self.connection.projects.get(project_name)
+            return self.connection.projects.get(group_repo)
         except GitlabError:     # e.g. GitlabGetError: 404: 404 Project Not Found
-            projects = cast(List[Project], self.connection.projects.list(search=project_name, owned=owned))
-
-        for prj in (projects or ()):
-            if prj.name.endswith(project_name):
-                return prj
-
-        if err_code:
-            _exit_error(err_code, err_msg.format(name=project_name))
-        elif _debug_or_verbose():
-            cae.po(f"   * project {project_name} not found on connected remote server")
-        return cast(Project, None)
+            if err_code:
+                _exit_error(err_code, err_msg.format(name=group_repo))
+            elif _debug_or_verbose():
+                cae.po(f"   * group/project {group_repo} not found on connected remote server")
+            return cast(Project, None)
 
     def project_owner(self, ini_pdv: PdvType) -> Union[Group, User]:
         """ determine owner (group|user) of the project specified by ini_pdv or quit with error if group/user not found.
 
         :param ini_pdv:         project dev vars.
         :return:                instance of Group or User, determined via the user-/group-names specified by ini_pdv.
         """
@@ -2562,15 +2781,15 @@
         """ delete local+remote release tags and branches of the specified project that got not published to PYPI. """
         pip_name = pdv_str(ini_pdv, 'pip_name')
         if not pip_name:
             cae.po(" ==== this project has no PyPi release tags/branches to clean")
             return []
 
         project_path = pdv_str(ini_pdv, 'project_path')
-        project_name = os.path.basename(project_path)
+        group_repo = f"{_get_host_group(ini_pdv, _get_host_domain(ini_pdv))}/{_get_prj_name(ini_pdv)}"
 
         all_branches = _git_branches(ini_pdv)
         cae.po(f"    - found {len(all_branches)} branches to check for to be deleted: {all_branches}")
 
         pypi_releases = pypi_versions(pip_name)
         _chk_if(34, bool(pypi_releases), "no PyPI releases found (check installation of pip)")
         cae.po(f"    - found {len(pypi_releases)} PyPI release versions protected from to be deleted: {pypi_releases}")
@@ -2578,16 +2797,16 @@
         deleted = []
         for branch_name in all_branches:
             chk, *ver = branch_name.split('release')
             if len(ver) != 1 or ver[0] in pypi_releases:
                 continue
             version = ver[0]
             if chk == 'remotes/origin/':        # un-deployed remote release branch found
-                # _git_push(ini_pdv, branch_name, extra_args=("--delete", )) protected release* branch raises error
-                project = self.project_from_name(33, "{name} not found at origin", project_name)
+                # _git_push(ini_pdv, branch_name, extra_args=("--delete", )) protected 'release*' branch raises error
+                project = self.repo_obj(33, "{name} not found at origin", group_repo)
                 try:
                     project.protectedbranches.delete(branch_name)
                 except GitlabError as ex:  # GitlabDeleteError on failed release upload
                     cae.po(f"    # try other method to delete protected branch {branch_name} on remote after err: {ex}")
                     try:
                         branch_obj = project.protectedbranches.get(branch_name)
                         branch_obj.delete()
@@ -2623,26 +2842,27 @@
         for chi_pdv in children_pdv:
             self.fork_project(chi_pdv)
         cae.po(f"===== forked {_children_desc(ini_pdv, children_pdv)}")
 
     @_action(PARENT_PRJ, *ANY_PRJ_TYPE, shortcut='fork')
     def fork_project(self, ini_pdv: PdvType):
         """ create/renew fork of a remote repo specified via the ``package`` option, into our user/group namespace. """
+        domain = _get_host_domain(ini_pdv)
+        _chk_if(20, domain == 'gitlab.com', f"invalid repo host domain '{domain}'! add option --domain=gitlab.com")
+
         if 'upstream' in _git_remotes(ini_pdv):    # renew origin from upstream if already forked
             with _in_prj_dir_venv(pdv_str(ini_pdv, 'project_path')):
                 _cl(20, f"git checkout {MAIN_BRANCH}")
                 _cl(20, "git fetch upstream")
                 _cl(20, f"git pull upstream {MAIN_BRANCH}")
                 _cl(20, f"git push origin {MAIN_BRANCH}")
         else:
-            domain = _get_host_domain(ini_pdv)
             group_name = _get_host_group(ini_pdv, domain)
             parent_path, _project_path, project_name = _get_path_package(ini_pdv)
-            prj_instance = self.project_from_name(20, "project {name} not found on remote",
-                                                  f"{group_name}/{project_name}")
+            prj_instance = self.repo_obj(20, "project {name} not found on remote", f"{group_name}/{project_name}")
 
             prj_instance.forks.create({})        # {'namespace': usr_name}
 
             usr_name = self.connection.user.name                # type: ignore # silly mypy
             host_url = f"{pdv_str(ini_pdv, 'REPO_HOST_PROTOCOL')}{domain}"
             with _in_prj_dir_venv(parent_path):
                 _cl(21, "git clone", extra_args=(f"{host_url}/{usr_name}/{project_name}.git", ))
@@ -2665,22 +2885,22 @@
     def push_project(self, ini_pdv: PdvType, branch_name: str = ''):
         """ push current/specified branch of project/package to remote host domain, version-tagged if release is True.
 
         :param ini_pdv:             project dev vars.
         :param branch_name:         optional branch name to push (alternatively specified by the ``branch`` command line
                                     option).
         """
-        project_name = _get_prj_name(ini_pdv)
+        group_repo = f"{_get_host_group(ini_pdv, _get_host_domain(ini_pdv))}/{_get_prj_name(ini_pdv)}"
 
         changed = _git_uncommitted(ini_pdv)
-        _chk_if(76, not changed, f"{project_name} has {len(changed)} uncommitted files: {changed}")
+        _chk_if(76, not changed, f"{group_repo} has {len(changed)} uncommitted files: {changed}")
 
         push_refs = []
-        if not self.project_from_name(0, "", project_name):
-            self.create_project(ini_pdv)
+        if not self.repo_obj(0, "", group_repo):
+            self.init_new_repo(ini_pdv)
             push_refs.append(MAIN_BRANCH)
 
         branch_name = branch_name or _get_branch(ini_pdv)
         if branch_name and branch_name not in push_refs:
             push_refs.append(branch_name)
 
         pkg_version = _git_project_version(ini_pdv, increment_part=cae.get_option('versionIncrementPart'))
@@ -2697,15 +2917,15 @@
             pkg_version = file_version
         tag = f"v{pkg_version}"
         _git_tag_add(ini_pdv, tag)
         push_refs.append(tag)
 
         _git_push(ini_pdv, *push_refs, extra_args=("--set-upstream", ))
 
-        cae.po(f" ==== pushed {' '.join(push_refs)} branches/tags to remote project {project_name}")
+        cae.po(f" ==== pushed {' '.join(push_refs)} branches/tags to remote project {group_repo}")
 
     @_action(PARENT_PRJ, ROOT_PRJ, shortcut='release')
     def release_children(self, ini_pdv: PdvType, *children_pdv: PdvType):
         """ release the latest versions of the specified parent/root children projects to remotes/origin. """
         for chi_pdv in children_pdv:
             cae.po(f" ---  {pdv_str(chi_pdv, 'project_name')}  ---  {pdv_str(chi_pdv, 'project_desc')}")
             self.release_project(chi_pdv, 'LATEST')
@@ -2717,101 +2937,56 @@
     def release_project(self, ini_pdv: PdvType, version_tag: str):
         """ update local MAIN_BRANCH from origin and if pip_name is set then also release the latest/specified version.
 
         :param ini_pdv:         project dev vars.
         :param version_tag:     push version tag in the format ``v<version-number>`` to release or ``LATEST`` to use
                                 the version tag of the latest git repository version.
         """
-        errors = _git_fetch(ini_pdv)
-        _chk_if(84, not bool(errors), f"git fetch errors:{_pp(errors)}" + _hint(
-            self.release_project, " later to retry if server is currently unavailable, or check remote configuration"))
-
-        # switch back to local MAIN_BRANCH and then merge-in the release-branch&-tag from remotes/origin/MAIN_BRANCH
-        _git_checkout(ini_pdv, branch=MAIN_BRANCH)
-        _git_merge(ini_pdv, f"origin/{MAIN_BRANCH}")
-
-        if version_tag == 'LATEST':
-            pkg_version = _git_project_version(ini_pdv, increment_part=0)
-            version_tag = f"v{pkg_version}"
-        else:
-            _chk_if(85, version_tag[0] == "v" and version_tag.count(".") == 2, f"version '{version_tag}' format error")
-            pkg_version = version_tag[1:]
-        _chk_if(85, _git_tag_in_branch(ini_pdv, version_tag),
-                f"push version tag {version_tag} has first to be merged into origin/{MAIN_BRANCH}" + _hint(
-                    self.request_merge, " to request to merge your branch."))
-
-        msg = f"updated local {MAIN_BRANCH} branch"
-        if pdv_str(ini_pdv, 'pip_name'):    # create release*ver branch only for projects available in PyPi via pip
-            release_branch = f"release{pkg_version}"
-            _chk_if(85, not _git_tag_in_branch(ini_pdv, release_branch),
-                    f"release branch {release_branch} already exists in origin/{MAIN_BRANCH}")
-
-            prj = self.project_from_name(95, "project {name} not found", pdv_str(ini_pdv, 'project_name'))
-            cae.dpo(f"   -- creating branch '{release_branch}' for tag '{version_tag}' at remotes/origin")
-            try:
-                prj.branches.create({'branch': release_branch, 'ref': version_tag})
-            except (GitlabHttpError, GitlabCreateError, GitlabError, Exception):
-                _exit_error(86, f"error '{format_exc()}' creating branch '{release_branch}' for tag '{version_tag}'")
-            msg += f" and released {pkg_version}"
-
-        cae.po(f" ==== {msg} of {pdv_str(ini_pdv, 'project_desc')}")
+        self._release_project(ini_pdv, version_tag)
 
     @_action(PARENT_PRJ, ROOT_PRJ, shortcut='request')
     def request_children_merge(self, ini_pdv: PdvType, *children_pdv: PdvType):
         """ request the merge of the specified children of a parent/namespace on remote/upstream. """
         for chi_pdv in children_pdv:
             cae.po(f" ---  {pdv_str(chi_pdv, 'project_name')}  ---  {pdv_str(chi_pdv, 'project_desc')}")
             self.request_merge(chi_pdv)
             if chi_pdv != children_pdv[-1]:
                 _wait()
         cae.po(f"===== requested merge of {_children_desc(ini_pdv, children_pdv)}")
 
     @_action(shortcut='request')
     def request_merge(self, ini_pdv: PdvType):
         """ request merge of the origin=fork repository into the main branch at remote/upstream=forked. """
-        branch = _get_branch(ini_pdv)
-        domain = _get_host_domain(ini_pdv)
-        group_name = _get_host_group(ini_pdv, domain)
-        user_name = _get_host_user_name(ini_pdv, domain)
-        project_name = _get_prj_name(ini_pdv)
-
-        remotes = _git_remotes(ini_pdv)
-        origin_user = remotes.get('origin', "/").split('/')[-2]
-        _chk_if(64, origin_user == user_name, f"user mismatch specified={user_name} != origin={origin_user}")
-        upstream_group = remotes.get('upstream', "/").split('/')[-2]
-        _chk_if(65, upstream_group == group_name, f"group mismatch spe={group_name} != upstream={upstream_group}")
-
         # https://docs.gitlab.com/ee/api/merge_requests.html#create-mr and https://stackoverflow.com/questions/51104622
-        # target_project_id/project_id is the upstream and source_project_id is the origin/fork
-        src_prj = self.project_from_name(65, "origin/fork repository {name} not found on remote server",
-                                         f"{user_name}/{project_name}")
-        tgt_prj = self.project_from_name(66, "target/upstream/forked repository {name} not found on remote",
-                                         f"{group_name}/{project_name}")
-
-        commit_msg_file = _check_commit_msg_file(ini_pdv)
+        src_prj, tgt_prj, forked, branch = self._repo_merge_src_dst_fork_branch(ini_pdv)
+        if TYPE_CHECKING:
+            assert isinstance(src_prj, Project)
+            assert isinstance(tgt_prj, Project)
+        commit_msg = read_file(_check_commit_msg_file(ini_pdv))
         merge_req = tgt_prj.mergerequests.create({
             'project_id': tgt_prj.id,
             'source_project_id': src_prj.id,
             'source_branch': branch,
             'target_project_id': tgt_prj.id,
             'target_branch': MAIN_BRANCH,
-            'title': read_file(commit_msg_file).split(os.linesep)[0],
+            'title': commit_msg.split(os.linesep)[0],
             # 'remove_source_branch': False,
             # 'force_remove_source_branch': False,
             # 'allow_collaboration': True,
             # 'subscribed': True,
         })
         if _debug_or_verbose():
             cae.po(f"    . merge request diffs: {PPF([_.attributes for _ in merge_req.diffs.list()])}")
 
         action = "requested merge"
-        if cae.get_option('force') and user_name == group_name:
+        if not forked:
             _wait()  # wait for created un-forked/direct maintainer merge request (with --force --user=group_name)
-            merge_req.merge(merge_commit_message=read_file(_check_commit_msg_file(ini_pdv)))
+            merge_req.merge(merge_commit_message=commit_msg)
             action = "auto-merged un-forked and forced merge request"
+
         cae.po(f" ==== {action} of branch {branch} from fork/origin ({src_prj.id}) into upstream ({tgt_prj.id})")
 
     @_action(arg_names=((), ('fragment', ), ))
     def search_repos(self, ini_pdv: PdvType, fragment: str = ""):
         """ search remote repositories via a text fragment in its project name/description. """
         fragment = fragment or _get_prj_name(ini_pdv)
         repos = self.connection.projects.list(search=fragment, get_all=True)
@@ -2826,26 +3001,26 @@
         for chi_pdv in children_pdv:
             self.show_repo(chi_pdv)
         cae.po(f"===== dumped info of {_children_desc(ini_pdv, children_pdv)}")
 
     @_action()
     def show_repo(self, ini_pdv: PdvType):
         """ display properties of remote repository. """
-        group_project = f"{_get_host_group(ini_pdv, _get_host_domain(ini_pdv))}/{_get_prj_name(ini_pdv)}"
-        repo_api = self.project_from_name(0, "", group_project)
+        group_repo = f"{_get_host_group(ini_pdv, _get_host_domain(ini_pdv))}/{_get_prj_name(ini_pdv)}"
+        repo_api = self.repo_obj(0, "", group_repo)
         if isinstance(repo_api, Project):
-            cae.po(f"   -- {group_project} remote repository attributes:")
+            cae.po(f"   -- {group_repo} remote repository attributes:")
             for attr in sorted(repo_api.attributes) if _debug_or_verbose() else \
                     ('created_at', 'default_branch', 'description', 'id', 'path_with_namespace', 'visibility'):
                 cae.po(f"    - {attr} = {getattr(repo_api, attr, None)}")
 
             cae.po(f"   -- protected branches = {PPF(repo_api.protectedbranches.list())}")
             cae.po(f"   -- protected tags = {PPF(repo_api.protectedtags.list())}")
         else:
-            cae.po(f"    * project {group_project} not found on remote server")
+            cae.po(f"    * project {group_repo} not found on remote server")
         cae.po(f" ==== dumped repo info of {pdv_str(ini_pdv, 'project_desc')}")
 
 
 class PythonanywhereCom(RemoteHost):
     """ remote actions on remote web host pythonanywhere.com (to be specified by --domain option). """
     connection: PythonanywhereApi               #: requests http connection
     name_prefix: str = 'web'                    #: config variable name prefix
```

### Comparing `aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/PKG-INFO` & `aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.78
+Version: 0.3.79
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -72,25 +72,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.78
+# git_repo_manager 0.3.79
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.77?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.77)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.78?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.78)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.78.
+>aedev_git_repo_manager package 0.3.79.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.78/aedev_git_repo_manager.egg-info/requires.txt` & `aedev_git_repo_manager-0.3.79/aedev_git_repo_manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.78/setup.py` & `aedev_git_repo_manager-0.3.79/setup.py`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.78/tests/test_git_repo_manager.py` & `aedev_git_repo_manager-0.3.79/tests/test_git_repo_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,16 +225,17 @@
     assert TPL_PACKAGES
     assert len(tst_namespaces_roots) + len(TPL_PACKAGES) == len(REGISTERED_TPL_PROJECTS)
 
 
 @skip_gitlab_ci  # skip on gitlab because of missing remote repository user account token
 class TestGitlabActions:
     def test_clean_releases(self, gitlab_remote, mocked_app_options, module_repo_path):
-        mocked_app_options['token'] = cae.get_variable('token')
+        mocked_app_options['domain'] = 'gitlab.com'
         mocked_app_options['path'] = module_repo_path
+        mocked_app_options['token'] = cae.get_variable('token')
         mocked_app_options['verbose'] = True
         gitlab_remote.clean_releases(project_dev_vars(project_path=module_repo_path))
 
     def test_show_repo(self, capsys, gitlab_remote, mocked_app_options):
         mocked_app_options['domain'] = None
         gitlab_remote.show_repo(project_dev_vars())
         output = capsys.readouterr().out
```

