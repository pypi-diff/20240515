# Comparing `tmp/gitlab_projects_migrate-2.1.0.tar.gz` & `tmp/gitlab_projects_migrate-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_migrate-2.1.0.tar", last modified: Sun Apr 28 18:42:05 2024, max compression
+gzip compressed data, was "gitlab_projects_migrate-3.0.0.tar", last modified: Wed May 15 00:04:32 2024, max compression
```

## Comparing `gitlab_projects_migrate-2.1.0.tar` & `gitlab_projects_migrate-3.0.0.tar`

### file list

```diff
@@ -1,51 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.337297 gitlab_projects_migrate-2.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.330297 gitlab_projects_migrate-2.1.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      702 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     7153 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.330297 gitlab_projects_migrate-2.1.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     2476 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5595 2024-04-28 18:42:05.337297 gitlab_projects_migrate-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3984 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.336297 gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5595 2024-04-28 18:42:05.000000 gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      894 2024-04-28 18:42:05.000000 gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 18:42:05.000000 gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-28 18:42:05.000000 gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-28 18:42:05.000000 gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-28 18:42:05.000000 gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.333297 gitlab_projects_migrate-2.1.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 18:42:05.337297 gitlab_projects_migrate-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2875 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.333297 gitlab_projects_migrate-2.1.0/src/
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.334297 gitlab_projects_migrate-2.1.0/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19797 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     5991 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.335297 gitlab_projects_migrate-2.1.0/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10277 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.335297 gitlab_projects_migrate-2.1.0/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.336297 gitlab_projects_migrate-2.1.0/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:05.336297 gitlab_projects_migrate-2.1.0/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-28 18:41:58.000000 gitlab_projects_migrate-2.1.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.681216 gitlab_projects_migrate-3.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.671216 gitlab_projects_migrate-3.0.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      702 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11965 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.672216 gitlab_projects_migrate-3.0.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     3965 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6640 2024-05-15 00:04:32.680216 gitlab_projects_migrate-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.680216 gitlab_projects_migrate-3.0.0/gitlab_projects_migrate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6640 2024-05-15 00:04:32.000000 gitlab_projects_migrate-3.0.0/gitlab_projects_migrate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-05-15 00:04:32.000000 gitlab_projects_migrate-3.0.0/gitlab_projects_migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 00:04:32.000000 gitlab_projects_migrate-3.0.0/gitlab_projects_migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-15 00:04:32.000000 gitlab_projects_migrate-3.0.0/gitlab_projects_migrate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-15 00:04:32.000000 gitlab_projects_migrate-3.0.0/gitlab_projects_migrate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-15 00:04:32.000000 gitlab_projects_migrate-3.0.0/gitlab_projects_migrate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.674216 gitlab_projects_migrate-3.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 00:04:32.681216 gitlab_projects_migrate-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.675216 gitlab_projects_migrate-3.0.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.676216 gitlab_projects_migrate-3.0.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:29.000000 gitlab_projects_migrate-3.0.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26787 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     7821 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.676216 gitlab_projects_migrate-3.0.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:29.000000 gitlab_projects_migrate-3.0.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12338 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.677216 gitlab_projects_migrate-3.0.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:29.000000 gitlab_projects_migrate-3.0.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/package/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/package/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.678216 gitlab_projects_migrate-3.0.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:29.000000 gitlab_projects_migrate-3.0.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/prints/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.679216 gitlab_projects_migrate-3.0.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:29.000000 gitlab_projects_migrate-3.0.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:32.679216 gitlab_projects_migrate-3.0.0/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:29.000000 gitlab_projects_migrate-3.0.0/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/types/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-15 00:04:28.000000 gitlab_projects_migrate-3.0.0/src/types/strings.py
```

### Comparing `gitlab_projects_migrate-2.1.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_migrate-3.0.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-2.1.0/.chglog/changelog.sh` & `gitlab_projects_migrate-3.0.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-2.1.0/.chglog/config.yml` & `gitlab_projects_migrate-3.0.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-2.1.0/.style.yapf` & `gitlab_projects_migrate-3.0.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-2.1.0/.vscode/extensions.json` & `gitlab_projects_migrate-3.0.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-2.1.0/.vscode/settings.json` & `gitlab_projects_migrate-3.0.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-2.1.0/CHANGELOG.md` & `gitlab_projects_migrate-3.0.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,45 @@
 
+<a name="3.0.0"></a>
+## [3.0.0](https://gitlab.com/AdrianDC/gitlab-projects-migrate/compare/2.1.0...3.0.0) (2024-05-15)
+
+### Bug Fixes
+
+* **entrypoint:** refactor to return no error upon final actions
+* **entrypoint:** use full paths instead of 'id' integer fields
+* **entrypoint:** minor Python codestyle improvement
+* **entrypoint:** detect if GitLab actions can continue
+* **entrypoint:** enforce against missing '.description' values
+* **gitlab:** accept deletion denials in 'project_reset_members'
+* **gitlab:** add 'description' field to fake project in '--dry-run'
+* **gitlab:** try to get real group before faking in '--dry-run'
+* **gitlab:** fix 'Any' and 'Optional' typings imports
+* **gitlab:** get all members in 'project_reset_members'
+
+### Ci
+
+* **gitlab-ci:** support multiple 'METAVAR' words in 'readme' job
+* **gitlab-ci:** deprecate requirements install in 'lint' job
+* **gitlab-ci:** implement 'images' and use project specific images
+* **gitlab-ci:** detect 'README.md' issues in 'readme' job
+* **gitlab-ci:** handle optional parameters and multiline in 'readme'
+* **gitlab-ci:** move 'readme' job after 'build' and local 'install'
+
+### Features
+
+* **entrypoint:** always flush progress output logs
+* **gitlab:** automatically wait for group and project deletions
+* **main:** document optional '--' positional arguments separator
+* **namespaces:** migrate 'Helper' class to 'Namespaces' class
+
+### Test
+
+* **version:** add 'DEBUG_VERSION_FAKE' for debugging purposes
+
+
 <a name="2.1.0"></a>
 ## [2.1.0](https://gitlab.com/AdrianDC/gitlab-projects-migrate/compare/2.0.0...2.1.0) (2024-04-28)
 
 ### Bug Fixes
 
 * **entrypoint:** resolve input group detection for projects
 * **entrypoint:** resolve input group for single project migration
