# Comparing `tmp/general_operator-0.1.tar.gz` & `tmp/general_operator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_operator-0.1.tar", last modified: Mon May 13 06:13:04 2024, max compression
+gzip compressed data, was "general_operator-0.1.1.tar", last modified: Wed May 15 07:43:25 2024, max compression
```

## Comparing `general_operator-0.1.tar` & `general_operator-0.1.1.tar`

### file list

```diff
@@ -1,125 +1,40 @@
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.078832 general_operator-0.1/
--rw-r--r--   0 wilson08   (501) staff       (20)     3539 2024-05-13 06:13:04.078611 general_operator-0.1/PKG-INFO
--rwxr-xr-x   0 wilson08   (501) staff       (20)     2551 2024-05-13 03:26:40.000000 general_operator-0.1/README.md
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.065941 general_operator-0.1/app/
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.066148 general_operator-0.1/app/SQL/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:37:48.000000 general_operator-0.1/app/SQL/__init__.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)    13954 2024-05-13 03:44:24.000000 general_operator-0.1/app/SQL/models.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2023-12-22 08:24:06.000000 general_operator-0.1/app/__init__.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.069154 general_operator-0.1/data/
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.069885 general_operator-0.1/data/API/
--rw-r--r--   0 wilson08   (501) staff       (20)      502 2024-05-11 09:53:05.000000 general_operator-0.1/data/API/API_control_href_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      345 2024-05-11 09:53:05.000000 general_operator-0.1/data/API/API_node.py
--rw-r--r--   0 wilson08   (501) staff       (20)      434 2024-05-13 03:26:40.000000 general_operator-0.1/data/API/API_node_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      533 2024-05-13 03:26:40.000000 general_operator-0.1/data/API/API_object.py
--rw-r--r--   0 wilson08   (501) staff       (20)      464 2024-05-13 03:26:40.000000 general_operator-0.1/data/API/API_object_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1/data/API/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1/data/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)      633 2024-05-13 03:44:24.000000 general_operator-0.1/data/control_href_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      768 2024-05-11 09:53:05.000000 general_operator-0.1/data/control_href_group_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)      672 2024-05-11 09:53:05.000000 general_operator-0.1/data/control_href_item.py
--rw-r--r--   0 wilson08   (501) staff       (20)      793 2024-05-11 09:53:05.000000 general_operator-0.1/data/control_href_item_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)      584 2024-05-11 09:53:05.000000 general_operator-0.1/data/device_info.py
--rw-r--r--   0 wilson08   (501) staff       (20)      625 2024-05-11 09:53:05.000000 general_operator-0.1/data/fake_data_config.py
--rw-r--r--   0 wilson08   (501) staff       (20)      841 2024-05-11 09:53:05.000000 general_operator-0.1/data/fake_data_config_base.py
--rw-r--r--   0 wilson08   (501) staff       (20)      746 2024-05-11 09:53:05.000000 general_operator-0.1/data/fake_data_config_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)      517 2024-05-13 03:26:40.000000 general_operator-0.1/data/node.py
--rw-r--r--   0 wilson08   (501) staff       (20)      648 2024-05-11 09:53:05.000000 general_operator-0.1/data/node_base.py
--rw-r--r--   0 wilson08   (501) staff       (20)      388 2024-05-13 03:26:40.000000 general_operator-0.1/data/node_copy.py
--rw-r--r--   0 wilson08   (501) staff       (20)      469 2024-05-11 09:53:05.000000 general_operator-0.1/data/node_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      776 2024-05-11 09:53:05.000000 general_operator-0.1/data/node_node_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      594 2024-05-11 09:53:05.000000 general_operator-0.1/data/node_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)      439 2024-05-11 09:53:05.000000 general_operator-0.1/data/node_template_copy.py
--rw-r--r--   0 wilson08   (501) staff       (20)      564 2024-05-13 03:26:40.000000 general_operator-0.1/data/object.py
--rw-r--r--   0 wilson08   (501) staff       (20)      681 2024-05-11 09:53:05.000000 general_operator-0.1/data/object_base.py
--rw-r--r--   0 wilson08   (501) staff       (20)      501 2024-05-11 09:53:05.000000 general_operator-0.1/data/object_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      841 2024-05-11 09:53:05.000000 general_operator-0.1/data/object_object_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      640 2024-05-11 09:53:05.000000 general_operator-0.1/data/object_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)      707 2024-05-11 09:53:05.000000 general_operator-0.1/data/third_dimension_instance.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.070081 general_operator-0.1/dependencies/
--rwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1/dependencies/__init__.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)      167 2024-05-11 09:53:05.000000 general_operator-0.1/dependencies/db_dependencies.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.070295 general_operator-0.1/function/
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.071071 general_operator-0.1/function/API/
--rw-r--r--   0 wilson08   (501) staff       (20)      781 2024-05-13 03:54:19.000000 general_operator-0.1/function/API/API_control_href_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)    14348 2024-05-13 03:40:09.000000 general_operator-0.1/function/API/API_node.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1563 2024-05-13 03:54:53.000000 general_operator-0.1/function/API/API_node_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)    12249 2024-05-13 03:44:24.000000 general_operator-0.1/function/API/API_object.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1164 2024-05-13 03:55:12.000000 general_operator-0.1/function/API/API_object_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1/function/API/__init__.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1/function/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)     2446 2024-05-13 03:26:40.000000 general_operator-0.1/function/config_manager.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.071159 general_operator-0.1/general_operator/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:34:24.000000 general_operator-0.1/general_operator/__init__.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.071762 general_operator-0.1/general_operator/app/
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.072096 general_operator-0.1/general_operator/app/SQL/
--rwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1/general_operator/app/SQL/__init__.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)      884 2024-05-13 03:26:40.000000 general_operator-0.1/general_operator/app/SQL/database.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)     4410 2024-05-13 03:26:40.000000 general_operator-0.1/general_operator/app/SQL/sql_operate.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:37:18.000000 general_operator-0.1/general_operator/app/__init__.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.072456 general_operator-0.1/general_operator/app/influxdb/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1/general_operator/app/influxdb/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)      664 2024-05-13 03:26:40.000000 general_operator-0.1/general_operator/app/influxdb/influxdb.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1382 2024-05-13 03:26:40.000000 general_operator-0.1/general_operator/app/influxdb/influxdb_operate.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.072810 general_operator-0.1/general_operator/app/redis_db/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1/general_operator/app/redis_db/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1088 2024-05-13 03:26:40.000000 general_operator-0.1/general_operator/app/redis_db/redis.py
--rw-r--r--   0 wilson08   (501) staff       (20)     6306 2024-05-13 03:26:40.000000 general_operator-0.1/general_operator/app/redis_db/redis_operate.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.073150 general_operator-0.1/general_operator/dependencies/
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:43:10.000000 general_operator-0.1/general_operator/dependencies/__init__.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)      167 2024-05-11 09:53:05.000000 general_operator-0.1/general_operator/dependencies/db_dependencies.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)     1178 2024-05-13 06:05:37.000000 general_operator-0.1/general_operator/dependencies/get_query_dependencies.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.073785 general_operator-0.1/general_operator/function/
--rw-r--r--   0 wilson08   (501) staff       (20)    11029 2024-05-13 03:50:09.000000 general_operator-0.1/general_operator/function/General_operate.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:38:18.000000 general_operator-0.1/general_operator/function/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1147 2024-05-13 03:26:40.000000 general_operator-0.1/general_operator/function/create_data_structure.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)      157 2024-05-13 03:26:40.000000 general_operator-0.1/general_operator/function/exception.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1878 2024-05-11 09:53:05.000000 general_operator-0.1/general_operator/function/search_function.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.074034 general_operator-0.1/general_operator/routers/
--rw-r--r--   0 wilson08   (501) staff       (20)     4726 2024-05-13 06:04:34.000000 general_operator-0.1/general_operator/routers/General_table_router.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:45:41.000000 general_operator-0.1/general_operator/routers/__init__.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.078310 general_operator-0.1/general_operator.egg-info/
--rw-r--r--   0 wilson08   (501) staff       (20)     3539 2024-05-13 06:13:04.000000 general_operator-0.1/general_operator.egg-info/PKG-INFO
--rw-r--r--   0 wilson08   (501) staff       (20)     6018 2024-05-13 06:13:04.000000 general_operator-0.1/general_operator.egg-info/SOURCES.txt
--rw-r--r--   0 wilson08   (501) staff       (20)        1 2024-05-13 06:13:04.000000 general_operator-0.1/general_operator.egg-info/dependency_links.txt
--rw-r--r--   0 wilson08   (501) staff       (20)      106 2024-05-13 06:13:04.000000 general_operator-0.1/general_operator.egg-info/requires.txt
--rw-r--r--   0 wilson08   (501) staff       (20)       17 2024-05-13 06:13:04.000000 general_operator-0.1/general_operator.egg-info/top_level.txt
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.074128 general_operator-0.1/routers/
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.074998 general_operator-0.1/routers/API/
--rw-r--r--   0 wilson08   (501) staff       (20)    11976 2024-05-13 03:52:32.000000 general_operator-0.1/routers/API/API_control_href_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)    13210 2024-05-13 03:53:10.000000 general_operator-0.1/routers/API/API_node.py
--rw-r--r--   0 wilson08   (501) staff       (20)    19093 2024-05-13 03:53:17.000000 general_operator-0.1/routers/API/API_node_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)    15517 2024-05-13 03:53:21.000000 general_operator-0.1/routers/API/API_object.py
--rw-r--r--   0 wilson08   (501) staff       (20)    17687 2024-05-13 03:53:30.000000 general_operator-0.1/routers/API/API_object_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-03-19 09:44:47.000000 general_operator-0.1/routers/API/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-03-19 09:44:47.000000 general_operator-0.1/routers/__init__.py
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.077397 general_operator-0.1/schemas/
-drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-13 06:13:04.078149 general_operator-0.1/schemas/API/
--rwxr-xr-x   0 wilson08   (501) staff       (20)     1350 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/API/API_control_href_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1892 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/API/API_node.py
--rw-r--r--   0 wilson08   (501) staff       (20)      396 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/API/API_node_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1620 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/API/API_object.py
--rw-r--r--   0 wilson08   (501) staff       (20)      413 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/API/API_object_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-03-19 09:44:47.000000 general_operator-0.1/schemas/API/__init__.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-03-19 09:44:47.000000 general_operator-0.1/schemas/__init__.py
--rw-r--r--   0 wilson08   (501) staff       (20)      704 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/control_href_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      727 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/control_href_group_template.py
--rwxr-xr-x   0 wilson08   (501) staff       (20)      713 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/control_href_item.py
--rw-r--r--   0 wilson08   (501) staff       (20)      670 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/control_href_item_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)      844 2024-03-19 09:44:47.000000 general_operator-0.1/schemas/device_info.py
--rw-r--r--   0 wilson08   (501) staff       (20)      831 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/fake_data_config.py
--rw-r--r--   0 wilson08   (501) staff       (20)      815 2024-03-19 09:44:47.000000 general_operator-0.1/schemas/fake_data_config_base.py
--rw-r--r--   0 wilson08   (501) staff       (20)      731 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/fake_data_config_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1271 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/node.py
--rw-r--r--   0 wilson08   (501) staff       (20)      628 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/node_base.py
--rw-r--r--   0 wilson08   (501) staff       (20)      681 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/node_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      453 2024-03-19 09:44:47.000000 general_operator-0.1/schemas/node_node_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      761 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/node_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)     1226 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/object.py
--rw-r--r--   0 wilson08   (501) staff       (20)      737 2024-03-19 09:44:47.000000 general_operator-0.1/schemas/object_base.py
--rw-r--r--   0 wilson08   (501) staff       (20)      679 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/object_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      497 2024-03-19 09:44:47.000000 general_operator-0.1/schemas/object_object_group.py
--rw-r--r--   0 wilson08   (501) staff       (20)      911 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/object_template.py
--rw-r--r--   0 wilson08   (501) staff       (20)      919 2024-05-13 03:26:40.000000 general_operator-0.1/schemas/third_dimension_instance.py
--rw-r--r--   0 wilson08   (501) staff       (20)       38 2024-05-13 06:13:04.078867 general_operator-0.1/setup.cfg
--rw-r--r--   0 wilson08   (501) staff       (20)     1395 2024-05-13 06:13:02.000000 general_operator-0.1/setup.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.637176 general_operator-0.1.1/
+-rw-r--r--   0 wilson08   (501) staff       (20)     3510 2024-05-15 07:43:25.636994 general_operator-0.1.1/PKG-INFO
+-rwxr-xr-x   0 wilson08   (501) staff       (20)     2551 2024-05-13 03:26:40.000000 general_operator-0.1.1/README.md
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.633534 general_operator-0.1.1/general_operator/
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:34:24.000000 general_operator-0.1.1/general_operator/__init__.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.634153 general_operator-0.1.1/general_operator/app/
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.634887 general_operator-0.1.1/general_operator/app/SQL/
+-rwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.1/general_operator/app/SQL/__init__.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)      884 2024-05-13 03:26:40.000000 general_operator-0.1.1/general_operator/app/SQL/database.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)     4410 2024-05-13 03:26:40.000000 general_operator-0.1.1/general_operator/app/SQL/sql_operate.py
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:37:18.000000 general_operator-0.1.1/general_operator/app/__init__.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.635179 general_operator-0.1.1/general_operator/app/influxdb/
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.1/general_operator/app/influxdb/__init__.py
+-rw-r--r--   0 wilson08   (501) staff       (20)      664 2024-05-13 03:26:40.000000 general_operator-0.1.1/general_operator/app/influxdb/influxdb.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     1382 2024-05-13 03:26:40.000000 general_operator-0.1.1/general_operator/app/influxdb/influxdb_operate.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.635471 general_operator-0.1.1/general_operator/app/redis_db/
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-11 09:53:05.000000 general_operator-0.1.1/general_operator/app/redis_db/__init__.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     1088 2024-05-13 03:26:40.000000 general_operator-0.1.1/general_operator/app/redis_db/redis.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     6306 2024-05-13 03:26:40.000000 general_operator-0.1.1/general_operator/app/redis_db/redis_operate.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.635939 general_operator-0.1.1/general_operator/dependencies/
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:43:10.000000 general_operator-0.1.1/general_operator/dependencies/__init__.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)      167 2024-05-11 09:53:05.000000 general_operator-0.1.1/general_operator/dependencies/db_dependencies.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)     1178 2024-05-13 06:05:37.000000 general_operator-0.1.1/general_operator/dependencies/get_query_dependencies.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.636458 general_operator-0.1.1/general_operator/function/
+-rw-r--r--   0 wilson08   (501) staff       (20)    11029 2024-05-13 03:50:09.000000 general_operator-0.1.1/general_operator/function/General_operate.py
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:38:18.000000 general_operator-0.1.1/general_operator/function/__init__.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     1147 2024-05-13 03:26:40.000000 general_operator-0.1.1/general_operator/function/create_data_structure.py
+-rwxr-xr-x   0 wilson08   (501) staff       (20)      157 2024-05-13 03:26:40.000000 general_operator-0.1.1/general_operator/function/exception.py
+-rw-r--r--   0 wilson08   (501) staff       (20)     1878 2024-05-11 09:53:05.000000 general_operator-0.1.1/general_operator/function/search_function.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.636672 general_operator-0.1.1/general_operator/routers/
+-rw-r--r--   0 wilson08   (501) staff       (20)     4726 2024-05-13 06:04:34.000000 general_operator-0.1.1/general_operator/routers/General_table_router.py
+-rw-r--r--   0 wilson08   (501) staff       (20)        0 2024-05-13 03:45:41.000000 general_operator-0.1.1/general_operator/routers/__init__.py
+drwxr-xr-x   0 wilson08   (501) staff       (20)        0 2024-05-15 07:43:25.636798 general_operator-0.1.1/general_operator.egg-info/
+-rw-r--r--   0 wilson08   (501) staff       (20)     3510 2024-05-15 07:43:25.000000 general_operator-0.1.1/general_operator.egg-info/PKG-INFO
+-rw-r--r--   0 wilson08   (501) staff       (20)     1106 2024-05-15 07:43:25.000000 general_operator-0.1.1/general_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 wilson08   (501) staff       (20)        1 2024-05-15 07:43:25.000000 general_operator-0.1.1/general_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 wilson08   (501) staff       (20)       90 2024-05-15 07:43:25.000000 general_operator-0.1.1/general_operator.egg-info/requires.txt
+-rw-r--r--   0 wilson08   (501) staff       (20)       17 2024-05-15 07:43:25.000000 general_operator-0.1.1/general_operator.egg-info/top_level.txt
+-rw-r--r--   0 wilson08   (501) staff       (20)       38 2024-05-15 07:43:25.637212 general_operator-0.1.1/setup.cfg
+-rw-r--r--   0 wilson08   (501) staff       (20)     1370 2024-05-15 07:40:17.000000 general_operator-0.1.1/setup.py
```

### Comparing `general_operator-0.1/PKG-INFO` & `general_operator-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general_operator
-Version: 0.1
+Version: 0.1.1
 Summary: general operator for fastapi write sql and redis
 Home-page: https://github.com/littlebluewhite/node_object_module
 Author: wilson
 Author-email: wwilson008@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -13,20 +13,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi==0.83.0
