# Comparing `tmp/popoll_backend-0.0.51.tar.gz` & `tmp/popoll_backend-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.51.tar", last modified: Tue May 14 09:43:19 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.52.tar", last modified: Wed May 15 21:15:04 2024, max compression
```

## Comparing `popoll_backend-0.0.51.tar` & `popoll_backend-0.0.52.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 09:43:19.244957 popoll_backend-0.0.51/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-14 09:43:19.244957 popoll_backend-0.0.51/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 09:43:19.229957 popoll_backend-0.0.51/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     6871 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 09:43:19.230958 popoll_backend-0.0.51/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 09:43:19.232957 popoll_backend-0.0.51/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 09:43:19.234958 popoll_backend-0.0.51/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/date_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/dates_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/instruments_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/user.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/user_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/users_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 09:43:19.239957 popoll_backend-0.0.51/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     1934 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/create_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1563 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 09:43:19.243957 popoll_backend-0.0.51/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-14 09:43:19.000000 popoll_backend-0.0.51/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2538 2024-05-14 09:43:19.000000 popoll_backend-0.0.51/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 09:43:19.000000 popoll_backend-0.0.51/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-14 09:43:19.000000 popoll_backend-0.0.51/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-14 09:43:19.000000 popoll_backend-0.0.51/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-14 09:43:13.000000 popoll_backend-0.0.51/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 09:43:19.244957 popoll_backend-0.0.51/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 09:43:19.243957 popoll_backend-0.0.51/tests/
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_01_db_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_02_simple_adds.py
--rw-rw-rw-   0 root         (0) root         (0)     1232 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_03_no_duplicates.py
--rw-rw-rw-   0 root         (0) root         (0)     1653 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_04_update_user_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_05_update_date_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_06_update_answer_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_07_delete_user_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_08_delete_date_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_09_delete_user_date_entries.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_10_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_11_get_users_sort_name.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_12_get_dates_sort_dateTime.py
--rw-rw-rw-   0 root         (0) root         (0)     2887 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_13_history.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_14_get_answers_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_15_multi_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     5130 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_16_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_17_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_18_post_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_19_delete_database.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_20_add_answer_no_dupe.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-14 09:42:57.000000 popoll_backend-0.0.51/tests/test_21_get_dates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.984267 popoll_backend-0.0.52/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-15 21:15:04.984267 popoll_backend-0.0.52/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.970267 popoll_backend-0.0.52/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     6871 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.971267 popoll_backend-0.0.52/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.973267 popoll_backend-0.0.52/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.975267 popoll_backend-0.0.52/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/date_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/dates_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/instruments_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/user_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/users_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.979267 popoll_backend-0.0.52/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.984267 popoll_backend-0.0.52/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-15 21:14:59.000000 popoll_backend-0.0.52/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 21:15:04.984267 popoll_backend-0.0.52/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.983267 popoll_backend-0.0.52/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_01_db_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_02_simple_adds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_03_no_duplicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_04_update_user_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_05_update_date_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_06_update_answer_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_07_delete_user_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_08_delete_date_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_09_delete_user_date_entries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_10_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_11_get_users_sort_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_12_get_dates_sort_dateTime.py
+-rw-rw-rw-   0 root         (0) root         (0)     2887 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_13_history.py
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_14_get_answers_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_15_multi_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     5130 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_16_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_17_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_18_post_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_19_delete_database.py
+-rw-rw-rw-   0 root         (0) root         (0)      537 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_20_add_answer_no_dupe.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_21_get_dates.py
```

### Comparing `popoll_backend-0.0.51/PKG-INFO` & `popoll_backend-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.51
+Version: 0.0.52
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.51/popoll_backend/__main__.py` & `popoll_backend-0.0.52/popoll_backend/__main__.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.52/popoll_backend/model/db/answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/model/db/date.py` & `popoll_backend-0.0.52/popoll_backend/model/db/date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/model/db/session.py` & `popoll_backend-0.0.52/popoll_backend/model/db/session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/model/db/user_instruments.py` & `popoll_backend-0.0.52/popoll_backend/model/db/user_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/model/payload/date_payload.py` & `popoll_backend-0.0.52/popoll_backend/model/payload/date_payload.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.52/popoll_backend/model/payload/history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/model/payload/user.py` & `popoll_backend-0.0.52/popoll_backend/model/payload/user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/model/payload/user_payload.py` & `popoll_backend-0.0.52/popoll_backend/model/payload/user_payload.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.52/popoll_backend/query/create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/create_date.py` & `popoll_backend-0.0.52/popoll_backend/query/create_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/create_instrument.py` & `popoll_backend-0.0.52/popoll_backend/query/create_instrument.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.52/popoll_backend/query/create_poll.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.id_payload import IdPayload
 from popoll_backend.query import Query
 
 
 class CreatePoll(Query):
     
