# Comparing `tmp/inventory-monitor-7.1.0.tar.gz` & `tmp/inventory-monitor-8.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventory-monitor-7.1.0.tar", last modified: Thu Jan 25 11:42:51 2024, max compression
+gzip compressed data, was "inventory-monitor-8.0.0b1.tar", last modified: Wed May 15 10:21:42 2024, max compression
```

## Comparing `inventory-monitor-7.1.0.tar` & `inventory-monitor-8.0.0b1.tar`

### file list

```diff
@@ -1,58 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 11:42:51.170275 inventory-monitor-7.1.0/
--rw-r--r--   0 root         (0) root         (0)       66 2022-08-17 08:16:04.000000 inventory-monitor-7.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      186 2024-01-25 11:42:51.170275 inventory-monitor-7.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2022-11-11 11:56:29.000000 inventory-monitor-7.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 11:42:51.162274 inventory-monitor-7.1.0/inventory_monitor/
--rw-r--r--   0 root         (0) root         (0)      316 2024-01-25 11:40:07.000000 inventory-monitor-7.1.0/inventory_monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 11:42:51.166275 inventory-monitor-7.1.0/inventory_monitor/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 10:45:32.000000 inventory-monitor-7.1.0/inventory_monitor/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7025 2023-04-04 11:53:46.000000 inventory-monitor-7.1.0/inventory_monitor/api/serializers.py
--rw-r--r--   0 root         (0) root         (0)      476 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/api/urls.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/api/views.py
--rw-r--r--   0 root         (0) root         (0)    16616 2023-03-27 12:08:03.000000 inventory-monitor-7.1.0/inventory_monitor/filtersets.py
--rw-r--r--   0 root         (0) root         (0)    20107 2023-06-06 11:41:23.000000 inventory-monitor-7.1.0/inventory_monitor/forms.py
--rw-r--r--   0 root         (0) root         (0)      459 2022-09-05 08:34:29.000000 inventory-monitor-7.1.0/inventory_monitor/graphql.py
--rw-r--r--   0 root         (0) root         (0)     1798 2024-01-25 11:41:07.000000 inventory-monitor-7.1.0/inventory_monitor/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 11:42:51.166275 inventory-monitor-7.1.0/inventory_monitor/migrations/
--rw-r--r--   0 root         (0) root         (0)     2329 2022-09-01 10:14:20.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     3198 2022-11-02 08:30:17.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0002_contractor_contract.py
--rw-r--r--   0 root         (0) root         (0)     1811 2022-11-11 11:48:13.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
--rw-r--r--   0 root         (0) root         (0)      342 2022-11-11 11:48:53.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0004_delete_invmonfileattachment.py
--rw-r--r--   0 root         (0) root         (0)     1840 2022-11-22 11:20:11.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0005_invoice.py
--rw-r--r--   0 root         (0) root         (0)      409 2022-12-01 11:16:30.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0006_invoice_project.py
--rw-r--r--   0 root         (0) root         (0)     5622 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0008_componentservice_comments.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0009_alter_component_items.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-03-27 12:15:02.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-03-27 12:09:05.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-03 15:32:31.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0012_probe_creation_time.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 12:29:41.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/0013_alter_probe_creation_time.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-22 08:26:09.000000 inventory-monitor-7.1.0/inventory_monitor/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2024-01-04 13:04:30.000000 inventory-monitor-7.1.0/inventory_monitor/models.py
--rw-r--r--   0 root         (0) root         (0)     1187 2023-06-06 11:41:23.000000 inventory-monitor-7.1.0/inventory_monitor/navigation.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/search.py
--rw-r--r--   0 root         (0) root         (0)     5070 2023-04-05 08:31:19.000000 inventory-monitor-7.1.0/inventory_monitor/tables.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-04-13 10:44:43.000000 inventory-monitor-7.1.0/inventory_monitor/template_content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 11:42:51.158274 inventory-monitor-7.1.0/inventory_monitor/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 11:42:51.170275 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-15 12:39:23.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-03-27 12:07:28.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/component.html
--rw-r--r--   0 root         (0) root         (0)     2988 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/componentservice.html
--rw-r--r--   0 root         (0) root         (0)     6537 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/contract.html
--rw-r--r--   0 root         (0) root         (0)     2109 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/contractor.html
--rw-r--r--   0 root         (0) root         (0)     1558 2023-04-13 10:27:02.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html
--rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 13:55:51.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/import_component_button.html
--rw-r--r--   0 root         (0) root         (0)     2238 2022-11-23 07:44:17.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
--rw-r--r--   0 root         (0) root         (0)     2301 2023-02-28 13:24:51.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/invoice.html
--rw-r--r--   0 root         (0) root         (0)     5690 2023-04-04 12:47:57.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/probe.html
--rw-r--r--   0 root         (0) root         (0)     3146 2023-06-06 11:41:23.000000 inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/probe_diff.html
--rw-r--r--   0 root         (0) root         (0)     4188 2023-06-06 11:41:23.000000 inventory-monitor-7.1.0/inventory_monitor/urls.py
--rw-r--r--   0 root         (0) root         (0)    15718 2024-01-25 11:32:41.000000 inventory-monitor-7.1.0/inventory_monitor/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 11:42:51.162274 inventory-monitor-7.1.0/inventory_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2024-01-25 11:42:51.000000 inventory-monitor-7.1.0/inventory_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2312 2024-01-25 11:42:51.000000 inventory-monitor-7.1.0/inventory_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-25 11:42:51.000000 inventory-monitor-7.1.0/inventory_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:55:56.000000 inventory-monitor-7.1.0/inventory_monitor.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2024-01-25 11:42:51.000000 inventory-monitor-7.1.0/inventory_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-25 11:42:51.170275 inventory-monitor-7.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      282 2024-01-25 11:39:54.000000 inventory-monitor-7.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-17 08:16:04.000000 inventory-monitor-8.0.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2022-11-11 11:56:29.000000 inventory-monitor-8.0.0b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor/
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 10:45:32.000000 inventory-monitor-8.0.0b1/inventory_monitor/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7075 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/api/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      496 2024-05-15 08:27:14.000000 inventory-monitor-8.0.0b1/inventory_monitor/api/urls.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/api/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-15 08:24:02.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7346 2024-05-15 08:24:36.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/component.py
+-rw-r--r--   0 root         (0) root         (0)     5525 2024-05-15 08:24:24.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2024-05-15 08:24:38.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/contract.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2024-05-15 08:24:40.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/contractor.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2024-05-15 08:24:43.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     5305 2024-05-15 08:24:46.000000 inventory-monitor-8.0.0b1/inventory_monitor/filtersets/probe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor/forms/
+-rw-r--r--   0 root         (0) root         (0)      289 2024-05-15 08:23:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6698 2024-05-15 10:03:15.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/component.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2024-05-15 10:03:19.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2024-05-15 10:03:13.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/contract.py
+-rw-r--r--   0 root         (0) root         (0)      766 2024-05-15 10:00:52.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/contractor.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-05-15 10:03:10.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2024-05-15 10:03:03.000000 inventory-monitor-8.0.0b1/inventory_monitor/forms/probe.py
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/graphql.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.687589 inventory-monitor-8.0.0b1/inventory_monitor/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2329 2022-09-01 10:14:20.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2022-11-02 08:30:17.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0002_contractor_contract.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2022-11-11 11:48:13.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
+-rw-r--r--   0 root         (0) root         (0)      342 2022-11-11 11:48:53.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0004_delete_invmonfileattachment.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2022-11-22 11:20:11.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0005_invoice.py
+-rw-r--r--   0 root         (0) root         (0)      409 2022-12-01 11:16:30.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0006_invoice_project.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0008_componentservice_comments.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0009_alter_component_items.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-03-27 12:15:02.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-03-27 12:09:05.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0011_alter_component_options_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-03 15:32:31.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0012_probe_creation_time.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 12:29:41.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/0013_alter_probe_creation_time.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-22 08:26:09.000000 inventory-monitor-8.0.0b1/inventory_monitor/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.687589 inventory-monitor-8.0.0b1/inventory_monitor/models/
+-rw-r--r--   0 root         (0) root         (0)      296 2024-05-15 08:20:10.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/component.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-05-15 08:12:07.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/contract.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/contractor.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/models/probe.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/navigation.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.687589 inventory-monitor-8.0.0b1/inventory_monitor/tables/
+-rw-r--r--   0 root         (0) root         (0)      296 2024-05-15 08:23:40.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/component.py
+-rw-r--r--   0 root         (0) root         (0)      857 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/contract.py
+-rw-r--r--   0 root         (0) root         (0)      487 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/contractor.py
+-rw-r--r--   0 root         (0) root         (0)      864 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/invoice.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/tables/probe.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/template_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.679589 inventory-monitor-8.0.0b1/inventory_monitor/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-15 12:39:23.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-03-27 12:07:28.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/component.html
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/componentservice.html
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/contract.html
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/contractor.html
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-04-13 10:27:02.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/device_probes_include.html
+-rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 13:55:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/import_component_button.html
+-rw-r--r--   0 root         (0) root         (0)     2238 2022-11-23 07:44:17.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-02-28 13:24:51.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/invoice.html
+-rw-r--r--   0 root         (0) root         (0)     5690 2023-04-04 12:47:57.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/probe.html
+-rw-r--r--   0 root         (0) root         (0)     3146 2023-06-06 11:41:23.000000 inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/probe_diff.html
+-rw-r--r--   0 root         (0) root         (0)     4203 2024-05-15 08:22:10.000000 inventory-monitor-8.0.0b1/inventory_monitor/urls.py
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/inventory_monitor/views/
+-rw-r--r--   0 root         (0) root         (0)      290 2024-05-15 08:23:28.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/component.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/component_service.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/contract.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/contractor.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/inventory_monitor/views/probe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:21:42.683589 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-15 10:21:42.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3548 2024-05-15 10:21:42.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:21:42.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:55:56.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-15 10:21:42.000000 inventory-monitor-8.0.0b1/inventory_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 10:21:42.691589 inventory-monitor-8.0.0b1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-05-15 08:05:18.000000 inventory-monitor-8.0.0b1/setup.py
```

### Comparing `inventory-monitor-7.1.0/inventory_monitor/api/serializers.py` & `inventory-monitor-8.0.0b1/inventory_monitor/api/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dcim.api.serializers import (NestedDeviceSerializer,
                                   NestedLocationSerializer,
                                   NestedSiteSerializer)
 from netbox.api.serializers import (NetBoxModelSerializer,
                                     WritableNestedSerializer)
 from rest_framework import serializers
 
