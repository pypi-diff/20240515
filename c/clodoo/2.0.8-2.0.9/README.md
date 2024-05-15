# Comparing `tmp/clodoo-2.0.8.tar.gz` & `tmp/clodoo-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clodoo-2.0.8.tar", last modified: Fri Nov 17 08:25:13 2023, max compression
+gzip compressed data, was "dist/clodoo-2.0.9.tar", last modified: Wed Feb  7 14:25:13 2024, max compression
```

## Comparing `clodoo-2.0.8.tar` & `clodoo-2.0.9.tar`

### file list

```diff
@@ -1,36 +1,196 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-11-17 08:25:13.000000 clodoo-2.0.8/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      164 2023-06-24 06:17:11.000000 clodoo-2.0.8/clodoo/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5932 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/update_coa.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4008 2022-12-09 05:08:44.000000 clodoo-2.0.8/clodoo/manage_odoo.man
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    50852 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/clodoocore.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21644 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/odoo_install_repository
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29879 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/transodoo.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    24391 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/clodoolib.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2774 2023-11-17 07:26:40.000000 clodoo-2.0.8/clodoo/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6803 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2023-05-14 13:22:41.000000 clodoo-2.0.8/clodoo/scripts/__init__.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)    24448 2023-04-02 18:39:37.000000 clodoo-2.0.8/clodoo/transodoo.xlsx
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    14545 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/manage_odoo
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4321 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/bck_filestore.sh
--rw-rw-r--   0 odoo      (1000) odoo      (1000)   233321 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/clodoo_main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20723 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/manage_db
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3084 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/check_one2many.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8613 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/export_db_model.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8766 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/moduli_da_installare.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      764 2023-08-05 11:36:47.000000 clodoo-2.0.8/clodoo/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    93689 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/migrate_odoo_db.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    34328 2023-11-16 07:27:22.000000 clodoo-2.0.8/clodoo/odoorc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-11-17 08:25:13.000000 clodoo-2.0.8/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2774 2023-11-16 17:01:44.000000 clodoo-2.0.8/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    11499 2023-11-17 08:25:13.000000 clodoo-2.0.8/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8239 2023-11-17 08:22:49.000000 clodoo-2.0.8/README.rst
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:50:55.000000 clodoo-2.0.8/clodoo.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       95 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      706 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      107 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo.egg-info/requires.txt
--rw-r--r--   0 odoo      (1000) odoo      (1000)    11499 2023-11-17 08:25:13.000000 clodoo-2.0.8/clodoo.egg-info/PKG-INFO
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      164 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/data/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       59 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/ir_config_parameter-03.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      327 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_bank-22.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       54 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/ir_config_parameter-13_10.0.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      144 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_company-new-12.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       73 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_group-new-12_6.1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      529 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/ir_rule-13_7.0.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      155 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/ir_mail_server-13.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1139 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_journal-15.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      419 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_invoice-61-2.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1045 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_partner_bank-92.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2647 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_journal-16.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       29 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_lang.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      238 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_invoice_line-61-3.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      519 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/payment-mode.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      137 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_user-main-11.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      805 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_partner-demo-52.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      803 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_group-main-11.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       26 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/sale_order-20.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      895 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_journal-main-90.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      250 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_invoice_line-61-1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    74184 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/product_product-demo-55.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      850 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/product_product-demo-55_6.1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    22510 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_partner-demo-53.xml
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      149 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_country-2.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       47 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/ir_config_parameter-13_8.0.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       80 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_company-main-12.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      126 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_fiscalyear-prior-31.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1103 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_user-new-12.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      138 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_fiscalyear-cur-31.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1219 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_group-demo-51.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2292 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_group-all-21.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      159 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/stock_location-18_8.0.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      234 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_invoice_line-61-2.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      895 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_journal-main-91.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3784 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_tax_code-20.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      186 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/sale_shop-19.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      146 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/stock_warehouse-18_7.0.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1705 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account-journal.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    41748 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_partner-30.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      424 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_user-demo-50.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      747 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/crm_lead-54.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      191 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/ir_sequence-16.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      198 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/sale_order-56.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      173 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/ir_sequence-15.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3680 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_partner-main-11.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       47 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/ir_config_parameter-13.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      436 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_invoice-61-3.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      411 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_move_line-62-1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    41750 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res-partners.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      614 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_user-new-12_6.1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      175 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_move-62-1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7543 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_partner-demo-53.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1700 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_period-cur-31.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6045 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_partner-company-90.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2306 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_journal-16_6.1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      120 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_group-new-12.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      698 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_partner-addr-53.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      159 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_user-main-11_6.1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       31 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/sale_config_settings.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      474 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_company-demo-52.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      316 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_invoice-61-1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       77 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_group-main-11_6.1.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      516 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/account_period-prior-31.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      118 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/stock_warehouse-18_8.0.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4746 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/res_group-all-14.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      133 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/sale_order-55.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      444 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/stock_location-18_7.0.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      532 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/data/sale_order_line-56.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5933 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/update_coa.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4008 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/manage_odoo.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9876 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/awsfw
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    50853 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/clodoocore.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21645 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/odoo_install_repository
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/tests/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23429 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/tests/clodoo_test_transodoo.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    32368 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/tests/__clodoo_test_01.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    23420 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/tests/test_odoorc.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       59 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/tests/res_users.csv
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6130 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/tests/__clodoo_test_odoo_skin.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1219 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/tests/conftest.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    50816 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/tests/clodoo_test_odoorc.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       39 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/tests/res_partner.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8867 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/tests/test_clodoo_library.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17516 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/tests/__clodoo_test_02.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      730 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/tests/__pytest_transodoo.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    16064 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/oe_watchdog
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    34521 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/LICENSE
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29880 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/transodoo.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    24392 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/clodoolib.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/junk/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5261 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/junk/set_color.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1845 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/junk/clean_pg_template.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2121 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/junk/check_4_seq.sh
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2775 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6804 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/scripts/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/examples/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      734 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/examples/import_products_gb.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5643 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/examples/import_products.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12653 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/examples/import_records.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/docs/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4399 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/rtd_getting_started.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      646 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/readthedocs.yml
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3540 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/rtd_description_transodoo.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4933 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/rtd_description.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4035 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/index.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3561 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/rtd_automodule.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3630 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/rtd_credits.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    25564 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/logozero_180x46.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3589 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/rtd_features.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4931 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/docs/conf.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4874 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/rtd_changelog.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      580 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/Makefile
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       17 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/requirements.txt
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/docs/_build/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/docs/_build/html/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      420 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4208 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15059 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4712 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/sphinx_highlight.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)   288580 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/jquery-3.6.0.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    18215 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/searchtools.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4472 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/doctools.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       90 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    68420 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/underscore-1.13.1.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    89501 2024-02-07 14:24:03.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/jquery.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4929 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      286 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/file.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    25564 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/logozero_180x46.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       90 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4289 2024-02-07 14:24:03.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4758 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/language_data.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    19530 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/docs/_build/html/_static/underscore.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7070 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/rtd_description.html
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10562 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/searchindex.js
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      414 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/objects.inv
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/docs/_build/html/_sources/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4035 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4933 2024-02-07 14:24:02.000000 clodoo-2.0.9/clodoo/docs/_build/html/_sources/rtd_description.rst.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3667 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/search.html
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      230 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/.buildinfo
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4054 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/genindex.html
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/.nojekyll
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8633 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/html/index.html
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/docs/_build/doctrees/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    23763 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/doctrees/rtd_description.doctree
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20214 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/doctrees/index.doctree
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)   255152 2024-02-07 14:24:04.000000 clodoo-2.0.9/clodoo/docs/_build/doctrees/environment.pickle
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17162 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/odoo_skin.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       23 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/travis.ini
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    24448 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/transodoo.xlsx
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6505 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/force_password.sh
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/z0_install/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      345 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/z0_install/main-journal.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       64 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/z0_install/main-company.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      367 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/z0_install/account-journal.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      112 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/z0_install/new-company.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      197 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/z0_install/update-sequence.csv
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      100 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/z0_install/update-user.csv
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    14546 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/manage_odoo
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5621 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/oe_watchdog-server
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4322 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/bck_filestore.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)   233322 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/clodoo_main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20724 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/manage_db
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3085 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/check_one2many.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1362 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/odoo12_notes.txt
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo/egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1659 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/egg-info/DESCRIPTION.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1382 2024-02-07 14:23:00.000000 clodoo-2.0.9/clodoo/egg-info/CHANGELOG.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       44 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/egg-info/description_transodoo.rst
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      115 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/egg-info/FEATURES.rst
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8614 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/export_db_model.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8767 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/moduli_da_installare.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      764 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    93690 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/migrate_odoo_db.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    34513 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/odoorc
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    13528 2024-02-07 14:23:33.000000 clodoo-2.0.9/clodoo/migrate_odoo_db
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1346 2023-12-30 07:50:43.000000 clodoo-2.0.9/clodoo/install_wkhtmltopdf.0.12.4.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2024-02-07 14:25:13.000000 clodoo-2.0.9/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2775 2024-02-07 14:23:33.000000 clodoo-2.0.9/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10870 2024-02-07 14:25:13.000000 clodoo-2.0.9/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7618 2024-02-07 14:24:01.000000 clodoo-2.0.9/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:50:55.000000 clodoo-2.0.9/clodoo.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       95 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5990 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      107 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo.egg-info/requires.txt
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    10870 2024-02-07 14:25:13.000000 clodoo-2.0.9/clodoo.egg-info/PKG-INFO
```

### Comparing `clodoo-2.0.8/clodoo/update_coa.py` & `clodoo-2.0.9/clodoo/update_coa.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 # import pdb
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
@@ -196,7 +196,8 @@
     oerp, uid, ctx = init_n_connect()
     print("Update Chart of Account on DB %s" % (ctx["db_name"]))
     ids = clodoo.searchL8(ctx, "res.company", [])
     for company_id in ids:
         ctx["company_id"] = company_id
         update_coa(ctx)
 
