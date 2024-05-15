# Comparing `tmp/libvirt_provider-0.0.0a6.tar.gz` & `tmp/libvirt_provider-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvirt_provider-0.0.0a6.tar", last modified: Tue May 14 13:12:21 2024, max compression
+gzip compressed data, was "libvirt_provider-0.0.0a7.tar", last modified: Wed May 15 10:15:56 2024, max compression
```

## Comparing `libvirt_provider-0.0.0a6.tar` & `libvirt_provider-0.0.0a7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.335917 libvirt_provider-0.0.0a6/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5925 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4884 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/README.rst
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.327916 libvirt_provider-0.0.0a6/libvirt_provider/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2023-11-27 15:36:25.000000 libvirt_provider-0.0.0a6/libvirt_provider/__init__.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.327916 libvirt_provider-0.0.0a6/libvirt_provider/cli/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-19 09:44:41.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4890 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/cli.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2962 2024-03-12 08:00:51.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/helpers.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.327916 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-19 10:27:45.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      821 2024-03-25 19:57:56.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/container.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      528 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/driver.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      815 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/instance.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-19 09:44:41.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      625 2024-02-21 12:40:24.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/actions.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1271 2024-03-25 19:58:29.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/container.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1018 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/driver.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4295 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/instance.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      575 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/client.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      112 2023-11-30 12:31:27.000000 libvirt_provider-0.0.0a6/libvirt_provider/config.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider/container/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-04-25 12:21:54.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      323 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/create.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      293 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/get.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      333 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/ls.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      268 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/remove.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      263 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/container/stop.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1564 2024-03-12 08:00:51.000000 libvirt_provider-0.0.0a6/libvirt_provider/defaults.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2023-11-29 14:27:13.000000 libvirt_provider-0.0.0a6/libvirt_provider/helpers.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider/instance/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-21 12:14:32.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      317 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/create.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      287 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/get.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      326 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/ls.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      283 2024-04-25 07:54:46.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/remove.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      290 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/show.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      263 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/start.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      300 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/state.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      261 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/libvirt_provider/instance/stop.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    11797 2024-05-03 05:33:44.000000 libvirt_provider-0.0.0a6/libvirt_provider/models.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2304 2024-03-12 08:00:51.000000 libvirt_provider-0.0.0a6/libvirt_provider/pool.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2023-11-29 11:23:03.000000 libvirt_provider-0.0.0a6/libvirt_provider/types.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider/utils/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2023-11-29 11:28:42.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      195 2024-01-09 15:39:48.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/db.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       86 2024-02-19 09:44:41.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/format.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5840 2024-05-06 12:44:20.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/io.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      759 2024-05-06 10:05:11.000000 libvirt_provider-0.0.0a6/libvirt_provider/utils/user.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5925 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1797 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/SOURCES.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/dependency_links.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      202 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/entry_points.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      131 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/requires.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       17 2024-05-14 13:12:21.000000 libvirt_provider-0.0.0a6/libvirt_provider.egg-info/top_level.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2024-05-14 13:12:21.335917 libvirt_provider-0.0.0a6/setup.cfg
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1839 2024-02-19 09:44:41.000000 libvirt_provider-0.0.0a6/setup.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-05-14 13:12:21.331916 libvirt_provider-0.0.0a6/tests/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     3436 2024-03-07 19:16:40.000000 libvirt_provider-0.0.0a6/tests/test_dummy.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2995 2024-05-14 06:07:05.000000 libvirt_provider-0.0.0a6/tests/test_dummy_pool.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    11781 2024-05-06 16:30:51.000000 libvirt_provider-0.0.0a6/tests/test_libvirt.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      334 2024-04-25 07:54:46.000000 libvirt_provider-0.0.0a6/tests/test_libvirt_lxc.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5752 2024-05-06 16:32:24.000000 libvirt_provider-0.0.0a6/tests/test_libvirt_pool.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     7547 2024-05-14 11:49:50.000000 libvirt_provider-0.0.0a6/tests/test_libvirt_remote_node.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.130895 libvirt_provider-0.0.0a7/
+-rw-r--r--   0 rasmunk    (501) staff       (20)     5925 2024-05-15 10:15:56.130320 libvirt_provider-0.0.0a7/PKG-INFO
+-rw-r--r--   0 rasmunk    (501) staff       (20)     4884 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/README.rst
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.106630 libvirt_provider-0.0.0a7/libvirt_provider/
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a7/libvirt_provider/__init__.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.110691 libvirt_provider-0.0.0a7/libvirt_provider/cli/
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/__init__.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     4856 2024-05-15 09:44:03.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/cli.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     2962 2024-03-08 15:26:04.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/helpers.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.112321 libvirt_provider-0.0.0a7/libvirt_provider/cli/input_groups/
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/input_groups/__init__.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      821 2024-04-24 07:39:00.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/input_groups/container.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      528 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/input_groups/driver.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      815 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/input_groups/instance.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.114486 libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/__init__.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      625 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/actions.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     1271 2024-04-24 07:39:00.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/container.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     1018 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/driver.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     4295 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/instance.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      575 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/client.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      112 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a7/libvirt_provider/config.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.117335 libvirt_provider-0.0.0a7/libvirt_provider/container/
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/libvirt_provider/container/__init__.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      323 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/container/create.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      293 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/container/get.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      333 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/container/ls.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      268 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/container/remove.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      263 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/container/stop.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     1564 2024-03-08 15:22:37.000000 libvirt_provider-0.0.0a7/libvirt_provider/defaults.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a7/libvirt_provider/helpers.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.121600 libvirt_provider-0.0.0a7/libvirt_provider/instance/
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/__init__.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      317 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/create.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      287 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/get.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      326 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/ls.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      283 2024-04-24 07:39:00.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/remove.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      290 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/show.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      263 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/start.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      300 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/state.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      261 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/libvirt_provider/instance/stop.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)    11797 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/libvirt_provider/models.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     2304 2024-03-11 10:13:55.000000 libvirt_provider-0.0.0a7/libvirt_provider/pool.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a7/libvirt_provider/types.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.125014 libvirt_provider-0.0.0a7/libvirt_provider/utils/
+-rw-r--r--   0 rasmunk    (501) staff       (20)        0 2024-01-09 11:29:37.000000 libvirt_provider-0.0.0a7/libvirt_provider/utils/__init__.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      195 2024-01-09 14:47:26.000000 libvirt_provider-0.0.0a7/libvirt_provider/utils/db.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)       86 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a7/libvirt_provider/utils/format.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     5840 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/libvirt_provider/utils/io.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      759 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/libvirt_provider/utils/user.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.128733 libvirt_provider-0.0.0a7/libvirt_provider.egg-info/
+-rw-r--r--   0 rasmunk    (501) staff       (20)     5925 2024-05-15 10:15:56.000000 libvirt_provider-0.0.0a7/libvirt_provider.egg-info/PKG-INFO
+-rw-r--r--   0 rasmunk    (501) staff       (20)     1797 2024-05-15 10:15:56.000000 libvirt_provider-0.0.0a7/libvirt_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 rasmunk    (501) staff       (20)        1 2024-05-15 10:15:56.000000 libvirt_provider-0.0.0a7/libvirt_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 rasmunk    (501) staff       (20)      202 2024-05-15 10:15:56.000000 libvirt_provider-0.0.0a7/libvirt_provider.egg-info/entry_points.txt
+-rw-r--r--   0 rasmunk    (501) staff       (20)      131 2024-05-15 10:15:56.000000 libvirt_provider-0.0.0a7/libvirt_provider.egg-info/requires.txt
+-rw-r--r--   0 rasmunk    (501) staff       (20)       17 2024-05-15 10:15:56.000000 libvirt_provider-0.0.0a7/libvirt_provider.egg-info/top_level.txt
+-rw-r--r--   0 rasmunk    (501) staff       (20)       38 2024-05-15 10:15:56.131017 libvirt_provider-0.0.0a7/setup.cfg
+-rw-r--r--   0 rasmunk    (501) staff       (20)     1839 2024-02-26 11:35:23.000000 libvirt_provider-0.0.0a7/setup.py
+drwxr-xr-x   0 rasmunk    (501) staff       (20)        0 2024-05-15 10:15:56.127792 libvirt_provider-0.0.0a7/tests/
+-rw-r--r--   0 rasmunk    (501) staff       (20)     3436 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/tests/test_dummy.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     2995 2024-03-07 13:55:58.000000 libvirt_provider-0.0.0a7/tests/test_dummy_pool.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)    11781 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/tests/test_libvirt.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)      334 2024-04-24 07:39:00.000000 libvirt_provider-0.0.0a7/tests/test_libvirt_lxc.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     5752 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/tests/test_libvirt_pool.py
+-rw-r--r--   0 rasmunk    (501) staff       (20)     6049 2024-05-15 09:42:57.000000 libvirt_provider-0.0.0a7/tests/test_libvirt_remote_node.py
```

### Comparing `libvirt_provider-0.0.0a6/PKG-INFO` & `libvirt_provider-0.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libvirt_provider
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: A corc plugin for a libvirt orchestration provider
 Home-page: https://github.com/rasmunk/libvirt_provider
 Author: Rasmus Munk
 Author-email: munk1@live.dk
 License: MIT
 Keywords: Orchstration,Virtual Machine
 Classifier: Intended Audience :: Developers