-from ..models import (Component, ComponentService, Contract, Contractor,
-                      Invoice, Probe)
+from inventory_monitor.models import (Component, ComponentService, Contract, Contractor,
+                                      Invoice, Probe)
 
 
 class ProbeSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:inventory_monitor-api:probe-detail'
     )
     device = NestedDeviceSerializer(allow_null=True)
@@ -46,15 +46,16 @@
 class NestedProbeSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:inventory_monitor-api:probe-detail'
     )
 
     class Meta:
         model = Probe
-        fields = ['id', 'url', 'display', 'name', 'serial', 'time', 'creation_time']
+        fields = ['id', 'url', 'display', 'name',
+                  'serial', 'time', 'creation_time']
 
 
 class ContractorSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:inventory_monitor-api:contractor-detail'
     )
```

### Comparing `inventory-monitor-7.1.0/inventory_monitor/api/views.py` & `inventory-monitor-8.0.0b1/inventory_monitor/api/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from netbox.api.viewsets import NetBoxModelViewSet
 
-from .. import filtersets, models
+from inventory_monitor import filtersets, models
 from .serializers import (ComponentSerializer, ComponentServiceSerializer,
                           ContractorSerializer, ContractSerializer,
                           InvoiceSerializer, ProbeSerializer)
 
 
 class ProbeViewSet(NetBoxModelViewSet):
     queryset = models.Probe.objects.prefetch_related('tags', 'device')
