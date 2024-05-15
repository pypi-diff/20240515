# Comparing `tmp/sqlalchemy_mate-1.4.28.4.tar.gz` & `tmp/sqlalchemy_mate-2.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mate-1.4.28.4.tar", last modified: Wed Mar 15 20:26:53 2023, max compression
+gzip compressed data, was "sqlalchemy_mate-2.0.0.0.tar", last modified: Wed May 15 06:24:51 2024, max compression
```

## Comparing `sqlalchemy_mate-1.4.28.4.tar` & `sqlalchemy_mate-2.0.0.0.tar`

### file list

```diff
@@ -1,86 +1,57 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.756786 sqlalchemy_mate-1.4.28.4/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2021-12-18 20:54:55.000000 sqlalchemy_mate-1.4.28.4/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1125 2021-12-15 19:53:39.000000 sqlalchemy_mate-1.4.28.4/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      346 2021-12-15 19:53:39.000000 sqlalchemy_mate-1.4.28.4/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)    10156 2023-03-15 20:26:53.756473 sqlalchemy_mate-1.4.28.4/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     9112 2021-12-29 16:50:07.000000 sqlalchemy_mate-1.4.28.4/README.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     4983 2023-03-15 17:19:31.000000 sqlalchemy_mate-1.4.28.4/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      149 2021-12-28 00:47:58.000000 sqlalchemy_mate-1.4.28.4/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      556 2021-12-18 16:38:12.000000 sqlalchemy_mate-1.4.28.4/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      136 2021-12-28 00:48:15.000000 sqlalchemy_mate-1.4.28.4/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       37 2023-03-15 17:18:14.000000 sqlalchemy_mate-1.4.28.4/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-03-15 20:26:53.756849 sqlalchemy_mate-1.4.28.4/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7130 2023-03-15 17:47:33.000000 sqlalchemy_mate-1.4.28.4/setup.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.726400 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/
--rw-r--r--   0 sanhehu    (505) staff       (20)     6148 2022-03-15 21:18:25.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/.DS_Store
--rw-r--r--   0 sanhehu    (505) staff       (20)      686 2021-12-18 16:29:30.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.730545 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__pycache__/
--rw-r--r--   0 sanhehu    (505) staff       (20)      946 2021-12-18 16:38:21.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)      245 2023-03-15 20:26:47.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)    13847 2021-12-18 20:54:05.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__pycache__/engine_creator.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     2182 2021-12-17 19:12:27.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__pycache__/io.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     5806 2021-12-18 20:40:16.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__pycache__/pt.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     3797 2021-12-17 19:06:06.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)      101 2023-03-15 17:18:54.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/_version.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.744761 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/
--rw-r--r--   0 sanhehu    (505) staff       (20)       85 2021-12-15 19:53:39.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.746064 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/__pycache__/
--rw-r--r--   0 sanhehu    (505) staff       (20)      244 2021-12-15 20:06:14.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)      596 2021-12-15 23:43:35.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/__pycache__/deleting.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     2423 2021-12-16 18:43:32.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/__pycache__/inserting.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     6558 2021-12-18 19:01:43.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/__pycache__/selecting.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     3109 2021-12-18 18:56:59.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/__pycache__/updating.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)      351 2021-12-15 23:36:56.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/deleting.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3198 2021-12-16 18:43:09.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/inserting.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     6268 2021-12-18 18:59:58.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/selecting.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3526 2021-12-18 18:52:30.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/updating.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.746233 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2021-12-18 16:36:05.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/docs/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.746607 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/docs/__pycache__/
--rw-r--r--   0 sanhehu    (505) staff       (20)      198 2021-12-18 16:38:48.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/docs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)    14141 2021-12-18 20:54:01.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/engine_creator.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2063 2021-12-17 19:12:24.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/io.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.747240 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/orm/
--rw-r--r--   0 sanhehu    (505) staff       (20)       50 2021-12-15 19:53:39.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/orm/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.747913 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/orm/__pycache__/
--rw-r--r--   0 sanhehu    (505) staff       (20)      208 2021-12-15 20:06:14.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/orm/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)    18729 2021-12-29 17:01:37.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/orm/__pycache__/extended_declarative_base.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)    20440 2021-12-29 16:46:45.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/orm/extended_declarative_base.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.748139 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/
--rw-r--r--   0 sanhehu    (505) staff       (20)       46 2021-12-15 19:53:39.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.748465 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/__pycache__/
--rw-r--r--   0 sanhehu    (505) staff       (20)      178 2021-12-15 20:06:14.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.748871 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/timeout_decorator/
--rw-r--r--   0 sanhehu    (505) staff       (20)      162 2021-12-15 19:53:39.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/timeout_decorator/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.749481 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/timeout_decorator/__pycache__/
--rw-r--r--   0 sanhehu    (505) staff       (20)      328 2021-12-15 20:06:14.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/timeout_decorator/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     6258 2021-12-15 20:06:14.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/timeout_decorator/__pycache__/timeout_decorator.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     6411 2021-12-15 19:53:39.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/timeout_decorator/timeout_decorator.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     6093 2021-12-18 20:40:15.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pt.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.749655 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)     5187 2021-12-28 00:49:04.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/tests/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.749974 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/tests/__pycache__/
--rw-r--r--   0 sanhehu    (505) staff       (20)     5825 2021-12-28 00:49:28.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/tests/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.751241 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/
--rw-r--r--   0 sanhehu    (505) staff       (20)      192 2021-12-29 16:55:40.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/__init__.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.753113 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/__pycache__/
--rw-r--r--   0 sanhehu    (505) staff       (20)      386 2021-12-29 17:01:36.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     2985 2021-12-29 18:36:33.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/__pycache__/compressed.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     3071 2021-12-29 18:36:33.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/__pycache__/compressed_json.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     2838 2021-12-29 18:36:33.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/__pycache__/json_serializable.cpython-38.pyc
--rw-r--r--   0 sanhehu    (505) staff       (20)     1931 2021-12-29 18:35:02.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/compressed.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2565 2021-12-29 18:35:45.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/compressed_json.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2453 2021-12-29 18:35:39.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/json_serializable.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3478 2021-12-17 19:02:27.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/utils.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.727523 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)    10156 2023-03-15 20:26:53.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     2546 2023-03-15 20:26:53.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-03-15 20:26:53.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      238 2023-03-15 20:26:53.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       16 2023-03-15 20:26:53.000000 sqlalchemy_mate-1.4.28.4/sqlalchemy_mate.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-15 20:26:53.755960 sqlalchemy_mate-1.4.28.4/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)     3003 2021-12-15 19:53:39.000000 sqlalchemy_mate-1.4.28.4/tests/test_engine_creator.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      475 2021-12-17 18:56:15.000000 sqlalchemy_mate-1.4.28.4/tests/test_import.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1308 2021-12-17 19:12:46.000000 sqlalchemy_mate-1.4.28.4/tests/test_io.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5877 2021-12-18 20:38:14.000000 sqlalchemy_mate-1.4.28.4/tests/test_pt.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1591 2021-12-28 00:49:18.000000 sqlalchemy_mate-1.4.28.4/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.073165 sqlalchemy_mate-2.0.0.0/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      356 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11668 2024-05-15 06:24:51.072941 sqlalchemy_mate-2.0.0.0/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9672 2024-05-15 06:12:00.000000 sqlalchemy_mate-2.0.0.0/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6707 2024-05-15 06:13:01.000000 sqlalchemy_mate-2.0.0.0/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      390 2024-05-14 20:30:28.000000 sqlalchemy_mate-2.0.0.0/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      871 2024-05-14 20:26:57.000000 sqlalchemy_mate-2.0.0.0/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/requirements-furo-sphinx-search.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2024-05-14 20:27:06.000000 sqlalchemy_mate-2.0.0.0/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       51 2024-05-14 20:57:38.000000 sqlalchemy_mate-2.0.0.0/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-05-15 06:24:51.073209 sqlalchemy_mate-2.0.0.0/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7479 2024-05-15 05:55:50.000000 sqlalchemy_mate-2.0.0.0/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.065862 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      803 2024-05-15 05:36:41.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      100 2024-05-15 06:02:49.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.067817 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       85 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      343 2024-05-15 05:07:50.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/deleting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3332 2024-05-15 04:37:22.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/inserting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6145 2024-05-15 05:01:17.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/selecting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3686 2024-05-15 05:07:15.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/updating.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.068067 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    14141 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/engine_creator.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2173 2024-05-14 21:20:06.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/io.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.068518 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/orm/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       50 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/orm/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    20444 2024-05-15 05:18:28.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/orm/extended_declarative_base.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5917 2024-05-15 04:01:42.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/pt.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.069299 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      192 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1931 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/compressed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2565 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/compressed_json.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2453 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/json_serializable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3476 2024-05-15 05:11:24.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.069674 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.070054 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/timeout_decorator/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      162 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/timeout_decorator/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6411 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.071708 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11668 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1331 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      291 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.071420 sqlalchemy_mate-2.0.0.0/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3190 2024-05-15 04:08:44.000000 sqlalchemy_mate-2.0.0.0/tests/test_engine_creator.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1051 2024-05-15 05:38:39.000000 sqlalchemy_mate-2.0.0.0/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1308 2024-05-14 21:00:03.000000 sqlalchemy_mate-2.0.0.0/tests/test_io.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6352 2024-05-15 03:57:04.000000 sqlalchemy_mate-2.0.0.0/tests/test_pt.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1527 2024-05-15 04:08:55.000000 sqlalchemy_mate-2.0.0.0/tests/test_utils.py
```

### Comparing `sqlalchemy_mate-1.4.28.4/LICENSE.txt` & `sqlalchemy_mate-2.0.0.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright 2018 Sanhe Hu <https://github.com/MacHu-GWU/sqlalchemy_mate-project>
+Copyright 2023 Sanhe Hu <https://github.com/MacHu-GWU/sqlalchemy_mate-project>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `sqlalchemy_mate-1.4.28.4/PKG-INFO` & `sqlalchemy_mate-2.0.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_mate
-Version: 1.4.28.4
+Version: 2.0.0.0
 Summary: A library extend sqlalchemy module, makes CRUD easier.
 Home-page: https://github.com/MacHu-GWU/sqlalchemy_mate-project
-Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/1.4.28.4#downloads
+Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.0#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -15,56 +15,79 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: tests
-Provides-Extra: docs
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
+Requires-Dist: sqlalchemy<3.0.0,>=2.0.0
+Requires-Dist: prettytable<4.0.0,>=3.0.0
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pg8000; extra == "tests"
+Requires-Dist: attrs; extra == "tests"
+Requires-Dist: superjson; extra == "tests"
+Requires-Dist: pandas; extra == "tests"
+Provides-Extra: docs
+Requires-Dist: Sphinx==5.3.0; extra == "docs"
+Requires-Dist: sphinx-jinja==2.0.2; extra == "docs"
+Requires-Dist: sphinx-copybutton==0.5.1; extra == "docs"
+Requires-Dist: sphinx-design==0.5.0; extra == "docs"
+Requires-Dist: furo==2023.03.27; extra == "docs"
+Requires-Dist: nbsphinx==0.8.12; extra == "docs"
+Requires-Dist: rstobj==1.2.1; extra == "docs"
+Requires-Dist: pygments==2.15.1; extra == "docs"
+Requires-Dist: ipython==8.10.0; extra == "docs"
+Requires-Dist: docfly==2.0.3; extra == "docs"
 
 .. image:: https://readthedocs.org/projects/sqlalchemy_mate/badge/?version=latest
-    :target: https://sqlalchemy_mate.readthedocs.io/index.html
+    :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
     :alt: Documentation Status
 
-.. image:: https://github.com/MacHu-GWU/sqlalchemy_mate-project/workflows/CI/badge.svg
+.. image:: https://github.com/MacHu-GWU/sqlalchemy_mate-project/actions/workflows/main.yml/badge.svg
     :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/sqlalchemy_mate-project/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/MacHu-GWU/sqlalchemy_mate-project
 
 .. image:: https://img.shields.io/pypi/v/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
 .. image:: https://img.shields.io/pypi/l/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project/blob/master/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project
 
 ------
 
-
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/index.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/py-modindex.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/py-modindex.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
       :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
       :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project
 
@@ -76,30 +99,32 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
       :target: https://pypi.org/pypi/sqlalchemy_mate#files
 
 
 Welcome to ``sqlalchemy_mate`` Documentation
 ==============================================================================
-
 A sweet syntax sugar library simplify your in writing ``sqlalchemy`` code.
 
+📔 `Full document is HERE <https://sqlalchemy-mate.readthedocs.io/latest/index.html>`_
+
+.. image:: https://sqlalchemy-mate.readthedocs.io/latest/_static/sqlalchemy_mate-logo.png
+    :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
+
 
 Features
 ------------------------------------------------------------------------------
-
 .. contents::
     :class: this-will-duplicate-information-and-it-is-still-useful-here
     :depth: 1
     :local:
 
 
 Read Database Credential Safely
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 .. contents::
     :class: this-will-duplicate-information-and-it-is-still-useful-here
     :depth: 1
     :local:
 
 Put your database connection credential in your source code is always a **BAD IDEA**.
 
@@ -241,24 +266,25 @@
     # leave aws_profile=None if you are on cloud
     ec = EngineCreator.from_env(prefix="DB_DEV", kms_decrypt=True, aws_profile="xxx")
     engine = ec.create_redshift()
 
 
 Smart Insert
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 In bulk insert, if there are some rows having primary_key conflict, the classic solution is:
 
 .. code-block:: python
 
-    for row in data:
-        try:
-            engine.execute(table.insert(), row)
-        except sqlalchemy.sql.IntegrityError:
-            pass
+    with engine.connect() as conn:
+        for row in data:
+            try:
+                conn.execute(table.insert(), row)
+                conn.commit()
+            except sqlalchemy.exc.IntegrityError:
+                conn.rollback()
 
 It is like one-by-one insert, which is super slow.
 
 ``sqlalchemy_mate`` uses ``smart_insert`` strategy to try with smaller bulk insert, which has higher probabily to work. As a result, total number of commits are greatly reduced.
 
 With sql expression:
 
@@ -311,15 +337,14 @@
     User.upsert_all(engine_or_session, user_list)
 
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
-
 ``sqlalchemy_mate`` is released on PyPI, so all you need is:
 
 .. code-block:: console
 
     $ pip install sqlalchemy_mate
 
 To upgrade to latest version:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sqlalchemy_mate-1.4.28.4/README.rst` & `sqlalchemy_mate-2.0.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 .. image:: https://readthedocs.org/projects/sqlalchemy_mate/badge/?version=latest
-    :target: https://sqlalchemy_mate.readthedocs.io/index.html
+    :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
     :alt: Documentation Status
 
-.. image:: https://github.com/MacHu-GWU/sqlalchemy_mate-project/workflows/CI/badge.svg
+.. image:: https://github.com/MacHu-GWU/sqlalchemy_mate-project/actions/workflows/main.yml/badge.svg
     :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/sqlalchemy_mate-project/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/MacHu-GWU/sqlalchemy_mate-project
 
 .. image:: https://img.shields.io/pypi/v/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
 .. image:: https://img.shields.io/pypi/l/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project/blob/master/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project
 
 ------
 
-
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/index.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/py-modindex.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/py-modindex.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
       :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
       :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project
 
@@ -46,30 +48,32 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
       :target: https://pypi.org/pypi/sqlalchemy_mate#files
 
 
 Welcome to ``sqlalchemy_mate`` Documentation
 ==============================================================================
-
 A sweet syntax sugar library simplify your in writing ``sqlalchemy`` code.
 
+📔 `Full document is HERE <https://sqlalchemy-mate.readthedocs.io/latest/index.html>`_
+
+.. image:: https://sqlalchemy-mate.readthedocs.io/latest/_static/sqlalchemy_mate-logo.png
+    :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
+
 
 Features
 ------------------------------------------------------------------------------
-
 .. contents::
     :class: this-will-duplicate-information-and-it-is-still-useful-here
     :depth: 1
     :local:
 
 
 Read Database Credential Safely
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 .. contents::
     :class: this-will-duplicate-information-and-it-is-still-useful-here
     :depth: 1
     :local:
 
 Put your database connection credential in your source code is always a **BAD IDEA**.
 
@@ -211,24 +215,25 @@
     # leave aws_profile=None if you are on cloud
     ec = EngineCreator.from_env(prefix="DB_DEV", kms_decrypt=True, aws_profile="xxx")
     engine = ec.create_redshift()
 
 
 Smart Insert
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 In bulk insert, if there are some rows having primary_key conflict, the classic solution is:
 
 .. code-block:: python
 
-    for row in data:
-        try:
-            engine.execute(table.insert(), row)
-        except sqlalchemy.sql.IntegrityError:
-            pass
+    with engine.connect() as conn:
+        for row in data:
+            try:
+                conn.execute(table.insert(), row)
+                conn.commit()
+            except sqlalchemy.exc.IntegrityError:
+                conn.rollback()
 
 It is like one-by-one insert, which is super slow.
 
 ``sqlalchemy_mate`` uses ``smart_insert`` strategy to try with smaller bulk insert, which has higher probabily to work. As a result, total number of commits are greatly reduced.
 
 With sql expression:
 
@@ -281,15 +286,14 @@
     User.upsert_all(engine_or_session, user_list)
 
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
-
 ``sqlalchemy_mate`` is released on PyPI, so all you need is:
 
 .. code-block:: console
 
     $ pip install sqlalchemy_mate
 
 To upgrade to latest version:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sqlalchemy_mate-1.4.28.4/release-history.rst` & `sqlalchemy_mate-2.0.0.0/release-history.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 .. _release_history:
 
 Release and Version History
-===========================
+==============================================================================
 
 
 Backlog (TODO)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+2.0.0.0 (TODO)