+
```

### Comparing `clodoo-2.0.8/clodoo/manage_odoo.man` & `clodoo-2.0.9/clodoo/manage_odoo.man`

 * *Files identical despite different names*

### Comparing `clodoo-2.0.8/clodoo/clodoocore.py` & `clodoo-2.0.9/clodoo/clodoocore.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 standard_library.install_aliases()  # noqa: E402
 
 
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 #############################################################################
 # Low level (driver) functions
 def psql_connect(ctx):
     cr = False
     if postgres_drive and ctx.get("psycopg2", False):
@@ -1537,7 +1537,8 @@
         n = name[:i]
         x = name[i + 1 : j]
     else:
         n = name
         x = deflt
     return n, x
 
+
```

### Comparing `clodoo-2.0.8/clodoo/odoo_install_repository` & `clodoo-2.0.9/clodoo/odoo_install_repository`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 rmdir_if_exists() {
     #rmdir_if_exists (DSTPATH REPOS odoo_vid new_vid)
     local DSTPATH="$1" REPOS="$2" odoo_vid="$3" new_vid="$4"
     local b fn CWD
     local odoo_fver=$(build_odoo_param FULLVER "$odoo_vid")
     if [[ -d $DSTPATH ]]; then
@@ -475,7 +475,8 @@
 #fi
 [[ ! $REPOS == "OCB" && -z "$(grep "$REPOS/" .gitignore 2>/dev/null)" ]] && run_traced "echo "$REPOS/">>.gitignore"
 update_confn "$CONFN" $DSTPATH
 [[ "$REPOS" == "OCB" ]] && update_confn "$CONFN" "$DSTPATH/addons"
 rm -f $TMPFILE
 exit 0
 
+
```

