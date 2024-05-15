# Comparing `tmp/fnschool-20240513.614.21.tar.gz` & `tmp/fnschool-20240515.322.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240513.614.21.tar", last modified: Sun May 12 22:14:23 2024, max compression
+gzip compressed data, was "fnschool-20240515.322.21.tar", last modified: Tue May 14 19:22:26 2024, max compression
```

## Comparing `fnschool-20240513.614.21.tar` & `fnschool-20240515.322.21.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.891404 fnschool-20240513.614.21/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 22:14:23.890403 fnschool-20240513.614.21/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-12 22:14:23.891404 fnschool-20240513.614.21/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.870401 fnschool-20240513.614.21/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.876402 fnschool-20240513.614.21/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-12 22:14:21.000000 fnschool-20240513.614.21/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.883403 fnschool-20240513.614.21/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240513.614.21/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13812 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6175 2024-05-12 21:46:20.000000 fnschool-20240513.614.21/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/consume.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.885403 fnschool-20240513.614.21/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240513.614.21/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240513.614.21/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240513.614.21/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-11 17:45:02.000000 fnschool-20240513.614.21/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240513.614.21/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240513.614.21/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2484 2024-05-12 19:33:41.000000 fnschool-20240513.614.21/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2804 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.888403 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2332 2024-05-12 21:46:19.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10292 2024-05-12 21:46:20.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1823 2024-05-12 19:33:41.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1893 2024-05-12 21:46:19.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5208 2024-05-12 21:46:20.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9360 2024-05-12 19:33:42.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7241 2024-05-12 20:48:06.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7013 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8829 2024-05-12 20:01:28.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2290 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3990 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9595 2024-05-12 20:57:04.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98369 2024-05-12 20:36:18.000000 fnschool-20240513.614.21/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240513.614.21/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.888403 fnschool-20240513.614.21/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-12 17:45:50.000000 fnschool-20240513.614.21/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1231 2024-05-12 22:13:50.000000 fnschool-20240513.614.21/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.872402 fnschool-20240513.614.21/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.871402 fnschool-20240513.614.21/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.889403 fnschool-20240513.614.21/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.871402 fnschool-20240513.614.21/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.889403 fnschool-20240513.614.21/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    15614 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.871402 fnschool-20240513.614.21/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.889403 fnschool-20240513.614.21/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.872402 fnschool-20240513.614.21/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.889403 fnschool-20240513.614.21/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.872402 fnschool-20240513.614.21/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.890403 fnschool-20240513.614.21/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-12 17:45:50.000000 fnschool-20240513.614.21/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-12 07:39:38.000000 fnschool-20240513.614.21/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.890403 fnschool-20240513.614.21/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240515.322.21/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240515.322.21/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240515.322.21/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.300031 fnschool-20240515.322.21/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.306031 fnschool-20240515.322.21/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.313032 fnschool-20240515.322.21/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-14 16:35:32.000000 fnschool-20240515.322.21/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6303 2024-05-14 19:01:24.000000 fnschool-20240515.322.21/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240515.322.21/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/consume.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.315032 fnschool-20240515.322.21/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-14 13:17:04.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-14 18:35:22.000000 fnschool-20240515.322.21/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-14 18:45:28.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-14 17:46:32.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1862 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1890 2024-05-14 17:12:30.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5695 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9357 2024-05-14 17:11:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8248 2024-05-14 18:51:12.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7193 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9722 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2286 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-14 18:25:45.000000 fnschool-20240515.322.21/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240515.322.21/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1298 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.301031 fnschool-20240515.322.21/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.301031 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    17269 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.303031 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.321032 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.321032 fnschool-20240515.322.21/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240513.614.21/LICENSE` & `fnschool-20240515.322.21/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/PKG-INFO` & `fnschool-20240515.322.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240513.614.21
+Version: 20240515.322.21
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240513.614.21/README.md` & `fnschool-20240515.322.21/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/pyproject.toml` & `fnschool-20240515.322.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/__init__.py` & `fnschool-20240515.322.21/src/fnschool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openpyxl import load_workbook
 from fnschool.language import _
 from fnschool.log import *
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 
-__version__ = "20240513.0614.21"
+__version__ = "20240515.0322.21"
 
 
 def print_app_name():
     app_name0 = [
         r" _____ _   _ ____   ____ _   _  ___   ___  _     ",
         r"|  ___| \ | / ___| / ___| | | |/ _ \ / _ \| |    ",
         r"| |_  |  \| \___ \| |   | |_| | | | | | | | |    ",
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/bill.cp.py` & `fnschool-20240515.322.21/src/fnschool/canteen/bill.cp.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
                     + "add the purchasing information of them into "
                     + "the end of the purchasing spreadsheet (e.g: "
                     + "the spreadsheets Changsheng provided)."
                 )
             )
         if has_tip:
             print_warning(_("Ok! I knew that.(press any key to continue)"))
-            input()
+            input(">_ ")
 
     def make_spreadsheet_by_time_nodes(self):
         self.set_profile_to_index0()
         self.print_basic_info()
 
         self.get_time_nodes()
         self.get_month()
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/bill.py` & `fnschool-20240515.322.21/src/fnschool/canteen/bill.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,19 @@
                     for name_like in name_likes:
                         if not name_like in user_name_likes:
                             user_name_likes.append(name_like)
                     self._food_classes[fclass] = user_name_likes
                 else:
                     self._food_classes[fclass] = name_likes
 
+            print_info(
+                _("Ok! I know it. (Press any key to continue)")
+            )
+            input(">_ ")
+
         return self._food_classes
 
     @property
     def operator(self):
         if not self._operator:
             self._operator = Operator(self)
         return self._operator
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/canteen.toml` & `fnschool-20240515.322.21/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/config.py` & `fnschool-20240515.322.21/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240515.322.21/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240515.322.21/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240515.322.21/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/food.cp.py` & `fnschool-20240515.322.21/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/food.py` & `fnschool-20240515.322.21/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/food_classes.toml` & `fnschool-20240515.322.21/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/operator.py` & `fnschool-20240515.322.21/src/fnschool/canteen/operator.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,67 +27,86 @@
                 with open(operator_name_fpath, "w", encoding="utf-8") as f:
                     f.write(self._name)
                 print_info(
                     _('Your name has been saved to "{0}".').format(
                         operator_name_fpath
                     )
                 )