+    fail_if_db_exists: bool = True
+    fail_if_db_not_exists: bool = False
+    
     name: str
     instruments: List[str]
     color: str
     
     def __init__(self, poll:str, name: str, instruments: List[str], color: str):
-        super().__init__(poll, isNoDBFileRequired=True)
+        super().__init__(poll)
         self.name = name
         self.instruments = instruments
         self.color = color
     
     def process(self, cursor: sqlite3.Cursor):
         cursor.execute(Option.create_table())
         cursor.execute('INSERT INTO options(name, color) values(?, ?)', (self.name, self.color))
```

### Comparing `popoll_backend-0.0.51/popoll_backend/query/create_session.py` & `popoll_backend-0.0.52/popoll_backend/query/create_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/create_user.py` & `popoll_backend-0.0.52/popoll_backend/query/create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.52/popoll_backend/query/delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.52/popoll_backend/query/delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.52/popoll_backend/query/delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/get_answer.py` & `popoll_backend-0.0.52/popoll_backend/query/get_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/get_date.py` & `popoll_backend-0.0.52/popoll_backend/query/get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.52/popoll_backend/query/get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.52/popoll_backend/query/get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/get_search_answer.py` & `popoll_backend-0.0.52/popoll_backend/query/get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/get_session.py` & `popoll_backend-0.0.52/popoll_backend/query/get_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/get_user.py` & `popoll_backend-0.0.52/popoll_backend/query/get_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/get_users.py` & `popoll_backend-0.0.52/popoll_backend/query/get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/update_answer.py` & `popoll_backend-0.0.52/popoll_backend/query/update_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/update_date.py` & `popoll_backend-0.0.52/popoll_backend/query/update_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/update_poll.py` & `popoll_backend-0.0.52/popoll_backend/query/update_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend/query/update_user.py` & `popoll_backend-0.0.52/popoll_backend/query/update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.52/popoll_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.51
+Version: 0.0.52
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.51/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.52/popoll_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/pyproject.toml` & `popoll_backend-0.0.52/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", 'wheel', 'flask', 'flask_cors', 'flask-restful', 'jsonpickle', 'sqlalchemy', 'sqlalchemy-utils', 'psycopg2-binary', 'pyyaml', 'pyopenssl']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "popoll_backend"
-version = "0.0.51"
+version = "0.0.52"
 authors = [
   { name="vivi5421", email="pypi@villard.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `popoll_backend-0.0.51/tests/test_01_db_creation.py` & `popoll_backend-0.0.52/tests/test_01_db_creation.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_02_simple_adds.py` & `popoll_backend-0.0.52/tests/test_02_simple_adds.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_03_no_duplicates.py` & `popoll_backend-0.0.52/tests/test_03_no_duplicates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_04_update_user_entry.py` & `popoll_backend-0.0.52/tests/test_04_update_user_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_05_update_date_entry.py` & `popoll_backend-0.0.52/tests/test_05_update_date_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_06_update_answer_entry.py` & `popoll_backend-0.0.52/tests/test_06_update_answer_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_07_delete_user_entry.py` & `popoll_backend-0.0.52/tests/test_07_delete_user_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_08_delete_date_entry.py` & `popoll_backend-0.0.52/tests/test_08_delete_date_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_09_delete_user_date_entries.py` & `popoll_backend-0.0.52/tests/test_09_delete_user_date_entries.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_10_get_users.py` & `popoll_backend-0.0.52/tests/test_10_get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_11_get_users_sort_name.py` & `popoll_backend-0.0.52/tests/test_11_get_users_sort_name.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_12_get_dates_sort_dateTime.py` & `popoll_backend-0.0.52/tests/test_12_get_dates_sort_dateTime.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_13_history.py` & `popoll_backend-0.0.52/tests/test_13_history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_14_get_answers_user.py` & `popoll_backend-0.0.52/tests/test_14_get_answers_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_15_multi_instruments.py` & `popoll_backend-0.0.52/tests/test_15_multi_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_16_get_date.py` & `popoll_backend-0.0.52/tests/test_16_get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_20_add_answer_no_dupe.py` & `popoll_backend-0.0.52/tests/test_20_add_answer_no_dupe.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.51/tests/test_21_get_dates.py` & `popoll_backend-0.0.52/tests/test_21_get_dates.py`

 * *Files identical despite different names*

