# Comparing `tmp/fairchem_demo_ocpapi-0.0.0b0.tar.gz` & `tmp/fairchem_demo_ocpapi-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairchem_demo_ocpapi-0.0.0b0.tar", last modified: Tue May 14 00:01:33 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fairchem_demo_ocpapi-0.0.0b0.tar` & `fairchem_demo_ocpapi-0.0.1b0.tar`

### file list

```diff
@@ -1,11 +1,18 @@
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-14 00:01:33.023428 fairchem_demo_ocpapi-0.0.0b0/
--rw-r--r--   0 lbluque    (501) staff       (20)      208 2024-05-14 00:01:33.022733 fairchem_demo_ocpapi-0.0.0b0/PKG-INFO
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-14 00:01:33.019017 fairchem_demo_ocpapi-0.0.0b0/fairchem/
--rw-r--r--   0 lbluque    (501) staff       (20)        0 2024-05-09 23:33:00.000000 fairchem_demo_ocpapi-0.0.0b0/fairchem/__init__.py
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-14 00:01:33.022202 fairchem_demo_ocpapi-0.0.0b0/fairchem_demo_ocpapi.egg-info/
--rw-r--r--   0 lbluque    (501) staff       (20)      208 2024-05-14 00:01:33.000000 fairchem_demo_ocpapi-0.0.0b0/fairchem_demo_ocpapi.egg-info/PKG-INFO
--rw-r--r--   0 lbluque    (501) staff       (20)      211 2024-05-14 00:01:33.000000 fairchem_demo_ocpapi-0.0.0b0/fairchem_demo_ocpapi.egg-info/SOURCES.txt
--rw-r--r--   0 lbluque    (501) staff       (20)        1 2024-05-14 00:01:33.000000 fairchem_demo_ocpapi-0.0.0b0/fairchem_demo_ocpapi.egg-info/dependency_links.txt
--rw-r--r--   0 lbluque    (501) staff       (20)        9 2024-05-14 00:01:33.000000 fairchem_demo_ocpapi-0.0.0b0/fairchem_demo_ocpapi.egg-info/top_level.txt
--rw-r--r--   0 lbluque    (501) staff       (20)      278 2024-05-14 00:01:27.000000 fairchem_demo_ocpapi-0.0.0b0/pyproject.toml
--rw-r--r--   0 lbluque    (501) staff       (20)       38 2024-05-14 00:01:33.023510 fairchem_demo_ocpapi-0.0.0b0/setup.cfg
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/.isort.cfg
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/LICENSE
+-rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/README.md
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/version.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/__init__.py
+-rw-r--r--   0        0        0    16402 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/client.py
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/models.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/ui.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/__init__.py
+-rw-r--r--   0        0        0    28890 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/adsorbates.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/context.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/filter.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/log.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/retry.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/PKG-INFO
```