+            else:
+                print_info(
+                    _(
+                        "Hi, your name is \"{0}\"? (Yes: 'Y' 'y' '', or enter your name)"
+                    ).format(self._name)
+                )
+                n_input = input(">_ ").replace(" ", "")
+                if len(n_input) > 1:
+                    with open(operator_name_fpath, "w", encoding="utf-8") as f:
+                        f.write(n_input)
+                    print_info(
+                        _('Ok, your name has been saved to "{0}".').format(
+                            operator_name_fpath
+                        )
+                    )
+                    self._name = n_input
+
         return self._name
 
     @property
     def dpath(self):
         if not self._dpath:
             self._dpath = user_config_dir / self.name
             if not self._dpath.exists():
                 os.makedirs(self._dpath, exist_ok=True)
         make_link(self._dpath, self.link_dpath)
         return self._dpath
 
     @property
     def preconsuming_dpath(self):
-        dpath = self.dpath / "preconsuming"
+        dpath = self.dpath / _("preconsuming")
         if not dpath.exists():
             os.makedirs(dpath, exist_ok=True)
         return dpath
 
     @property
     def link_dpath(self):
         dpath0 = canteen_links_dpath / self.name
         dpath1 = user_documents_dpath / app_name / self.name
         dpath = dpath0
         return dpath
 
     @property
     def config_dpath(self):
-        dpath = self.dpath / "config"
+        dpath = self.dpath / _("config")
         if not dpath.exists():
             os.makedirs(dpath, exist_ok=True)
         return dpath
 
     @property
     def food_classes_fpath(self):
         fpath = self.config_dpath / "food_classes.toml"
         if not fpath.exists():
             shutil.copy(food_classes_config0_fpath, fpath)
         return fpath
 
     @property
     def bill_dpath(self):
-        dpath = self.dpath / "bill"
+        dpath = self.dpath / _("bill")
         if not dpath.exists():
             os.makedirs(dpath)
         return dpath
 
     @property
     def bill_fpath(self):
-        fpath = self.bill_dpath / "bill.xlsx"
+        fpath = self.bill_dpath / (_("bill") + ".xlsx")
         if not fpath.exists():
             shutil.copy(bill0_fpath, fpath)
         return fpath
 
     @property
     def bill_fpath_uuid(self):
-        fpath = self.bill_fpath.parent / ("bill." + str(uuid.uuid4()) + ".xlsx")
+        fpath = self.bill_fpath.parent / (
+            _("bill") + "." + str(uuid.uuid4()) + ".xlsx"
+        )
         return fpath
 
 
 # The end.
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/path.py` & `fnschool-20240515.322.21/src/fnschool/canteen/path.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 if not canteen_links_dpath.exists():
     os.makedirs(canteen_links_dpath, exist_ok=True)
 
 if not operator_name_fpath.exists():
     with open(operator_name_fpath, "w", encoding="utf-8") as f:
         f.write("")
-    os.link(operator_name_fpath.as_posix(), operator_name_link_fpath.as_posix())
+    os.link(
+        operator_name_fpath.as_posix(), operator_name_link_fpath.as_posix()
+    )
 
 
 def get_food_classes_config_fpath(user_name):
     fpath = user_config_dir / user_name / "food_classes.toml"
 
     if not fpath.exists():
         shutil.copy(food_classes_config0_fpath, fpath)
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/profile.py` & `fnschool-20240515.322.21/src/fnschool/canteen/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,17 @@
                         + "    ]\n"
                         + "]\n"
                         + "# {the_end}"
                     ).format(
                         profile_label=_("Profile label"),
                         operator_name=_("Operator name"),
                         operator_email=_("Operator email"),
-                        organization_name=_("Organization name or school name"),
+                        organization_name=_(
+                            "Organization name or school name"
+                        ),
                         supplier_name_1=_("Supplier name 1"),
                         supplier_name_2=_("Supplier name 2"),
                         the_end=_("The end."),
                     )
                 )
             print_warning(_("Please update your profile file."))
             print_info(
@@ -61,15 +63,15 @@
                     "Profile label for data directory making, "
                     + "it shouldn't contain any space character.\n"
                     + "Supplier names are the supplier's alias."
                 )
             )
             open_file(self.fpath)
             print_info(_("Ok! it was configured. (enter any key)"))
