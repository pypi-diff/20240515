# Comparing `tmp/mns-scheduler-1.0.4.5.tar.gz` & `tmp/mns-scheduler-1.0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.4.5.tar", last modified: Thu May  9 14:49:30 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.4.6.tar", last modified: Tue May 14 08:14:46 2024, max compression
```

## Comparing `mns-scheduler-1.0.4.5.tar` & `mns-scheduler-1.0.4.6.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.769423 mns-scheduler-1.0.4.5/
--rw-rw-rw-   0        0        0       62 2024-05-09 14:49:30.768427 mns-scheduler-1.0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.730136 mns-scheduler-1.0.4.5/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.732131 mns-scheduler-1.0.4.5/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.733128 mns-scheduler-1.0.4.5/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.735123 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.736120 mns-scheduler-1.0.4.5/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.737657 mns-scheduler-1.0.4.5/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.739161 mns-scheduler-1.0.4.5/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.740158 mns-scheduler-1.0.4.5/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.741155 mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.742153 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.743151 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.745145 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.746960 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.748950 mns-scheduler-1.0.4.5/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-04-30 07:00:04.000000 mns-scheduler-1.0.4.5/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.748950 mns-scheduler-1.0.4.5/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.749947 mns-scheduler-1.0.4.5/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-05 14:54:50.000000 mns-scheduler-1.0.4.5/mns_scheduler/finance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.749947 mns-scheduler-1.0.4.5/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.751941 mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.752938 mns-scheduler-1.0.4.5/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.753935 mns-scheduler-1.0.4.5/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.753935 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.755930 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.756927 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.757924 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.759921 mns-scheduler-1.0.4.5/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.5/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.761915 mns-scheduler-1.0.4.5/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.5/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.5/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.5/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.762912 mns-scheduler-1.0.4.5/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.765434 mns-scheduler-1.0.4.5/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.767428 mns-scheduler-1.0.4.5/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    15670 2024-05-09 08:01:31.000000 mns-scheduler-1.0.4.5/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.768427 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-09 14:49:30.000000 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3334 2024-05-09 14:49:30.000000 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 14:49:30.000000 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-09 14:49:30.000000 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 14:49:30.769423 mns-scheduler-1.0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-09 14:49:28.000000 mns-scheduler-1.0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.752375 mns-scheduler-1.0.4.6/
+-rw-rw-rw-   0        0        0       62 2024-05-14 08:14:46.752375 mns-scheduler-1.0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.717468 mns-scheduler-1.0.4.6/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.719463 mns-scheduler-1.0.4.6/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.720460 mns-scheduler-1.0.4.6/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.722455 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.723452 mns-scheduler-1.0.4.6/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.724450 mns-scheduler-1.0.4.6/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.725447 mns-scheduler-1.0.4.6/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15735 2024-05-13 09:25:17.000000 mns-scheduler-1.0.4.6/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20342 2024-05-13 09:29:51.000000 mns-scheduler-1.0.4.6/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.726444 mns-scheduler-1.0.4.6/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.727449 mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.727449 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.729436 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.730434 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.732428 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.733426 mns-scheduler-1.0.4.6/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.4.6/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.734423 mns-scheduler-1.0.4.6/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.735420 mns-scheduler-1.0.4.6/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-05 14:54:50.000000 mns-scheduler-1.0.4.6/mns_scheduler/finance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.735420 mns-scheduler-1.0.4.6/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.737415 mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.738412 mns-scheduler-1.0.4.6/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.738412 mns-scheduler-1.0.4.6/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.738412 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.740407 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.741404 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.742402 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.743399 mns-scheduler-1.0.4.6/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.6/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.745394 mns-scheduler-1.0.4.6/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.6/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.6/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.6/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.746391 mns-scheduler-1.0.4.6/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.749383 mns-scheduler-1.0.4.6/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17272 2024-05-11 03:32:32.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-09 15:06:22.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.751378 mns-scheduler-1.0.4.6/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    15670 2024-05-09 08:01:31.000000 mns-scheduler-1.0.4.6/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.752375 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-14 08:14:46.000000 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3334 2024-05-14 08:14:46.000000 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:14:46.000000 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 08:14:46.000000 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:14:46.753372 mns-scheduler-1.0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-14 08:14:23.000000 mns-scheduler-1.0.4.6/setup.py
```

### Comparing `mns-scheduler-1.0.4.5/README.md` & `mns-scheduler-1.0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.4.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.4.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.4.6/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.4.6/mns_scheduler/company_info/company_constant_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 17
 project_path = file_path[0:end]
 sys.path.append(project_path)
 import pandas as pd
 from mns_common.db.MongodbUtil import MongodbUtil
