# Comparing `tmp/mns-scheduler-1.0.4.6.tar.gz` & `tmp/mns-scheduler-1.0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.4.6.tar", last modified: Tue May 14 08:14:46 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.4.7.tar", last modified: Wed May 15 07:01:38 2024, max compression
```

## Comparing `mns-scheduler-1.0.4.6.tar` & `mns-scheduler-1.0.4.7.tar`

### file list

```diff
@@ -1,107 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.752375 mns-scheduler-1.0.4.6/
--rw-rw-rw-   0        0        0       62 2024-05-14 08:14:46.752375 mns-scheduler-1.0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.717468 mns-scheduler-1.0.4.6/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.719463 mns-scheduler-1.0.4.6/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.720460 mns-scheduler-1.0.4.6/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.722455 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.723452 mns-scheduler-1.0.4.6/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.724450 mns-scheduler-1.0.4.6/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.725447 mns-scheduler-1.0.4.6/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15735 2024-05-13 09:25:17.000000 mns-scheduler-1.0.4.6/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20342 2024-05-13 09:29:51.000000 mns-scheduler-1.0.4.6/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.726444 mns-scheduler-1.0.4.6/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.727449 mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.727449 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.729436 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.730434 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.732428 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.733426 mns-scheduler-1.0.4.6/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.4.6/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.734423 mns-scheduler-1.0.4.6/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.735420 mns-scheduler-1.0.4.6/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-05 14:54:50.000000 mns-scheduler-1.0.4.6/mns_scheduler/finance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.735420 mns-scheduler-1.0.4.6/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.737415 mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.738412 mns-scheduler-1.0.4.6/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.4.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.738412 mns-scheduler-1.0.4.6/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.738412 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.740407 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.741404 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.742402 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.743399 mns-scheduler-1.0.4.6/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.6/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.745394 mns-scheduler-1.0.4.6/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.6/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.6/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.6/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.746391 mns-scheduler-1.0.4.6/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.749383 mns-scheduler-1.0.4.6/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17272 2024-05-11 03:32:32.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7604 2024-05-09 15:06:22.000000 mns-scheduler-1.0.4.6/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.751378 mns-scheduler-1.0.4.6/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    15670 2024-05-09 08:01:31.000000 mns-scheduler-1.0.4.6/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:14:46.752375 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-14 08:14:46.000000 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3334 2024-05-14 08:14:46.000000 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:14:46.000000 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 08:14:46.000000 mns-scheduler-1.0.4.6/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 08:14:46.753372 mns-scheduler-1.0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-14 08:14:23.000000 mns-scheduler-1.0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.483652 mns-scheduler-1.0.4.7/
+-rw-rw-rw-   0        0        0       62 2024-05-15 07:01:38.482655 mns-scheduler-1.0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.447748 mns-scheduler-1.0.4.7/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-05-15 00:08:32.000000 mns-scheduler-1.0.4.7/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.449744 mns-scheduler-1.0.4.7/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.449744 mns-scheduler-1.0.4.7/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.452735 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.453732 mns-scheduler-1.0.4.7/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.453732 mns-scheduler-1.0.4.7/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.455727 mns-scheduler-1.0.4.7/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15735 2024-05-13 09:25:17.000000 mns-scheduler-1.0.4.7/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20342 2024-05-13 09:29:51.000000 mns-scheduler-1.0.4.7/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.455727 mns-scheduler-1.0.4.7/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.457722 mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.457722 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.459717 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.460714 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.462708 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.463706 mns-scheduler-1.0.4.7/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.4.7/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.464703 mns-scheduler-1.0.4.7/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.465700 mns-scheduler-1.0.4.7/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-14 13:59:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/finance/__init__.py
+-rw-rw-rw-   0        0        0    26721 2024-05-15 06:18:00.000000 mns-scheduler-1.0.4.7/mns_scheduler/finance/em_financial_sync_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.465700 mns-scheduler-1.0.4.7/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.467695 mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.468692 mns-scheduler-1.0.4.7/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.4.7/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.468692 mns-scheduler-1.0.4.7/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.469690 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.470687 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.471684 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.472682 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.473679 mns-scheduler-1.0.4.7/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.7/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.474677 mns-scheduler-1.0.4.7/mns_scheduler/risk/
+-rw-rw-rw-   0        0        0      163 2024-05-14 14:32:33.000000 mns-scheduler-1.0.4.7/mns_scheduler/risk/__init__.py
+-rw-rw-rw-   0        0        0     4883 2024-05-15 00:18:26.000000 mns-scheduler-1.0.4.7/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.476672 mns-scheduler-1.0.4.7/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.7/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.7/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.7/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.477669 mns-scheduler-1.0.4.7/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.480661 mns-scheduler-1.0.4.7/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17272 2024-05-11 03:32:32.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-09 15:06:22.000000 mns-scheduler-1.0.4.7/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.482655 mns-scheduler-1.0.4.7/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    16100 2024-05-14 16:54:03.000000 mns-scheduler-1.0.4.7/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.7/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:01:38.482655 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-15 07:01:38.000000 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3482 2024-05-15 07:01:38.000000 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 07:01:38.000000 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 07:01:38.000000 mns-scheduler-1.0.4.7/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 07:01:38.483652 mns-scheduler-1.0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-15 07:01:25.000000 mns-scheduler-1.0.4.7/setup.py
```

### Comparing `mns-scheduler-1.0.4.6/README.md` & `mns-scheduler-1.0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.4.7/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.4.7/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.4.7/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.4.7/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.4.7/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.4.7/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.4.7/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.4.7/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.4.7/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.4.7/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.4.7/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.4.7/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.4.7/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.4.7/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.4.7/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.4.7/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.4.7/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 17
 project_path = file_path[0:end]
 sys.path.append(project_path)
 
