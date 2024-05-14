# Comparing `tmp/fudstop-2.5.9.tar.gz` & `tmp/fudstop-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fudstop-2.5.9.tar", last modified: Wed May  8 05:05:07 2024, max compression
+gzip compressed data, was "fudstop-2.6.0.tar", last modified: Tue May 14 22:43:10 2024, max compression
```

## Comparing `fudstop-2.5.9.tar` & `fudstop-2.6.0.tar`

### file list

```diff
@@ -1,362 +1,367 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.592007 fudstop-2.5.9/
--rw-rw-rw-   0        0        0     7618 2024-05-08 05:05:07.591007 fudstop-2.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2024-01-05 23:27:36.000000 fudstop-2.5.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.349257 fudstop-2.5.9/app/
--rw-rw-rw-   0        0        0    43348 2024-01-23 23:29:23.000000 fudstop-2.5.9/app/__init__.py
--rw-rw-rw-   0        0        0     4011 2024-01-12 03:32:55.000000 fudstop-2.5.9/app/fetcher.py
--rw-rw-rw-   0        0        0    17884 2024-01-12 06:07:09.000000 fudstop-2.5.9/app/fudstop_info.py
--rw-rw-rw-   0        0        0    38553 2024-01-12 03:47:25.000000 fudstop-2.5.9/app/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.361545 fudstop-2.5.9/fudstop/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.414939 fudstop-2.5.9/fudstop/_markets/
--rw-rw-rw-   0        0        0     1327 2024-01-18 15:18:48.000000 fudstop-2.5.9/fudstop/_markets/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-02-22 04:18:16.000000 fudstop-2.5.9/fudstop/_markets/analyzers.py
--rw-rw-rw-   0        0        0    67237 2024-02-07 15:09:55.000000 fudstop-2.5.9/fudstop/_markets/embeddings.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.418081 fudstop-2.5.9/fudstop/_markets/finished/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:49:02.000000 fudstop-2.5.9/fudstop/_markets/finished/__init__.py
--rw-rw-rw-   0        0        0    25622 2024-01-21 19:47:09.000000 fudstop-2.5.9/fudstop/_markets/finished/db_manager.py
--rw-rw-rw-   0        0        0     2530 2023-10-12 23:34:06.000000 fudstop-2.5.9/fudstop/_markets/finished/economic_data.py
--rw-rw-rw-   0        0        0    53472 2024-02-11 04:30:33.000000 fudstop-2.5.9/fudstop/_markets/finished/master_class.py
--rw-rw-rw-   0        0        0     9940 2024-01-25 21:35:47.000000 fudstop-2.5.9/fudstop/_markets/finished/td9_states.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.422081 fudstop-2.5.9/fudstop/_markets/list_sets/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/_markets/list_sets/__init__.py
--rw-rw-rw-   0        0        0    92394 2024-02-22 03:17:43.000000 fudstop-2.5.9/fudstop/_markets/list_sets/dicts.py
--rw-rw-rw-   0        0        0    88831 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/_markets/list_sets/saved_tickers.py
--rw-rw-rw-   0        0        0   125429 2024-01-17 16:34:32.000000 fudstop-2.5.9/fudstop/_markets/list_sets/ticker_lists.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.429151 fudstop-2.5.9/fudstop/_markets/market_handlers/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/__init__.py
--rw-rw-rw-   0        0        0     1265 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/cfg.py
--rw-rw-rw-   0        0        0     1491 2024-01-09 04:43:27.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/crypto.py
--rw-rw-rw-   0        0        0    17424 2024-02-12 18:43:10.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/database_.py
--rw-rw-rw-   0        0        0      768 2024-01-09 05:02:23.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/forex.py
--rw-rw-rw-   0        0        0     1770 2024-01-08 17:15:06.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/indices.py
--rw-rw-rw-   0        0        0   762960 2024-01-11 23:53:54.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/list_sets.py
--rw-rw-rw-   0        0        0    13155 2024-01-11 17:06:04.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/options.py
--rw-rw-rw-   0        0        0     3929 2024-01-09 21:38:56.000000 fudstop-2.5.9/fudstop/_markets/market_handlers/stocks.py
--rw-rw-rw-   0        0        0     1166 2024-01-12 17:40:54.000000 fudstop-2.5.9/fudstop/_markets/monitor.py
--rw-rw-rw-   0        0        0    31105 2024-02-12 14:30:27.000000 fudstop-2.5.9/fudstop/_markets/multimarkets.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.430153 fudstop-2.5.9/fudstop/_markets/plotting/
--rw-rw-rw-   0        0        0     1814 2024-01-13 01:48:40.000000 fudstop-2.5.9/fudstop/_markets/plotting/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.431152 fudstop-2.5.9/fudstop/_markets/reference_markets/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/_markets/reference_markets/__init__.py
--rw-rw-rw-   0        0        0     1400 2024-01-08 00:31:15.000000 fudstop-2.5.9/fudstop/_markets/reference_markets/conditional_scans.py
--rw-rw-rw-   0        0        0     8389 2024-01-10 04:38:30.000000 fudstop-2.5.9/fudstop/_markets/reference_markets/reference_market.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.439667 fudstop-2.5.9/fudstop/_markets/scripts/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/_markets/scripts/__init__.py
--rw-rw-rw-   0        0        0      846 2024-01-20 18:45:32.000000 fudstop-2.5.9/fudstop/_markets/scripts/all_polygon_options.py
--rw-rw-rw-   0        0        0      683 2024-01-07 06:56:40.000000 fudstop-2.5.9/fudstop/_markets/scripts/all_webull_options.py
--rw-rw-rw-   0        0        0     1208 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/_markets/scripts/generation.py
--rw-rw-rw-   0        0        0     1351 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/_markets/scripts/million_dollar_trades.py
--rw-rw-rw-   0        0        0     1533 2024-01-18 14:58:07.000000 fudstop-2.5.9/fudstop/_markets/scripts/option_scripts.py
--rw-rw-rw-   0        0        0    20845 2024-01-20 18:50:03.000000 fudstop-2.5.9/fudstop/_markets/scripts/options_market.py
--rw-rw-rw-   0        0        0     2961 2024-01-11 18:09:48.000000 fudstop-2.5.9/fudstop/_markets/scripts/options_volume_analysis.py
--rw-rw-rw-   0        0        0     1942 2024-01-11 18:07:34.000000 fudstop-2.5.9/fudstop/_markets/scripts/rsi_2_4_8.py
--rw-rw-rw-   0        0        0     2172 2024-01-24 23:43:15.000000 fudstop-2.5.9/fudstop/_markets/scripts/rsi_screener.py
--rw-rw-rw-   0        0        0     1197 2024-01-20 05:06:57.000000 fudstop-2.5.9/fudstop/_markets/scripts/ssr_scanner.py
--rw-rw-rw-   0        0        0     7315 2024-01-23 17:20:40.000000 fudstop-2.5.9/fudstop/_markets/scripts/stock_market.py
--rw-rw-rw-   0        0        0     6271 2024-01-12 19:46:21.000000 fudstop-2.5.9/fudstop/_markets/scripts/td9_states.py
--rw-rw-rw-   0        0        0    14287 2024-02-06 18:37:20.000000 fudstop-2.5.9/fudstop/_markets/scripts/universal_snapshot.py
--rw-rw-rw-   0        0        0    13782 2024-01-25 20:46:06.000000 fudstop-2.5.9/fudstop/_markets/stock_market.py
--rw-rw-rw-   0        0        0     1893 2024-01-10 18:26:30.000000 fudstop-2.5.9/fudstop/_markets/webhook_dicts.py
--rw-rw-rw-   0        0        0    14911 2024-01-06 18:40:07.000000 fudstop-2.5.9/fudstop/all_helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.441665 fudstop-2.5.9/fudstop/apis/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.442665 fudstop-2.5.9/fudstop/apis/_asyncpg/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:59.000000 fudstop-2.5.9/fudstop/apis/_asyncpg/__init__.py
--rw-rw-rw-   0        0        0    15085 2024-04-14 15:28:27.000000 fudstop-2.5.9/fudstop/apis/_asyncpg/asyncpg_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.443665 fudstop-2.5.9/fudstop/apis/_datetime/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:52.000000 fudstop-2.5.9/fudstop/apis/_datetime/__init__.py
--rw-rw-rw-   0        0        0     3440 2024-04-14 23:10:42.000000 fudstop-2.5.9/fudstop/apis/_datetime/datetime_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.446175 fudstop-2.5.9/fudstop/apis/_openai/
--rw-rw-rw-   0        0        0        0 2024-01-07 17:40:15.000000 fudstop-2.5.9/fudstop/apis/_openai/__init__.py
--rw-rw-rw-   0        0        0     4824 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/_openai/agent.py
--rw-rw-rw-   0        0        0     7552 2024-03-07 23:34:16.000000 fudstop-2.5.9/fudstop/apis/_openai/openai_sdk.py
--rw-rw-rw-   0        0        0    27388 2024-02-25 03:36:21.000000 fudstop-2.5.9/fudstop/apis/_openai/tools_shcema.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.447177 fudstop-2.5.9/fudstop/apis/_pandas/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:42:25.000000 fudstop-2.5.9/fudstop/apis/_pandas/__init__.py
--rw-rw-rw-   0        0        0      226 2024-02-29 20:44:07.000000 fudstop-2.5.9/fudstop/apis/_pandas/pandas_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.448179 fudstop-2.5.9/fudstop/apis/_selenium/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/_selenium/__init__.py
--rw-rw-rw-   0        0        0     1863 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/_selenium/selenium_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.449178 fudstop-2.5.9/fudstop/apis/alphaquery/
--rw-rw-rw-   0        0        0        0 2024-04-13 21:58:49.000000 fudstop-2.5.9/fudstop/apis/alphaquery/__init__.py
--rw-rw-rw-   0        0        0     3639 2024-04-13 22:04:47.000000 fudstop-2.5.9/fudstop/apis/alphaquery/alpha_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.450176 fudstop-2.5.9/fudstop/apis/alphaquery/models/
--rw-rw-rw-   0        0        0        0 2024-04-13 21:58:58.000000 fudstop-2.5.9/fudstop/apis/alphaquery/models/__init__.py
--rw-rw-rw-   0        0        0       41 2024-04-13 21:59:36.000000 fudstop-2.5.9/fudstop/apis/alphaquery/models/alpha_models.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.454177 fudstop-2.5.9/fudstop/apis/cfr/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/cfr/__init__.py
--rw-rw-rw-   0        0        0     3742 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/cfr/cfr_2.0.py
--rw-rw-rw-   0        0        0       87 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/cfr/cfr_helpers.py
--rw-rw-rw-   0        0        0     7590 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/cfr/cfr_sdk.py
--rw-rw-rw-   0        0        0     2525 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/cfr/title_12.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.455177 fudstop-2.5.9/fudstop/apis/datalink/
--rw-rw-rw-   0        0        0        0 2024-03-25 21:17:59.000000 fudstop-2.5.9/fudstop/apis/datalink/__init__.py
--rw-rw-rw-   0        0        0     2661 2024-03-27 07:04:34.000000 fudstop-2.5.9/fudstop/apis/datalink/datalink_sdk.py
--rw-rw-rw-   0        0        0     2609 2024-03-25 21:32:23.000000 fudstop-2.5.9/fudstop/apis/datalink/models.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.456709 fudstop-2.5.9/fudstop/apis/discord_/
--rw-rw-rw-   0        0        0     4430 2024-01-08 04:14:36.000000 fudstop-2.5.9/fudstop/apis/discord_/__init__.py
--rw-rw-rw-   0        0        0    12863 2024-02-23 01:28:51.000000 fudstop-2.5.9/fudstop/apis/discord_/discord_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.459711 fudstop-2.5.9/fudstop/apis/discord_/models/
--rw-rw-rw-   0        0        0        0 2024-01-18 14:52:13.000000 fudstop-2.5.9/fudstop/apis/discord_/models/__init__.py
--rw-rw-rw-   0        0        0     5431 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/discord_/models/application_commands.py
--rw-rw-rw-   0        0        0     2767 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/discord_/models/search.py
--rw-rw-rw-   0        0        0     1101 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/discord_/models/webhooks.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.460710 fudstop-2.5.9/fudstop/apis/earnings_whisper/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/earnings_whisper/__init__.py
--rw-rw-rw-   0        0        0    12823 2024-03-25 21:47:38.000000 fudstop-2.5.9/fudstop/apis/earnings_whisper/ew_models.py
--rw-rw-rw-   0        0        0     4016 2024-03-25 21:44:18.000000 fudstop-2.5.9/fudstop/apis/earnings_whisper/ew_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.462713 fudstop-2.5.9/fudstop/apis/fastcase/
--rw-rw-rw-   0        0        0        0 2024-04-14 15:00:18.000000 fudstop-2.5.9/fudstop/apis/fastcase/__init__.py
--rw-rw-rw-   0        0        0     6212 2024-05-02 15:37:07.000000 fudstop-2.5.9/fudstop/apis/fastcase/fastcase_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.463714 fudstop-2.5.9/fudstop/apis/fed_print/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/fed_print/__init__.py
--rw-rw-rw-   0        0        0     2908 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/fed_print/fed_print_sync.py
--rw-rw-rw-   0        0        0     5322 2024-02-24 20:29:40.000000 fudstop-2.5.9/fudstop/apis/fed_print/fedprint_models.py
--rw-rw-rw-   0        0        0     3354 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/fed_print/fedprint_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.467228 fudstop-2.5.9/fudstop/apis/federal_register/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/federal_register/__init__.py
--rw-rw-rw-   0        0        0     3075 2024-02-25 17:21:39.000000 fudstop-2.5.9/fudstop/apis/federal_register/fed_register_sdk.py
--rw-rw-rw-   0        0        0     2924 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/federal_register/fed_register_sync.py
--rw-rw-rw-   0        0        0     2904 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/federal_register/register_models.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.468339 fudstop-2.5.9/fudstop/apis/gexbot/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/gexbot/__init__.py
--rw-rw-rw-   0        0        0     4095 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/gexbot/gexbot.py
--rw-rw-rw-   0        0        0     4139 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/gexbot/models.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.470336 fudstop-2.5.9/fudstop/apis/gpts/
--rw-rw-rw-   0        0        0      231 2024-01-08 03:41:52.000000 fudstop-2.5.9/fudstop/apis/gpts/DiscoAI.py
--rw-rw-rw-   0        0        0        2 2024-01-08 03:38:45.000000 fudstop-2.5.9/fudstop/apis/gpts/__init__.py
--rw-rw-rw-   0        0        0    36326 2024-05-01 23:15:01.000000 fudstop-2.5.9/fudstop/apis/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.472339 fudstop-2.5.9/fudstop/apis/master/
--rw-rw-rw-   0        0        0        0 2024-02-25 05:43:46.000000 fudstop-2.5.9/fudstop/apis/master/__init__.py
--rw-rw-rw-   0        0        0     1459 2024-02-25 09:02:57.000000 fudstop-2.5.9/fudstop/apis/master/master_helpers.py
--rw-rw-rw-   0        0        0    29960 2024-02-25 19:23:31.000000 fudstop-2.5.9/fudstop/apis/master/master_sdk.py
--rw-rw-rw-   0        0        0    34633 2024-02-25 09:11:27.000000 fudstop-2.5.9/fudstop/apis/master/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.474844 fudstop-2.5.9/fudstop/apis/misc/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/misc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.475852 fudstop-2.5.9/fudstop/apis/misc/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/misc/models/__init__.py
--rw-rw-rw-   0        0        0      249 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/misc/models/unsplash_models.py
--rw-rw-rw-   0        0        0     2204 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/misc/models/weather_models.py
--rw-rw-rw-   0        0        0      869 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/misc/unsplash.py
--rw-rw-rw-   0        0        0     1790 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/misc/weather.py
--rw-rw-rw-   0        0        0      294 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/misc/weather_helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.477942 fudstop-2.5.9/fudstop/apis/nasdaq/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4200 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/nasdaq/nasdaq_lists.py
--rw-rw-rw-   0        0        0    12177 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/nasdaq/nasdaq_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.479942 fudstop-2.5.9/fudstop/apis/newyork_fed/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/newyork_fed/__init__.py
--rw-rw-rw-   0        0        0    14970 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/newyork_fed/models.py
--rw-rw-rw-   0        0        0    22750 2024-03-27 00:32:52.000000 fudstop-2.5.9/fudstop/apis/newyork_fed/newyork_fed_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.480941 fudstop-2.5.9/fudstop/apis/occ/
--rw-rw-rw-   0        0        0        0 2024-01-12 03:42:31.000000 fudstop-2.5.9/fudstop/apis/occ/__init__.py
--rw-rw-rw-   0        0        0    30622 2024-04-23 04:08:03.000000 fudstop-2.5.9/fudstop/apis/occ/occ_models.py
--rw-rw-rw-   0        0        0    14151 2024-04-23 04:21:11.000000 fudstop-2.5.9/fudstop/apis/occ/occ_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.482941 fudstop-2.5.9/fudstop/apis/ofr/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/ofr/__init__.py
--rw-rw-rw-   0        0        0    37577 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/ofr/ofr_list_sets.py
--rw-rw-rw-   0        0        0     5462 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/ofr/ofr_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.484946 fudstop-2.5.9/fudstop/apis/oic/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/oic/__init__.py
--rw-rw-rw-   0        0        0    16116 2024-01-07 16:09:24.000000 fudstop-2.5.9/fudstop/apis/oic/async_oic_sdk.py
--rw-rw-rw-   0        0        0    11292 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/oic/oic_models.py
--rw-rw-rw-   0        0        0     4938 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/oic/oic_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.491394 fudstop-2.5.9/fudstop/apis/polygonio/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/__init__.py
--rw-rw-rw-   0        0        0    30935 2024-04-24 03:26:35.000000 fudstop-2.5.9/fudstop/apis/polygonio/async_polygon_sdk.py
--rw-rw-rw-   0        0        0     2368 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/db_polygon.py
--rw-rw-rw-   0        0        0    47011 2024-01-10 15:38:01.000000 fudstop-2.5.9/fudstop/apis/polygonio/mapping.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.495901 fudstop-2.5.9/fudstop/apis/polygonio/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/__init__.py
--rw-rw-rw-   0        0        0     1330 2024-04-13 19:03:08.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/aggregates.py
--rw-rw-rw-   0        0        0     1319 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/company_info.py
--rw-rw-rw-   0        0        0     4295 2024-04-14 23:13:19.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/gainers_losers.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.498001 fudstop-2.5.9/fudstop/apis/polygonio/models/option_models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/option_models/__init__.py
--rw-rw-rw-   0        0        0     5734 2024-01-12 15:43:51.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/option_models/option_snapshot.py
--rw-rw-rw-   0        0        0     7043 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/option_models/universal_option.py
--rw-rw-rw-   0        0        0    57290 2024-03-07 18:09:56.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/option_models/universal_snapshot.py
--rw-rw-rw-   0        0        0     6954 2024-01-10 06:10:49.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/technicals.py
--rw-rw-rw-   0        0        0     2271 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/ticker_news.py
--rw-rw-rw-   0        0        0     3801 2024-01-07 01:51:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/ticker_snapshot.py
--rw-rw-rw-   0        0        0     5787 2024-01-21 19:53:33.000000 fudstop-2.5.9/fudstop/apis/polygonio/models/trades.py
--rw-rw-rw-   0        0        0    13028 2024-02-18 06:32:56.000000 fudstop-2.5.9/fudstop/apis/polygonio/polygon_database.py
--rw-rw-rw-   0        0        0    41160 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/polygon_helpers.py
--rw-rw-rw-   0        0        0    71524 2024-04-23 04:12:44.000000 fudstop-2.5.9/fudstop/apis/polygonio/polygon_options.py
--rw-rw-rw-   0        0        0     3692 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/polygon_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.500001 fudstop-2.5.9/fudstop/apis/polygonio/scripts/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/scripts/__init__.py
--rw-rw-rw-   0        0        0     2267 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/polygonio/scripts/daily_aggregates.py
--rw-rw-rw-   0        0        0     1716 2024-02-04 09:29:32.000000 fudstop-2.5.9/fudstop/apis/polygonio/scripts/rsi.py
--rw-rw-rw-   0        0        0     9164 2024-03-01 01:05:43.000000 fudstop-2.5.9/fudstop/apis/polygonio/technicals.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.502004 fudstop-2.5.9/fudstop/apis/rapid/
--rw-rw-rw-   0        0        0        0 2024-05-08 03:47:05.000000 fudstop-2.5.9/fudstop/apis/rapid/__init__.py
--rw-rw-rw-   0        0        0     8348 2024-05-08 05:03:43.000000 fudstop-2.5.9/fudstop/apis/rapid/rapid_models.py
--rw-rw-rw-   0        0        0     3188 2024-05-08 04:36:56.000000 fudstop-2.5.9/fudstop/apis/rapid/rapid_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.505504 fudstop-2.5.9/fudstop/apis/rss/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/rss/__init__.py
--rw-rw-rw-   0        0        0      736 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/rss/rss_helpers.py
--rw-rw-rw-   0        0        0     1497 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/rss/rss_models.py
--rw-rw-rw-   0        0        0    10360 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/apis/rss/rss_sdk.py
--rw-rw-rw-   0        0        0    10203 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/apis/rss/snyc_rss.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.506507 fudstop-2.5.9/fudstop/apis/sec/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:34.000000 fudstop-2.5.9/fudstop/apis/sec/__init__.py
--rw-rw-rw-   0        0        0     8441 2024-02-29 22:33:02.000000 fudstop-2.5.9/fudstop/apis/sec/sec_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.507604 fudstop-2.5.9/fudstop/apis/stocksera_/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.517234 fudstop-2.5.9/fudstop/apis/stocksera_/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/__init__.py
--rw-rw-rw-   0        0        0      487 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/borrowed_shares.py
--rw-rw-rw-   0        0        0      827 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/daily_treasury.py
--rw-rw-rw-   0        0        0      747 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/ftds.py
--rw-rw-rw-   0        0        0      871 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/highest_shorted.py
--rw-rw-rw-   0        0        0      813 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/inflation.py
--rw-rw-rw-   0        0        0     1062 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/insider_trades.py
--rw-rw-rw-   0        0        0      667 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/jim_cramer.py
--rw-rw-rw-   0        0        0      850 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/jobless_claims.py
--rw-rw-rw-   0        0        0     1043 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/low_float.py
--rw-rw-rw-   0        0        0      660 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/market_news.py
--rw-rw-rw-   0        0        0    21824 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/models.py
--rw-rw-rw-   0        0        0      676 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/news_sentiment.py
--rw-rw-rw-   0        0        0      693 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/retail_sales.py
--rw-rw-rw-   0        0        0      708 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/reverse_repo.py
--rw-rw-rw-   0        0        0      777 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/sec_filings.py
--rw-rw-rw-   0        0        0      789 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/models/short_volume.py
--rw-rw-rw-   0        0        0    19676 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/stocksera_/stocksera_.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.519236 fudstop-2.5.9/fudstop/apis/treasury/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/treasury/__init__.py
--rw-rw-rw-   0        0        0    10964 2024-01-20 19:15:58.000000 fudstop-2.5.9/fudstop/apis/treasury/treasury_models.py
--rw-rw-rw-   0        0        0    10281 2024-01-20 19:16:09.000000 fudstop-2.5.9/fudstop/apis/treasury/treasury_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.521236 fudstop-2.5.9/fudstop/apis/udio/
--rw-rw-rw-   0        0        0        0 2024-05-04 04:08:21.000000 fudstop-2.5.9/fudstop/apis/udio/__init__.py
--rw-rw-rw-   0        0        0     4605 2024-05-04 04:20:04.000000 fudstop-2.5.9/fudstop/apis/udio/imps.py
--rw-rw-rw-   0        0        0     2130 2024-05-04 05:03:43.000000 fudstop-2.5.9/fudstop/apis/udio/udio_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.529855 fudstop-2.5.9/fudstop/apis/webull/
--rw-rw-rw-   0        0        0     4945 2024-01-15 22:06:39.000000 fudstop-2.5.9/fudstop/apis/webull/__init__.py
--rw-rw-rw-   0        0        0    12127 2024-01-23 03:47:19.000000 fudstop-2.5.9/fudstop/apis/webull/database_manager.py
--rw-rw-rw-   0        0        0     2732 2024-01-11 18:10:25.000000 fudstop-2.5.9/fudstop/apis/webull/get_volume_analysis.py
--rw-rw-rw-   0        0        0    10628 2024-01-11 18:10:17.000000 fudstop-2.5.9/fudstop/apis/webull/modal.py
--rw-rw-rw-   0        0        0     5320 2024-01-10 21:10:43.000000 fudstop-2.5.9/fudstop/apis/webull/opt_modal.py
--rw-rw-rw-   0        0        0     9390 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/options.py
--rw-rw-rw-   0        0        0     3357 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/screener_models.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.539211 fudstop-2.5.9/fudstop/apis/webull/trade_models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-02-18 21:14:42.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/analyst_ratings.py
--rw-rw-rw-   0        0        0    12121 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/capital_flow.py
--rw-rw-rw-   0        0        0     2147 2024-02-24 19:57:32.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/company_brief.py
--rw-rw-rw-   0        0        0     2235 2024-01-23 05:04:58.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/cost_distribution.py
--rw-rw-rw-   0        0        0     1053 2024-02-18 19:14:15.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/etf_holdings.py
--rw-rw-rw-   0        0        0     1727 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/events.py
--rw-rw-rw-   0        0        0    19884 2024-02-18 19:14:03.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/financials.py
--rw-rw-rw-   0        0        0     3780 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/forecast_evaluator.py
--rw-rw-rw-   0        0        0     3500 2024-02-18 18:48:35.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/institutional_holdings.py
--rw-rw-rw-   0        0        0     1335 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/news.py
--rw-rw-rw-   0        0        0     1195 2024-03-01 01:13:55.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/price_streamer.py
--rw-rw-rw-   0        0        0      601 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/short_interest.py
--rw-rw-rw-   0        0        0     4714 2024-04-29 02:51:39.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/stock_quote.py
--rw-rw-rw-   0        0        0    11042 2024-03-07 17:43:34.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/ticker_query.py
--rw-rw-rw-   0        0        0     1314 2024-01-13 16:23:06.000000 fudstop-2.5.9/fudstop/apis/webull/trade_models/volume_analysis.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.540211 fudstop-2.5.9/fudstop/apis/webull/trader_models/
--rw-rw-rw-   0        0        0        0 2024-04-23 22:21:57.000000 fudstop-2.5.9/fudstop/apis/webull/trader_models/__init__.py
--rw-rw-rw-   0        0        0    39759 2024-04-28 00:01:42.000000 fudstop-2.5.9/fudstop/apis/webull/trader_models/trader_models.py
--rw-rw-rw-   0        0        0    13181 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/webull/webull_helpers.py
--rw-rw-rw-   0        0        0    12274 2024-02-25 06:46:04.000000 fudstop-2.5.9/fudstop/apis/webull/webull_markets.py
--rw-rw-rw-   0        0        0    35666 2024-01-21 19:47:41.000000 fudstop-2.5.9/fudstop/apis/webull/webull_options.py
--rw-rw-rw-   0        0        0     9106 2024-01-18 22:00:22.000000 fudstop-2.5.9/fudstop/apis/webull/webull_parsing.py
--rw-rw-rw-   0        0        0     7131 2024-02-26 02:07:00.000000 fudstop-2.5.9/fudstop/apis/webull/webull_screener.py
--rw-rw-rw-   0        0        0     5509 2024-04-28 00:03:05.000000 fudstop-2.5.9/fudstop/apis/webull/webull_trader.py
--rw-rw-rw-   0        0        0    28866 2024-04-29 02:52:02.000000 fudstop-2.5.9/fudstop/apis/webull/webull_trading.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.542212 fudstop-2.5.9/fudstop/apis/whale/
--rw-rw-rw-   0        0        0        0 2024-03-27 06:54:53.000000 fudstop-2.5.9/fudstop/apis/whale/__init__.py
--rw-rw-rw-   0        0        0    42102 2024-03-27 21:07:42.000000 fudstop-2.5.9/fudstop/apis/whale/whale_models.py
--rw-rw-rw-   0        0        0     7065 2024-03-27 21:07:56.000000 fudstop-2.5.9/fudstop/apis/whale/whale_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.543212 fudstop-2.5.9/fudstop/apis/y_finance/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/apis/y_finance/__init__.py
--rw-rw-rw-   0        0        0     9028 2024-02-18 15:18:29.000000 fudstop-2.5.9/fudstop/apis/y_finance/yf_sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.543212 fudstop-2.5.9/fudstop/database_/
--rw-rw-rw-   0        0        0    66479 2024-02-18 06:41:46.000000 fudstop-2.5.9/fudstop/database_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.547351 fudstop-2.5.9/fudstop/discord_/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/discord_/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-01-11 18:10:55.000000 fudstop-2.5.9/fudstop/discord_/autocomp.py
--rw-rw-rw-   0        0        0    63300 2024-04-27 23:49:56.000000 fudstop-2.5.9/fudstop/discord_/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.548350 fudstop-2.5.9/fudstop/discord_/bot_menus/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/discord_/bot_menus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.550351 fudstop-2.5.9/fudstop/discord_/bot_menus/modals/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/discord_/bot_menus/modals/__init__.py
--rw-rw-rw-   0        0        0     2226 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/discord_/bot_menus/modals/dalle_modal.py
--rw-rw-rw-   0        0        0    13054 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/discord_/bot_menus/modals/options_modal.py
--rw-rw-rw-   0        0        0     3597 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/discord_/bot_menus/pagination.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.563860 fudstop-2.5.9/fudstop/discord_/cogs/
--rw-rw-rw-   0        0        0     4305 2024-01-07 18:05:54.000000 fudstop-2.5.9/fudstop/discord_/cogs/__init__.py
--rw-rw-rw-   0        0        0    20340 2024-01-06 18:32:34.000000 fudstop-2.5.9/fudstop/discord_/cogs/accounting.py
--rw-rw-rw-   0        0        0    11559 2024-01-06 18:29:35.000000 fudstop-2.5.9/fudstop/discord_/cogs/assistant.py
--rw-rw-rw-   0        0        0    11795 2024-02-06 17:49:34.000000 fudstop-2.5.9/fudstop/discord_/cogs/database.py
--rw-rw-rw-   0        0        0    12937 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/discord_/cogs/earnings.py
--rw-rw-rw-   0        0        0     2104 2024-01-06 18:30:08.000000 fudstop-2.5.9/fudstop/discord_/cogs/fed_print.py
--rw-rw-rw-   0        0        0     4463 2024-01-11 18:16:25.000000 fudstop-2.5.9/fudstop/discord_/cogs/filter.py
--rw-rw-rw-   0        0        0    34896 2024-01-11 18:17:51.000000 fudstop-2.5.9/fudstop/discord_/cogs/fiscal_service.py
--rw-rw-rw-   0        0        0     4482 2024-01-07 16:10:05.000000 fudstop-2.5.9/fudstop/discord_/cogs/gex.py
--rw-rw-rw-   0        0        0     6390 2024-02-07 19:46:50.000000 fudstop-2.5.9/fudstop/discord_/cogs/gpt.py
--rw-rw-rw-   0        0        0     3906 2024-02-17 21:04:28.000000 fudstop-2.5.9/fudstop/discord_/cogs/ibrs.py
--rw-rw-rw-   0        0        0     2313 2024-01-06 18:31:02.000000 fudstop-2.5.9/fudstop/discord_/cogs/main_view.py
--rw-rw-rw-   0        0        0    29489 2024-04-06 03:42:15.000000 fudstop-2.5.9/fudstop/discord_/cogs/options.py
--rw-rw-rw-   0        0        0     3827 2024-01-11 18:16:07.000000 fudstop-2.5.9/fudstop/discord_/cogs/plays.py
--rw-rw-rw-   0        0        0     3428 2024-01-06 18:35:15.000000 fudstop-2.5.9/fudstop/discord_/cogs/register.py
--rw-rw-rw-   0        0        0     3800 2024-01-06 18:31:37.000000 fudstop-2.5.9/fudstop/discord_/cogs/spx.py
--rw-rw-rw-   0        0        0     9302 2024-01-11 18:15:53.000000 fudstop-2.5.9/fudstop/discord_/cogs/strategy.py
--rw-rw-rw-   0        0        0     2776 2024-01-06 18:31:52.000000 fudstop-2.5.9/fudstop/discord_/cogs/ta.py
--rw-rw-rw-   0        0        0     3071 2024-01-06 18:32:00.000000 fudstop-2.5.9/fudstop/discord_/cogs/weather.py
--rw-rw-rw-   0        0        0     1346 2024-01-06 18:32:07.000000 fudstop-2.5.9/fudstop/discord_/cogs/webull.py
--rw-rw-rw-   0        0        0    11097 2024-01-06 18:32:21.000000 fudstop-2.5.9/fudstop/discord_/cogs/yfin.py
--rw-rw-rw-   0        0        0     1843 2024-01-14 21:57:53.000000 fudstop-2.5.9/fudstop/discord_/database_getter.py
--rw-rw-rw-   0        0        0     6337 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/discord_/discord_rsi.py
--rw-rw-rw-   0        0        0     3697 2024-01-06 18:23:33.000000 fudstop-2.5.9/fudstop/discord_/embeddings.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.573938 fudstop-2.5.9/fudstop/examples/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/__init__.py
--rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/ecfr_test.py
--rw-rw-rw-   0        0        0      178 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/fed_print_test.py
--rw-rw-rw-   0        0        0      237 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/fed_reg_test.py
--rw-rw-rw-   0        0        0      258 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/nasdaq_test.py
--rw-rw-rw-   0        0        0      181 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/newyork_fed_test.py
--rw-rw-rw-   0        0        0     3793 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/ofr_test.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.581396 fudstop-2.5.9/fudstop/examples/polygonio/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/polygonio/__init__.py
--rw-rw-rw-   0        0        0     1392 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/examples/polygonio/aggregates_second.py
--rw-rw-rw-   0        0        0      709 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/examples/polygonio/company_info.py
--rw-rw-rw-   0        0        0     2345 2024-01-07 23:40:02.000000 fudstop-2.5.9/fudstop/examples/polygonio/get_all_options.py
--rw-rw-rw-   0        0        0      379 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/examples/polygonio/get_all_tickers.py
--rw-rw-rw-   0        0        0      611 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/polygonio/get_near_the_money.py
--rw-rw-rw-   0        0        0     2307 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/polygonio/get_option_aggs.py
--rw-rw-rw-   0        0        0     1190 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/polygonio/get_option_rsi.py
--rw-rw-rw-   0        0        0     3751 2024-01-06 00:03:40.000000 fudstop-2.5.9/fudstop/examples/polygonio/get_option_trades.py
--rw-rw-rw-   0        0        0     2409 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/polygonio/get_ticker_aggs.py
--rw-rw-rw-   0        0        0      683 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/examples/polygonio/market_news.py
--rw-rw-rw-   0        0        0     1305 2024-01-11 18:07:47.000000 fudstop-2.5.9/fudstop/examples/polygonio/polygon_test.py
--rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/scripty.py
--rw-rw-rw-   0        0        0     1871 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/stocksera_test.py
--rw-rw-rw-   0        0        0      776 2024-01-06 17:35:55.000000 fudstop-2.5.9/fudstop/examples/test.py
--rw-rw-rw-   0        0        0     2721 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/test_gex.py
--rw-rw-rw-   0        0        0      284 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/test_insert.py
--rw-rw-rw-   0        0        0     2255 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/test_openai.py
--rw-rw-rw-   0        0        0      698 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/test_opts.py
--rw-rw-rw-   0        0        0      633 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/test_screener.py
--rw-rw-rw-   0        0        0     4324 2024-01-11 18:10:12.000000 fudstop-2.5.9/fudstop/examples/test_sec.py
--rw-rw-rw-   0        0        0     1758 2024-01-11 18:11:03.000000 fudstop-2.5.9/fudstop/examples/test_webull.py
--rw-rw-rw-   0        0        0        0 2024-01-08 17:00:41.000000 fudstop-2.5.9/fudstop/examples/tests_discord.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.582396 fudstop-2.5.9/fudstop/examples/webull/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/webull/__init__.py
--rw-rw-rw-   0        0        0      805 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/webull/markets_example.py
--rw-rw-rw-   0        0        0     2439 2024-01-05 23:27:36.000000 fudstop-2.5.9/fudstop/examples/webull/trade_example.py
--rw-rw-rw-   0        0        0     7753 2024-01-11 18:14:32.000000 fudstop-2.5.9/fudstop/options_filter.py
--rw-rw-rw-   0        0        0    21800 2024-01-11 18:09:07.000000 fudstop-2.5.9/fudstop/plots.py
--rw-rw-rw-   0        0        0    15233 2024-01-11 18:14:18.000000 fudstop-2.5.9/fudstop/schema.py
--rw-rw-rw-   0        0        0      490 2024-02-04 05:36:05.000000 fudstop-2.5.9/fudstop/wet.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:05:07.409437 fudstop-2.5.9/fudstop.egg-info/
--rw-rw-rw-   0        0        0     7618 2024-05-08 05:05:07.000000 fudstop-2.5.9/fudstop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11237 2024-05-08 05:05:07.000000 fudstop-2.5.9/fudstop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 05:05:07.000000 fudstop-2.5.9/fudstop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4028 2024-05-08 05:05:07.000000 fudstop-2.5.9/fudstop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-08 05:05:07.000000 fudstop-2.5.9/fudstop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 05:05:07.592007 fudstop-2.5.9/setup.cfg
--rw-rw-rw-   0        0        0      363 2024-05-08 05:04:05.000000 fudstop-2.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.999782 fudstop-2.6.0/
+-rw-rw-rw-   0        0        0     7618 2024-05-14 22:43:10.999782 fudstop-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2341 2024-01-05 23:27:36.000000 fudstop-2.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.803133 fudstop-2.6.0/app/
+-rw-rw-rw-   0        0        0    43348 2024-01-23 23:29:23.000000 fudstop-2.6.0/app/__init__.py
+-rw-rw-rw-   0        0        0     4011 2024-01-12 03:32:55.000000 fudstop-2.6.0/app/fetcher.py
+-rw-rw-rw-   0        0        0    17884 2024-01-12 06:07:09.000000 fudstop-2.6.0/app/fudstop_info.py
+-rw-rw-rw-   0        0        0    38553 2024-01-12 03:47:25.000000 fudstop-2.6.0/app/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.803133 fudstop-2.6.0/fudstop/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.834383 fudstop-2.6.0/fudstop/_markets/
+-rw-rw-rw-   0        0        0     1327 2024-01-18 15:18:48.000000 fudstop-2.6.0/fudstop/_markets/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-02-22 04:18:16.000000 fudstop-2.6.0/fudstop/_markets/analyzers.py
+-rw-rw-rw-   0        0        0    67237 2024-02-07 15:09:55.000000 fudstop-2.6.0/fudstop/_markets/embeddings.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.834383 fudstop-2.6.0/fudstop/_markets/finished/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:49:02.000000 fudstop-2.6.0/fudstop/_markets/finished/__init__.py
+-rw-rw-rw-   0        0        0    25622 2024-01-21 19:47:09.000000 fudstop-2.6.0/fudstop/_markets/finished/db_manager.py
+-rw-rw-rw-   0        0        0     2530 2023-10-12 23:34:06.000000 fudstop-2.6.0/fudstop/_markets/finished/economic_data.py
+-rw-rw-rw-   0        0        0    53472 2024-02-11 04:30:33.000000 fudstop-2.6.0/fudstop/_markets/finished/master_class.py
+-rw-rw-rw-   0        0        0     9940 2024-01-25 21:35:47.000000 fudstop-2.6.0/fudstop/_markets/finished/td9_states.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.834383 fudstop-2.6.0/fudstop/_markets/list_sets/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/_markets/list_sets/__init__.py
+-rw-rw-rw-   0        0        0    92394 2024-02-22 03:17:43.000000 fudstop-2.6.0/fudstop/_markets/list_sets/dicts.py
+-rw-rw-rw-   0        0        0    88831 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/_markets/list_sets/saved_tickers.py
+-rw-rw-rw-   0        0        0   125429 2024-01-17 16:34:32.000000 fudstop-2.6.0/fudstop/_markets/list_sets/ticker_lists.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.834383 fudstop-2.6.0/fudstop/_markets/market_handlers/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/__init__.py
+-rw-rw-rw-   0        0        0     1265 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/cfg.py
+-rw-rw-rw-   0        0        0     1491 2024-01-09 04:43:27.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/crypto.py
+-rw-rw-rw-   0        0        0    17424 2024-02-12 18:43:10.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/database_.py
+-rw-rw-rw-   0        0        0      768 2024-01-09 05:02:23.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/forex.py
+-rw-rw-rw-   0        0        0     1770 2024-01-08 17:15:06.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/indices.py
+-rw-rw-rw-   0        0        0   762960 2024-01-11 23:53:54.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/list_sets.py
+-rw-rw-rw-   0        0        0    13155 2024-01-11 17:06:04.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/options.py
+-rw-rw-rw-   0        0        0     3929 2024-01-09 21:38:56.000000 fudstop-2.6.0/fudstop/_markets/market_handlers/stocks.py
+-rw-rw-rw-   0        0        0     1166 2024-01-12 17:40:54.000000 fudstop-2.6.0/fudstop/_markets/monitor.py
+-rw-rw-rw-   0        0        0    31105 2024-02-12 14:30:27.000000 fudstop-2.6.0/fudstop/_markets/multimarkets.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.834383 fudstop-2.6.0/fudstop/_markets/plotting/
+-rw-rw-rw-   0        0        0     1814 2024-01-13 01:48:40.000000 fudstop-2.6.0/fudstop/_markets/plotting/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.834383 fudstop-2.6.0/fudstop/_markets/reference_markets/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/_markets/reference_markets/__init__.py
+-rw-rw-rw-   0        0        0     1400 2024-01-08 00:31:15.000000 fudstop-2.6.0/fudstop/_markets/reference_markets/conditional_scans.py
+-rw-rw-rw-   0        0        0     8389 2024-01-10 04:38:30.000000 fudstop-2.6.0/fudstop/_markets/reference_markets/reference_market.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.850007 fudstop-2.6.0/fudstop/_markets/scripts/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/_markets/scripts/__init__.py
+-rw-rw-rw-   0        0        0      846 2024-01-20 18:45:32.000000 fudstop-2.6.0/fudstop/_markets/scripts/all_polygon_options.py
+-rw-rw-rw-   0        0        0      683 2024-01-07 06:56:40.000000 fudstop-2.6.0/fudstop/_markets/scripts/all_webull_options.py
+-rw-rw-rw-   0        0        0     1208 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/_markets/scripts/generation.py
+-rw-rw-rw-   0        0        0     1351 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/_markets/scripts/million_dollar_trades.py
+-rw-rw-rw-   0        0        0     1533 2024-01-18 14:58:07.000000 fudstop-2.6.0/fudstop/_markets/scripts/option_scripts.py
+-rw-rw-rw-   0        0        0    20845 2024-01-20 18:50:03.000000 fudstop-2.6.0/fudstop/_markets/scripts/options_market.py
+-rw-rw-rw-   0        0        0     2961 2024-01-11 18:09:48.000000 fudstop-2.6.0/fudstop/_markets/scripts/options_volume_analysis.py
+-rw-rw-rw-   0        0        0     1942 2024-01-11 18:07:34.000000 fudstop-2.6.0/fudstop/_markets/scripts/rsi_2_4_8.py
+-rw-rw-rw-   0        0        0     2172 2024-01-24 23:43:15.000000 fudstop-2.6.0/fudstop/_markets/scripts/rsi_screener.py
+-rw-rw-rw-   0        0        0     1197 2024-01-20 05:06:57.000000 fudstop-2.6.0/fudstop/_markets/scripts/ssr_scanner.py
+-rw-rw-rw-   0        0        0     7315 2024-01-23 17:20:40.000000 fudstop-2.6.0/fudstop/_markets/scripts/stock_market.py
+-rw-rw-rw-   0        0        0     6271 2024-01-12 19:46:21.000000 fudstop-2.6.0/fudstop/_markets/scripts/td9_states.py
+-rw-rw-rw-   0        0        0    14287 2024-02-06 18:37:20.000000 fudstop-2.6.0/fudstop/_markets/scripts/universal_snapshot.py
+-rw-rw-rw-   0        0        0    13782 2024-01-25 20:46:06.000000 fudstop-2.6.0/fudstop/_markets/stock_market.py
+-rw-rw-rw-   0        0        0     1893 2024-01-10 18:26:30.000000 fudstop-2.6.0/fudstop/_markets/webhook_dicts.py
+-rw-rw-rw-   0        0        0    14911 2024-01-06 18:40:07.000000 fudstop-2.6.0/fudstop/all_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.850007 fudstop-2.6.0/fudstop/apis/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.850007 fudstop-2.6.0/fudstop/apis/_asyncpg/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:59.000000 fudstop-2.6.0/fudstop/apis/_asyncpg/__init__.py
+-rw-rw-rw-   0        0        0    15085 2024-04-14 15:28:27.000000 fudstop-2.6.0/fudstop/apis/_asyncpg/asyncpg_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.850007 fudstop-2.6.0/fudstop/apis/_datetime/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:52.000000 fudstop-2.6.0/fudstop/apis/_datetime/__init__.py
+-rw-rw-rw-   0        0        0     3440 2024-04-14 23:10:42.000000 fudstop-2.6.0/fudstop/apis/_datetime/datetime_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.850007 fudstop-2.6.0/fudstop/apis/_openai/
+-rw-rw-rw-   0        0        0        0 2024-01-07 17:40:15.000000 fudstop-2.6.0/fudstop/apis/_openai/__init__.py
+-rw-rw-rw-   0        0        0     4824 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/_openai/agent.py
+-rw-rw-rw-   0        0        0     7552 2024-03-07 23:34:16.000000 fudstop-2.6.0/fudstop/apis/_openai/openai_sdk.py
+-rw-rw-rw-   0        0        0    27388 2024-02-25 03:36:21.000000 fudstop-2.6.0/fudstop/apis/_openai/tools_shcema.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.850007 fudstop-2.6.0/fudstop/apis/_pandas/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:42:25.000000 fudstop-2.6.0/fudstop/apis/_pandas/__init__.py
+-rw-rw-rw-   0        0        0      226 2024-02-29 20:44:07.000000 fudstop-2.6.0/fudstop/apis/_pandas/pandas_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/_selenium/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/_selenium/__init__.py
+-rw-rw-rw-   0        0        0     1863 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/_selenium/selenium_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/alphaquery/
+-rw-rw-rw-   0        0        0        0 2024-04-13 21:58:49.000000 fudstop-2.6.0/fudstop/apis/alphaquery/__init__.py
+-rw-rw-rw-   0        0        0     3639 2024-04-13 22:04:47.000000 fudstop-2.6.0/fudstop/apis/alphaquery/alpha_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/alphaquery/models/
+-rw-rw-rw-   0        0        0        0 2024-04-13 21:58:58.000000 fudstop-2.6.0/fudstop/apis/alphaquery/models/__init__.py
+-rw-rw-rw-   0        0        0       41 2024-04-13 21:59:36.000000 fudstop-2.6.0/fudstop/apis/alphaquery/models/alpha_models.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/caselaw/
+-rw-rw-rw-   0        0        0        0 2024-05-09 17:36:00.000000 fudstop-2.6.0/fudstop/apis/caselaw/__init__.py
+-rw-rw-rw-   0        0        0     3199 2024-05-09 18:13:57.000000 fudstop-2.6.0/fudstop/apis/caselaw/caselaw_models.py
+-rw-rw-rw-   0        0        0     1709 2024-05-09 18:18:24.000000 fudstop-2.6.0/fudstop/apis/caselaw/caselaw_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/cfr/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/cfr/__init__.py
+-rw-rw-rw-   0        0        0     3742 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/cfr/cfr_2.0.py
+-rw-rw-rw-   0        0        0       87 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/cfr/cfr_helpers.py
+-rw-rw-rw-   0        0        0     7590 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/cfr/cfr_sdk.py
+-rw-rw-rw-   0        0        0     2525 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/cfr/title_12.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/datalink/
+-rw-rw-rw-   0        0        0        0 2024-03-25 21:17:59.000000 fudstop-2.6.0/fudstop/apis/datalink/__init__.py
+-rw-rw-rw-   0        0        0     2661 2024-03-27 07:04:34.000000 fudstop-2.6.0/fudstop/apis/datalink/datalink_sdk.py
+-rw-rw-rw-   0        0        0     2609 2024-03-25 21:32:23.000000 fudstop-2.6.0/fudstop/apis/datalink/models.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/discord_/
+-rw-rw-rw-   0        0        0     4430 2024-01-08 04:14:36.000000 fudstop-2.6.0/fudstop/apis/discord_/__init__.py
+-rw-rw-rw-   0        0        0    12863 2024-02-23 01:28:51.000000 fudstop-2.6.0/fudstop/apis/discord_/discord_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/discord_/models/
+-rw-rw-rw-   0        0        0        0 2024-01-18 14:52:13.000000 fudstop-2.6.0/fudstop/apis/discord_/models/__init__.py
+-rw-rw-rw-   0        0        0     5431 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/discord_/models/application_commands.py
+-rw-rw-rw-   0        0        0     2767 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/discord_/models/search.py
+-rw-rw-rw-   0        0        0     1101 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/discord_/models/webhooks.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.865632 fudstop-2.6.0/fudstop/apis/earnings_whisper/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/earnings_whisper/__init__.py
+-rw-rw-rw-   0        0        0    12823 2024-03-25 21:47:38.000000 fudstop-2.6.0/fudstop/apis/earnings_whisper/ew_models.py
+-rw-rw-rw-   0        0        0     4016 2024-03-25 21:44:18.000000 fudstop-2.6.0/fudstop/apis/earnings_whisper/ew_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/fastcase/
+-rw-rw-rw-   0        0        0        0 2024-04-14 15:00:18.000000 fudstop-2.6.0/fudstop/apis/fastcase/__init__.py
+-rw-rw-rw-   0        0        0     6212 2024-05-02 15:37:07.000000 fudstop-2.6.0/fudstop/apis/fastcase/fastcase_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/fed_print/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/fed_print/__init__.py
+-rw-rw-rw-   0        0        0     2908 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/fed_print/fed_print_sync.py
+-rw-rw-rw-   0        0        0     5322 2024-02-24 20:29:40.000000 fudstop-2.6.0/fudstop/apis/fed_print/fedprint_models.py
+-rw-rw-rw-   0        0        0     3354 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/fed_print/fedprint_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/federal_register/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/federal_register/__init__.py
+-rw-rw-rw-   0        0        0     3075 2024-02-25 17:21:39.000000 fudstop-2.6.0/fudstop/apis/federal_register/fed_register_sdk.py
+-rw-rw-rw-   0        0        0     2924 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/federal_register/fed_register_sync.py
+-rw-rw-rw-   0        0        0     2904 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/federal_register/register_models.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/gexbot/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/gexbot/__init__.py
+-rw-rw-rw-   0        0        0     4095 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/gexbot/gexbot.py
+-rw-rw-rw-   0        0        0     4139 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/gexbot/models.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/gpts/
+-rw-rw-rw-   0        0        0      231 2024-01-08 03:41:52.000000 fudstop-2.6.0/fudstop/apis/gpts/DiscoAI.py
+-rw-rw-rw-   0        0        0        2 2024-01-08 03:38:45.000000 fudstop-2.6.0/fudstop/apis/gpts/__init__.py
+-rw-rw-rw-   0        0        0    36326 2024-05-01 23:15:01.000000 fudstop-2.6.0/fudstop/apis/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/master/
+-rw-rw-rw-   0        0        0        0 2024-02-25 05:43:46.000000 fudstop-2.6.0/fudstop/apis/master/__init__.py
+-rw-rw-rw-   0        0        0     1459 2024-02-25 09:02:57.000000 fudstop-2.6.0/fudstop/apis/master/master_helpers.py
+-rw-rw-rw-   0        0        0    29960 2024-02-25 19:23:31.000000 fudstop-2.6.0/fudstop/apis/master/master_sdk.py
+-rw-rw-rw-   0        0        0    34633 2024-02-25 09:11:27.000000 fudstop-2.6.0/fudstop/apis/master/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/misc/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/misc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/misc/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/misc/models/__init__.py
+-rw-rw-rw-   0        0        0      249 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/misc/models/unsplash_models.py
+-rw-rw-rw-   0        0        0     2204 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/misc/models/weather_models.py
+-rw-rw-rw-   0        0        0      869 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/misc/unsplash.py
+-rw-rw-rw-   0        0        0     1790 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/misc/weather.py
+-rw-rw-rw-   0        0        0      294 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/misc/weather_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.881257 fudstop-2.6.0/fudstop/apis/nasdaq/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4200 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/nasdaq/nasdaq_lists.py
+-rw-rw-rw-   0        0        0    12177 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/nasdaq/nasdaq_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.896882 fudstop-2.6.0/fudstop/apis/newyork_fed/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/newyork_fed/__init__.py
+-rw-rw-rw-   0        0        0    14970 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/newyork_fed/models.py
+-rw-rw-rw-   0        0        0    22750 2024-03-27 00:32:52.000000 fudstop-2.6.0/fudstop/apis/newyork_fed/newyork_fed_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.896882 fudstop-2.6.0/fudstop/apis/occ/
+-rw-rw-rw-   0        0        0        0 2024-01-12 03:42:31.000000 fudstop-2.6.0/fudstop/apis/occ/__init__.py
+-rw-rw-rw-   0        0        0    30622 2024-04-23 04:08:03.000000 fudstop-2.6.0/fudstop/apis/occ/occ_models.py
+-rw-rw-rw-   0        0        0    14151 2024-04-23 04:21:11.000000 fudstop-2.6.0/fudstop/apis/occ/occ_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.896882 fudstop-2.6.0/fudstop/apis/ofr/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/ofr/__init__.py
+-rw-rw-rw-   0        0        0    37577 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/ofr/ofr_list_sets.py
+-rw-rw-rw-   0        0        0     5462 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/ofr/ofr_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.896882 fudstop-2.6.0/fudstop/apis/oic/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/oic/__init__.py
+-rw-rw-rw-   0        0        0    16116 2024-01-07 16:09:24.000000 fudstop-2.6.0/fudstop/apis/oic/async_oic_sdk.py
+-rw-rw-rw-   0        0        0    11292 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/oic/oic_models.py
+-rw-rw-rw-   0        0        0     4938 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/oic/oic_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.896882 fudstop-2.6.0/fudstop/apis/polygonio/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/__init__.py
+-rw-rw-rw-   0        0        0    30935 2024-04-24 03:26:35.000000 fudstop-2.6.0/fudstop/apis/polygonio/async_polygon_sdk.py
+-rw-rw-rw-   0        0        0     2368 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/db_polygon.py
+-rw-rw-rw-   0        0        0    47011 2024-01-10 15:38:01.000000 fudstop-2.6.0/fudstop/apis/polygonio/mapping.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.912508 fudstop-2.6.0/fudstop/apis/polygonio/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/__init__.py
+-rw-rw-rw-   0        0        0     1330 2024-04-13 19:03:08.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/aggregates.py
+-rw-rw-rw-   0        0        0     1319 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/company_info.py
+-rw-rw-rw-   0        0        0     4295 2024-04-14 23:13:19.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/gainers_losers.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.912508 fudstop-2.6.0/fudstop/apis/polygonio/models/option_models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/option_models/__init__.py
+-rw-rw-rw-   0        0        0     5734 2024-01-12 15:43:51.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/option_models/option_snapshot.py
+-rw-rw-rw-   0        0        0     7043 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/option_models/universal_option.py
+-rw-rw-rw-   0        0        0    57290 2024-03-07 18:09:56.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/option_models/universal_snapshot.py
+-rw-rw-rw-   0        0        0     6954 2024-01-10 06:10:49.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/technicals.py
+-rw-rw-rw-   0        0        0     2271 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/ticker_news.py
+-rw-rw-rw-   0        0        0     3801 2024-01-07 01:51:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/ticker_snapshot.py
+-rw-rw-rw-   0        0        0     5787 2024-01-21 19:53:33.000000 fudstop-2.6.0/fudstop/apis/polygonio/models/trades.py
+-rw-rw-rw-   0        0        0    13028 2024-02-18 06:32:56.000000 fudstop-2.6.0/fudstop/apis/polygonio/polygon_database.py
+-rw-rw-rw-   0        0        0    41160 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/polygon_helpers.py
+-rw-rw-rw-   0        0        0    71524 2024-04-23 04:12:44.000000 fudstop-2.6.0/fudstop/apis/polygonio/polygon_options.py
+-rw-rw-rw-   0        0        0     3692 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/polygon_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.912508 fudstop-2.6.0/fudstop/apis/polygonio/scripts/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2267 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/polygonio/scripts/daily_aggregates.py
+-rw-rw-rw-   0        0        0     1716 2024-02-04 09:29:32.000000 fudstop-2.6.0/fudstop/apis/polygonio/scripts/rsi.py
+-rw-rw-rw-   0        0        0     9164 2024-03-01 01:05:43.000000 fudstop-2.6.0/fudstop/apis/polygonio/technicals.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.912508 fudstop-2.6.0/fudstop/apis/rapid/
+-rw-rw-rw-   0        0        0        0 2024-05-08 03:47:05.000000 fudstop-2.6.0/fudstop/apis/rapid/__init__.py
+-rw-rw-rw-   0        0        0     8348 2024-05-08 05:03:43.000000 fudstop-2.6.0/fudstop/apis/rapid/rapid_models.py
+-rw-rw-rw-   0        0        0     3188 2024-05-08 04:36:56.000000 fudstop-2.6.0/fudstop/apis/rapid/rapid_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.912508 fudstop-2.6.0/fudstop/apis/rss/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/rss/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/rss/rss_helpers.py
+-rw-rw-rw-   0        0        0     1497 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/rss/rss_models.py
+-rw-rw-rw-   0        0        0    10360 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/apis/rss/rss_sdk.py
+-rw-rw-rw-   0        0        0    10203 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/apis/rss/snyc_rss.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.912508 fudstop-2.6.0/fudstop/apis/sec/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:34.000000 fudstop-2.6.0/fudstop/apis/sec/__init__.py
+-rw-rw-rw-   0        0        0     8441 2024-02-29 22:33:02.000000 fudstop-2.6.0/fudstop/apis/sec/sec_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.912508 fudstop-2.6.0/fudstop/apis/stocksera_/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.928134 fudstop-2.6.0/fudstop/apis/stocksera_/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/borrowed_shares.py
+-rw-rw-rw-   0        0        0      827 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/daily_treasury.py
+-rw-rw-rw-   0        0        0      747 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/ftds.py
+-rw-rw-rw-   0        0        0      871 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/highest_shorted.py
+-rw-rw-rw-   0        0        0      813 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/inflation.py
+-rw-rw-rw-   0        0        0     1062 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/insider_trades.py
+-rw-rw-rw-   0        0        0      667 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/jim_cramer.py
+-rw-rw-rw-   0        0        0      850 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/jobless_claims.py
+-rw-rw-rw-   0        0        0     1043 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/low_float.py
+-rw-rw-rw-   0        0        0      660 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/market_news.py
+-rw-rw-rw-   0        0        0    21824 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/models.py
+-rw-rw-rw-   0        0        0      676 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/news_sentiment.py
+-rw-rw-rw-   0        0        0      693 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/retail_sales.py
+-rw-rw-rw-   0        0        0      708 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/reverse_repo.py
+-rw-rw-rw-   0        0        0      777 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/sec_filings.py
+-rw-rw-rw-   0        0        0      789 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/models/short_volume.py
+-rw-rw-rw-   0        0        0    19676 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/stocksera_/stocksera_.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.928134 fudstop-2.6.0/fudstop/apis/treasury/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/treasury/__init__.py
+-rw-rw-rw-   0        0        0    10964 2024-01-20 19:15:58.000000 fudstop-2.6.0/fudstop/apis/treasury/treasury_models.py
+-rw-rw-rw-   0        0        0    10281 2024-01-20 19:16:09.000000 fudstop-2.6.0/fudstop/apis/treasury/treasury_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.928134 fudstop-2.6.0/fudstop/apis/udio/
+-rw-rw-rw-   0        0        0        0 2024-05-04 04:08:21.000000 fudstop-2.6.0/fudstop/apis/udio/__init__.py
+-rw-rw-rw-   0        0        0     4605 2024-05-04 04:20:04.000000 fudstop-2.6.0/fudstop/apis/udio/imps.py
+-rw-rw-rw-   0        0        0     2130 2024-05-04 05:03:43.000000 fudstop-2.6.0/fudstop/apis/udio/udio_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.945408 fudstop-2.6.0/fudstop/apis/webull/
+-rw-rw-rw-   0        0        0     4945 2024-01-15 22:06:39.000000 fudstop-2.6.0/fudstop/apis/webull/__init__.py
+-rw-rw-rw-   0        0        0    12127 2024-01-23 03:47:19.000000 fudstop-2.6.0/fudstop/apis/webull/database_manager.py
+-rw-rw-rw-   0        0        0     2732 2024-01-11 18:10:25.000000 fudstop-2.6.0/fudstop/apis/webull/get_volume_analysis.py
+-rw-rw-rw-   0        0        0    10628 2024-01-11 18:10:17.000000 fudstop-2.6.0/fudstop/apis/webull/modal.py
+-rw-rw-rw-   0        0        0     5320 2024-01-10 21:10:43.000000 fudstop-2.6.0/fudstop/apis/webull/opt_modal.py
+-rw-rw-rw-   0        0        0     9390 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/options.py
+-rw-rw-rw-   0        0        0     3357 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/screener_models.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.955334 fudstop-2.6.0/fudstop/apis/webull/trade_models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-02-18 21:14:42.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/analyst_ratings.py
+-rw-rw-rw-   0        0        0    12121 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/capital_flow.py
+-rw-rw-rw-   0        0        0     2147 2024-02-24 19:57:32.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/company_brief.py
+-rw-rw-rw-   0        0        0     2235 2024-01-23 05:04:58.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/cost_distribution.py
+-rw-rw-rw-   0        0        0     1053 2024-02-18 19:14:15.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/etf_holdings.py
+-rw-rw-rw-   0        0        0     1727 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/events.py
+-rw-rw-rw-   0        0        0    19884 2024-02-18 19:14:03.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/financials.py
+-rw-rw-rw-   0        0        0     3780 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/forecast_evaluator.py
+-rw-rw-rw-   0        0        0     3500 2024-02-18 18:48:35.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/institutional_holdings.py
+-rw-rw-rw-   0        0        0     1335 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/news.py
+-rw-rw-rw-   0        0        0     2235 2024-05-14 22:42:18.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/order_flow.py
+-rw-rw-rw-   0        0        0     1195 2024-03-01 01:13:55.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/price_streamer.py
+-rw-rw-rw-   0        0        0      601 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/short_interest.py
+-rw-rw-rw-   0        0        0     4714 2024-04-29 02:51:39.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/stock_quote.py
+-rw-rw-rw-   0        0        0    11042 2024-03-07 17:43:34.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/ticker_query.py
+-rw-rw-rw-   0        0        0     1314 2024-01-13 16:23:06.000000 fudstop-2.6.0/fudstop/apis/webull/trade_models/volume_analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.956333 fudstop-2.6.0/fudstop/apis/webull/trader_models/
+-rw-rw-rw-   0        0        0        0 2024-04-23 22:21:57.000000 fudstop-2.6.0/fudstop/apis/webull/trader_models/__init__.py
+-rw-rw-rw-   0        0        0    39759 2024-04-28 00:01:42.000000 fudstop-2.6.0/fudstop/apis/webull/trader_models/trader_models.py
+-rw-rw-rw-   0        0        0    13181 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/webull/webull_helpers.py
+-rw-rw-rw-   0        0        0    12274 2024-02-25 06:46:04.000000 fudstop-2.6.0/fudstop/apis/webull/webull_markets.py
+-rw-rw-rw-   0        0        0    35666 2024-01-21 19:47:41.000000 fudstop-2.6.0/fudstop/apis/webull/webull_options.py
+-rw-rw-rw-   0        0        0     9106 2024-01-18 22:00:22.000000 fudstop-2.6.0/fudstop/apis/webull/webull_parsing.py
+-rw-rw-rw-   0        0        0     7131 2024-02-26 02:07:00.000000 fudstop-2.6.0/fudstop/apis/webull/webull_screener.py
+-rw-rw-rw-   0        0        0     5509 2024-04-28 00:03:05.000000 fudstop-2.6.0/fudstop/apis/webull/webull_trader.py
+-rw-rw-rw-   0        0        0    30450 2024-05-14 22:11:22.000000 fudstop-2.6.0/fudstop/apis/webull/webull_trading.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.958401 fudstop-2.6.0/fudstop/apis/whale/
+-rw-rw-rw-   0        0        0        0 2024-03-27 06:54:53.000000 fudstop-2.6.0/fudstop/apis/whale/__init__.py
+-rw-rw-rw-   0        0        0    42102 2024-03-27 21:07:42.000000 fudstop-2.6.0/fudstop/apis/whale/whale_models.py
+-rw-rw-rw-   0        0        0     7065 2024-03-27 21:07:56.000000 fudstop-2.6.0/fudstop/apis/whale/whale_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.958811 fudstop-2.6.0/fudstop/apis/y_finance/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/apis/y_finance/__init__.py
+-rw-rw-rw-   0        0        0     9028 2024-02-18 15:18:29.000000 fudstop-2.6.0/fudstop/apis/y_finance/yf_sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.958811 fudstop-2.6.0/fudstop/database_/
+-rw-rw-rw-   0        0        0    66479 2024-02-18 06:41:46.000000 fudstop-2.6.0/fudstop/database_/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.958811 fudstop-2.6.0/fudstop/discord_/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/discord_/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-01-11 18:10:55.000000 fudstop-2.6.0/fudstop/discord_/autocomp.py
+-rw-rw-rw-   0        0        0    63300 2024-04-27 23:49:56.000000 fudstop-2.6.0/fudstop/discord_/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.958811 fudstop-2.6.0/fudstop/discord_/bot_menus/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/discord_/bot_menus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.966885 fudstop-2.6.0/fudstop/discord_/bot_menus/modals/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/discord_/bot_menus/modals/__init__.py
+-rw-rw-rw-   0        0        0     2226 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/discord_/bot_menus/modals/dalle_modal.py
+-rw-rw-rw-   0        0        0    13054 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/discord_/bot_menus/modals/options_modal.py
+-rw-rw-rw-   0        0        0     3597 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/discord_/bot_menus/pagination.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.978886 fudstop-2.6.0/fudstop/discord_/cogs/
+-rw-rw-rw-   0        0        0     4305 2024-01-07 18:05:54.000000 fudstop-2.6.0/fudstop/discord_/cogs/__init__.py
+-rw-rw-rw-   0        0        0    20340 2024-01-06 18:32:34.000000 fudstop-2.6.0/fudstop/discord_/cogs/accounting.py
+-rw-rw-rw-   0        0        0    11559 2024-01-06 18:29:35.000000 fudstop-2.6.0/fudstop/discord_/cogs/assistant.py
+-rw-rw-rw-   0        0        0    11795 2024-02-06 17:49:34.000000 fudstop-2.6.0/fudstop/discord_/cogs/database.py
+-rw-rw-rw-   0        0        0    12937 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/discord_/cogs/earnings.py
+-rw-rw-rw-   0        0        0     2104 2024-01-06 18:30:08.000000 fudstop-2.6.0/fudstop/discord_/cogs/fed_print.py
+-rw-rw-rw-   0        0        0     4463 2024-01-11 18:16:25.000000 fudstop-2.6.0/fudstop/discord_/cogs/filter.py
+-rw-rw-rw-   0        0        0    34896 2024-01-11 18:17:51.000000 fudstop-2.6.0/fudstop/discord_/cogs/fiscal_service.py
+-rw-rw-rw-   0        0        0     4482 2024-01-07 16:10:05.000000 fudstop-2.6.0/fudstop/discord_/cogs/gex.py
+-rw-rw-rw-   0        0        0     6390 2024-02-07 19:46:50.000000 fudstop-2.6.0/fudstop/discord_/cogs/gpt.py
+-rw-rw-rw-   0        0        0     3906 2024-02-17 21:04:28.000000 fudstop-2.6.0/fudstop/discord_/cogs/ibrs.py
+-rw-rw-rw-   0        0        0     2313 2024-01-06 18:31:02.000000 fudstop-2.6.0/fudstop/discord_/cogs/main_view.py
+-rw-rw-rw-   0        0        0    29489 2024-04-06 03:42:15.000000 fudstop-2.6.0/fudstop/discord_/cogs/options.py
+-rw-rw-rw-   0        0        0     3827 2024-01-11 18:16:07.000000 fudstop-2.6.0/fudstop/discord_/cogs/plays.py
+-rw-rw-rw-   0        0        0     3428 2024-01-06 18:35:15.000000 fudstop-2.6.0/fudstop/discord_/cogs/register.py
+-rw-rw-rw-   0        0        0     3800 2024-01-06 18:31:37.000000 fudstop-2.6.0/fudstop/discord_/cogs/spx.py
+-rw-rw-rw-   0        0        0     9302 2024-01-11 18:15:53.000000 fudstop-2.6.0/fudstop/discord_/cogs/strategy.py
+-rw-rw-rw-   0        0        0     2776 2024-01-06 18:31:52.000000 fudstop-2.6.0/fudstop/discord_/cogs/ta.py
+-rw-rw-rw-   0        0        0     3071 2024-01-06 18:32:00.000000 fudstop-2.6.0/fudstop/discord_/cogs/weather.py
+-rw-rw-rw-   0        0        0     1346 2024-01-06 18:32:07.000000 fudstop-2.6.0/fudstop/discord_/cogs/webull.py
+-rw-rw-rw-   0        0        0    11097 2024-01-06 18:32:21.000000 fudstop-2.6.0/fudstop/discord_/cogs/yfin.py
+-rw-rw-rw-   0        0        0     1843 2024-01-14 21:57:53.000000 fudstop-2.6.0/fudstop/discord_/database_getter.py
+-rw-rw-rw-   0        0        0     6337 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/discord_/discord_rsi.py
+-rw-rw-rw-   0        0        0     3697 2024-01-06 18:23:33.000000 fudstop-2.6.0/fudstop/discord_/embeddings.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.989782 fudstop-2.6.0/fudstop/examples/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/__init__.py
+-rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/ecfr_test.py
+-rw-rw-rw-   0        0        0      178 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/fed_print_test.py
+-rw-rw-rw-   0        0        0      237 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/fed_reg_test.py
+-rw-rw-rw-   0        0        0      258 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/nasdaq_test.py
+-rw-rw-rw-   0        0        0      181 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/newyork_fed_test.py
+-rw-rw-rw-   0        0        0     3793 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/ofr_test.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.995781 fudstop-2.6.0/fudstop/examples/polygonio/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/polygonio/__init__.py
+-rw-rw-rw-   0        0        0     1392 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/examples/polygonio/aggregates_second.py
+-rw-rw-rw-   0        0        0      709 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/examples/polygonio/company_info.py
+-rw-rw-rw-   0        0        0     2345 2024-01-07 23:40:02.000000 fudstop-2.6.0/fudstop/examples/polygonio/get_all_options.py
+-rw-rw-rw-   0        0        0      379 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/examples/polygonio/get_all_tickers.py
+-rw-rw-rw-   0        0        0      611 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/polygonio/get_near_the_money.py
+-rw-rw-rw-   0        0        0     2307 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/polygonio/get_option_aggs.py
+-rw-rw-rw-   0        0        0     1190 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/polygonio/get_option_rsi.py
+-rw-rw-rw-   0        0        0     3751 2024-01-06 00:03:40.000000 fudstop-2.6.0/fudstop/examples/polygonio/get_option_trades.py
+-rw-rw-rw-   0        0        0     2409 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/polygonio/get_ticker_aggs.py
+-rw-rw-rw-   0        0        0      683 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/examples/polygonio/market_news.py
+-rw-rw-rw-   0        0        0     1305 2024-01-11 18:07:47.000000 fudstop-2.6.0/fudstop/examples/polygonio/polygon_test.py
+-rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/scripty.py
+-rw-rw-rw-   0        0        0     1871 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/stocksera_test.py
+-rw-rw-rw-   0        0        0      776 2024-01-06 17:35:55.000000 fudstop-2.6.0/fudstop/examples/test.py
+-rw-rw-rw-   0        0        0     2721 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/test_gex.py
+-rw-rw-rw-   0        0        0      284 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/test_insert.py
+-rw-rw-rw-   0        0        0     2255 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/test_openai.py
+-rw-rw-rw-   0        0        0      698 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/test_opts.py
+-rw-rw-rw-   0        0        0      633 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/test_screener.py
+-rw-rw-rw-   0        0        0     4324 2024-01-11 18:10:12.000000 fudstop-2.6.0/fudstop/examples/test_sec.py
+-rw-rw-rw-   0        0        0     1758 2024-01-11 18:11:03.000000 fudstop-2.6.0/fudstop/examples/test_webull.py
+-rw-rw-rw-   0        0        0        0 2024-01-08 17:00:41.000000 fudstop-2.6.0/fudstop/examples/tests_discord.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.997781 fudstop-2.6.0/fudstop/examples/webull/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/webull/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/webull/markets_example.py
+-rw-rw-rw-   0        0        0     2439 2024-01-05 23:27:36.000000 fudstop-2.6.0/fudstop/examples/webull/trade_example.py
+-rw-rw-rw-   0        0        0     7753 2024-01-11 18:14:32.000000 fudstop-2.6.0/fudstop/options_filter.py
+-rw-rw-rw-   0        0        0    21800 2024-01-11 18:09:07.000000 fudstop-2.6.0/fudstop/plots.py
+-rw-rw-rw-   0        0        0    15233 2024-01-11 18:14:18.000000 fudstop-2.6.0/fudstop/schema.py
+-rw-rw-rw-   0        0        0      490 2024-02-04 05:36:05.000000 fudstop-2.6.0/fudstop/wet.py
+drwxrwxrwx   0        0        0        0 2024-05-14 22:43:10.818759 fudstop-2.6.0/fudstop.egg-info/
+-rw-rw-rw-   0        0        0     7618 2024-05-14 22:43:10.000000 fudstop-2.6.0/fudstop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11392 2024-05-14 22:43:10.000000 fudstop-2.6.0/fudstop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 22:43:10.000000 fudstop-2.6.0/fudstop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4028 2024-05-14 22:43:10.000000 fudstop-2.6.0/fudstop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-14 22:43:10.000000 fudstop-2.6.0/fudstop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 22:43:10.999782 fudstop-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      363 2024-05-14 22:42:41.000000 fudstop-2.6.0/setup.py
```

### Comparing `fudstop-2.5.9/PKG-INFO` & `fudstop-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudstop
-Version: 2.5.9
+Version: 2.6.0
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
```

### Comparing `fudstop-2.5.9/README.md` & `fudstop-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/app/__init__.py` & `fudstop-2.6.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/app/fetcher.py` & `fudstop-2.6.0/app/fetcher.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/app/fudstop_info.py` & `fudstop-2.6.0/app/fudstop_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/app/helpers.py` & `fudstop-2.6.0/app/helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/__init__.py` & `fudstop-2.6.0/fudstop/_markets/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/analyzers.py` & `fudstop-2.6.0/fudstop/_markets/analyzers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/embeddings.py` & `fudstop-2.6.0/fudstop/_markets/embeddings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/finished/db_manager.py` & `fudstop-2.6.0/fudstop/_markets/finished/db_manager.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/finished/economic_data.py` & `fudstop-2.6.0/fudstop/_markets/finished/economic_data.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/finished/master_class.py` & `fudstop-2.6.0/fudstop/_markets/finished/master_class.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/finished/td9_states.py` & `fudstop-2.6.0/fudstop/_markets/finished/td9_states.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/list_sets/dicts.py` & `fudstop-2.6.0/fudstop/_markets/list_sets/dicts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/list_sets/saved_tickers.py` & `fudstop-2.6.0/fudstop/_markets/list_sets/saved_tickers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/list_sets/ticker_lists.py` & `fudstop-2.6.0/fudstop/_markets/list_sets/ticker_lists.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/market_handlers/cfg.py` & `fudstop-2.6.0/fudstop/_markets/market_handlers/cfg.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/market_handlers/crypto.py` & `fudstop-2.6.0/fudstop/_markets/market_handlers/crypto.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/market_handlers/database_.py` & `fudstop-2.6.0/fudstop/_markets/market_handlers/database_.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/market_handlers/forex.py` & `fudstop-2.6.0/fudstop/_markets/market_handlers/forex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/market_handlers/indices.py` & `fudstop-2.6.0/fudstop/_markets/market_handlers/indices.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/market_handlers/list_sets.py` & `fudstop-2.6.0/fudstop/_markets/market_handlers/list_sets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/market_handlers/options.py` & `fudstop-2.6.0/fudstop/_markets/market_handlers/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/market_handlers/stocks.py` & `fudstop-2.6.0/fudstop/_markets/market_handlers/stocks.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/monitor.py` & `fudstop-2.6.0/fudstop/_markets/monitor.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/multimarkets.py` & `fudstop-2.6.0/fudstop/_markets/multimarkets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/plotting/__init__.py` & `fudstop-2.6.0/fudstop/_markets/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/reference_markets/conditional_scans.py` & `fudstop-2.6.0/fudstop/_markets/reference_markets/conditional_scans.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/reference_markets/reference_market.py` & `fudstop-2.6.0/fudstop/_markets/reference_markets/reference_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/all_polygon_options.py` & `fudstop-2.6.0/fudstop/_markets/scripts/all_polygon_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/all_webull_options.py` & `fudstop-2.6.0/fudstop/_markets/scripts/all_webull_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/generation.py` & `fudstop-2.6.0/fudstop/_markets/scripts/generation.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/million_dollar_trades.py` & `fudstop-2.6.0/fudstop/_markets/scripts/million_dollar_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/option_scripts.py` & `fudstop-2.6.0/fudstop/_markets/scripts/option_scripts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/options_market.py` & `fudstop-2.6.0/fudstop/_markets/scripts/options_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/options_volume_analysis.py` & `fudstop-2.6.0/fudstop/_markets/scripts/options_volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/rsi_2_4_8.py` & `fudstop-2.6.0/fudstop/_markets/scripts/rsi_2_4_8.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/rsi_screener.py` & `fudstop-2.6.0/fudstop/_markets/scripts/rsi_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/ssr_scanner.py` & `fudstop-2.6.0/fudstop/_markets/scripts/ssr_scanner.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/stock_market.py` & `fudstop-2.6.0/fudstop/_markets/scripts/stock_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/td9_states.py` & `fudstop-2.6.0/fudstop/_markets/scripts/td9_states.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/scripts/universal_snapshot.py` & `fudstop-2.6.0/fudstop/_markets/scripts/universal_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/stock_market.py` & `fudstop-2.6.0/fudstop/_markets/stock_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/_markets/webhook_dicts.py` & `fudstop-2.6.0/fudstop/_markets/webhook_dicts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/all_helpers.py` & `fudstop-2.6.0/fudstop/all_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/_asyncpg/asyncpg_sdk.py` & `fudstop-2.6.0/fudstop/apis/_asyncpg/asyncpg_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/_datetime/datetime_sdk.py` & `fudstop-2.6.0/fudstop/apis/_datetime/datetime_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/_openai/agent.py` & `fudstop-2.6.0/fudstop/apis/_openai/agent.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/_openai/openai_sdk.py` & `fudstop-2.6.0/fudstop/apis/_openai/openai_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/_openai/tools_shcema.py` & `fudstop-2.6.0/fudstop/apis/_openai/tools_shcema.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/_selenium/selenium_sdk.py` & `fudstop-2.6.0/fudstop/apis/_selenium/selenium_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/alphaquery/alpha_sdk.py` & `fudstop-2.6.0/fudstop/apis/alphaquery/alpha_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/cfr/cfr_2.0.py` & `fudstop-2.6.0/fudstop/apis/cfr/cfr_2.0.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/cfr/cfr_sdk.py` & `fudstop-2.6.0/fudstop/apis/cfr/cfr_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/cfr/title_12.py` & `fudstop-2.6.0/fudstop/apis/cfr/title_12.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/datalink/datalink_sdk.py` & `fudstop-2.6.0/fudstop/apis/datalink/datalink_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/datalink/models.py` & `fudstop-2.6.0/fudstop/apis/datalink/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/discord_/__init__.py` & `fudstop-2.6.0/fudstop/apis/discord_/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/discord_/discord_sdk.py` & `fudstop-2.6.0/fudstop/apis/discord_/discord_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/discord_/models/application_commands.py` & `fudstop-2.6.0/fudstop/apis/discord_/models/application_commands.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/discord_/models/search.py` & `fudstop-2.6.0/fudstop/apis/discord_/models/search.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/discord_/models/webhooks.py` & `fudstop-2.6.0/fudstop/apis/discord_/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/earnings_whisper/ew_models.py` & `fudstop-2.6.0/fudstop/apis/earnings_whisper/ew_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/earnings_whisper/ew_sdk.py` & `fudstop-2.6.0/fudstop/apis/earnings_whisper/ew_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/fastcase/fastcase_sdk.py` & `fudstop-2.6.0/fudstop/apis/fastcase/fastcase_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/fed_print/fed_print_sync.py` & `fudstop-2.6.0/fudstop/apis/fed_print/fed_print_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/fed_print/fedprint_models.py` & `fudstop-2.6.0/fudstop/apis/fed_print/fedprint_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/fed_print/fedprint_sdk.py` & `fudstop-2.6.0/fudstop/apis/fed_print/fedprint_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/federal_register/fed_register_sdk.py` & `fudstop-2.6.0/fudstop/apis/federal_register/fed_register_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/federal_register/fed_register_sync.py` & `fudstop-2.6.0/fudstop/apis/federal_register/fed_register_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/federal_register/register_models.py` & `fudstop-2.6.0/fudstop/apis/federal_register/register_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/gexbot/gexbot.py` & `fudstop-2.6.0/fudstop/apis/gexbot/gexbot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/gexbot/models.py` & `fudstop-2.6.0/fudstop/apis/gexbot/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/helpers.py` & `fudstop-2.6.0/fudstop/apis/helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/master/master_helpers.py` & `fudstop-2.6.0/fudstop/apis/master/master_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/master/master_sdk.py` & `fudstop-2.6.0/fudstop/apis/master/master_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/master/tools.py` & `fudstop-2.6.0/fudstop/apis/master/tools.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/misc/models/weather_models.py` & `fudstop-2.6.0/fudstop/apis/misc/models/weather_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/misc/unsplash.py` & `fudstop-2.6.0/fudstop/apis/misc/unsplash.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/misc/weather.py` & `fudstop-2.6.0/fudstop/apis/misc/weather.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/nasdaq/nasdaq_lists.py` & `fudstop-2.6.0/fudstop/apis/nasdaq/nasdaq_lists.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/nasdaq/nasdaq_sdk.py` & `fudstop-2.6.0/fudstop/apis/nasdaq/nasdaq_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/newyork_fed/models.py` & `fudstop-2.6.0/fudstop/apis/newyork_fed/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/newyork_fed/newyork_fed_sdk.py` & `fudstop-2.6.0/fudstop/apis/newyork_fed/newyork_fed_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/occ/occ_models.py` & `fudstop-2.6.0/fudstop/apis/occ/occ_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/occ/occ_sdk.py` & `fudstop-2.6.0/fudstop/apis/occ/occ_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/ofr/ofr_list_sets.py` & `fudstop-2.6.0/fudstop/apis/ofr/ofr_list_sets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/ofr/ofr_sdk.py` & `fudstop-2.6.0/fudstop/apis/ofr/ofr_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/oic/async_oic_sdk.py` & `fudstop-2.6.0/fudstop/apis/oic/async_oic_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/oic/oic_models.py` & `fudstop-2.6.0/fudstop/apis/oic/oic_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/oic/oic_sdk.py` & `fudstop-2.6.0/fudstop/apis/oic/oic_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/async_polygon_sdk.py` & `fudstop-2.6.0/fudstop/apis/polygonio/async_polygon_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/db_polygon.py` & `fudstop-2.6.0/fudstop/apis/polygonio/db_polygon.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/mapping.py` & `fudstop-2.6.0/fudstop/apis/polygonio/mapping.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/aggregates.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/aggregates.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/company_info.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/company_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/gainers_losers.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/gainers_losers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/option_models/option_snapshot.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/option_models/option_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/option_models/universal_option.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/option_models/universal_option.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/option_models/universal_snapshot.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/option_models/universal_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/technicals.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/technicals.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/ticker_news.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/ticker_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/ticker_snapshot.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/ticker_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/models/trades.py` & `fudstop-2.6.0/fudstop/apis/polygonio/models/trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/polygon_database.py` & `fudstop-2.6.0/fudstop/apis/polygonio/polygon_database.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/polygon_helpers.py` & `fudstop-2.6.0/fudstop/apis/polygonio/polygon_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/polygon_options.py` & `fudstop-2.6.0/fudstop/apis/polygonio/polygon_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/polygon_sync.py` & `fudstop-2.6.0/fudstop/apis/polygonio/polygon_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/scripts/daily_aggregates.py` & `fudstop-2.6.0/fudstop/apis/polygonio/scripts/daily_aggregates.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/scripts/rsi.py` & `fudstop-2.6.0/fudstop/apis/polygonio/scripts/rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/polygonio/technicals.py` & `fudstop-2.6.0/fudstop/apis/polygonio/technicals.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/rapid/rapid_models.py` & `fudstop-2.6.0/fudstop/apis/rapid/rapid_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/rapid/rapid_sdk.py` & `fudstop-2.6.0/fudstop/apis/rapid/rapid_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/rss/rss_helpers.py` & `fudstop-2.6.0/fudstop/apis/rss/rss_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/rss/rss_models.py` & `fudstop-2.6.0/fudstop/apis/rss/rss_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/rss/rss_sdk.py` & `fudstop-2.6.0/fudstop/apis/rss/rss_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/rss/snyc_rss.py` & `fudstop-2.6.0/fudstop/apis/rss/snyc_rss.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/sec/sec_sdk.py` & `fudstop-2.6.0/fudstop/apis/sec/sec_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/daily_treasury.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/daily_treasury.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/ftds.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/ftds.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/highest_shorted.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/highest_shorted.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/inflation.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/inflation.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/insider_trades.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/insider_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/jim_cramer.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/jim_cramer.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/jobless_claims.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/jobless_claims.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/low_float.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/low_float.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/market_news.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/market_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/models.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/news_sentiment.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/news_sentiment.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/retail_sales.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/retail_sales.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/reverse_repo.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/reverse_repo.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/sec_filings.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/sec_filings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/models/short_volume.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/stocksera_/stocksera_.py` & `fudstop-2.6.0/fudstop/apis/stocksera_/stocksera_.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/treasury/treasury_models.py` & `fudstop-2.6.0/fudstop/apis/treasury/treasury_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/treasury/treasury_sdk.py` & `fudstop-2.6.0/fudstop/apis/treasury/treasury_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/udio/imps.py` & `fudstop-2.6.0/fudstop/apis/udio/imps.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/udio/udio_sdk.py` & `fudstop-2.6.0/fudstop/apis/udio/udio_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/__init__.py` & `fudstop-2.6.0/fudstop/apis/webull/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/database_manager.py` & `fudstop-2.6.0/fudstop/apis/webull/database_manager.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/get_volume_analysis.py` & `fudstop-2.6.0/fudstop/apis/webull/get_volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/modal.py` & `fudstop-2.6.0/fudstop/apis/webull/modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/opt_modal.py` & `fudstop-2.6.0/fudstop/apis/webull/opt_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/options.py` & `fudstop-2.6.0/fudstop/apis/webull/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/screener_models.py` & `fudstop-2.6.0/fudstop/apis/webull/screener_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/analyst_ratings.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/capital_flow.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/capital_flow.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/company_brief.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/company_brief.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/cost_distribution.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/cost_distribution.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/etf_holdings.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/events.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/events.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/financials.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/financials.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/forecast_evaluator.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/forecast_evaluator.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/institutional_holdings.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/news.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/price_streamer.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/price_streamer.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/short_interest.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/short_interest.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/stock_quote.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/stock_quote.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/ticker_query.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/ticker_query.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trade_models/volume_analysis.py` & `fudstop-2.6.0/fudstop/apis/webull/trade_models/volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/trader_models/trader_models.py` & `fudstop-2.6.0/fudstop/apis/webull/trader_models/trader_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/webull_helpers.py` & `fudstop-2.6.0/fudstop/apis/webull/webull_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/webull_markets.py` & `fudstop-2.6.0/fudstop/apis/webull/webull_markets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/webull_options.py` & `fudstop-2.6.0/fudstop/apis/webull/webull_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/webull_parsing.py` & `fudstop-2.6.0/fudstop/apis/webull/webull_parsing.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/webull_screener.py` & `fudstop-2.6.0/fudstop/apis/webull/webull_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/webull_trader.py` & `fudstop-2.6.0/fudstop/apis/webull/webull_trader.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/webull/webull_trading.py` & `fudstop-2.6.0/fudstop/apis/webull/webull_trading.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .trade_models.forecast_evaluator import ForecastEvaluator
 from .trade_models.short_interest import ShortInterest
 from .trade_models.volume_analysis import WebullVolAnalysis
 from .trade_models.ticker_query import WebullStockData
 from .trade_models.analyst_ratings import Analysis
 from .trade_models.price_streamer import PriceStreamer
 from .trade_models.company_brief import CompanyBrief, Executives, Sectors