### Comparing `clodoo-2.0.8/clodoo/transodoo.py` & `clodoo-2.0.9/clodoo/transodoo.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     from z0lib.z0lib import z0lib
 except ImportError:
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 VERSIONS = [
     "6.1",
     "7.0",
     "8.0",
     "9.0",
     "10.0",
     "11.0",
@@ -865,7 +865,8 @@
     sts = transodoo(ctx=ctx)
     return sts
 
 
 if __name__ == "__main__":
     exit(main())
 
+
```

### Comparing `clodoo-2.0.8/clodoo/clodoolib.py` & `clodoo-2.0.9/clodoo/clodoolib.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 # switch values of options
 LX_OPT_ARGS = {}
 DEFDCT = {}
 
 msg_time = time.time()
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 #############################################################################
 # Message and output
 #
 def init_logger(ctx):
     if ctx["quiet_mode"]:
@@ -871,7 +871,8 @@
     if not out:
         return False
     out = os0.u(out)
     if item in ("LPPORT", "MAJVER", "RPCPORT"):
         return eval(out.split("\n")[0])
     return out.split("\n")[0]
 
+
```

### Comparing `clodoo-2.0.8/clodoo/scripts/setup.info` & `clodoo-2.0.9/clodoo/scripts/setup.info`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         "python-plus",
         "unidecode==1.2.0",
         "z0lib",
     ]
 
 setup(
     name=name,
-    version="2.0.8",
+    version="2.0.9",
     description="Do massive operations on Odoo Cloud",
     long_description=long_description,
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 2.7",
@@ -92,7 +92,8 @@
             # "clodoo.py = clodoo.clodoo_main:main",
             "transodoo.py = clodoo.transodoo:main",
         ]
     },
     zip_safe=False,
 )
 
+
```

### Comparing `clodoo-2.0.8/clodoo/scripts/main.py` & `clodoo-2.0.9/clodoo/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import os.path as pth
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -173,7 +173,8 @@
     elif action in ("-H", "--help"):
         for text in __doc__.split("\n"):
             print(text)
     elif action in ("-C", "--copy-pkg-data"):
         copy_pkg_data(setup_args, verbose)
     return 0
 
+
```

### Comparing `clodoo-2.0.8/clodoo/transodoo.xlsx` & `clodoo-2.0.9/clodoo/transodoo.xlsx`

 * *Files identical despite different names*

### Comparing `clodoo-2.0.8/clodoo/manage_odoo` & `clodoo-2.0.9/clodoo/manage_odoo`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 
 explore() {
 # explore(odoo_vid excl_list)
     local res=OCB
     local pkgdir=$(build_odoo_param HOME "$1" "" "$opt_org" "$opt_deploy")
     for fn in $pkgdir/*; do
@@ -322,7 +322,8 @@
         [[ $a =~ ^q ]] && exit $sts
       fi
     fi
   done
 done
 exit $sts
 
+
```

### Comparing `clodoo-2.0.8/clodoo/bck_filestore.sh` & `clodoo-2.0.9/clodoo/bck_filestore.sh`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 
 OPTOPTS=(h        b          n            q           t       V           v)
 OPTDEST=(opt_help opt_branch opt_dry_run  opt_verbose opt_tgt opt_version opt_verbose)
 OPTACTI=("+"      "="        "1"          0           "=>"    "*>"        "+" )
 OPTDEFL=(1        ""         0            -1          ""      ""          -1)
 OPTMETA=("help"   "vid"      "do nothing" "verbose"   "host"  "version"   "silent")
@@ -82,7 +82,8 @@
 for odoo_vid in ${opt_branch//,/ };do
   DDIR=$(build_odoo_param DDIR $odoo_vid)
   echo "rsync -avz $DDIR/filestore/ $opt_tgt:$DDIR/filestore/"
   [ $opt_dry_run -eq 0 ] && rsync -avz $DDIR/filestore/ $opt_tgt:$DDIR/filestore/
 done
 exit $sts
 
+
```

### Comparing `clodoo-2.0.8/clodoo/clodoo_main.py` & `clodoo-2.0.9/clodoo/clodoo_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     from clodoo.transodoo import read_stored_dict, translate_from_to
 
 # TMP
 from subprocess import PIPE, Popen
 
 standard_library.install_aliases()  # noqa: E402
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 # Apply for configuration file (True/False)
 APPLY_CONF = True
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 PAY_MOVE_STS_2_DRAFT = ['posted']
@@ -6557,7 +6557,8 @@
     msg_log(ctx, ctx['level'], msg)
     return sts
 
 
 if __name__ == "__main__":
     exit(main())
 
+
```

### Comparing `clodoo-2.0.8/clodoo/manage_db` & `clodoo-2.0.9/clodoo/manage_db`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 
 up_oemod() {
 #up_oemod(DB branch)
     local DB=$1
     local oe_version=$2
     local passed_file=./upd_oemod_passed.log
@@ -512,7 +512,8 @@
   else
     echo "Invalid action!"
     sts=1
   fi
 done
 exit $sts
 
+
```

### Comparing `clodoo-2.0.8/clodoo/check_one2many.py` & `clodoo-2.0.9/clodoo/check_one2many.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import pdb
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
     if t > 3:
@@ -94,7 +94,8 @@
                 with open("check_one2many.log", "ab") as log:
                     log.write("**** Error in model %s id %d! ****\n" % (model2, id))
     except BaseException:
         print("**** Error in model %s id %d! ****" % (model_fld, fld_id))
         with open("check_one2many.log", "ab") as log:
             log.write("**** Error in model %s id %d! ****\n" % (model_fld, fld_id))
 
+
```

### Comparing `clodoo-2.0.8/clodoo/export_db_model.py` & `clodoo-2.0.9/clodoo/export_db_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import pdb
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 CACHE = {}
 
 
 def get_symbolic_value(ctx, model, name, value):
     name_model = "ir.model.data"
@@ -276,7 +276,8 @@
 ctx = parser.parseoptargs(sys.argv[1:], apply_conf=False)
 uid, ctx = clodoo.oerp_set_env(confn=ctx["conf_fn"], db=ctx["db_name"], ctx=ctx)
 if ctx["model"]:
     export_table(ctx)
 else:
     print("Missed model name!")
 
+
```

### Comparing `clodoo-2.0.8/clodoo/moduli_da_installare.py` & `clodoo-2.0.9/clodoo/moduli_da_installare.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import transodoo
 # import pdb
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 VERSIONS = ["vg7", "61", "70", "80", "90", "100", "110", "120"]
 VERSIONS_PLUS = ["vg7", "61", "70", "80", "90", "100", "110", "120", "0"]
 ALIAS = {}
 
 
@@ -334,7 +334,8 @@
 print(line)
 line = "TOTALE"
 for id in VERSIONS:
     line = "%s,%s" % (line, ctrs[id])
 fd.write(line)
 fd.close()
 
+
```

### Comparing `clodoo-2.0.8/clodoo/__init__.py` & `clodoo-2.0.9/clodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `clodoo-2.0.8/clodoo/migrate_odoo_db.py` & `clodoo-2.0.9/clodoo/migrate_odoo_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 00000290: 2020 2020 2020 6672 6f6d 207a 306c 6962        from z0lib
 000002a0: 2069 6d70 6f72 7420 7a30 6c69 620a 2020   import z0lib.  
 000002b0: 2020 6578 6365 7074 2049 6d70 6f72 7445    except ImportE
 000002c0: 7272 6f72 3a0a 2020 2020 2020 2020 696d  rror:.        im
 000002d0: 706f 7274 207a 306c 6962 0a69 6d70 6f72  port z0lib.impor
 000002e0: 7420 7472 616e 736f 646f 6f0a 0a23 2069  t transodoo..# i
 000002f0: 6d70 6f72 7420 7064 620a 0a0a 5f5f 7665  mport pdb...__ve
-00000300: 7273 696f 6e5f 5f20 3d20 2232 2e30 2e38  rsion__ = "2.0.8
+00000300: 7273 696f 6e5f 5f20 3d20 2232 2e30 2e39  rsion__ = "2.0.9
 00000310: 220a 4d41 585f 4445 4550 203d 2032 300a  ".MAX_DEEP = 20.
 00000320: 5359 5354 454d 5f4d 4f44 454c 5f52 4f4f  SYSTEM_MODEL_ROO
 00000330: 5420 3d20 5b0a 2020 2020 2762 6173 652e  T = [.    'base.
 00000340: 636f 6e66 6967 2e27 2c0a 2020 2020 2762  config.',.    'b
 00000350: 6173 655f 696d 706f 7274 2e27 2c0a 2020  ase_import.',.  
 00000360: 2020 2762 6173 652e 6c61 6e67 7561 6765    'base.language
 00000370: 2e27 2c0a 2020 2020 2762 6173 652e 6d6f  .',.    'base.mo
@@ -5849,8 +5849,8 @@
 00016d80: 7372 635f 6374 785b 2773 656c 5f6d 6f64  src_ctx['sel_mod
 00016d90: 656c 275d 3a0a 2020 2020 2020 2020 6d69  el']:.        mi
 00016da0: 6772 6174 655f 7365 6c5f 7461 626c 6573  grate_sel_tables
 00016db0: 2873 7263 5f63 7478 2c20 7467 745f 6374  (src_ctx, tgt_ct
 00016dc0: 7829 0a20 2020 2065 6c73 653a 0a20 2020  x).    else:.   
 00016dd0: 2020 2020 206d 6967 7261 7465 5f64 6174       migrate_dat
 00016de0: 6162 6173 6528 7372 635f 6374 782c 2074  abase(src_ctx, t
-00016df0: 6774 5f63 7478 290a 0a                   gt_ctx)..
+00016df0: 6774 5f63 7478 290a 0a0a                 gt_ctx)...
```

### Comparing `clodoo-2.0.8/clodoo/odoorc` & `clodoo-2.0.9/clodoo/odoorc`

 * *Files 0% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 # ODOO_GIT_ORGID    -> default git organization
 # ODOO_GIT_HOSTNAME -> git hostname (def github.com)
 # ODOO_GIT_PROT     -> default protocol (git|https) for default git organization
 # ODOO_GIT_SHORT    -> regex of git organizations with short name (def /(oca)/)
 # ODOO_GIT_MULTI    -> multi version environment
 #
 
-__version__=2.0.8
+__version__=2.0.9
 
 
-ODOO_FVERS="16\.0|15\.0|14\.0|13\.0|12\.0|11\.0|10\.0|9\.0|8\.0|7\.0|6\.1"
-ODOO_VERS="16|15|14|13|12|11|10|9|8|7|6"
+ODOO_FVERS="18\.0|17\.0|16\.0|15\.0|14\.0|13\.0|12\.0|11\.0|10\.0|9\.0|8\.0|7\.0|6\.1"
+ODOO_VERS="18|17|16|15|14|13|12|11|10|9|8|7|6"
 DEFMLIST="OCB account-analytic account-budgeting account-closing
  account-consolidation account-financial-reporting account-financial-tools
  account-fiscal-rule account-invoice-reporting account-invoicing
  account-payment account-reconcile ansible-odoo apps-store bank-payment
  bank-statement-import brand business-requirement calendar commission
  community-data-files connector contract contribute-md-template
  credit-control crm currency data-protection ddmrp delivery-carrier department
@@ -203,15 +203,15 @@
         fi
     fi
     echo "$PKGNAME|$PKGPATH|$PARENTDIR|$REPOS|$PRJPATH"
 }
 
 build_odoo_param() {
     # build_odoo_param(ALL|BIN|CONFN|DB_USER|DDIR|DIRLEVEL|FLOG|FPID|FULLVER|FULL_SVCNAME|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGNM|GIT_PROT|GIT_URL|HOME|INVALID_MODNAMES|INVALID_MODNAMES_RE|IS_MULTI|LICENSE|LCONFN|LPPORT|MAJVER|MANIFEST|OCB_SUBDIRS|OCB_SUBDIRS_RE|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RPCPORT|RUPSTREAM|SESS_PATH|SVCNAME|UPSTREAM|URL|URL_BRANCH|USER|VCS|VDIR|VENV
-    #                  vid [(search|DEBUG|default|tree|SERVER|<rptname>|<modname>)] [oca|zero|zero-http|zero-git|librerp|flectra] [(search|DEBUG|default|tree|SERVER)])
+    #                  vid [(search|DEBUG|default|tree|SERVER|<rptname>|<modname>)] [oca|zero|zero-http|zero-git|librerp|flectra] [(search|DEBUG|default|tree|SERVER|MULTI)])
     [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
     if [[ $1 =~ (INVALID_MODNAMES|INVALID_MODNAMES_RE|OCB_SUBDIRS|OCB_SUBDIRS_RE) ]]; then
         echo "${!1}"
         $SETX
         return
     fi
     if [[ $1 == "IS_MULTI" ]]; then
@@ -246,15 +246,15 @@
     local reo="^($p1)"
     local reg="($p2)"
     local ref="($ODOO_FVERS)"
     [[ -n "$ODOO_GIT_SHORT" ]] && SHORT="$ODOO_GIT_SHORT" || SHORT="(oca)"
     [[ -z "$ODOO_GIT_HOSTNAME" ]] && ODOO_GIT_HOSTNAME="(github.com)"
     [[ -z "$ODOO_DB_USER" ]] && ODOO_DB_USER="odoo%(MAJVER)s"
     [[ $3 =~ ^((DEBUG|default|search|SERVER|tree|odoo|short),?)+$ ]] && spec=$3 || REPOS=$3
-    [[ $5 =~ ^((DEBUG|default|search|SERVER|tree|odoo|short),?)+$ ]] && spec=$5
+    [[ $5 =~ ^((DEBUG|default|search|SERVER|tree|odoo|short|MULTI),?)+$ ]] && spec=$5
     exorg=0
     GIT_ORGNM=""
     GIT_PROT=""
     RUPSTREAM=""
     RORIGIN=""
     if [[ "$2" =~ (^\.$|^\.\.$|(\./|\.\./|~/|/)) ]]; then
         if [[ $ITEM == "DIRLEVEL" ]]; then
@@ -349,15 +349,15 @@
     [[ -z "$GIT_BRANCH" ]] && GIT_BRANCH="$FULLVER"
     MAJVER=$(get_odoo_major_ver "$FULLVER")
     if [[ "$ITEM" == "MANIFEST" ]]; then
         [[ $MAJVER -ge 10 ]] && echo "__manifest__.py" || echo "__openerp__.py"
         $SETX
         return
     fi
-    [[ -n $ODOO_ODOO_GIT_MULTI ]] && MULITVER=$ODOO_GIT_MULTI || [[ ${opt_multi:-0} -ne 0 ]] && MULTIVER=1 || MULTIVER=0
+    [[ -n $ODOO_ODOO_GIT_MULTI ]] && MULITVER=$ODOO_GIT_MULTI || [[ ${opt_multi:-0} -ne 0 || $5 =~ MULTI ]] && MULTIVER=1 || MULTIVER=0
     ORGSFX=$(echo $noenv_vid | grep --color=never -Eo "[-_][a-z][a-z0-9]+$" | grep --color=never -Eo "[a-z0-9]+")
     if [[ -n $ORGSFX ]]; then
         [[ $ORGSFX =~ -git$ ]] && GIT_PROT="git" && ORGSFX=${ORGSFX:0: -4}
         [[ $ORGSFX =~ -http$ ]] && GIT_PROT="https" && ORGSFX=${ORGSFX:0: -5}
         [[ $ORGSFX == "librerp6" ]] && ORGSFX="librerp"
     fi
     if [[ -n $ORGSFX && $ORGSFX =~ ^$reg ]]; then
@@ -399,14 +399,15 @@
     fi
     [[ $GIT_ORGNM == "OCA" ]] && GIT_ORGID="oca"
     [[ $GIT_ORGNM == "zeroincombenze" ]] && GIT_ORGID="zero"
     [[ $GIT_ORGNM =~ ^(LibrERP-network|LibrERP) ]] && GIT_ORGID="librerp"
     [[ $GIT_ORGNM == "iw3hxn" ]] && GIT_ORGID="librerp6"
     [[ $GIT_ORGNM =~ ^(PowERP-cloud|powerp1) ]] && GIT_ORGID="powerp"
     [[ -z $GIT_ORGID ]] && GIT_ORGID="$GIT_ORGNM"
+    [[ -n "$4" && $GIT_ORGID != $4 && -z $ORGSFX ]] && ORGSFX=$4
     [[ -n $ODOO_GIT_ORGID && ( $GIT_ORGID == $ODOO_GIT_ORGID || $GIT_ORGID =~ ^$ODOO_GIT_ORGID$ ) ]] && GIT_PROT="git"
     [[ -n $ODOO_GIT_PROT ]] && GIT_PROT="$ODOO_GIT_PROT"
     if [[ "$ITEM" == "LICENSE" ]]; then
         if [[ -z "$LICENSE" ]]; then
           [[ $GIT_ORGID == "powerp" ]] && LICENSE="OPL"
           [[ -z "$LICENSE" && $MAJVER -le 8 ]] && LICENSE="AGPL"
           [[ -z "$LICENSE" ]] && LICENSE="LGPL"
@@ -482,14 +483,15 @@
     if [[ $main -ne 0 ]]; then
         DB_USER="odoo"
     elif [[ $MAJVER -lt 8 && $USER == "openerp" ]]; then
         DB_USER="openerp"
     elif [[ $MULTIVER -ne 0 ]]; then
         DB_USER=${ODOO_DB_USER/\%(MAJVER)s/$MAJVER}
         DB_USER=${DB_USER/\%(ORGSFX)s/$ORGSFX}
+        [[ $GIT_ORGID == "oca" ]] && DB_USER=${DB_USER/odoo/oca}
     else
         DB_USER="odoo"
     fi
     [[ -z "$VDIR" ]] && VDIR="$ROOT/venv_odoo"
     if [[ "$ITEM" =~ ^(DB_USER|FULLVER|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGID|GIT_ORGNM|GIT_URL|MAJVER|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RUPSTREAM|URL|URL_BRANCH|VCS|VDIR|VENV)$ ]]; then
         echo "${!ITEM}"
         $SETX
@@ -511,15 +513,15 @@
         if [[ $spec =~ (debug|DEBUG) ]]; then
             ((p = 18060 + $MAJVER))
         elif [[ $main -ne 0 || $MULTIVER -eq 0 ]]; then
             p=8069
         elif [[ $MULTIVER -ne 0 ]]; then
             if [ $exorg -eq 0 ]; then
                 ((p = 8160 + $MAJVER))
-            elif [[ $GIT_ORGID == "oca" ]]; then
+            elif [[ $GIT_ORGID =~ (odoo|oca) ]]; then
                 ((p = 8260 + $MAJVER))
             elif [[ $GIT_ORGID =~ ^(powerp|librerp[6]?)$ ]]; then
                 ((p = 8360 + $MAJVER))
             elif [[ $GIT_ORGID =~ ^(zero|flectra)$ ]]; then
                 ((p = 8460 + $MAJVER))
             else
                 ((p = 8160 + $MAJVER))
@@ -534,15 +536,15 @@
         if [[ $spec =~ (debug|DEBUG) ]]; then
             ((p = 18160 + $MAJVER))
         elif [[ $main -ne 0 || $MULTIVER -eq 0 ]]; then
             p=8072
         elif [[ $MULTIVER -ne 0 ]]; then
             if [[ $exorg -eq 0 ]]; then
                 ((p = 8130 + $MAJVER))
-            elif [[ $GIT_ORGID == "oca" ]]; then
+            elif [[ $GIT_ORGID =~ (odoo|oca) ]]; then
                 ((p = 8230 + $MAJVER))
             elif [[ $GIT_ORGID =~ ^(powerp|librerp[6]?)$ ]]; then
                 ((p = 8330 + $MAJVER))
             elif [[ $GIT_ORGID =~ ^(zero|flectra)$ ]]; then
                 ((p = 8430 + $MAJVER))
             else
                 ((p = 8130 + $MAJVER))
```

### Comparing `clodoo-2.0.8/setup.py` & `clodoo-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         "python-plus",
         "unidecode==1.2.0",
         "z0lib",
     ]
 
 setup(
     name=name,
-    version="2.0.8",
+    version="2.0.9",
     description="Do massive operations on Odoo Cloud",
     long_description=long_description,
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 2.7",
@@ -92,7 +92,8 @@
             # "clodoo.py = clodoo.clodoo_main:main",
             "transodoo.py = clodoo.transodoo:main",
         ]
     },
     zip_safe=False,
 )
 