+import mns_scheduler.risk.register_and_investigate_stock_sync_api as register_and_investigate_stock_sync_api
 from loguru import logger
 from apscheduler.schedulers.blocking import BlockingScheduler
 from datetime import datetime
 import mns_scheduler.dt.stock_dt_pool_sync as stock_dt_pool_sync_api
 import mns_scheduler.zb.stock_zb_pool_sync as stock_zb_pool_sync_api
 import mns_common.component.trade_date.trade_date_common_service_api as trade_date_common_service_api
 import mns_common.utils.date_handle_util as date_handle_util
@@ -308,14 +309,20 @@
     str_day = now_date.strftime('%Y-%m-%d')
     last_trade_day = trade_date_common_service_api.get_last_trade_day(str_day)
     if trade_date_common_service_api.is_trade_day(last_trade_day):
         sync_best_choose_his_index.sync_best_choose_his_index(last_trade_day)
         logger.info('同步开盘啦当日精选指数行情数据任务完成')
 
 
+# 同步被立案调查的股票
+def sync_new_high_risk_stocks():
+    logger.info('同步被立案调查的股票')
+    register_and_investigate_stock_sync_api.sync_new_high_risk_stocks()
+
+
 # # 定义BlockingScheduler
 blockingScheduler = BlockingScheduler()
 # sync_trade_date 同步交易日期
 blockingScheduler.add_job(sync_trade_date, 'cron', hour='20', minute='43')
 
 # 跌停信息同步
 blockingScheduler.add_job(sync_stock_dt_pool, 'cron', hour='15,17,21,03,07', minute='37')
@@ -380,12 +387,15 @@
 
 # 更新开盘啦指数关系
 blockingScheduler.add_job(sync_kpl_best_his_quotes, 'cron', hour='18,22', minute='25')
 
 # 更新开盘啦指数关系
 blockingScheduler.add_job(sync_position, 'cron', hour='0,08', minute='10')
 
+# 同步被立案调查的股票
+blockingScheduler.add_job(sync_new_high_risk_stocks, 'cron', hour='0,09', minute='20')
+
 print('定时任务启动成功')
 blockingScheduler.start()
 #
 # if __name__ == '__main__':
 #     sync_kpl_best_his_quotes()
```

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.4.7/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.6/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.4.7/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
 mns_scheduler/db/__init__.py
 mns_scheduler/db/col_move_service.py
 mns_scheduler/db/db_status.py
 mns_scheduler/dt/__init__.py
 mns_scheduler/dt/stock_dt_pool_sync.py
 mns_scheduler/finance/__init__.py
+mns_scheduler/finance/em_financial_sync_service_api.py
 mns_scheduler/k_line/__init__.py
 mns_scheduler/k_line/clean/__init__.py
 mns_scheduler/k_line/clean/k_line_info_clean_impl.py
 mns_scheduler/k_line/clean/k_line_info_clean_service.py
 mns_scheduler/k_line/sync/__init__.py
 mns_scheduler/k_line/sync/daily_week_month_line_sync.py
 mns_scheduler/kpl/__init__.py
@@ -53,14 +54,16 @@
 mns_scheduler/kpl/selection/symbol/__init__.py
 mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
 mns_scheduler/kpl/selection/total/__init__.py
 mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
 mns_scheduler/real_time/__init__.py
 mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
 mns_scheduler/real_time/realtime_quotes_now_sync.py
+mns_scheduler/risk/__init__.py
+mns_scheduler/risk/register_and_investigate_stock_sync_api.py
 mns_scheduler/trade/__init__.py
 mns_scheduler/trade/auto_ipo_buy_api.py
 mns_scheduler/trade/auto_sell_service_api.py
 mns_scheduler/trade/sync_position_api.py
 mns_scheduler/zb/__init__.py
 mns_scheduler/zb/stock_zb_pool_sync.py
 mns_scheduler/zt/__init__.py
```

