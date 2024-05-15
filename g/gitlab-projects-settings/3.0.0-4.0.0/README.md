# Comparing `tmp/gitlab_projects_settings-3.0.0.tar.gz` & `tmp/gitlab_projects_settings-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_settings-3.0.0.tar", last modified: Mon May  6 01:25:25 2024, max compression
+gzip compressed data, was "gitlab_projects_settings-4.0.0.tar", last modified: Wed May 15 00:04:27 2024, max compression
```

## Comparing `gitlab_projects_settings-3.0.0.tar` & `gitlab_projects_settings-4.0.0.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.491876 gitlab_projects_settings-3.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.484876 gitlab_projects_settings-3.0.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     7147 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.484876 gitlab_projects_settings-3.0.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     3518 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5642 2024-05-06 01:25:25.491876 gitlab_projects_settings-3.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4033 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.491876 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5642 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      946 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.487877 gitlab_projects_settings-3.0.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 01:25:25.491876 gitlab_projects_settings-3.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.487877 gitlab_projects_settings-3.0.0/src/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.488876 gitlab_projects_settings-3.0.0/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14204 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     6683 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.488876 gitlab_projects_settings-3.0.0/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14867 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.489876 gitlab_projects_settings-3.0.0/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.489876 gitlab_projects_settings-3.0.0/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.490877 gitlab_projects_settings-3.0.0/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.490877 gitlab_projects_settings-3.0.0/src/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/types/namespaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.672427 gitlab_projects_settings-4.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.661428 gitlab_projects_settings-4.0.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11981 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.662428 gitlab_projects_settings-4.0.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     5064 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7311 2024-05-15 00:04:27.671427 gitlab_projects_settings-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5664 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.671427 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7311 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.665428 gitlab_projects_settings-4.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 00:04:27.672427 gitlab_projects_settings-4.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.665428 gitlab_projects_settings-4.0.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.666427 gitlab_projects_settings-4.0.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16950 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     8980 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.667427 gitlab_projects_settings-4.0.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14733 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.668428 gitlab_projects_settings-4.0.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.669427 gitlab_projects_settings-4.0.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/prints/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.669427 gitlab_projects_settings-4.0.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.670427 gitlab_projects_settings-4.0.0/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11270 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/types/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/types/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/types/strings.py
```

### Comparing `gitlab_projects_settings-3.0.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_settings-4.0.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/.chglog/changelog.sh` & `gitlab_projects_settings-4.0.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/.chglog/config.yml` & `gitlab_projects_settings-4.0.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/.style.yapf` & `gitlab_projects_settings-4.0.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/.vscode/extensions.json` & `gitlab_projects_settings-4.0.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/.vscode/settings.json` & `gitlab_projects_settings-4.0.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/CHANGELOG.md` & `gitlab_projects_settings-4.0.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,51 @@
 
+<a name="4.0.0"></a>
+## [4.0.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/3.0.0...4.0.0) (2024-05-15)
+
+### Bug Fixes
+
+* **entrypoint:** refactor to return no error upon final actions
+* **entrypoint:** avoid missing 'namespace_id' in 'User' responses
+* **entrypoint:** use full paths instead of 'id' integer fields
+* **gitlab:** disable all 'Repository' member features too
+* **gitlab:** disable 'Repository' group feature after its members
+* **gitlab:** accept deletion denials in 'project_reset_members'
+
+### Ci
+
+* **gitlab-ci:** support multiple 'METAVAR' words in 'readme' job
+* **gitlab-ci:** deprecate requirements install in 'lint' job
+* **gitlab-ci:** implement 'images' and use project specific images
+* **gitlab-ci:** detect 'README.md' issues in 'readme' job
+* **gitlab-ci:** handle optional parameters and multiline in 'readme'
+
+### Cleanups
+
+* **entrypoint:** minor Python codestyle improvement
+
+### Code Refactoring
+
+* **gitlab:** optimize and centralize GitLab features handlings
+* **gitlab:** isolate GitLab types to 'types/gitlab.py'
+* **gitlab:** isolate 'GitLabFeature.AccessLevels' constants
+
+### Features
+
+* **gitlab:** parse input features list and accept similar texts
+* **gitlab:** prepare future access levels in 'project_reset_features'
+* **gitlab:** isolate GitLab project features enumeration
+* **gitlab:** automatically wait for group and project deletions
+* **main:** document optional '--' positional arguments separator
+
+### Test
+
+* **version:** add 'DEBUG_VERSION_FAKE' for debugging purposes
+
+
 <a name="3.0.0"></a>
 ## [3.0.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/2.1.0...3.0.0) (2024-05-06)
 
 ### Bug Fixes
 
 * **entrypoint:** resolve support for private user namespaces
 * **entrypoint:** detect if GitLab actions can continue