+
```

### Comparing `clodoo-2.0.8/PKG-INFO` & `clodoo-2.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 1.2
 Name: clodoo
-Version: 2.0.8
+Version: 2.0.9
 Summary: Do massive operations on Odoo Cloud
 Home-page: https://github.com/zeroincombenze/tools
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools/tree/master/clodoo
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io/en/latest/#clodoo
 Project-URL: Changelog, https://github.com/zeroincombenze/tools/blob/master/clodoo/egg-info/CHANGELOG.rst
 Description: ============
-        clodoo 2.0.8
+        clodoo 2.0.9
         ============
         
         
         
         |Maturity| |license gpl|
         
         
@@ -57,23 +57,18 @@
             PARAM is one of (ALL|BIN|CONFN|DB_USER|DDIR|FLOG|FPID|FULLVER|FULL_SVCNAME|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGNM|GIT_PROT|GIT_URL|HOME|INVALID_MODNAMES|INVALID_MODNAMES_RE|LICENSE|LCONFN|MAJVER|MANIFEST|OCB_SUBDIRS|OCB_SUBDIRS_RE|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RPCPORT|RUPSTREAM|SVCNAME|UPSTREAM|URL|URL_BRANCH|USER|VCS|VDIR|VENV)
         
         
         
         Features
         --------
         
