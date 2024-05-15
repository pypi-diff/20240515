# Comparing `tmp/mns-scheduler-1.0.4.7.tar.gz` & `tmp/mns-scheduler-1.0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.4.7.tar", last modified: Wed May 15 07:01:38 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.4.8.tar", last modified: Wed May 15 13:31:41 2024, max compression
```

## Comparing `mns-scheduler-1.0.4.7.tar` & `mns-scheduler-1.0.4.8.tar`

### file list

```diff
@@ -1,111 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.483652 mns-scheduler-1.0.4.7/
--rw-rw-rw-   0        0        0       62 2024-05-15 07:01:38.482655 mns-scheduler-1.0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.447748 mns-scheduler-1.0.4.7/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-05-15 00:08:32.000000 mns-scheduler-1.0.4.7/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.449744 mns-scheduler-1.0.4.7/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.449744 mns-scheduler-1.0.4.7/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.452735 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.453732 mns-scheduler-1.0.4.7/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.453732 mns-scheduler-1.0.4.7/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.455727 mns-scheduler-1.0.4.7/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15735 2024-05-13 09:25:17.000000 mns-scheduler-1.0.4.7/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20342 2024-05-13 09:29:51.000000 mns-scheduler-1.0.4.7/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.455727 mns-scheduler-1.0.4.7/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.457722 mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.457722 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.459717 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.460714 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.462708 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.463706 mns-scheduler-1.0.4.7/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.4.7/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.464703 mns-scheduler-1.0.4.7/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.465700 mns-scheduler-1.0.4.7/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-14 13:59:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/finance/__init__.py
--rw-rw-rw-   0        0        0    26721 2024-05-15 06:18:00.000000 mns-scheduler-1.0.4.7/mns_scheduler/finance/em_financial_sync_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.465700 mns-scheduler-1.0.4.7/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.467695 mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.468692 mns-scheduler-1.0.4.7/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.468692 mns-scheduler-1.0.4.7/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.469690 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.470687 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.471684 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.472682 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.473679 mns-scheduler-1.0.4.7/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.7/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.474677 mns-scheduler-1.0.4.7/mns_scheduler/risk/
--rw-rw-rw-   0        0        0      163 2024-05-14 14:32:33.000000 mns-scheduler-1.0.4.7/mns_scheduler/risk/__init__.py
--rw-rw-rw-   0        0        0     4883 2024-05-15 00:18:26.000000 mns-scheduler-1.0.4.7/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.476672 mns-scheduler-1.0.4.7/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.7/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.7/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.7/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.477669 mns-scheduler-1.0.4.7/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.480661 mns-scheduler-1.0.4.7/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17272 2024-05-11 03:32:32.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7604 2024-05-09 15:06:22.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.482655 mns-scheduler-1.0.4.7/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    16100 2024-05-14 16:54:03.000000 mns-scheduler-1.0.4.7/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.482655 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-15 07:01:38.000000 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2024-05-15 07:01:38.000000 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 07:01:38.000000 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-15 07:01:38.000000 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 07:01:38.483652 mns-scheduler-1.0.4.7/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-15 07:01:25.000000 mns-scheduler-1.0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.786311 mns-scheduler-1.0.4.8/
+-rw-rw-rw-   0        0        0       62 2024-05-15 13:31:41.786311 mns-scheduler-1.0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.745420 mns-scheduler-1.0.4.8/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-05-15 00:08:32.000000 mns-scheduler-1.0.4.8/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.747415 mns-scheduler-1.0.4.8/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.748412 mns-scheduler-1.0.4.8/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.750408 mns-scheduler-1.0.4.8/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.751405 mns-scheduler-1.0.4.8/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.752402 mns-scheduler-1.0.4.8/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.754397 mns-scheduler-1.0.4.8/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15735 2024-05-13 09:25:17.000000 mns-scheduler-1.0.4.8/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20342 2024-05-13 09:29:51.000000 mns-scheduler-1.0.4.8/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.755394 mns-scheduler-1.0.4.8/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.756392 mns-scheduler-1.0.4.8/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.756392 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.758386 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.760380 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.762376 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.763374 mns-scheduler-1.0.4.8/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.4.8/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.764370 mns-scheduler-1.0.4.8/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.768360 mns-scheduler-1.0.4.8/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-14 13:59:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/finance/__init__.py
+-rw-rw-rw-   0        0        0    17231 2024-05-15 08:23:18.000000 mns-scheduler-1.0.4.8/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
+-rw-rw-rw-   0        0        0    13875 2024-05-15 10:06:25.000000 mns-scheduler-1.0.4.8/mns_scheduler/finance/em_financial_profit_sync_service_api.py
+-rw-rw-rw-   0        0        0     1075 2024-05-15 09:52:38.000000 mns-scheduler-1.0.4.8/mns_scheduler/finance/finance_common_api.py
+-rw-rw-rw-   0        0        0     8328 2024-05-15 11:53:51.000000 mns-scheduler-1.0.4.8/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
+-rw-rw-rw-   0        0        0     6007 2024-05-15 13:23:56.000000 mns-scheduler-1.0.4.8/mns_scheduler/finance/sync_financial_report_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.768360 mns-scheduler-1.0.4.8/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.770354 mns-scheduler-1.0.4.8/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.771352 mns-scheduler-1.0.4.8/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.4.8/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.771352 mns-scheduler-1.0.4.8/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.772349 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.773346 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.774344 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.775341 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.777336 mns-scheduler-1.0.4.8/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.8/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.778333 mns-scheduler-1.0.4.8/mns_scheduler/risk/
+-rw-rw-rw-   0        0        0      163 2024-05-14 14:32:33.000000 mns-scheduler-1.0.4.8/mns_scheduler/risk/__init__.py
+-rw-rw-rw-   0        0        0     4949 2024-05-15 12:17:25.000000 mns-scheduler-1.0.4.8/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.779330 mns-scheduler-1.0.4.8/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.8/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.8/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.8/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.780327 mns-scheduler-1.0.4.8/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.784317 mns-scheduler-1.0.4.8/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17272 2024-05-11 03:32:32.000000 mns-scheduler-1.0.4.8/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-09 15:06:22.000000 mns-scheduler-1.0.4.8/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.785314 mns-scheduler-1.0.4.8/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    16100 2024-05-14 16:54:03.000000 mns-scheduler-1.0.4.8/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.8/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:41.785314 mns-scheduler-1.0.4.8/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-15 13:31:41.000000 mns-scheduler-1.0.4.8/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3732 2024-05-15 13:31:41.000000 mns-scheduler-1.0.4.8/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 13:31:41.000000 mns-scheduler-1.0.4.8/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 13:31:41.000000 mns-scheduler-1.0.4.8/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 13:31:41.786311 mns-scheduler-1.0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-15 13:31:18.000000 mns-scheduler-1.0.4.8/setup.py
```

### Comparing `mns-scheduler-1.0.4.7/README.md` & `mns-scheduler-1.0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.4.8/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.4.8/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.4.8/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.4.8/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.4.8/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.4.8/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.4.8/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.4.8/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.4.8/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/finance/em_financial_sync_service_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 16
 project_path = file_path[0:end]
 sys.path.append(project_path)
 import akshare as ak
 from mns_common.db.MongodbUtil import MongodbUtil