-
+from .trade_models.order_flow import OrderFlow
 import asyncio
 
 from datetime import datetime, timedelta, timezone
 
 class WebullTrading:
     def __init__(self):
         self.most_active_tickers= ['SNOW', 'IBM', 'DKNG', 'SLV', 'NWL', 'SPXS', 'DIA', 'QCOM', 'CMG', 'WYNN', 'PENN', 'HLF', 'CCJ', 'WW', 'NEM', 'MOS', 'SRPT', 'MS', 'DPST', 'AG', 'PAA', 'PANW', 'XPEV', 'BHC', 'KSS', 'XLP', 'LLY', 'MDB', 'AZN', 'NVO', 'BOIL', 'ZM', 'HUT', 'VIX', 'PDD', 'SLB', 'PCG', 'DIS', 'TFC', 'SIRI', 'TDOC', 'CRSP', 'BSX', 'BITF', 'AAL', 'EOSE', 'RIVN', 'X', 'CCL', 'SOXS', 'NOVA', 'TMUS', 'HES', 'LI', 'NVAX', 'TSM', 'CNC', 'IAU', 'GDDY', 'CVX', 'TGT', 'MCD', 'GDXJ', 'AAPL', 'NKLA', 'EDR', 'NOK', 'SPWR', 'NKE', 'HYG', 'FSLR', 'SGEN', 'DNN', 'BAX', 'CRWD', 'OSTK', 'XLC', 'RIG', 'SEDG', 'SNDL', 'RSP', 'M', 'CD', 'UNG', 'LQD', 'TTD', 'AMGN', 'EQT', 'YINN', 'MULN', 'FTNT', 'WBD', 'MRNA', 'PTON', 'SCHW', 'ABNB', 'EW', 'PM', 'UCO', 'TXN', 'DLR', 'KHC', 'MMAT', 'QQQ', 'GOOGL', 'AEM', 'RTX', 'AVGO', 'RBLX', 'PAAS', 'UUP', 'OXY', 'SQ', 'PLUG', 'CLF', 'GOEV', 'BKLN', 'ALB', 'BALL', 'SMH', 'CVE', 'F', 'KRE', 'TWLO', 'ARCC', 'ARM', 'U', 'SOFI', 'SBUX', 'FXI', 'BMY', 'HSBC', 'EFA', 'SVXY', 'VALE', 'GOLD', 'MSFT', 'OIH', 'ARKK', 'AMD', 'AA', 'DXCM', 'ABT', 'WOLF', 'FDX', 'SOXL', 'MA', 'KWEB', 'BP', 'SNAP', 'NLY', 'KGC', 'URA', 'UVIX', 'KMI', 'ACB', 'NET', 'W', 'GRAB', 'LMT', 'EPD', 'FCX', 'STNE', 'NIO', 'SU', 'ET', 'CVS', 'ADBE', 'MXL', 'HOOD', 'FUBO', 'RIOT', 'CRM', 'TNA', 'DISH', 'XBI', 'VFS', 'GPS', 'NVDA', 'MGM', 'MRK', 'ABBV', 'LABU', 'BEKE', 'VRT', 'LVS', 'CPNG', 'BA', 'MTCH', 'PEP', 'EBAY', 'GDX', 'XLV', 'UBER', 'GOOG', 'COF', 'XLU', 'BILI', 'XLK', 'VXX', 'DVN', 'MSOS', 'KOLD', 'XOM', 'BKNG', 'SPY', 'RUT', 'CMCSA', 'STLA', 'NCLH', 'GRPN', 'ZION', 'UAL', 'GM', 'NDX', 'TQQQ', 'COIN', 'WBA', 'CLSK', 'NFLX', 'FREY', 'AFRM', 'NAT', 'EEM', 'IYR', 'KEY', 'OPEN', 'DM', 'TSLA', 'BXMT', 'T', 'TZA', 'BAC', 'MARA', 'UVXY', 'LOW', 'COST', 'HL', 'CHTR', 'TMF', 'ROKU', 'DOCU', 'PSEC', 'XHB', 'VMW', 'SABR', 'USB', 'DDOG', 'DB', 'V', 'NOW', 'XRT', 'SMCI', 'PFE', 'NYCB', 'BIDU', 'C', 'SPX', 'ETSY', 'EMB', 'SQQQ', 'CHPT', 'DASH', 'VZ', 'DNA', 'CL', 'ANET', 'WMT', 'MRO', 'WFC', 'MO', 'USO', 'ENVX', 'INTC', 'GEO', 'VFC', 'WE', 'MET', 'CHWY', 'PBR', 'KO', 'TH', 'QS', 'BTU', 'GLD', 'JD', 'XLY', 'KR', 'ASTS', 'WDC', 'HTZ', 'XLF', 'COP', 'PATH', 'SHEL', 'MXEF', 'SE', 'SPCE', 'UPS', 'RUN', 'DOW', 'ASHR', 'ONON', 'DAL', 'SPXL', 'SAVE', 'LUV', 'HD', 'JNJ', 'LYFT', 'UNH', 'BBY', 'CZR', 'NEE', 'STNG', 'SPXU', 'MMM', 'VNQ', 'IMGN', 'MSTR', 'AXP', 'TMO', 'XPO', 'FEZ', 'ENPH', 'AX', 'NVCR', 'GS', 'MRVL', 'ADM', 'GILD', 'IBB', 'FTCH', 'PARA', 'PINS', 'JBLU', 'SNY', 'BITO', 'PYPL', 'FAS', 'GME', 'LAZR', 'URNM', 'BX', 'MPW', 'UPRO', 'HPQ', 'AMZN', 'SAVA', 'TLT', 'ON', 'CAT', 'VLO', 'AR', 'IDXX', 'SWN', 'META', 'BABA', 'ZS', 'EWZ', 'ORCL', 'XOP', 'TJX', 'XP', 'EL', 'HAL', 'IEF', 'XLI', 'UPST', 'Z', 'TELL', 'LRCX', 'DLTR', 'BYND', 'PACW', 'CVNA', 'GSAT', 'CSCO', 'NU', 'KVUE', 'JPM', 'LCID', 'TLRY', 'AGNC', 'CGC', 'XLE', 'VOD', 'TEVA', 'JETS', 'UEC', 'FSR', 'ZIM', 'ABR', 'IQ', 'AMC', 'ALLY', 'HE', 'OKTA', 'ACN', 'MU', 'FLEX', 'SHOP', 'PLTR', 'CLX', 'LUMN', 'WHR', 'PAGP', 'IWM', 'WPM', 'TTWO', 'AI', 'ALGN', 'SPOT', 'BTG', 'IONQ', 'GE', 'DG', 'AMAT', 'XSP', 'PG', 'LULU', 'DE', 'MDT', 'RCL']