+------------------------------------------------------------------------------
+**💥Breaking Change**
+
+- From ``sqlalchemy_mate>=2.0.0.0``, it only support ``sqlalchemy>=2.0.0`` and only compatible with sqlalchemy 2.X API. Everything marked as ``no longer supported`` or ``no longer accepted`` in `SQLAlchemy 2.0 - Major Migration Guide <https://docs.sqlalchemy.org/en/20/changelog/migration_20.html#migration-core-connection-transaction>`_ document will no longer be supported from this version.
+- Drop Python3.7 support.
+
+**Features and Improvements**
+
+- Fully adapt sqlalchemy 2.X API.
+
+**Minor Improvements**
+
+- Migrate to `cookiecutter-pyproject v4 <https://github.com/MacHu-GWU/cookiecutter-pyproject/releases/tag/v4>`_ code skeleton.
+
+
 1.4.28.4 (2023-03-15)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Bugfixes**
 
 - fix a syntax bug in ``requirements.txt``
 
 
 1.4.28.3 (2021-12-29)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - add ``sqlalchemy_mate.types.JSONSerializableType``
 - add ``sqlalchemy_mate.types.CompressedStringType``
 - add ``sqlalchemy_mate.types.CompressedBinaryType``
 - add ``sqlalchemy_mate.ExtendedBase.select_all`` method
 
 **Bugfixes**
 
 - Fix the underlying implementation type for ``sqlalchemy_mate.types.CompressedJSONType``
 
 
 1.4.28.2 (2021-12-18)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - add ``sqlalchemy_mate.types.CompressedJSONType`` column type.
 - add ``sqlalchemy_mate.selecting.by_pk`` function.
 
 
 1.4.28.1 (2021-12-17)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - fully migrate to ``sqlalchemy`` 1.4+ 2.0 styled API, dropped < 1.3 API support
 - maintain a big version number compatability with Sqlalchemy, won't be responsible to be compatible with different major version. For example, ``sqlalchemy_mate==1.4.x`` maintain compatibility to ``sqlalchemy>=1.4.0,<1.5.0``.
 
 
 0.0.11 (2020-12-05)
-~~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - ``ExtendedBase.by_id`` is renamed to ``ExtendedBase.by_pk``. The old method name is kept for backward API compatibility.
 - add ``ExtendedBase.pk_fields`` method
 - refact ``ExtendedBase.update_all`` method, allow working with session
 
 **Minor Improvements**
@@ -69,22 +85,22 @@
 
 **Miscellaneous**
 
 - use in-package timeout_decorator library to ensure api compatibility
 
 
 0.0.10 (2019-04-26)
-~~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Minor Improvements**
 
-add type hint
+add type hint.
 
 
 0.0.9 (2019-04-26)
-~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - pretty table ``from_everything`` now support textual sql
 - add ``ExtendedBase.random()`` method
 
 **Minor Improvements**
 
@@ -95,75 +111,74 @@
 
 **Miscellaneous**
 
 - include type hint!
 
 
 0.0.8 (2019-03-04)
-~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Bugfixes**
 
 - fix import error in ``Credential.from_env`` with AWS KMS.
 
 **Miscellaneous**
 
 - allow ``EngineCreator`` to return sqlalchemy connect string.
 - improved docs
 
 
 0.0.7 (2019-03-02)
-~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - add ``test_connection(engine, timeout=3)`` function.
 - integrate ``Credential.from_env`` with AWS Key management Service.
 
 **Miscellaneous**
 
 - Deprecating ``sqlalchemy_mate.engine_creator``
 
 
 0.0.6 (2019-03-02)
-~~~~~~~~~~~~~~~~~~
-
+------------------------------------------------------------------------------
 **Bugfixes**
 
 - add ``import boto3`` in ``Credential.from_s3_json()``
 
 
 0.0.5 (2019-03-01)
-~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - ``ExtendedBase.keys()`` now is a class method.
 - ``ExtendedBase.glance()`` can print major attributes and values.
 - **A New DB Credential reader** ``from sqlalchemy_mate import Credential, EngineCreator``
 
 **Minor Improvements**
 
 - change ``FromClause.count()`` -> ``func.count()``, since previous one will be deprecated soon in sqlalchemy.
 
 
 0.0.4 (2018-08-11)
-~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - add ``ExtendedBase.pk_names``, ``ExtendedBase.id_field_name``, ``ExtendedBase.by_id``, ``ExtendedBase.by_sql``, ``ExtendedBase.update_all``, ``ExtendedBase.upsert_all``.
 
 **Minor Improvements**
 
 - use ``pygitrepo==0.0.21``
 
 **Miscellaneous**
 
 - Now ``ExtendedBase.smart_insert`` method returns number of insertion operation. So you can see the difference now.
 
 
 0.0.3 (2018-07-22)
-~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - add a ``ExtendedBase`` class to give orm Declaritive Base more useful method.
 - add a new method performs ``smart_insert`` in orm. It is 10 times faster in average than one by one insert. Can do bulk insert even there is a ``IntegrityError``.
 - add a new ``engine_creator`` module to quickly create engines.
 
 **Minor Improvements**
@@ -179,25 +194,25 @@
 
 - improve testing coverage from 60% to 100%.
 - add unittest for import.
 - add documentation site.
 
 
 0.0.2 (2018-07-03)
-~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 **Features and Improvements**
 
 - add more function can create PrettyTable from orm query, orm object, sql statement, table.
 
 **Minor Improvements**
 
 **Bugfixes**
 
 - fix a bug that sometimes prettytable using bytes str for column name, now it ensures unicode str.
 
 **Miscellaneous**
 
 
 0.0.1 (2017-06-15)
-~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------
 - First release
-- Add ``insert``, ``select``, ``update``, ``io``, ``pt`` module.
+- Add ``insert``, ``select``, ``update``, ``io``, ``pt`` module.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sqlalchemy_mate-1.4.28.4/setup.py` & `sqlalchemy_mate-2.0.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,18 @@
     PACKAGES, INCLUDE_PACKAGE_DATA, PACKAGE_DATA, PY_MODULES = (
         None, None, None, None,
     )
 
     # It's a directory style package
     if os.path.exists(__file__[:-8] + PKG_NAME):
         # Include all sub packages in package directory
-        PACKAGES = [PKG_NAME] + ["%s.%s" % (PKG_NAME, i)
-                                 for i in find_packages(PKG_NAME)]
+        PACKAGES = [PKG_NAME] + [
+            "%s.%s" % (PKG_NAME, i)
+            for i in find_packages(PKG_NAME)
+        ]
 
         # Include everything in package directory
         INCLUDE_PACKAGE_DATA = True
         PACKAGE_DATA = {
             "": ["*.*"],
         }
 
@@ -114,18 +116,20 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3 :: Only",
     ]
     """
     Full list can be found at: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     """
 
 
     def read_requirements_file(path):
@@ -155,15 +159,15 @@
         EXTRA_REQUIRE["tests"] = read_requirements_file("requirements-test.txt")
     except:
         print("'requirements-test.txt' not found!")
 
     try:
         EXTRA_REQUIRE["docs"] = read_requirements_file("requirements-doc.txt")
     except:
-        print("'requirements-test.txt' not found!")
+        print("'requirements-doc.txt' not found!")
 
     setup(
         name=PKG_NAME,
         description=SHORT_DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         version=VERSION,
         author=AUTHOR,
@@ -175,62 +179,64 @@
         package_data=PACKAGE_DATA,
         py_modules=PY_MODULES,
         url=URL,
         download_url=DOWNLOAD_URL,
         classifiers=CLASSIFIERS,
         platforms=PLATFORMS,
         license=LICENSE,
+        python_requires=">=3.8",
         install_requires=REQUIRES,
         extras_require=EXTRA_REQUIRE,
     )
 
 """
 Appendix
 --------
-::
+Frequent used classifiers List::
+
+    [
+        "Development Status :: 1 - Planning",
+        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 6 - Mature",
+        "Development Status :: 7 - Inactive",
+
+        "Intended Audience :: Customer Service",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Education",
+        "Intended Audience :: End Users/Desktop",
+        "Intended Audience :: Financial and Insurance Industry",
+        "Intended Audience :: Healthcare Industry",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: Legal Industry",
+        "Intended Audience :: Manufacturing",
+        "Intended Audience :: Other Audience",
+        "Intended Audience :: Religion",
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: System Administrators",
+        "Intended Audience :: Telecommunications Industry",
+
+        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: BSD License",
+        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: GNU General Public License (GPL)",
+        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+
+        "Natural Language :: English",
+        "Natural Language :: Chinese (Simplified)",
 
-Frequent used classifiers List = [
-    "Development Status :: 1 - Planning",
-    "Development Status :: 2 - Pre-Alpha",
-    "Development Status :: 3 - Alpha",
-    "Development Status :: 4 - Beta",
-    "Development Status :: 5 - Production/Stable",
-    "Development Status :: 6 - Mature",
-    "Development Status :: 7 - Inactive",
-
-    "Intended Audience :: Customer Service",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Education",
-    "Intended Audience :: End Users/Desktop",
-    "Intended Audience :: Financial and Insurance Industry",
-    "Intended Audience :: Healthcare Industry",
-    "Intended Audience :: Information Technology",
-    "Intended Audience :: Legal Industry",
-    "Intended Audience :: Manufacturing",
-    "Intended Audience :: Other Audience",
-    "Intended Audience :: Religion",
-    "Intended Audience :: Science/Research",
-    "Intended Audience :: System Administrators",
-    "Intended Audience :: Telecommunications Industry",
-
-    "License :: OSI Approved :: MIT License",
-    "License :: OSI Approved :: BSD License",
-    "License :: OSI Approved :: Apache Software License",
-    "License :: OSI Approved :: GNU General Public License (GPL)",
-    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
-
-    "Natural Language :: English",
-    "Natural Language :: Chinese (Simplified)",
-
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: MacOS",
-    "Operating System :: Unix",
-
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3 :: Only",
-]
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS",
+        "Operating System :: Unix",
+
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3 :: Only",
+    ]
 """
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/__init__.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,23 @@
 __license__ = "MIT"
 __author__ = "Sanhe Hu"
 __author_email__ = "husanhe@gmail.com"
 __github_username__ = "MacHu-GWU"
 
 
 try:
-    from . import engine_creator, io, pt, types
+    from . import engine_creator
+    from . import io
+    from . import pt
+    from . import types
     from .utils import test_connection
     from .engine_creator import EngineCreator
-    from .crud import selecting, inserting, updating, deleting
+    from .crud import selecting
+    from .crud import inserting
+    from .crud import updating
+    from .crud import deleting
     from .orm.extended_declarative_base import ExtendedBase
-    from .pkg.timeout_decorator import TimeoutError
+    from .vendor.timeout_decorator import TimeoutError
 except ImportError as e:  # pragma: no cover
     print(e)
 except Exception as e:  # pragma: no cover
     raise e
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/inserting.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/inserting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 
 """
 This module provide utility functions for insert operation.
 """
 
+import typing as T
 import math
-from typing import Union, List, Tuple
-from sqlalchemy import Table
-from sqlalchemy.engine import Engine, Connection
+
+import sqlalchemy as sa
 from sqlalchemy.exc import IntegrityError
 
 from ..utils import grouper_list
 
 
 def smart_insert(
-    engine: Engine,
-    table: Table,
-    data: Union[dict, List[dict]],
+    engine: sa.Engine,
+    table: sa.Table,
+    data: T.Union[dict, T.List[dict]],
     minimal_size: int = 5,
-    _connection: Connection = None,
+    _connection: sa.Connection = None,
     _op_counter: int = 0,
     _ins_counter: int = 0,
     _is_first_call: bool = True,
-) -> Tuple[int, int]:
+) -> T.Tuple[int, int]:
     """
     An optimized Insert strategy. Guarantee successful and highest insertion
     speed. But ATOMIC WRITE IS NOT ENSURED IF THE PROGRAM IS INTERRUPTED.
 
     :return: number of successful INSERT sql execution; number of inserted rows.
 
     **中文文档**
@@ -44,51 +44,55 @@
     """
     if _connection is None:
         _connection = engine.connect()
 
     insert = table.insert()
 
     if isinstance(data, list):
-        # 首先进行尝试bulk insert
+        # 首先进行尝试 bulk insert
         try:
             _connection.execute(insert, data)
+            _connection.commit()
             _op_counter += 1
             _ins_counter += len(data)
         # 失败了
         except IntegrityError:
+            _connection.rollback()
             # 分析数据量
             n = len(data)
             # 如果数据条数多于一定数量
-            if n >= minimal_size ** 2:
+            if n >= minimal_size**2:
                 # 则进行分包
                 n_chunk = math.floor(math.sqrt(n))
                 for chunk in grouper_list(data, n_chunk):
                     _op_counter, _ins_counter = smart_insert(
                         engine=engine,
                         table=table,
                         data=chunk,
                         minimal_size=minimal_size,
                         _connection=_connection,
                         _op_counter=_op_counter,
                         _ins_counter=_ins_counter,
-                        _is_first_call=False
+                        _is_first_call=False,
                     )
             # 否则则一条条地逐条插入
             else:
                 for row in data:
                     try:
-                        _connection.execute(insert, row)
+                        _connection.execute(insert.values(**row))
+                        _connection.commit()
                         _op_counter += 1
                         _ins_counter += 1
                     except IntegrityError:
-                        pass
+                        _connection.rollback()
     else:
         try:
             _connection.execute(insert, data)
+            _connection.commit()
             _op_counter += 1
             _ins_counter += 1
         except IntegrityError:
-            pass
+            _connection.rollback()
 
     if _is_first_call:
         _connection.close()
     return _op_counter, _ins_counter
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/selecting.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/selecting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 
 """
 This module provide utility functions for select operation.
 """
 
-from typing import List, Union, Iterable
-from sqlalchemy import select, func, Column, Table, and_
-from sqlalchemy.engine import Engine, Result, Row
+import typing as T
+
+import sqlalchemy as sa
+
 from ..utils import ensure_exact_one_arg_is_not_none
 
 
 def count_row(
-    engine: Engine,
-    table: Table,
+    engine: sa.Engine,
+    table: sa.Table,
 ) -> int:
     """
     Return number of rows in a table.
 
     Example::
 
         import sqlalchemy as sa
@@ -28,23 +29,23 @@
 
     **中文文档**
 
     返回一个表中的行数。
     """
     with engine.connect() as connection:
         return connection.execute(
-            select([func.count()]).select_from(table)
+            sa.select(sa.func.count()).select_from(table)
         ).fetchone()[0]
 
 
 def by_pk(
-    engine: Engine,
-    table: Table,
+    engine: sa.Engine,
+    table: sa.Table,
     id_,
-) -> Union[Row, None]:
+) -> T.Union[sa.Row, None]:
     """
     Return single row or None by primary key values.
 
     :param id_: single value if table has only one primary key, tuple / list of
         values if table has multiple primary keys, positioning is sensitive.
 
     Example::
@@ -66,113 +67,112 @@
     with engine.connect() as connection:
         if isinstance(id_, (tuple, list)):
             if len(id_) != len(table.primary_key):
                 raise ValueError
             where_args = list()
             for column, value in zip(table.primary_key, id_):
                 where_args.append(column == value)
-            return connection.execute(
-                select(table).where(and_(*where_args))
-            ).fetchone()
+            stmt = sa.select(table).where(sa.and_(*where_args))
+            return connection.execute(stmt).fetchone()
         else:
             if len(table.primary_key) != 1:
                 raise ValueError
             return connection.execute(
-                select(table).where(list(table.primary_key)[0] == id_)
+                sa.select(table).where(list(table.primary_key)[0] == id_)
             ).fetchone()
 
 
 def select_all(
-    engine: Engine,
-    table: Table,
-) -> Result:
+    engine: sa.Engine,
+    table: sa.Table,
+) -> sa.Result:
     """
     Select all rows from a table.
 
     Example::
 
         for row in sam.selecting.select_all(engine, t_users):
             ...
     """
-    s = select([table])
+    s = sa.select(table)
     with engine.connect() as connection:
         return connection.execute(s)
 
 
 def select_single_column(
-    engine: Engine,
-    column: Column,
+    engine: sa.Engine,
+    column: sa.Column,
 ) -> list:
     """
     Select data from single column.
 
     Example::
 
         id_list = sam.selecting.select_all(engine, t_users.c.id)
     """
-    s = select([column])
+    s = sa.select(column)
     with engine.connect() as connection:
         return [row[0] for row in connection.execute(s)]
 
 
 def select_many_column(
-    engine: Engine,
-    columns: List[Column],
-) -> List[tuple]:
+    engine: sa.Engine,
+    columns: T.List[sa.Column],
+) -> T.List[tuple]:
     """
     Select data from multiple columns.
 
     Example::
 
         dataframe = sam.selecting.select_all(engine, [t_users.c.id, t_users.c.name])
     """
-    s = select(columns)
+    s = sa.select(*columns)
     with engine.connect() as connection:
         return [tuple(row) for row in connection.execute(s)]
 
 
 def select_single_distinct(
-    engine: Engine,
-    column: Column,
+    engine: sa.Engine,
+    column: sa.Column,
 ) -> list:
     """
     Select distinct data from single column.
 
     Example::
 
         unique_name_list = sam.selecting.select_all(engine, t_users.c.name)
     """
-    s = select([column]).distinct()
+    s = sa.select(column).distinct()
     with engine.connect() as connection:
         return [row[0] for row in connection.execute(s)]
 
 
 def select_many_distinct(
-    engine: Engine,
-    columns: List[Column],
-) -> List[tuple]:
+    engine: sa.Engine,
+    columns: T.List[sa.Column],
+) -> T.List[tuple]:
     """
     Select distinct data from multiple columns.
 
     Example::
 
         dataframe = sam.selecting.select_many_distinct(engine, [t_users.c.id, t_users.c.name])
     """
-    s = select(columns).distinct()
+    s = sa.select(*columns).distinct()
     with engine.connect() as connection:
         return [tuple(row) for row in connection.execute(s)]
 
 
 def select_random(
-    engine: Engine,
-    table: Table = None,
-    columns: List[Column] = None,
+    engine: sa.Engine,
+    table: sa.Table = None,
+    columns: T.List[sa.Column] = None,
     limit: int = None,
-    perc: int = None
-) -> Result:
+    perc: int = None,
+) -> sa.Result:
     """
     Randomly select some rows from table.
 
     :param perc: int from 1 ~ 99. (means 1% ~ 99%)
 
     Example::
 