-            input()
+            input(">_ ")
 
         with open(self.fpath, "r", encoding="utf-8") as f:
             profile = tomllib.load(f)["profile"]
             profile = Profile(
                 label=profile[0],
                 name=profile[1],
                 email=profile[2],
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from fnschool.canteen.spreadsheet.base import *
 
 
 class Consuming(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
-        self.sheet_name = "出库单"
+        self.sheet_name = self.s.consuming_name
+        self.entry_row_len0 = 21
         pass
 
     @property
     def form_indexes(self):
         if not self._form_indexes:
             csheet = self.sheet
             indexes = []
@@ -205,14 +206,16 @@
                     max_row=food_index1,
                     min_col=2,
                     max_col=7,
                 ):
                     for cell in row:
                         cell.value = ""
 
+        self.del_form_empty_row(2)
+
         self.format()
 
         wb = self.bwb
         wb.active = csheet
         print_info(_("Sheet '%s' was updated.") % self.sheet.title)
 
     def format(self):
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from fnschool.canteen.food import *
 from fnschool.canteen.spreadsheet.base import *
 
 
 class ConsumingSum(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
-        self.sheet_name = "出库汇总表"
+        self.sheet_name = self.s.consumingsum_name
         pass
 
     def update(self):
         cssheet = self.sheet
         year = self.bfoods[-1].xdate.year
         month = self.bfoods[-1].xdate.month
         day = self.consuming_day_m1
@@ -29,15 +29,17 @@
                         [
                             _count * food.unit_price
                             for _date, _count in food.consumptions
                         ]
                     )
             total_price += m_total_price
             cssheet.cell(row[0].row, 2, m_total_price)
-            cssheet.cell(row[0].row, 2).number_format = numbers.FORMAT_NUMBER_00
+            cssheet.cell(row[0].row, 2).number_format = (
+                numbers.FORMAT_NUMBER_00
+            )
 
         total_price_CNY = self.bill.get_CNY_chars(total_price)
         cssheet.cell(
             2,
             1,
             f"编制单位：{self.purchaser}       "
             + f"单位：元         "
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from fnschool import *
 from fnschool.canteen.spreadsheet.base import *
 
 
 class Cover(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
-        self.sheet_name = "六大类总封面"
+        self.sheet_name = self.s.cover_name
         pass
 
     def update(self):
         year = self.bfoods[-1].xdate.year
         month = self.bfoods[-1].xdate.month
         day = self.consuming_day_m1
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,25 @@
         self._warehousing = None
         self._unwareshousing = None
         self._purchasingsum = None
         self._consumingsum = None
         self._sfood = None
         self._cover = None
 
+        self.preconsuming_name0 = "出库计划表"
+        self.purchasing_name = None
+        self.consuming_name = "出库单"
+        self.inventory_name = "食材盘存表"
+        self.warehousing_name = "入库单"
+        self.unwarehousing_name = "未入库明细表"
+        self.purchasingsum_name = "入库、未入库汇总表"
+        self.consumingsum_name = "出库汇总表"
+        self.sfood_name = "材料台账母表"
+        self.cover_name = "六大类总封面"
+
     @property
     def bill_fpath(self):
         if not self._bill_fpath:
             self._bill_fpath = self.bill.operator.bill_fpath
         return self._bill_fpath
 
     @property
@@ -144,15 +155,15 @@
         s_input = input(">_ ")
 
         print()
         print_info(_("Saving. . ."))
 
         if len(s_input) > 0 and s_input in "Yy":
             self.bwb.save(self.operator.bill_fpath)
-            bill_fpath0 = sefl.operator.bill_fpath
+            bill_fpath0 = self.operator.bill_fpath
             print_info(
                 _(
                     "You can fill in the monthly missing data "
                     + "to food sheets, they will be saved "
                     + "for next updating."
                 )
             )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/food.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from fnschool import *
 from fnschool.canteen.spreadsheet.base import *
 
 
 class Food(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
-        self.sheet_name = "材料台账母表"
+        self.sheet_name = self.s.sfood_name
         pass
 
     def get_sheet(self, name=None):
         sheet = None
         if name in self.bwb.sheetnames:
             sheet = self.bwb[name]
         else:
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from fnschool import *
 from fnschool.canteen.spreadsheet.base import *
 
 
 class Inventory(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
-        self.sheet_name = "食材盘存表"
+        self.sheet_name = self.s.inventory_name
+        self.entry_row_len0 = 17
         pass
 
     def format(self):
         sheet = self.sheet
         self.unmerge_sheet_cells(sheet)
 
         for row in sheet.iter_rows(
@@ -129,15 +130,18 @@
                 tn = list(set(tn))
                 tn.remove(0)
             tn0, tn1 = tn[0], tn[-1]
             for d in range(tn1, tn0 - 1, -1):
                 d_date = datetime(year, month, d)
                 if d_date in consuming_dates:
                     foods.append(
-                        [d_date, [f for f in bfoods if f.get_remainder(d_date)]]
+                        [
+                            d_date,
+                            [f for f in bfoods if f.get_remainder(d_date)],
+                        ]
                     )
                     break
         return foods
 
     def update(self):
         sheet = self.sheet
         tnfoods = self.foods
@@ -170,14 +174,30 @@
                 1,
                 f"     "
                 + f"学校名称：{self.purchaser}"
                 + f"                "
                 + f"{t1.year} 年 {t1.month} 月 {t1.day} 日"
                 + f"              ",
             )
+            sheet.cell(
+                form_i1 + 2,
+                1,
+                (
+                    "   "
+                    + "审核人："
+                    + "        "
+                    + "经办人："
+                    + self.operator.name
+                    + "　    "
+                    + "过称人："
+                    + "        "
+                    + "仓管人："
+                    + " 　     "
+                ),
+            )
 
             for row in sheet.iter_rows(
                 min_row=fentry_i0,
                 max_row=fentry_i1,
                 min_col=1,
                 max_col=9,
             ):
@@ -188,16 +208,25 @@
 
             for findex, food in enumerate(_foods):
                 row_index = fentry_i0 + findex
                 if (
                     sheet.cell(row_index + 1, 1).value.replace(" ", "")
                     == "合计"
                 ):
-                    self.row_inserting_tip(row_index + 1)
-                    sheet.insert_rows(row_index + 1, 1)
+                    i_row_index = row_index + 1
+                    self.row_inserting_tip(i_row_index)
+                    sheet.insert_rows(i_row_index, 1)
+
+                    for i_col_index in range(1, 10):
+                        cell = sheet.cell(i_row_index, i_col_index)
+                        cell.alignment = self.cell_alignment0
+                        cell.border = self.cell_border0
+
+                    self.del_form_indexes()
+                    form_indexes = self.form_indexes
                 sheet.cell(row_index, 1, food.name)
                 sheet.cell(row_index, 2, food.unit_name)
                 sheet.cell(row_index, 3, food.get_remainder(t1))
                 sheet.cell(
                     row_index,
                     4,
                     food.get_remainder(t1) * food.unit_price,
@@ -205,14 +234,15 @@
                 sheet.cell(row_index, 5, food.get_remainder(t1))
                 sheet.cell(
                     row_index,
                     6,
                     food.get_remainder(t1) * food.unit_price,
                 )
 
+        self.del_form_empty_row(1)
         self.format()
 
         wb = self.bwb
         wb.active = sheet
         print_info(_("Sheet '%s' was updated.") % (self.sheet_name))
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 class PreConsuming(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
         self.path0 = pre_consuming0_fpath
         self.row_index_offset = 3
         self.col_index_offset = 5
 
-        self.sheet_name0 = "出库计划表"
+        self.sheet_name0 = self.s.preconsuming_name0
 
     def pre_consume_foods(self, foods):
         cfoods = [f for f in foods if not f.is_abandoned]
+        if len(cfoods) < 1:
+            print_error(_("No food found, exit."))
+            exit()
         year = cfoods[-1].xdate.year
         month = cfoods[-1].xdate.month
         residual_mark = _("(Remaining)")
         time_nodes = sorted(
             list(
                 set(
                     [f.xdate for f in cfoods]
@@ -75,15 +78,17 @@
             tn1 = time_nodes[i + 1]
             tn0 = time_nodes[i]
             tn0_cp = tn0
             if not tn0.month == tn1.month:
                 tn0 = datetime(tn1.year, tn1.month, 1)
 
             wbfoods = [
-                f for f in cfoods if f.get_remainder(tn0) > 0 and f.xdate <= tn0
+                f
+                for f in cfoods
+                if f.get_remainder(tn0) > 0 and f.xdate <= tn0
             ]
             for wbfood in [f for f in wbfoods if f.xdate < tn0]:
                 if not wbfood.name.endswith(residual_mark):
                     wbfood.name = wbfood.name + residual_mark
 
             col_index = 0
             for d_index in range(0, (tn1 - tn0).days + 1):
@@ -122,15 +127,17 @@
                 _(
                     "Sheet '{0}' of \"{1}\" was updated.\n"
                     + "Press any key to continue when you have "
                     + "completed the foods allocation."
                 ).format(sheet.title, wb_fpath)
             )
             new_wbfoods = [
-                f for f in cfoods if f.get_remainder(tn1) > 0 and f.xdate == tn1
+                f
+                for f in cfoods
+                if f.get_remainder(tn1) > 0 and f.xdate == tn1
             ]
             if len(new_wbfoods) > 0:
                 print_info(
                     (
                         _("New purchased food for date {0} is:")
                         if len(new_wbfoods) > 1
                         else _("New purchased foods for date {0} are:")
@@ -156,23 +163,23 @@
             print_error(
                 _(
                     "There is no need to design for "
                     + "dates without food consumption. "
                     + "(Ok, I know [press any key to continue])"
                 )
             )
-            input()
+            input(">_ ")
             wb.close()
             open_file(wb_fpath)
             print_info(
                 _(
                     "Ok! I have updated spreadsheet '{0}'. (Press any key)"
                 ).format(wb_fpath)
             )
-            input()
+            input(">_ ")
             wb = load_workbook(wb_fpath)
             sheet = wb[self.sheet_name0]
 
             f_index = 0
             for row in sheet.iter_rows(
                 min_row=self.row_index_offset,
                 min_col=self.col_index_offset,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,28 +31,29 @@
             "购入单位名",
         ]
         self.purchaser_name_col_name = None
         self.count_cols = ["总数", "数量", "下单数量", "订货数量", "发货数量"]
         self.count_col_name = None
         self.abandoned_cols = [
             "不计",
+            "是不计",
             "未入库",
             "非入库",
             "不需入库",
             "是非入库",
         ]
         self.abandoned_col_name = None
         self.inventory_cols = [
             "盘存",
             "存余",
             "结余",
+            "是结余",
             "剩余",
             "是剩余",
             "是盘存",
-            "是结余",
         ]
         self.food_class_col_name = "食材大类"
         self.inventory_col_name = None
 
     @property
     def food_classes(self):
         food_classes = self.bill.food_classes
@@ -126,15 +127,34 @@
                     )
                 )
                 exit()
 
     @property
     def path(self):
         if not self._path:
-            print_info(_("Select a purchasing file, please!"))
+            print_info(
+                _(
+                    "{0} need a purchasing list file, "
+                    + "and it's file type should be '.xlsx'. "
+                    + "The column names of it:"
+                ).format(app_name)
+                + _(
+                    ""
+                    + "\n\tcolumn   type    example"
+                    + "\n\t送货日期 Text    2024-03-01"
+                    + "\n\t食材名称 Text    香菜"
+                    + "\n\t数量     Number  20"
+                    + "\n\t计量单位 Text    斤"
+                    + "\n\t总价     Number  20.0"
+                    + "\n\t购买者   Text    "
+                    + "\n\t是不计   Text    y"
+                    + "\n\t是结余   Text    y"
+                )
+            )
+            print_info(_("Please select a purchasing file."))
             filetypes = ((_("Spreadsheet Files"), "*.xlsx"),)
 
             filename = filedialog.askopenfilename(
                 title=_("Please select the purchasing file"),
                 initialdir=(Path.home() / "Downloads").as_posix(),
                 filetypes=filetypes,
             )
@@ -152,15 +172,16 @@
 
     def update_fclass(self):
         wb = load_workbook(self.path)
         sheet = wb.active
         headers = [
             h
             for h in [
-                sheet.cell(1, ci).value for ci in range(1, sheet.max_column + 1)
+                sheet.cell(1, ci).value
+                for ci in range(1, sheet.max_column + 1)
             ]
             if h
         ]
         if self.food_class_col_name in headers:
             wb.close
             return
 
@@ -199,24 +220,25 @@
             )
             food_class_list_dv.add(sheet.cell(row_index, food_class_col_index))
             food_len += 1
         wb.save(self.path)
         wb.close()
         print_info(
             _(
-                "Food class column has been updated, "
+                'Column "{0}" has been updated, '
                 + "please verify/modify it. "
                 + "Feel free to open new issue if some "
-                + "food with the wrong class ({new_issue_url})."
-                + "(Ok, I checked it. "
-                + "[press any key to continue])"
-            ).format(new_issue_url=get_new_issue_url())
+                + "food with the wrong class ({1}). "
+                + "(Press any key to check it)"
+            ).format(self.food_class_col_name, get_new_issue_url())
         )
+        input(">_ ")
         open_file(self.path)
-        input()
+        print_info(_("Ok, I checked it, it's ok. (Press any key to continue)"))
+        input(">_ ")
         pass
 
     def read_pfoods(self):
         self.update_fclass()
         foods = pd.read_excel(self.path)
         self.set_col_names(foods.columns)
         _foods = []
@@ -228,17 +250,17 @@
                 count=food[self.count_col_name],
                 total_price=food[self.total_price_col_name],
                 xdate=food[self.xdate_col_name],
                 purchaser=food[self.purchaser_name_col_name],
                 fclass=food[self.food_class_col_name],
             )
             if self.abandoned_col_name:
-                _food.is_abandoned = not food[self.abandoned_col_name] is np.nan
+                _food.is_abandoned = not pd.isna(food[self.abandoned_col_name])
             if self.inventory_col_name:
-                _food.is_inventory = not food[self.inventory_col_name] is np.nan
+                _food.is_inventory = not pd.isna(food[self.inventory_col_name])
             _foods.append(_food)
 
         foods = _foods
         foods = sorted(foods, key=lambda f: f.xdate)
         self.spreadsheet.preconsuming.pre_consume_foods(foods)
         return foods
         pass
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from fnschool import *
 from fnschool.canteen.spreadsheet.base import *
 
 
 class PurchasingSum(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
-        self.sheet_name = "入库、未入库汇总表"
+        self.sheet_name = self.s.purchasingsum_name
         pass
 
     def update(self):
 
         pssheet = self.sheet
         year = self.bfoods[-1].xdate.year
         month = self.bfoods[-1].xdate.month
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from fnschool import *
 from fnschool.canteen.spreadsheet.base import *
 
 
 class Unwarehousing(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
-        self.sheet_name = "未入库明细表"
+        self.sheet_name = self.s.unwarehousing_name
+        self.entry_row_len0 = 11
         pass
 
     @property
     def form_indexes(self):
         if not self._form_indexes:
             unwsheet = self.sheet
             indexes = []
@@ -43,14 +44,23 @@
         return self._form_indexes
 
     def update(self):
         unwsheet = self.sheet
         form_indexes = self.form_indexes
 
         foods = [f for f in self.bfoods if f.is_abandoned]
+        if len(foods) < 1:
+            print_info(
+                _(
+                    "There is no abandoned food. "
+                    + "Sheet {0} updating skipped."
+                ).format(self.sheet.title)
+            )
+            return None
+
         foods = sorted(foods, key=lambda f: f.xdate)
 
         t1 = []
 
         for bf in self.bfoods:
             for d, __ in bf.consumptions:
                 t1.append(d)
@@ -84,16 +94,26 @@
             total_price += food.total_price
             unwsheet.cell(row_index, 1, food.xdate.strftime("%Y.%m.%d"))
             unwsheet.cell(row_index, 2, food.name)
             unwsheet.cell(row_index, 3, food.unit_name)
             unwsheet.cell(row_index, 4, food.count)
             unwsheet.cell(row_index, 5, food.unit_price)
             unwsheet.cell(row_index, 6, food.total_price)
-            unwsheet.cell(row_index, 5).number_format = numbers.FORMAT_NUMBER_00
-            unwsheet.cell(row_index, 6).number_format = numbers.FORMAT_NUMBER_00
+            unwsheet.cell(row_index, 5).number_format = (
+                numbers.FORMAT_NUMBER_00
+            )
+            unwsheet.cell(row_index, 6).number_format = (
+                numbers.FORMAT_NUMBER_00
+            )
+
+            for u_col_index in range(1, 7):
+                cell = unwsheet.cell(row_index, u_col_index)
+                cell.alignment = self.cell_alignment0
+                cell.border = self.cell_border0
+
             if (
                 str(unwsheet.cell(row_index + 1, 2).value)
                 .replace(" ", "")
                 .endswith("合计")
                 and len(foods) - 1 > _index
             ):
                 unwsheet.cell(row_index + 1, 2, "合计")
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 from fnschool import *
 
 from fnschool.canteen.spreadsheet.base import *
 
 
 class Warehousing(SpreadsheetBase):
-    def __init__(self, bill):
+    def __init__(self, bill, form_row_len=21):
         super().__init__(bill)
-        self.sheet_name = "入库单"
+        self.sheet_name = self.s.warehousing_name
+        self.entry_row_len0 = 21
         pass
 
     def format(self):
         wsheet = self.sheet
         self.unmerge_sheet_cells()
 
         for row in wsheet.iter_rows(
@@ -262,14 +263,15 @@
                     max_row=food_index1,
                     min_col=2,
                     max_col=7,
                 ):
                     for cell in row:
                         cell.value = ""
 
+        self.del_form_empty_row(2)
         self.format()
 
         wb = self.bwb
         wb.active = wsheet
 
         print_info(_("Sheet '%s' was updated.") % (self.sheet.title))
```

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/test.py` & `fnschool-20240515.322.21/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/canteen/workbook.py` & `fnschool-20240515.322.21/src/fnschool/canteen/workbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,17 @@
         self._unit_df = None
         self._negligible_class_list = None
         self._base_class_df = None
         self.purchase_workbook_fdpath = None
         self.pre_consuming_sheet_col_index_offset = 5
         self.pre_consuming_sheet_row_index_offset = 3
         self.spreadsheet_ext_names = ["xlsx"]
-        self.cell_alignment0 = Alignment(horizontal="center", vertical="center")
+        self.cell_alignment0 = Alignment(
+            horizontal="center", vertical="center"
+        )
         self.cell_side0 = Side(border_style="thin")
         self.cell_border0 = Border(
             top=self.cell_side0,
             left=self.cell_side0,
             right=self.cell_side0,
             bottom=self.cell_side0,
         )
@@ -481,15 +483,19 @@
                     _total_price += f.count * f.unit_price
             cvsheet.cell(row[0].row, 2, _total_price)
 
             total_price += _total_price
         cvsheet.cell(10, 2, total_price)
 
         w_seasoning_total_price = sum(
-            [f.count * f.unit_price for f in wfoods if ("调味" in f.class_name)]
+            [
+                f.count * f.unit_price
+                for f in wfoods
+                if ("调味" in f.class_name)
+            ]
         )
         unw_seasoning_total_price = sum(
             [
                 f.count * f.unit_price
                 for f in uwfoods
                 if ("调味" in f.class_name)
             ]
@@ -1028,15 +1034,18 @@
                 if ptimes:
                     print_info(
                         _(
                             "The food purchasing times of preadsheet {0} is {1} ."
                         ).format(
                             _file,
                             " | ".join(
-                                [ptime.strftime("%Y.%m.%d") for ptime in ptimes]
+                                [
+                                    ptime.strftime("%Y.%m.%d")
+                                    for ptime in ptimes
+                                ]
                             ),
                         )
                     )
                     properties.append([_file, sheet_name, chwb_fpath, ptimes])
 
         return properties if properties else None
 
@@ -1132,15 +1141,17 @@
             t0, t1 = time_node
             wb = load_workbook(fpath)
             sheet = wb[self.pre_consuming_sheet0_name]
             ckt0, ckt1 = self.bill.get_check_times(time_node)
             _foods = [
                 f
                 for f in foods
-                if (f.xdate <= ckt1 and f.remainder > 0 and not f.is_negligible)
+                if (
+                    f.xdate <= ckt1 and f.remainder > 0 and not f.is_negligible
+                )
             ]
             if len(_foods) < 1:
                 print_warning(
                     _(
                         "There is not food of time node %s ,skip workbook designing."
                     )
                     % (t0.strftime("%Y.%m.%d") + t1.strftime("%Y.%m.%d"))
@@ -1170,15 +1181,15 @@
                     _(
                         "Workbook '{0}' was updated, please design the "
                         + "daily foods consumption and press ANY key "
                         + "to continue."
                     ).format(fpath)
                 )
                 open_file(fpath)
-                input()
+                input(">_ ")
                 wb = load_workbook(fpath)
                 sheet = wb[self.pre_consuming_sheet0_name]
                 print_info(_("Workbook %s was read.") % fpath)
 
             for i, _f in enumerate(_foods):
                 row_index = row_index_offset + i
                 for col_index in range(col_index_offset, sheet.max_column + 1):
@@ -1200,15 +1211,15 @@
                     "Unable to find {0} from {1}, "
                     + "You can input it (1 base) directly or "
                     + "give feedback to the maintainers "
                     + "--> {2} ."
                 ).format(name, workbook_fpath, get_new_issue_url())
                 print_error(error_msg)
                 for __ in range(3):
-                    cn_index = input()
+                    cn_index = input(">_ ")
                     if cn_index.isnumeric():
                         cn_index = int(cn_index) - 1
                         indexes[i] = [name, cn_index]
                         break
                     else:
                         print("Unexpected value was got.")
         indexes = [i for __, i in indexes]
@@ -1276,15 +1287,15 @@
                     print_warning(
                         _(
                             "{app_name} desn't pick the index of organization name"
                             + " column, input it (0 base) or '{wb_fpath}' will be ignored."
                         ).format(app_name=app_name, wb_fpath=wb_fpath)
                     )
                     open_file(wb_fpath)
-                    _org_name_col_index = input()
+                    _org_name_col_index = input(">_ ")
                     if not _org_name_col_index.isnumeric():
                         continue
                     _org_name_col_index = int(_org_name_col_index)
 
                 _org_names = list(
                     set(
                         [
@@ -1300,15 +1311,17 @@
                 if not any(
                     [o == self.bill.profile.org_name for o in _org_names]
                 ):
                     print_warning(
                         (
                             _('Organization name read from {0} are "{1}",')
                             if len(_org_names) > 1
-                            else _('Organization name read from {0} is "{1}", ')
+                            else _(
+                                'Organization name read from {0} is "{1}", '
+                            )
                         ).format(wb_fpath, " | ".join(_org_names))
                         + _('but organization name of {0} is "{1}".').format(
                             f"{self.profile.label}({self.profile.name})",
                             self.profile.org_name,
                         )
                     )
                     print_error(
@@ -1336,15 +1349,15 @@
                         _(
                             "The column names of 'negligible' mark are following:"
                         )
                         + "\n\t"
                         + " | ".join(self.negligible_col_names)
                     )
                     open_file(wb_fpath)
-                    input()
+                    input(">_ ")
                     wb = load_workbook(wb_fpath, read_only=True)
                     sheet = wb[sheetnames[0]]
 
                 print_info(_("Spreadsheet '%s' was used."))
 
                 (
                     food_name_index,
@@ -1620,15 +1633,17 @@
         indexes_len = len(indexes)
         _index = None
         if indexes_len <= tn_index:
             return None
         _index = indexes[tn_index]
         return _index
 
-    def update_inventory_sheet_of_time_node(self, fd_path=None, time_node=None):
+    def update_inventory_sheet_of_time_node(
+        self, fd_path=None, time_node=None
+    ):
         fd_path = self.purchase_workbook_fd_path or fd_path
         time_node = time_node or self.bill.time_node
         t0, t1 = time_node
         isheet = self.get_inventory_sheet()
         foods = self.food.time_node_residue_foods
         (
             iform_index0,
@@ -1758,15 +1773,17 @@
                             _count * food.unit_price
                             for _date, _count in food.consuming_list
                             if _date.month == self.bill.month
                         ]
                     )
             total_price += _total_price
             cssheet.cell(row[0].row, 2, _total_price)
-            cssheet.cell(row[0].row, 2).number_format = numbers.FORMAT_NUMBER_00
+            cssheet.cell(row[0].row, 2).number_format = (
+                numbers.FORMAT_NUMBER_00
+            )
 
         total_price_cn = self.bill.convert_num_to_cnmoney_chars(total_price)
         cssheet.cell(
             2,
             1,
             f"编制单位：{self.bill.profile.org_name}       "
             + f"单位：元         "
@@ -1778,15 +1795,17 @@
             (f"总金额（大写)：{total_price_cn}    " + f"¥{total_price:.2f}"),
         )
         cssheet.cell(12, 1, f"经办人：{self.bill.profile.name}  ")
 
         wb = self.get_bill_workbook()
         wb.active = cssheet
 
-        print_info(_("Sheet '%s' was updated.") % self.consuming_sum_sheet_name)
+        print_info(
+            _("Sheet '%s' was updated.") % self.consuming_sum_sheet_name
+        )
 
     def update_consuming_sheet(self):
         foods = self.food.get_foods()
         csheet = self.get_consuming_sheet()
         form_indexes = self.get_consuming_form_indexes()
 
         time_nodes = self.bill.get_time_nodes()
@@ -2014,15 +2033,15 @@
         )
         print_info(
             _("Ok! I have updated spreadsheet '{0}'. (Press any key)").format(
                 wb_fpath
             )
         )
         open_file(wb_fpath)
-        input()
+        input(">_ ")
 
     def set_warehousing_form_index_offset(self, offset=0):
         self.warehousing_form_index_offset = offset
 
     def set_inventory_form_index_offset(self, offset=0):
         self.inventory_form_index_offset = offset
 
@@ -2063,15 +2082,17 @@
         return none
 
     def get_unwarehousing_form_indexes(self):
         unwsheet = self.get_unwarehousing_sheet()
         indexes = []
         row_index = 1
         for row in unwsheet.iter_rows(max_row=unwsheet.max_row + 1, max_col=7):
-            if row[0].value and "未入库明细表" in row[0].value.replace(" ", ""):
+            if row[0].value and "未入库明细表" in row[0].value.replace(
+                " ", ""
+            ):
                 indexes.append([row_index + 1, 0])
 
             if row[1].value and "合计" in row[1].value.replace(" ", ""):
                 indexes[-1][1] = row_index
 
             row_index += 1
 
@@ -2246,15 +2267,17 @@
                     start_column=1,
                     end_column=8,
                 )
 
         wb = self.get_bill_workbook()
         wb.active = wsheet
 
-        print_info(_("Sheet '%s' was formatted.") % self.warehousing_sheet_name)
+        print_info(
+            _("Sheet '%s' was formatted.") % self.warehousing_sheet_name
+        )
 
     def update_unwarehousing_sheet(self):
         unwsheet = self.get_unwarehousing_sheet()
         form_indexes = self.get_unwarehousing_form_indexes()
         time_nodes = [
             tn
             for tn in self.bill.get_time_nodes()
@@ -2298,16 +2321,20 @@
             total_price += food.total_price
             unwsheet.cell(row_index, 1, food.xdate.strftime("%Y.%m.%d"))
             unwsheet.cell(row_index, 2, food.name)
             unwsheet.cell(row_index, 3, food.unit_name)
             unwsheet.cell(row_index, 4, food.count)
             unwsheet.cell(row_index, 5, food.unit_price)
             unwsheet.cell(row_index, 6, food.total_price)
-            unwsheet.cell(row_index, 5).number_format = numbers.FORMAT_NUMBER_00
-            unwsheet.cell(row_index, 6).number_format = numbers.FORMAT_NUMBER_00
+            unwsheet.cell(row_index, 5).number_format = (
+                numbers.FORMAT_NUMBER_00
+            )
+            unwsheet.cell(row_index, 6).number_format = (
+                numbers.FORMAT_NUMBER_00
+            )
             if (
                 str(unwsheet.cell(row_index + 1, 2).value)
                 .replace(" ", "")
                 .endswith("合计")
                 and len(foods) - 1 > _index
             ):
                 unwsheet.cell(row_index + 1, 2, "合计")
@@ -2325,15 +2352,17 @@
                         " ", ""
                     ).endswith("合计"):
                         row[2].value = "总合计" if use_forms else "合计"
                         row[6].value = total_price
                         break
                 break
 
-        print_info(_("Sheet '%s' was updated.") % self.unwarehousing_sheet_name)
+        print_info(
+            _("Sheet '%s' was updated.") % self.unwarehousing_sheet_name
+        )
 
     def update_warehousing_sheet(self):
         wsheet = self.get_warehousing_sheet()
         foods = [
             f
             for f in self.food.get_foods()
             if (
@@ -2381,15 +2410,17 @@
             food_index1 = form_index1 - 1
             entry_index = food_index0
             warehousing_n = windex + 1
 
             wfoods = [f for f in foods if (f.xdate == time_point)]
             foods_class_names = [f.class_name for f in wfoods]
             class_names_without_food = [
-                _name for _name in class_names if not _name in foods_class_names
+                _name
+                for _name in class_names
+                if not _name in foods_class_names
             ]
             row_difference = (
                 len(wfoods)
                 + len(class_names_without_food)
                 - (food_index1 - food_index0 + 1)
             )
 
@@ -2507,15 +2538,17 @@
                     for cell in row:
                         cell.value = ""
 
         self.format_warehousing_sheet()
         wb = self.get_bill_workbook()
         wb.active = wsheet
 
-        print_info(_("Sheet '%s' was updated.") % (self.warehousing_sheet_name))
+        print_info(
+            _("Sheet '%s' was updated.") % (self.warehousing_sheet_name)
+        )
 
     def get_unit_df(self):
         if not self._unit_df is None:
             return self._unit_df
         self._unit_df = pd.read_excel(
             self.get_main_spreadsheet_path(),
             sheet_name=self.unit_sheet_name,
```

### Comparing `fnschool-20240513.614.21/src/fnschool/entry.py` & `fnschool-20240515.322.21/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/external.py` & `fnschool-20240515.322.21/src/fnschool/external.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 
 
 def get_sponsor_url():
     return (
         (
             "https://gitee.com/larryw3i/funingschool"
             + "/blob/master/Documentation/"
-            + "README.zh_CN.md#赞助"
+            + "README.zh_CN.md#%E8%B5%9E%E5%8A%A9"
         )
         if is_zh_CN
-        else ""
+        else ("https://github.com/larryw3i/" + "funingschool#support")
     )
 
 
 def open_file(file_path):
     file_path = str(file_path)
     bin_name = "open" if (sys_is_linux() or sys_is_darwin()) else "start"
     file_path = '"' + file_path + '"'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fnschool-20240513.614.21/src/fnschool/language.py` & `fnschool-20240515.322.21/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,45 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-13 04:18+0800\n"
-"PO-Revision-Date: 2024-05-13 04:18+0800\n"
+"POT-Creation-Date: 2024-05-15 03:02+0800\n"
+"PO-Revision-Date: 2024-05-15 03:02+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
-"Language: en_US\n"
-"Language-Team: English - United States <larryw3i@163.com>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: zh_CN\n"
+"Language-Team: Chinese - China <larryw3i@163.com>\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
+msgid ""
+"\n"
+"\tcolumn   type    example\n"
+"\t送货日期 Text    2024-03-01\n"
+"\t食材名称 Text    香菜\n"
+"\t数量     Number  20\n"
+"\t计量单位 Text    斤\n"
+"\t总价     Number  20.0\n"
+"\t购买者   Text    \n"
+"\t是不计   Text    y\n"
+"\t是结余   Text    y"
+msgstr ""
+"\n"
+"　　列名　　　类型　样例\n"
+"　　送货日期　文本　2024-03-01\n"
+"　　食材名称　文本　香菜\n"
+"　　数量　　　数字　20\n"
+"　　计量单位　文本　斤\n"
+"　　总价　　　数字　20.0\n"
+"　　购买者　　文本\n"
+"　　不计　　　文本　y\n"
+"　　结余　　　文本　y"
+
 msgid "%s can't change."
 msgstr "%s 无法转换。"
 
 msgid "'{wb_fpath}' was discarded."
 msgstr "“{wb_fpath}” 已被舍去。"
 
 msgid "(Remaining)"
@@ -27,14 +50,22 @@
 
 msgid "Canteen related functions."
 msgstr "Cateen 的相关函数。"
 
 msgid "Cells of {0} was unmerged."
 msgstr "工作表 “{0}” 的所有单元格被取消合并。"
 
+msgid ""
+"Column \"{0}\" has been updated, please verify/modify it. Feel free to open "
+"new issue if some food with the wrong class ({1}). (Press any key to check "
+"it)"
+msgstr ""
+"“{0}”列已添加，请检查/更改它。如果食材的大类名有错误，还请您随时提交反馈"
+"（{1}）。（按任意键打开文件检查）"
+
 msgid "Command line interface of fnschool."
 msgstr "“fnschool“ 的命令行接口。"
 
 msgid "Configuration file '%s' was copied to '%s'."
 msgstr "配置文件 “%s” 被复制到 “%s” 。"
 
 msgid "Consuming days:"
@@ -64,14 +95,17 @@
 msgstr ""
 "保存被更新的数据到 “{0}” 吗？或者仅保存为副本到 “{1}” 。 （YyNn：“Y” 或 “y” "
 "为 “是”，其它为“否”）"
 
 msgid "Email:"
 msgstr "电子邮箱："
 
+msgid "Empty row {0} of sheet \"{1}\" has been deleted."
+msgstr "{1} 表的 空行 （第{0}行）已被删除。"
+
 msgid "Enjoy it."
 msgstr "请慢用。"
 
 msgid "Enter the month (1~12) to generate spreadsheet: (default: {0})"
 msgstr "输入月份（1～12）以设计工作簿：（默认为 {0}）"
 
 msgid "Entered directory: %s"
@@ -91,22 +125,14 @@
 
 msgid "Food check date: %s"
 msgstr "食材清点日期：%s"
 
 msgid "Food checking time range of {0} is {1}."
 msgstr "在 {0} 时间段 食材的清点时间范围是 {1} 。"
 
-msgid ""
-"Food class column has been updated, please verify/modify it. Feel free to "
-"open new issue if some food with the wrong class ({new_issue_url}).(Ok, I "
-"checked it. [press any key to continue])"
-msgstr ""
-"“食材大类”列已更新，请检查/更改它。如果食材的大类名有错误，还请您随时提交反馈"
-"（{new_issue_url}）。（好的，我已经检查好了。【按任意键继续】）"
-
 msgid "Food classes files:"
 msgstr "食材大类文件："
 
 msgid "Food count index"
 msgstr "食材数量索引"
 
 msgid "Food count: %s"
@@ -144,14 +170,17 @@
 
 msgid "Got no purchased foods of time node %s ."
 msgstr "时间节点 %s 没有购入的食材。"
 
 msgid "Hello! helping information is here for you:"
 msgstr "您好！这里是给您的帮助信息："
 
+msgid "Hi, your name is \"{0}\"? (Yes: 'Y' 'y' '', or enter your name)"
+msgstr "您好！您是 “{0}” 吗？（是：“Y”、“y”、“”，或者输入您的姓名）"
+
 msgid ""
 "If new Xuelan milks is purchased. you have to add the purchasing information "
 "of them into the end of the purchasing spreadsheet (e.g: the spreadsheets "
 "Changsheng provided)."
 msgstr ""
 "如果有新购入的雪兰奶，您需要将购入信息添加在购入表单里面（比如添加在“昌盛”提"
 "供的表单）。"
@@ -205,26 +234,38 @@
 
 msgid "New purchased foods for date {0} are:"
 msgstr "{0} 新购入的食材："
 
 msgid "No file was selected, exit."
 msgstr "未选择文件，退出。"
 
+msgid "No food found, exit."
+msgstr "未读取到食材，退出。"
+
 msgid "No profile information was got."
 msgstr "没有获取到您的个人信息。"
 
 msgid "Ok! I have updated spreadsheet '{0}'. (Press any key)"
 msgstr "好的，我已经更新工作簿 “{0}” 了。（按任意键继续）"
 
 msgid "Ok! I knew that.(press any key to continue)"
 msgstr "好的，我知道了。（按任意键继续）"
 
+msgid "Ok! I know it. (Press any key to continue)"
+msgstr "好的，我知道了。（按任意键继续）"
+
 msgid "Ok! it was configured. (enter any key)"
 msgstr "好的，我已配置。（按任意键继续）"
 
+msgid "Ok, I checked it, it's ok. (Press any key to continue)"
+msgstr "好了，我已经检查每个食材的大类了，它们都是对的。（按任意键继续）"
+
+msgid "Ok, your name has been saved to \"{0}\"."
+msgstr "好了，您的名字被保存到 “{0}”。"
+
 msgid "Operator email"
 msgstr "操作员电子邮箱"
 
 msgid "Operator name"
 msgstr "操作员姓名"
 
 msgid "Organization Name:"
@@ -257,14 +298,17 @@
 msgstr ""
 "请输入 昌盛 提供的购入单文件的路径，或者输入一个目录，{app_name} 会读取所有的"
 "工作簿并获取购入数据。（默认的目录：{seeking_dpath0}）"
 
 msgid "Please input the year for design consuming"
 msgstr "请输入年份以设计出库"
 
+msgid "Please select a purchasing file."
+msgstr "请选择购入食材的列表文件。"
+
 msgid "Please select the purchasing file"
 msgstr "请选择购入食材的列表文件"
 
 msgid "Please update your profile file."
 msgstr "请更新您的个人信息文件。"
 
 msgid "Preset food classes were read from \"{0}\"."
@@ -295,17 +339,14 @@
 
 msgid "Saving workbook. . ."
 msgstr "正在保存......"
 
 msgid "Saving. . ."
 msgstr "正在保存......"
 
-msgid "Select a purchasing file, please!"
-msgstr "请您选择一个购入食材的列表文件。"
-
 msgid "Sheet \"{0}\" has been reformatted."
 msgstr "“{0}” 表已被重新格式化。"
 
 msgid "Sheet '%s' was formatted."
 msgstr "“%s” 表已被格式化。"
 
 msgid "Sheet '%s' was updated."
@@ -378,14 +419,17 @@
 
 msgid "The functions of canteen."
 msgstr "“canteen“ 的函数。"
 
 msgid "The modules to run."
 msgstr "要运行的模块。"
 
+msgid "There is no abandoned food. Sheet {0} updating skipped."
+msgstr "没有不计（无需入库）的食材，{0} 表的更新被跳过。"
+
 msgid ""
 "There is no need to design for dates without food consumption. (Ok, I know "
 "[press any key to continue])"
 msgstr "没有食材消耗的日期不需要设计出库。（好的，知道了的【按任意键继续】）"
 
 msgid "There is no purchased food for {0}."
 msgstr "{0} 没有新购入的食材。"
@@ -482,29 +526,45 @@
 
 msgid "Your food classes were read from \"{0}\". It will be used first."
 msgstr "您的食材大类已从 “{0}”  读取。它会被优先匹配。"
 
 msgid "Your name has been saved to \"{0}\"."
 msgstr "您的名字被保存到 “{0}”。"
 
+msgid "bill"
+msgstr "账单"
+
 msgid "but organization name of {0} is \"{1}\"."
 msgstr "但是 “{0}” 的 机构名（学校名）是 “{1}”。"
 
+msgid "config"
+msgstr "配置"
+
 msgid "fnschool"
 msgstr "fnschool"
 
 msgid "food_consuming"
 msgstr "食材出库"
 
 msgid "line '%s' has been discarded."
 msgstr "行 “%s” 被舍去。"
 
+msgid "preconsuming"
+msgstr "预出库"
+
 msgid "values length is less than %s."
 msgstr "值的长度小于 %s 。"
 
+msgid ""
+"{0} need a purchasing list file, and it's file type should be '.xlsx'. The "
+"column names of it:"
+msgstr ""
+"{0} 需要一个购入食材的列表文件，这个列表文件的类型应为 “.xlsx”。它的列（表"
+"头）为："
+
 msgid "{0}.{1}.{2}--{3}.{4}.{5}"
 msgstr "{0}年{1}月{2}日——{3}年{4}月{5}日"
 
 msgid ""
 "{app_name} desn't pick the index of organization name column, input it (0 "
 "base) or '{wb_fpath}' will be ignored."
 msgstr ""
```

### Comparing `fnschool-20240513.614.21/src/fnschool/log.py` & `fnschool-20240515.322.21/src/fnschool/log.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/path.py` & `fnschool-20240515.322.21/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool/test.py` & `fnschool-20240515.322.21/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.614.21/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240515.322.21/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240513.614.21
+Version: 20240515.322.21
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240513.614.21/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240515.322.21/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