@@ -45,30 +45,55 @@
         self.fifteen_days_ago = (datetime.now() - timedelta(days=15)).strftime('%Y-%m-%d')
         self.fifteen_days_from_now = (datetime.now() + timedelta(days=15)).strftime('%Y-%m-%d')
         self.eight_days_from_now = (datetime.now() + timedelta(days=8)).strftime('%Y-%m-%d')
         self.eight_days_ago = (datetime.now() - timedelta(days=8)).strftime('%Y-%m-%d')
         self.timeframes = ['m1','m5', 'm10', 'm15', 'm20', 'm30', 'm60', 'm120', 'm240', 'd1']
         self.now_timestamp_int = int(datetime.now(timezone.utc).timestamp())
         self.day = int(86400)
-        self.headers = {
-        "Access_token": os.environ.get('ACCESS_TOKEN'),
-        "App": "global",
-        "App-Group": "broker",
-        "Appid": "wb_web_app",
-        "Content-Type": "application/json",
-        "Device-Type": "Web",
-        "Did": os.environ.get('DID'),
-        "Hl": "en",
-        "Locale": "eng",
-        "Os": "web",
-        "Osv": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36",
-        "Ph": "Windows Chrome",
-        "Platform": "web",
-        "Referer": "https://app.webull.com/",
+        self.id = 15765933
+        self.headers  = {
+        "Accept": os.getenv("ACCEPT"),
+        "Accept-Encoding": os.getenv("ACCEPT_ENCODING"),
+        "Accept-Language": "en-US,en;q=0.9",
+        'Content-Type': 'application/json',
+        "App": os.getenv("APP"),
+        "App-Group": os.getenv("APP_GROUP"),
+        "Appid": os.getenv("APPID"),
+        "Device-Type": os.getenv("DEVICE_TYPE"),
+        "Did": 'gldaboazf4y28thligawz4a7xamqu91g',
+        "Hl": os.getenv("HL"),
+        "Locale": os.getenv("LOCALE"),
+        "Origin": os.getenv("ORIGIN"),
+        "Os": os.getenv("OS"),
+        "Osv": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36",
+        "Ph": os.getenv("PH"),
+        "Platform": os.getenv("PLATFORM"),
+        "Priority": os.getenv("PRIORITY"),
+        "Referer": os.getenv("REFERER"),
+        "Reqid": os.getenv("REQID"),
+        "T_time": os.getenv("T_TIME"),
+        "Tz": os.getenv("TZ"),
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36",
+        "Ver": os.getenv("VER"),
+        "X-S": os.getenv("X_S"),
+        "X-Sv": os.getenv("X_SV")
     }
+        #miscellaenous
+                #sessions
+        self._account_id = ''
+        self._trade_token = ''
+        self._access_token = ''
+        self._refresh_token = ''
+        self._token_expire = ''
+        self._uuid = ''
+
+        self._region_code = 6
+        self.zone_var = 'dc_core_r001'
+        self.timeout = 15
+        self.device_id = "gldaboazf4y28thligawz4a7xamqu91g"
     async def fetch_endpoint(self, endpoint):
         async with aiohttp.ClientSession(headers=self.headers) as session:
             async with session.get(endpoint) as resp:
                 return await resp.json()
 
     async def get_ticker_id(self, symbol):
         """Converts ticker name to ticker ID to be passed to other API endpoints from Webull."""
@@ -413,14 +438,27 @@
         ticker_id = await self.get_ticker_id(symbol)
         endpoint = f"https://quotes-gw.webullfintech.com/api/information/financial/incomestatement?tickerId={ticker_id}&type=102&fiscalPeriod=1,2,3,4&limit={limit}"
         datas = await self.fetch_endpoint(endpoint)
         data = FinancialStatement(datas)
         return data
     
 
+    async def order_flow(self, symbol:str, type:str='0', count:str='1'):
+        """
+        Gets order flow for tickers
+        """
+        ticker_id = await self.get_ticker_id(symbol)
+        endpoint = f"https://quotes-gw.webullfintech.com/api/stock/capitalflow/stat?count={count}&tickerId={ticker_id}&type={type}"
+
+        async with httpx.AsyncClient(headers=self.headers) as client:
+            data = await client.get(endpoint)
+            data = data.json()
+            return OrderFlow(data)
+    
+
     async def price_streamer(self, symbol:str, type:str='0'):
         """
         Type:
         >>> 0 = today
         >>> 1 = yesterday
         """
         ticker_id = await self.get_ticker_id(symbol)
```

### Comparing `fudstop-2.5.9/fudstop/apis/whale/whale_models.py` & `fudstop-2.6.0/fudstop/apis/whale/whale_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/whale/whale_sdk.py` & `fudstop-2.6.0/fudstop/apis/whale/whale_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/apis/y_finance/yf_sdk.py` & `fudstop-2.6.0/fudstop/apis/y_finance/yf_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/database_/__init__.py` & `fudstop-2.6.0/fudstop/database_/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/autocomp.py` & `fudstop-2.6.0/fudstop/discord_/autocomp.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/bot.py` & `fudstop-2.6.0/fudstop/discord_/bot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/bot_menus/modals/dalle_modal.py` & `fudstop-2.6.0/fudstop/discord_/bot_menus/modals/dalle_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/bot_menus/modals/options_modal.py` & `fudstop-2.6.0/fudstop/discord_/bot_menus/modals/options_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/bot_menus/pagination.py` & `fudstop-2.6.0/fudstop/discord_/bot_menus/pagination.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/__init__.py` & `fudstop-2.6.0/fudstop/discord_/cogs/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/accounting.py` & `fudstop-2.6.0/fudstop/discord_/cogs/accounting.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/assistant.py` & `fudstop-2.6.0/fudstop/discord_/cogs/assistant.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/database.py` & `fudstop-2.6.0/fudstop/discord_/cogs/database.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/earnings.py` & `fudstop-2.6.0/fudstop/discord_/cogs/earnings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/fed_print.py` & `fudstop-2.6.0/fudstop/discord_/cogs/fed_print.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/filter.py` & `fudstop-2.6.0/fudstop/discord_/cogs/filter.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/fiscal_service.py` & `fudstop-2.6.0/fudstop/discord_/cogs/fiscal_service.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/gex.py` & `fudstop-2.6.0/fudstop/discord_/cogs/gex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/gpt.py` & `fudstop-2.6.0/fudstop/discord_/cogs/gpt.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/ibrs.py` & `fudstop-2.6.0/fudstop/discord_/cogs/ibrs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/main_view.py` & `fudstop-2.6.0/fudstop/discord_/cogs/main_view.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/options.py` & `fudstop-2.6.0/fudstop/discord_/cogs/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/plays.py` & `fudstop-2.6.0/fudstop/discord_/cogs/plays.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/register.py` & `fudstop-2.6.0/fudstop/discord_/cogs/register.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/spx.py` & `fudstop-2.6.0/fudstop/discord_/cogs/spx.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/strategy.py` & `fudstop-2.6.0/fudstop/discord_/cogs/strategy.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/ta.py` & `fudstop-2.6.0/fudstop/discord_/cogs/ta.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/weather.py` & `fudstop-2.6.0/fudstop/discord_/cogs/weather.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/webull.py` & `fudstop-2.6.0/fudstop/discord_/cogs/webull.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/cogs/yfin.py` & `fudstop-2.6.0/fudstop/discord_/cogs/yfin.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/database_getter.py` & `fudstop-2.6.0/fudstop/discord_/database_getter.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/discord_rsi.py` & `fudstop-2.6.0/fudstop/discord_/discord_rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/discord_/embeddings.py` & `fudstop-2.6.0/fudstop/discord_/embeddings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/ecfr_test.py` & `fudstop-2.6.0/fudstop/examples/ecfr_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/ofr_test.py` & `fudstop-2.6.0/fudstop/examples/ofr_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/aggregates_second.py` & `fudstop-2.6.0/fudstop/examples/polygonio/aggregates_second.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/company_info.py` & `fudstop-2.6.0/fudstop/examples/polygonio/company_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/get_all_options.py` & `fudstop-2.6.0/fudstop/examples/polygonio/get_all_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/get_near_the_money.py` & `fudstop-2.6.0/fudstop/examples/polygonio/get_near_the_money.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/get_option_aggs.py` & `fudstop-2.6.0/fudstop/examples/polygonio/get_option_aggs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/get_option_rsi.py` & `fudstop-2.6.0/fudstop/examples/polygonio/get_option_rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/get_option_trades.py` & `fudstop-2.6.0/fudstop/examples/polygonio/get_option_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/get_ticker_aggs.py` & `fudstop-2.6.0/fudstop/examples/polygonio/get_ticker_aggs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/market_news.py` & `fudstop-2.6.0/fudstop/examples/polygonio/market_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/polygonio/polygon_test.py` & `fudstop-2.6.0/fudstop/examples/polygonio/polygon_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/scripty.py` & `fudstop-2.6.0/fudstop/examples/scripty.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/stocksera_test.py` & `fudstop-2.6.0/fudstop/examples/stocksera_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/test.py` & `fudstop-2.6.0/fudstop/examples/test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/test_gex.py` & `fudstop-2.6.0/fudstop/examples/test_gex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/test_openai.py` & `fudstop-2.6.0/fudstop/examples/test_openai.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/test_opts.py` & `fudstop-2.6.0/fudstop/examples/test_opts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/test_screener.py` & `fudstop-2.6.0/fudstop/examples/test_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/test_sec.py` & `fudstop-2.6.0/fudstop/examples/test_sec.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/test_webull.py` & `fudstop-2.6.0/fudstop/examples/test_webull.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/webull/markets_example.py` & `fudstop-2.6.0/fudstop/examples/webull/markets_example.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/examples/webull/trade_example.py` & `fudstop-2.6.0/fudstop/examples/webull/trade_example.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/options_filter.py` & `fudstop-2.6.0/fudstop/options_filter.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/plots.py` & `fudstop-2.6.0/fudstop/plots.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop/schema.py` & `fudstop-2.6.0/fudstop/schema.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.5.9/fudstop.egg-info/PKG-INFO` & `fudstop-2.6.0/fudstop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudstop
-Version: 2.5.9
+Version: 2.6.0
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
```

### Comparing `fudstop-2.5.9/fudstop.egg-info/SOURCES.txt` & `fudstop-2.6.0/fudstop.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 fudstop/apis/_pandas/pandas_sdk.py
 fudstop/apis/_selenium/__init__.py
 fudstop/apis/_selenium/selenium_sdk.py
 fudstop/apis/alphaquery/__init__.py
 fudstop/apis/alphaquery/alpha_sdk.py
 fudstop/apis/alphaquery/models/__init__.py
 fudstop/apis/alphaquery/models/alpha_models.py
+fudstop/apis/caselaw/__init__.py
+fudstop/apis/caselaw/caselaw_models.py
+fudstop/apis/caselaw/caselaw_sdk.py
 fudstop/apis/cfr/__init__.py
 fudstop/apis/cfr/cfr_2.0.py
 fudstop/apis/cfr/cfr_helpers.py
 fudstop/apis/cfr/cfr_sdk.py
 fudstop/apis/cfr/title_12.py
 fudstop/apis/datalink/__init__.py
 fudstop/apis/datalink/datalink_sdk.py
@@ -215,14 +218,15 @@
 fudstop/apis/webull/trade_models/cost_distribution.py
 fudstop/apis/webull/trade_models/etf_holdings.py
 fudstop/apis/webull/trade_models/events.py
 fudstop/apis/webull/trade_models/financials.py
 fudstop/apis/webull/trade_models/forecast_evaluator.py
 fudstop/apis/webull/trade_models/institutional_holdings.py
 fudstop/apis/webull/trade_models/news.py
+fudstop/apis/webull/trade_models/order_flow.py
 fudstop/apis/webull/trade_models/price_streamer.py
 fudstop/apis/webull/trade_models/short_interest.py
 fudstop/apis/webull/trade_models/stock_quote.py
 fudstop/apis/webull/trade_models/ticker_query.py
 fudstop/apis/webull/trade_models/volume_analysis.py
 fudstop/apis/webull/trader_models/__init__.py
 fudstop/apis/webull/trader_models/trader_models.py
```

### Comparing `fudstop-2.5.9/fudstop.egg-info/requires.txt` & `fudstop-2.6.0/fudstop.egg-info/requires.txt`

 * *Files identical despite different names*