-        +------------------------------------------------------------+-------------------------+
-        | Function                                                   | Note                    |
-        +------------------------------------------------------------+-------------------------+
-        | Manage version depending names                             | transodoo.py            |
-        +------------------------------------------------------------+-------------------------+
-        | Odoo general purpose library                               | odoorc                  |
-        +------------------------------------------------------------+-------------------------+
-        | Examples                                                   | example*.py             |
-        +------------------------------------------------------------+-------------------------+
+        Function,Note
+        Manage version depending names,transodoo.py
+        Odoo general purpose library,odoorc
+        Examples,example*.py
         
         
         
         Getting started
         ===============
         
         
@@ -117,29 +112,33 @@
         Stable version via Python Package
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         ::
         
             pip install --upgrade clodoo
         
-        
         Current version via Git
         ~~~~~~~~~~~~~~~~~~~~~~~
         
         ::
         
             cd ./tools
             ./install_tools.sh -pUT
             source $HOME/devel/activate_tools
         
         
         
         ChangeLog History
         -----------------
         
+        2.0.9 (2024-02-02)
+        ~~~~~~~~~~~~~~~~~~
+        
+        [IMP] odoorc improvements
+        
         2.0.8 (2023-11-16)
         ~~~~~~~~~~~~~~~~~~
         
         [FIX] Discard odoorpc 0.10 which does not work
         
         2.0.7 (2023-09-26)
         ~~~~~~~~~~~~~~~~~~