```

### Comparing `gitlab_projects_settings-3.0.0/LICENSE` & `gitlab_projects_settings-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/PKG-INFO` & `gitlab_projects_settings-4.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: gitlab-projects-settings
-Version: 3.0.0
-Summary: Configure GitLab groups and projects settings automatically
-Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
-Author: Adrian DC
-Author-email: radian.dc@gmail.com
-License: Apache License 2.0
-Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
-Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
-Project-URL: Documentation, https://gitlab.com/AdrianDC/gitlab-projects-settings#gitlab-projects-settings
-Project-URL: Source, https://gitlab.com/AdrianDC/gitlab-projects-settings
-Project-URL: Statistics, https://pypistats.org/packages/gitlab-projects-settings
-Keywords: gitlab issues sync
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
-Requires-Python: >=3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: colored>=1.4.2
-Requires-Dist: python-gitlab>=4.4.0
-Requires-Dist: setuptools>=45.1.0
-
 # gitlab-projects-settings
 
 <!-- markdownlint-disable no-inline-html -->
 
 [![Build](https://gitlab.com/AdrianDC/gitlab-projects-settings/badges/main/pipeline.svg)](https://gitlab.com/AdrianDC/gitlab-projects-settings/-/commits/main/)
 
 Configure GitLab groups and projects settings automatically
@@ -58,69 +24,95 @@
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group] [--exclude-subgroups]
-                                [--exclude-projects] [--reset-features] [--reset-members] [--set-avatar FILE]
-                                [--set-description TEXT] [--update-description] [--run-housekeeping]
-                                [--archive-project | --unarchive-project] [--delete-group] [--delete-project]
-                                [--protect-branches] [--protect-tags LEVEL]
+usage: gitlab-projects-settings [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-t TOKEN]
+                                [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
+                                [--available-features] [--reset-features [KEEP_FEATURES]]
+                                [--disable-features FEATURES] [--enable-features FEATURES] [--reset-members]
+                                [--set-avatar FILE] [--set-description TEXT] [--update-description]
+                                [--run-housekeeping] [--archive-project | --unarchive-project] [--delete-group]
+                                [--delete-project] [--protect-branches] [--protect-tags LEVEL] [--]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
-  -h, --help              # Show this help message
-  --version               # Show the current version
+  -h, --help                        # Show this help message
+  --version                         # Show the current version
+  --update-check                    # Check for newer package updates
+  --settings                        # Show the current settings path and contents
+  --set GROUP KEY VAL               # Set settings specific 'VAL' value to [GROUP] > KEY
+                                    # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
-  -t TOKEN                # GitLab API token (default: GITLAB_TOKEN environment)
+  -t TOKEN                          # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
-  --dry-run               # Enable dry run mode to check without saving
-  --exclude-group         # Exclude parent group settings
-  --exclude-subgroups     # Exclude children subgroups settings
-  --exclude-projects      # Exclude children projects settings
+  --dry-run                         # Enable dry run mode to check without saving
+  --exclude-group                   # Exclude parent group settings
+  --exclude-subgroups               # Exclude children subgroups settings
+  --exclude-projects                # Exclude children projects settings
 
 general settings arguments:
-  --reset-features        # Reset features of GitLab projects based on usage
-  --reset-members         # Reset members of GitLab projects and groups
-  --set-avatar FILE       # Set avatar of GitLab projects and groups
-  --set-description TEXT  # Set description of GitLab projects and groups
-  --update-description    # Update description of GitLab projects and groups automatically
+  --available-features              # List the available GitLab project features known by the tool
+  --reset-features [KEEP_FEATURES]  # Reset features of GitLab projects based on usage
+                                    # (Optionally keep features separated by ",")
+  --disable-features FEATURES       # List of features to disable separated by ","
+  --enable-features FEATURES        # List of features to enable separated by ","
+  --reset-members                   # Reset members of GitLab projects and groups
+  --set-avatar FILE                 # Set avatar of GitLab projects and groups
+  --set-description TEXT            # Set description of GitLab projects and groups
+  --update-description              # Update description of GitLab projects and groups automatically
 
 advanced settings arguments:
-  --run-housekeeping      # Run housekeeping of project or projects GitLab in groups
-  --archive-project       # Archive project or projects in GitLab groups
-  --unarchive-project     # Unarchive project or projects in GitLab groups
-  --delete-group          # Delete group or groups in GitLab groups
-  --delete-project        # Delete project or projects in GitLab groups
+  --run-housekeeping                # Run housekeeping of project or projects GitLab in groups
+  --archive-project                 # Archive project or projects in GitLab groups
+  --unarchive-project               # Unarchive project or projects in GitLab groups
+  --delete-group                    # Delete group or groups in GitLab groups
+  --delete-project                  # Delete project or projects in GitLab groups
 
 repository settings arguments:
-  --protect-branches      # Protect branches with default master/main, develop and staging
-  --protect-tags LEVEL    # Protect tags at level [no-one,admins,maintainers,developers]
+  --protect-branches                # Protect branches with default master/main, develop and staging
+  --protect-tags LEVEL              # Protect tags at level [no-one,admins,maintainers,developers]
 
 positional arguments:
-  gitlab                  # GitLab URL (default: https://gitlab.com)
-  path                    # GitLab group, user namespace or project path
+  --                                # Positional arguments separator (recommended)
+  gitlab                            # GitLab URL (default: https://gitlab.com)
+  path                              # GitLab group, user namespace or project path
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
+## Userspace available settings
+
+`gitlab-projects-settings` creates a `settings.ini` configuration file in a userspace folder.
+
+For example, it allows to disable the automated updates daily check (`[updates] > enabled`)
+
+The `settings.ini` file location and contents can be shown with the following command:
+
+```bash
+gitlab-projects-settings --settings
+```
+
+---
+
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
 - [python-gitlab](https://pypi.org/project/python-gitlab/): A python wrapper for the GitLab API
 - [setuptools](https://pypi.org/project/setuptools/): Build and manage Python packages
+- [update-checker](https://pypi.org/project/update-checker/): Check for package updates on PyPI
 
 ---
 
 ## References
 
 - [git-chglog](https://github.com/git-chglog/git-chglog): CHANGELOG generator
 - [gitlab-release](https://pypi.org/project/gitlab-release/): Utility for publishing on GitLab
```

### Comparing `gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/PKG-INFO` & `gitlab_projects_settings-4.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 3.0.0
+Version: 4.0.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -27,14 +27,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colored>=1.4.2
 Requires-Dist: python-gitlab>=4.4.0
 Requires-Dist: setuptools>=45.1.0
+Requires-Dist: update_checker>=0.18.0
 
 # gitlab-projects-settings
 
 <!-- markdownlint-disable no-inline-html -->
 
 [![Build](https://gitlab.com/AdrianDC/gitlab-projects-settings/badges/main/pipeline.svg)](https://gitlab.com/AdrianDC/gitlab-projects-settings/-/commits/main/)
 
@@ -58,69 +59,95 @@
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group] [--exclude-subgroups]
-                                [--exclude-projects] [--reset-features] [--reset-members] [--set-avatar FILE]
-                                [--set-description TEXT] [--update-description] [--run-housekeeping]
-                                [--archive-project | --unarchive-project] [--delete-group] [--delete-project]
-                                [--protect-branches] [--protect-tags LEVEL]
+usage: gitlab-projects-settings [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-t TOKEN]
+                                [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
+                                [--available-features] [--reset-features [KEEP_FEATURES]]
+                                [--disable-features FEATURES] [--enable-features FEATURES] [--reset-members]
+                                [--set-avatar FILE] [--set-description TEXT] [--update-description]
+                                [--run-housekeeping] [--archive-project | --unarchive-project] [--delete-group]
+                                [--delete-project] [--protect-branches] [--protect-tags LEVEL] [--]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
-  -h, --help              # Show this help message
-  --version               # Show the current version
+  -h, --help                        # Show this help message
+  --version                         # Show the current version
+  --update-check                    # Check for newer package updates
+  --settings                        # Show the current settings path and contents
+  --set GROUP KEY VAL               # Set settings specific 'VAL' value to [GROUP] > KEY
+                                    # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
-  -t TOKEN                # GitLab API token (default: GITLAB_TOKEN environment)
+  -t TOKEN                          # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
-  --dry-run               # Enable dry run mode to check without saving
-  --exclude-group         # Exclude parent group settings
-  --exclude-subgroups     # Exclude children subgroups settings
-  --exclude-projects      # Exclude children projects settings
+  --dry-run                         # Enable dry run mode to check without saving
+  --exclude-group                   # Exclude parent group settings
+  --exclude-subgroups               # Exclude children subgroups settings
+  --exclude-projects                # Exclude children projects settings
 
 general settings arguments:
-  --reset-features        # Reset features of GitLab projects based on usage
-  --reset-members         # Reset members of GitLab projects and groups
-  --set-avatar FILE       # Set avatar of GitLab projects and groups
-  --set-description TEXT  # Set description of GitLab projects and groups
-  --update-description    # Update description of GitLab projects and groups automatically
+  --available-features              # List the available GitLab project features known by the tool
+  --reset-features [KEEP_FEATURES]  # Reset features of GitLab projects based on usage
+                                    # (Optionally keep features separated by ",")
+  --disable-features FEATURES       # List of features to disable separated by ","
+  --enable-features FEATURES        # List of features to enable separated by ","
+  --reset-members                   # Reset members of GitLab projects and groups
+  --set-avatar FILE                 # Set avatar of GitLab projects and groups
+  --set-description TEXT            # Set description of GitLab projects and groups
+  --update-description              # Update description of GitLab projects and groups automatically
 
 advanced settings arguments:
-  --run-housekeeping      # Run housekeeping of project or projects GitLab in groups
-  --archive-project       # Archive project or projects in GitLab groups
-  --unarchive-project     # Unarchive project or projects in GitLab groups
-  --delete-group          # Delete group or groups in GitLab groups
-  --delete-project        # Delete project or projects in GitLab groups
+  --run-housekeeping                # Run housekeeping of project or projects GitLab in groups
+  --archive-project                 # Archive project or projects in GitLab groups
+  --unarchive-project               # Unarchive project or projects in GitLab groups
+  --delete-group                    # Delete group or groups in GitLab groups
+  --delete-project                  # Delete project or projects in GitLab groups
 
 repository settings arguments:
-  --protect-branches      # Protect branches with default master/main, develop and staging
-  --protect-tags LEVEL    # Protect tags at level [no-one,admins,maintainers,developers]
+  --protect-branches                # Protect branches with default master/main, develop and staging
+  --protect-tags LEVEL              # Protect tags at level [no-one,admins,maintainers,developers]
 
 positional arguments:
-  gitlab                  # GitLab URL (default: https://gitlab.com)
-  path                    # GitLab group, user namespace or project path
+  --                                # Positional arguments separator (recommended)
+  gitlab                            # GitLab URL (default: https://gitlab.com)
+  path                              # GitLab group, user namespace or project path
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
+## Userspace available settings
+
+`gitlab-projects-settings` creates a `settings.ini` configuration file in a userspace folder.
+
+For example, it allows to disable the automated updates daily check (`[updates] > enabled`)
+
+The `settings.ini` file location and contents can be shown with the following command:
+
+```bash
+gitlab-projects-settings --settings
+```
+
+---
+
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
 - [python-gitlab](https://pypi.org/project/python-gitlab/): A python wrapper for the GitLab API
 - [setuptools](https://pypi.org/project/setuptools/): Build and manage Python packages
+- [update-checker](https://pypi.org/project/update-checker/): Check for package updates on PyPI
 
 ---
 
 ## References
 
 - [git-chglog](https://github.com/git-chglog/git-chglog): CHANGELOG generator
 - [gitlab-release](https://pypi.org/project/gitlab-release/): Utility for publishing on GitLab
```

### Comparing `gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/SOURCES.txt` & `gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 src/cli/__init__.py
 src/cli/entrypoint.py
 src/cli/main.py
 src/features/__init__.py
 src/features/gitlab.py
 src/package/__init__.py
 src/package/bundle.py
+src/package/settings.py
+src/package/updates.py
 src/package/version.py
 src/prints/__init__.py
+src/prints/boxes.py
 src/prints/colors.py
 src/system/__init__.py
 src/system/platform.py
 src/types/__init__.py
-src/types/namespaces.py
+src/types/gitlab.py
+src/types/namespaces.py
+src/types/strings.py
```

### Comparing `gitlab_projects_settings-3.0.0/setup.py` & `gitlab_projects_settings-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/src/cli/entrypoint.py` & `gitlab_projects_settings-4.0.0/src/cli/entrypoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 #!/usr/bin/env python3
 
 # Standard libraries
 from argparse import Namespace
+from enum import Enum
+from typing import Optional
 
 # Modules libraries
 from gitlab.exceptions import GitlabGetError
-from gitlab.v4.objects import Group as GitLabGroup, Project as GitLabProject, User as GitLabUser
+from gitlab.v4.objects import (
+    Group as GitLabGroup,
+    Project as GitLabProject,
+    User as GitLabUser,
+)
 
 # Components
 from ..features.gitlab import GitLabFeature
 from ..prints.colors import Colors
 from ..system.platform import Platform
 from ..types.namespaces import Namespaces
 
 # Entrypoint class, pylint: disable=too-few-public-methods
 class Entrypoint:
 
+    # Enumerations
+    Result = Enum('Result', ['SUCCESS', 'FINALIZE', 'ERROR'])
+
     # CLI, pylint: disable=too-many-branches
     @staticmethod
-    def cli(options: Namespace) -> bool:
+    def cli(options: Namespace) -> Result:
 
         # Variables
-        group: GitLabGroup = None
-        project: GitLabProject = None
-        user: GitLabUser = None
+        group: Optional[GitLabGroup] = None
+        project: Optional[GitLabProject] = None
+        result: Entrypoint.Result = Entrypoint.Result.ERROR
+        user: Optional[GitLabUser] = None
 
         # Header
         print(' ')
 
         # GitLab client
         gitlab = GitLabFeature(
             options.gitlab,
@@ -49,15 +59,15 @@
             print(' ')
             Platform.flush()
         except GitlabGetError as exception:
             try:
                 if '/' in options.path:
                     raise TypeError from exception
                 user = gitlab.user(options.path)
-                namespace = gitlab.namespace(user.namespace_id)
+                namespace = gitlab.namespace(options.path)
                 print(f'{Colors.BOLD} - GitLab user namespace: '
                       f'{Colors.GREEN}{namespace.full_path}'
                       f'{Colors.CYAN} ({namespace.name})'
                       f'{Colors.RESET}')
                 print(' ')
                 Platform.flush()
             except (GitlabGetError, TypeError):
@@ -65,108 +75,122 @@
                 print(f'{Colors.BOLD} - GitLab project: '
                       f'{Colors.GREEN}{project.path_with_namespace}'
                       f'{Colors.CYAN} ({project.description})'
                       f'{Colors.RESET}')
                 print(' ')
                 Platform.flush()
 
+        # Handle available features
+        if options.available_features:
+            print(f'{Colors.BOLD} - GitLab project:'
+                  f'{Colors.RESET}')
+            print(f'{Colors.BOLD}   - Available features: '
+                  f'{Colors.CYAN}{", ".join(GitLabFeature.project_features_available())}'
+                  f'{Colors.RESET}')
+            Platform.flush()
+            return Entrypoint.Result.FINALIZE
+
         # Handle single project
         if project:
             Entrypoint.project(
                 options,
                 gitlab,
-                project.id,
+                project.path_with_namespace,
             )
 
         # Handle group recursively
         elif group:
 
             # Handle group
             if not options.exclude_group:
-                if not Entrypoint.group(
-                        options,
-                        gitlab,
-                        group.id,
-                ):
-                    return False
+                result = Entrypoint.group(
+                    options,
+                    gitlab,
+                    group.full_path,
+                )
+                if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
+                    return result
 
             # Iterate through subgroups
             if not options.exclude_subgroups:
                 for group_subgroup in sorted(
                         group.descendant_groups.list(
                             get_all=True,
                             include_subgroups=True,
                             order_by='path',
                             sort='asc',
                         ),
                         key=lambda item: item.full_path,
                 ):
-                    if not Entrypoint.group(
-                            options,
-                            gitlab,
-                            group_subgroup.id,
-                            True,
-                    ):
-                        return False
+                    result = Entrypoint.group(
+                        options,
+                        gitlab,
+                        group_subgroup.full_path,
+                        True,
+                    )
+                    if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
+                        return result
 
             # Iterate through projects
             if not options.exclude_projects:
                 for group_project in sorted(
                         group.projects.list(
                             get_all=True,
                             include_subgroups=not options.exclude_subgroups,
                             order_by='path',
                             sort='asc',
                         ),
                         key=lambda item: item.path_with_namespace,
                 ):
-                    if not Entrypoint.project(
-                            options,
-                            gitlab,
-                            group_project.id,
-                    ):
-                        return False
+                    result = Entrypoint.project(
+                        options,
+                        gitlab,
+                        group_project.path_with_namespace,
+                    )
+                    if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
+                        return result
 
         # Handle user recursively
         elif user:
 
             # Iterate through projects
             if not options.exclude_projects:
                 for user_project in sorted(
                         user.projects.list(
                             get_all=True,
                             order_by='path',
                             sort='asc',
                         ),
                         key=lambda item: item.path_with_namespace,
                 ):
-                    if not Entrypoint.project(
-                            options,
-                            gitlab,
-                            user_project.id,
-                    ):
-                        return False
+                    result = Entrypoint.project(
+                        options,
+                        gitlab,
+                        user_project.path_with_namespace,
+                    )
+                    if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
+                        return result
 
         # Result
-        return True
+        return Entrypoint.Result.SUCCESS
 
     # Group
     @staticmethod
     def group(
         options: Namespace,
         gitlab: GitLabFeature,
         criteria: str,
         subgroup: bool = False,
-    ) -> bool:
+    ) -> Result:
 
         # Acquire group
         group = gitlab.group(criteria)
 
         # Acquire parent group
-        parent_group: GitLabGroup = None
+        parent_group: Optional[GitLabGroup] = None
         if group.parent_id:
             parent_group = gitlab.group(group.parent_id)
 
         # Get parent description
         parent_description: str = ''
         parent_name: str = ''
         if parent_group:
@@ -185,15 +209,15 @@
         if options.delete_group:
             gitlab.group_delete(criteria)
             print(f'{Colors.BOLD}   - Delete {group_type}: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
-            return subgroup
+            return Entrypoint.Result.SUCCESS if subgroup else Entrypoint.Result.FINALIZE
 
         # Set group description
         if options.set_description:
             gitlab.group_set_description(criteria, options.set_description)
             print(f'{Colors.BOLD}   - Set description: '
                   f'{Colors.CYAN}{options.set_description}'
                   f'{Colors.RESET}')
@@ -241,23 +265,23 @@
             Platform.flush()
 
         # Footer
         print(' ')
         Platform.flush()
 
         # Result
-        return True
+        return Entrypoint.Result.SUCCESS
 
     # Project, pylint: disable=too-many-branches,too-many-statements
     @staticmethod
     def project(
         options: Namespace,
         gitlab: GitLabFeature,
         criteria: str,
-    ) -> bool:
+    ) -> Result:
 
         # Acquire project
         project = gitlab.project(criteria)
 
         # Show project details
         print(f'{Colors.BOLD} - GitLab project: '
               f'{Colors.YELLOW_LIGHT}{project.path_with_namespace} '
@@ -269,15 +293,15 @@
         if options.delete_project:
             gitlab.project_delete(criteria)
             print(f'{Colors.BOLD}   - Delete project: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
-            return True
+            return Entrypoint.Result.SUCCESS
 
         # Set project description
         if options.set_description:
             gitlab.project_set_description(criteria, options.set_description)
             print(f'{Colors.BOLD}   - Set description: '
                   f'{Colors.CYAN}{options.set_description}'
                   f'{Colors.RESET}')
@@ -307,27 +331,67 @@
             else:
                 print(f'{Colors.BOLD}   - Kept description: '
                       f'{Colors.GREEN}{project.description}'
                       f'{Colors.RESET}')
                 Platform.flush()
 
         # Reset project features
-        if options.reset_features:
-            features = ', '.join(gitlab.project_reset_features(criteria))
+        if options.reset_features is not None:
+            features = ', '.join(
+                gitlab.project_features_reset(
+                    criteria,
+                    GitLabFeature.project_features_parse(options.reset_features),
+                ))
             if features:
                 print(f'{Colors.BOLD}   - Reset features: '
                       f'{Colors.CYAN}{features}'
                       f'{Colors.RESET}')
                 Platform.flush()
             else:
                 print(f'{Colors.BOLD}   - Reset features: '
                       f'{Colors.GREEN}Already done'
                       f'{Colors.RESET}')
                 Platform.flush()
 
+        # Disable project features
+        if options.disable_features:
+            features = ', '.join(
+                gitlab.project_features_disable(
+                    criteria,
+                    GitLabFeature.project_features_parse(options.disable_features),
+                ))
+            if features:
+                print(f'{Colors.BOLD}   - Disable features: '
+                      f'{Colors.CYAN}{features}'
+                      f'{Colors.RESET}')
+                Platform.flush()
+            else:
+                print(f'{Colors.BOLD}   - Disable features: '
+                      f'{Colors.GREEN}Already done'
+                      f'{Colors.RESET}')
+                Platform.flush()
+
+        # Enable project features
+        if options.enable_features:
+            features = ', '.join(
+                gitlab.project_features_enable(
+                    criteria,
+                    GitLabFeature.project_features_parse(options.enable_features),
+                ))
+            if features:
+                print(f'{Colors.BOLD}   - Enable features: '
+                      f'{Colors.CYAN}{features}'
+                      f'{Colors.RESET}')
+                Platform.flush()
+            else:
+                print(f'{Colors.BOLD}   - Enable features: '
+                      f'{Colors.GREEN}Already done'
+                      f'{Colors.RESET}')
+                Platform.flush()
+
         # Reset project members
         if options.reset_members:
             gitlab.project_reset_members(criteria)
             print(f'{Colors.BOLD}   - Reset members: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
             Platform.flush()
@@ -394,8 +458,8 @@
                 Platform.flush()
 
         # Footer
         print(' ')
         Platform.flush()
 
         # Result
-        return True
+        return Entrypoint.Result.SUCCESS
```

### Comparing `gitlab_projects_settings-3.0.0/src/cli/main.py` & `gitlab_projects_settings-4.0.0/src/cli/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,35 +5,37 @@
                       RawTextHelpFormatter)
 from os import environ
 from shutil import get_terminal_size
 from sys import exit as sys_exit
 
 # Components
 from ..package.bundle import Bundle
+from ..package.settings import Settings
+from ..package.updates import Updates
 from ..package.version import Version
 from ..prints.colors import Colors
 from ..system.platform import Platform
 from .entrypoint import Entrypoint
 
 # Main, pylint: disable=too-many-statements
 def main() -> None:
 
     # Variables
     group: _ArgumentGroup
-    result: bool = False
+    result: Entrypoint.Result = Entrypoint.Result.ERROR
     subgroup: _MutuallyExclusiveGroup
 
     # Arguments creation
     parser: ArgumentParser = ArgumentParser(
         prog=Bundle.NAME,
         description=f'{Bundle.NAME}: {Bundle.DESCRIPTION}',
         add_help=False,
         formatter_class=lambda prog: RawTextHelpFormatter(
             prog,
-            max_help_position=30,
+            max_help_position=40,
             width=min(
                 120,
                 get_terminal_size().columns - 2,
             ),
         ),
     )
 
@@ -48,14 +50,35 @@
     )
     group.add_argument(
         '--version',
         dest='version',
         action='store_true',
         help='Show the current version',
     )
+    group.add_argument(
+        '--update-check',
+        dest='update_check',
+        action='store_true',
+        help='Check for newer package updates',
+    )
+    group.add_argument(
+        '--settings',
+        dest='settings',
+        action='store_true',
+        help='Show the current settings path and contents',
+    )
+    group.add_argument(
+        '--set',
+        dest='set',
+        action='store',
+        metavar=('GROUP', 'KEY', 'VAL'),
+        nargs=3,
+        help='Set settings specific \'VAL\' value to [GROUP] > KEY\n' \
+             'or unset by using \'UNSET\' as \'VAL\'',
+    )
 
     # Arguments credentials definitions
     group = parser.add_argument_group('credentials arguments')
     group.add_argument(
         '-t',
         dest='token',
         default=environ.get(Bundle.ENV_GITLAB_TOKEN, ''), #
@@ -88,18 +111,40 @@
         action='store_true',
         help='Exclude children projects settings',
     )
 
     # Arguments general settings definitions
     group = parser.add_argument_group('general settings arguments')
     group.add_argument(
+        '--available-features',
+        dest='available_features',
+        action='store_true',
+        help='List the available GitLab project features known by the tool',
+    )
+    group.add_argument(
         '--reset-features',
         dest='reset_features',
-        action='store_true',
-        help='Reset features of GitLab projects based on usage',
+        action='store',
+        metavar='KEEP_FEATURES',
+        nargs='?',
+        const='',
+        help='Reset features of GitLab projects based on usage\n'
+        '(Optionally keep features separated by ",")',
+    )
+    group.add_argument(
+        '--disable-features',
+        dest='disable_features',
+        metavar='FEATURES',
+        help='List of features to disable separated by ","',
+    )
+    group.add_argument(
+        '--enable-features',
+        dest='enable_features',
+        metavar='FEATURES',
+        help='List of features to enable separated by ","',
     )
     group.add_argument(
         '--reset-members',
         dest='reset_members',
         action='store_true',
         help='Reset members of GitLab projects and groups',
     )
@@ -173,14 +218,20 @@
         metavar='LEVEL',
         help='Protect tags at level [no-one,admins,maintainers,developers]',
     )
 
     # Arguments positional definitions
     group = parser.add_argument_group('positional arguments')
     group.add_argument(
+        '--',
+        dest='double_dash',
+        action='store_true',
+        help='Positional arguments separator (recommended)',
+    )
+    group.add_argument(
         dest='gitlab',
         action='store',
         nargs='?',
         default='https://gitlab.com',
         help='GitLab URL (default: https://gitlab.com)',
     )
     group.add_argument(
@@ -197,25 +248,48 @@
     if options.help:
         print(' ')
         parser.print_help()
         print(' ')
         Platform.flush()
         sys_exit(0)
 
+    # Instantiate settings
+    settings: Settings = Settings(name=Bundle.NAME)
+
     # Prepare colors
     Colors.prepare()
 
+    # Settings setter
+    if options.set:
+        settings.set(options.set[0], options.set[1], options.set[2])
+        settings.show()
+        sys_exit(0)
+
+    # Settings informations
+    if options.settings:
+        settings.show()
+        sys_exit(0)
+
+    # Instantiate updates
+    updates: Updates = Updates(name=Bundle.NAME, settings=settings)
+
     # Version informations
     if options.version:
         print(
             f'{Bundle.NAME} {Version.get()} from {Version.path()} (python {Version.python()})'
         )
         Platform.flush()
         sys_exit(0)
 
+    # Check for current updates
+    if options.update_check:
+        if not updates.check():
+            updates.check(older=True)
+        sys_exit(0)
+
     # Arguments validation
     if not options.token or not options.gitlab or not options.path:
         print(' ')
         parser.print_help()
         print(' ')
         Platform.flush()
         sys_exit(1)
@@ -227,16 +301,20 @@
     # CLI entrypoint
     result = Entrypoint.cli(options)
 
     # Footer
     print(' ')
     Platform.flush()
 
+    # Check for daily updates
+    if updates.enabled and updates.daily:
+        updates.check()
+
     # Result
-    if result:
+    if result in [Entrypoint.Result.SUCCESS, Entrypoint.Result.FINALIZE]:
         sys_exit(0)
     else:
         sys_exit(1)
 
 # Entrypoint
 if __name__ == '__main__': # pragma: no cover
     main()
```

### Comparing `gitlab_projects_settings-3.0.0/src/features/gitlab.py` & `gitlab_projects_settings-4.0.0/src/features/gitlab.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #!/usr/bin/env python3
 
 # Standard libraries
 from time import sleep
-from typing import List
+from typing import cast, List
 
 # Modules libraries
 from gitlab import Gitlab
-from gitlab.exceptions import GitlabGetError, GitlabListError
+from gitlab.exceptions import GitlabDeleteError, GitlabGetError, GitlabListError
 from gitlab.v4.objects import Group, Namespace, Project, User
 
-# GitLabFeature class
+# Components
+from ..types.gitlab import AccessLevels, ProjectFeatures
+
+# GitLabFeature class, pylint: disable=too-many-public-methods
 class GitLabFeature:
 
+    # Constants
+    TIMEOUT_DELETION: int = 300
+
     # Members
     __dry_run: bool = False
     __gitlab: Gitlab
 
     # Constructor
     def __init__(self, url: str, token: str, dry_run: bool = False) -> None:
         self.__dry_run = dry_run
@@ -29,15 +35,22 @@
     # Group delete
     def group_delete(self, criteria: str) -> None:
 
         # Delete group
         if not self.__dry_run:
             group = self.group(criteria)
             group.delete()
-            sleep(10)
+
+            # Wait for deletion
+            for _ in range(GitLabFeature.TIMEOUT_DELETION):
+                try:
+                    self.group(criteria)
+                    sleep(1)
+                except GitlabGetError:
+                    break
 
     # Group reset members
     def group_reset_members(self, criteria: str) -> None:
 
         # Remove group members
         group = self.group(criteria)
         for member in group.members.list(get_all=True):
@@ -82,15 +95,22 @@
     # Project delete
     def project_delete(self, criteria: str) -> None:
 
         # Delete project
         project = self.project(criteria)
         if not self.__dry_run:
             project.delete()
-            sleep(5)
+
+            # Wait for deletion
+            for _ in range(GitLabFeature.TIMEOUT_DELETION):
+                try:
+                    self.project(criteria)
+                    sleep(1)
+                except GitlabGetError:
+                    break
 
     # Project protect branches
     def project_protect_branches(self, criteria: str) -> List[str]:
 
         # Validate project feature
         result: List[str] = []
         project = self.project(criteria)
@@ -145,14 +165,181 @@
         # Save project
         if not self.__dry_run:
             project.save()
 
         # Result
         return result
 
+    # Project available features
+    @staticmethod
+    def project_features_available() -> List[str]:
+        return ProjectFeatures.names()
+
+    # Project parse features
+    @staticmethod
+    def project_features_parse(input_string: str) -> List[str]:
+
+        # Handle empty input
+        if not input_string:
+            return []
+
+        # Parse features from input
+        return [
+            key # Key
+            for search in input_string.split(',') # Input features
+            for key in ProjectFeatures.keys() # GitLab features
+            if ProjectFeatures.get(key).name.lower().startswith(search.strip().lower())
+        ]
+
+    # Project disable features
+    def project_features_disable(
+        self,
+        criteria: str,
+        features: List[str],
+    ) -> List[str]:
+
+        # Variables
+        result: List[str] = []
+        project = self.__gitlab.projects.get(criteria, statistics=True)
+
+        # Iterate through features
+        for key in features:
+            if key in ProjectFeatures.keys():
+                changed: bool = False
+                feature = ProjectFeatures.get(key)
+
+                # Disable 'access_level' feature
+                for level in feature.access_level:
+                    if getattr(project, level.key) != AccessLevels.DISABLED:
+                        changed = True
+                        setattr(
+                            project,
+                            level.key,
+                            AccessLevels.DISABLED,
+                        )
+
+                # Disable 'enabled' feature
+                for key in feature.enabled:
+                    if getattr(project, key):
+                        changed = True
+                        setattr(
+                            project,
+                            key,
+                            False,
+                        )
+
+                # Add changed feature
+                if changed:
+                    result.append(feature.name)
+
+        # Save project
+        if not self.__dry_run:
+            project.save()
+
+        # Result
+        return result
+
+    # Project enable features
+    def project_features_enable(
+        self,
+        criteria: str,
+        features: List[str],
+    ) -> List[str]:
+
+        # Variables
+        result: List[str] = []
+        project = self.__gitlab.projects.get(criteria, statistics=True)
+
+        # Iterate through features
+        for key in features:
+            if key in ProjectFeatures.keys():
+                changed: bool = False
+                feature = ProjectFeatures.get(key)
+
+                # Enable 'access_level' feature
+                for level in feature.access_level:
+                    if getattr(project, level.key) == AccessLevels.DISABLED:
+                        changed = True
+                        setattr(
+                            project,
+                            level.key,
+                            level.settings[project.visibility],
+                        )
+
+                # Enable 'enabled' feature
+                for key in feature.enabled:
+                    if not getattr(project, key):
+                        changed = True
+                        setattr(
+                            project,
+                            key,
+                            True,
+                        )
+
+                # Add changed feature
+                if changed:
+                    result.append(feature.name)
+
+        # Save project
+        if not self.__dry_run:
+            project.save()
+
+        # Result
+        return result
+
+    # Project reset features
+    def project_features_reset(
+        self,
+        criteria: str,
+        keep_features: List[str],
+    ) -> List[str]:
+
+        # Variables
+        result: List[str] = []
+        project = self.__gitlab.projects.get(criteria, statistics=True)
+
+        # Iterate through features
+        for key in ProjectFeatures.keys():
+            if key not in keep_features:
+                changed: bool = False
+                feature = ProjectFeatures.get(key)
+
+                # Disable 'access_level' feature
+                for level in feature.access_level:
+                    if changed or (getattr(project, level.key) != AccessLevels.DISABLED \
+                            and not ProjectFeatures.test(self.__gitlab, project, feature.tests)):
+                        changed = True
+                        setattr(
+                            project,
+                            level.key,
+                            AccessLevels.DISABLED,
+                        )
+
+                # Disable 'enabled' feature
+                for key in feature.enabled:
+                    if changed or (getattr(project, key) \
+                            and not ProjectFeatures.test(self.__gitlab, project, feature.tests)):
+                        changed = True
+                        setattr(
+                            project,
+                            key,
+                            False,
+                        )
+
+                # Add changed feature
+                if changed:
+                    result.append(feature.name)
+
+        # Save project
+        if not self.__dry_run:
+            project.save()
+
+        # Result
+        return result
+
     # Project protect tags, pylint: disable=too-many-branches
     def project_protect_tags(self, criteria: str, protect_level: str) -> List[str]:
 
         # Validate project feature
         result: List[str] = []
         project = self.project(criteria)
         try:
@@ -206,179 +393,25 @@
         if not self.__dry_run:
             project.save()
 
         # Result
         result.sort()
         return result
 
-    # Project reset features, pylint: disable=too-many-branches,too-many-statements
-    def project_reset_features(self, criteria: str) -> List[str]:
-
-        # Variables
-        result: List[str] = []
-        project = self.__gitlab.projects.get(criteria, statistics=True)
-
-        # Disable unused feature (Issues)
-        if project.issues_enabled and not project.issues.list(get_all=False):
-            project.issues_enabled = False
-            result += ['Issues']
-
-        # Disable unused feature (Repository)
-        try:
-            assert project.commits.list(get_all=False)
-        except (AssertionError, GitlabListError):
-            if project.repository_access_level != 'disabled':
-                project.repository_access_level = 'disabled'
-                result += ['Repository']
-
-        # Disable unused feature (Merge requests)
-        try:
-            if not project.mergerequests.list(get_all=False):
-                pass
-            elif len(project.branches.list(get_all=False)) > 1:
-                pass
-            else:
-                assert False
-        except (AssertionError, GitlabListError):
-            if project.merge_requests_enabled:
-                project.merge_requests_enabled = False
-                result += ['Merge requests']
-
-        # Disable unused feature (Forks)
-        if project.forking_access_level != 'disabled' and not project.forks.list(
-                get_all=False):
-            project.forking_access_level = 'disabled'
-            result += ['Forks']
-
-        # Disable unused feature (Git LFS)
-        if project.lfs_enabled and project.statistics['lfs_objects_size'] == 0:
-            project.lfs_enabled = False
-            result += ['Git LFS']
-
-        # Disable unused feature (CI/CD)
-        try:
-            if project.jobs.list(get_all=False):
-                pass
-            elif any('name' in item and item['name'] == '.gitlab-ci.yml'
-                     for item in project.repository_tree(get_all=True)):
-                pass
-            elif any('path_with_namespace' in item
-                     and item['path_with_namespace'] != project.path_with_namespace
-                     for item in self.__gitlab.http_get(
-                         f'/projects/{project.id}/job_token_scope/allowlist',
-                         get_all=True,
-                     )):
-                pass
-            else:
-                assert False
-        except (AssertionError, GitlabGetError, GitlabListError):
-            if project.jobs_enabled:
-                project.jobs_enabled = False
-                result += ['CI/CD']
-
-        # Disable unused feature (Container registry)
-        if project.container_registry_enabled and not project.repositories.list(
-                get_all=False):
-            project.container_registry_enabled = False
-            result += ['Container registry']
-
-        # Disable unused feature (Analytics)
-        if project.analytics_access_level != 'disabled':
-            project.analytics_access_level = 'disabled'
-            result += ['Analytics']
-
-        # Disable unused feature (Security and Compliance)
-        if project.security_and_compliance_access_level != 'disabled':
-            project.security_and_compliance_access_level = 'disabled'
-            result += ['Security and Compliance']
-
-        # Disable unused feature (Wiki)
-        if project.wiki_enabled and not project.wikis.list(get_all=False):
-            project.wiki_enabled = False
-            result += ['Wiki']
-
-        # Disable unused feature (Snippets)
-        if project.snippets_enabled and not project.snippets.list(get_all=False):
-            project.snippets_enabled = False
-            result += ['Snippets']
-
-        # Disable unused feature (Package registry)
-        if project.packages_enabled and not project.packages.list(get_all=False):
-            project.packages_enabled = False
-            result += ['Package registry']
-
-        # Disable unused feature (Model experiments)
-        if project.model_experiments_access_level != 'disabled':
-            project.model_experiments_access_level = 'disabled'
-            result += ['Model experiments']
-
-        # Disable unused feature (Model registry)
-        if project.model_registry_access_level != 'disabled':
-            project.model_registry_access_level = 'disabled'
-            result += ['Model registry']
-
-        # Disable unused feature (Pages)
-        if project.pages_access_level != 'disabled':
-            project.pages_access_level = 'disabled'
-            result += ['Pages']
-
-        # Disable unused feature (Monitor)
-        if project.monitor_access_level != 'disabled':
-            project.monitor_access_level = 'disabled'
-            result += ['Monitor']
-
-        # Disable unused feature (Environments)
-        try:
-            assert project.environments.list(get_all=False)
-        except (AssertionError, GitlabListError):
-            if project.environments_access_level != 'disabled':
-                project.environments_access_level = 'disabled'
-                result += ['Environments']
-
-        # Disable unused feature (Feature flags)
-        if project.feature_flags_access_level != 'disabled':
-            project.feature_flags_access_level = 'disabled'
-            result += ['Feature flags']
-
-        # Disable unused feature (Infrastructure)
-        if project.infrastructure_access_level != 'disabled':
-            project.infrastructure_access_level = 'disabled'
-            result += ['Infrastructure']
-
-        # Disable unused feature (Releases)
-        if project.releases_access_level != 'disabled' and not project.releases.list(
-                get_all=False):
-            project.releases_access_level = 'disabled'
-            result += ['Releases']
-
-        # Disable unused feature (Service Desk)
-        if project.service_desk_enabled:
-            project.service_desk_enabled = False
-            result += ['Service Desk']
-
-        # Disable unused feature (Auto DevOps)
-        if project.auto_devops_enabled:
-            project.auto_devops_enabled = False
-            result += ['Auto DevOps']
-
-        # Save project
-        if not self.__dry_run:
-            project.save()
-
-        # Result
-        return result
-
     # Project reset members
     def project_reset_members(self, criteria: str) -> None:
 
         # Remove project members
         if not self.__dry_run:
             project = self.project(criteria)
             for member in project.members.list(get_all=True):
-                project.members.delete(member.id)
+                try:
+                    project.members.delete(member.id)
+                except GitlabDeleteError:
+                    pass
 
             # Save project
             project.save()
 
     # Project run housekeeping
     def project_run_housekeeping(self, criteria: str) -> None:
 
@@ -421,13 +454,16 @@
             project.description = description
 
             # Save project
             project.save()
 
     # User
     def user(self, criteria: str) -> User:
-        return self.__gitlab.users.list(username=criteria)[0]
+        users = self.__gitlab.users.list(all=True, iterator=True, username=criteria)
+        for user in users:
+            return cast(User, user)
+        raise RuntimeError()
 
     # URL
     @property
     def url(self) -> str:
         return str(self.__gitlab.api_url)
```

### Comparing `gitlab_projects_settings-3.0.0/src/package/version.py` & `gitlab_projects_settings-4.0.0/src/package/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 #!/usr/bin/env python3
 
 # Standard libraries
+from os import environ
 from sys import version_info
 
 # Components
 from ..system.platform import Platform
 from .bundle import Bundle
 
 # Version class
 class Version:
 
     # Getter
     @staticmethod
     def get() -> str:
 
+        # Fake test version
+        if Bundle.ENV_DEBUG_VERSION_FAKE in environ:
+            return environ[Bundle.ENV_DEBUG_VERSION_FAKE]
+
         # Acquire version from metadata
         try:
             from importlib import metadata # pylint: disable=import-outside-toplevel
             return metadata.version(Bundle.NAME)
         except Exception: # pylint: disable=broad-exception-caught # pragma: no cover
             pass
```

### Comparing `gitlab_projects_settings-3.0.0/src/prints/colors.py` & `gitlab_projects_settings-4.0.0/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-3.0.0/src/types/namespaces.py` & `gitlab_projects_settings-4.0.0/src/types/namespaces.py`

 * *Files identical despite different names*