```

### Comparing `gitlab_projects_migrate-2.1.0/LICENSE` & `gitlab_projects_migrate-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-2.1.0/PKG-INFO` & `gitlab_projects_migrate-3.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: gitlab-projects-migrate
-Version: 2.1.0
-Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
-Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
-Author: Adrian DC
-Author-email: radian.dc@gmail.com
-License: Apache License 2.0
-Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
-Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
-Project-URL: Documentation, https://gitlab.com/AdrianDC/gitlab-projects-migrate#gitlab-projects-migrate
-Project-URL: Source, https://gitlab.com/AdrianDC/gitlab-projects-migrate
-Project-URL: Statistics, https://pypistats.org/packages/gitlab-projects-migrate
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
 # gitlab-projects-migrate
 
 <!-- markdownlint-disable no-inline-html -->
 
 [![Build](https://gitlab.com/AdrianDC/gitlab-projects-migrate/badges/main/pipeline.svg)](https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/commits/main/)
 
 Migrate GitLab projects from a GitLab group to another GitLab's group
@@ -76,58 +42,80 @@
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--dry-run] [--exclude-group]
+usage: gitlab-projects-migrate [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-I INPUT_TOKEN]
+                               [-O OUTPUT_TOKEN] [--delete-sources] [--dry-run] [--exclude-group]
                                [--exclude-subgroups] [--exclude-projects] [--keep-members] [--overwrite]
-                               [--set-avatar FILE] [--update-description]
-                               [input_gitlab] [input_path] [output_gitlab] [output_group]
+                               [--set-avatar FILE] [--update-description] [--]
+                               [input_gitlab] [input_path] [output_gitlab] [output_namespace]
 
 gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
   -h, --help            # Show this help message
   --version             # Show the current version
+  --update-check        # Check for newer package updates
+  --settings            # Show the current settings path and contents
+  --set GROUP KEY VAL   # Set settings specific 'VAL' value to [GROUP] > KEY
+                        # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
   -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
   -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
 
 migration arguments:
+  --delete-sources      # Delete sources after successful migration
   --dry-run             # Enable dry run mode to check without saving
   --exclude-group       # Exclude parent group migration
   --exclude-subgroups   # Exclude children subgroups migration
   --exclude-projects    # Exclude children projects migration
   --keep-members        # Keep input members after importing on output GitLab
   --overwrite           # Overwrite existing projects on output GitLab
 
 general settings arguments:
   --set-avatar FILE     # Set avatar of GitLab output projects and groups
   --update-description  # Update description of GitLab output projects and groups automatically
 
 positional arguments:
+  --                    # Positional arguments separator (recommended)
   input_gitlab          # Input GitLab URL (default: https://gitlab.com)
-  input_path            # Input GitLab group or project path
+  input_path            # Input GitLab group, user namespace or project path
   output_gitlab         # Output GitLab URL (default: https://gitlab.com)
-  output_group          # Output GitLab group
+  output_namespace      # Output GitLab group or user namespace
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
+## Userspace available settings
+
+`gitlab-projects-migrate` creates a `settings.ini` configuration file in a userspace folder.
+
+For example, it allows to disable the automated updates daily check (`[updates] > enabled`)
+
+The `settings.ini` file location and contents can be shown with the following command:
+
+```bash
+gitlab-projects-migrate --settings
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

### Comparing `gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/PKG-INFO` & `gitlab_projects_migrate-3.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 2.1.0
+Version: 3.0.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
@@ -27,14 +27,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colored>=1.4.2
 Requires-Dist: python-gitlab>=4.4.0
 Requires-Dist: setuptools>=45.1.0
+Requires-Dist: update_checker>=0.18.0
 
 # gitlab-projects-migrate
 
 <!-- markdownlint-disable no-inline-html -->
 
 [![Build](https://gitlab.com/AdrianDC/gitlab-projects-migrate/badges/main/pipeline.svg)](https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/commits/main/)
 
@@ -76,58 +77,80 @@
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--dry-run] [--exclude-group]
+usage: gitlab-projects-migrate [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-I INPUT_TOKEN]
+                               [-O OUTPUT_TOKEN] [--delete-sources] [--dry-run] [--exclude-group]
                                [--exclude-subgroups] [--exclude-projects] [--keep-members] [--overwrite]
-                               [--set-avatar FILE] [--update-description]
-                               [input_gitlab] [input_path] [output_gitlab] [output_group]
+                               [--set-avatar FILE] [--update-description] [--]
+                               [input_gitlab] [input_path] [output_gitlab] [output_namespace]
 
 gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
   -h, --help            # Show this help message
   --version             # Show the current version
+  --update-check        # Check for newer package updates
+  --settings            # Show the current settings path and contents
+  --set GROUP KEY VAL   # Set settings specific 'VAL' value to [GROUP] > KEY
+                        # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
   -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
   -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
 
 migration arguments:
+  --delete-sources      # Delete sources after successful migration
   --dry-run             # Enable dry run mode to check without saving
   --exclude-group       # Exclude parent group migration
   --exclude-subgroups   # Exclude children subgroups migration
   --exclude-projects    # Exclude children projects migration
   --keep-members        # Keep input members after importing on output GitLab
   --overwrite           # Overwrite existing projects on output GitLab
 
 general settings arguments:
   --set-avatar FILE     # Set avatar of GitLab output projects and groups
   --update-description  # Update description of GitLab output projects and groups automatically
 
 positional arguments:
+  --                    # Positional arguments separator (recommended)
   input_gitlab          # Input GitLab URL (default: https://gitlab.com)
-  input_path            # Input GitLab group or project path
+  input_path            # Input GitLab group, user namespace or project path
   output_gitlab         # Output GitLab URL (default: https://gitlab.com)
-  output_group          # Output GitLab group
+  output_namespace      # Output GitLab group or user namespace
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
+## Userspace available settings
+
+`gitlab-projects-migrate` creates a `settings.ini` configuration file in a userspace folder.
+
+For example, it allows to disable the automated updates daily check (`[updates] > enabled`)
+
+The `settings.ini` file location and contents can be shown with the following command:
+
+```bash
+gitlab-projects-migrate --settings
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

### Comparing `gitlab_projects_migrate-2.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt` & `gitlab_projects_migrate-3.0.0/gitlab_projects_migrate.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -27,12 +27,18 @@
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
-src/system/platform.py
+src/system/platform.py
+src/types/__init__.py
+src/types/namespaces.py
+src/types/strings.py
```

### Comparing `gitlab_projects_migrate-2.1.0/setup.py` & `gitlab_projects_migrate-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-2.1.0/src/cli/entrypoint.py` & `gitlab_projects_migrate-3.0.0/src/cli/entrypoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 #!/usr/bin/env python3
 
 # Standard libraries
 from argparse import Namespace
+from enum import Enum
 from tempfile import NamedTemporaryFile
+from typing import Optional
 
 # Modules libraries
 from gitlab.exceptions import GitlabGetError
-from gitlab.v4.objects import Group, Project
+from gitlab.v4.objects import (
+    Group as GitLabGroup,
+    Namespace as GitLabNamespace,
+    Project as GitLabProject,
+    ProjectImport as GitLabProjectImport,
+    User as GitLabUser,
+)
 
 # Components
 from ..features.gitlab import GitLabFeature
 from ..prints.colors import Colors
 from ..system.platform import Platform
+from ..types.namespaces import Namespaces
 
-# Entrypoint class, pylint: disable=too-few-public-methods
+# Entrypoint class, pylint: disable=too-few-public-methods,too-many-statements
 class Entrypoint:
 
-    # CLI
+    # Enumerations
+    Result = Enum('Result', ['SUCCESS', 'FINALIZE', 'ERROR'])
+
+    # CLI, pylint: disable=too-many-branches
     @staticmethod
-    def cli(options: Namespace) -> bool:
+    def cli(options: Namespace) -> Result:
 
         # Variables
-        input_group: Group = None
-        input_project: Project = None
+        input_group: Optional[GitLabGroup] = None
+        input_project: Optional[GitLabProject] = None
+        input_user: Optional[GitLabUser] = None
         output_exists: bool = False
-        output_group: Group = None
+        output_namespace: Optional[GitLabNamespace] = None
+        result: Entrypoint.Result = Entrypoint.Result.ERROR
 
         # Header
         print(' ')
 
         # Input client
         input_gitlab = GitLabFeature(
             options.input_gitlab,
@@ -50,432 +64,574 @@
         Platform.flush()
 
         # Input path
         try:
             input_group = input_gitlab.group(options.input_path)
             print(f'{Colors.BOLD} - GitLab input group: '
                   f'{Colors.GREEN}{input_group.full_path}'
-                  f'{Colors.CYAN} ({input_group.description})'
-                  f'{Colors.RESET}')
-            Platform.flush()
-        except GitlabGetError:
-            input_project = input_gitlab.project(options.input_path)
-            print(f'{Colors.BOLD} - GitLab input project: '
-                  f'{Colors.GREEN}{input_project.path_with_namespace}'
-                  f'{Colors.CYAN} ({input_project.description})'
+                  f'{Colors.CYAN} ({Namespaces.text(input_group.description)})'
                   f'{Colors.RESET}')
             Platform.flush()
+        except GitlabGetError as exception:
+            try:
+                if '/' in options.input_path:
+                    raise TypeError from exception
+                input_user = input_gitlab.user(options.input_path)
+                input_namespace = input_gitlab.namespace(options.input_path)
+                print(f'{Colors.BOLD} - GitLab input user namespace: '
+                      f'{Colors.GREEN}{input_namespace.full_path}'
+                      f'{Colors.CYAN} ({input_namespace.name})'
+                      f'{Colors.RESET}')
+                print(' ')
+                Platform.flush()
+            except (GitlabGetError, TypeError):
+                input_project = input_gitlab.project(options.input_path)
+                print(f'{Colors.BOLD} - GitLab input project: '
+                      f'{Colors.GREEN}{input_project.path_with_namespace}'
+                      f'{Colors.CYAN} ({Namespaces.text(input_project.description)})'
+                      f'{Colors.RESET}')
+                Platform.flush()
 
         # Output group
         try:
             output_exists = False
-            output_group = output_gitlab.group(options.output_group)
+            output_group = output_gitlab.group(options.output_namespace)
+            output_namespace = output_gitlab.namespace(options.output_namespace)
             output_exists = True
             print(f'{Colors.BOLD} - GitLab output group: '
                   f'{Colors.GREEN}{output_group.full_path}'
-                  f'{Colors.CYAN} ({output_group.description})'
+                  f'{Colors.CYAN} ({Namespaces.text(output_group.description)})'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
 
-        # Output parent group
+        # Output namespace
         except GitlabGetError as exception:
+            try:
+                if '/' in options.output_namespace:
+                    raise TypeError from exception
+                _output_user = output_gitlab.user(options.output_namespace)
+                output_namespace = output_gitlab.namespace(options.output_namespace)
+                print(f'{Colors.BOLD} - GitLab output user namespace: '
+                      f'{Colors.GREEN}{output_namespace.full_path}'
+                      f'{Colors.CYAN} ({output_namespace.name})'
+                      f'{Colors.RESET}')
+                print(' ')
+                Platform.flush()
 
-            # Validate options
-            if not input_group or options.exclude_group:
-                raise exception
+            # Output parent group
+            except (GitlabGetError, TypeError): # pylint: disable=raise-missing-from
 
-            # Missing output group
-            print(f'{Colors.BOLD} - GitLab output group: '
-                  f'{Colors.GREEN}{options.output_group}'
-                  f'{Colors.RED} (Non-existent output group)'
-                  f'{Colors.RESET}')
-            print(' ')
-            Platform.flush()
+                # Validate options
+                if (not input_group and not input_user) or options.exclude_group:
+                    raise exception
+
+                # Missing output group
+                print(f'{Colors.BOLD} - GitLab output group: '
+                      f'{Colors.GREEN}{options.output_namespace}'
+                      f'{Colors.RED} (Non-existent output group)'
+                      f'{Colors.RESET}')
+                print(' ')
+                Platform.flush()
+
+        # Validate types
+        assert output_namespace
 
         # Handle single project
         if input_project:
+
+            # Handle project
             Entrypoint.project(
                 options,
                 input_gitlab,
                 output_gitlab,
-                input_project.id,
+                input_project.path_with_namespace,
                 input_project.namespace['id'],
-                output_group.id,
+                output_namespace.full_path,
             )
 
+            # Delete input project
+            if options.delete_sources:
+                print(f'{Colors.BOLD} - GitLab input project: '
+                      f'{Colors.GREEN}{input_project.path_with_namespace}'
+                      f'{Colors.CYAN} ({Namespaces.text(input_project.description)})'
+                      f'{Colors.RESET}')
+                Platform.flush()
+                input_gitlab.project_delete(input_project.path_with_namespace)
+                print(f'{Colors.BOLD}   - Delete sources project: '
+                      f'{Colors.GREEN}Success'
+                      f'{Colors.RESET}')
+                print(' ')
+                Platform.flush()
+
         # Handle group recursively
         elif input_group:
 
             # Handle group if missing
             if not options.exclude_group:
-                Entrypoint.group(
+                result = Entrypoint.group(
                     options,
                     input_gitlab,
                     output_gitlab,
-                    input_group.id,
-                    options.output_group,
+                    input_group.full_path,
+                    options.output_namespace,
                     migration=not output_exists,
                 )
-                output_group = output_gitlab.group(options.output_group, optional=True)
+                if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
+                    return result
+
+                # Acquire output namespace
+                output_namespace = output_gitlab.namespace(
+                    options.output_namespace,
+                    optional=True,
+                )
 
             # Iterate through subgroups
             if not options.exclude_subgroups or not output_exists:
                 for input_subgroup in sorted(
                         input_group.descendant_groups.list(
                             get_all=True,
                             include_subgroups=True,
                             order_by='path',
                             sort='asc',
                         ),
                         key=lambda item: item.full_path,
                 ):
-                    Entrypoint.subgroup(
+                    result = Entrypoint.subgroup(
                         options,
                         input_gitlab,
                         output_gitlab,
-                        input_group.id,
-                        input_subgroup.id,
-                        output_group.id,
+                        input_group.full_path,
+                        input_subgroup.full_path,
+                        output_namespace.full_path,
                         migration=output_exists,
                     )
+                    if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
+                        return result
 
             # Iterate through projects
             if not options.exclude_projects:
-                for input_project in sorted(
+                for project in sorted(
                         input_group.projects.list(
                             get_all=True,
                             include_subgroups=not options.exclude_subgroups,
                             order_by='path',
                             sort='asc',
                         ),
                         key=lambda item: item.path_with_namespace,
                 ):
-                    Entrypoint.project(
+                    result = Entrypoint.project(
                         options,
                         input_gitlab,
                         output_gitlab,
-                        input_project.id,
-                        input_group.id,
-                        output_group.id,
+                        project.path_with_namespace,
+                        input_group.full_path,
+                        output_namespace.full_path,
                     )
+                    if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
+                        return result
+
+            # Delete input group
+            if options.delete_sources:
+                print(f'{Colors.BOLD} - GitLab input group: '
+                      f'{Colors.GREEN}{input_group.full_path}'
+                      f'{Colors.CYAN} ({Namespaces.text(input_group.description)})'
+                      f'{Colors.RESET}')
+                Platform.flush()
+                input_gitlab.group_delete(input_group.full_path)
+                print(f'{Colors.BOLD}   - Delete sources group: '
+                      f'{Colors.GREEN}Success'
+                      f'{Colors.RESET}')
+                print(' ')
+                Platform.flush()
+
+        # Handle user
+        elif input_user:
+
+            # Iterate through projects
+            if not options.exclude_projects:
+                for project in sorted(
+                        input_user.projects.list(
+                            get_all=True,
+                            order_by='path',
+                            sort='asc',
+                        ),
+                        key=lambda item: item.path_with_namespace,
+                ):
+                    result = Entrypoint.project(
+                        options,
+                        input_gitlab,
+                        output_gitlab,
+                        project.path_with_namespace,
+                        input_namespace.full_path,
+                        output_namespace.full_path,
+                    )
+                    if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
+                        return result
+
+                    # Delete input project
+                    if options.delete_sources:
+                        print(f'{Colors.BOLD} - GitLab input project: '
+                              f'{Colors.GREEN}{project.path_with_namespace}'
+                              f'{Colors.CYAN} ({Namespaces.text(project.description)})'
+                              f'{Colors.RESET}')
+                        Platform.flush()
+                        input_gitlab.project_delete(project.path_with_namespace)
+                        print(f'{Colors.BOLD}   - Delete sources project: '
+                              f'{Colors.GREEN}Success'
+                              f'{Colors.RESET}')
+                        print(' ')
+                        Platform.flush()
 
         # Result
-        return True
+        return Entrypoint.Result.SUCCESS
 
     # Group, pylint: disable=too-many-arguments
     @staticmethod
     def group(
         options: Namespace,
         input_gitlab: GitLabFeature,
         output_gitlab: GitLabFeature,
         criteria_input_group: str,
         criteria_output_group: str,
         migration: bool = True,
-    ) -> None:
+    ) -> Result:
 
         # Acquire input group
         input_group = input_gitlab.group(criteria_input_group)
 
         # Detect group or subgroup
-        output_group_namespace, output_group_path = GitLabFeature.Helper.split_namespace(
+        output_group_namespace, output_group_path = Namespaces.split_namespace(
             criteria_output_group,
             relative=False,
         )
         output_group_name = input_group.name \
             if input_group.name != input_group.path \
             else output_group_path
 
         # Show group details
         print(f'{Colors.BOLD} - GitLab group: '
               f'{Colors.YELLOW_LIGHT}{input_group.full_path} '
-              f'{Colors.CYAN}({input_group.description})'
+              f'{Colors.CYAN}({Namespaces.text(input_group.description)})'
               f'{Colors.RESET}')
+        Platform.flush()
 
         # Migration mode
         if not migration:
             output_subgroup = output_gitlab.group(criteria_output_group)
             print(f'{Colors.BOLD}   - Already exists in GitLab output: '
                   f'{Colors.GREEN}{output_subgroup.full_path}'
-                  f'{Colors.CYAN} ({output_subgroup.description})'
+                  f'{Colors.CYAN} ({Namespaces.text(output_subgroup.description)})'
                   f'{Colors.RESET}')
             print(' ')
-            return
+            Platform.flush()
+            return Entrypoint.Result.SUCCESS
 
         # Export group
         print(f'{Colors.BOLD}   - Exporting from: '
               f'{Colors.GREEN}{input_group.full_path}'
               f'{Colors.RESET}')
+        Platform.flush()
         with NamedTemporaryFile(suffix='.tar.gz') as file_export:
             input_gitlab.group_export(
                 file_export.name,
-                input_group.id,
+                input_group.full_path,
                 options.keep_members,
             )
 
             # Import group
             print(f'{Colors.BOLD}   - Importing to: '
                   f'{Colors.GREEN}{criteria_output_group}'
                   f'{Colors.RESET}')
+            Platform.flush()
             output_gitlab.group_import(
                 file_export.name,
                 output_group_namespace,
                 output_group_path,
                 output_group_name,
             )
 
         # Acquire output group
-        output_group_id: str = ''
+        output_group_criteria: str = ''
         if not options.dry_run:
             output_group = output_gitlab.group(criteria_output_group)
-            output_group_id = output_group.id
+            output_group_criteria = output_group.full_path
 
         # Set group description
-        description = GitLabFeature.Helper.describe(
-            input_group.description,
-            output_group_name,
+        description = Namespaces.describe(
+            name=output_group_name,
+            description=input_group.description,
         )
         output_gitlab.group_set_description(
-            output_group_id,
+            output_group_criteria,
             description,
         )
         print(f'{Colors.BOLD}   - Set description: '
               f'{Colors.CYAN}{description}'
               f'{Colors.RESET}')
+        Platform.flush()
 
         # Set group avatar
         if options.set_avatar:
             output_gitlab.group_set_avatar(
-                output_group_id,
+                output_group_criteria,
                 options.set_avatar,
             )
             print(f'{Colors.BOLD}   - Set avatar: '
                   f'{Colors.CYAN}{options.set_avatar}'
                   f'{Colors.RESET}')
+            Platform.flush()
 
         # Show group result
         print(f'{Colors.BOLD}   - Migrated group: '
               f'{Colors.GREEN}Success'
               f'{Colors.RESET}')
+        Platform.flush()
 
         # Footer
         print(' ')
         Platform.flush()
 
+        # Result
+        return Entrypoint.Result.SUCCESS
+
     # Project, pylint: disable=too-many-arguments,too-many-branches,too-many-locals
     @staticmethod
     def project(
         options: Namespace,
         input_gitlab: GitLabFeature,
         output_gitlab: GitLabFeature,
         criteria_project: str,
-        criteria_input_group: str,
-        criteria_output_group: str,
-    ) -> None:
+        criteria_input_namespace: str,
+        criteria_output_namespace: str,
+    ) -> Result:
+
+        # Variables
+        output_project: GitLabProjectImport
 
         # Acquire input project
         input_project = input_gitlab.project(criteria_project)
 
-        # Acquire input group
-        input_group = input_gitlab.group(criteria_input_group)
+        # Acquire input namespace
+        input_namespace = input_gitlab.namespace(criteria_input_namespace)
 
-        # Acquire output group
-        output_group = output_gitlab.group(criteria_output_group, optional=True)
+        # Acquire output namespace
+        output_namespace = output_gitlab.namespace(
+            criteria_output_namespace,
+            optional=True,
+        )
 
         # Show project details
         print(f'{Colors.BOLD} - GitLab input project: '
               f'{Colors.YELLOW_LIGHT}{input_project.path_with_namespace} '
-              f'{Colors.CYAN}({input_project.description})'
+              f'{Colors.CYAN}({Namespaces.text(input_project.description)})'
               f'{Colors.RESET}')
+        Platform.flush()
 
         # Ignore existing projects
-        input_subpath = GitLabFeature.Helper.subpath(
-            input_group.full_path,
+        input_subpath = Namespaces.subpath(
+            input_namespace.full_path,
             input_project.path_with_namespace,
         )
         if not options.overwrite and input_subpath in [
-                GitLabFeature.Helper.subpath(
-                    output_group.full_path,
+                Namespaces.subpath(
+                    output_namespace.full_path,
                     output_project.path_with_namespace,
-                ) for output_project in output_group.projects.list(
-                    get_all=True,
-                    include_subgroups=True,
-                )
+                ) for output_project in output_gitlab.namespace_projects(
+                    criteria_output_namespace)
         ]:
-            output_group_project = output_gitlab.project(
-                f'{output_group.full_path}/{input_subpath}')
+            project = output_gitlab.project(
+                f'{output_namespace.full_path}/{input_subpath}')
             print(f'{Colors.BOLD}   - Already exists in GitLab output: '
-                  f'{Colors.GREEN}{output_group_project.path_with_namespace}'
-                  f'{Colors.CYAN} ({output_group_project.description})'
+                  f'{Colors.GREEN}{project.path_with_namespace}'
+                  f'{Colors.CYAN} ({Namespaces.text(project.description)})'
                   f'{Colors.RESET}')
             print(' ')
-            return
+            Platform.flush()
+            return Entrypoint.Result.SUCCESS
 
         # Export project
         print(f'{Colors.BOLD}   - Exporting from: '
               f'{Colors.GREEN}{options.input_path}'
               f'{Colors.CYAN} / {input_subpath}'
               f'{Colors.RESET}')
+        Platform.flush()
         with NamedTemporaryFile(suffix='.tar.gz') as file_export:
             input_gitlab.project_export(
                 file_export.name,
-                input_project.id,
+                input_project.path_with_namespace,
                 options.keep_members,
             )
 
             # Existing project removal
             if options.overwrite:
-                output_gitlab.project_delete(f'{output_group.full_path}/{input_subpath}')
+                output_gitlab.project_delete(
+                    f'{output_namespace.full_path}/{input_subpath}')
 
             # Import project
             print(f'{Colors.BOLD}   - Importing to: '
-                  f'{Colors.GREEN}{options.output_group}'
+                  f'{Colors.GREEN}{options.output_namespace}'
                   f'{Colors.CYAN} / {input_subpath}'
                   f'{Colors.RESET}')
-            output_namespace, output_path = GitLabFeature.Helper.split_namespace(
+            Platform.flush()
+            output_subnamespace, output_path = Namespaces.split_namespace(
                 input_subpath,
                 relative=True,
             )
-            imported_project = output_gitlab.project_import(
+            output_project = output_gitlab.project_import(
                 file_export.name,
-                f'{options.output_group}{output_namespace}',
+                f'{options.output_namespace}{output_subnamespace}',
                 output_path,
                 input_project.name,
                 options.overwrite,
             )
 
-            # Acquire subgroup description
-            output_subgroup_description: str
-            if not options.dry_run:
-                output_subgroup = output_gitlab.group(
-                    f'{options.output_group}{output_namespace}')
-                output_subgroup_description = output_subgroup.description
-            else:
-                output_subgroup_description = input_project.description
+        # Acquire subgroup description
+        output_subgroup_description: str
+        if options.dry_run:
+            output_subgroup_description = input_project.description
+        elif output_namespace.kind == 'user':
+            output_subgroup_description = output_namespace.name
+        else:
+            output_subgroup = output_gitlab.group(
+                f'{options.output_namespace}{output_subnamespace}')
+            output_subgroup_description = output_subgroup.description
 
-            # Update project description
-            if options.update_description:
-                group_description = GitLabFeature.Helper.describe(
-                    output_subgroup_description,
-                    input_project.name,
-                )
-                if not imported_project.description.endswith(f' - {group_description}'):
-                    description = f'{GitLabFeature.Helper.capitalize(imported_project.name)}' \
+        # Update project description
+        if options.update_description:
+            group_description = Namespaces.describe(
+                name=input_project.name,
+                description=output_subgroup_description,
+            )
+            if not output_project.description or \
+                    not output_project.description.endswith(f' - {group_description}'):
+                description = f'{Namespaces.describe(name=output_project.name)}' \
                                 f' - {group_description}'
-                    output_gitlab.project_set_description(
-                        imported_project.id,
-                        description,
-                    )
-                    print(f'{Colors.BOLD}   - Updated description: '
-                          f'{Colors.CYAN}{description}'
-                          f'{Colors.RESET}')
-                else:
-                    print(f'{Colors.BOLD}   - Kept description: '
-                          f'{Colors.GREEN}{imported_project.description}'
-                          f'{Colors.RESET}')
-
-            # Reset project members
-            if not options.keep_members:
-                output_gitlab.project_reset_members(imported_project.id)
-                print(f'{Colors.BOLD}   - Reset members: '
-                      f'{Colors.GREEN}Success'
-                      f'{Colors.RESET}')
-
-            # Set project avatar
-            if options.set_avatar:
-                output_gitlab.project_set_avatar(
-                    imported_project.id,
-                    options.set_avatar,
+                output_gitlab.project_set_description(
+                    output_project.path_with_namespace,
+                    description,
                 )
-                print(f'{Colors.BOLD}   - Set avatar: '
-                      f'{Colors.CYAN}{options.set_avatar}'
+                print(f'{Colors.BOLD}   - Updated description: '
+                      f'{Colors.CYAN}{description}'
+                      f'{Colors.RESET}')
+                Platform.flush()
+            else:
+                print(f'{Colors.BOLD}   - Kept description: '
+                      f'{Colors.GREEN}{Namespaces.text(output_project.description)}'
                       f'{Colors.RESET}')
+                Platform.flush()
+
+        # Reset project members
+        if not options.keep_members:
+            output_gitlab.project_reset_members(output_project.path_with_namespace)
+            print(f'{Colors.BOLD}   - Reset members: '
+                  f'{Colors.GREEN}Success'
+                  f'{Colors.RESET}')
+            Platform.flush()
+
+        # Set project avatar
+        if options.set_avatar:
+            output_gitlab.project_set_avatar(
+                output_project.path_with_namespace,
+                options.set_avatar,
+            )
+            print(f'{Colors.BOLD}   - Set avatar: '
+                  f'{Colors.CYAN}{options.set_avatar}'
+                  f'{Colors.RESET}')
+            Platform.flush()
 
         # Show project result
         print(f'{Colors.BOLD}   - Migrated project: '
               f'{Colors.GREEN}Success'
               f'{Colors.RESET}')
         print(' ')
         Platform.flush()
 
-    # Subgroup, pylint: disable=too-many-arguments
+        # Result
+        return Entrypoint.Result.SUCCESS
+
+    # Subgroup, pylint: disable=too-many-arguments,too-many-statements
     @staticmethod
     def subgroup(
         options: Namespace,
         input_gitlab: GitLabFeature,
         output_gitlab: GitLabFeature,
         criteria_input_group: str,
         criteria_input_subgroup: str,
         criteria_output_group: str,
         migration: bool = True,
-    ) -> None:
+    ) -> Result:
 
         # Acquire input group
         input_group = input_gitlab.group(criteria_input_group)
 
         # Acquire input subgroup
         input_subgroup = input_gitlab.group(criteria_input_subgroup)
 
         # Acquire output group
         output_group = output_gitlab.group(criteria_output_group, optional=True)
 
         # Show subgroup details
         print(f'{Colors.BOLD} - GitLab subgroup: '
               f'{Colors.YELLOW_LIGHT}{input_subgroup.full_path} '
-              f'{Colors.CYAN}({input_subgroup.description})'
+              f'{Colors.CYAN}({Namespaces.text(input_subgroup.description)})'
               f'{Colors.RESET}')
+        Platform.flush()
 
         # Parse subgroup paths
-        input_subpath = GitLabFeature.Helper.subpath(
+        input_subpath = Namespaces.subpath(
             input_group.full_path,
             input_subgroup.full_path,
         )
-        output_namespace, output_path = GitLabFeature.Helper.split_namespace(
+        output_namespace, output_path = Namespaces.split_namespace(
             input_subpath,
             relative=True,
         )
 
         # Migration mode
         if migration:
 
             # Ignore existing group
             if input_subpath in [
-                    GitLabFeature.Helper.subpath(
+                    Namespaces.subpath(
                         output_group.full_path,
                         output_subgroup.full_path,
                     ) for output_subgroup in output_group.descendant_groups.list(
                         get_all=True,
                         include_subgroups=True,
                     )
             ]:
                 output_subgroup = output_gitlab.group(
                     f'{output_group.full_path}/{input_subpath}')
                 print(f'{Colors.BOLD}   - Already exists in GitLab output: '
                       f'{Colors.GREEN}{output_subgroup.full_path}'
-                      f'{Colors.CYAN} ({output_subgroup.description})'
+                      f'{Colors.CYAN} ({Namespaces.text(output_subgroup.description)})'
                       f'{Colors.RESET}')
                 print(' ')
-                return
+                Platform.flush()
+                return Entrypoint.Result.SUCCESS
 
             # Export subgroup
             print(f'{Colors.BOLD}   - Exporting from: '
                   f'{Colors.GREEN}{input_subgroup.full_path}'
                   f'{Colors.RESET}')
+            Platform.flush()
             with NamedTemporaryFile(suffix='.tar.gz') as file_export:
                 input_gitlab.group_export(
                     file_export.name,
-                    input_subgroup.id,
+                    input_subgroup.full_path,
                     options.keep_members,
                 )
 
                 # Import subgroup
                 print(
                     f'{Colors.BOLD}   - Importing to: '
                     f'{Colors.GREEN}{output_group.full_path}{output_namespace}/{output_path}'
                     f'{Colors.RESET}')
+                Platform.flush()
                 output_gitlab.group_import(
                     file_export.name,
                     f'{output_group.full_path}{output_namespace}',
                     output_path,
                     input_subgroup.name,
                 )
 
@@ -494,44 +650,51 @@
         else:
             output_subgroup_parent_description = input_subgroup.description
             output_subgroup_child_description = input_subgroup.description
             output_subgroup_child_name = input_subgroup.name
 
         # Update group description
         if options.update_description:
-            parent_description = GitLabFeature.Helper.describe(
-                output_subgroup_parent_description,
-                output_subgroup_child_name,
+            parent_description = Namespaces.describe(
+                name=output_subgroup_child_name,
+                description=output_subgroup_parent_description,
             )
             if not output_subgroup_child_description.endswith(f' - {parent_description}'):
-                description = f'{GitLabFeature.Helper.capitalize(output_subgroup_child_name)}' \
-                            f' - {parent_description}'
+                description = f'{Namespaces.describe(name=output_subgroup_child_name)}' \
+                              f' - {parent_description}'
                 output_gitlab.group_set_description(
                     f'{output_group.full_path}/{input_subpath}',
                     description,
                 )
                 print(f'{Colors.BOLD}   - Updated description: '
                       f'{Colors.CYAN}{description}'
                       f'{Colors.RESET}')
+                Platform.flush()
             else:
                 print(f'{Colors.BOLD}   - Kept description: '
                       f'{Colors.GREEN}{output_subgroup_child_description}'
                       f'{Colors.RESET}')
+                Platform.flush()
 
         # Set group avatar
         if options.set_avatar:
             output_gitlab.group_set_avatar(
                 f'{output_group.full_path}/{input_subpath}',
                 options.set_avatar,
             )
             print(f'{Colors.BOLD}   - Set avatar: '
                   f'{Colors.CYAN}{options.set_avatar}'
                   f'{Colors.RESET}')
+            Platform.flush()
 
         # Show subgroup result
         print(f'{Colors.BOLD}   - Migrated subgroup: '
               f'{Colors.GREEN}Success'
               f'{Colors.RESET}')
+        Platform.flush()
 
         # Footer
         print(' ')
         Platform.flush()
+
+        # Result
+        return Entrypoint.Result.SUCCESS
```

### Comparing `gitlab_projects_migrate-2.1.0/src/cli/main.py` & `gitlab_projects_migrate-3.0.0/src/cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 from argparse import (_ArgumentGroup, ArgumentParser, Namespace, RawTextHelpFormatter)
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
 
     # Arguments creation
     parser: ArgumentParser = ArgumentParser(
         prog=Bundle.NAME,
         description=f'{Bundle.NAME}: {Bundle.DESCRIPTION}',
         add_help=False,
         formatter_class=lambda prog: RawTextHelpFormatter(
@@ -46,14 +48,35 @@
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
         '-I',
         dest='input_token',
         default=environ.get(
@@ -81,14 +104,20 @@
         f', {Bundle.ENV_GITLAB_TOKEN} environments,'
         ' or INPUT_TOKEN argument)',
     )
 
     # Arguments migration definitions
     group = parser.add_argument_group('migration arguments')
     group.add_argument(
+        '--delete-sources',
+        dest='delete_sources',
+        action='store_true',
+        help='Delete sources after successful migration',
+    )
+    group.add_argument(
         '--dry-run',
         dest='dry_run',
         action='store_true',
         help='Enable dry run mode to check without saving',
     )
     group.add_argument(
         '--exclude-group',
@@ -136,66 +165,95 @@
         action='store_true',
         help='Update description of GitLab output projects and groups automatically',
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
         dest='input_gitlab',
         action='store',
         nargs='?',
         default='https://gitlab.com',
         help='Input GitLab URL (default: https://gitlab.com)',
     )
     group.add_argument(
         dest='input_path',
         action='store',
         nargs='?',
-        help='Input GitLab group or project path',
+        help='Input GitLab group, user namespace or project path',
     )
     group.add_argument(
         dest='output_gitlab',
         action='store',
         nargs='?',
         default='https://gitlab.com',
         help='Output GitLab URL (default: https://gitlab.com)',
     )
     group.add_argument(
-        dest='output_group',
+        dest='output_namespace',
         action='store',
         nargs='?',
         default='',
-        help='Output GitLab group',
+        help='Output GitLab group or user namespace',
     )
 
     # Arguments parser
     options: Namespace = parser.parse_args()
 
     # Help informations
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
     if not options.input_token or not options.input_gitlab or not options.input_path \
-            or not options.output_gitlab or not options.output_group:
+            or not options.output_gitlab or not options.output_namespace:
         print(' ')
         parser.print_help()
         print(' ')
         Platform.flush()
         sys_exit(1)
 
     # Arguments adaptations
@@ -209,16 +267,20 @@
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

### Comparing `gitlab_projects_migrate-2.1.0/src/features/gitlab.py` & `gitlab_projects_migrate-3.0.0/src/features/gitlab.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,61 +4,76 @@
 from collections import namedtuple
 from os import remove
 from os.path import join
 from pathlib import Path
 from shutil import make_archive, unpack_archive
 from tempfile import TemporaryDirectory
 from time import sleep
-from typing import List, Tuple
+from typing import Any, cast, List, Optional
 
 # Modules libraries
 from gitlab import Gitlab
-from gitlab.exceptions import GitlabGetError
-from gitlab.v4.objects import Any, Group, Optional, Project
+from gitlab.exceptions import GitlabDeleteError, GitlabGetError
+from gitlab.v4.objects import Group, Namespace, Project, ProjectImport, User
+
+# Components
+from ..types.namespaces import Namespaces
 
 # GitLabFeature class
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
         self.__gitlab = Gitlab(url, private_token=token)
         self.__gitlab.auth()
 
     # Group
     def group(self, criteria: str, optional: bool = False) -> Group:
 
-        # Fake group for dry run
+        # Optional group for dry run
         if self.__dry_run and optional:
-            GroupTuple = namedtuple('GroupTuple', [
-                'id',
-                'name',
-                'full_path',
-                'projects',
-            ])
+            try:
+                return self.group(criteria, optional=False)
 
-            # pylint: disable=no-self-use,too-few-public-methods
-            class GroupProjects:
-                def list(self, **_kwargs: Optional[Any]) -> List[str]:
-                    return []
-
-            _, path = GitLabFeature.Helper.split_namespace(
-                criteria,
-                relative=False,
-            )
-            return GroupTuple(
-                id='dry-run',
-                name=path,
-                full_path=criteria,
-                projects=GroupProjects(),
-            )
+            # Simulate group
+            except GitlabGetError:
+                GroupTuple = namedtuple('GroupTuple', [
+                    'id',
+                    'name',
+                    'full_path',
+                    'projects',
+                ])
+
+                # pylint: disable=no-self-use,too-few-public-methods
+                class GroupProjects:
+                    def list(self, **_kwargs: Optional[Any]) -> List[str]:
+                        return []
+
+                # Create fake group
+                _, path = Namespaces.split_namespace(
+                    criteria,
+                    relative=False,
+                )
+                return cast(
+                    Group,
+                    GroupTuple(
+                        id='dry-run',
+                        name=path,
+                        full_path=criteria,
+                        projects=GroupProjects(),
+                    ),
+                )
 
         # Get group
         return self.__gitlab.groups.get(criteria)
 
     # Group create
     def group_create(self, path: str, name: str) -> None:
 
@@ -67,14 +82,30 @@
             self.__gitlab.groups.create({
                 'parent_id': None,
                 'path': path,
                 'name': name,
             })
             sleep(5)
 
+    # Group delete
+    def group_delete(self, criteria: str) -> None:
+
+        # Delete group
+        if not self.__dry_run:
+            group = self.group(criteria)
+            group.delete()
+
+            # Wait for deletion
+            for _ in range(GitLabFeature.TIMEOUT_DELETION):
+                try:
+                    self.group(criteria)
+                    sleep(1)
+                except GitlabGetError:
+                    break
+
     # Group export
     def group_export(
         self,
         archive: str,
         criteria: str,
         keep_members: bool = False,
     ) -> None:
@@ -129,15 +160,15 @@
             sleep(5)
 
     # Group reset members
     def group_reset_members(self, criteria: str) -> None:
 
         # Remove group members
         group = self.group(criteria)
-        for member in group.members.list():
+        for member in group.members.list(get_all=True):
             if not self.__dry_run:
                 group.members.delete(member.id)
 
         # Save group
         if not self.__dry_run:
             group.save()
 
@@ -160,28 +191,88 @@
         if not self.__dry_run:
             group = self.group(criteria)
             group.description = description
 
             # Save group
             group.save()
 
+    # Namespace
+    def namespace(self, criteria: str, optional: bool = False) -> Namespace:
+
+        # Optional namespace for dry run
+        if self.__dry_run and optional:
+            try:
+                return self.namespace(criteria, optional=False)
+
+            # Simulate namespace
+            except GitlabGetError:
+                NamespaceTuple = namedtuple('NamespaceTuple', [
+                    'id',
+                    'name',
+                    'full_path',
+                ])
+
+                # Create fake namespace
+                _, path = Namespaces.split_namespace(
+                    criteria,
+                    relative=False,
+                )
+                return cast(
+                    Namespace,
+                    NamespaceTuple(
+                        id='dry-run',
+                        name=path,
+                        full_path=criteria,
+                    ),
+                )
+
+        # Get namespace
+        return self.__gitlab.namespaces.get(criteria)
+
+    # Namespace projects
+    def namespace_projects(self, criteria: str) -> Any:
+
+        # Acquire namespace
+        namespace = self.namespace(criteria)
+
+        # Get user projects
+        if namespace.kind == 'user':
+            user = self.user(criteria)
+            return user.projects.list(get_all=True)
+
+        # Get group projects
+        return self.group(criteria).projects.list(
+            get_all=True,
+            include_subgroups=True,
+        )
+
     # Project
     def project(self, criteria: str) -> Project:
         return self.__gitlab.projects.get(criteria)
 
     # Project delete
     def project_delete(self, criteria: str) -> None:
 
         # Delete project
-        try:
-            if not self.__dry_run:
-                self.project(criteria).delete()
-                sleep(5)
-        except GitlabGetError:
-            pass
+        if not self.__dry_run:
+            try:
+                project = self.project(criteria)
+                project.delete()
+
+                # Wait for deletion
+                for _ in range(GitLabFeature.TIMEOUT_DELETION):
+                    try:
+                        self.project(criteria)
+                        sleep(1)
+                    except GitlabGetError:
+                        break
+
+            # Ignore missing project
+            except GitlabGetError:
+                pass
 
     # Project export
     def project_export(
         self,
         archive: str,
         criteria: str,
         keep_members: bool = False,
@@ -222,31 +313,39 @@
     def project_import(
         self,
         archive: str,
         group: str,
         path: str,
         name: str,
         overwrite: bool = False,
-    ) -> Project:
+    ) -> ProjectImport:
 
         # Validate project access
         if self.__dry_run:
             ProjectTuple = namedtuple('ProjectTuple', [
                 'id',
                 'name',
+                'description',
             ])
-            return ProjectTuple(
-                id='dry-run',
-                name=name,
+            return cast(
+                ProjectImport,
+                ProjectTuple(
+                    id='dry-run',
+                    name=name,
+                    description=Namespaces.capitalize(
+                        name,
+                        words=True,
+                    ),
+                ),
             )
 
         # Upload project import
         with open(archive, 'rb') as file:
             project_imported = self.__gitlab.projects.import_project(
-                file,
+                str(file),
                 path=path,
                 name=name,
                 namespace=group,
                 overwrite=overwrite,
             )
 
         # Wait project import
@@ -261,16 +360,19 @@
 
     # Project reset members
     def project_reset_members(self, criteria: str) -> None:
 
         # Remove project members
         if not self.__dry_run:
             project = self.project(criteria)
-            for member in project.members.list():
-                project.members.delete(member.id)
+            for member in project.members.list(get_all=True):
+                try:
+                    project.members.delete(member.id)
+                except GitlabDeleteError:
+                    pass
 
             # Save project
             project.save()
 
     # Project set avatar
     def project_set_avatar(self, criteria: str, file: str) -> None:
 
@@ -303,59 +405,18 @@
             self.__gitlab.groups.create({
                 'parent_id': group.id,
                 'path': path,
                 'name': name,
             })
             sleep(5)
 
+    # User
+    def user(self, criteria: str) -> User:
+        users = self.__gitlab.users.list(all=True, iterator=True, username=criteria)
+        for user in users:
+            return cast(User, user)
+        raise RuntimeError()
+
     # URL
     @property
     def url(self) -> str:
         return str(self.__gitlab.api_url)
-
-    # Helper class
-    class Helper:
-
-        # Capitalize
-        @staticmethod
-        def capitalize(text: str) -> str:
-            return f'{text[:1].capitalize()}{text[1:]}'
-
-        # Describe
-        @staticmethod
-        def describe(
-            description: str,
-            name: str,
-        ) -> str:
-            if description:
-                return description
-            return GitLabFeature.Helper.capitalize(name)
-
-        # Split namespace
-        @staticmethod
-        def split_namespace(
-            path: str,
-            relative: bool = False,
-        ) -> Tuple[str, str]:
-            return (
-                # Namespace
-                f'/{path[:path.rfind("/")]}' if '/' in path and relative else \
-                f'{path[:path.rfind("/")]}' if '/' in path else \
-                '',
-                # Path
-                f'{path[path.rfind("/") + 1:]}' if '/' in path else \
-                path,
-            )
-
-        # Subpath
-        @staticmethod
-        def subpath(
-            parent_path: str,
-            child_path: str,
-        ) -> str:
-
-            # Parse relative path
-            if child_path.startswith(f'{parent_path}/'):
-                return child_path[len(f'{parent_path}/'):]
-
-            # Default absolute path
-            return child_path
```

### Comparing `gitlab_projects_migrate-2.1.0/src/package/version.py` & `gitlab_projects_migrate-3.0.0/src/package/version.py`

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

### Comparing `gitlab_projects_migrate-2.1.0/src/prints/colors.py` & `gitlab_projects_migrate-3.0.0/src/prints/colors.py`

 * *Files identical despite different names*