@@ -240,18 +239,18 @@
         .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
             :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
             :alt: License: AGPL-3
         .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
             :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
             :alt: License: OPL
         .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
-            :target: https://wiki.zeroincombenze.org/en/Odoo/2.0.8/dev
+            :target: https://wiki.zeroincombenze.org/en/Odoo/2.0.9/dev
             :alt: Technical Documentation
         .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
-            :target: https://wiki.zeroincombenze.org/it/Odoo/2.0.8/man
+            :target: https://wiki.zeroincombenze.org/it/Odoo/2.0.9/man
             :alt: Technical Documentation
         .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
             :target: https://erp2.zeroincombenze.it
             :alt: Try Me
         .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
            :target: https://www.zeroincombenze.it/
            :alt: Zeroincombenze
```

### Comparing `clodoo-2.0.8/README.rst` & `clodoo-2.0.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ============
-clodoo 2.0.8
+clodoo 2.0.9
 ============
 
 
 
 |Maturity| |license gpl|
 
 
@@ -46,23 +46,18 @@
     PARAM is one of (ALL|BIN|CONFN|DB_USER|DDIR|FLOG|FPID|FULLVER|FULL_SVCNAME|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGNM|GIT_PROT|GIT_URL|HOME|INVALID_MODNAMES|INVALID_MODNAMES_RE|LICENSE|LCONFN|MAJVER|MANIFEST|OCB_SUBDIRS|OCB_SUBDIRS_RE|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RPCPORT|RUPSTREAM|SVCNAME|UPSTREAM|URL|URL_BRANCH|USER|VCS|VDIR|VENV)
 
 
 
 Features
 --------
 