@@ -185,59 +185,49 @@
             ...
     """
     ensure_exact_one_arg_is_not_none(limit, perc)
     ensure_exact_one_arg_is_not_none(table, columns)
 
     if table is not None:
         if limit is not None:
-            stmt = select(table).order_by(func.random()).limit(limit)
+            stmt = sa.select(table).order_by(sa.func.random()).limit(limit)
         else:
             if perc >= 100 or perc <= 0:
                 raise ValueError
 
             selectable = table.tablesample(
-                func.bernoulli(perc),
-                name="alias",
-                seed=func.random()
+                sa.func.bernoulli(perc), name="alias", seed=sa.func.random()
             )
-            args = [
-                getattr(selectable.c, column.name)
-                for column in table.columns
-            ]
-            stmt = select(*args)
+            args = [getattr(selectable.c, column.name) for column in table.columns]
+            stmt = sa.select(*args)
     elif columns is not None:
         if limit is not None:
-            stmt = select(columns).order_by(func.random()).limit(limit)
+            stmt = sa.select(*columns).order_by(sa.func.random()).limit(limit)
         else:
             if perc >= 100 or perc <= 0:
                 raise ValueError
             selectable = columns[0].table.tablesample(
-                func.bernoulli(perc),
-                name="alias",
-                seed=func.random()
+                sa.func.bernoulli(perc), name="alias", seed=sa.func.random()
             )
-            args = [
-                getattr(selectable.c, column.name)
-                for column in columns
-            ]
-            stmt = select(*args)
+            args = [getattr(selectable.c, column.name) for column in columns]
+            stmt = sa.select(*args)
     else:  # pragma: no cover, for readability only
         raise NotImplementedError
 
     with engine.connect() as connection:
         return connection.execute(stmt)
 
 
-def yield_tuple(result: Result) -> Iterable[tuple]:
+def yield_tuple(result: sa.Result) -> T.Iterable[tuple]:
     """
     Yield rows in tuple values view.
     """
     for row in result:
         yield tuple(row)
 
 
-def yield_dict(result: Result) -> Iterable[dict]:
+def yield_dict(result: sa.Result) -> T.Iterable[dict]:
     """
     Yield rows in dict view.
     """
     for row in result:
-        yield dict(row)
+        yield row._asdict()
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/crud/updating.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/updating.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # -*- coding: utf-8 -*-
 
 """
 This module provide utility functions for update operation.
 """
 
-from typing import Union, List, Tuple, Dict, Any
+# from typing import Union, List, Tuple, Dict, Any
+import typing as T
 from collections import OrderedDict
-from sqlalchemy import and_
-from sqlalchemy import Table
-from sqlalchemy.engine import Engine
+
+import sqlalchemy as sa
+
+# from sqlalchemy import and_
+# from sqlalchemy import Table
+# from sqlalchemy.engine import Engine
 
 from ..utils import ensure_list
 
 
 def update_all(
-    engine: Engine,
-    table: Table,
-    data: Union[Dict[str, Any], List[Dict[str, Any]]],
+    engine: sa.Engine,
+    table: sa.Table,
+    data: T.Union[T.Dict[str, T.Any], T.List[T.Dict[str, T.Any]]],
     upsert=False,
-) -> Tuple[int, int]:
+) -> T.Tuple[int, int]:
     """
     Update data by its primary_key column values. By default upsert is False.
     """
     with engine.connect() as connection:
         update_counter = 0
         insert_counter = 0
 
@@ -38,54 +42,55 @@
                 pk_cols[column.name] = column
 
         data_to_insert = list()
 
         # Multiple primary key column
         if len(pk_cols) >= 2:
             for row in data:
-                result = engine.execute(
+                result = connection.execute(
                     upd.where(
-                        and_(
-                            *[col == row[name] for name, col in pk_cols.items()]
-                        )
+                        sa.and_(*[col == row[name] for name, col in pk_cols.items()])
                     ).values(**row)
                 )
+                connection.commit()
                 if result.rowcount == 0:
                     data_to_insert.append(row)
                 else:
                     update_counter += 1
         # Single primary key column
         elif len(pk_cols) == 1:
             for row in data:
-                result = engine.execute(
+                result = connection.execute(
                     upd.where(
                         [col == row[name] for name, col in pk_cols.items()][0]
                     ).values(**row)
                 )
+                connection.commit()
                 if result.rowcount == 0:
                     data_to_insert.append(row)
                 else:
                     update_counter += 1
         else:  # pragma: no cover
             data_to_insert = data
 
         # Insert rest of data
         if upsert:
             if len(data_to_insert):
-                engine.execute(ins, data_to_insert)
+                connection.execute(ins, data_to_insert)
+                connection.commit()
                 insert_counter += len(data_to_insert)
 
         return update_counter, insert_counter
 
 
 def upsert_all(
-    engine: Engine,
-    table: Table,
-    data: Union[Dict[str, Any], List[Dict[str, Any]]],
-) -> Tuple[int, int]:
+    engine: sa.Engine,
+    table: sa.Table,
+    data: T.Union[T.Dict[str, T.Any], T.List[T.Dict[str, T.Any]]],
+) -> T.Tuple[int, int]:
     """
     Update data by primary key columns. If not able to update, do insert.
 
     Example::
 
         # define data model
         t_user = Table(
@@ -101,15 +106,15 @@
         ]
         update_count, insert_count = upsert_all(engine, t_user, data)
         print(update_count) # number of row updated counter
         print(insert_count) # number of row inserted counter
 
         # will return: [{"id": 1, "name": "Bob"}, {"id": 2, "name": "Cathy"}]
         with engine.connect() as connection:
-            print(connection.execute(select([table_user])).all())
+            print(connection.execute(select(table_user)).all())
 
     **中文文档**
 
     批量更新文档. 如果该表格定义了Primary Key, 则用Primary Key约束where语句. 对于
     where语句无法找到的行, 自动进行批量 bulk insert.
     """
     return update_all(engine=engine, table=table, data=data, upsert=True)
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/engine_creator.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/engine_creator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/io.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 
 """
 Database data/Local File I/O module.
 """
 
 import os
-from sqlalchemy import select
-from sqlalchemy.engine import Engine
+import sqlalchemy as sa
 
 
 def sql_to_csv(
     stmt,
-    engine: Engine,
+    engine: sa.Engine,
     filepath: str,
     chunksize: int = 1000,
     overwrite: bool = False,
 ):
     """
     Export sql stmt result to csv file.
 
@@ -32,40 +31,47 @@
     """
     if overwrite:  # pragma: no cover
         if os.path.exists(filepath):
             raise Exception("'%s' already exists!" % filepath)
 
     import pandas as pd
 
-    columns = [str(column.name) for column in stmt.columns]
+    columns = [str(column.name) for column in stmt.selected_columns]
     with open(filepath, "w") as f:
         # write header
         df = pd.DataFrame([], columns=columns)
         df.to_csv(f, header=True, index=False)
 
         # iterate big database table
-        result_proxy = engine.execute(stmt)
-        while True:
-            data = result_proxy.fetchmany(chunksize)
-            if len(data) == 0:
-                break
-            else:
-                df = pd.DataFrame(data, columns=columns)
-                df.to_csv(f, header=False, index=False)
+        with engine.connect() as connection:
+            result_proxy = connection.execute(stmt)
+            while True:
+                data = result_proxy.fetchmany(chunksize)
+                if len(data) == 0:
+                    break
+                else:
+                    df = pd.DataFrame(data, columns=columns)
+                    df.to_csv(f, header=False, index=False)
 
 
-def table_to_csv(table, engine, filepath, chunksize=1000, overwrite=False):
+def table_to_csv(
+    table: sa.Table,
+    engine: sa.Engine,
+    filepath,
+    chunksize: int = 1000,
+    overwrite: bool = False,
+):
     """
     Export entire table to a csv file.
 
     :param table: :class:`sqlalchemy.Table` instance.
     :param engine: :class:`sqlalchemy.engine.base.Engine`.
     :param filepath: file path.
     :param chunksize: number of rows write to csv each time.
     :param overwrite: bool, if True, avoid to overite existing file.
 
     **中文文档**
 
     将整个表中的所有数据, 写入csv文件。
     """
-    sql = select([table])
+    sql = sa.select(table)
     sql_to_csv(sql, engine, filepath, chunksize)
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/orm/extended_declarative_base.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/orm/extended_declarative_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,12 +637,12 @@
                 seed=func.random()
             )
             args = [
                 getattr(selectable.c, column.name)
                 for column in cls.__table__.columns
             ]
             stmt = select(*args)
-            results = [cls(**dict(row)) for row in ses.execute(stmt)]
+            results = [cls(**row._asdict()) for row in ses.execute(stmt)]
         else:
             raise ValueError
         clean_session(ses, auto_close)
         return results
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pkg/timeout_decorator/timeout_decorator.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/pt.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/pt.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,83 +9,72 @@
 
 因为 PrettyTable 只能通过 from_db_cursor 来创建, 也就是说要求返回
 ResultProxy, 而不是 ORM 对象的列表. 所以在 :func:`from_object`, :func:`from_query`
 这些使用 ``session.query(Entity)`` 的函数中, 我们需要用特殊技巧, 让 session.query
 最终返回 ResultProxy.
 """
 
-from typing import Union, Tuple, List
-from sqlalchemy import select, Table, text
-from sqlalchemy.engine import Engine
-from sqlalchemy.orm import Session
-
-from sqlalchemy.orm import DeclarativeMeta
-from sqlalchemy.sql.selectable import Select
-from sqlalchemy.sql.elements import TextClause
-from sqlalchemy.engine.result import Result, ScalarResult, Row
+import typing as T
+
+import sqlalchemy as sa
+import sqlalchemy.orm as orm
 
 from prettytable import PrettyTable
 
 from .utils import ensure_session, clean_session
 
 
