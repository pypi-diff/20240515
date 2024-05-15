# Comparing `tmp/netbox-contract-2.0.9.tar.gz` & `tmp/netbox_contract-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-contract-2.0.9.tar", last modified: Fri Dec 15 21:42:05 2023, max compression
+gzip compressed data, was "netbox_contract-2.1.0.tar", last modified: Wed May 15 19:33:50 2024, max compression
```

## Comparing `netbox-contract-2.0.9.tar` & `netbox_contract-2.1.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.089381 netbox-contract-2.0.9/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.9/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.9/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5490 2023-12-15 21:42:05.085381 netbox-contract-2.0.9/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4920 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      854 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-12-15 21:42:05.089381 netbox-contract-2.0.9/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.053381 netbox-contract-2.0.9/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.061381 netbox-contract-2.0.9/src/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.065381 netbox-contract-2.0.9/src/netbox_contract/api/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.9/src/netbox_contract/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5036 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/api/serializers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      388 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/api/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      979 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/api/views.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      185 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/constants.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1320 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/filtersets.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10398 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/forms.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.077381 netbox-contract-2.0.9/src/netbox_contract/migrations/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6090 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0001_initial.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      856 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1578 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      583 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      562 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0006_alter_contract_circuit.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      402 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0007_invoice_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      385 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0008_invoice_comments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      427 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0009_contract_external_reference.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      493 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0010_invoice_contracts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      603 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0011_auto_20230122_2112.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      338 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0012_remove_invoice_contract.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      548 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      421 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0014_contract_end_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2103 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0015_contractassignement.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      629 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0016_contract_parent.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      415 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1386 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0018_contract_external_partie_object_id_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1382 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0019_auto_20230924_1813.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      623 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0020_alter_contract_external_partie.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      662 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0021_alter_contract_external_partie.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-12-15 21:38:43.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0022_alter_contract_internal_partie_alter_contract_parent.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5642 2023-12-15 21:27:05.000000 netbox-contract-2.0.9/src/netbox_contract/models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2192 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/navigation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/search.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5365 2023-12-15 21:27:24.000000 netbox-contract-2.0.9/src/netbox_contract/tables.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3364 2023-12-15 21:11:25.000000 netbox-contract-2.0.9/src/netbox_contract/template_content.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.077381 netbox-contract-2.0.9/src/netbox_contract/templates/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2566 2023-06-25 09:18:53.000000 netbox-contract-2.0.9/src/netbox_contract/templates/contact_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      917 2023-06-18 13:30:49.000000 netbox-contract-2.0.9/src/netbox_contract/templates/contract_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-06-18 13:30:49.000000 netbox-contract-2.0.9/src/netbox_contract/templates/contract_list_bottom.html
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.085381 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4818 2023-12-15 21:28:15.000000 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/contract.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/contract_assignement.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2334 2023-09-03 08:33:50.000000 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/invoice.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1136 2023-06-25 09:18:53.000000 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/serviceprovider.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4662 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9803 2023-12-15 21:38:42.000000 netbox-contract-2.0.9/src/netbox_contract/views.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.085381 netbox-contract-2.0.9/src/netbox_contract.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5490 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2745 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-11-12 14:38:39.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:50.405434 netbox_contract-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-15 19:33:50.405434 netbox_contract-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:33:50.405434 netbox_contract-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:50.393434 netbox_contract-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:50.397434 netbox_contract-2.1.0/src/netbox_contract/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:50.401434 netbox_contract-2.1.0/src/netbox_contract/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:50.405434 netbox_contract-2.1.0/src/netbox_contract/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0006_alter_contract_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0007_invoice_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0008_invoice_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0009_contract_external_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0010_invoice_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0011_auto_20230122_2112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0012_remove_invoice_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0014_contract_end_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0015_contractassignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0016_contract_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0018_contract_external_partie_object_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0019_auto_20230924_1813.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0020_alter_contract_external_partie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0021_alter_contract_external_partie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0022_alter_contract_internal_partie_alter_contract_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0023_rename_contractassignement_contractassignment_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0024_remove_contract_external_partie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0025_remove_contract_circuit_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/0026_auto_20240421_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:50.405434 netbox_contract-2.1.0/src/netbox_contract/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/templates/contract_assignments_bottom.html
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/templates/contract_assignments_bottom_old.html
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/templates/contract_list_bottom.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:50.405434 netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/contract.html
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/contractassignment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/serviceprovider.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-05-15 19:33:40.000000 netbox_contract-2.1.0/src/netbox_contract/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:33:50.405434 netbox_contract-2.1.0/src/netbox_contract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-15 19:33:50.000000 netbox_contract-2.1.0/src/netbox_contract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-15 19:33:50.000000 netbox_contract-2.1.0/src/netbox_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:33:50.000000 netbox_contract-2.1.0/src/netbox_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:33:50.000000 netbox_contract-2.1.0/src/netbox_contract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:33:50.000000 netbox_contract-2.1.0/src/netbox_contract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:33:50.000000 netbox_contract-2.1.0/src/netbox_contract.egg-info/top_level.txt
```

### Comparing `netbox-contract-2.0.9/LICENSE` & `netbox_contract-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/pyproject.toml` & `netbox_contract-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "netbox-contract"
-version = "2.0.9"
+version = "2.1.0"
 authors = [
   { name="Marc Lebreuil", email="marc@famillelebreuil.net" },
 ]
 description = "Contract management plugin for Netbox"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dependencies = [
     'python-dateutil',
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/__init__.py` & `netbox_contract-2.1.0/src/netbox_contract/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 
 
 class ContractsConfig(PluginConfig):
     name = 'netbox_contract'
     verbose_name = 'Netbox contract'
     description = 'Contract management plugin for Netbox'
-    version = '2.0.9'
+    version = '2.1.0'
     author = 'Marc Lebreuil'
     author_email = 'marc@famillelebreuil.net'
     base_url = 'contracts'
-    min_version = '3.5.0'
+    min_version = '4.0.2'
     required_settings = []
     default_settings = {
         'top_level_menu': False,
         'default_accounting_dimensions': {
             'account': '',
             'project': '',
             'cost center': '',
         },
+        'mandatory_contract_fields': [],
+        'hidden_contract_fields': [],
+        'mandatory_invoice_fields': [],
+        'hidden_invoice_fields': [],
     }
 
 
 config = ContractsConfig
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/api/serializers.py` & `netbox_contract-2.1.0/src/netbox_contract/api/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from netbox.api.fields import ContentTypeField
 from netbox.api.serializers import NetBoxModelSerializer, WritableNestedSerializer
 from netbox.constants import NESTED_SERIALIZER_PREFIX
 from rest_framework import serializers
 from tenancy.api.nested_serializers import NestedTenantSerializer
 from utilities.api import get_serializer_for_model
 
-from ..models import Contract, ContractAssignement, Invoice, ServiceProvider
+from ..models import Contract, ContractAssignment, Invoice, ServiceProvider
 
 
 class NestedServiceProviderSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_contract-api:serviceprovider-detail'
     )
 
@@ -34,63 +34,86 @@
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_contract-api:invoice-detail'
     )
 
     class Meta:
         model = Invoice
         fields = ('id', 'url', 'display', 'number')