-+------------------------------------------------------------+-------------------------+
-| Function                                                   | Note                    |
-+------------------------------------------------------------+-------------------------+
-| Manage version depending names                             | transodoo.py            |
-+------------------------------------------------------------+-------------------------+
-| Odoo general purpose library                               | odoorc                  |
-+------------------------------------------------------------+-------------------------+
-| Examples                                                   | example*.py             |
-+------------------------------------------------------------+-------------------------+
+Function,Note
+Manage version depending names,transodoo.py
+Odoo general purpose library,odoorc
+Examples,example*.py
 
 
 
 Getting started
 ===============
 
 
@@ -106,29 +101,33 @@
 Stable version via Python Package
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     pip install --upgrade clodoo
 
-
 Current version via Git
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd ./tools
     ./install_tools.sh -pUT
     source $HOME/devel/activate_tools
 
 
 
 ChangeLog History
 -----------------
 
+2.0.9 (2024-02-02)
+~~~~~~~~~~~~~~~~~~
+
+[IMP] odoorc improvements
+
 2.0.8 (2023-11-16)
 ~~~~~~~~~~~~~~~~~~
 
 [FIX] Discard odoorpc 0.10 which does not work
 
 2.0.7 (2023-09-26)
 ~~~~~~~~~~~~~~~~~~