-def get_keys_values(item) -> Tuple[Union[list, tuple], Union[list, tuple]]:
-    if isinstance(item.__class__, DeclarativeMeta):
+def get_keys_values(
+    item,
+) -> T.Tuple[T.Union[list, tuple], T.Union[list, tuple]]:
+    if isinstance(item.__class__, orm.DeclarativeMeta):
         keys, values = list(), list()
         for column in item.__class__.__table__.columns:
             keys.append(column.name)
             values.append(getattr(item, column.name))
         return keys, values
-    elif isinstance(item, Row):
+    elif isinstance(item, sa.Row):
         return list(item._fields), list(item)
     else:  # pragma: no cover
         raise TypeError
 
 
-def from_result(result: Union[Result, ScalarResult]):
+def from_result(result: T.Union[sa.Result, sa.ScalarResult]):
     pt = PrettyTable()
     try:
         first_item = next(result)
         keys, values = get_keys_values(first_item)
         pt.field_names = keys
         pt.add_row(values)
     except StopIteration:
         return pt
 
-    if isinstance(result, ScalarResult):
+    if isinstance(result, sa.ScalarResult):
         for obj in result:
             pt.add_row([getattr(obj, key) for key in keys])
-    elif isinstance(result, Result):
+    elif isinstance(result, sa.Result):
         for row in result:
             pt.add_row(list(row))
     else:
         raise Exception
 
     return pt
 
 
-def from_text_clause(
-    t: TextClause,
-    engine: Engine,
-    **kwargs
-) -> PrettyTable:
+def from_text_clause(t: sa.TextClause, engine: sa.Engine, **kwargs) -> PrettyTable:
     """
     Execute a query in form of texture clause, return the result in form of
     :class:`PrettyTable`.
     """
     with engine.connect() as connection:
         result = connection.execute(t, **kwargs)
         return from_result(result)
 
 
-def from_stmt(
-    stmt: Select,
-    engine: Engine,
-    **kwargs
-) -> PrettyTable:
+def from_stmt(stmt: sa.Select, engine: sa.Engine, **kwargs) -> PrettyTable:
     """
     Create a :class:`prettytable.PrettyTable` from :class:`sqlalchemy.select`.
 
     :param sql: a ``sqlalchemy.sql.selectable.Select`` object.
     :param engine: an ``sqlalchemy.engine.base.Engine`` object.
 
     **中文文档**
@@ -94,43 +83,40 @@
     """
     with engine.connect() as connection:
         result = connection.execute(stmt, **kwargs)
         return from_result(result)
 
 
 def from_table(
-    table: Table,
-    engine: Engine,
-    limit: int = None,
-    **kwargs
+    table: sa.Table, engine: sa.Engine, limit: int = None, **kwargs
 ) -> PrettyTable:
     """
     Select data in a database table and put into prettytable.
 
     Create a :class:`prettytable.PrettyTable` from :class:`sqlalchemy.Table`.
 
     :param table: a ``sqlalchemy.sql.schema.Table`` object
     :param engine: the engine or session used to execute the query.
     :param limit: int, limit rows to return.
 
     **中文文档**
 
     将数据表中的数据放入 PrettyTable 中.
     """
-    stmt = select([table])
+    stmt = sa.select(table)
     if limit is not None:
         stmt = stmt.limit(limit)
     with engine.connect() as connection:
         result = connection.execute(stmt, **kwargs)
         return from_result(result)
 
 
 def from_model(
     orm_class,
-    engine_or_session: Union[Engine, Session],
+    engine_or_session: T.Union[sa.Engine, orm.Session],
     limit: int = None,
     **kwargs
 ):
     """
     Select data from the table defined by a ORM class, and put into prettytable
 
     :param orm_class: an orm class inherit from
@@ -141,79 +127,83 @@
     **中文文档**
 
     将数据对象的数据放入 PrettyTable 中.
 
     常用于快速预览某个对象背后的数据.
     """
     ses, auto_close = ensure_session(engine_or_session)
-    stmt = select(orm_class.__table__)
+    stmt = sa.select(orm_class.__table__)
     if limit is not None:
         stmt = stmt.limit(limit)
     result = ses.execute(stmt, **kwargs)
     tb = from_result(result)
     clean_session(ses, auto_close)
     return tb
 
 
