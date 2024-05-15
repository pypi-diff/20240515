# Comparing `tmp/scottbrian_utils-4.0.0.tar.gz` & `tmp/scottbrian_utils-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scottbrian_utils-4.0.0.tar", last modified: Mon May 13 00:36:01 2024, max compression
+gzip compressed data, was "scottbrian_utils-4.0.1.tar", last modified: Wed May 15 02:40:10 2024, max compression
```

## Comparing `scottbrian_utils-4.0.0.tar` & `scottbrian_utils-4.0.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.795690 scottbrian_utils-4.0.0/
--rw-rw-rw-   0        0        0     2054 2023-11-24 16:34:06.000000 scottbrian_utils-4.0.0/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.703669 scottbrian_utils-4.0.0/.idea/
--rw-rw-rw-   0        0        0      184 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.704670 scottbrian_utils-4.0.0/.idea/codeStyles/
--rw-rw-rw-   0        0        0      153 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/codeStyles/codeStyleConfig.xml
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.705670 scottbrian_utils-4.0.0/.idea/dictionaries/
--rw-rw-rw-   0        0        0       86 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/dictionaries/Tiger.xml
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.707670 scottbrian_utils-4.0.0/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      234 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      426 2023-11-23 15:37:03.000000 scottbrian_utils-4.0.0/.idea/misc.xml
--rw-rw-rw-   0        0        0      291 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/modules.xml
--rw-rw-rw-   0        0        0      191 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.0/.idea/other.xml
--rw-rw-rw-   0        0        0     1265 2023-11-22 18:32:15.000000 scottbrian_utils-4.0.0/.idea/scottbrian_utils.iml
--rw-rw-rw-   0        0        0      185 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/vcs.xml
--rw-rw-rw-   0        0        0      701 2023-12-02 22:36:11.000000 scottbrian_utils-4.0.0/.readthedocs.yml
--rw-rw-rw-   0        0        0     1092 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      609 2023-11-24 17:53:09.000000 scottbrian_utils-4.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7678 2024-05-13 00:36:01.793689 scottbrian_utils-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5392 2024-05-11 18:57:18.000000 scottbrian_utils-4.0.0/README.rst
--rw-rw-rw-   0        0        0     4338 2024-04-21 18:34:57.000000 scottbrian_utils-4.0.0/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.708670 scottbrian_utils-4.0.0/docs/
--rw-rw-rw-   0        0        0       57 2023-12-02 22:55:23.000000 scottbrian_utils-4.0.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.730675 scottbrian_utils-4.0.0/docs/source/
--rw-rw-rw-   0        0        0    83406 2023-10-14 18:15:17.000000 scottbrian_utils-4.0.0/docs/source/UniqueTS_UseCase1.svg
--rw-rw-rw-   0        0        0        0 2022-01-14 00:08:20.000000 scottbrian_utils-4.0.0/docs/source/_static
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.733676 scottbrian_utils-4.0.0/docs/source/adjust_sphinx/
--rw-rw-rw-   0        0        0        0 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/docs/source/adjust_sphinx/__init__.py
--rw-rw-rw-   0        0        0     2425 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/docs/source/adjust_sphinx/adjust_sphinx.py
--rw-rw-rw-   0        0        0     2356 2024-04-09 16:58:14.000000 scottbrian_utils-4.0.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      107 2024-03-31 17:44:01.000000 scottbrian_utils-4.0.0/docs/source/diag_msg_link.rst
--rw-rw-rw-   0        0        0       41 2024-03-31 01:45:20.000000 scottbrian_utils-4.0.0/docs/source/doc_checker_link.rst
--rw-rw-rw-   0        0        0       41 2024-04-21 18:48:29.000000 scottbrian_utils-4.0.0/docs/source/entry_trace_link.rst
--rw-rw-rw-   0        0        0       54 2024-03-31 17:05:54.000000 scottbrian_utils-4.0.0/docs/source/file_catalog_link.rst
--rw-rw-rw-   0        0        0       40 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/docs/source/flower_box_link.rst
--rw-rw-rw-   0        0        0      835 2024-04-21 18:48:29.000000 scottbrian_utils-4.0.0/docs/source/index.rst
--rw-rw-rw-   0        0        0       49 2024-03-31 01:41:28.000000 scottbrian_utils-4.0.0/docs/source/log_verifier_link.rst
--rw-rw-rw-   0        0        0       39 2024-03-31 01:41:28.000000 scottbrian_utils-4.0.0/docs/source/msgs_link.rst
--rw-rw-rw-   0        0        0       58 2024-03-31 17:11:13.000000 scottbrian_utils-4.0.0/docs/source/pauser_link.rst
--rw-rw-rw-   0        0        0      306 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/docs/source/setup.py
--rw-rw-rw-   0        0        0       50 2024-03-31 17:12:31.000000 scottbrian_utils-4.0.0/docs/source/stop_watch_link.rst
--rw-rw-rw-   0        0        0       74 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.0/docs/source/time_hdr_link.rst
--rw-rw-rw-   0        0        0       41 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.0/docs/source/timer_link.rst
--rw-rw-rw-   0        0        0       48 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.0/docs/source/unique_ts_link.rst
--rw-rw-rw-   0        0        0      266 2024-04-24 17:55:01.000000 scottbrian_utils-4.0.0/mypy.ini
--rw-rw-rw-   0        0        0     1207 2024-04-24 15:49:06.000000 scottbrian_utils-4.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      886 2024-04-23 02:16:03.000000 scottbrian_utils-4.0.0/pytest.ini
--rw-rw-rw-   0        0        0       42 2024-05-13 00:36:01.795690 scottbrian_utils-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      192 2023-11-22 18:11:03.000000 scottbrian_utils-4.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.734676 scottbrian_utils-4.0.0/src/
--rw-rw-rw-   0        0        0     5191 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.0/src/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.754681 scottbrian_utils-4.0.0/src/scottbrian_utils/
--rw-rw-rw-   0        0        0      141 2024-04-09 16:58:14.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/__init__.py
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/__init__.pyi
--rw-rw-rw-   0        0        0    12890 2023-11-24 00:13:36.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/diag_msg.py
--rw-rw-rw-   0        0        0     8201 2023-11-30 17:05:18.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/doc_checker.py
--rw-rw-rw-   0        0        0    13327 2024-05-12 01:24:29.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/entry_trace.py
--rw-rw-rw-   0        0        0    15194 2024-03-31 01:49:03.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/file_catalog.py
--rw-rw-rw-   0        0        0     1833 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/flower_box.py
--rw-rw-rw-   0        0        0    48973 2024-05-10 18:26:16.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/log_verifier.py
--rw-rw-rw-   0        0        0     7606 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/msgs.py
--rw-rw-rw-   0        0        0    20415 2023-11-24 00:11:58.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/pauser.py
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/py.typed
--rw-rw-rw-   0        0        0     6792 2023-01-26 16:36:30.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/stop_watch.py
--rw-rw-rw-   0        0        0    18522 2024-04-14 23:53:31.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/time_hdr.py
--rw-rw-rw-   0        0        0    24423 2023-04-11 22:05:38.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/timer.py
--rw-rw-rw-   0        0        0     2322 2023-10-14 23:15:12.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/unique_ts.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.792688 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/
--rw-rw-rw-   0        0        0     7678 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2638 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.678663 scottbrian_utils-4.0.0/tests/
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.781687 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/
--rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/__init__.py
--rw-rw-rw-   0        0        0     8171 2023-11-24 21:49:34.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py
--rw-rw-rw-   0        0        0     5699 2024-04-24 20:25:46.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/conftest.py
--rw-rw-rw-   0        0        0   493189 2023-11-24 21:49:35.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_diag_msg.py
--rw-rw-rw-   0        0        0   106995 2024-05-12 19:26:02.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_entry_trace.py
--rw-rw-rw-   0        0        0    17147 2023-11-24 00:16:31.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_file_catalog.py
--rw-rw-rw-   0        0        0     7704 2023-07-01 17:34:46.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_flower_box.py
--rw-rw-rw-   0        0        0   152540 2024-05-10 20:20:22.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_log_verifier.py
--rw-rw-rw-   0        0        0    15938 2024-05-08 01:06:25.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_msgs.py
--rw-rw-rw-   0        0        0    36592 2023-11-24 00:15:56.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_pauser.py
--rw-rw-rw-   0        0        0    17642 2023-07-01 17:34:46.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_stop_watch.py
--rw-rw-rw-   0        0        0    77560 2024-04-22 00:08:46.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_time_hdr.py
--rw-rw-rw-   0        0        0    40767 2023-11-23 15:44:47.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_timer.py
--rw-rw-rw-   0        0        0     5972 2023-11-25 00:12:19.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_unique_ts.py
--rw-rw-rw-   0        0        0     6635 2024-05-03 14:48:19.000000 scottbrian_utils-4.0.0/tox.ini
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.679664 scottbrian_utils-4.0.0/type_stubs/
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.783687 scottbrian_utils-4.0.0/type_stubs/mypywrapt/
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.785687 scottbrian_utils-4.0.0/type_stubs/mypywrapt/adjust_src/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/adjust_src/__init__.pyi
--rw-rw-rw-   0        0        0     1292 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/adjust_src/adjust_src.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.680663 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.680663 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/lib/
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.788689 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/__init__.pyi
--rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/decorators.pyi
--rw-rw-rw-   0        0        0      388 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.791689 scottbrian_utils-4.0.0/type_stubs/mypywrapt/wrapt-stubs/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/wrapt-stubs/__init__.pyi
--rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/wrapt-stubs/decorators.pyi
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.679466 scottbrian_utils-4.0.1/
+-rw-rw-rw-   0        0        0     2054 2023-11-24 16:34:06.000000 scottbrian_utils-4.0.1/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.580544 scottbrian_utils-4.0.1/.idea/
+-rw-rw-rw-   0        0        0      184 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.582539 scottbrian_utils-4.0.1/.idea/codeStyles/
+-rw-rw-rw-   0        0        0      153 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/.idea/codeStyles/codeStyleConfig.xml
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.583539 scottbrian_utils-4.0.1/.idea/dictionaries/
+-rw-rw-rw-   0        0        0       86 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/.idea/dictionaries/Tiger.xml
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.584539 scottbrian_utils-4.0.1/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      234 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      426 2023-11-23 15:37:03.000000 scottbrian_utils-4.0.1/.idea/misc.xml
+-rw-rw-rw-   0        0        0      291 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/.idea/modules.xml
+-rw-rw-rw-   0        0        0      191 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.1/.idea/other.xml
+-rw-rw-rw-   0        0        0     1265 2023-11-22 18:32:15.000000 scottbrian_utils-4.0.1/.idea/scottbrian_utils.iml
+-rw-rw-rw-   0        0        0      185 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/.idea/vcs.xml
+-rw-rw-rw-   0        0        0      701 2023-12-02 22:36:11.000000 scottbrian_utils-4.0.1/.readthedocs.yml
+-rw-rw-rw-   0        0        0     1092 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      609 2023-11-24 17:53:09.000000 scottbrian_utils-4.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7748 2024-05-15 02:40:10.678470 scottbrian_utils-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5462 2024-05-15 02:25:12.000000 scottbrian_utils-4.0.1/README.rst
+-rw-rw-rw-   0        0        0     4338 2024-04-21 18:34:57.000000 scottbrian_utils-4.0.1/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.586539 scottbrian_utils-4.0.1/docs/
+-rw-rw-rw-   0        0        0       57 2023-12-02 22:55:23.000000 scottbrian_utils-4.0.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.610346 scottbrian_utils-4.0.1/docs/source/
+-rw-rw-rw-   0        0        0    83406 2023-10-14 18:15:17.000000 scottbrian_utils-4.0.1/docs/source/UniqueTS_UseCase1.svg
+-rw-rw-rw-   0        0        0        0 2022-01-14 00:08:20.000000 scottbrian_utils-4.0.1/docs/source/_static
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.612347 scottbrian_utils-4.0.1/docs/source/adjust_sphinx/
+-rw-rw-rw-   0        0        0        0 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/docs/source/adjust_sphinx/__init__.py
+-rw-rw-rw-   0        0        0     2425 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/docs/source/adjust_sphinx/adjust_sphinx.py
+-rw-rw-rw-   0        0        0     2356 2024-05-15 02:25:12.000000 scottbrian_utils-4.0.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0      107 2024-03-31 17:44:01.000000 scottbrian_utils-4.0.1/docs/source/diag_msg_link.rst
+-rw-rw-rw-   0        0        0       41 2024-03-31 01:45:20.000000 scottbrian_utils-4.0.1/docs/source/doc_checker_link.rst
+-rw-rw-rw-   0        0        0       41 2024-04-21 18:48:29.000000 scottbrian_utils-4.0.1/docs/source/entry_trace_link.rst
+-rw-rw-rw-   0        0        0       54 2024-03-31 17:05:54.000000 scottbrian_utils-4.0.1/docs/source/file_catalog_link.rst
+-rw-rw-rw-   0        0        0       40 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/docs/source/flower_box_link.rst
+-rw-rw-rw-   0        0        0      835 2024-04-21 18:48:29.000000 scottbrian_utils-4.0.1/docs/source/index.rst
+-rw-rw-rw-   0        0        0       49 2024-03-31 01:41:28.000000 scottbrian_utils-4.0.1/docs/source/log_verifier_link.rst
+-rw-rw-rw-   0        0        0       39 2024-03-31 01:41:28.000000 scottbrian_utils-4.0.1/docs/source/msgs_link.rst
+-rw-rw-rw-   0        0        0       58 2024-03-31 17:11:13.000000 scottbrian_utils-4.0.1/docs/source/pauser_link.rst
+-rw-rw-rw-   0        0        0      306 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/docs/source/setup.py
+-rw-rw-rw-   0        0        0       50 2024-03-31 17:12:31.000000 scottbrian_utils-4.0.1/docs/source/stop_watch_link.rst
+-rw-rw-rw-   0        0        0       74 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.1/docs/source/time_hdr_link.rst
+-rw-rw-rw-   0        0        0       41 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.1/docs/source/timer_link.rst
+-rw-rw-rw-   0        0        0       48 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.1/docs/source/unique_ts_link.rst
+-rw-rw-rw-   0        0        0      266 2024-04-24 17:55:01.000000 scottbrian_utils-4.0.1/mypy.ini
+-rw-rw-rw-   0        0        0     1207 2024-05-15 02:25:12.000000 scottbrian_utils-4.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      886 2024-04-23 02:16:03.000000 scottbrian_utils-4.0.1/pytest.ini
+-rw-rw-rw-   0        0        0       42 2024-05-15 02:40:10.680466 scottbrian_utils-4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      192 2023-11-22 18:11:03.000000 scottbrian_utils-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.614349 scottbrian_utils-4.0.1/src/
+-rw-rw-rw-   0        0        0     5191 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.1/src/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.636357 scottbrian_utils-4.0.1/src/scottbrian_utils/
+-rw-rw-rw-   0        0        0      141 2024-05-15 02:25:12.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/__init__.pyi
+-rw-rw-rw-   0        0        0    12890 2023-11-24 00:13:36.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/diag_msg.py
+-rw-rw-rw-   0        0        0     8201 2023-11-30 17:05:18.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/doc_checker.py
+-rw-rw-rw-   0        0        0    13338 2024-05-15 01:23:40.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/entry_trace.py
+-rw-rw-rw-   0        0        0    15194 2024-03-31 01:49:03.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/file_catalog.py
+-rw-rw-rw-   0        0        0     1833 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/flower_box.py
+-rw-rw-rw-   0        0        0    48973 2024-05-10 18:26:16.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/log_verifier.py
+-rw-rw-rw-   0        0        0     7606 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/msgs.py
+-rw-rw-rw-   0        0        0    20415 2023-11-24 00:11:58.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/pauser.py
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/py.typed
+-rw-rw-rw-   0        0        0     6792 2023-01-26 16:36:30.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/stop_watch.py
+-rw-rw-rw-   0        0        0    18522 2024-04-14 23:53:31.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/time_hdr.py
+-rw-rw-rw-   0        0        0    24423 2023-04-11 22:05:38.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/timer.py
+-rw-rw-rw-   0        0        0     2322 2023-10-14 23:15:12.000000 scottbrian_utils-4.0.1/src/scottbrian_utils/unique_ts.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.676960 scottbrian_utils-4.0.1/src/scottbrian_utils.egg-info/
+-rw-rw-rw-   0        0        0     7748 2024-05-15 02:40:10.000000 scottbrian_utils-4.0.1/src/scottbrian_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2638 2024-05-15 02:40:10.000000 scottbrian_utils-4.0.1/src/scottbrian_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 02:40:10.000000 scottbrian_utils-4.0.1/src/scottbrian_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-15 02:40:10.000000 scottbrian_utils-4.0.1/src/scottbrian_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 02:40:10.000000 scottbrian_utils-4.0.1/src/scottbrian_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.555527 scottbrian_utils-4.0.1/tests/
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.664453 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/
+-rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/__init__.py
+-rw-rw-rw-   0        0        0     8171 2023-11-24 21:49:34.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py
+-rw-rw-rw-   0        0        0     5699 2024-04-24 20:25:46.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/conftest.py
+-rw-rw-rw-   0        0        0   493189 2023-11-24 21:49:35.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_diag_msg.py
+-rw-rw-rw-   0        0        0   107052 2024-05-15 01:23:40.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_entry_trace.py
+-rw-rw-rw-   0        0        0    17147 2023-11-24 00:16:31.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_file_catalog.py
+-rw-rw-rw-   0        0        0     7704 2023-07-01 17:34:46.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_flower_box.py
+-rw-rw-rw-   0        0        0   152540 2024-05-10 20:20:22.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_log_verifier.py
+-rw-rw-rw-   0        0        0    15938 2024-05-08 01:06:25.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_msgs.py
+-rw-rw-rw-   0        0        0    36592 2023-11-24 00:15:56.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_pauser.py
+-rw-rw-rw-   0        0        0    17642 2023-07-01 17:34:46.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_stop_watch.py
+-rw-rw-rw-   0        0        0    77560 2024-04-22 00:08:46.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_time_hdr.py
+-rw-rw-rw-   0        0        0    40767 2023-11-23 15:44:47.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_timer.py
+-rw-rw-rw-   0        0        0     5972 2023-11-25 00:12:19.000000 scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_unique_ts.py
+-rw-rw-rw-   0        0        0     6635 2024-05-03 14:48:19.000000 scottbrian_utils-4.0.1/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.555527 scottbrian_utils-4.0.1/type_stubs/
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.666453 scottbrian_utils-4.0.1/type_stubs/mypywrapt/
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.668959 scottbrian_utils-4.0.1/type_stubs/mypywrapt/adjust_src/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/type_stubs/mypywrapt/adjust_src/__init__.pyi
+-rw-rw-rw-   0        0        0     1292 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/type_stubs/mypywrapt/adjust_src/adjust_src.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.556538 scottbrian_utils-4.0.1/type_stubs/mypywrapt/build/
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.556538 scottbrian_utils-4.0.1/type_stubs/mypywrapt/build/lib/
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.671959 scottbrian_utils-4.0.1/type_stubs/mypywrapt/build/lib/wrapt-stubs/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/type_stubs/mypywrapt/build/lib/wrapt-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/type_stubs/mypywrapt/build/lib/wrapt-stubs/decorators.pyi
+-rw-rw-rw-   0        0        0      388 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/type_stubs/mypywrapt/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:40:10.674960 scottbrian_utils-4.0.1/type_stubs/mypywrapt/wrapt-stubs/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/type_stubs/mypywrapt/wrapt-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.1/type_stubs/mypywrapt/wrapt-stubs/decorators.pyi
```

### Comparing `scottbrian_utils-4.0.0/.gitignore` & `scottbrian_utils-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/.idea/scottbrian_utils.iml` & `scottbrian_utils-4.0.1/.idea/scottbrian_utils.iml`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/.readthedocs.yml` & `scottbrian_utils-4.0.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/LICENSE.txt` & `scottbrian_utils-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/MANIFEST.in` & `scottbrian_utils-4.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/PKG-INFO` & `scottbrian_utils-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scottbrian_utils
-Version: 4.0.0
+Version: 4.0.1
 Summary: Miscellaneous utilities
 Author-email: Scott Tuttle <sbtuttle@outlook.com>
 License: MIT License
         
         Copyright (c) [2020] [Scott Tuttle]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -197,14 +197,16 @@
     * restructured log_verifier:
         * performance improvements
         * changes to clarify that regex patterns are used
         * changed report format
         * method add_pattern replaces deprecated method add_msg
         * method verify_match_results replaces deprecated verify_log_results
 
+* 4.0.1
+    * fix etrace to put 2 colons between file name and func
 
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-4.0.0/README.rst` & `scottbrian_utils-4.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,16 @@
     * restructured log_verifier:
         * performance improvements
         * changes to clarify that regex patterns are used
         * changed report format
         * method add_pattern replaces deprecated method add_msg
         * method verify_match_results replaces deprecated verify_log_results
 
+* 4.0.1
+    * fix etrace to put 2 colons between file name and func
 
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-4.0.0/conftest.py` & `scottbrian_utils-4.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/docs/source/UniqueTS_UseCase1.svg` & `scottbrian_utils-4.0.1/docs/source/UniqueTS_UseCase1.svg`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/docs/source/adjust_sphinx/adjust_sphinx.py` & `scottbrian_utils-4.0.1/docs/source/adjust_sphinx/adjust_sphinx.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/docs/source/conf.py` & `scottbrian_utils-4.0.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "scottbrian_utils"
 copyright = "2020, 2023, Scott Tuttle"
 author = "Scott Tuttle"
 
 # The full version, including alpha/beta/rc tags
