# Comparing `tmp/pywebframework_uz-0.1.0.tar.gz` & `tmp/pywebframework_uz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebframework_uz-0.1.0.tar", last modified: Wed May 15 08:44:52 2024, max compression
+gzip compressed data, was "pywebframework_uz-0.1.1.tar", last modified: Wed May 15 09:13:40 2024, max compression
```

## Comparing `pywebframework_uz-0.1.0.tar` & `pywebframework_uz-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 08:44:52.854667 pywebframework_uz-0.1.0/
--rw-rw-rw-   0        0        0      920 2024-05-15 08:44:52.853944 pywebframework_uz-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 08:44:52.852161 pywebframework_uz-0.1.0/pywebframework_uz.egg-info/
--rw-rw-rw-   0        0        0      920 2024-05-15 08:44:52.000000 pywebframework_uz-0.1.0/pywebframework_uz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-15 08:44:52.000000 pywebframework_uz-0.1.0/pywebframework_uz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 08:44:52.000000 pywebframework_uz-0.1.0/pywebframework_uz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-15 08:44:52.000000 pywebframework_uz-0.1.0/pywebframework_uz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 08:44:52.000000 pywebframework_uz-0.1.0/pywebframework_uz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 08:44:52.854667 pywebframework_uz-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4069 2024-05-15 08:44:39.000000 pywebframework_uz-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:13:40.925589 pywebframework_uz-0.1.1/
+-rw-rw-rw-   0        0        0     4750 2024-05-15 09:13:40.924159 pywebframework_uz-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3878 2024-05-15 09:05:04.000000 pywebframework_uz-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:13:40.921163 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/
+-rw-rw-rw-   0        0        0     4750 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:13:40.925902 pywebframework_uz-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     4069 2024-05-15 09:13:12.000000 pywebframework_uz-0.1.1/setup.py
```

### Comparing `pywebframework_uz-0.1.0/setup.py` & `pywebframework_uz-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pywebframework_uz'
 DESCRIPTION = 'Python web-framework building for learning purpose'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'hojiakbarmadaminov45@gmail.com'
 AUTHOR = 'Madaminov Khojiakbar'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     'requests-wsgi-adapter==0.4.1',
```