@@ -229,18 +228,18 @@
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
     :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
     :alt: License: OPL
 .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
-    :target: https://wiki.zeroincombenze.org/en/Odoo/2.0.8/dev
+    :target: https://wiki.zeroincombenze.org/en/Odoo/2.0.9/dev
     :alt: Technical Documentation
 .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
-    :target: https://wiki.zeroincombenze.org/it/Odoo/2.0.8/man
+    :target: https://wiki.zeroincombenze.org/it/Odoo/2.0.9/man
     :alt: Technical Documentation
 .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
     :target: https://erp2.zeroincombenze.it
     :alt: Try Me
 .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
    :target: https://www.zeroincombenze.it/
    :alt: Zeroincombenze
```

### Comparing `clodoo-2.0.8/clodoo.egg-info/PKG-INFO` & `clodoo-2.0.9/clodoo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 1.2
 Name: clodoo
-Version: 2.0.8
+Version: 2.0.9
 Summary: Do massive operations on Odoo Cloud
 Home-page: https://github.com/zeroincombenze/tools
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools/tree/master/clodoo
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io/en/latest/#clodoo
 Project-URL: Changelog, https://github.com/zeroincombenze/tools/blob/master/clodoo/egg-info/CHANGELOG.rst
 Description: ============
-        clodoo 2.0.8
+        clodoo 2.0.9
         ============
         
         
         
         |Maturity| |license gpl|
         
         
@@ -57,23 +57,18 @@
             PARAM is one of (ALL|BIN|CONFN|DB_USER|DDIR|FLOG|FPID|FULLVER|FULL_SVCNAME|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGNM|GIT_PROT|GIT_URL|HOME|INVALID_MODNAMES|INVALID_MODNAMES_RE|LICENSE|LCONFN|MAJVER|MANIFEST|OCB_SUBDIRS|OCB_SUBDIRS_RE|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RPCPORT|RUPSTREAM|SVCNAME|UPSTREAM|URL|URL_BRANCH|USER|VCS|VDIR|VENV)
         
         
         
         Features
         --------
         
-        +------------------------------------------------------------+-------------------------+
-        | Function                                                   | Note                    |
-        +------------------------------------------------------------+-------------------------+
-        | Manage version depending names                             | transodoo.py            |
-        +------------------------------------------------------------+-------------------------+
-        | Odoo general purpose library                               | odoorc                  |
-        +------------------------------------------------------------+-------------------------+
-        | Examples                                                   | example*.py             |
-        +------------------------------------------------------------+-------------------------+
+        Function,Note
+        Manage version depending names,transodoo.py
+        Odoo general purpose library,odoorc
+        Examples,example*.py
         
         
         
         Getting started
         ===============
         
         
@@ -117,29 +112,33 @@
         Stable version via Python Package
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         ::
         
             pip install --upgrade clodoo
         
-        
         Current version via Git
         ~~~~~~~~~~~~~~~~~~~~~~~
         
         ::
         
             cd ./tools
             ./install_tools.sh -pUT
             source $HOME/devel/activate_tools
         
         
         
         ChangeLog History
         -----------------
         
+        2.0.9 (2024-02-02)
+        ~~~~~~~~~~~~~~~~~~
+        
+        [IMP] odoorc improvements
+        
         2.0.8 (2023-11-16)
         ~~~~~~~~~~~~~~~~~~
         
         [FIX] Discard odoorpc 0.10 which does not work
         
         2.0.7 (2023-09-26)
         ~~~~~~~~~~~~~~~~~~
@@ -240,18 +239,18 @@
         .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
             :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
             :alt: License: AGPL-3
         .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
             :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
             :alt: License: OPL
         .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
-            :target: https://wiki.zeroincombenze.org/en/Odoo/2.0.8/dev
+            :target: https://wiki.zeroincombenze.org/en/Odoo/2.0.9/dev
             :alt: Technical Documentation
         .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
-            :target: https://wiki.zeroincombenze.org/it/Odoo/2.0.8/man
+            :target: https://wiki.zeroincombenze.org/it/Odoo/2.0.9/man
             :alt: Technical Documentation
         .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
             :target: https://erp2.zeroincombenze.it
             :alt: Try Me
         .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
            :target: https://www.zeroincombenze.it/
            :alt: Zeroincombenze
```