-
+import mns_scheduler.finance.finance_common_api as finance_common_api
+import mns_common.constant.db_name_constant as db_name_constant
 mongodb_util = MongodbUtil('27017')
+from loguru import logger
+import mns_common.utils.data_frame_util as data_frame_util
 
 
 #
 # {
 #     "_id" : ObjectId("6644358f8eb1db9684c8b75d"),
 #     "SECUCODE" : "600519.SH",
 #     "SECURITY_CODE" : "600519",
@@ -333,16 +336,23 @@
 #     "OPINION_TYPE" : null, 审计意见(境内)
 #     "OSOPINION_TYPE" : NaN,
 #     "LISTING_STATE" : "0"
 # }
 
 # 资产负债表
 # https://emweb.securities.eastmoney.com/PC_HSF10/NewFinanceAnalysis/Index?type=web&code=sh600519#zcfzb-0
-def get_em_debt_api(symbol):
-    stock_balance_sheet_by_report_em_df = ak.stock_balance_sheet_by_report_em(symbol)
+def get_em_asset_liability_api(symbol):
+    sec_code = finance_common_api.get_sec_code(symbol)
+    try:
+        stock_balance_sheet_by_report_em_df = ak.stock_balance_sheet_by_report_em(sec_code)
+    except Exception as e:
+        logger.error("同步利润表异常:{},{}", symbol, e)
+        return None
+    if data_frame_util.is_empty(stock_balance_sheet_by_report_em_df):
+        return None
     stock_balance_sheet_by_report_em_df = stock_balance_sheet_by_report_em_df[[
         'SECUCODE',
         'SECURITY_CODE',
         'SECURITY_NAME_ABBR',
         'ORG_CODE',
         'ORG_TYPE',
         'REPORT_DATE',
@@ -399,280 +409,28 @@
         'TOTAL_OTHER_RECE',
         'TOTAL_PARENT_EQUITY',
         'TRADE_FINASSET_NOTFVTPL',
         'UNASSIGN_RPOFIT',
         'USERIGHT_ASSET',
         'OPINION_TYPE'
     ]]