-Requires-Dist: influxdb-client==1.42.0
-Requires-Dist: pydantic==1.10.15
-Requires-Dist: redis==5.0.4
-Requires-Dist: SQLAlchemy==2.0.30
-Requires-Dist: uvicorn==0.29.0
+Requires-Dist: fastapi>=0.83.0
+Requires-Dist: influxdb-client>=1.42.0
+Requires-Dist: pydantic>=1.10.15
+Requires-Dist: redis>=5.0.4
+Requires-Dist: SQLAlchemy>=2.0.30
 
 # node_object_module version 2.3.3
 
 * API node rule
   1. API node 包含四張表(node, node_base, device_info, third_dimension_instance)一對一關係
   2. 只能透過API node的update去修改或新增device_info和third_dimension_instance這兩張表
   3. node只能有一個parent node, 可以有多個child nodes
```

### Comparing `general_operator-0.1/README.md` & `general_operator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/app/SQL/database.py` & `general_operator-0.1.1/general_operator/app/SQL/database.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/app/SQL/sql_operate.py` & `general_operator-0.1.1/general_operator/app/SQL/sql_operate.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/app/influxdb/influxdb.py` & `general_operator-0.1.1/general_operator/app/influxdb/influxdb.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/app/influxdb/influxdb_operate.py` & `general_operator-0.1.1/general_operator/app/influxdb/influxdb_operate.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/app/redis_db/redis.py` & `general_operator-0.1.1/general_operator/app/redis_db/redis.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/app/redis_db/redis_operate.py` & `general_operator-0.1.1/general_operator/app/redis_db/redis_operate.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/dependencies/get_query_dependencies.py` & `general_operator-0.1.1/general_operator/dependencies/get_query_dependencies.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/function/General_operate.py` & `general_operator-0.1.1/general_operator/function/General_operate.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/function/create_data_structure.py` & `general_operator-0.1.1/general_operator/function/create_data_structure.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/function/search_function.py` & `general_operator-0.1.1/general_operator/function/search_function.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator/routers/General_table_router.py` & `general_operator-0.1.1/general_operator/routers/General_table_router.py`

 * *Files identical despite different names*

### Comparing `general_operator-0.1/general_operator.egg-info/PKG-INFO` & `general_operator-0.1.1/general_operator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general_operator
-Version: 0.1
+Version: 0.1.1
 Summary: general operator for fastapi write sql and redis
 Home-page: https://github.com/littlebluewhite/node_object_module
 Author: wilson
 Author-email: wwilson008@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -13,20 +13,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi==0.83.0
