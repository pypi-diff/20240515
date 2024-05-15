# Comparing `tmp/piaas-0.0.1.tar.gz` & `tmp/piaas-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piaas-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "piaas-0.1.tar", last modified: Wed May 15 14:26:59 2024, max compression
```

## Comparing `piaas-0.0.1.tar` & `piaas-0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1926 2024-05-15 16:14:41.133829 piaas-0.0.1/PIaaS/__init__.py
--rw-r--r--   0        0        0      100 2024-05-15 16:14:41.133829 piaas-0.0.1/PIaaS/config.py
--rw-r--r--   0        0        0       96 2024-05-15 16:14:41.137829 piaas-0.0.1/PIaaS/static/css/style.css
--rw-r--r--   0        0        0     1229 2024-05-15 16:14:41.137829 piaas-0.0.1/PIaaS/static/ethernet-port-icon-20.jpeg
--rw-r--r--   0        0        0     4480 2024-05-15 16:14:41.137829 piaas-0.0.1/PIaaS/templates/base.html
--rw-r--r--   0        0        0      814 2024-05-15 16:14:41.137829 piaas-0.0.1/PIaaS/templates/index.html
--rw-r--r--   0        0        0     1774 2024-05-15 16:14:41.137829 piaas-0.0.1/PIaaS/views.py
--rw-r--r--   0        0        0       82 2024-05-15 16:14:41.137829 piaas-0.0.1/README.md
--rw-r--r--   0        0        0      236 2024-05-15 16:14:41.137829 piaas-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      248 1970-01-01 00:00:00.000000 piaas-0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:26:59.265758 piaas-0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:26:59.265758 piaas-0.1/PIaaS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-15 14:26:59.000000 piaas-0.1/PIaaS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 14:26:59.000000 piaas-0.1/PIaaS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:26:59.000000 piaas-0.1/PIaaS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 14:26:59.000000 piaas-0.1/PIaaS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:26:59.000000 piaas-0.1/PIaaS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-15 14:26:59.265758 piaas-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 14:26:53.000000 piaas-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:26:59.265758 piaas-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-15 14:26:53.000000 piaas-0.1/setup.py
```