```

### Comparing `libvirt_provider-0.0.0a6/README.rst` & `libvirt_provider-0.0.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/cli.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 module_name="{}".format(libvirt_cli_type),
                 func_name=operation,
                 provider_groups=provider_groups,
                 argument_groups=argument_groups,
             )
 
 
-def libvirt_provider_cli(commands):
+def cli(commands):
     for libvirt_cli_structure in LIBVIRT_CLI_STRUCTURE:
         for libvirt_cli_type, libvirt_cli_operations in libvirt_cli_structure.items():
             function_provider = commands.add_parser(libvirt_cli_type)
             function_parser = function_provider.add_subparsers(title="COMMAND")
             if has_driver_group(libvirt_cli_type):
                 add_driver_group(function_provider, libvirt_cli_type)
             recursive_add_libvirt_operations(
@@ -95,15 +95,15 @@
 
 def run():
     parser = argparse.ArgumentParser(
         prog=PACKAGE_NAME, formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
     commands = parser.add_subparsers(title="COMMAND")
     # Add libvirt functions to the CLI
-    libvirt_provider_cli(commands)
+    cli(commands)
     args = parser.parse_args()
     # Convert to a dictionary
     arguments = vars(args)
     # Execute default function
     if "func" in arguments:
         func = arguments.pop("func")
         success, response = func(arguments)
```

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/helpers.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/container.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/input_groups/container.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/driver.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/input_groups/driver.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/input_groups/instance.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/input_groups/instance.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/actions.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/actions.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/container.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/container.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/driver.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/driver.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/cli/parsers/instance.py` & `libvirt_provider-0.0.0a7/libvirt_provider/cli/parsers/instance.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/client.py` & `libvirt_provider-0.0.0a7/libvirt_provider/client.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/defaults.py` & `libvirt_provider-0.0.0a7/libvirt_provider/defaults.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/models.py` & `libvirt_provider-0.0.0a7/libvirt_provider/models.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/pool.py` & `libvirt_provider-0.0.0a7/libvirt_provider/pool.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/utils/io.py` & `libvirt_provider-0.0.0a7/libvirt_provider/utils/io.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider/utils/user.py` & `libvirt_provider-0.0.0a7/libvirt_provider/utils/user.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider.egg-info/PKG-INFO` & `libvirt_provider-0.0.0a7/libvirt_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libvirt_provider
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: A corc plugin for a libvirt orchestration provider
 Home-page: https://github.com/rasmunk/libvirt_provider
 Author: Rasmus Munk
 Author-email: munk1@live.dk
 License: MIT
 Keywords: Orchstration,Virtual Machine
 Classifier: Intended Audience :: Developers
```

### Comparing `libvirt_provider-0.0.0a6/libvirt_provider.egg-info/SOURCES.txt` & `libvirt_provider-0.0.0a7/libvirt_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/setup.py` & `libvirt_provider-0.0.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/tests/test_dummy.py` & `libvirt_provider-0.0.0a7/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/tests/test_dummy_pool.py` & `libvirt_provider-0.0.0a7/tests/test_dummy_pool.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/tests/test_libvirt.py` & `libvirt_provider-0.0.0a7/tests/test_libvirt.py`

 * *Files identical despite different names*

### Comparing `libvirt_provider-0.0.0a6/tests/test_libvirt_pool.py` & `libvirt_provider-0.0.0a7/tests/test_libvirt_pool.py`

 * *Files identical despite different names*