-    print(stock_balance_sheet_by_report_em_df)
-    mongodb_util.insert_mongo(stock_balance_sheet_by_report_em_df, 'stock_balance_sheet_by_report_em_df')
-
+    stock_balance_sheet_by_report_em_df['_id'] = (stock_balance_sheet_by_report_em_df['SECURITY_CODE']
+                                                  + "_" + stock_balance_sheet_by_report_em_df['REPORT_DATE'])
 
-# 利润表
-#  "_id" : ObjectId("6644085f608b7737dee21a3a"),
-#     "SECUCODE" : "600519.SH",
-#     "SECURITY_CODE" : "600519",
-#     "SECURITY_NAME_ABBR" : "贵州茅台",
-#     "ORG_CODE" : "10002602",
-#     "ORG_TYPE" : "通用",
-#     "REPORT_DATE" : "2023-12-31 00:00:00",
-#     "REPORT_TYPE" : "年报",
-#     "REPORT_DATE_NAME" : "2023年报",
-#     "SECURITY_TYPE_CODE" : "058001001",
-#     "NOTICE_DATE" : "2024-04-03 00:00:00",
-#     "UPDATE_DATE" : "2024-04-03 00:00:00",
-#     "CURRENCY" : "CNY",
-#     "TOTAL_OPERATE_INCOME" : 150560330316.45,  营业总收入
-#     "TOTAL_OPERATE_INCOME_YOY" : 18.0365792459, 总运营收入修正
-#     "OPERATE_INCOME" : 147693604994.14,  营业收入
-#     "OPERATE_INCOME_YOY" : 19.0119185529, 营业收入修正
-#     "INTEREST_INCOME" : 2866725322.31, 利息收入
-#     "INTEREST_INCOME_YOY" : 利息收入修正
-#     "EARNED_PREMIUM" : NaN,
-#     "EARNED_PREMIUM_YOY" : NaN,
-#     "FEE_COMMISSION_INCOME" : NaN,
-#     "FEE_COMMISSION_INCOME_YOY" : NaN,
-#     "OTHER_BUSINESS_INCOME" : NaN,
-#     "OTHER_BUSINESS_INCOME_YOY" : NaN,
-#     "TOI_OTHER" : NaN,
-#     "TOI_OTHER_YOY" : NaN,
-#     "TOTAL_OPERATE_COST" : 46960889468.54, 营业总成本
-#     "TOTAL_OPERATE_COST_YOY" : 18.1456266222,
-#     "OPERATE_COST" : 11867273851.78, 营业成本
-#     "OPERATE_COST_YOY" : 17.5737925437,
-#     "INTEREST_EXPENSE" : 113500129.93, 利息支出
-#     "INTEREST_EXPENSE_YOY" : 7.4972611642,
-#     "FEE_COMMISSION_EXPENSE" : 68578.57,  手续费及佣金支出
-#     "FEE_COMMISSION_EXPENSE_YOY" : -52.0903684752,
-#     "RESEARCH_EXPENSE" : 157371873.01, 研发费用
-#     "RESEARCH_EXPENSE_YOY" : 16.4116440028,
-#     "SURRENDER_VALUE" : NaN,
-#     "SURRENDER_VALUE_YOY" : NaN,
-#     "NET_COMPENSATE_EXPENSE" : NaN,
-#     "NET_COMPENSATE_EXPENSE_YOY" : NaN,
-#     "NET_CONTRACT_RESERVE" : NaN,
-#     "NET_CONTRACT_RESERVE_YOY" : NaN,
-#     "POLICY_BONUS_EXPENSE" : NaN,
-#     "POLICY_BONUS_EXPENSE_YOY" : NaN,
-#     "REINSURE_EXPENSE" : NaN,
-#     "REINSURE_EXPENSE_YOY" : NaN,
-#     "OTHER_BUSINESS_COST" : NaN,
-#     "OTHER_BUSINESS_COST_YOY" : NaN,
-#     "OPERATE_TAX_ADD" : 22234175898.6, 税金及附加
-#     "OPERATE_TAX_ADD_YOY" : 20.2119055043,
-#     "SALE_EXPENSE" : 4648613585.82, 销售费用
-#     "SALE_EXPENSE_YOY" : 40.9642928475,
-#     "MANAGE_EXPENSE" : 9729389252.31, 管理费用
-#     "MANAGE_EXPENSE_YOY" : 7.9580889133,
-#     "ME_RESEARCH_EXPENSE" : NaN,
-#     "ME_RESEARCH_EXPENSE_YOY" : NaN,
-#     "FINANCE_EXPENSE" : -1789503701.48, 财务费用
-#     "FINANCE_EXPENSE_YOY" : -28.5742355094,
-#     "FE_INTEREST_EXPENSE" : 12624628.35, 利息费用
-#     "FE_INTEREST_EXPENSE_YOY" : 5.0021902771,
-#     "FE_INTEREST_INCOME" : 1942301920.98, 利息收入
-#     "FE_INTEREST_INCOME_YOY" : 31.6437955552,
-#     "ASSET_IMPAIRMENT_LOSS" : NaN,
-#     "ASSET_IMPAIRMENT_LOSS_YOY" : NaN,
-#     "CREDIT_IMPAIRMENT_LOSS" : NaN,
-#     "CREDIT_IMPAIRMENT_LOSS_YOY" : NaN,
-#     "TOC_OTHER" : NaN,
-#     "TOC_OTHER_YOY" : NaN,
-#     "FAIRVALUE_CHANGE_INCOME" : 3151962.5, :公允价值变动收益
-#     "FAIRVALUE_CHANGE_INCOME_YOY" : NaN,
-#     "INVEST_INCOME" : 34025967.82, 投资收益
-#     "INVEST_INCOME_YOY" : -46.7011782268,
-#     "INVEST_JOINT_INCOME" : NaN,
-#     "INVEST_JOINT_INCOME_YOY" : NaN,
-#     "NET_EXPOSURE_INCOME" : NaN,
-#     "NET_EXPOSURE_INCOME_YOY" : NaN,
-#     "EXCHANGE_INCOME" : NaN,
-#     "EXCHANGE_INCOME_YOY" : NaN,
-#     "ASSET_DISPOSAL_INCOME" : -479736.97, 资产处置收益
-#     "ASSET_DISPOSAL_INCOME_YOY" : -324.9796785895,
-#     "ASSET_IMPAIRMENT_INCOME" : NaN,
-#     "ASSET_IMPAIRMENT_INCOME_YOY" : NaN,
-#     "CREDIT_IMPAIRMENT_INCOME" : 37871293.26, 信用减值损失(新)
-#     "CREDIT_IMPAIRMENT_INCOME_YOY" : 357.8638477375,
-#     "OTHER_INCOME" : 34644873.86, 其他收益
-#     "OTHER_INCOME_YOY" : 41.3767542405,
-#     "OPERATE_PROFIT_OTHER" : NaN,
-#     "OPERATE_PROFIT_OTHER_YOY" : NaN,
-#     "OPERATE_PROFIT_BALANCE" : 0.0,
-#     "OPERATE_PROFIT_BALANCE_YOY" : NaN,
-#     "OPERATE_PROFIT" : 103708655208.38, 营业利润
-#     "OPERATE_PROFIT_YOY" : 18.0123117479,
-#     "NONBUSINESS_INCOME" : 86779655.95, 加:营业外收入
-#     "NONBUSINESS_INCOME_YOY" : 22.4796849672,
-#     "NONCURRENT_DISPOSAL_INCOME" : NaN,
-#     "NONCURRENT_DISPOSAL_INCOME_YOY" : NaN,
-#     "NONBUSINESS_EXPENSE" : 132881174.52, 减:营业外支出
-#     "NONBUSINESS_EXPENSE_YOY" : -46.6092621953,
-#     "NONCURRENT_DISPOSAL_LOSS" : NaN,
-#     "NONCURRENT_DISPOSAL_LOSS_YOY" : NaN,
-#     "EFFECT_TP_OTHER" : NaN,
-#     "EFFECT_TP_OTHER_YOY" : NaN,
-#     "TOTAL_PROFIT_BALANCE" : 0.0,
-#     "TOTAL_PROFIT_BALANCE_YOY" : NaN,
-#     "TOTAL_PROFIT" : 103662553689.81, 利润总额
-#     "TOTAL_PROFIT_YOY" : 18.1993076599,
-#     "INCOME_TAX" : 26141077412.01, 减:所得税
-#     "INCOME_TAX_YOY" : 17.0909328034,
-#     "EFFECT_NETPROFIT_OTHER" : NaN,
-#     "EFFECT_NETPROFIT_OTHER_YOY" : NaN,
-#     "EFFECT_NETPROFIT_BALANCE" : NaN,
-#     "EFFECT_NETPROFIT_BALANCE_YOY" : NaN,
-#     "UNCONFIRM_INVEST_LOSS" : NaN,
-#     "UNCONFIRM_INVEST_LOSS_YOY" : NaN,
-#     "NETPROFIT" : 77521476277.8, 净利润
-#     "NETPROFIT_YOY" : 18.5778097415,
-#     "PRECOMBINE_PROFIT" : NaN,
-#     "PRECOMBINE_PROFIT_YOY" : NaN,
-#     "CONTINUED_NETPROFIT" : 77521476277.8, 持续经营净利润
-#     "CONTINUED_NETPROFIT_YOY" : 18.5778097415,
-#     "DISCONTINUED_NETPROFIT" : NaN,
-#     "DISCONTINUED_NETPROFIT_YOY" : NaN,
-#     "PARENT_NETPROFIT" : 74734071550.75, 归属于母公司股东的净利润
-#     "PARENT_NETPROFIT_YOY" : 19.1598992892,
-#     "MINORITY_INTEREST" : 2787404727.05,  少数股东损益
-#     "MINORITY_INTEREST_YOY" : 4.8459336455,
-#     "DEDUCT_PARENT_NETPROFIT" : 74752564425.52, 扣除非经常性损益后的净利润
-#     "DEDUCT_PARENT_NETPROFIT_YOY" : 19.0462109566,
-#     "NETPROFIT_OTHER" : NaN,
-#     "NETPROFIT_OTHER_YOY" : NaN,
-#     "NETPROFIT_BALANCE" : NaN,
-#     "NETPROFIT_BALANCE_YOY" : NaN,
-#     "BASIC_EPS" : 59.49,  基本每股收益
-#     "BASIC_EPS_YOY" : 19.1468055277,
-#     "DILUTED_EPS" : 59.49,  稀释每股收益
-#     "DILUTED_EPS_YOY" : 19.1468055277,
-#     "OTHER_COMPRE_INCOME" : 4715179.82, 其他综合收益
-#     "OTHER_COMPRE_INCOME_YOY" : 110.40766101,
-#     "PARENT_OCI" : 4715179.82, 归属于母公司股东的其他综合收益
-#     "PARENT_OCI_YOY" : 110.40766101,
-#     "MINORITY_OCI" : NaN,
-#     "MINORITY_OCI_YOY" : NaN,
-#     "PARENT_OCI_OTHER" : NaN,
-#     "PARENT_OCI_OTHER_YOY" : NaN,
-#     "PARENT_OCI_BALANCE" : NaN,
-#     "PARENT_OCI_BALANCE_YOY" : NaN,
-#     "UNABLE_OCI" : NaN,
-#     "UNABLE_OCI_YOY" : NaN,
-#     "CREDITRISK_FAIRVALUE_CHANGE" : NaN,
-#     "CREDITRISK_FAIRVALUE_CHANGE_YOY" : NaN,
-#     "OTHERRIGHT_FAIRVALUE_CHANGE" : NaN,
-#     "OTHERRIGHT_FAIRVALUE_CHANGE_YOY" : NaN,
-#     "SETUP_PROFIT_CHANGE" : NaN,
-#     "SETUP_PROFIT_CHANGE_YOY" : NaN,
-#     "RIGHTLAW_UNABLE_OCI" : NaN,
-#     "RIGHTLAW_UNABLE_OCI_YOY" : NaN,
-#     "UNABLE_OCI_OTHER" : NaN,
-#     "UNABLE_OCI_OTHER_YOY" : NaN,
-#     "UNABLE_OCI_BALANCE" : NaN,
-#     "UNABLE_OCI_BALANCE_YOY" : NaN,
-#     "ABLE_OCI" : 4715179.82,
-#     "ABLE_OCI_YOY" : 110.40766101,
-#     "RIGHTLAW_ABLE_OCI" : NaN,
-#     "RIGHTLAW_ABLE_OCI_YOY" : NaN,
-#     "AFA_FAIRVALUE_CHANGE" : NaN,
-#     "AFA_FAIRVALUE_CHANGE_YOY" : NaN,
-#     "HMI_AFA" : NaN,
-#     "HMI_AFA_YOY" : NaN,
-#     "CASHFLOW_HEDGE_VALID" : NaN,
-#     "CASHFLOW_HEDGE_VALID_YOY" : NaN,
-#     "CREDITOR_FAIRVALUE_CHANGE" : NaN,
-#     "CREDITOR_FAIRVALUE_CHANGE_YOY" : NaN,
-#     "CREDITOR_IMPAIRMENT_RESERVE" : NaN,
-#     "CREDITOR_IMPAIRMENT_RESERVE_YOY" : NaN,
-#     "FINANCE_OCI_AMT" : NaN,
-#     "FINANCE_OCI_AMT_YOY" : NaN,
-#     "CONVERT_DIFF" : 4715179.82,
-#     "CONVERT_DIFF_YOY" : 110.40766101,
-#     "ABLE_OCI_OTHER" : NaN,
-#     "ABLE_OCI_OTHER_YOY" : NaN,
-#     "ABLE_OCI_BALANCE" : NaN,
-#     "ABLE_OCI_BALANCE_YOY" : NaN,
-#     "OCI_OTHER" : NaN,
-#     "OCI_OTHER_YOY" : NaN,
-#     "OCI_BALANCE" : NaN,
-#     "OCI_BALANCE_YOY" : NaN,
-#     "TOTAL_COMPRE_INCOME" : 77526191457.62, 综合收益总额
-#     "TOTAL_COMPRE_INCOME_YOY" : 18.5809573963,
-#     "PARENT_TCI" : 74738786730.57, 归属于母公司股东的综合收益总额
-#     "PARENT_TCI_YOY" : 19.1631595692,
-#     "MINORITY_TCI" : 2787404727.05,  归属于少数股东的综合收益总额
-#     "MINORITY_TCI_YOY" : 4.8459336455,
-#     "PRECOMBINE_TCI" : NaN,
-#     "PRECOMBINE_TCI_YOY" : NaN,
-#     "EFFECT_TCI_BALANCE" : NaN,
-#     "EFFECT_TCI_BALANCE_YOY" : NaN,
-#     "TCI_OTHER" : NaN,
-#     "TCI_OTHER_YOY" : NaN,
-#     "TCI_BALANCE" : NaN,
-#     "TCI_BALANCE_YOY" : NaN,
-#     "ACF_END_INCOME" : NaN,
-#     "ACF_END_INCOME_YOY" : NaN,
-#     "OPINION_TYPE" : "标准无保留意见" 审计意见(境内)
-# https://emweb.securities.eastmoney.com/PC_HSF10/NewFinanceAnalysis/Index?type=web&code=sh600519#lrb-0
-def get_em_benefit_api(symbol):
-    stock_financial_benefit_ths_df = ak.stock_profit_sheet_by_report_em(symbol)
-    stock_financial_benefit_ths_df = stock_financial_benefit_ths_df[[
-        "SECUCODE",
-        "SECURITY_CODE",
-        "SECURITY_NAME_ABBR",
-        "ORG_CODE",
-        "ORG_TYPE",
-        "REPORT_DATE",
-        "REPORT_TYPE",
-        "REPORT_DATE_NAME",
-        "SECURITY_TYPE_CODE",
-        "NOTICE_DATE",
-        "UPDATE_DATE",
-        "CURRENCY",
-        "TOTAL_OPERATE_INCOME",
-        "OPERATE_INCOME",
-        "INTEREST_INCOME",
-        "TOTAL_OPERATE_COST",
-        "OPERATE_COST",
-        "INTEREST_EXPENSE",
-        "FEE_COMMISSION_EXPENSE",
-        "RESEARCH_EXPENSE",
-        "OPERATE_TAX_ADD",
-        "SALE_EXPENSE",
-        "MANAGE_EXPENSE",
-        "FINANCE_EXPENSE",
-        "FE_INTEREST_EXPENSE",
-        "FE_INTEREST_INCOME",
-        "FAIRVALUE_CHANGE_INCOME",
-        "INVEST_INCOME",
-        "ASSET_DISPOSAL_INCOME",
-        "CREDIT_IMPAIRMENT_INCOME",
-        "OTHER_INCOME",
-        "OPERATE_PROFIT",
-        "NONBUSINESS_INCOME",
-        "NONBUSINESS_EXPENSE",
-        "TOTAL_PROFIT",
-        "INCOME_TAX",
-        "NETPROFIT",
-        "CONTINUED_NETPROFIT",
-        "PARENT_NETPROFIT",
-        'MINORITY_INTEREST',
-        'DEDUCT_PARENT_NETPROFIT',
-        'BASIC_EPS',
-        'DILUTED_EPS',
-        'OTHER_COMPRE_INCOME',
-        'PARENT_OCI',
-        'TOTAL_COMPRE_INCOME',
-        'PARENT_TCI',
-        'MINORITY_TCI',
-        'OPINION_TYPE'
-    ]]
-    mongodb_util.insert_mongo(stock_financial_benefit_ths_df, 'stock_financial_benefit_ths_df')
-    return stock_financial_benefit_ths_df
+    query = {'SECURITY_CODE': symbol}
+    exist_asset_em_df = mongodb_util.find_query_data(db_name_constant.EM_STOCK_ASSET_LIABILITY, query)
+    if data_frame_util.is_not_empty(exist_asset_em_df):
+        new_asset_df = stock_balance_sheet_by_report_em_df.loc[
+            ~(stock_balance_sheet_by_report_em_df['SECURITY_CODE'].isin(list(exist_asset_em_df['SECURITY_CODE'])))]
+    else:
+        new_asset_df = stock_balance_sheet_by_report_em_df
+    if data_frame_util.is_empty(new_asset_df):
+        return None
+    new_asset_df.fillna(0, inplace=True)
+    mongodb_util.insert_mongo(new_asset_df, db_name_constant.EM_STOCK_ASSET_LIABILITY)
 
 
 if __name__ == '__main__':