-Requires-Dist: influxdb-client==1.42.0
-Requires-Dist: pydantic==1.10.15
-Requires-Dist: redis==5.0.4
-Requires-Dist: SQLAlchemy==2.0.30
-Requires-Dist: uvicorn==0.29.0
+Requires-Dist: fastapi>=0.83.0
+Requires-Dist: influxdb-client>=1.42.0
+Requires-Dist: pydantic>=1.10.15
+Requires-Dist: redis>=5.0.4
+Requires-Dist: SQLAlchemy>=2.0.30
 
 # node_object_module version 2.3.3
 
 * API node rule
   1. API node 包含四張表(node, node_base, device_info, third_dimension_instance)一對一關係
   2. 只能透過API node的update去修改或新增device_info和third_dimension_instance這兩張表
   3. node只能有一個parent node, 可以有多個child nodes
```

### Comparing `general_operator-0.1/setup.py` & `general_operator-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='general_operator',
-    version='0.1',
+    version='0.1.1',
     packages=['general_operator', 'general_operator.app', 'general_operator.app.SQL', 'general_operator.app.influxdb',
               'general_operator.app.redis_db', 'general_operator.dependencies', 'general_operator.function', 'general_operator.routers',],
     install_requires=[
-        'fastapi==0.83.0',
-        'influxdb-client==1.42.0',
-        'pydantic==1.10.15',
-        'redis==5.0.4',
-        'SQLAlchemy==2.0.30',
-        'uvicorn==0.29.0'
+        'fastapi>=0.83.0',
+        'influxdb-client>=1.42.0',
+        'pydantic>=1.10.15',
+        'redis>=5.0.4',
+        'SQLAlchemy>=2.0.30'
     ],
     author='wilson',
     author_email='wwilson008@gmail.com',
     description='general operator for fastapi write sql and redis',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/littlebluewhite/node_object_module',
```