+        brief_fields = ('id', 'url', 'display', 'number')
 
 
-class NestedContractAssignementSerializer(WritableNestedSerializer):
+class NestedContractAssignmentSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
-        view_name='plugins-api:netbox_contract-api:ContractAssignement-detail'
+        view_name='plugins-api:netbox_contract-api:ContractAssignment-detail'
     )
 
     class Meta:
-        model = ContractAssignement
+        model = ContractAssignment
         fields = ('id', 'url', 'display', 'contract', 'content_object')
+        brief_fields = ('id', 'url', 'display', 'contract', 'content_object')
 
 
 class ContractSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_contract-api:contract-detail'
     )
-    # circuit= NestedCircuitSerializer(many=True, required=False)
-    external_partie = NestedServiceProviderSerializer(many=False)
+    yrc = serializers.DecimalField(max_digits=10, decimal_places=2, read_only=True)
     parent = NestedContractSerializer(many=False, required=False)
     tenant = NestedTenantSerializer(many=False, required=False)
+    external_partie_object_type = ContentTypeField(queryset=ContentType.objects.all())
+    external_partie_object = serializers.SerializerMethodField(read_only=True)
 
     class Meta:
         model = Contract
         fields = (
             'id',
             'url',
             'display',
             'name',
-            'external_partie',
+            'external_partie_object_type',
+            'external_partie_object_id',
+            'external_partie_object',
             'external_reference',
             'internal_partie',
             'tenant',
             'status',
             'start_date',
             'end_date',
             'initial_term',
             'renewal_term',
             'currency',
             'accounting_dimensions',
             'mrc',
+            'yrc',
             'nrc',
             'invoice_frequency',
             'comments',
             'parent',
             'tags',
             'custom_fields',
             'created',
             'last_updated',
         )
+        brief_fields = (
+            'id',
+            'url',
+            'display',
+            'name',
+            'external_partie_object',
+            'status',
+        )
+
+    @swagger_serializer_method(serializer_or_field=serializers.JSONField)
+    def get_external_partie_object(self, instance):
+        serializer = get_serializer_for_model(
+            instance.external_partie_object_type.model_class(),
+            prefix=NESTED_SERIALIZER_PREFIX,
+        )
+        context = {'request': self.context['request']}
+        return serializer(instance.external_partie_object, context=context).data
 
 
 class InvoiceSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_contract-api:invoice-detail'
     )
     contracts = NestedContractSerializer(many=True, required=False)
@@ -111,14 +134,15 @@
             'amount',
             'comments',
             'tags',
             'custom_fields',
             'created',
             'last_updated',
         )
+        brief_fields = ('id', 'url', 'display', 'number', 'contracts')
 
 
 class ServiceProviderSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_contract-api:serviceprovider-detail'
     )
 
@@ -131,37 +155,39 @@
             'name',
             'portal_url',
             'tags',
             'custom_fields',
             'created',
             'last_updated',
         )
+        brief_fields = ('id', 'url', 'display', 'name')
 
 
-class ContractAssignementSerializer(NetBoxModelSerializer):
+class ContractAssignmentSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
-        view_name='plugins-api:netbox_contract-api:contractassignement-detail'
+        view_name='plugins-api:netbox_contract-api:contractassignment-detail'
     )
     content_type = ContentTypeField(queryset=ContentType.objects.all())
     content_object = serializers.SerializerMethodField(read_only=True)
     contract = NestedContractSerializer()
 
     class Meta:
-        model = ContractAssignement
-        fields = [
+        model = ContractAssignment
+        fields = (
             'id',
             'url',
             'display',
             'content_type',
             'object_id',
             'content_object',
             'contract',
             'created',
             'last_updated',
-        ]
+        )
+        brief_fields = ('id', 'url', 'display', 'content_object', 'contract')
 
     @swagger_serializer_method(serializer_or_field=serializers.JSONField)
     def get_content_object(self, instance):
         serializer = get_serializer_for_model(
             instance.content_type.model_class(), prefix=NESTED_SERIALIZER_PREFIX
         )
         context = {'request': self.context['request']}
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/api/views.py` & `netbox_contract-2.1.0/src/netbox_contract/api/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+from django.db.models import F
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from .. import filtersets, models
 from .serializers import (
-    ContractAssignementSerializer,
+    ContractAssignmentSerializer,
     ContractSerializer,
     InvoiceSerializer,
     ServiceProviderSerializer,
 )
 
 
 class ContractViewSet(NetBoxModelViewSet):
-    queryset = models.Contract.objects.prefetch_related('parent', 'circuit', 'tags')
+    queryset = models.Contract.objects.prefetch_related(
+        'parent', 'circuit', 'tags'
+    ).annotate(yrc=F('mrc') * 12)
     serializer_class = ContractSerializer
 
 
 class InvoiceViewSet(NetBoxModelViewSet):
     queryset = models.Invoice.objects.prefetch_related('contracts', 'tags')
     serializer_class = InvoiceSerializer
     filterset_class = filtersets.InvoiceFilterSet
 
 
 class ServiceProviderViewSet(NetBoxModelViewSet):
     queryset = models.ServiceProvider.objects.prefetch_related('tags')
     serializer_class = ServiceProviderSerializer
 
 
-class ContractAssignementViewSet(NetBoxModelViewSet):
-    queryset = models.ContractAssignement.objects.prefetch_related('contract', 'tags')
-    serializer_class = ContractAssignementSerializer
+class ContractAssignmentViewSet(NetBoxModelViewSet):
+    queryset = models.ContractAssignment.objects.prefetch_related('contract', 'tags')
+    serializer_class = ContractAssignmentSerializer
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/filtersets.py` & `netbox_contract-2.1.0/src/netbox_contract/filtersets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from django.db.models import Q
 from netbox.filtersets import NetBoxModelFilterSet
 
-from .models import Contract, ContractAssignement, Invoice, ServiceProvider
+from .models import Contract, ContractAssignment, Invoice, ServiceProvider
 
 
 class ContractFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = Contract
         fields = ('id', 'internal_partie', 'status', 'parent')
 
     def search(self, queryset, name, value):
         return queryset.filter(
             Q(name__icontains=value)
             | Q(external_reference__icontains=value)
-            | Q(comments__icontains=value)
+            | Q(comments__icontains=value),
+            Q(status__iexact='Active')
         )
 
 
 class InvoiceFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = Invoice
         fields = ('id', 'contracts')
 
     def search(self, queryset, name, value):
         return queryset.filter(
-            Q(number__icontains=value) | Q(contracts__name__icontains=value)
+            Q(number__icontains=value) 
+            | Q(contracts__name__icontains=value)
         )
 
 
 class ServiceProviderFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = ServiceProvider
         fields = ('id', 'name')
 
     def search(self, queryset, name, value):
         return queryset.filter(name__icontains=value)
 
 
-class ContractAssignementFilterSet(NetBoxModelFilterSet):
+class ContractAssignmentFilterSet(NetBoxModelFilterSet):
     class Meta:
-        model = ContractAssignement
+        model = ContractAssignment
         fields = ('id', 'contract')
 
     def search(self, queryset, name, value):
         return queryset.filter(Q(contract__name__icontains=value))
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/forms.py` & `netbox_contract-2.1.0/src/netbox_contract/forms.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     SlugField,
 )
 from utilities.forms.widgets import DatePicker, HTMXSelect
 
 from .constants import SERVICE_PROVIDER_MODELS
 from .models import (
     Contract,
-    ContractAssignement,
+    ContractAssignment,
     InternalEntityChoices,
     Invoice,
     ServiceProvider,
     StatusChoices,
 )
 
 plugin_settings = settings.PLUGINS_CONFIG['netbox_contract']
