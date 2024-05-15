# Comparing `tmp/pyams_security_views-2.3.0.tar.gz` & `tmp/pyams_security_views-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_security_views-2.3.0.tar", last modified: Mon Feb 26 22:45:34 2024, max compression
+gzip compressed data, was "dist/pyams_security_views-2.3.1.tar", last modified: Wed May 15 16:36:04 2024, max compression
```

## Comparing `pyams_security_views-2.3.0.tar` & `pyams_security_views-2.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4924 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)     3242 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2683 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/api/
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3705 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/api/principal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    11157 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/src/pyams_security_views/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1373 2024-02-01 12:15:55.000000 pyams_security_views-2.3.0/src/pyams_security_views/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      750 2024-02-01 12:15:55.000000 pyams_security_views-2.3.0/src/pyams_security_views/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5280 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/src/pyams_security_views/interfaces/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11328 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo
--rw-rw-rw-   0 root         (0) root         (0)    18080 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po
--rw-rw-rw-   0 root         (0) root         (0)    12112 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/src/pyams_security_views/locales/pyams_security_views.pot
--rw-rw-rw-   0 root         (0) root         (0)     2503 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/src/pyams_security_views/login.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/skin/
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12831 2024-02-14 16:28:55.000000 pyams_security_views-2.3.0/src/pyams_security_views/skin/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      299 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/skin/templates/login-logo.pt
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/skin/templates/login-viewlet.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/tests/
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/widget/
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/widget/permission.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-02-01 12:15:55.000000 pyams_security_views-2.3.0/src/pyams_security_views/widget/principal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7312 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4989 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/login.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     6980 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4196 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     9534 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/group.py
--rw-rw-rw-   0 root         (0) root         (0)      716 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    21686 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/userfolder.py
--rw-rw-rw-   0 root         (0) root         (0)     6482 2024-02-26 22:40:06.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     3613 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2024-01-03 11:51:37.000000 pyams_security_views-2.3.0/src/pyams_security_views/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4924 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2048 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 22:45:24.000000 pyams_security_views-2.3.0/src/pyams_security_views.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      291 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-26 22:45:34.000000 pyams_security_views-2.3.0/src/pyams_security_views.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4989 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     3307 2024-05-15 16:29:32.000000 pyams_security_views-2.3.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2683 2024-05-15 16:29:32.000000 pyams_security_views-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/api/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3705 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/api/principal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    11157 2024-02-26 22:40:06.000000 pyams_security_views-2.3.1/src/pyams_security_views/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2024-02-01 12:15:55.000000 pyams_security_views-2.3.1/src/pyams_security_views/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      750 2024-02-01 12:15:55.000000 pyams_security_views-2.3.1/src/pyams_security_views/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5280 2024-02-26 22:40:06.000000 pyams_security_views-2.3.1/src/pyams_security_views/interfaces/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11328 2024-02-26 22:40:06.000000 pyams_security_views-2.3.1/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo
+-rw-rw-rw-   0 root         (0) root         (0)    18080 2024-02-26 22:40:06.000000 pyams_security_views-2.3.1/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po
+-rw-rw-rw-   0 root         (0) root         (0)    12112 2024-02-26 22:40:06.000000 pyams_security_views-2.3.1/src/pyams_security_views/locales/pyams_security_views.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2024-02-26 22:40:06.000000 pyams_security_views-2.3.1/src/pyams_security_views/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12910 2024-05-15 16:29:32.000000 pyams_security_views-2.3.1/src/pyams_security_views/skin/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/skin/templates/login-logo.pt
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/skin/templates/login-viewlet.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/widget/permission.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-02-01 12:15:55.000000 pyams_security_views-2.3.1/src/pyams_security_views/widget/principal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7312 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2024-02-26 22:40:06.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/notifications.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     6980 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4196 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     9534 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/group.py
+-rw-rw-rw-   0 root         (0) root         (0)      716 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    21686 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/userfolder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6482 2024-02-26 22:40:06.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3613 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2024-01-03 11:51:37.000000 pyams_security_views-2.3.1/src/pyams_security_views/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4989 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:35:55.000000 pyams_security_views-2.3.1/src/pyams_security_views.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 16:36:04.000000 pyams_security_views-2.3.1/src/pyams_security_views.egg-info/top_level.txt
```

### Comparing `pyams_security_views-2.3.0/LICENSE` & `pyams_security_views-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/PKG-INFO` & `pyams_security_views-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_security_views
-Version: 2.3.0
+Version: 2.3.1
 Summary: Pyramid views for PyAMS_security package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -46,14 +46,18 @@
 interface (based on PyAMS_zmi package), custom widgets and a small Cornice REST API to look for
 principals.
 
 
 Changelog
 =========
 