-release = "4.0.0"
+release = "4.0.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `scottbrian_utils-4.0.0/docs/source/index.rst` & `scottbrian_utils-4.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/pyproject.toml` & `scottbrian_utils-4.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scottbrian_utils"
-version = "4.0.0"
+version = "4.0.1"
 description = "Miscellaneous utilities"
 readme = "README.rst"
 requires-python = "~=3.12"
 license = {file = "LICENSE.txt"}
 keywords = ["utilities"]
 authors = [{name = "Scott Tuttle", email = "sbtuttle@outlook.com"}]
 classifiers = [
```

### Comparing `scottbrian_utils-4.0.0/pytest.ini` & `scottbrian_utils-4.0.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/conftest.py` & `scottbrian_utils-4.0.1/src/conftest.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/diag_msg.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/diag_msg.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/doc_checker.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/doc_checker.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/entry_trace.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/entry_trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         pass
 
     f1()
 
 
 Expected trace output for Example 1::
 
-    test_entry_trace.py:f1:69 entry: caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example1:77
-    test_entry_trace.py:f1:69 exit: return_value=None
+    test_entry_trace.py::f1:69 entry: caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example1:77
+    test_entry_trace.py::f1:69 exit: return_value=None
 
 
 :Example 2: Decorate a function that has 1 positional arg and 1 keyword
             arg.
 
 .. code-block:: python
 
@@ -52,16 +52,16 @@
         return f"{a1=}, {kw1=}"
 
     f1(42, kw1="forty two")
 
 
 Expected trace output for Example 2::
 
-    test_entry_trace.py:f1:122 entry: a1=42, kw1='forty two', caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example2:130
-    test_entry_trace.py:f1:122 exit: return_value="a1=42, kw1='forty two'"
+    test_entry_trace.py::f1:122 entry: a1=42, kw1='forty two', caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example2:130
+    test_entry_trace.py::f1:122 exit: return_value="a1=42, kw1='forty two'"
 
 
 :Example 3: Decorate two functions, the first with etrace enabled and
             the second with etrace disabled.
 
 .. code-block:: python
 
@@ -80,16 +80,16 @@
         return f"{a1=}, {kw1=}"
 
     f1(42, kw1="forty two")
     f2(24, kw1="twenty four")
 
 Expected trace output for Example 3::
 
-    test_entry_trace.py:f1:180 entry: a1=42, kw1='forty two', caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example3:194
-    test_entry_trace.py:f1:180 exit: return_value="a1=42, kw1='forty two'"
+    test_entry_trace.py::f1:180 entry: a1=42, kw1='forty two', caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example3:194
+    test_entry_trace.py::f1:180 exit: return_value="a1=42, kw1='forty two'"
 
 
 :Example 4: Decorate a function with the positional arg omitted.
 
 .. code-block:: python
 
     from scottbrian_utils.entry_trace import etrace
@@ -98,16 +98,16 @@
     def f1(a1: int, kw1: str = "42") -> str:
         return f"{a1=}, {kw1=}"
 
     f1(42, kw1="forty two")
 
 Expected trace output for Example 4::
 
-    test_entry_trace.py:f1:244 entry: a1='...', kw1='forty two', caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example4:252
-    test_entry_trace.py:f1:244 exit: return_value="a1=42, kw1='forty two'"
+    test_entry_trace.py::f1:244 entry: a1='...', kw1='forty two', caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example4:252
+    test_entry_trace.py::f1:244 exit: return_value="a1=42, kw1='forty two'"
 
 
 :Example 5: Decorate a function with the first keyword arg omitted.
 
 .. code-block:: python
 
     from scottbrian_utils.entry_trace import etrace
@@ -116,16 +116,16 @@
     def f1(a1: int, kw1: str = "42", kw2: int = 24) -> str:
         return f"{a1=}, {kw1=}, {kw2=}"
 
     f1(42, kw1="forty two", kw2=84)
 
 Expected trace output for Example 5::
 
-    test_entry_trace.py:f1:300 entry: a1=42, kw1='...', kw2=84, caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example5:308
-    test_entry_trace.py:f1:300 exit: return_value="a1=42, kw1='forty two', kw2=84"
+    test_entry_trace.py::f1:300 entry: a1=42, kw1='...', kw2=84, caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example5:308
+    test_entry_trace.py::f1:300 exit: return_value="a1=42, kw1='forty two', kw2=84"
 
 
 :Example 6: Decorate a function with the return value omitted.
 
 .. code-block:: python
 
     from scottbrian_utils.entry_trace import etrace
@@ -134,16 +134,16 @@
     def f1(a1: int, kw1: str = "42", kw2: int = 24) -> str:
         return f"{a1=}, {kw1=}, {kw2=}"
 
     f1(42, kw1="forty two", kw2=84)
 
 Expected trace output for Example 6::
 
-    test_entry_trace.py:f1:347 entry: a1=42, kw1='forty two', kw2=84, caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example6:356
-    test_entry_trace.py:f1:347 exit: return value omitted
+    test_entry_trace.py::f1:347 entry: a1=42, kw1='forty two', kw2=84, caller: test_entry_trace.py::TestEntryTraceExamples.test_etrace_example6:356
+    test_entry_trace.py::f1:347 exit: return value omitted
 
   .. # noqa: E501, W505
 
 """
 
 ########################################################################
 # Standard Library
@@ -269,15 +269,15 @@
 
     skip_self_cls = False
     if len(qual_name_list) == 1 or qual_name_list[-2] == "<locals>":
         # set target_name to function name
         target_name = qual_name_list[-1]
     else:
         # set target_name to class name and method name
-        target_name = f":{qual_name_list[-2]}.{qual_name_list[-1]}"
+        target_name = f"{qual_name_list[-2]}.{qual_name_list[-1]}"
         if type(wrapped).__name__ != "staticmethod":
             skip_self_cls = True
 
     try:
         target_line_num: Union[int, str] = inspect.getsourcelines(wrapped)[1]
     except OSError:
         target_line_num = "?"
```

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/file_catalog.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/file_catalog.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/flower_box.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/flower_box.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/log_verifier.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/log_verifier.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/msgs.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/msgs.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/pauser.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/pauser.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/stop_watch.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/stop_watch.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/time_hdr.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/time_hdr.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/timer.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/timer.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils/unique_ts.py` & `scottbrian_utils-4.0.1/src/scottbrian_utils/unique_ts.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/PKG-INFO` & `scottbrian_utils-4.0.1/src/scottbrian_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scottbrian_utils
-Version: 4.0.0
+Version: 4.0.1
 Summary: Miscellaneous utilities
 Author-email: Scott Tuttle <sbtuttle@outlook.com>
 License: MIT License
         
         Copyright (c) [2020] [Scott Tuttle]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -197,14 +197,16 @@
     * restructured log_verifier:
         * performance improvements
         * changes to clarify that regex patterns are used
         * changed report format
         * method add_pattern replaces deprecated method add_msg
         * method verify_match_results replaces deprecated verify_log_results
 
+* 4.0.1
+    * fix etrace to put 2 colons between file name and func
 
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/SOURCES.txt` & `scottbrian_utils-4.0.1/src/scottbrian_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/conftest.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/conftest.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_diag_msg.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_diag_msg.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_entry_trace.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_entry_trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,28 +75,28 @@
         # mainline
         ################################################################
         log_ver = LogVer()
         f1()
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: "
             "caller: test_entry_trace.py::TestEntryTraceExamples."
             "test_etrace_example1:[0-9]+"
         )
 
         log_ver.add_pattern(
             level=logging.DEBUG,
             pattern=exp_entry_log_msg,
             log_name="scottbrian_utils.entry_trace",
             fullmatch=True,
         )
 
         exp_exit_log_msg = (
-            f"test_entry_trace.py:f1:{f1_line_num} exit: " f"return_value=None"
+            f"test_entry_trace.py::f1:{f1_line_num} exit: " f"return_value=None"
         )
 
         log_ver.add_pattern(
             level=logging.DEBUG,
             pattern=exp_exit_log_msg,
             log_name="scottbrian_utils.entry_trace",
             fullmatch=True,
@@ -128,30 +128,30 @@
         # mainline
         ################################################################
         log_ver = LogVer()
         f1(42, kw1="forty two")
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: a1=42, "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: a1=42, "
             "kw1='forty two', "
             "caller: test_entry_trace.py::TestEntryTraceExamples."
             "test_etrace_example2:[0-9]+"
         )
 
         log_ver.add_pattern(
             level=logging.DEBUG,
             pattern=exp_entry_log_msg,
             log_name="scottbrian_utils.entry_trace",
             fullmatch=True,
         )
         kw_value = "forty two"
         quote = "'"
         exp_exit_log_msg = (
-            f'test_entry_trace.py:f1:{f1_line_num} exit: return_value="a1=42, '
+            f'test_entry_trace.py::f1:{f1_line_num} exit: return_value="a1=42, '
             f'kw1={quote}{kw_value}{quote}"'
         )
 
         log_ver.add_pattern(
             level=logging.DEBUG,
             pattern=exp_exit_log_msg,
             log_name="scottbrian_utils.entry_trace",
@@ -194,30 +194,30 @@
         log_ver = LogVer()
         f1(42, kw1="forty two")
         f2(24, kw1="twenty four")
 
         f1_line_num = inspect.getsourcelines(f1)[1]
 
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: a1=42, "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: a1=42, "
             "kw1='forty two', "
             "caller: test_entry_trace.py::TestEntryTraceExamples."
             "test_etrace_example3:[0-9]+"
         )
 
         log_ver.add_pattern(
             level=logging.DEBUG,
             pattern=exp_entry_log_msg,
             log_name="scottbrian_utils.entry_trace",
             fullmatch=True,
         )
         kw_value = "forty two"
         quote = "'"
         exp_exit_log_msg = (
-            f'test_entry_trace.py:f1:{f1_line_num} exit: return_value="a1=42, '
+            f'test_entry_trace.py::f1:{f1_line_num} exit: return_value="a1=42, '
             f'kw1={quote}{kw_value}{quote}"'
         )
 
         log_ver.add_pattern(
             level=logging.DEBUG,
             pattern=exp_exit_log_msg,
             log_name="scottbrian_utils.entry_trace",
@@ -250,30 +250,30 @@
         # mainline
         ################################################################
         log_ver = LogVer()
         f1(42, kw1="forty two")
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: a1='...', "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: a1='...', "
             "kw1='forty two', "
             "caller: test_entry_trace.py::TestEntryTraceExamples."
             "test_etrace_example4:[0-9]+"
         )
 
         log_ver.add_pattern(
             level=logging.DEBUG,
             pattern=exp_entry_log_msg,
             log_name="scottbrian_utils.entry_trace",
             fullmatch=True,
         )
         kw_value = "forty two"
         quote = "'"
         exp_exit_log_msg = (
-            f'test_entry_trace.py:f1:{f1_line_num} exit: return_value="a1=42, '
+            f'test_entry_trace.py::f1:{f1_line_num} exit: return_value="a1=42, '
             f'kw1={quote}{kw_value}{quote}"'
         )
 
         log_ver.add_pattern(
             level=logging.DEBUG,
             pattern=exp_exit_log_msg,
             log_name="scottbrian_utils.entry_trace",
@@ -307,25 +307,25 @@
         ################################################################
         log_ver = LogVer(log_name="scottbrian_utils.entry_trace")
         f1(42, kw1="forty two", kw2=84)
 
         f1_line_num = inspect.getsourcelines(f1)[1]
 
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: a1=42, "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: a1=42, "
             "kw1='...', kw2=84, "
             "caller: test_entry_trace.py::TestEntryTraceExamples."
             "test_etrace_example5:[0-9]+"
         )
 
         log_ver.add_pattern(pattern=exp_entry_log_msg)
         kw_value = "forty two"
         quote = "'"
         exp_exit_log_msg = (
-            f'test_entry_trace.py:f1:{f1_line_num} exit: return_value="a1=42, '
+            f'test_entry_trace.py::f1:{f1_line_num} exit: return_value="a1=42, '
             f'kw1={quote}{kw_value}{quote}, kw2=84"'
         )
 
         log_ver.add_pattern(pattern=exp_exit_log_msg)
         ################################################################
         # check log results
         ################################################################
@@ -354,24 +354,24 @@
         ################################################################
         log_ver = LogVer(log_name="scottbrian_utils.entry_trace")
 
         f1(42, kw1="forty two", kw2=84)
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: a1=42, "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: a1=42, "
             "kw1='forty two', kw2=84, "
             "caller: test_entry_trace.py::TestEntryTraceExamples."
             "test_etrace_example6:[0-9]+"
         )
 
         log_ver.add_pattern(pattern=exp_entry_log_msg)
 
         exp_exit_log_msg = (
-            f"test_entry_trace.py:f1:{f1_line_num} exit: return value omitted"
+            f"test_entry_trace.py::f1:{f1_line_num} exit: return value omitted"
         )
 
         log_ver.add_pattern(pattern=exp_exit_log_msg)
         ################################################################
         # check log results
         ################################################################
         match_results = log_ver.get_match_results(caplog=caplog)
@@ -408,23 +408,23 @@
         # mainline
         ################################################################
         log_ver = LogVer(log_name="scottbrian_utils.entry_trace")
         f1()
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: "
             "caller: test_entry_trace.py::TestEntryTraceBasic."
             "test_etrace_on_function_no_parm:[0-9]+"
         )
 
         log_ver.add_pattern(pattern=exp_entry_log_msg)
 
         exp_exit_log_msg = (
-            f"test_entry_trace.py:f1:{f1_line_num} exit: return_value=None"
+            f"test_entry_trace.py::f1:{f1_line_num} exit: return_value=None"
         )
 
         log_ver.add_pattern(pattern=exp_exit_log_msg)
         ################################################################
         # check log results
         ################################################################
         match_results = log_ver.get_match_results(caplog=caplog)
@@ -715,22 +715,24 @@
         # mainline
         ################################################################
         log_ver = LogVer(log_name="scottbrian_utils.entry_trace")
         f1(42)
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: a1=42, "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: a1=42, "
             "caller: test_entry_trace.py::TestEntryTraceBasic."
             "test_etrace_on_function_one_parm:[0-9]+"
         )
 
         log_ver.add_pattern(pattern=exp_entry_log_msg)
 
-        exp_exit_log_msg = f"test_entry_trace.py:f1:{f1_line_num} exit: return_value=42"
+        exp_exit_log_msg = (
+            f"test_entry_trace.py::f1:{f1_line_num} exit: " "return_value=42"
+        )
 
         log_ver.add_pattern(pattern=exp_exit_log_msg)
         ################################################################
         # check log results
         ################################################################
         match_results = log_ver.get_match_results(caplog=caplog)
         log_ver.print_match_results(match_results, print_matched=True)
@@ -761,24 +763,24 @@
         # mainline
         ################################################################
         log_ver = LogVer(log_name="scottbrian_utils.entry_trace")
         f1(42, "forty_two", 83)
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: "
             r"args=\(42, 'forty_two', 83\), "
             "caller: test_entry_trace.py::TestEntryTraceBasic."
             "test_etrace_on_function_args:[0-9]+"
         )
 
         log_ver.add_pattern(pattern=exp_entry_log_msg)
 
         exp_exit_log_msg = (
-            f"test_entry_trace.py:f1:{f1_line_num} exit: "
+            f"test_entry_trace.py::f1:{f1_line_num} exit: "
             "return_value='42 forty_two 83 '"
         )
 
         log_ver.add_pattern(pattern=exp_exit_log_msg)
         ################################################################
         # check log results
         ################################################################
@@ -811,24 +813,24 @@
         # mainline
         ################################################################
         log_ver = LogVer(log_name="scottbrian_utils.entry_trace")
         f1(kw1=42, kw2="forty_two", kw3=83)
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: "
             "kw1=42, kw2='forty_two', kw3=83, "
             "caller: test_entry_trace.py::TestEntryTraceBasic."
             "test_etrace_on_function_kwargs:[0-9]+"
         )
 
         log_ver.add_pattern(pattern=exp_entry_log_msg)
 
         exp_exit_log_msg = (
-            f"test_entry_trace.py:f1:{f1_line_num} exit: return_value='kw1=42 "
+            f"test_entry_trace.py::f1:{f1_line_num} exit: return_value='kw1=42 "
             f"kw2=forty_two kw3=83 '"
         )
 
         log_ver.add_pattern(pattern=exp_exit_log_msg)
         ################################################################
         # check log results
         ################################################################
@@ -861,24 +863,24 @@
         # mainline
         ################################################################
         log_ver = LogVer(log_name="scottbrian_utils.entry_trace")
         f1(42, "forty_two", 83)
 
         f1_line_num = inspect.getsourcelines(f1)[1]
         exp_entry_log_msg = (
-            rf"test_entry_trace.py:f1:{f1_line_num} entry: "
+            rf"test_entry_trace.py::f1:{f1_line_num} entry: "
             r"a1=42, args=\('forty_two', 83\), "
             "caller: test_entry_trace.py::TestEntryTraceBasic."
             "test_etrace_on_function_args2:[0-9]+"
         )
 
         log_ver.add_pattern(pattern=exp_entry_log_msg)
 
         exp_exit_log_msg = (
-            f"test_entry_trace.py:f1:{f1_line_num} exit: "
+            f"test_entry_trace.py::f1:{f1_line_num} exit: "
             f"return_value='42 forty_two 83 '"
         )
 
         log_ver.add_pattern(pattern=exp_exit_log_msg)
         ################################################################
         # check log results
         ################################################################
@@ -1956,27 +1958,27 @@
 
                 for idx2, arg_spec_ret_res in enumerate(
                     omit_variation.arg_specs_ret_reses
                 ):
                     exec(f"f999({arg_spec_ret_res.arg_spec})")
 
                     exp_entry_log_msg = (
-                        rf"<string>:f1:\? entry: {arg_spec_ret_res.log_result}"
+                        rf"<string>::f1:\? entry: {arg_spec_ret_res.log_result}"
                         "caller: <string>:1"
                     )
 
                     log_ver.add_pattern(
                         level=logging.DEBUG,
                         pattern=exp_entry_log_msg,
                         log_name="scottbrian_utils.entry_trace",
                         fullmatch=True,
                     )
 
                     exp_exit_log_msg = (
-                        rf"<string>:f1:\? exit: return_value='"
+                        rf"<string>::f1:\? exit: return_value='"
                         rf"{arg_spec_ret_res.ret_result}'"
                     )
 
                     log_ver.add_pattern(
                         level=logging.DEBUG,
                         pattern=exp_exit_log_msg,
                         log_name="scottbrian_utils.entry_trace",
@@ -2061,15 +2063,15 @@
         ################################################################
         # choose the target function or method
         ################################################################
         target_rtn: Callable[[], None] | type[Target]
         if target_type_arg == FunctionType.Function:
             target_rtn = f1
             target_line_num = inspect.getsourcelines(f1)[1]
-            target_qual_name = ":f1"
+            target_qual_name = "::f1"
 
         elif target_type_arg == FunctionType.Method:
             target_rtn = Target().target
             target_line_num = inspect.getsourcelines(Target.target)[1]
             target_qual_name = "::Target.target"
 
         elif target_type_arg == FunctionType.StaticMethod:
@@ -2221,15 +2223,15 @@
         ################################################################
         # choose the target function or method
         ################################################################
         target_rtn: Callable[[], None] | type[Target]
         if target_type_arg == FunctionType.Function:
             target_rtn = f1
             target_line_num = inspect.getsourcelines(f1)[1]
-            target_qual_name = ":f1"
+            target_qual_name = "::f1"
 
         elif target_type_arg == FunctionType.Method:
             target_rtn = Target().target
             target_line_num = inspect.getsourcelines(Target.target)[1]
             target_qual_name = "::Target.target"
 
         elif target_type_arg == FunctionType.StaticMethod:
@@ -2440,15 +2442,15 @@
 
         ################################################################
         # choose the target function or method
         ################################################################
         if target_type_arg == FunctionType.Function:
             target_rtn = f1
             target_line_num = inspect.getsourcelines(f1)[1]
-            target_qual_name = ":f1"
+            target_qual_name = "::f1"
 
         elif target_type_arg == FunctionType.Method:
             target_rtn = Target().target
             target_line_num = inspect.getsourcelines(Target.target)[1]
             target_qual_name = "::Target.target"
 
         elif target_type_arg == FunctionType.StaticMethod:
@@ -2732,15 +2734,15 @@
         ################################################################
         # choose the target function or method
         ################################################################
         target_rtn: CallTarget | Callable[[str | int | list[Any] | float | None], Any]
         if target_type_arg == FunctionType.Function:
             target_rtn = f1
             target_line_num = inspect.getsourcelines(f1)[1]
-            target_qual_name = ":f1"
+            target_qual_name = "::f1"
 
         elif target_type_arg == FunctionType.Method:
             target_rtn = Target().target
             target_line_num = inspect.getsourcelines(Target.target)[1]
             target_qual_name = "::Target.target"
 
         elif target_type_arg == FunctionType.StaticMethod:
```

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_file_catalog.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_file_catalog.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_flower_box.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_flower_box.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_log_verifier.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_log_verifier.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_msgs.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_msgs.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_pauser.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_pauser.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_stop_watch.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_stop_watch.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_time_hdr.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_time_hdr.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_timer.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_timer.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_unique_ts.py` & `scottbrian_utils-4.0.1/tests/test_scottbrian_utils/test_unique_ts.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/tox.ini` & `scottbrian_utils-4.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-4.0.0/type_stubs/mypywrapt/adjust_src/adjust_src.py` & `scottbrian_utils-4.0.1/type_stubs/mypywrapt/adjust_src/adjust_src.py`

 * *Files identical despite different names*