-def from_dict_list(data: List[dict]) -> PrettyTable:
+def from_dict_list(data: T.List[dict]) -> PrettyTable:
     """
     Construct a Prettytable from list of dictionary.
     """
     tb = PrettyTable()
     if len(data) == 0:  # pragma: no cover
         return tb
     else:
         tb.field_names = list(data[0].keys())
         for row in data:
             tb.add_row(list(row.values()))
         return tb
 
 
 def from_everything(
-    everything: Union[
-        TextClause, Select, Table, List[dict], DeclarativeMeta
+    everything: T.Union[
+        sa.TextClause,
+        sa.Select,
+        sa.Table,
+        T.List[dict],
+        orm.DeclarativeMeta,
     ],
-    engine_or_session: Union[Engine, Session] = None,
+    engine_or_session: T.Union[sa.Engine, orm.Session] = None,
     limit: int = None,
     **kwargs
 ):
     """
     Construct a Prettytable from any kinds of sqlalchemy query.
 
     :type engine_or_session: Union[Engine, Session]
 
     :rtype: PrettyTable
 
     Usage::
 
         from sqlalchemy import select
 
-        sql = select([t_user])
+        sql = select(t_user)
         print(from_everything(sql, engine))
 
         query = session.query(User)
         print(from_everything(query, session))
 
         session.query(User)
     """
-    if isinstance(everything, TextClause):
+    if isinstance(everything, sa.TextClause):
         return from_text_clause(everything, engine_or_session, **kwargs)
 
     if isinstance(everything, str):
-        return from_text_clause(text(everything), engine_or_session, **kwargs)
+        return from_text_clause(sa.text(everything), engine_or_session, **kwargs)
 
-    if isinstance(everything, Select):
+    if isinstance(everything, sa.Select):
         return from_stmt(everything, engine_or_session, **kwargs)
 
-    if isinstance(everything, Table):
+    if isinstance(everything, sa.Table):
         return from_table(everything, engine_or_session, limit=limit, **kwargs)
 
-    if isinstance(everything, DeclarativeMeta):
+    if isinstance(everything, orm.DeclarativeMeta):
         return from_model(everything, engine_or_session, limit=limit, **kwargs)
 
-    if isinstance(everything, Result):
+    if isinstance(everything, sa.Result):
         return from_result(everything)
 
     if isinstance(everything, list):
         return from_dict_list(everything)
 
     raise Exception
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/compressed.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/compressed.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/compressed_json.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/compressed_json.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/types/json_serializable.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/json_serializable.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate/utils.py` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
 
 """
 Utilities function.
 """
 
-from typing import Type, Union, Tuple, Dict, Iterable
+import typing as T
 
 import sqlalchemy as sa
-from sqlalchemy.engine import Engine
-from sqlalchemy.orm import sessionmaker, Session
+import sqlalchemy.orm as orm
 
 
 def ensure_exact_one_arg_is_not_none(*args):
     if sum([bool(arg is not None) for arg in args]) != 1:
         raise ValueError
 
 
 def ensure_list(item) -> list:
     if not isinstance(item, (list, tuple)):
-        return [item, ]
+        return [
+            item,
+        ]
     else:
         return item
 
 
-def grouper_list(l: Iterable, n: int) -> Iterable[list]:
+def grouper_list(l: T.Iterable, n: int) -> T.Iterable[list]:
     """Evenly divide list into fixed-length piece, no filled value if chunk
     size smaller than fixed-length.
 
     Example::
 
         >>> list(grouper(range(10), n=3)
         [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9]]
@@ -52,68 +53,68 @@
             yield chunk
             chunk = list()
             counter = 0
     if len(chunk) > 0:
         yield chunk
 
 
-session_klass_cache = dict()  # type: Dict[int, Type[Session]]
+session_klass_cache: T.Dict[int, T.Type[orm.Session]] = dict()
 
 
 def ensure_session(
-    engine_or_session: Union[Engine, Session]
-) -> Tuple[Session, bool]:
+    engine_or_session: T.Union[sa.Engine, orm.Session]
+) -> T.Tuple[orm.Session, bool]:
     """
     If it is an engine, then create a session from it. And indicate that
     this session should be closed after the job done.
 
     **中文文档**
 
     在 ORM 中对数据进行操作主要是通过 Session. 如果传入的参数是 Engine, 则创建一个
     Session, 用完之后是要 close 的, 所以 ``auto_close = True`` 因为这个
     Session 反正是新创建的. 如果传入的参数是 Session, 用完之后是否 close 取决于业务,
     所以 ``auto_close = False``.
     """
-    if isinstance(engine_or_session, Engine):
+    if isinstance(engine_or_session, sa.Engine):
         engine_id = id(engine_or_session)
         if engine_id not in session_klass_cache:  # pragma: no cover
-            session_klass_cache[engine_id] = sessionmaker(bind=engine_or_session)
+            session_klass_cache[engine_id] = orm.Session
         SessionClass = session_klass_cache[engine_id]
-        session = SessionClass()
+        session = SessionClass(engine_or_session)
         auto_close = True
         return session, auto_close
-    elif isinstance(engine_or_session, Session):
+    elif isinstance(engine_or_session, orm.Session):
         session = engine_or_session
         auto_close = False
         return session, auto_close
 
 
 def clean_session(
-    session: Session,
+    session: orm.Session,
     auto_close: bool,
 ):
     """
     Close session if necessary. Just a syntax sugar.
     """
     if auto_close:
         session.close()
 
 
-from .pkg import timeout_decorator
+from .vendor import timeout_decorator
 
 
 def test_connection(engine, timeout=3):
     @timeout_decorator.timeout(timeout)
     def _test_connection(engine):
-        v = engine.execute(sa.text("SELECT 1;")).fetchall()[0][0]
-        assert v == 1
+        with engine.connect() as connection:
+            v = connection.execute(sa.text("SELECT 1;")).fetchall()[0][0]
+            assert v == 1
 
     try:
         _test_connection(engine)
         return True
     except timeout_decorator.TimeoutError:
-        raise timeout_decorator.TimeoutError(
-            "time out in %s seconds!" % timeout)
+        raise timeout_decorator.TimeoutError("time out in %s seconds!" % timeout)
     except AssertionError:  # pragma: no cover
         raise ValueError
     except Exception as e:
         raise e
```

### Comparing `sqlalchemy_mate-1.4.28.4/sqlalchemy_mate.egg-info/PKG-INFO` & `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: sqlalchemy-mate
-Version: 1.4.28.4
+Name: sqlalchemy_mate
+Version: 2.0.0.0
 Summary: A library extend sqlalchemy module, makes CRUD easier.
 Home-page: https://github.com/MacHu-GWU/sqlalchemy_mate-project
-Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/1.4.28.4#downloads
+Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.0#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -15,56 +15,79 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: tests
-Provides-Extra: docs
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
+Requires-Dist: sqlalchemy<3.0.0,>=2.0.0
+Requires-Dist: prettytable<4.0.0,>=3.0.0
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pg8000; extra == "tests"
+Requires-Dist: attrs; extra == "tests"
+Requires-Dist: superjson; extra == "tests"
+Requires-Dist: pandas; extra == "tests"
+Provides-Extra: docs
+Requires-Dist: Sphinx==5.3.0; extra == "docs"
+Requires-Dist: sphinx-jinja==2.0.2; extra == "docs"
+Requires-Dist: sphinx-copybutton==0.5.1; extra == "docs"
+Requires-Dist: sphinx-design==0.5.0; extra == "docs"
+Requires-Dist: furo==2023.03.27; extra == "docs"
+Requires-Dist: nbsphinx==0.8.12; extra == "docs"
+Requires-Dist: rstobj==1.2.1; extra == "docs"
+Requires-Dist: pygments==2.15.1; extra == "docs"
+Requires-Dist: ipython==8.10.0; extra == "docs"
+Requires-Dist: docfly==2.0.3; extra == "docs"
 
 .. image:: https://readthedocs.org/projects/sqlalchemy_mate/badge/?version=latest
-    :target: https://sqlalchemy_mate.readthedocs.io/index.html
+    :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
     :alt: Documentation Status
 
-.. image:: https://github.com/MacHu-GWU/sqlalchemy_mate-project/workflows/CI/badge.svg
+.. image:: https://github.com/MacHu-GWU/sqlalchemy_mate-project/actions/workflows/main.yml/badge.svg
     :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/sqlalchemy_mate-project/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/MacHu-GWU/sqlalchemy_mate-project
 
 .. image:: https://img.shields.io/pypi/v/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
 .. image:: https://img.shields.io/pypi/l/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/sqlalchemy_mate.svg
     :target: https://pypi.python.org/pypi/sqlalchemy_mate
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project/blob/master/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project
 
 ------
 
-
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/index.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/py-modindex.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
-      :target: https://sqlalchemy_mate.readthedocs.io/py-modindex.html
+      :target: https://sqlalchemy-mate.readthedocs.io/latest/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
       :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
       :target: https://github.com/MacHu-GWU/sqlalchemy_mate-project
 
@@ -76,30 +99,32 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
       :target: https://pypi.org/pypi/sqlalchemy_mate#files
 
 
 Welcome to ``sqlalchemy_mate`` Documentation
 ==============================================================================
-
 A sweet syntax sugar library simplify your in writing ``sqlalchemy`` code.
 
+📔 `Full document is HERE <https://sqlalchemy-mate.readthedocs.io/latest/index.html>`_
+
+.. image:: https://sqlalchemy-mate.readthedocs.io/latest/_static/sqlalchemy_mate-logo.png
+    :target: https://sqlalchemy-mate.readthedocs.io/latest/index.html
+
 
 Features
 ------------------------------------------------------------------------------
-
 .. contents::
     :class: this-will-duplicate-information-and-it-is-still-useful-here
     :depth: 1
     :local:
 
 
 Read Database Credential Safely
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 .. contents::
     :class: this-will-duplicate-information-and-it-is-still-useful-here
     :depth: 1
     :local:
 
 Put your database connection credential in your source code is always a **BAD IDEA**.
 
@@ -241,24 +266,25 @@
     # leave aws_profile=None if you are on cloud
     ec = EngineCreator.from_env(prefix="DB_DEV", kms_decrypt=True, aws_profile="xxx")
     engine = ec.create_redshift()
 
 
 Smart Insert
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 In bulk insert, if there are some rows having primary_key conflict, the classic solution is:
 
 .. code-block:: python
 
-    for row in data:
-        try:
-            engine.execute(table.insert(), row)
-        except sqlalchemy.sql.IntegrityError:
-            pass
+    with engine.connect() as conn:
+        for row in data:
+            try:
+                conn.execute(table.insert(), row)
+                conn.commit()
+            except sqlalchemy.exc.IntegrityError:
+                conn.rollback()
 
 It is like one-by-one insert, which is super slow.
 
 ``sqlalchemy_mate`` uses ``smart_insert`` strategy to try with smaller bulk insert, which has higher probabily to work. As a result, total number of commits are greatly reduced.
 
 With sql expression:
 
@@ -311,15 +337,14 @@
     User.upsert_all(engine_or_session, user_list)
 
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
-
 ``sqlalchemy_mate`` is released on PyPI, so all you need is:
 
 .. code-block:: console
 
     $ pip install sqlalchemy_mate
 
 To upgrade to latest version:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sqlalchemy_mate-1.4.28.4/tests/test_engine_creator.py` & `sqlalchemy_mate-2.0.0.0/tests/test_engine_creator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 # -*- coding: utf-8 -*-
 
 import json
 import os
 
-import pytest
 from pytest import raises
 
 from sqlalchemy_mate.engine_creator import EngineCreator
 
 json_file = os.path.join(os.path.dirname(__file__), "db.json")
 with open(json_file, "wb") as f:
     f.write(
-        json.dumps({
-            "mydb": dict(host="host", port=1234, database="dev",
-                         username="user", password="pass")
-        }).encode("utf-8")
+        json.dumps(
+            {
+                "mydb": dict(
+                    host="host",
+                    port=1234,
+                    database="dev",
+                    username="user",
+                    password="pass",
+                )
+            }
+        ).encode("utf-8")
     )
 
 
 class TestEngineCreator(object):
     def test_uri(self):
-        cred = EngineCreator(host="host", port=1234, database="dev",
-                             username="user", password="pass")
+        cred = EngineCreator(
+            host="host", port=1234, database="dev", username="user", password="pass"
+        )
         assert cred.uri == "user:pass@host:1234/dev"
 
-        cred = EngineCreator(host="host", port=1234,
-                             database="dev", username="user")
+        cred = EngineCreator(host="host", port=1234, database="dev", username="user")
         assert cred.uri == "user@host:1234/dev"
 
-        cred = EngineCreator(host="host", database="dev",
-                             username="user", password="pass")
+        cred = EngineCreator(
+            host="host", database="dev", username="user", password="pass"
+        )
         assert cred.uri == "user:pass@host/dev"
 
         cred = EngineCreator(host="host", database="dev", username="user")
         assert cred.uri == "user@host/dev"
 
     def test_from_json_data(self):
         cred = EngineCreator.from_json(json_file, json_path="mydb")
@@ -67,29 +74,34 @@
 
         with raises(ValueError):
             EngineCreator._validate_key_mapping(dict(a=1, b=2))
 
         EngineCreator._validate_key_mapping(None)
         EngineCreator._validate_key_mapping(
             dict(
-                host="host", port="port", database="db",
-                username="user", password="pass"
+                host="host",
+                port="port",
+                database="db",
+                username="user",
+                password="pass",
             )
         )
 
     def test_transform(self):
         data = {"host": 1, "port": 2, "db": 3, "user": 4, "pass": 5}
         new_data = EngineCreator._transform(
-            data, dict(
-                host="host", port="port", database="db",
-                username="user", password="pass"
-            )
+            data,
+            dict(
+                host="host",
+                port="port",
+                database="db",
+                username="user",
+                password="pass",
+            ),
         )
-        assert new_data == dict(
-            host=1, port=2, database=3, username=4, password=5)
+        assert new_data == dict(host=1, port=2, database=3, username=4, password=5)
 
 
 if __name__ == "__main__":
-    import os
+    from sqlalchemy_mate.tests import run_cov_test
 
-    basename = os.path.basename(__file__)
-    pytest.main([basename, "-s", "--tb=native"])
+    run_cov_test(__file__, "sqlalchemy_mate.engine_creator", preview=False)
```

### Comparing `sqlalchemy_mate-1.4.28.4/tests/test_io.py` & `sqlalchemy_mate-2.0.0.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-1.4.28.4/tests/test_pt.py` & `sqlalchemy_mate-2.0.0.0/tests/test_pt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from sqlalchemy import select, text
-from sqlalchemy.orm import Session
-from sqlalchemy_mate import pt, selecting
+
+import sqlalchemy as sa
+import sqlalchemy.orm as orm
+
 from prettytable import PrettyTable
+
+from sqlalchemy_mate import pt, selecting
 from sqlalchemy_mate.tests import (
     IS_WINDOWS,
-    engine_sqlite, engine_psql,
-    t_user, t_inv, User, Association,
+    engine_sqlite,
+    engine_psql,
+    t_user,
+    t_inv,
+    User,
+    Association,
     BaseTest,
 )
 
 
 class PrettyTableTestBase(BaseTest):
     @classmethod
     def class_level_data_setup(cls):
@@ -32,128 +39,129 @@
             {"store_id": 2, "item_id": 1},
             {"store_id": 2, "item_id": 2},
             {"store_id": 3, "item_id": 1},
             {"store_id": 3, "item_id": 2},
         ]
 
         with cls.engine.connect() as connection:
-            connection.execute(t_user.insert(), t_user_data)
+            connection.execute(sa.insert(t_user), t_user_data)
             connection.execute(t_inv.insert(), t_inv_data)
-
-        with Session(cls.engine) as ses:
-            ses.add_all([
-                User(id=1, name="X"),
-                User(id=2, name="Y"),
-                User(id=3, name="Z"),
-            ])
-            ses.add_all([
-                Association(x_id=1, y_id=1, flag=1),
-                Association(x_id=1, y_id=2, flag=2),
-                Association(x_id=2, y_id=1, flag=3),
-                Association(x_id=2, y_id=2, flag=4),
-            ])
+            connection.commit()
+        
+        with orm.Session(cls.engine) as ses:
+            ses.add_all(
+                [
+                    User(id=1, name="X"),
+                    User(id=2, name="Y"),
+                    User(id=3, name="Z"),
+                ]
+            )
+            ses.add_all(
+                [
+                    Association(x_id=1, y_id=1, flag=1),
+                    Association(x_id=1, y_id=2, flag=2),
+                    Association(x_id=2, y_id=1, flag=3),
+                    Association(x_id=2, y_id=2, flag=4),
+                ]
+            )
             ses.commit()
 
-    def test_get_headers(self):
-        with Session(self.eng) as ses:
+    def _test_get_headers(self):
+        with orm.Session(self.eng) as ses:
             user = ses.get(User, 1)
             keys, values = pt.get_keys_values(user)
             assert keys == ["id", "name"]
             assert values == [1, "X"]
 
         with self.eng.connect() as connection:
-            row = connection.execute(select(t_user).limit(1)).first()
+            row = connection.execute(sa.select(t_user).limit(1)).fetchone()
             keys, values = pt.get_keys_values(row)
             assert keys == ["user_id", "name"]
             assert values == [1, "Alice"]
 
-    def test_from_result(self):
-        with Session(self.eng) as ses:
-            res = ses.scalars(select(User))
+    def _test_from_result(self):
+        with orm.Session(self.eng) as ses:
+            res = ses.scalars(sa.select(User))
             ptable = pt.from_result(res)
             assert len(ptable._rows) == 3
 
         with self.eng.connect() as connection:
-            res = connection.execute(select(t_user))
+            res = connection.execute(sa.select(t_user))
             ptable = pt.from_result(res)
             assert len(ptable._rows) == 4
 
-    def test_from_text_clause(self):
-        stmt = text(f"SELECT * FROM {t_user.name} LIMIT 2")
+    def _test_from_text_clause(self):
+        stmt = sa.text(f"SELECT * FROM {t_user.name} LIMIT 2")
         tb = pt.from_text_clause(stmt, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 2
-
-        stmt = text(f"SELECT * FROM {t_user.name} WHERE {t_user.name}.user_id = :user_id;")
-        tb = pt.from_text_clause(stmt, self.eng, user_id=1)
+        stmt = sa.text(
+            f"SELECT * FROM {t_user.name} WHERE {t_user.name}.user_id = :user_id;"
+        )
+        stmt = stmt.bindparams(user_id=1)
+        tb = pt.from_text_clause(stmt, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 1
 
-    def test_from_stmt(self):
-        stmt = select([t_inv])
+    def _test_from_stmt(self):
+        stmt = sa.select(t_inv)
         tb = pt.from_stmt(stmt, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 6
 
-        stmt = select([t_inv]).limit(3)
+        stmt = sa.select(t_inv).limit(3)
         tb = pt.from_stmt(stmt, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 3
 
         # ORM also works
-        query = select(User).where(User.id >= 2)
+        query = sa.select(User).where(User.id >= 2)
         tb = pt.from_stmt(query, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 2
 
-        query = select(User).limit(2)
+        query = sa.select(User).limit(2)
         tb = pt.from_stmt(query, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 2
 
-    def test_from_table(self):
+    def _test_from_table(self):
         tb = pt.from_table(t_inv, self.eng, limit=10)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 6
 
         tb = pt.from_table(t_inv, self.eng, limit=3)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 3
 
-    def test_from_model(self):
+    def _test_from_model(self):
         tb = pt.from_model(Association, self.eng, limit=2)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 2
 
-        with Session(self.eng) as ses:
+        with orm.Session(self.eng) as ses:
             tb = pt.from_model(User, ses, limit=2)
             assert isinstance(tb, PrettyTable)
             assert len(tb._rows) == 2
 
-    def test_from_data(self):
+    def _test_from_data(self):
         with self.eng.connect() as connection:
-            rows = [
-                dict(row)
-                for row in connection.execute(select(t_user))
-            ]
+            rows = [row._asdict() for row in connection.execute(sa.select(t_user))]
             tb = pt.from_dict_list(rows)
             assert isinstance(tb, PrettyTable)
             assert len(tb._rows) == 4
 
-    def test_from_everything(self):
-        t = text(f"SELECT * FROM {t_user.name} LIMIT 2")
-        stmt = select([t_user])
+    def _test_from_everything(self):
+        t = sa.text(f"SELECT * FROM {t_user.name} LIMIT 2")
+        stmt = sa.select(t_user)
         table = t_inv
-        query = select(Association)
+        query = sa.select(Association)
         orm_class = User
         result = selecting.select_all(self.engine, t_user)
-        data = [
-            dict(row)
-            for row in selecting.select_all(self.engine, t_user)
-        ]
+        data = [row._asdict() for row in selecting.select_all(self.engine, t_user)]
 
         everything = [
             t,
             stmt,
             table,
             query,
             orm_class,
@@ -164,25 +172,34 @@
         for thing in everything:
             tb = pt.from_everything(thing, self.engine, limit=10)
             assert isinstance(tb, PrettyTable)
 
         with pytest.raises(Exception):
             pt.from_everything(None)
 
+    def test(self):
+        self._test_get_headers()
+        self._test_from_result()
+        self._test_from_text_clause()
+        self._test_from_stmt()
+        self._test_from_table()
+        self._test_from_model()
+        self._test_from_data()
+        self._test_from_everything()
+
 
-class TestPrettyyTableSqlite(PrettyTableTestBase):
+class TestPrettyTableSqlite(PrettyTableTestBase):
     engine = engine_sqlite
 
 
 @pytest.mark.skipif(
     IS_WINDOWS,
     reason="no psql service container for windows",
 )
-class TestPrettyyTablePostgres(PrettyTableTestBase):
+class TestPrettyTablePostgres(PrettyTableTestBase):
     engine = engine_psql
 
 
 if __name__ == "__main__":
-    import os
+    from sqlalchemy_mate.tests import run_cov_test
 
-    basename = os.path.basename(__file__)
-    pytest.main([basename, "-s", "--tb=native"])
+    run_cov_test(__file__, "sqlalchemy_mate.pt", preview=False)
```

### Comparing `sqlalchemy_mate-1.4.28.4/tests/test_utils.py` & `sqlalchemy_mate-2.0.0.0/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # -*- coding: utf-8 -*-
 
-import sys
 
 import pytest
-from sqlalchemy import select
-from sqlalchemy.orm import Session
 from sqlalchemy_mate import utils
 from sqlalchemy_mate import EngineCreator, TimeoutError
 from sqlalchemy_mate.tests import (
     IS_WINDOWS,
     engine_sqlite, engine_psql, User, BaseTest,
 )
 
@@ -50,11 +47,10 @@
             database="diyvavwx", username="diyvavwx", password="wrongpassword"
         ).create_postgresql_pg8000()
         with pytest.raises(Exception):
             utils.test_connection(engine, timeout=10)
 
 
 if __name__ == "__main__":
-    import os
+    from sqlalchemy_mate.tests import run_cov_test
 
-    basename = os.path.basename(__file__)
-    pytest.main([basename, "-s", "--tb=native"])
+    run_cov_test(__file__, "sqlalchemy_mate.utils", preview=False)
```