+import mns_common.utils.data_frame_util as data_frame_util
 
 mongodb_util = MongodbUtil('27017')
 
 # 退市股票
 de_listed_stock_list = [
     "002018",
     "600240",
@@ -104,18 +105,40 @@
     '300836',
     '300293',
     '688630',
     '001309',
     '600338',
     '000032',
     '300042',
-    '300295'
+    '300295',
+    '300483'
 ]
 
 
+def get_fix_symbol_industry():
+    return pd.DataFrame([['688480', '赛恩斯', '760103', '环境治理'],
+                         ['000032', '深桑达Ａ', '730200', '通信网络设备及器件'],
+                         ['688480', '赛恩斯', '640704', '自动化设备'],
+                         ['603260', '合盛硅业', '220316', '有机硅'],
+                         ['300559', '佳发教育', '461102', '培训教育'],
+                         ['300836', '佰奥智能', '640701', '机器人'],
+                         ['300293', '蓝英装备', '640701', '机器人'],
+                         ['688630', '芯碁微装', '270108', '半导体设备'],
+                         ['001309', '德明利', '270108', '半导体设备'],
+                         ['600338', '西藏珠峰', '240603', '锂'],
+                         ['300042', '朗科科技', '270108', '半导体设备'],
+                         ['688507', '索辰科技', '710402', '横向通用软件'],
+                         ['301387', '光大同创', '270504', '消费电子零部件及组装'],
+                         ['300295', '三六五网', '430300', '物业管理'],
+                         ['300947', '德必集团', '430300', '物业管理'],
+                         ['300483', '首华燃气', '410301', '燃气Ⅲ'],
+                         ],
+                        columns=['symbol', 'name', 'new_industry_code', 'new_industry'])
+
+
 def get_industry_final_fix_df():
     return pd.DataFrame([
         # 汽车
         ['汽车零部件', '汽车零部件'],
         ['汽车服务', '汽车服务'],
         ['乘用车', '汽车整车'],  # = merge 汽车整车
         ['商用车', '汽车整车'],
@@ -370,59 +393,25 @@
     company_info['second_industry_code'] = sw_industry.second_industry_code
     company_info['third_sw_industry'] = sw_industry.third_sw_industry
     company_info['third_industry_code'] = sw_industry.industry_code
     return company_info
 
 
 def fix_symbol_industry(company_info, symbol):
-    if symbol == '688480':
-        company_info = fix_industry_data('760103', company_info)
-    if symbol == '000032':
-        company_info = fix_industry_data('730204', company_info)
-
-    if symbol == '301112':
-        company_info = fix_industry_data('640209', company_info)
-
-    if symbol == '603260':
-        company_info = fix_industry_data('220316', company_info)
-
-    if symbol == '300559':
-        company_info = fix_industry_data('461102', company_info)
-
-    if symbol == '300836':
-        company_info = fix_industry_data('640701', company_info)
-
-    if symbol == '300293':
-        company_info = fix_industry_data('640701', company_info)
-    if symbol == '688630':
-        company_info = fix_industry_data('270108', company_info)
-
-    if symbol == '001309':
-        company_info = fix_industry_data('270108', company_info)
-
-    if symbol == '600338':
-        company_info = fix_industry_data('240603', company_info)
-
-    if symbol == '300042':
-        company_info = fix_industry_data('270100', company_info)
-
-    if symbol == '688507':
-        company_info = fix_industry_data('710402', company_info)
-
-    if symbol == '301387':
-        company_info = fix_industry_data('270504', company_info)
-    # 修改到房地产行业
-    if symbol == '300295':
-        company_info = fix_industry_data('430301', company_info)
+    fix_symbol_df = get_fix_symbol_industry()
+    fix_symbol_df_one = fix_symbol_df.loc[fix_symbol_df['symbol'] == symbol]
+    if data_frame_util.is_not_empty(fix_symbol_df_one):
+        new_industry_code = list(fix_symbol_df_one['new_industry_code'])[0]
+        company_info = fix_industry_data(new_industry_code, company_info)
 
     return company_info
 
 
 def fix_one_symbol():
-    symbol = '301387'
+    symbol = '300483'
     company_info = mongodb_util.find_query_data('company_info', query={'_id': symbol})
     company_info = fix_symbol_industry(company_info, symbol)
     company_info['industry'] = company_info['second_sw_industry']
     mongodb_util.save_mongo(company_info, 'company_info')
 
 
 if __name__ == '__main__':
```

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,10 +466,10 @@
     # sync_company_base_info()
     # fix_company_industry()
     # calculate_circu_ratio("601069")
     # sync_company_base_info()
     # 300293
     # sync_company_base_info(None)
     # new_company_info_update()
-    sync_company_base_info(None)
-    fix_company_industry(None)
+    sync_company_base_info(['300483'])
+    fix_company_industry('300483')
     # group_by_industry()
```

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.4.6/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.4.6/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.4.6/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.4.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         mongodb_util.create_index(db_name, [("symbol", 1), ("date", 1)])
         logger.info("创建索引成功:{}", db_name)
     except BaseException as e:
         logger.warning("创建索引异常:{}", e)
 
 
 if __name__ == '__main__':
-    # sync_all_daily_data('daily', 'qfq', 'stock_qfq_daily', None, None)
-    # sync_all_daily_data('weekly', 'qfq', 'stock_qfq_weekly', None, None)
-    sync_all_daily_data('monthly', 'qfq', 'stock_qfq_monthly', None, None)
+    sync_all_daily_data('daily', 'qfq', 'stock_qfq_daily', None, None)
+    sync_all_daily_data('weekly', 'qfq', 'stock_qfq_weekly', None, None)
+    # sync_all_daily_data('monthly', 'qfq', 'stock_qfq_monthly', None, None)
 
     # sync_all_daily_data('monthly', '1990-12-19', 'qfq', 'stock_qfq_monthly', None, None)
     # sync_all_daily_data('daily', '1990-12-19', 'qfq', 'stock_qfq_daily', '2023-10-31', None)
     # sync_all_daily_data('weekly', '1990-12-19', 'qfq', 'stock_qfq_weekly', '2023-10-15', None)
     # sync_all_daily_data('monthly', '1990-12-19', 'qfq', 'stock_qfq_monthly', '2023-09-30', None)
```

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.4.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.4.6/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.4.6/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.4.6/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.4.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
             miss_symbol_list = list(stock_high_chg_pool_df['symbol'])
             sync_all_kc_zt_data(str_day, miss_symbol_list)
         except BaseException as e:
             logger.error("发生异常:{},{}", str_day, e)
 
 
 if __name__ == '__main__':
-    sync_all_high_chg_data('2024-03-08')
+    sync_all_kc_zt_data('2024-05-10', None)
     # sync_all_kc_zt_data('2023-08-16')
     # sync_all_kc_zt_data('2023-07-07')
     # realtime_quotes_now_zt_new_kc_open_sync()
     # hui_ce_all('2023-06-16')
     # fix_diff_day()
     # sync_all_kc_zt_data('2023-06-30')
```

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.4.6/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 
         # del stock_em_zt_pool_df_data['ths_concept_name']
         # del stock_em_zt_pool_df_data['ths_concept_code']
 
         for stock_one in stock_em_zt_pool_df_data.itertuples():
             try:
                 stock_em_zt_pool_df_data = ths_concept_common_service_api.set_last_ths_concept(stock_one.symbol,
-                                                                                           stock_em_zt_pool_df_data,
-                                                                                           str_day)
+                                                                                               stock_em_zt_pool_df_data,
+                                                                                               str_day)
                 ths_zt_pool_one_df = ths_zt_pool_df_data.loc[ths_zt_pool_df_data['symbol'] == stock_one.symbol]
                 if data_frame_util.is_empty(ths_zt_pool_one_df):
                     continue
                 stock_em_zt_pool_df_data.loc[stock_em_zt_pool_df_data['symbol'] == stock_one.symbol, 'zt_reason'] = \
                     list(ths_zt_pool_one_df['zt_reason'])[0]
 
                 stock_em_zt_pool_df_data.loc[stock_em_zt_pool_df_data['symbol'] == stock_one.symbol, 'quantity_ratio'] = \
@@ -122,14 +122,17 @@
     stock_em_zt_pool_df_data['str_day'] = str_day
     stock_em_zt_pool_df_data['_id'] = stock_em_zt_pool_df_data['symbol'] + "_" + str_day
 
     stock_em_zt_pool_df_data = stock_em_zt_pool_df_data[ZT_FIELD]
     mongodb_util.save_mongo(stock_em_zt_pool_df_data, 'stock_zt_pool')
     return stock_em_zt_pool_df_data
 
+
+if __name__ == '__main__':
+    save_zt_info('2024-05-07')
 # from datetime import datetime
 #
 # if __name__ == '__main__':
 #
 #     sync_date = date_handle_util.add_date_day('20240110', 0)
 #
 #     now_date = datetime.now()
```

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.4.6/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.4.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.5/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.4.6/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