@@ -51,17 +51,17 @@
 
     external_partie_object_type = ContentTypeChoiceField(
         queryset=ContentType.objects.all(),
         limit_choices_to=SERVICE_PROVIDER_MODELS,
         widget=HTMXSelect(),
     )
     external_partie_object = forms.ModelChoiceField(queryset=None)
-    tenant = DynamicModelChoiceField(queryset=Tenant.objects.all())
+    tenant = DynamicModelChoiceField(queryset=Tenant.objects.all(), required=False)
     parent = DynamicModelChoiceField(queryset=Contract.objects.all(), required=False)
-    accounting_dimensions = Dimensions()
+    accounting_dimensions = Dimensions(required=False)
 
     def __init__(self, *args, **kwargs):
         initial = kwargs.get('initial', None)
         super().__init__(*args, **kwargs)
 
         # Initialize the external party object gfk
         if initial and 'external_partie_object_type' in initial:
@@ -99,14 +99,23 @@
             self.fields['external_partie_object'].initial = None
 
         # initialize accounting dimentsions widget
         # self.fields[
         #         'accounting_dimensions'
         #     ].widget.attrs['placeholder'] = '{"key": "value"}'
 
+        # Initialise fields settings
+        mandatory_fields = plugin_settings.get('mandatory_contract_fields')
+        for field in mandatory_fields:
+            self.fields[field].required = True
+        hidden_fields = plugin_settings.get('hidden_contract_fields')
+        for field in hidden_fields:
+            if not self.fields[field].required:
+                self.fields[field].widget = forms.HiddenInput()
+
     class Meta:
         model = Contract
         fields = (
             'name',
             'external_partie_object_type',
             'external_partie_object',
             'external_reference',
@@ -134,14 +143,27 @@
         }
 
 
 class InvoiceForm(NetBoxModelForm):
     contracts = DynamicModelMultipleChoiceField(
         queryset=Contract.objects.all(), required=False
     )
+    accounting_dimensions = Dimensions(required=False)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Initialise fields settings
+        mandatory_fields = plugin_settings.get('mandatory_invoice_fields')
+        for field in mandatory_fields:
+            self.fields[field].required = True
+        hidden_fields = plugin_settings.get('hidden_invoice_fields')
+        for field in hidden_fields:
+            if not self.fields[field].required:
+                self.fields[field].widget = forms.HiddenInput()
 
     class Meta:
         model = Invoice
         fields = (
             'number',
             'date',
             'contracts',
@@ -310,39 +332,39 @@
 class ServiceProviderBulkEditForm(NetBoxModelBulkEditForm):
     name = forms.CharField(max_length=100, required=True)
     comments = CommentField()
     nullable_fields = ('comments',)
     model = ServiceProvider
 
 
-# ContractAssignement
+# ContractAssignment
 
 
-class ContractAssignementForm(NetBoxModelForm):
+class ContractAssignmentForm(NetBoxModelForm):
     contract = DynamicModelChoiceField(queryset=Contract.objects.all())
 
     class Meta:
-        model = ContractAssignement
+        model = ContractAssignment
         fields = ['content_type', 'object_id', 'contract', 'tags']
         widgets = {
             'content_type': forms.HiddenInput(),
             'object_id': forms.HiddenInput(),
         }
 
 
-class ContractAssignementFilterSetForm(NetBoxModelFilterSetForm):
-    model = ContractAssignement
+class ContractAssignmentFilterSetForm(NetBoxModelFilterSetForm):
+    model = ContractAssignment
     contract = DynamicModelChoiceField(queryset=Contract.objects.all())
 
 
-class ContractAssignementImportForm(NetBoxModelImportForm):
+class ContractAssignmentImportForm(NetBoxModelImportForm):
     content_type = CSVContentTypeField(
         queryset=ContentType.objects.all(),
         help_text='Content Type in the form <app>.<model>',
     )
     contract = CSVModelChoiceField(
         queryset=Contract.objects.all(), help_text='Contract id'
     )
 
     class Meta:
-        model = ContractAssignement
+        model = ContractAssignment
         fields = ['content_type', 'object_id', 'contract', 'tags']
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0001_initial.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0006_alter_contract_circuit.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0006_alter_contract_circuit.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0011_auto_20230122_2112.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0011_auto_20230122_2112.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0015_contractassignement.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0015_contractassignement.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0016_contract_parent.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0016_contract_parent.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0018_contract_external_partie_object_id_and_more.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0018_contract_external_partie_object_id_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0019_auto_20230924_1813.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0019_auto_20230924_1813.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0020_alter_contract_external_partie.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0020_alter_contract_external_partie.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0021_alter_contract_external_partie.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0021_alter_contract_external_partie.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/migrations/0022_alter_contract_internal_partie_alter_contract_parent.py` & `netbox_contract-2.1.0/src/netbox_contract/migrations/0022_alter_contract_internal_partie_alter_contract_parent.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.9/src/netbox_contract/models.py` & `netbox_contract-2.1.0/src/netbox_contract/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from circuits.models import Circuit
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.urls import reverse
 from netbox.models import NetBoxModel
+from netbox.models.features import ContactsMixin
 from utilities.choices import ChoiceSet
 
 
 class StatusChoices(ChoiceSet):
     key = 'Contract.status'
 
     STATUS_ACTIVE = 'Active'
@@ -36,15 +36,15 @@
     CHOICES = [
         (CURRENCY_USD, 'USD'),
         ('eur', 'EUR'),
         ('chf', 'CHF'),
     ]
 
 
-class ServiceProvider(NetBoxModel):
+class ServiceProvider(ContactsMixin, NetBoxModel):
     name = models.CharField(max_length=100)
     slug = models.SlugField(max_length=100, unique=True)
     contacts = GenericRelation(to='tenancy.ContactAssignment')
     portal_url = models.URLField(blank=True, verbose_name='Portal URL')
     comments = models.TextField(blank=True)
 
     class Meta:
@@ -53,42 +53,35 @@
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_contract:serviceprovider', args=[self.pk])
 
 
-class ContractAssignement(NetBoxModel):
+class ContractAssignment(NetBoxModel):
     content_type = models.ForeignKey(to=ContentType, on_delete=models.CASCADE)
     object_id = models.PositiveBigIntegerField()
     content_object = GenericForeignKey(ct_field='content_type', fk_field='object_id')
     contract = models.ForeignKey(
-        to='Contract', on_delete=models.PROTECT, related_name='assignments'
+        to='Contract', on_delete=models.CASCADE, related_name='assignments'
     )
     clone_fields = ('content_type', 'object_id', 'contract')
 
     class Meta:
         ordering = ('contract',)
         indexes = [
             models.Index(fields=['content_type', 'object_id']),
         ]
 
     def get_absolute_url(self):
-        return reverse('plugins:netbox_contract:contractassignement', args=[self.pk])
+        return reverse('plugins:netbox_contract:contractassignment', args=[self.pk])
 
 
 class Contract(NetBoxModel):
     name = models.CharField(max_length=100)
-    external_partie = models.ForeignKey(
-        to=ServiceProvider,
-        on_delete=models.CASCADE,
-        related_name='contracts',
-        blank=True,
-        null=True,
-    )
 
     external_partie_object_type = models.ForeignKey(
         to=ContentType, on_delete=models.CASCADE, blank=True, null=True
     )
     external_partie_object_id = models.PositiveBigIntegerField(blank=True, null=True)
     external_partie_object = GenericForeignKey(
         ct_field='external_partie_object_type', fk_field='external_partie_object_id'
@@ -126,15 +119,14 @@
     )
     nrc = models.DecimalField(
         verbose_name='None recuring cost', default=0, max_digits=10, decimal_places=2
     )
     invoice_frequency = models.IntegerField(
         help_text='The frequency of invoices in month', default=1
     )
-    circuit = models.ManyToManyField(Circuit, related_name='contracts', blank=True)
     documents = models.URLField(blank=True)
     comments = models.TextField(blank=True)
     parent = models.ForeignKey(
         'self', on_delete=models.CASCADE, related_name='childs', null=True, blank=True
     )
 
     def get_absolute_url(self):
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/navigation.py` & `netbox_contract-2.1.0/src/netbox_contract/navigation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 from django.conf import settings
-from extras.plugins import PluginMenu, PluginMenuButton, PluginMenuItem
-from utilities.choices import ButtonColorChoices
+from netbox.plugins import PluginMenu, PluginMenuButton, PluginMenuItem
 
 plugin_settings = settings.PLUGINS_CONFIG['netbox_contract']
 
 contract_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:contract_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
-        color=ButtonColorChoices.GREEN,
         permissions=['netbox_contract.add_contract'],
     )
 ]
 
 invoice_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:invoice_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