@@ -27,15 +27,16 @@
 class InvoiceViewSet(NetBoxModelViewSet):
     queryset = models.Invoice.objects.prefetch_related('tags', 'contract')
     serializer_class = InvoiceSerializer
     filterset_class = filtersets.InvoiceFilterSet
 
 
 class ComponentViewSet(NetBoxModelViewSet):
-    queryset = models.Component.objects.prefetch_related('tags', 'order_contract')
+    queryset = models.Component.objects.prefetch_related(
+        'tags', 'order_contract')
     serializer_class = ComponentSerializer
     filterset_class = filtersets.ComponentFilterSet
 
 
 class ComponentServiceViewSet(NetBoxModelViewSet):
     queryset = models.ComponentService.objects.prefetch_related(
         'tags', 'contract')
```

### Comparing `inventory-monitor-7.1.0/inventory_monitor/helpers.py` & `inventory-monitor-8.0.0b1/inventory_monitor/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import django_tables2
 from utilities.templatetags.builtins.filters import register
 from django.contrib.contenttypes.models import ContentType
 
 
 def get_content_type_or_none(app_label, model):
     try:
-        content_type = ContentType.objects.get(app_label=app_label, model=model)
+        content_type = ContentType.objects.get(
+            app_label=app_label, model=model)
         return content_type
     except Exception as e:
         return None
 
 
 @register.filter()
 def to_czech_crown(number):
