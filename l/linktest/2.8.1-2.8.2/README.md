# Comparing `tmp/linktest-2.8.1.tar.gz` & `tmp/linktest-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.8.1.tar", last modified: Tue May 14 06:39:20 2024, max compression
+gzip compressed data, was "linktest-2.8.2.tar", last modified: Wed May 15 06:44:02 2024, max compression
```

## Comparing `linktest-2.8.1.tar` & `linktest-2.8.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-14 06:39:20.613822 linktest-2.8.1/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-14 06:39:20.613583 linktest-2.8.1/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-14 06:39:20.609349 linktest-2.8.1/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-14 04:10:42.000000 linktest-2.8.1/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-13 08:05:43.000000 linktest-2.8.1/linktest/auto_generate_testcase_list-backup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29078 2024-05-14 04:05:58.000000 linktest-2.8.1/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38554 2024-05-14 06:11:04.000000 linktest-2.8.1/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102436 2024-05-14 06:04:30.000000 linktest-2.8.1/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-14 04:10:47.000000 linktest-2.8.1/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-14 03:54:33.000000 linktest-2.8.1/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-14 06:39:20.613277 linktest-2.8.1/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-14 06:39:20.000000 linktest-2.8.1/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1498 2024-05-14 06:39:20.000000 linktest-2.8.1/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-14 06:39:20.000000 linktest-2.8.1/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-14 06:39:20.000000 linktest-2.8.1/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-14 06:39:20.000000 linktest-2.8.1/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-14 06:39:20.613870 linktest-2.8.1/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-14 06:39:15.000000 linktest-2.8.1/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-15 06:44:02.695959 linktest-2.8.2/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-15 06:44:02.695634 linktest-2.8.2/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-15 06:44:02.692582 linktest-2.8.2/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-15 06:35:55.000000 linktest-2.8.2/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/auto_generate_testcase_list-backup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    28841 2024-05-15 06:37:29.000000 linktest-2.8.2/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38554 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102436 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-15 06:35:59.000000 linktest-2.8.2/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-15 06:44:02.695225 linktest-2.8.2/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1498 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-15 06:44:02.696015 linktest-2.8.2/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-15 06:43:57.000000 linktest-2.8.2/setup.py
```

### Comparing `linktest-2.8.1/linktest/appium_utils.py` & `linktest-2.8.2/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/auto_generate_testcase_list-backup.py` & `linktest-2.8.2/linktest/auto_generate_testcase_list-backup.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/auto_generate_testcase_list.py` & `linktest-2.8.2/linktest/auto_generate_testcase_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,20 +148,15 @@
                     exec("base_class_name = %s" % base_class_name_string, namespace)
                     base_class_name = namespace['base_class_name']
 
                     # If base_class_name is not a subclass of BaseTestCase, then this class is not considered a TestCase class.
                     if not issubclass(base_class_name, BaseTestCase):
                         break
 
-                    module_path_str = file_full_name.split(PROJECT_INFO.project_path)[1]
-                    module_path_str = module_path_str.replace(os.sep, ".")
-                    module_path_str = module_path_str.replace(".tests.", "tests.")
-                    module_path_str = module_path_str.strip()
-                    module_path_str = module_path_str[:-3]
-
+                    module_path_str = file_full_name.split(PROJECT_INFO.project_path + os.sep)[1].replace(os.sep, ".").strip()[:-3]
                     module_import_str = "from %s import %s" % (module_path_str, class_name)
                     exec(module_import_str, namespace)
 
                     testcase = None
                     exec("testcase = %s" % class_name, namespace)
                     testcase = namespace['testcase']
                     ignore_flag = False
```

### Comparing `linktest-2.8.1/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.8.2/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/base_testcase.py` & `linktest-2.8.2/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/clean_data.py` & `linktest-2.8.2/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/conver_xml_into_db.py` & `linktest-2.8.2/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/database_helper.py` & `linktest-2.8.2/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/date_utilities.py` & `linktest-2.8.2/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/doctor.py` & `linktest-2.8.2/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/framework_log.py` & `linktest-2.8.2/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/generate_html_log.py` & `linktest-2.8.2/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/get_adb_devices.py` & `linktest-2.8.2/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/get_ios_devices_list.py` & `linktest-2.8.2/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/get_platform_info.py` & `linktest-2.8.2/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/get_project_info.py` & `linktest-2.8.2/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/html_report.py` & `linktest-2.8.2/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/logged_requests.py` & `linktest-2.8.2/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/main.py` & `linktest-2.8.2/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/memory_usage.py` & `linktest-2.8.2/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/re_func.py` & `linktest-2.8.2/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/run.py` & `linktest-2.8.2/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/run_testcase_thread.py` & `linktest-2.8.2/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/scp_report_to_specified_path.py` & `linktest-2.8.2/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/selenium_helper.py` & `linktest-2.8.2/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/timeout_thread.py` & `linktest-2.8.2/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/ui_testcase.py` & `linktest-2.8.2/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/update_config.py` & `linktest-2.8.2/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/webdriver_wrapper.py` & `linktest-2.8.2/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/webdriver_wrapper_chrome.py` & `linktest-2.8.2/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/webdriver_wrapper_edge.py` & `linktest-2.8.2/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/webdriver_wrapper_firefox.py` & `linktest-2.8.2/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/webdriver_wrapper_ie.py` & `linktest-2.8.2/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/webdriver_wrapper_safari.py` & `linktest-2.8.2/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest/xml_report.py` & `linktest-2.8.2/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.1/linktest.egg-info/SOURCES.txt` & `linktest-2.8.2/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