-        color=ButtonColorChoices.GREEN,
         permissions=['netbox_contract.add_invoice'],
     )
 ]
 
 serviceprovider_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:serviceprovider_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
-        color=ButtonColorChoices.GREEN,
         permissions=['netbox_contract.add_serviceprovider'],
     )
 ]
 
 contract_menu_item = PluginMenuItem(
     link='plugins:netbox_contract:contract_list',
     link_text='Contracts',
@@ -51,17 +47,17 @@
 service_provider_menu_item = PluginMenuItem(
     link='plugins:netbox_contract:serviceprovider_list',
     link_text='Service Providers',
     buttons=serviceprovider_buttons,
     permissions=['netbox_contract.view_serviceprovider'],
 )
 contract_assignemnt_menu_item = PluginMenuItem(
-    link='plugins:netbox_contract:contractassignement_list',
-    link_text='Contract assignements',
-    permissions=['netbox_contract.view_contractassignement'],
+    link='plugins:netbox_contract:contractassignment_list',
+    link_text='Contract assignments',
+    permissions=['netbox_contract.view_contractassignment'],
 )
 
 items = (
     contract_menu_item,
     invoices_menu_item,
     service_provider_menu_item,
     contract_assignemnt_menu_item,
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/search.py` & `netbox_contract-2.1.0/src/netbox_contract/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from netbox.search import SearchIndex, register_search
+from netbox.search import SearchIndex
 
 from .models import Contract, Invoice, ServiceProvider
 
 
-@register_search
 class ServiceProviderIndex(SearchIndex):
     model = ServiceProvider
     fields = (
         ('name', 100),
         ('comments', 5000),
     )
 
 
-@register_search
 class ContractIndex(SearchIndex):
     model = Contract
     fields = (
         ('name', 100),
         ('comments', 5000),
     )
 
 
-@register_search
 class InvoiceIndex(SearchIndex):
     model = Invoice
     fields = (
         ('number', 100),
         ('comments', 5000),
     )
+
+indexes = [ServiceProviderIndex,ContractIndex,InvoiceIndex]
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/tables.py` & `netbox_contract-2.1.0/src/netbox_contract/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import django_tables2 as tables
 from netbox.tables import NetBoxTable, columns
 
-from .models import Contract, ContractAssignement, Invoice, ServiceProvider
+from .models import Contract, ContractAssignment, Invoice, ServiceProvider
 
 
-class ContractAssignementListTable(NetBoxTable):
+class ContractAssignmentListTable(NetBoxTable):
     content_type = columns.ContentTypeColumn(verbose_name='Object Type')
     content_object = tables.Column(linkify=True, orderable=False)
     contract = tables.Column(linkify=True)
     actions = columns.ActionsColumn(actions=('edit', 'delete'))
     contract__external_partie_object = tables.Column(linkify=True)
 
     class Meta(NetBoxTable.Meta):
-        model = ContractAssignement
+        model = ContractAssignment
         fields = (
             'pk',
             'content_type',
             'content_object',
             'contract',
             'contract__external_partie_object_type',
             'contract__external_partie_object',
@@ -28,21 +28,21 @@
             'content_object',
             'contract',
             'contract__external_partie_object_type',
             'contract__external_partie_object',
         )
 
 
-class ContractAssignementObjectTable(NetBoxTable):
+class ContractAssignmentObjectTable(NetBoxTable):
     contract = tables.Column(linkify=True)
     actions = columns.ActionsColumn(actions=('edit', 'delete'))
     contract__external_partie_object = tables.Column(linkify=True)
 
     class Meta(NetBoxTable.Meta):
-        model = ContractAssignement
+        model = ContractAssignment
         fields = (
             'pk',
             'contract',
             'contract__external_partie_object_type',
             'contract__external_partie_object',
             'contract__status',
             'contract__start_date',
@@ -60,22 +60,22 @@
             'contract__start_date',
             'contract__end_date',
             'contract__mrc',
             'contract__nrc',
         )
 
 
-class ContractAssignementContractTable(NetBoxTable):
+class ContractAssignmentContractTable(NetBoxTable):
     content_type = columns.ContentTypeColumn(verbose_name='Object Type')
     content_object = tables.Column(linkify=True, verbose_name='Object', orderable=False)
     content_object__status = tables.Column(verbose_name='Status')
     actions = columns.ActionsColumn(actions=('edit', 'delete'))
 
     class Meta(NetBoxTable.Meta):
-        model = ContractAssignement
+        model = ContractAssignment
         fields = (
             'pk',
             'content_type',
             'content_object',
             'content_object__status',
             'actions',
         )
@@ -85,16 +85,17 @@
             'content_object',
             'content_object__status',
         )
 
 
 class ContractListTable(NetBoxTable):
     name = tables.Column(linkify=True)
-    external_partie_object = tables.Column(linkify=True)
+    external_partie_object = tables.Column(verbose_name='External partie', linkify=True)
     parent = tables.Column(linkify=True)
+    yrc = tables.Column(verbose_name='Yerly recuring costs')
 
     class Meta(NetBoxTable.Meta):
         model = Contract
         fields = (
             'pk',
             'id',
             'name',
@@ -107,14 +108,15 @@
             'start_date',
             'end_date',
             'initial_term',
             'renewal_term',
             'currency',
             'accounting_dimensions',
             'mrc',
+            'yrc',
             'nrc',
             'invoice_frequency',
             'documents',
             'comments',
             'parent',
             'actions',
         )
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/template_content.py` & `netbox_contract-2.1.0/src/netbox_contract/template_content.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,104 +1,96 @@
 from circuits.models import Circuit
 from dcim.models import Device, Site
 from django.contrib.contenttypes.models import ContentType
-from extras.plugins import PluginTemplateExtension
+from netbox.plugins import PluginTemplateExtension
 from virtualization.models import VirtualMachine
 
 from . import tables
-from .models import ContractAssignement
+from .models import ContractAssignment
 
 
-class CircuitContractAssignements(PluginTemplateExtension):
+class CircuitContractAssignments(PluginTemplateExtension):
     model = 'circuits.circuit'
 
     def full_width_page(self):
         circuit = self.context['object']
         circuit_type = ContentType.objects.get_for_model(Circuit)
-        contract_assignements = ContractAssignement.objects.filter(
+        contract_assignments = ContractAssignment.objects.filter(
             content_type__pk=circuit_type.id, object_id=circuit.id
         )
-        assignements_table = tables.ContractAssignementObjectTable(
-            contract_assignements
-        )
-        assignements_table.configure(self.context['request'])
+        assignments_table = tables.ContractAssignmentObjectTable(contract_assignments)
+        assignments_table.configure(self.context['request'])
 
         return self.render(
-            'contract_assignements_bottom.html',
+            'contract_assignments_bottom.html',
             extra_context={
-                'assignements_table': assignements_table,
+                'assignments_table': assignments_table,
             },
         )
 
 
-class DeviceContractAssignements(PluginTemplateExtension):
+class DeviceContractAssignments(PluginTemplateExtension):
     model = 'dcim.device'
 
     def full_width_page(self):
         device = self.context['object']
         device_type = ContentType.objects.get_for_model(Device)
-        contract_assignements = ContractAssignement.objects.filter(
+        contract_assignments = ContractAssignment.objects.filter(
             content_type__pk=device_type.id, object_id=device.id
         )
-        assignements_table = tables.ContractAssignementObjectTable(
-            contract_assignements
-        )
-        assignements_table.configure(self.context['request'])
+        assignments_table = tables.ContractAssignmentObjectTable(contract_assignments)
+        assignments_table.configure(self.context['request'])
 
         return self.render(
-            'contract_assignements_bottom.html',
+            'contract_assignments_bottom.html',
             extra_context={
-                'assignements_table': assignements_table,
+                'assignments_table': assignments_table,
             },
         )
 
 
-class VMContractAssignements(PluginTemplateExtension):
+class VMContractAssignments(PluginTemplateExtension):
     model = 'virtualization.virtualmachine'
 
     def full_width_page(self):
         vm = self.context['object']
         vm_type = ContentType.objects.get_for_model(VirtualMachine)
-        contract_assignements = ContractAssignement.objects.filter(
+        contract_assignments = ContractAssignment.objects.filter(
             content_type__pk=vm_type.id, object_id=vm.id
         )
-        assignements_table = tables.ContractAssignementObjectTable(
-            contract_assignements
-        )
-        assignements_table.configure(self.context['request'])
+        assignments_table = tables.ContractAssignmentObjectTable(contract_assignments)
+        assignments_table.configure(self.context['request'])
 
         return self.render(
-            'contract_assignements_bottom.html',
+            'contract_assignments_bottom.html',
             extra_context={
-                'assignements_table': assignements_table,
+                'assignments_table': assignments_table,
             },
         )
 
 
-class SiteContractAssignements(PluginTemplateExtension):
+class SiteContractAssignments(PluginTemplateExtension):
     model = 'dcim.site'
 
     def full_width_page(self):
         site = self.context['object']
         site_type = ContentType.objects.get_for_model(Site)
-        contract_assignements = ContractAssignement.objects.filter(
+        contract_assignments = ContractAssignment.objects.filter(
             content_type__pk=site_type.id, object_id=site.id
         )
-        assignements_table = tables.ContractAssignementObjectTable(
-            contract_assignements
-        )
-        assignements_table.configure(self.context['request'])
+        assignments_table = tables.ContractAssignmentObjectTable(contract_assignments)
+        assignments_table.configure(self.context['request'])
 
         return self.render(
-            'contract_assignements_bottom.html',
+            'contract_assignments_bottom.html',
             extra_context={
-                'assignements_table': assignements_table,
+                'assignments_table': assignments_table,
             },
         )
 
 
 template_extensions = [
-    CircuitContractAssignements,
-    DeviceContractAssignements,
-    VMContractAssignements,
-    SiteContractAssignements,
+    CircuitContractAssignments,
+    DeviceContractAssignments,
+    VMContractAssignments,
+    SiteContractAssignments,
 ]
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/templates/contract_assignements_bottom.html` & `netbox_contract-2.1.0/src/netbox_contract/templates/contract_assignments_bottom.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 {% load render_table from django_tables2 %}
 {% if perms.netbox_contract.view_contract %}
 <div class="row">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Contracts Assignements</h5>
-        {% if assignements_table %}
-        <div class="card-body table-responsive">
-          {% render_table assignements_table %}
-        </div>
+        <h5 class="card-header">Contracts Assignments</h5>
+        {% if assignments_table %}
+          {% render_table assignments_table %}
         {% endif %}
-        {% if perms.netbox_contract.add_contractassignement %}
+        {% if perms.netbox_contract.add_contractassignment %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_contract:contractassignement_add' %}?content_type={{ object|content_type_id }}&object_id={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_contract:contractassignment_add' %}?content_type={{ object|content_type_id }}&object_id={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
               <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
-              Add assignement
+              Add assignment
           </a>
         </div>
         {% endif %}
       </div>
     </div>
 </div>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
 {% load render_table from django_tables2 %} {% if
 perms.netbox_contract.view_contract %}
-**** CCoonnttrraaccttss AAssssiiggnneemmeennttss ****
-{% if assignements_table %}
-{% render_table assignements_table %}
-{% endif %} {% if perms.netbox_contract.add_contractassignement %}
-_A_d_d_ _a_s_s_i_g_n_e_m_e_n_t
+**** CCoonnttrraaccttss AAssssiiggnnmmeennttss ****
+{% if assignments_table %} {% render_table assignments_table %} {% endif %} {%
+if perms.netbox_contract.add_contractassignment %}
+_A_d_d_ _a_s_s_i_g_n_m_e_n_t
 {% endif %}
 {% endif %}
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/contract.html` & `netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/contract.html`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,14 @@
   <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_contract:contract_list' %}?external_partie={{ object.external_partie.pk }}">{{ object.external_partie }}</a></li>
 {% endblock %}
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Contract</h5>
-        <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
                 <tr>
               <th scope="row">External partie type</th>
@@ -34,109 +33,120 @@
               <th scope="row">External reference</th>
               <td>{{ object.external_reference }}</td>
             </tr>
             <tr>
               <th scope="row">Internal partie</th>
               <td>{{ object.internal_partie }}</td>
             </tr>
+            {% if not 'tenant' in hidden_fields %}
             <tr>
               <th scope="row">Tenant</th>
               <td>{{ object.tenant }}</td>
             </tr>
+            {% endif %}
+            {% if not 'start_date' in hidden_fields %}
             <tr>
               <th scope="row">Start date</th>
               <td>{{ object.start_date }}</td>
             </tr>
+            {% endif %}
+            {% if not 'end_date' in hidden_fields %}
             <tr>
               <th scope="row">End date</th>
               <td>{{ object.end_date }}</td>
             </tr>
+            {% endif %}
+            {% if not 'initial_term' in hidden_fields %}
             <tr>
               <th scope="row">Initial term</th>
               <td>{{ object.initial_term }}</td>
             </tr>
+            {% endif %}
+            {% if not 'renewal_term' in hidden_fields %}
             <tr>
               <th scope="row">Renewal term</th>
               <td>{{ object.renewal_term }}</td>
             </tr>
+            {% endif %}
             <tr>
               <th scope="row">Currency</th>
               <td>{{ object.currency }}</td>
             </tr>
+            {% if not 'accounting_dimensions' in hidden_fields %}
             <tr>
               <th scope="row">Accounting dimensions</th>
               <td>{{ object.accounting_dimensions }}</td>
             </tr>
+            {% endif %}
             <tr>
               <th scope="row">Monthly recuring costs</th>
               <td>{{ object.mrc }}</td>
             </tr>
             <tr>
+              <th scope="row">Yearly recuring costs</th>
+              <td>{{ object.yrc }}</td>
+            </tr>
+            <tr>
               <th scope="row">Non recuring costs</th>
               <td>{{ object.nrc }}</td>
             </tr>
             <tr>
               <th scope="row">Invoice frequency</th>
               <td>{{ object.invoice_frequency }}</td>
             </tr>
+            {% if not 'parent' in hidden_fields %}
             <tr>
               <th scope="row">Parent</th>
               <td>
                 <a href="{{ object.parent.get_absolute_url }}">{{ object.parent.name }}</a>
               </td>
             </tr>
+            {% endif %}
             {% if object.documents %}
             <tr>
               <th scope="row">Documents</th>
                 <td>
                   <a href="{{ object.documents }}" target="_blank">Documents</a>
                 </td>
             </tr>
             {% endif %}
           </table>
-        </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Assignements</h5>
-        <div class="card-body table-responsive">
-          {% render_table assignements_table %}
-        </div>
+        <h5 class="card-header">Assignments</h5>
+          {% render_table assignments_table %}
       </div>
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">childs</h5>
-        <div class="card-body table-responsive">
           {% render_table childs_table %}
-        </div>
       </div>
     </div>
   </div>
   {% if perms.netbox_contract.view_invoice %}
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Invoices</h5>
-        <div class="card-body table-responsive">
           {% render_table invoices_table %}
-        </div>
         {% if perms.netbox_contract.add_invoice %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_contract:invoice_add' %}?contracts={{ object.pk }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_contract:invoice_add' %}?contracts={{ object.pk }}" class="btn btn-primary">
               <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
               Add an invoice
           </a>
         </div>
         {% endif %}
       </div>
     </div>
```

#### html2text {}

```diff
@@ -13,24 +13,24 @@
 SSttaarrtt ddaattee             {{ object.start_date }}
 EEnndd ddaattee               {{ object.end_date }}
 IInniittiiaall tteerrmm           {{ object.initial_term }}
 RReenneewwaall tteerrmm           {{ object.renewal_term }}
 CCuurrrreennccyy               {{ object.currency }}
 AAccccoouunnttiinngg ddiimmeennssiioonnss  {{ object.accounting_dimensions }}
 MMoonntthhllyy rreeccuurriinngg ccoossttss {{ object.mrc }}
+YYeeaarrllyy rreeccuurriinngg ccoossttss  {{ object.yrc }}
 NNoonn rreeccuurriinngg ccoossttss     {{ object.nrc }}
 IInnvvooiiccee ffrreeqquueennccyy      {{ object.invoice_frequency }}
 PPaarreenntt                 _{_{_ _o_b_j_e_c_t_._p_a_r_e_n_t_._n_a_m_e_ _}_}
 DDooccuummeennttss              _D_o_c_u_m_e_n_t_s
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
-**** AAssssiiggnneemmeennttss ****
-{% render_table assignements_table %}
+**** AAssssiiggnnmmeennttss ****
+{% render_table assignments_table %}
 **** cchhiillddss ****
 {% render_table childs_table %}
 {% if perms.netbox_contract.view_invoice %}
 **** IInnvvooiicceess ****
-{% render_table invoices_table %}
-{% if perms.netbox_contract.add_invoice %}
+{% render_table invoices_table %} {% if perms.netbox_contract.add_invoice %}
 _A_d_d_ _a_n_ _i_n_v_o_i_c_e
 {% endif %}
 {% endif %} {% plugin_right_page object %} {% endblock content %}
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/contract_assignement.html` & `netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/contractassignment.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 {% extends 'generic/object.html' %}
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
-        <h5 class="card-header">Contract assignement</h5>
-        <div class="card-body">
+        <h5 class="card-header">Contract assignment</h5>
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Model</th>
               <td>{{ object.content_type }}</td>
             </tr>
             <tr>
               <th scope="row">Object</th>
-              <td>{{ object.object_id }}</td>
+              <td><a href="{{ object.content_object.get_absolute_url }}">{{ object.content_object.name }}</a></td>
             </tr>
             <tr>
               <th scope="row">Contract</th>
-              <td>{{ object.contract }}</td>
+              <td><a href="{{ object.contract.get_absolute_url }}">{{ object.contract.name }}</a></td>
             </tr>
-            {% endif %}
           </table>
-        </div>
       </div>
       {% include 'inc/panels/tags.html' %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% extends 'generic/object.html' %} {% block content %}
-**** CCoonnttrraacctt aassssiiggnneemmeenntt ****
+**** CCoonnttrraacctt aassssiiggnnmmeenntt ****
 MMooddeell    {{ object.content_type }}
-OObbjjeecctt   {{ object.object_id }}
-CCoonnttrraacctt {{ object.contract }}
+OObbjjeecctt   _{_{_ _o_b_j_e_c_t_._c_o_n_t_e_n_t___o_b_j_e_c_t_._n_a_m_e_ _}_}
+CCoonnttrraacctt _{_{_ _o_b_j_e_c_t_._c_o_n_t_r_a_c_t_._n_a_m_e_ _}_}
 {% include 'inc/panels/tags.html' %}
 {% endblock content %}
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/invoice.html` & `netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/invoice.html`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
   </li>
 {% endblock %}
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Invoices</h5>
-        <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Number</th>
               <td>{{ object.number }}</td>
             </tr>
             <tr>
               <th scope="row">Date</th>
@@ -32,40 +31,39 @@
               <th scope="row">Period end</th>
               <td>{{ object.period_end }}</td>
             </tr>
             <tr>
               <th scope="row">Currency</th>
               <td>{{ object.currency }}</td>
             </tr>
+            {% if not 'accounting_dimensions' in hidden_fields %}
             <tr>
               <th scope="row">Accounting dimensions</th>
               <td>{{ object.accounting_dimensions }}</td>
             </tr>
+            {% endif %}
             <tr>
               <th scope="row">Amount</th>
               <td>{{ object.amount }}</td>
             </tr>
             {% if object.documents %}
             <tr>
               <th scope="row">Documents</th>
                 <td>
                   <a href="{{ object.documents }}" target="_blank">Documents</a>
                 </td>
             </tr>
             {% endif %}
           </table>
-        </div>
       </div>
       <div class="row">
         <div class="col col-md-12">
           <div class="card">
             <h5 class="card-header">Contracts</h5>
-            <div class="card-body table-responsive">
               {% render_table contracts_table %}
-            </div>
           </div>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
     </div>
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/serviceprovider.html` & `netbox_contract-2.1.0/src/netbox_contract/templates/netbox_contract/serviceprovider.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 {% extends 'generic/object.html' %}
+{% load static %}
+{% load helpers %}
+{% load i18n %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Service Provider</h5>
-        <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
               <th scope="row">slug</th>
@@ -22,16 +24,14 @@
                     <a href="{{ object.portal_url }}">{{ object.portal_url }}</a>
                 {% else %}
                     {{ ''|placeholder }}
                 {% endif %}
             </td>
             </tr>
           </table>
-        </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/tags.html' %}
-      {% include 'contact_assignements_bottom.html' %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends 'generic/object.html' %} {% block content %}
+{% extends 'generic/object.html' %} {% load static %} {% load helpers %} {%
+load i18n %} {% block content %}
 **** SSeerrvviiccee PPrroovviiddeerr ****
 NNaammee       {{ object.name }}
 sslluugg       {{ object.slug }}
 ppoorrttaall__uurrll {% if object.portal_url %} _{_{_ _o_b_j_e_c_t_._p_o_r_t_a_l___u_r_l_ _}_} {% else %} {
            { ''|placeholder }} {% endif %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
-comments.html' %} {% include 'inc/panels/tags.html' %} {% include
-'contact_assignements_bottom.html' %}
+comments.html' %} {% include 'inc/panels/tags.html' %}
 {% endblock content %}
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/urls.py` & `netbox_contract-2.1.0/src/netbox_contract/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from django.urls import path
+from django.urls import include, path
 from netbox.views.generic import ObjectChangeLogView
+from utilities.urls import get_model_urls
 
 from . import models, views
 
 urlpatterns = (
     # Service Providers
     path(
         'serviceproviders/',
@@ -47,14 +48,19 @@
     ),
     path(
         'serviceproviders/<int:pk>/changelog/',
         ObjectChangeLogView.as_view(),
         name='serviceprovider_changelog',
         kwargs={'model': models.ServiceProvider},
     ),
+    path(
+        'serviceproviders/<int:pk>/contacts/',
+        views.ServiceProviderContactsView.as_view(),
+        name='serviceprovider_contacts',
+    ),
     # Contracts
     path('contracts/', views.ContractListView.as_view(), name='contract_list'),
     path('contracts/add/', views.ContractEditView.as_view(), name='contract_add'),
     path(
         'contracts/import/',
         views.ContractBulkImportView.as_view(),
         name='contract_import',
@@ -65,15 +71,19 @@
         name='contract_bulk_edit',
     ),
     path(
         'contracts/delete/',
         views.ContractBulkDeleteView.as_view(),
         name='contract_bulk_delete',
     ),
-    path('contracts/<int:pk>/', views.ContractView.as_view(), name='contract'),
+    path(
+        'contracts/<int:pk>/',
+        include(get_model_urls('netbox_contract', 'contract')),
+        name='contract',
+    ),
     path(
         'contracts/<int:pk>/edit/',
         views.ContractEditView.as_view(),
         name='contract_edit',
     ),
     path(
         'contracts/<int:pk>/delete/',
@@ -96,60 +106,64 @@
         'invoices/edit/', views.InvoiceBulkEditView.as_view(), name='invoice_bulk_edit'
     ),
     path(
         'invoices/delete/',
         views.InvoiceBulkDeleteView.as_view(),
         name='invoice_bulk_delete',
     ),
-    path('invoices/<int:pk>/', views.InvoiceView.as_view(), name='invoice'),
+    path(
+        'invoices/<int:pk>/',
+        include(get_model_urls('netbox_contract', 'invoice')),
+        name='invoice',
+    ),
     path(
         'invoices/<int:pk>/edit/', views.InvoiceEditView.as_view(), name='invoice_edit'
     ),
     path(
         'invoices/<int:pk>/delete/',
         views.InvoiceDeleteView.as_view(),
         name='invoice_delete',
     ),
     path(
         'invoices/<int:pk>/changelog/',
         ObjectChangeLogView.as_view(),
         name='invoice_changelog',
         kwargs={'model': models.Invoice},
     ),
-    # Contract assignements
+    # Contract assignments
     path(
-        'assignements/',
-        views.ContractAssignementListView.as_view(),
-        name='contractassignement_list',
+        'assignments/',
+        views.ContractAssignmentListView.as_view(),
+        name='contractassignment_list',
     ),
     path(
-        'assignements/add/',
-        views.ContractAssignementEditView.as_view(),
-        name='contractassignement_add',
+        'assignments/add/',
+        views.ContractAssignmentEditView.as_view(),
+        name='contractassignment_add',
     ),
     path(
-        'assignements/import/',
-        views.ContractAssignementBulkImportView.as_view(),
-        name='contractassignement_import',
+        'assignments/import/',
+        views.ContractAssignmentBulkImportView.as_view(),
+        name='contractassignment_import',
     ),
     path(
-        'assignements/<int:pk>/',
-        views.ContractAssignementView.as_view(),
-        name='contractassignement',
+        'assignments/<int:pk>/',
+        views.ContractAssignmentView.as_view(),
+        name='contractassignment',
     ),
     path(
-        'assignements/<int:pk>/edit/',
-        views.ContractAssignementEditView.as_view(),
-        name='contractassignement_edit',
+        'assignments/<int:pk>/edit/',
+        views.ContractAssignmentEditView.as_view(),
+        name='contractassignment_edit',
     ),
     path(
-        'assignements/<int:pk>/delete/',
-        views.ContractAssignementDeleteView.as_view(),
-        name='contractassignement_delete',
+        'assignments/<int:pk>/delete/',
+        views.ContractAssignmentDeleteView.as_view(),
+        name='contractassignment_delete',
     ),
     path(
-        'assignements/<int:pk>/changelog/',
+        'assignments/<int:pk>/changelog/',
         ObjectChangeLogView.as_view(),
-        name='contractassignement_changelog',
-        kwargs={'model': models.ContractAssignement},
+        name='contractassignment_changelog',
+        kwargs={'model': models.ContractAssignment},
     ),
 )
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract/views.py` & `netbox_contract-2.1.0/src/netbox_contract/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 from datetime import date, timedelta
 
-from circuits.models import Circuit
 from dateutil.relativedelta import relativedelta
+from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ObjectDoesNotExist
+from django.db.models import F
 from django.shortcuts import get_object_or_404, render
 from netbox.views import generic
 from netbox.views.generic.utils import get_prerequisite_model
+from tenancy.views import ObjectContactsView
 from utilities.forms import restrict_form_fields
-from utilities.utils import count_related, normalize_querydict
+from utilities.querydict import normalize_querydict
+from utilities.views import register_model_view
 
 from . import filtersets, forms, tables
-from .models import Contract, ContractAssignement, Invoice, ServiceProvider
+from .models import Contract, ContractAssignment, Invoice, ServiceProvider
+
+plugin_settings = settings.PLUGINS_CONFIG['netbox_contract']
 
 # ServiceProvider views
 
 
+@register_model_view(ServiceProvider, 'contacts')
+class ServiceProviderContactsView(ObjectContactsView):
+    queryset = ServiceProvider.objects.all()
+
+
 class ServiceProviderView(generic.ObjectView):
     queryset = ServiceProvider.objects.all()
 
 
 class ServiceProviderListView(generic.ObjectListView):
     queryset = ServiceProvider.objects.all()
     table = tables.ServiceProviderListTable
@@ -51,35 +61,37 @@
 
 class ServiceProviderBulkDeleteView(generic.BulkDeleteView):
     queryset = ServiceProvider.objects.annotate()
     filterset = filtersets.ServiceProviderFilterSet
     table = tables.ServiceProviderListTable
 
 
-# Contract assignement view
+# Contract assignment view
 
 
-class ContractAssignementView(generic.ObjectView):
-    queryset = ContractAssignement.objects.all()
+class ContractAssignmentView(generic.ObjectView):
+    queryset = ContractAssignment.objects.all()
 
 
-class ContractAssignementListView(generic.ObjectListView):
-    queryset = ContractAssignement.objects.all()
-    table = tables.ContractAssignementListTable
-    filterset = filtersets.ContractAssignementFilterSet
-    filterset_form = forms.ContractAssignementFilterSetForm
-    actions = [
-        'import',
-        'export',
-    ]
+class ContractAssignmentListView(generic.ObjectListView):
+    queryset = ContractAssignment.objects.all()
+    table = tables.ContractAssignmentListTable
+    filterset = filtersets.ContractAssignmentFilterSet
+    filterset_form = forms.ContractAssignmentFilterSetForm
+    actions = {
+        'import': {'add'},
+        'export': set(),
+        'bulk_edit': {'change'},
+        'bulk_delete': {'delete'},
+    }
 
 
-class ContractAssignementEditView(generic.ObjectEditView):
-    queryset = ContractAssignement.objects.all()
-    form = forms.ContractAssignementForm
+class ContractAssignmentEditView(generic.ObjectEditView):
+    queryset = ContractAssignment.objects.all()
+    form = forms.ContractAssignmentForm
 
     def alter_object(self, instance, request, args, kwargs):
         if not instance.pk and kwargs:
             # Assign the object based on URL kwargs
             content_type = get_object_or_404(
                 ContentType, pk=request.GET.get('content_type')
             )
@@ -91,49 +103,53 @@
     def get_extra_addanother_params(self, request):
         return {
             'content_type': request.GET.get('content_type'),
             'object_id': request.GET.get('object_id'),
         }
 
 
-class ContractAssignementDeleteView(generic.ObjectDeleteView):
-    queryset = ContractAssignement.objects.all()
+class ContractAssignmentDeleteView(generic.ObjectDeleteView):
+    queryset = ContractAssignment.objects.all()
 
 
-class ContractAssignementBulkImportView(generic.BulkImportView):
-    queryset = ContractAssignement.objects.all()
-    model_form = forms.ContractAssignementImportForm
-    table = tables.ContractAssignementListTable
+class ContractAssignmentBulkImportView(generic.BulkImportView):
+    queryset = ContractAssignment.objects.all()
+    model_form = forms.ContractAssignmentImportForm
+    table = tables.ContractAssignmentListTable
 
 
 # Contract views
 
 
+@register_model_view(Contract)
 class ContractView(generic.ObjectView):
-    queryset = Contract.objects.all()
+    queryset = Contract.objects.annotate(yrc=F('mrc') * 12)
 
     def get_extra_context(self, request, instance):
         invoices_table = tables.InvoiceListTable(instance.invoices.all())
         invoices_table.configure(request)
-        assignements_table = tables.ContractAssignementContractTable(
+        assignments_table = tables.ContractAssignmentContractTable(
             instance.assignments.all()
         )
-        assignements_table.configure(request)
+        assignments_table.configure(request)
         childs_table = tables.ContractListBottomTable(instance.childs.all())
         childs_table.configure(request)
 
+        hidden_fields = plugin_settings.get('hidden_contract_fields')
+
         return {
+            'hidden_fields': hidden_fields,
             'invoices_table': invoices_table,
-            'assignements_table': assignements_table,
+            'assignments_table': assignments_table,
             'childs_table': childs_table,
         }
 
 
 class ContractListView(generic.ObjectListView):
-    queryset = Contract.objects.all()
+    queryset = Contract.objects.annotate(yrc=F('mrc') * 12)
     table = tables.ContractListTable
     filterset = filtersets.ContractFilterSet
     filterset_form = forms.ContractFilterSetForm
 
 
 class ContractEditView(generic.ObjectEditView):
     queryset = Contract.objects.all()
@@ -183,32 +199,33 @@
     queryset = Contract.objects.all()
     filterset = filtersets.ContractFilterSet
     table = tables.ContractListTable
     form = forms.ContractBulkEditForm
 
 
 class ContractBulkDeleteView(generic.BulkDeleteView):
-    queryset = Contract.objects.annotate(
-        count_circuits=count_related(Circuit, 'contracts')
-    )
+    queryset = Contract.objects.all()
     filterset = filtersets.ContractFilterSet
     table = tables.ContractListTable
 
 
 # Invoice views
 
 
+@register_model_view(Invoice)
 class InvoiceView(generic.ObjectView):
     queryset = Invoice.objects.all()
 
     def get_extra_context(self, request, instance):
         contracts_table = tables.ContractListTable(instance.contracts.all())
         contracts_table.configure(request)
+        hidden_fields = plugin_settings.get('hidden_invoice_fields')
 
         return {
+            'hidden_fields': hidden_fields,
             'contracts_table': contracts_table,
         }
 
 
 class InvoiceListView(generic.ObjectListView):
     queryset = Invoice.objects.all()
     table = tables.InvoiceListTable
```

### Comparing `netbox-contract-2.0.9/src/netbox_contract.egg-info/SOURCES.txt` & `netbox_contract-2.1.0/src/netbox_contract.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,19 @@
 src/netbox_contract/migrations/0016_contract_parent.py
 src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
 src/netbox_contract/migrations/0018_contract_external_partie_object_id_and_more.py
 src/netbox_contract/migrations/0019_auto_20230924_1813.py
 src/netbox_contract/migrations/0020_alter_contract_external_partie.py
 src/netbox_contract/migrations/0021_alter_contract_external_partie.py
 src/netbox_contract/migrations/0022_alter_contract_internal_partie_alter_contract_parent.py
+src/netbox_contract/migrations/0023_rename_contractassignement_contractassignment_and_more.py
+src/netbox_contract/migrations/0024_remove_contract_external_partie.py
+src/netbox_contract/migrations/0025_remove_contract_circuit_and_more.py
+src/netbox_contract/migrations/0026_auto_20240421_1550.py
 src/netbox_contract/migrations/__init__.py
-src/netbox_contract/templates/contact_assignements_bottom.html
-src/netbox_contract/templates/contract_assignements_bottom.html
+src/netbox_contract/templates/contract_assignments_bottom.html
+src/netbox_contract/templates/contract_assignments_bottom_old.html
 src/netbox_contract/templates/contract_list_bottom.html
 src/netbox_contract/templates/netbox_contract/contract.html
-src/netbox_contract/templates/netbox_contract/contract_assignement.html
+src/netbox_contract/templates/netbox_contract/contractassignment.html
 src/netbox_contract/templates/netbox_contract/invoice.html
 src/netbox_contract/templates/netbox_contract/serviceprovider.html
```