```

### Comparing `inventory-monitor-7.1.0/inventory_monitor/migrations/0001_initial.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/migrations/0002_contractor_contract.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0002_contractor_contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/migrations/0005_invoice.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0005_invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py` & `inventory-monitor-8.0.0b1/inventory_monitor/migrations/0011_alter_component_options_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/navigation.py` & `inventory-monitor-8.0.0b1/inventory_monitor/navigation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from extras.plugins import PluginMenu, PluginMenuItem
+from netbox.plugins import PluginMenu, PluginMenuItem
 
 menu = PluginMenu(
     label='Inventory Monitor',
     icon_class="mdi mdi-monitor",
     groups=(
         ("Network Probe",
          (
```

### Comparing `inventory-monitor-7.1.0/inventory_monitor/search.py` & `inventory-monitor-8.0.0b1/inventory_monitor/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 from netbox.search import SearchIndex, register_search
 from .models import Contract, Contractor, Invoice, Probe, Component, ComponentService
 
+
 @register_search
 class ContractIndex(SearchIndex):
     model = Contract
 
     fields = (
         ('name', 100),
         ('name_internal', 100),
         ('comments', 5000)
     )
 
+
 @register_search
 class ContractorIndex(SearchIndex):
     model = Contractor
 
     fields = (
         ('name', 100),
         ('company', 100),
         ('address', 5000),
         ('address', 5000)
     )
 
+
 @register_search
 class InvoiceIndex(SearchIndex):
     model = Invoice
     fields = (
         ('name', 100),
         ('name_internal', 100),
         ('project', 300),
         ('comments', 5000)
     )
 
+
 @register_search
 class ProbeIndex(SearchIndex):
     model = Probe
 
     fields = (
         ('device_descriptor', 100),
         ('site_descriptor', 100),
         ('location_descriptor', 100),
         ('name', 100),
         ('serial', 100),
         ('description', 5000),
         ('comments', 5000)
     )
 
+
 @register_search
 class ComponentIndex(SearchIndex):
     model = Component
 
     fields = (
         ('serial', 100),
         ('serial_actual', 100),
         ('partnumber', 100),
         ('comments', 5000)
     )
 
+
 @register_search
 class ComponentServiceIndex(SearchIndex):
     model = ComponentService
 
     fields = (
         ('service_category', 100),
         ('service_category_vendor', 100),
```

### Comparing `inventory-monitor-7.1.0/inventory_monitor/template_content.py` & `inventory-monitor-8.0.0b1/inventory_monitor/template_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcim.models import InventoryItem
-from extras.plugins import PluginTemplateExtension
+from netbox.plugins import PluginTemplateExtension
 
 from .models import Probe
 
 from django.conf import settings
 plugin_settings = settings.PLUGINS_CONFIG.get('inventory_monitor', {})
 import_component_url = plugin_settings.get(
     "import_component_url", '/extras/scripts/component_import.ImportComponent/')
```

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/component.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/component.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/componentservice.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/componentservice.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/contract.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/contract.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/contractor.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/contractor.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/device_probes_include.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/invoice.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/invoice.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/probe.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/probe.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/templates/inventory_monitor/probe_diff.html` & `inventory-monitor-8.0.0b1/inventory_monitor/templates/inventory_monitor/probe_diff.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-7.1.0/inventory_monitor/urls.py` & `inventory-monitor-8.0.0b1/inventory_monitor/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from django.urls import path
 from netbox.views.generic import ObjectChangeLogView
 
-from . import models, views
+from inventory_monitor import models, views
 
 urlpatterns = (
     # Probes
     path('probes/', views.ProbeListView.as_view(), name='probe_list'),
     path('probes/add/', views.ProbeEditView.as_view(), name='probe_add'),
     path('probes/<int:pk>/', views.ProbeView.as_view(), name='probe'),
     path('probes/<int:pk>/edit/', views.ProbeEditView.as_view(), name='probe_edit'),
     path('probes/<int:pk>/delete/',
          views.ProbeDeleteView.as_view(), name='probe_delete'),
     path('probes/<int:pk>/changelog/', ObjectChangeLogView.as_view(),
          name='probe_changelog', kwargs={'model': models.Probe}),
     path("probes/delete/", views.ProbeBulkDeleteView.as_view(),
          name="probe_bulk_delete",),
     # Probe Diff
-     path('probe_diff/', views.ProbeDiffView.as_view(), name='probediff'),
+    path('probe_diff/', views.ProbeDiffView.as_view(), name='probediff'),
 
     # Contractors
     path('contractors/', views.ContractorListView.as_view(), name='contractor_list'),
     path('contractors/add/', views.ContractorEditView.as_view(),
          name='contractor_add'),
     path('contractors/<int:pk>/', views.ContractorView.as_view(), name='contractor'),
     path('contractors/<int:pk>/edit/',
```

### Comparing `inventory-monitor-7.1.0/inventory_monitor.egg-info/SOURCES.txt` & `inventory-monitor-8.0.0b1/inventory_monitor.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,80 @@
 MANIFEST.in
 README.md
 setup.py
 inventory_monitor/__init__.py
-inventory_monitor/filtersets.py
-inventory_monitor/forms.py
 inventory_monitor/graphql.py
 inventory_monitor/helpers.py
-inventory_monitor/models.py
 inventory_monitor/navigation.py
 inventory_monitor/search.py
-inventory_monitor/tables.py
 inventory_monitor/template_content.py
 inventory_monitor/urls.py
-inventory_monitor/views.py
+inventory_monitor/version.py
 inventory_monitor.egg-info/PKG-INFO
 inventory_monitor.egg-info/SOURCES.txt
 inventory_monitor.egg-info/dependency_links.txt
 inventory_monitor.egg-info/not-zip-safe
 inventory_monitor.egg-info/top_level.txt
 inventory_monitor/api/__init__.py
 inventory_monitor/api/serializers.py
 inventory_monitor/api/urls.py
 inventory_monitor/api/views.py
+inventory_monitor/filtersets/__init__.py
+inventory_monitor/filtersets/component.py
+inventory_monitor/filtersets/component_service.py
+inventory_monitor/filtersets/contract.py
+inventory_monitor/filtersets/contractor.py
+inventory_monitor/filtersets/invoice.py
+inventory_monitor/filtersets/probe.py
+inventory_monitor/forms/__init__.py
+inventory_monitor/forms/component.py
+inventory_monitor/forms/component_service.py
+inventory_monitor/forms/contract.py
+inventory_monitor/forms/contractor.py
+inventory_monitor/forms/invoice.py
+inventory_monitor/forms/probe.py
 inventory_monitor/migrations/0001_initial.py
 inventory_monitor/migrations/0002_contractor_contract.py
 inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
 inventory_monitor/migrations/0004_delete_invmonfileattachment.py
 inventory_monitor/migrations/0005_invoice.py
 inventory_monitor/migrations/0006_invoice_project.py
 inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
 inventory_monitor/migrations/0008_componentservice_comments.py
 inventory_monitor/migrations/0009_alter_component_items.py
 inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
 inventory_monitor/migrations/0011_alter_component_options_and_more.py
 inventory_monitor/migrations/0012_probe_creation_time.py
 inventory_monitor/migrations/0013_alter_probe_creation_time.py
 inventory_monitor/migrations/__init__.py
+inventory_monitor/models/__init__.py
+inventory_monitor/models/component.py
+inventory_monitor/models/component_service.py
+inventory_monitor/models/contract.py
+inventory_monitor/models/contractor.py
+inventory_monitor/models/invoice.py
+inventory_monitor/models/probe.py
+inventory_monitor/tables/__init__.py
+inventory_monitor/tables/component.py
+inventory_monitor/tables/component_service.py
+inventory_monitor/tables/contract.py
+inventory_monitor/tables/contractor.py
+inventory_monitor/tables/invoice.py
+inventory_monitor/tables/probe.py
 inventory_monitor/templates/inventory_monitor/__init__.py
 inventory_monitor/templates/inventory_monitor/component.html
 inventory_monitor/templates/inventory_monitor/componentservice.html
 inventory_monitor/templates/inventory_monitor/contract.html
 inventory_monitor/templates/inventory_monitor/contractor.html
 inventory_monitor/templates/inventory_monitor/device_probes_include.html
 inventory_monitor/templates/inventory_monitor/import_component_button.html
 inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
 inventory_monitor/templates/inventory_monitor/invoice.html
 inventory_monitor/templates/inventory_monitor/probe.html
-inventory_monitor/templates/inventory_monitor/probe_diff.html
+inventory_monitor/templates/inventory_monitor/probe_diff.html
+inventory_monitor/views/__init__.py
+inventory_monitor/views/component.py
+inventory_monitor/views/component_service.py
+inventory_monitor/views/contract.py
+inventory_monitor/views/contractor.py
+inventory_monitor/views/invoice.py
+inventory_monitor/views/probe.py
```