+2.3.1
+-----
+ - added support for custom modal content CSS class
+
 2.3.0
 -----
  - added property in login configuration to set user registration activation delay
  - updated roles edit form permission
 
 2.2.0
 -----
```

### Comparing `pyams_security_views-2.3.0/docs/HISTORY.rst` & `pyams_security_views-2.3.1/docs/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.3.1
+-----
+ - added support for custom modal content CSS class
+
 2.3.0
 -----
  - added property in login configuration to set user registration activation delay
  - updated roles edit form permission
 
 2.2.0
 -----
```

### Comparing `pyams_security_views-2.3.0/docs/README.rst` & `pyams_security_views-2.3.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/setup.py` & `pyams_security_views-2.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.3.0'
+version = '2.3.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'cornice_swagger',
     'pyams_i18n_views',
     'pyams_zmi',
     'pyramid_zcml',
```

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/__init__.py` & `pyams_security_views-2.3.1/src/pyams_security_views/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/api/__init__.py` & `pyams_security_views-2.3.1/src/pyams_security_views/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/api/principal.py` & `pyams_security_views-2.3.1/src/pyams_security_views/api/principal.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/doctests/README.rst` & `pyams_security_views-2.3.1/src/pyams_security_views/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/include.py` & `pyams_security_views-2.3.1/src/pyams_security_views/include.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/interfaces/__init__.py` & `pyams_security_views-2.3.1/src/pyams_security_views/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/interfaces/login.py` & `pyams_security_views-2.3.1/src/pyams_security_views/interfaces/login.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo` & `pyams_security_views-2.3.1/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po` & `pyams_security_views-2.3.1/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/locales/pyams_security_views.pot` & `pyams_security_views-2.3.1/src/pyams_security_views/locales/pyams_security_views.pot`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/login.py` & `pyams_security_views-2.3.1/src/pyams_security_views/login.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/site.py` & `pyams_security_views-2.3.1/src/pyams_security_views/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/skin/__init__.py` & `pyams_security_views-2.3.1/src/pyams_security_views/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/skin/login.py` & `pyams_security_views-2.3.1/src/pyams_security_views/skin/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 class LoginForm(AddForm):
     """Login form"""
 
     prefix = 'login_form.'
     legend = _("Please enter valid credentials")
 
     modal_class = FieldProperty(IModalFullPage['modal_class'])
+    modal_content_class = FieldProperty(IModalFullPage['modal_content_class'])
 
     fields = Fields(ILoginFormFields)
 
     def __init__(self, context, request):
         super().__init__(context, request)
         login_config = ILoginConfiguration(self.request.root)
         apply_skin(self.request, login_config.skin)
```

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/tests/__init__.py` & `pyams_security_views-2.3.1/src/pyams_security_views/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/tests/test_utilsdocs.py` & `pyams_security_views-2.3.1/src/pyams_security_views/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/tests/test_utilsdocstrings.py` & `pyams_security_views-2.3.1/src/pyams_security_views/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/widget/__init__.py` & `pyams_security_views-2.3.1/src/pyams_security_views/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/widget/interfaces.py` & `pyams_security_views-2.3.1/src/pyams_security_views/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/widget/permission.py` & `pyams_security_views-2.3.1/src/pyams_security_views/widget/permission.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/widget/principal.py` & `pyams_security_views-2.3.1/src/pyams_security_views/widget/principal.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/__init__.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/interfaces.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/login.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/login.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/manager.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/notifications.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/notifications.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/__init__.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/admin.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/admin.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/group.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/group.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/interfaces.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/plugin/userfolder.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/plugin/userfolder.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/policy.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/policy.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/rest.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views/zmi/widget.py` & `pyams_security_views-2.3.1/src/pyams_security_views/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views.egg-info/PKG-INFO` & `pyams_security_views-2.3.1/src/pyams_security_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-security-views
-Version: 2.3.0
+Version: 2.3.1
 Summary: Pyramid views for PyAMS_security package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -46,14 +46,18 @@
 interface (based on PyAMS_zmi package), custom widgets and a small Cornice REST API to look for
 principals.
 
 
 Changelog
 =========
 
+2.3.1
+-----
+ - added support for custom modal content CSS class
+
 2.3.0
 -----
  - added property in login configuration to set user registration activation delay
  - updated roles edit form permission
 
 2.2.0
 -----
```

### Comparing `pyams_security_views-2.3.0/src/pyams_security_views.egg-info/SOURCES.txt` & `pyams_security_views-2.3.1/src/pyams_security_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