-    get_em_benefit_api('SH600519')
-    get_em_debt_api('SH600519')
+    get_em_asset_liability_api('832876')
 
     stock_cash_flow_sheet_by_report_em_df = ak.stock_cash_flow_sheet_by_report_em(symbol="SH600519")
     print(stock_cash_flow_sheet_by_report_em_df)
```

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.4.8/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.4.8/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.4.8/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.4.8/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.4.8/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/risk/register_and_investigate_stock_sync_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/risk/register_and_investigate_stock_sync_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,15 +101,16 @@
                     key_id,
                     symbol,
                     high_risk_stocks_one.secName,
                     announce_str_day,
                     announce_time,
                     high_risk_stocks_one.announcementTitle,
                     high_risk_stocks_one.announcementTitle,
-                    announce_url)
+                    announce_url,
+                    black_list_service_api.REGISTER_INVESTIGATE)
         except Exception as e:
             logger.error("保存风险警示股票异常:{},{}", symbol, e)
 
 
 if __name__ == '__main__':
     sync_new_high_risk_stocks()
     result_df = sync_all_investigate_stocks(30, '立案', '2023-01-01', '2024-05-15')
```

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.4.8/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.4.8/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.4.8/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.4.8/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.4.8/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.4.8/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.7/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.4.8/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -35,15 +35,19 @@
 mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
 mns_scheduler/db/__init__.py
 mns_scheduler/db/col_move_service.py
 mns_scheduler/db/db_status.py
 mns_scheduler/dt/__init__.py
 mns_scheduler/dt/stock_dt_pool_sync.py
 mns_scheduler/finance/__init__.py
-mns_scheduler/finance/em_financial_sync_service_api.py
+mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
+mns_scheduler/finance/em_financial_profit_sync_service_api.py
+mns_scheduler/finance/finance_common_api.py
+mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
+mns_scheduler/finance/sync_financial_report_service_api.py
 mns_scheduler/k_line/__init__.py
 mns_scheduler/k_line/clean/__init__.py
 mns_scheduler/k_line/clean/k_line_info_clean_impl.py
 mns_scheduler/k_line/clean/k_line_info_clean_service.py
 mns_scheduler/k_line/sync/__init__.py
 mns_scheduler/k_line/sync/daily_week_month_line_sync.py
 mns_scheduler/kpl/__init__.py
```

