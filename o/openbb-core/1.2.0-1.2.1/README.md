# Comparing `tmp/openbb_core-1.2.0.tar.gz` & `tmp/openbb_core-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_core-1.2.0.tar", max compression
+gzip compressed data, was "openbb_core-1.2.1.tar", max compression
```

## Comparing `openbb_core-1.2.0.tar` & `openbb_core-1.2.1.tar`

### file list

```diff
@@ -1,222 +1,243 @@
--rw-r--r--   0        0        0     2302 2023-12-05 14:48:33.326684 openbb_core-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/__init__.py
--rw-r--r--   0        0        0      418 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1945 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     3995 2023-12-11 11:20:42.124620 openbb_core-1.2.0/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     5970 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1181 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2023-12-11 15:22:00.730855 openbb_core-1.2.0/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4201 2023-12-11 15:22:00.730855 openbb_core-1.2.0/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      468 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/api/router/user.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    11058 2023-12-14 14:27:37.011130 openbb_core-1.2.0/openbb_core/app/charting_service.py
--rw-r--r--   0        0        0    15200 2023-12-14 14:27:37.011130 openbb_core-1.2.0/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      292 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/constants.py
--rw-r--r--   0        0        0     5312 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2474 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4076 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2691 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     7984 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2137 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      859 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2047 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      239 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       52 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      411 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      161 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      321 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0      906 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2118 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      346 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3974 2023-12-18 15:08:58.014784 openbb_core-1.2.0/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      577 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/custom_parameter.py
--rw-r--r--   0        0        0      435 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     2064 2023-12-18 15:08:58.014784 openbb_core-1.2.0/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1754 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/fast_api_settings.py
--rw-r--r--   0        0        0     2242 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/hub/features_keys.py
--rw-r--r--   0        0        0      561 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      472 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     4429 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9854 2023-12-12 16:19:00.107613 openbb_core-1.2.0/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1305 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      450 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0       92 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     3806 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      977 2023-11-30 15:38:42.080883 openbb_core-1.2.0/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    16903 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2573 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/query.py
--rw-r--r--   0        0        0    20080 2023-12-18 15:08:58.014784 openbb_core-1.2.0/openbb_core/app/router.py
--rw-r--r--   0        0        0     2352 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10338 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3386 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3024 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7616 2023-12-14 09:43:22.868572 openbb_core-1.2.0/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     1722 2023-12-11 15:22:00.734855 openbb_core-1.2.0/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0      769 2023-12-14 09:43:22.868572 openbb_core-1.2.0/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1717 2023-12-11 15:22:00.734855 openbb_core-1.2.0/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    39930 2023-12-14 09:43:22.880572 openbb_core-1.2.0/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0      407 2023-12-14 09:43:22.884573 openbb_core-1.2.0/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0      811 2023-12-14 09:43:22.888573 openbb_core-1.2.0/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0      339 2023-12-14 09:43:22.888573 openbb_core-1.2.0/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1654 2023-12-14 09:43:22.888573 openbb_core-1.2.0/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     4827 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1477 2023-12-13 10:09:19.526944 openbb_core-1.2.0/openbb_core/app/version.py
--rw-r--r--   0        0        0     2529 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/env.py
--rw-r--r--   0        0        0      170 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0     3330 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     6913 2023-12-11 11:20:42.124620 openbb_core-1.2.0/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1368 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0      924 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3612 2023-11-30 15:38:42.080883 openbb_core-1.2.0/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1778 2023-12-18 15:11:32.721244 openbb_core-1.2.0/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     7031 2023-12-12 16:19:00.107613 openbb_core-1.2.0/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      875 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3417 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0      631 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     7104 2023-12-05 14:48:33.326684 openbb_core-1.2.0/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5913 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     4013 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2956 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2805 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1538 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1301 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2269 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1118 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     5826 2023-12-05 14:48:33.326684 openbb_core-1.2.0/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5184 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0     2536 2023-12-11 11:20:42.124620 openbb_core-1.2.0/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     1569 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4691 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      714 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1127 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     1329 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     2852 2023-12-07 10:00:37.819630 openbb_core-1.2.0/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2208 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      666 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2261 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      424 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     1549 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1026 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1714 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1201 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2378 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1755 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2207 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5654 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1397 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5546 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      992 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1033 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     1383 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      903 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      765 2023-12-07 10:00:37.819630 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3566 2023-11-29 11:52:09.037008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    11088 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1795 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     2053 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      952 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      851 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      953 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1992 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0     1032 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      768 2023-12-07 10:00:37.823630 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      359 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1063 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1283 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0     1005 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      943 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     1839 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/european_index_constituents.py
--rw-r--r--   0        0        0     1350 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/european_indices.py
--rw-r--r--   0        0        0     2448 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1235 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      845 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1198 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1527 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     7841 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     2715 2023-11-30 15:38:42.080883 openbb_core-1.2.0/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1331 2023-12-18 15:08:58.014784 openbb_core-1.2.0/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1204 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     2001 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1317 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1167 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1201 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     1572 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1107 2023-11-30 15:38:42.080883 openbb_core-1.2.0/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2835 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1676 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1269 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1153 2023-12-11 11:19:02.612105 openbb_core-1.2.0/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1167 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     5816 2023-12-05 14:48:33.326684 openbb_core-1.2.0/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4884 2023-12-11 11:20:42.124620 openbb_core-1.2.0/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0     1966 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     1435 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      939 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1693 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3295 2023-12-11 11:20:42.124620 openbb_core-1.2.0/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1544 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1549 2023-12-11 11:20:42.124620 openbb_core-1.2.0/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1791 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0      701 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2094 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1418 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1828 2023-12-18 15:09:00.202818 openbb_core-1.2.0/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1113 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     4079 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1059 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0      981 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2287 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1797 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     2080 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     1462 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     2154 2023-11-30 15:38:42.080883 openbb_core-1.2.0/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      828 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0     1280 2023-11-30 15:38:42.080883 openbb_core-1.2.0/openbb_core/provider/standard_models/sector_news.py
--rw-r--r--   0        0        0      819 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1995 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1476 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      851 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      857 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     2265 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1521 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0     1086 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1101 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      751 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23271 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     1636 2023-12-07 10:00:37.823630 openbb_core-1.2.0/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     1897 2023-12-18 15:09:00.202818 openbb_core-1.2.0/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0      838 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     1161 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     4908 2023-12-11 11:20:42.124620 openbb_core-1.2.0/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1076 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2023-11-30 15:38:42.080883 openbb_core-1.2.0/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     7497 2023-12-18 15:09:00.202818 openbb_core-1.2.0/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2023-11-29 11:52:09.041008 openbb_core-1.2.0/openbb_core/py.typed
--rw-r--r--   0        0        0      815 2023-12-18 16:53:59.224769 openbb_core-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 openbb_core-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-04-02 11:35:59.266636 openbb_core-1.2.1/README.md
+-rw-r--r--   0        0        0       19 2024-04-23 10:22:39.570135 openbb_core-1.2.1/openbb_core/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-25 15:03:16.107506 openbb_core-1.2.1/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-04-23 10:22:39.570481 openbb_core-1.2.1/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-04-23 10:22:39.570645 openbb_core-1.2.1/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-02-29 11:03:36.668814 openbb_core-1.2.1/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-03-01 13:58:22.591666 openbb_core-1.2.1/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4206 2024-04-25 15:03:16.107765 openbb_core-1.2.1/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-04-23 10:22:39.570887 openbb_core-1.2.1/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7189 2024-04-25 15:03:16.107968 openbb_core-1.2.1/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-04-08 12:02:16.491932 openbb_core-1.2.1/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-04-02 11:35:59.267527 openbb_core-1.2.1/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-23 08:46:54.460027 openbb_core-1.2.1/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-04-08 12:02:16.492136 openbb_core-1.2.1/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-03-01 13:58:22.592202 openbb_core-1.2.1/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-04-23 10:22:39.571151 openbb_core-1.2.1/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    19033 2024-05-10 11:33:20.067018 openbb_core-1.2.1/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-04-08 12:02:16.492449 openbb_core-1.2.1/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-04-23 10:22:39.571883 openbb_core-1.2.1/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-04-25 15:03:16.111594 openbb_core-1.2.1/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-04-25 15:03:16.111982 openbb_core-1.2.1/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-04-25 15:03:16.112147 openbb_core-1.2.1/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-04-08 12:02:16.492804 openbb_core-1.2.1/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-04-23 10:22:39.572391 openbb_core-1.2.1/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8326 2024-04-25 15:03:16.112434 openbb_core-1.2.1/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-04-23 10:22:39.572707 openbb_core-1.2.1/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-04-23 10:22:39.572853 openbb_core-1.2.1/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-04-23 10:22:39.572965 openbb_core-1.2.1/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-04-23 10:22:39.573057 openbb_core-1.2.1/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-23 10:22:39.573150 openbb_core-1.2.1/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-23 10:22:39.573260 openbb_core-1.2.1/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-04-23 10:22:39.573351 openbb_core-1.2.1/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-04-23 10:22:39.573483 openbb_core-1.2.1/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-04-23 10:22:39.573585 openbb_core-1.2.1/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-04-25 15:03:16.112659 openbb_core-1.2.1/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1908 2024-04-23 10:22:39.573750 openbb_core-1.2.1/openbb_core/app/model/api_settings.py
+-rw-r--r--   0        0        0     1035 2024-04-25 15:03:16.112814 openbb_core-1.2.1/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-04-08 12:02:16.493305 openbb_core-1.2.1/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-04-23 10:22:39.573965 openbb_core-1.2.1/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3915 2024-05-13 15:41:33.848674 openbb_core-1.2.1/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      502 2024-04-23 10:22:39.574297 openbb_core-1.2.1/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-04-25 15:03:16.113143 openbb_core-1.2.1/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2385 2024-05-10 19:27:56.003979 openbb_core-1.2.1/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1054 2024-04-23 10:22:39.574498 openbb_core-1.2.1/openbb_core/app/model/field.py
+-rw-r--r--   0        0        0      694 2024-04-23 10:22:39.574636 openbb_core-1.2.1/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      474 2024-04-23 10:22:39.574977 openbb_core-1.2.1/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     5669 2024-04-25 15:03:16.113495 openbb_core-1.2.1/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9240 2024-05-10 19:27:56.004268 openbb_core-1.2.1/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1477 2024-05-09 13:34:29.173272 openbb_core-1.2.1/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-04-23 10:22:39.575520 openbb_core-1.2.1/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0      801 2024-04-23 10:22:39.575578 openbb_core-1.2.1/openbb_core/app/model/python_settings.py
+-rw-r--r--   0        0        0       37 2024-04-23 10:22:39.575663 openbb_core-1.2.1/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-04-23 10:22:39.575753 openbb_core-1.2.1/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     4044 2024-04-23 10:22:39.575870 openbb_core-1.2.1/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-04-08 12:02:16.494392 openbb_core-1.2.1/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    21634 2024-05-10 10:40:27.270236 openbb_core-1.2.1/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-04-25 15:03:16.114105 openbb_core-1.2.1/openbb_core/app/query.py
+-rw-r--r--   0        0        0    23086 2024-04-25 15:03:16.114305 openbb_core-1.2.1/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-04-23 10:22:39.576501 openbb_core-1.2.1/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10381 2024-05-14 15:30:05.603980 openbb_core-1.2.1/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3511 2024-04-25 15:03:16.114783 openbb_core-1.2.1/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3064 2024-04-25 15:03:16.114933 openbb_core-1.2.1/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-04-23 10:22:39.576930 openbb_core-1.2.1/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7595 2024-04-23 10:22:39.577041 openbb_core-1.2.1/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2024 2024-04-23 10:22:39.577156 openbb_core-1.2.1/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-04-23 10:22:39.577258 openbb_core-1.2.1/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1948 2024-04-23 10:22:39.577365 openbb_core-1.2.1/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    66879 2024-05-14 15:30:05.604307 openbb_core-1.2.1/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-04-08 12:02:16.496174 openbb_core-1.2.1/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-04-08 12:02:16.496278 openbb_core-1.2.1/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3077 2024-04-25 15:03:16.115099 openbb_core-1.2.1/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2699 2024-05-10 10:40:27.271743 openbb_core-1.2.1/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-04-25 15:03:16.115234 openbb_core-1.2.1/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-04-25 15:03:16.115412 openbb_core-1.2.1/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-04-23 10:22:39.578140 openbb_core-1.2.1/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-04-23 10:22:39.578249 openbb_core-1.2.1/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-04-08 12:02:16.496937 openbb_core-1.2.1/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-29 11:03:36.674333 openbb_core-1.2.1/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-25 15:03:16.115559 openbb_core-1.2.1/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-04-08 12:02:16.497126 openbb_core-1.2.1/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-05-02 09:44:26.753713 openbb_core-1.2.1/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1985 2024-05-14 15:30:05.604736 openbb_core-1.2.1/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2702 2024-05-10 10:40:27.272293 openbb_core-1.2.1/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.674777 openbb_core-1.2.1/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-05-02 09:01:30.398382 openbb_core-1.2.1/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-04-25 15:03:16.115739 openbb_core-1.2.1/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     8297 2024-05-10 10:40:27.272879 openbb_core-1.2.1/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-02-29 11:03:36.675239 openbb_core-1.2.1/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-25 15:03:16.116069 openbb_core-1.2.1/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-04-08 12:02:16.497948 openbb_core-1.2.1/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-04-25 15:03:16.116209 openbb_core-1.2.1/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0     1377 2024-05-09 13:34:29.176884 openbb_core-1.2.1/openbb_core/provider/standard_models/available_indicators.py
+-rw-r--r--   0        0        0      630 2024-04-08 12:02:16.498191 openbb_core-1.2.1/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-04-03 09:25:56.556032 openbb_core-1.2.1/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-04-25 15:03:16.116401 openbb_core-1.2.1/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-04-08 12:02:16.498533 openbb_core-1.2.1/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-04-25 15:03:16.116828 openbb_core-1.2.1/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-04-25 15:03:16.117074 openbb_core-1.2.1/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-04-25 15:03:16.117279 openbb_core-1.2.1/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-04-25 15:03:16.117443 openbb_core-1.2.1/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-04-25 15:03:16.117587 openbb_core-1.2.1/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-04-25 15:03:16.117709 openbb_core-1.2.1/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-04-08 12:02:16.499392 openbb_core-1.2.1/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-04-25 15:03:16.117834 openbb_core-1.2.1/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-04-08 12:02:16.499607 openbb_core-1.2.1/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-04-08 12:02:16.499687 openbb_core-1.2.1/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-04-08 12:02:16.499789 openbb_core-1.2.1/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-05-08 16:35:29.989158 openbb_core-1.2.1/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-04-08 12:02:16.500022 openbb_core-1.2.1/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-04-08 12:02:16.500083 openbb_core-1.2.1/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-04-25 15:03:16.118094 openbb_core-1.2.1/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-02-29 11:03:36.676815 openbb_core-1.2.1/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1246 2024-05-09 13:34:29.177209 openbb_core-1.2.1/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     3722 2024-05-09 13:34:29.177287 openbb_core-1.2.1/openbb_core/provider/standard_models/country_profile.py
+-rw-r--r--   0        0        0     1591 2024-04-25 15:03:16.118591 openbb_core-1.2.1/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-04-23 10:22:39.579222 openbb_core-1.2.1/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-04-25 15:03:16.118756 openbb_core-1.2.1/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-04-08 12:02:16.500724 openbb_core-1.2.1/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-04-25 15:03:16.118894 openbb_core-1.2.1/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      732 2024-05-09 15:04:29.062516 openbb_core-1.2.1/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-04-25 15:03:16.119239 openbb_core-1.2.1/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-04-25 15:03:16.119360 openbb_core-1.2.1/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-04-25 15:03:16.119499 openbb_core-1.2.1/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-04-25 15:03:16.119634 openbb_core-1.2.1/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-04-08 12:02:16.501134 openbb_core-1.2.1/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-04-25 15:03:16.119769 openbb_core-1.2.1/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2125 2024-05-14 15:30:05.604941 openbb_core-1.2.1/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1680 2024-05-09 15:04:29.062707 openbb_core-1.2.1/openbb_core/provider/standard_models/economic_indicators.py
+-rw-r--r--   0        0        0     1750 2024-04-25 15:03:16.120051 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-05-07 10:10:32.921917 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-04-08 12:02:16.501659 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-04-25 15:03:16.120282 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-04-08 12:02:16.501882 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-04-08 12:02:16.502012 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-04-25 15:03:16.120534 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-04-23 10:22:39.579383 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-04-08 12:02:16.502348 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      912 2024-05-09 13:34:29.177837 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-04-08 12:02:16.502654 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-04-08 12:02:16.502786 openbb_core-1.2.1/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-04-08 12:02:16.502907 openbb_core-1.2.1/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-04-08 12:02:16.503093 openbb_core-1.2.1/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-04-08 12:02:16.503199 openbb_core-1.2.1/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-04-08 12:02:16.503299 openbb_core-1.2.1/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-04-08 12:02:16.503410 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1448 2024-05-15 11:17:30.039088 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-04-08 12:02:16.503633 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-04-08 12:02:16.503765 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      939 2024-04-23 10:22:39.580561 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-02-29 11:03:36.679311 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-04-08 12:02:16.503908 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-04-08 12:02:16.504049 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-04-08 12:02:16.504179 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-02-29 11:03:36.679587 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-04-08 12:02:16.504319 openbb_core-1.2.1/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      905 2024-05-15 11:17:30.039210 openbb_core-1.2.1/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-04-08 12:02:16.504572 openbb_core-1.2.1/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-04-08 12:02:16.504687 openbb_core-1.2.1/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-04-08 12:02:16.504804 openbb_core-1.2.1/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-04-08 12:02:16.504912 openbb_core-1.2.1/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-04-08 12:02:16.505036 openbb_core-1.2.1/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-04-08 12:02:16.505143 openbb_core-1.2.1/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-04-08 12:02:16.505225 openbb_core-1.2.1/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2321 2024-04-23 10:22:39.580852 openbb_core-1.2.1/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     1645 2024-05-14 15:30:05.605050 openbb_core-1.2.1/openbb_core/provider/standard_models/forward_pe_estimates.py
+-rw-r--r--   0        0        0     2390 2024-04-23 10:22:39.580922 openbb_core-1.2.1/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-04-03 09:24:18.659331 openbb_core-1.2.1/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-04-08 12:02:16.505455 openbb_core-1.2.1/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-04-08 12:02:16.505531 openbb_core-1.2.1/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-04-08 12:02:16.505610 openbb_core-1.2.1/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-04-08 12:02:16.505708 openbb_core-1.2.1/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-04-08 12:02:16.505795 openbb_core-1.2.1/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-04-08 12:02:16.505879 openbb_core-1.2.1/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-04-08 12:02:16.505957 openbb_core-1.2.1/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-04-08 12:02:16.506053 openbb_core-1.2.1/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-04-08 12:02:16.506140 openbb_core-1.2.1/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-04-08 12:02:16.506219 openbb_core-1.2.1/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-04-08 12:02:16.506314 openbb_core-1.2.1/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-04-08 12:02:16.506419 openbb_core-1.2.1/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-04-08 12:02:16.506533 openbb_core-1.2.1/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-04-08 12:02:16.506619 openbb_core-1.2.1/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-04-08 12:02:16.506718 openbb_core-1.2.1/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-04-08 12:02:16.506824 openbb_core-1.2.1/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-04-08 12:02:16.506908 openbb_core-1.2.1/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-04-08 12:02:16.506989 openbb_core-1.2.1/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-02-29 11:03:36.681716 openbb_core-1.2.1/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-04-08 12:02:16.507066 openbb_core-1.2.1/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-04-08 12:02:16.507183 openbb_core-1.2.1/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-02-29 11:03:36.681951 openbb_core-1.2.1/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-04-08 12:02:16.507267 openbb_core-1.2.1/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-04-08 12:02:16.507425 openbb_core-1.2.1/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-04-03 09:24:18.677029 openbb_core-1.2.1/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-04-08 12:02:16.507566 openbb_core-1.2.1/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-04-08 12:02:16.507677 openbb_core-1.2.1/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-04-08 12:02:16.507774 openbb_core-1.2.1/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-04-08 12:02:16.507840 openbb_core-1.2.1/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-04-08 12:02:16.507922 openbb_core-1.2.1/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-04-08 12:02:16.508020 openbb_core-1.2.1/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-02-29 11:03:36.682563 openbb_core-1.2.1/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-04-08 12:02:16.508134 openbb_core-1.2.1/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-04-08 12:02:16.508236 openbb_core-1.2.1/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-04-08 12:02:16.508327 openbb_core-1.2.1/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-05-09 13:34:29.178067 openbb_core-1.2.1/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-04-08 12:02:16.508525 openbb_core-1.2.1/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-04-08 12:02:16.508617 openbb_core-1.2.1/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-04-08 12:02:16.508712 openbb_core-1.2.1/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-04-23 10:22:39.581171 openbb_core-1.2.1/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-04-08 12:02:16.508945 openbb_core-1.2.1/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-04-08 12:02:16.509044 openbb_core-1.2.1/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-04-08 12:02:16.509150 openbb_core-1.2.1/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-04-08 12:02:16.509243 openbb_core-1.2.1/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-04-08 12:02:16.509331 openbb_core-1.2.1/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-04-02 11:35:59.289085 openbb_core-1.2.1/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-02-29 11:03:36.683510 openbb_core-1.2.1/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-02-29 11:03:36.683639 openbb_core-1.2.1/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-02-29 11:03:36.683703 openbb_core-1.2.1/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-04-08 12:02:16.509420 openbb_core-1.2.1/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-04-08 12:02:16.509468 openbb_core-1.2.1/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-04-08 12:02:16.509556 openbb_core-1.2.1/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-04-08 12:02:16.509643 openbb_core-1.2.1/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-04-08 12:02:16.509724 openbb_core-1.2.1/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-04-08 12:02:16.509820 openbb_core-1.2.1/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-04-23 10:22:39.581294 openbb_core-1.2.1/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-04-08 12:02:16.509962 openbb_core-1.2.1/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-04-08 12:02:16.510053 openbb_core-1.2.1/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-04-08 12:02:16.510132 openbb_core-1.2.1/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-02-29 11:03:36.684333 openbb_core-1.2.1/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-04-08 12:02:16.510225 openbb_core-1.2.1/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-04-08 12:02:16.510364 openbb_core-1.2.1/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3073 2024-05-09 13:34:29.178434 openbb_core-1.2.1/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3526 2024-05-09 15:04:29.062912 openbb_core-1.2.1/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-04-08 12:02:16.510669 openbb_core-1.2.1/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-02-29 11:03:36.684683 openbb_core-1.2.1/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-02-29 11:03:36.684745 openbb_core-1.2.1/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-04-08 12:02:16.510809 openbb_core-1.2.1/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-02-29 11:03:36.684895 openbb_core-1.2.1/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-04-23 10:22:39.581426 openbb_core-1.2.1/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-04-08 12:02:16.511096 openbb_core-1.2.1/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-04-02 11:35:59.291045 openbb_core-1.2.1/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9699 2024-05-02 09:48:24.768519 openbb_core-1.2.1/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.685216 openbb_core-1.2.1/openbb_core/py.typed
+-rw-r--r--   0        0        0      816 2024-05-15 15:58:02.476333 openbb_core-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 openbb_core-1.2.1/PKG-INFO
```

### Comparing `openbb_core-1.2.0/README.md` & `openbb_core-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/api/auth/user.py` & `openbb_core-1.2.1/openbb_core/api/auth/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""User authentication."""
+
 import secrets
 from typing import Optional
 
 from fastapi import Depends, HTTPException, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from openbb_core.app.model.user_settings import UserSettings
 from openbb_core.app.service.user_service import UserService
@@ -11,15 +13,14 @@
 security = HTTPBasic() if Env().API_AUTH else lambda: None
 
 
 async def authenticate_user(
     credentials: Annotated[Optional[HTTPBasicCredentials], Depends(security)]
 ):
     """Authenticate the user."""
-
     if credentials:
         username = Env().API_USERNAME
         password = Env().API_PASSWORD
 
         is_correct_username = False
         is_correct_password = False
```

### Comparing `openbb_core-1.2.0/openbb_core/api/dependency/coverage.py` & `openbb_core-1.2.1/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/api/dependency/system.py` & `openbb_core-1.2.1/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/api/rest_api.py` & `openbb_core-1.2.1/openbb_core/api/rest_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """REST API for the OpenBB Platform."""
+
 import logging
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI, Request
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse
 from openbb_core.api.app_loader import AppLoader
@@ -62,45 +63,53 @@
             "url": s.url,
             "description": s.description,
         }
         for s in system.api_settings.servers
     ],
     lifespan=lifespan,
 )
-
 app.add_middleware(
     CORSMiddleware,
     allow_origins=system.api_settings.cors.allow_origins,
     allow_methods=system.api_settings.cors.allow_methods,
     allow_headers=system.api_settings.cors.allow_headers,
 )
+app.openapi_tags = AppLoader.get_openapi_tags()
 AppLoader.from_routers(
     app=app,
-    routers=[AuthService().router, router_system, router_coverage, router_commands]
-    if Env().DEV_MODE
-    else [router_commands],
+    routers=(
+        [AuthService().router, router_system, router_coverage, router_commands]
+        if Env().DEV_MODE
+        else [router_commands]
+    ),
     prefix=system.api_settings.prefix,
 )
 
 
 @app.exception_handler(Exception)
 async def api_exception_handler(_: Request, exc: Exception):
     """Exception handler for all other exceptions."""
+    if Env().DEBUG_MODE:
+        raise exc
+    logger.error(exc)
     return JSONResponse(
         status_code=404,
         content={
             "detail": str(exc),
             "error_kind": exc.__class__.__name__,
         },
     )
 
 
 @app.exception_handler(OpenBBError)
 async def openbb_exception_handler(_: Request, exc: OpenBBError):
     """Exception handler for OpenBB errors."""
+    if Env().DEBUG_MODE:
+        raise exc
+    logger.error(exc.original)
     openbb_error = exc.original
     status_code = 400 if "No results" in str(openbb_error) else 500
     return JSONResponse(
         status_code=status_code,
         content={
             "detail": str(openbb_error),
             "error_kind": openbb_error.__class__.__name__,
```

### Comparing `openbb_core-1.2.0/openbb_core/api/router/commands.py` & `openbb_core-1.2.1/openbb_core/api/router/commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,35 @@
+"""Commands: generates the command map."""
+
 import inspect
 from functools import partial, wraps
 from inspect import Parameter, Signature, signature
-from typing import Any, Callable, Dict, Tuple, TypeVar
+from typing import Any, Callable, Dict, Optional, Tuple, TypeVar
 
-from fastapi import APIRouter, Depends
+from fastapi import APIRouter, Depends, Header
 from fastapi.routing import APIRoute
-from openbb_core.app.charting_service import ChartingService
 from openbb_core.app.command_runner import CommandRunner
 from openbb_core.app.model.command_context import CommandContext
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.model.user_settings import UserSettings
 from openbb_core.app.router import RouterLoader
 from openbb_core.app.service.auth_service import AuthService
 from openbb_core.app.service.system_service import SystemService
 from openbb_core.app.service.user_service import UserService
 from openbb_core.env import Env
 from pydantic import BaseModel
 from typing_extensions import Annotated, ParamSpec
 
+try:
+    from openbb_charting import Charting
+
+    CHARTING_INSTALLED = True
+except ImportError:
+    CHARTING_INSTALLED = False
+
 T = TypeVar("T")
 P = ParamSpec("P")
 
 router = APIRouter(prefix="")
 
 
 def build_new_annotation_map(sig: Signature) -> Dict[str, Any]:
@@ -39,105 +47,134 @@
 
 def build_new_signature(path: str, func: Callable) -> Signature:
     """Build new function signature."""
     sig = signature(func)
     parameter_list = sig.parameters.values()
     return_annotation = sig.return_annotation
     new_parameter_list = []
-
-    for parameter in parameter_list:
+    var_kw_pos = len(parameter_list)
+    for pos, parameter in enumerate(parameter_list):
         if parameter.name == "cc" and parameter.annotation == CommandContext:
             continue
 
+        if parameter.kind == Parameter.VAR_KEYWORD:
+            # We track VAR_KEYWORD parameter to insert the any additional
+            # parameters we need to add before it and avoid a SyntaxError
+            var_kw_pos = pos
+
         new_parameter_list.append(
             Parameter(
                 parameter.name,
                 kind=parameter.kind,
                 default=parameter.default,
                 annotation=parameter.annotation,
             )
         )
 
-    if (
-        path.replace("/", "_")[1:]
-        in ChartingService.get_implemented_charting_functions()
-    ):
-        new_parameter_list.append(
+    if CHARTING_INSTALLED and path.replace("/", "_")[1:] in Charting.functions():
+        new_parameter_list.insert(
+            var_kw_pos,
             Parameter(
                 "chart",
                 kind=Parameter.POSITIONAL_OR_KEYWORD,
                 default=False,
                 annotation=bool,
-            )
+            ),
         )
+        var_kw_pos += 1
+
+    if custom_headers := SystemService().system_settings.api_settings.custom_headers:
+        for name, default in custom_headers.items():
+            new_parameter_list.insert(
+                var_kw_pos,
+                Parameter(
+                    name.replace("-", "_"),
+                    kind=Parameter.POSITIONAL_OR_KEYWORD,
+                    default=default,
+                    annotation=Annotated[
+                        Optional[str], Header(include_in_schema=False)
+                    ],
+                ),
+            )
+            var_kw_pos += 1
 
     if Env().API_AUTH:
-        new_parameter_list.append(
+        new_parameter_list.insert(
+            var_kw_pos,
             Parameter(
                 "__authenticated_user_settings",
                 kind=Parameter.POSITIONAL_OR_KEYWORD,
                 default=UserSettings(),
                 annotation=Annotated[
                     UserSettings, Depends(AuthService().user_settings_hook)
                 ],
-            )
+            ),
         )
+        var_kw_pos += 1
 
     return Signature(
         parameters=new_parameter_list,
         return_annotation=return_annotation,
     )
 
 
 def validate_output(c_out: OBBject) -> OBBject:
     """
     Validate OBBject object.
+
     Checks against the OBBject schema and removes fields that contain the
     `exclude_from_api` extra `pydantic.Field` kwarg.
     Note that the modification to the `OBBject` object is done in-place.
 
     Parameters
     ----------
     c_out : OBBject
         OBBject object to validate.
 
     Returns
     -------
-    OBBject
-        Validated OBBject object.
+    Dict
+        Serialized OBBject.
     """
 
     def is_model(type_):
         return inspect.isclass(type_) and issubclass(type_, BaseModel)
 
     def exclude_fields_from_api(key: str, value: Any):
         type_ = type(value)
         field = c_out.model_fields.get(key, None)
         json_schema_extra = field.json_schema_extra if field else None
 
         # case where 1st layer field needs to be excluded
-        if json_schema_extra and json_schema_extra.get("exclude_from_api", None):
+        if (
+            json_schema_extra
+            and isinstance(json_schema_extra, dict)
+            and json_schema_extra.get("exclude_from_api", None)
+        ):
             delattr(c_out, key)
 
         # if it's a model with nested fields
         elif is_model(type_):
             for field_name, field in type_.__fields__.items():
-                if field.json_schema_extra and field.json_schema_extra.get(
-                    "exclude_from_api", None
+                extra = getattr(field, "json_schema_extra", None)
+                if (
+                    extra
+                    and isinstance(extra, dict)
+                    and extra.get("exclude_from_api", None)
                 ):
                     delattr(value, field_name)
 
                 # if it's a yet a nested model we need to go deeper in the recursion
-                elif is_model(field.annotation):
+                elif is_model(getattr(field, "annotation", None)):
                     exclude_fields_from_api(field_name, getattr(value, field_name))
 
     for k, v in c_out.model_copy():
         exclude_fields_from_api(k, v)
 
-    return c_out.model_dump()
+    return c_out
 
 
 def build_api_wrapper(
     command_runner: CommandRunner,
     route: APIRoute,
 ) -> Callable:
     """Build API wrapper for a command."""
@@ -147,26 +184,25 @@
     new_signature = build_new_signature(path=path, func=func)
     new_annotations_map = build_new_annotation_map(sig=new_signature)
 
     func.__signature__ = new_signature  # type: ignore
     func.__annotations__ = new_annotations_map
 
     @wraps(wrapped=func)
-    async def wrapper(*args: Tuple[Any], **kwargs: Dict[str, Any]):
+    async def wrapper(*args: Tuple[Any], **kwargs: Dict[str, Any]) -> OBBject:
         user_settings: UserSettings = UserSettings.model_validate(
             kwargs.pop(
                 "__authenticated_user_settings",
                 UserService.read_default_user_settings(),
             )
         )
         execute = partial(command_runner.run, path, user_settings)
         output: OBBject = await execute(*args, **kwargs)
 
-        output = validate_output(output)
-        return output
+        return validate_output(output)
 
     return wrapper
 
 
 def add_command_map(command_runner: CommandRunner, api_router: APIRouter) -> None:
     """Add command map to the API router."""
     plugins_router = RouterLoader.from_extensions()
```

### Comparing `openbb_core-1.2.0/openbb_core/api/router/coverage.py` & `openbb_core-1.2.1/openbb_core/api/router/coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Coverage API router."""
+
 from fastapi import APIRouter, Depends
 from openbb_core.api.dependency.coverage import get_command_map, get_provider_interface
 from openbb_core.app.provider_interface import ProviderInterface
 from openbb_core.app.router import CommandMap
 from typing_extensions import Annotated
 
 router = APIRouter(prefix="/coverage", tags=["Coverage"])
```

### Comparing `openbb_core-1.2.0/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_core-1.2.1/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Coverage API router helper functions."""
+
 from inspect import _empty, signature
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, Type
 
 from openbb_core.app.provider_interface import ProviderInterface
 from pydantic import BaseModel, Field, create_model
 
 if TYPE_CHECKING:
```

### Comparing `openbb_core-1.2.0/openbb_core/api/router/user.py` & `openbb_core-1.2.1/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/app/command_runner.py` & `openbb_core-1.2.1/openbb_core/app/command_runner.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-import warnings
-from contextlib import nullcontext
+"""Command runner module."""
+
+# pylint: disable=R0903
+
 from copy import deepcopy
+from dataclasses import asdict, is_dataclass
 from datetime import datetime
 from inspect import Parameter, signature
 from sys import exc_info
 from time import perf_counter_ns
-from typing import Any, Callable, ContextManager, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type
+from warnings import catch_warnings, showwarning, warn
 
-from pydantic import ConfigDict, create_model
+from pydantic import BaseModel, ConfigDict, create_model
 
-from openbb_core.app.charting_service import ChartingService
 from openbb_core.app.logs.logging_service import LoggingService
 from openbb_core.app.model.abstract.error import OpenBBError
-from openbb_core.app.model.abstract.warning import cast_warning
+from openbb_core.app.model.abstract.warning import OpenBBWarning, cast_warning
 from openbb_core.app.model.command_context import CommandContext
 from openbb_core.app.model.metadata import Metadata
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.app.model.user_settings import UserSettings
-from openbb_core.app.provider_interface import ProviderInterface
+from openbb_core.app.provider_interface import ExtraParams, ProviderInterface
 from openbb_core.app.router import CommandMap
 from openbb_core.app.service.system_service import SystemService
 from openbb_core.app.service.user_service import UserService
 from openbb_core.env import Env
 from openbb_core.provider.utils.helpers import maybe_coroutine, run_async
 
 
 class ExecutionContext:
+    """Execution context."""
+
     def __init__(
         self,
         command_map: CommandMap,
         route: str,
         system_settings: SystemSettings,
         user_settings: UserSettings,
     ) -> None:
+        """Initialize the execution context."""
         self.command_map = command_map
         self.route = route
         self.system_settings = system_settings
         self.user_settings = user_settings
 
 
 class ParametersBuilder:
@@ -141,16 +147,19 @@
             available_providers = ProviderInterface().available_providers
             return available_providers[0] if available_providers else None
 
         def _get_default_provider(
             command_coverage: Dict[str, List[str]],
             route_default: Optional[Dict[str, Optional[str]]],
         ) -> Optional[str]:
-            """Get the default provider for the given route.
-            Either pick it from the user defaults or from the command coverage."""
+            """
+            Get the default provider for the given route.
+
+            Either pick it from the user defaults or from the command coverage.
+            """
             cmd_cov_given_route = command_coverage.get(route, None)
             command_cov_provider = (
                 cmd_cov_given_route[0] if cmd_cov_given_route else None
             )
 
             if route_default:
                 return route_default.get("provider", None) or command_cov_provider  # type: ignore
@@ -167,45 +176,83 @@
                 else _get_first_provider()
             )
             kwargs["provider_choices"] = {"provider": provider}
 
         return kwargs
 
     @staticmethod
+    def _warn_kwargs(
+        extra_params: Dict[str, Any],
+        model: Type[BaseModel],
+    ) -> None:
+        """Warn if kwargs received and ignored by the validation model."""
+        # We only check the extra_params annotation because ignored fields
+        # will always be there
+        annotation = getattr(
+            model.model_fields.get("extra_params", None), "annotation", None
+        )
+        if is_dataclass(annotation) and any(
+            t is ExtraParams for t in getattr(annotation, "__bases__", [])
+        ):
+            valid = asdict(annotation())  # type: ignore
+            for p in extra_params:
+                if "chart_params" in p:
+                    continue
+                if p not in valid:
+                    warn(
+                        message=f"Parameter '{p}' not found.",
+                        category=OpenBBWarning,
+                    )
+
+    @staticmethod
+    def _as_dict(obj: Any) -> Dict[str, Any]:
+        """Safely convert an object to a dict."""
+        try:
+            if isinstance(obj, dict):
+                return obj
+            return asdict(obj) if is_dataclass(obj) else dict(obj)
+        except Exception:
+            return {}
+
+    @staticmethod
     def validate_kwargs(
         func: Callable,
         kwargs: Dict[str, Any],
     ) -> Dict[str, Any]:
-        """Validate kwargs and if possible coerce to the correct type"""
-
-        config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
-
+        """Validate kwargs and if possible coerce to the correct type."""
         sig = signature(func)
         fields = {
             n: (
-                p.annotation,
+                Any if p.annotation is Parameter.empty else p.annotation,
                 ... if p.default is Parameter.empty else p.default,
             )
             for n, p in sig.parameters.items()
         }
-        ValidationModel = create_model(func.__name__, __config__=config, **fields)  # type: ignore
+        # We allow extra fields to return with model with 'cc: CommandContext'
+        config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
+        ValidationModel = create_model(func.__name__, __config__=config, **fields)  # type: ignore  # pylint: disable=C0103
+        # Validate and coerce
         model = ValidationModel(**kwargs)
-        result = dict(model)
-
-        return result
+        ParametersBuilder._warn_kwargs(
+            ParametersBuilder._as_dict(kwargs.get("extra_params", {})),
+            ValidationModel,
+        )
+        return dict(model)
 
+    # pylint: disable=R0913
     @classmethod
     def build(
         cls,
-        args: Tuple[Any],
+        args: Tuple[Any, ...],
         execution_context: ExecutionContext,
         func: Callable,
         route: str,
         kwargs: Dict[str, Any],
     ) -> Dict[str, Any]:
+        """Build the parameters for a function."""
         func = cls.get_polished_func(func=func)
         system_settings = execution_context.system_settings
         user_settings = execution_context.user_settings
         command_map = execution_context.command_map
 
         kwargs = cls.merge_args_and_kwargs(
             func=func,
@@ -221,135 +268,168 @@
         kwargs = cls.update_provider_choices(
             func=func,
             command_coverage=command_map.command_coverage,
             route=route,
             kwargs=kwargs,
             route_default=user_settings.defaults.routes.get(route, None),
         )
-        kwargs = cls.validate_kwargs(func=func, kwargs=kwargs)
+        kwargs = cls.validate_kwargs(
+            func=func,
+            kwargs=kwargs,
+        )
         return kwargs
 
 
+# pylint: disable=too-few-public-methods
 class StaticCommandRunner:
+    """Static Command Runner."""
+
     @classmethod
-    async def _command(cls, func: Callable, kwargs: Dict[str, Any]) -> OBBject:
-        """Run a command and return the output"""
-        context_manager: Union[warnings.catch_warnings, ContextManager[None]] = (
-            warnings.catch_warnings(record=True)
-            if not Env().DEBUG_MODE
-            else nullcontext()
+    async def _command(
+        cls,
+        func: Callable,
+        kwargs: Dict[str, Any],
+        show_warnings: bool = True,  # pylint: disable=unused-argument   # type: ignore
+    ) -> OBBject:
+        """Run a command and return the output."""
+        obbject = await maybe_coroutine(func, **kwargs)
+        obbject.provider = getattr(
+            kwargs.get("provider_choices", None), "provider", None
         )
-
-        with context_manager as warning_list:
-            obbject = await maybe_coroutine(func, **kwargs)
-
-            obbject.provider = getattr(
-                kwargs.get("provider_choices", None), "provider", None
-            )
-
-            if warning_list:
-                obbject.warnings = list(map(cast_warning, warning_list))
-
         return obbject
 
     @classmethod
     def _chart(
         cls,
         obbject: OBBject,
-        user_settings: UserSettings,
-        system_settings: SystemSettings,
-        route: str,
         **kwargs,
     ) -> None:
         """Create a chart from the command output."""
-        cs = ChartingService(
-            user_settings=user_settings, system_settings=system_settings
-        )
-        obbject.chart = cs.chart(
-            user_settings=user_settings,
-            system_settings=system_settings,
-            route=route,
-            obbject_item=obbject.results,
-            **kwargs,
-        )
+        try:
+            if "charting" not in obbject.accessors:
+                raise OpenBBError(
+                    "Charting is not installed. Please install `openbb-charting`."
+                )
+            chart_params = {}
+            extra_params = kwargs.get("extra_params", {})
+
+            if hasattr(extra_params, "__dict__") and hasattr(
+                extra_params, "chart_params"
+            ):
+                chart_params = kwargs["extra_params"].__dict__.get("chart_params", {})
+            elif isinstance(extra_params, dict) and "chart_params" in extra_params:
+                chart_params = kwargs["extra_params"].get("chart_params", {})
+
+            if "chart_params" in kwargs and kwargs["chart_params"] is not None:
+                chart_params.update(kwargs.pop("chart_params", {}))
+
+            if (
+                "kwargs" in kwargs
+                and "chart_params" in kwargs["kwargs"]
+                and kwargs["kwargs"].get("chart_params") is not None
+            ):
+                chart_params.update(kwargs.pop("kwargs", {}).get("chart_params", {}))
+
+            if chart_params:
+                kwargs.update(chart_params)
+            obbject.charting.show(render=False, **kwargs)
+        except Exception as e:  # pylint: disable=broad-exception-caught
+            if Env().DEBUG_MODE:
+                raise OpenBBError(e) from e
+            warn(str(e), OpenBBWarning)
 
+    # pylint: disable=R0913, R0914
     @classmethod
     async def _execute_func(
         cls,
         route: str,
-        args: Tuple[Any],
+        args: Tuple[Any, ...],
         execution_context: ExecutionContext,
         func: Callable,
         kwargs: Dict[str, Any],
     ) -> OBBject:
-        """Execute a function and return the output"""
+        """Execute a function and return the output."""
         user_settings = execution_context.user_settings
         system_settings = execution_context.system_settings
 
-        # If we're on Jupyter we need to pop here because we will lose "chart" after
-        # ParametersBuilder.build. This needs to be fixed in a way that chart is
-        # added to the function signature and shared for jupyter and api
-        # We can check in the router decorator if the given function has a chart
-        # in the charting extension then we add it there. This way we can remove
-        # the chart parameter from the commands.py and package_builder, it will be
-        # added to the function signature in the router decorator
-        chart = kwargs.pop("chart", False)
+        with catch_warnings(record=True) as warning_list:
+            # If we're on Jupyter we need to pop here because we will lose "chart" after
+            # ParametersBuilder.build. This needs to be fixed in a way that chart is
+            # added to the function signature and shared for jupyter and api
+            # We can check in the router decorator if the given function has a chart
+            # in the charting extension then we add it there. This way we can remove
+            # the chart parameter from the commands.py and package_builder, it will be
+            # added to the function signature in the router decorator
+            chart = kwargs.pop("chart", False)
 
-        kwargs = ParametersBuilder.build(
-            args=args,
-            execution_context=execution_context,
-            func=func,
-            route=route,
-            kwargs=kwargs,
-        )
-
-        # If we're on the api we need to remove "chart" here because the parameter is added on
-        # commands.py and the function signature does not expect "chart"
-        kwargs.pop("chart", None)
-
-        try:
-            obbject = await cls._command(
+            kwargs = ParametersBuilder.build(
+                args=args,
+                execution_context=execution_context,
                 func=func,
+                route=route,
                 kwargs=kwargs,
             )
 
-            if chart and obbject.results:
-                cls._chart(
-                    obbject=obbject,
+            # If we're on the api we need to remove "chart" here because the parameter is added on
+            # commands.py and the function signature does not expect "chart"
+            kwargs.pop("chart", None)
+            # We also pop custom headers
+            model_headers = system_settings.api_settings.custom_headers or {}
+            custom_headers = {
+                name: kwargs.pop(name.replace("-", "_"), default)
+                for name, default in model_headers.items() or {}
+            } or None
+
+            try:
+                obbject = await cls._command(func, kwargs)
+                # pylint: disable=protected-access
+                obbject._route = route
+                obbject._standard_params = kwargs.get("standard_params", None)
+                if chart and obbject.results:
+                    cls._chart(obbject, **kwargs)
+
+            except Exception as e:
+                raise OpenBBError(e) from e
+            finally:
+                ls = LoggingService(system_settings, user_settings)
+                ls.log(
                     user_settings=user_settings,
                     system_settings=system_settings,
                     route=route,
-                    **kwargs,
+                    func=func,
+                    kwargs=kwargs,
+                    exec_info=exc_info(),
+                    custom_headers=custom_headers,
                 )
 
-        except Exception as e:
-            raise OpenBBError(e) from e
-        finally:
-            ls = LoggingService(
-                user_settings=user_settings, system_settings=system_settings
-            )
-            ls.log(
-                user_settings=user_settings,
-                system_settings=system_settings,
-                route=route,
-                func=func,
-                kwargs=kwargs,
-                exec_info=exc_info(),
-            )
-
+        if warning_list:
+            obbject.warnings = []
+            for w in warning_list:
+                obbject.warnings.append(cast_warning(w))
+                if user_settings.preferences.show_warnings:
+                    showwarning(
+                        message=w.message,
+                        category=w.category,
+                        filename=w.filename,
+                        lineno=w.lineno,
+                        file=w.file,
+                        line=w.line,
+                    )
         return obbject
 
+    # pylint: disable=W0718
     @classmethod
     async def run(
         cls,
         execution_context: ExecutionContext,
         /,
         *args,
         **kwargs,
     ) -> OBBject:
+        """Run a command and return the OBBject as output."""
         timestamp = datetime.now()
         start_ns = perf_counter_ns()
 
         command_map = execution_context.command_map
         route = execution_context.route
 
         if func := command_map.get_command(route=route):
@@ -372,52 +452,59 @@
                     duration=duration,
                     route=route,
                     timestamp=timestamp,
                 )
             except Exception as e:
                 if Env().DEBUG_MODE:
                     raise OpenBBError(e) from e
+                warn(str(e), OpenBBWarning)
 
         return obbject
 
 
 class CommandRunner:
+    """Command runner."""
+
     def __init__(
         self,
         command_map: Optional[CommandMap] = None,
         system_settings: Optional[SystemSettings] = None,
         user_settings: Optional[UserSettings] = None,
     ) -> None:
+        """Initialize the command runner."""
         self._command_map = command_map or CommandMap()
         self._system_settings = system_settings or SystemService().system_settings
         self._user_settings = user_settings or UserService.read_default_user_settings()
 
-        self._logging_service = LoggingService(
-            system_settings=self._system_settings, user_settings=self._user_settings
-        )
-        self._charting_service = ChartingService(
+    def init_logging_service(self) -> None:
+        """Initialize the logging service."""
+        _ = LoggingService(
             system_settings=self._system_settings, user_settings=self._user_settings
         )
 
     @property
     def command_map(self) -> CommandMap:
+        """Command map."""
         return self._command_map
 
     @property
     def system_settings(self) -> SystemSettings:
+        """System settings."""
         return self._system_settings
 
     @property
     def user_settings(self) -> UserSettings:
+        """User settings."""
         return self._user_settings
 
     @user_settings.setter
     def user_settings(self, user_settings: UserSettings) -> None:
         self._user_settings = user_settings
 
+    # pylint: disable=W1113
     async def run(
         self,
         route: str,
         user_settings: Optional[UserSettings] = None,
         /,
         *args,
         **kwargs,
@@ -430,14 +517,15 @@
             route=route,
             system_settings=self._system_settings,
             user_settings=self._user_settings,
         )
 
         return await StaticCommandRunner.run(execution_context, *args, **kwargs)
 
+    # pylint: disable=W1113
     def sync_run(
         self,
         route: str,
         user_settings: Optional[UserSettings] = None,
         /,
         *args,
         **kwargs,
```

### Comparing `openbb_core-1.2.0/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_core-1.2.1/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,167 +1,179 @@
-# IMPORTATION STANDARD
+"""Logging Formatter that includes formatting of Exceptions."""
+
 import logging
 import re
 from copy import deepcopy
 from pathlib import Path
 
-# IMPORTATION THIRDPARTY
-# IMPORTATION INTERNAL
 from openbb_core.app.logs.models.logging_settings import LoggingSettings
 
 
 class FormatterWithExceptions(logging.Formatter):
-    """Logging Formatter that includes formatting of Exceptions"""
+    """Logging Formatter that includes formatting of Exceptions."""
 
     DATEFORMAT = "%Y-%m-%dT%H:%M:%S%z"
     LOGFORMAT = "%(asctime)s|%(name)s|%(funcName)s|%(lineno)s|%(message)s"
     LOGPREFIXFORMAT = (
         "%(levelname)s|%(appName)s|%(commitHash)s|%(appId)s|%(sessionId)s|%(userId)s|"
     )
 
     @staticmethod
     def calculate_level_name(record: logging.LogRecord) -> str:
+        """Calculate the level name of the log record."""
         if record.exc_text:
             level_name = "X"
         elif record.levelname:
             level_name = record.levelname[0]
         else:
             level_name = "U"
 
         return level_name
 
     @staticmethod
     def extract_log_extra(record: logging.LogRecord):
+        """Extract extra log information from the record."""
         log_extra = dict()
 
         if hasattr(record, "func_name_override"):
             record.funcName = record.func_name_override  # type: ignore
             record.lineno = 0
 
         if hasattr(record, "session_id"):
             log_extra["sessionId"] = record.session_id  # type: ignore
 
         return log_extra
 
     @staticmethod
     def mock_ipv4(text: str) -> str:
+        """Mock IPv4 addresses in the text."""
         pattern = r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}"
         replacement = " FILTERED_IP "
         text_mocked = re.sub(pattern, replacement, text)
 
         return text_mocked
 
     @staticmethod
     def mock_email(text: str) -> str:
+        """Mock email addresses in the text."""
         pattern = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b"
         replacement = " FILTERED_EMAIL "
         text_mocked = re.sub(pattern, replacement, text)
 
         return text_mocked
 
     @staticmethod
     def mock_password(text: str) -> str:
+        """Mock passwords in the text."""
         pattern = r'("password": ")[^"]+'
         replacement = r"\1 FILTERED_PASSWORD "
         text_mocked = re.sub(pattern, replacement, text)
         return text_mocked
 
     @staticmethod
     def mock_flair(text: str) -> str:
+        """Mock flair in the text."""
         pattern = r'("FLAIR": "\[)(.*?)\]'
         replacement = r"\1 FILTERED_FLAIR ]"
         text_mocked = re.sub(pattern, replacement, text)
 
         return text_mocked
 
     @staticmethod
     def mock_home_directory(text: str) -> str:
+        """Mock home directory in the text."""
         user_home_directory = str(Path.home().as_posix())
         text_mocked = text.replace("\\", "/").replace(
             user_home_directory, "MOCKING_USER_PATH"
         )
 
         return text_mocked
 
     @staticmethod
     def filter_special_tags(text: str) -> str:
+        """Filter special tags in the text."""
         text_filtered = text.replace("\n", " MOCKING_BREAKLINE ")
         text_filtered = text_filtered.replace("'Traceback", "Traceback")
 
         return text_filtered
 
     @classmethod
     def filter_piis(cls, text: str) -> str:
+        """Filter Personally Identifiable Information in the text."""
         text_filtered = cls.mock_ipv4(text=text)
         text_filtered = cls.mock_email(text=text_filtered)
         text_filtered = cls.mock_password(text=text_filtered)
         text_filtered = cls.mock_home_directory(text=text_filtered)
         text_filtered = cls.mock_flair(text=text_filtered)
 
         return text_filtered
 
     @classmethod
     def filter_log_line(cls, text: str):
+        """Filter log line."""
         text_filtered = cls.filter_special_tags(text=text)
         text_filtered = cls.filter_piis(text=text_filtered)
 
         return text_filtered
 
     # OVERRIDE
     def __init__(
         self,
         settings: LoggingSettings,
         style="%",
         validate=True,
     ) -> None:
+        """Initialize the FormatterWithExceptions."""
         super().__init__(
             fmt=self.LOGFORMAT,
             datefmt=self.DATEFORMAT,
             style=style,
             validate=validate,
         )
         self.settings = settings
 
     @property
     def settings(self) -> LoggingSettings:
+        """Get the settings."""
         return deepcopy(self.__settings)
 
     @settings.setter
     def settings(self, settings: LoggingSettings) -> None:
+        """Set the settings."""
         self.__settings = settings
 
     # OVERRIDE
     def formatException(self, ei) -> str:
-        """Exception formatting handler
+        """Define the Exception formatting handler.
+
         Parameters
         ----------
         ei : logging._SysExcInfoType
             Exception to be logged
         Returns
         ----------
         str
             Formatted exception
         """
-
         result = super().formatException(ei)
         return repr(result)
 
     # OVERRIDE
     def format(self, record: logging.LogRecord) -> str:
-        """Log formatter
+        """Define the Log formatter.
+
         Parameters
         ----------
         record : logging.LogRecord
             Logging record
         Returns
         ----------
         str
             Formatted_log message
         """
-
         level_name = self.calculate_level_name(record=record)
         log_prefix_content = {
             "appName": self.settings.app_name,
             "levelname": level_name,
             "appId": self.settings.app_id,
             "sessionId": self.settings.session_id,
             "commitHash": "unknown-commit",
```

### Comparing `openbb_core-1.2.0/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_core-1.2.1/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,97 @@
-# IMPORT STANDARD
+"""Posthog Handler."""
+
 import json
 import logging
 import re
-import warnings
 from copy import deepcopy
 from enum import Enum
 from typing import Any, Dict
 
+import posthog
 from openbb_core.app.logs.formatters.formatter_with_exceptions import (
     FormatterWithExceptions,
 )
 from openbb_core.app.logs.models.logging_settings import LoggingSettings
 from openbb_core.env import Env
-from posthog import Posthog
-
-openbb_posthog = Posthog(
-    "phc_6FXLqu4uW9yxfyN8DpPdgzCdlYXOmIWdMGh6GnBgJLX",  # pragma: allowlist secret
-    host="https://app.posthog.com",
-)
 
 
 class PosthogHandler(logging.Handler):
-    """Posthog Handler"""
+    """Posthog Handler."""
 
     class AllowedEvents(Enum):
-        """Allowed Posthog Events"""
+        """Allowed Posthog Events."""
 
         log_startup = "log_startup"
         log_cmd = "log_cmd"
         log_error = "log_error"
         log_warning = "log_warning"
 
     def __init__(self, settings: LoggingSettings):
+        """Initialize Posthog Handler."""
         super().__init__()
         self._settings = settings
         self.logged_in = False
+        posthog.api_key = "phc_6FXLqu4uW9yxfyN8DpPdgzCdlYXOmIWdMGh6GnBgJLX"  # pragma: allowlist secret
+        posthog.host = "https://app.posthog.com"
 
     @property
     def settings(self) -> LoggingSettings:
+        """Get logging settings."""
         return deepcopy(self._settings)
 
     @settings.setter
     def settings(self, settings: LoggingSettings) -> None:
+        """Set logging settings."""
         self._settings = settings
 
     def emit(self, record: logging.LogRecord):
+        """Emit log record."""
         try:
             self.send(record=record)
-        except Exception:
+        except Exception as e:
             self.handleError(record)
+            if Env().DEBUG_MODE:
+                raise e
+
+    def distinct_id(self) -> str:
+        """Get distinct id."""
+        return self._settings.user_id or self._settings.app_id
+
+    def identify(self) -> None:
+        """Identify user."""
+        if self.logged_in or not self._settings.user_id:
+            return
+
+        posthog.identify(
+            self._settings.user_id,
+            {
+                "email": self._settings.user_email,
+                "primaryUsage": self._settings.user_primary_usage,
+            },
+        )
+
+        if self._settings.sub_app_name == "pro":
+            return
+
+        self.logged_in = True
+        posthog.alias(self._settings.user_id, self._settings.app_id)
 
     def log_to_dict(self, log_info: str) -> dict:
-        """Log to dict"""
+        """Log to dict."""
         log_regex = r"(STARTUP|CMD|ERROR): (.*)"
         log_dict: Dict[str, Any] = {}
 
         for log in re.findall(log_regex, log_info):
             log_dict[log[0]] = json.loads(log[1])
 
         return log_dict
 
     def send(self, record: logging.LogRecord):
-        """Send log record to Posthog"""
-
+        """Send log record to Posthog."""
         level_name = logging.getLevelName(record.levelno)
         log_line = FormatterWithExceptions.filter_log_line(text=record.getMessage())
 
         log_extra = self.extract_log_extra(record=record)
         log_extra.update(dict(level=level_name, message=log_line))
         event_name = f"log_{level_name.lower()}"
 
@@ -79,36 +104,19 @@
 
         if re.match(r"^(QUEUE|START|END|INPUT:)", log_line) and not log_dict:
             return
 
         if event_name not in [e.value for e in self.AllowedEvents]:
             return
 
-        if not self.logged_in and self._settings.user_id:
-            self.logged_in = True
-            openbb_posthog.identify(
-                self._settings.user_id,
-                {
-                    "email": self._settings.user_email,
-                    "primaryUsage": self._settings.user_primary_usage,
-                },
-            )
-            openbb_posthog.alias(self._settings.user_id, self._settings.app_id)
-
-        result = openbb_posthog.capture(
-            self._settings.app_id,
-            event_name,
-            properties=log_extra,
-        )
-        if Env().DEBUG_MODE:
-            warnings.warn(result)
+        self.identify()
+        posthog.capture(self.distinct_id(), event_name, properties=log_extra)
 
     def extract_log_extra(self, record: logging.LogRecord) -> Dict[str, Any]:
-        """Extract log extra from record"""
-
+        """Extract log extra from record."""
         log_extra: Dict[str, Any] = {
             "appName": self._settings.app_name,
             "subAppName": self._settings.sub_app_name,
             "appId": self._settings.app_id,
             "sessionId": self._settings.session_id,
             "platform": self._settings.platform,
             "pythonVersion": self._settings.python_version,
```

### Comparing `openbb_core-1.2.0/openbb_core/app/logs/handlers_manager.py` & `openbb_core-1.2.1/openbb_core/app/logs/handlers_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# IMPORT STANDARD
+"""Handlers Manager."""
+
 import logging
 import sys
 
-# IMPORT THIRD-PARTY
-# IMPORT INTERNAL
 from openbb_core.app.logs.formatters.formatter_with_exceptions import (
     FormatterWithExceptions,
 )
 from openbb_core.app.logs.handlers.path_tracking_file_handler import (
     PathTrackingFileHandler,
 )
 from openbb_core.app.logs.handlers.posthog_handler import PosthogHandler
 from openbb_core.app.logs.models.logging_settings import LoggingSettings
 
 
 class HandlersManager:
+    """Handlers Manager."""
+
     def __init__(self, settings: LoggingSettings):
+        """Initialize the HandlersManager."""
         self._handlers = settings.handler_list
         self._settings = settings
 
         for handler_type in self._handlers:
             if handler_type == "stdout":
                 self._add_stdout_handler()
             elif handler_type == "stderr":
@@ -30,42 +32,48 @@
                 self._add_file_handler()
             elif handler_type == "posthog":
                 self._add_posthog_handler()
             else:
                 logging.getLogger().debug("Unknown log handler.")
 
     def _add_posthog_handler(self):
+        """Add a Posthog handler."""
         handler = PosthogHandler(settings=self._settings)
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def _add_stdout_handler(self):
+        """Add a stdout handler."""
         handler = logging.StreamHandler(sys.stdout)
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def _add_stderr_handler(self):
+        """Add a stderr handler."""
         handler = logging.StreamHandler(sys.stderr)
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def _add_noop_handler(self):
+        """Add a null handler."""
         handler = logging.NullHandler()
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def _add_file_handler(self):
+        """Add a file handler."""
         handler = PathTrackingFileHandler(settings=self._settings)
         formatter = FormatterWithExceptions(settings=self._settings)
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
     def update_handlers(self, settings: LoggingSettings):
+        """Update the handlers with new settings."""
         logger = logging.getLogger()
         for hdlr in logger.handlers:
             if isinstance(hdlr, (PathTrackingFileHandler, PosthogHandler)):
                 hdlr.settings = settings
                 hdlr.formatter.settings = settings  # type: ignore
```

### Comparing `openbb_core-1.2.0/openbb_core/app/logs/logging_service.py` & `openbb_core-1.2.1/openbb_core/app/logs/logging_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+"""Logging Service Module."""
+
 import json
 import logging
 from enum import Enum
 from types import TracebackType
-from typing import Any, Callable, Dict, Optional, Tuple, Type, cast
+from typing import Any, Callable, Dict, Optional, Tuple, Type, Union, cast
 
 from openbb_core.app.logs.formatters.formatter_with_exceptions import (
     FormatterWithExceptions,
 )
 from openbb_core.app.logs.handlers_manager import HandlersManager
 from openbb_core.app.logs.models.logging_settings import LoggingSettings
 from openbb_core.app.model.abstract.error import OpenBBError
 from openbb_core.app.model.abstract.singleton import SingletonMeta
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.app.model.user_settings import UserSettings
 from pydantic_core import to_jsonable_python
 
 
 class LoggingService(metaclass=SingletonMeta):
-    """
-    Logging Manager class responsible for managing logging settings and handling logs.
+    """Logging Manager class responsible for managing logging settings and handling logs.
 
     Attributes
     ----------
     _user_settings : Optional[UserSettings]
         User Settings object.
     _system_settings : Optional[SystemSettings]
         System Settings object.
@@ -53,16 +54,16 @@
     """
 
     def __init__(
         self,
         system_settings: SystemSettings,
         user_settings: UserSettings,
     ) -> None:
-        """
-        Logging Manager Constructor
+        """Define the Logging Service Constructor.
+
         Sets up the logging settings and handlers and then logs the startup information.
 
         Parameters
         ----------
         system_settings : SystemSettings
             System Settings, by default None
         user_settings : UserSettings
@@ -75,43 +76,40 @@
             system_settings=self._system_settings,
         )
         self._handlers_manager = self._setup_handlers()
         self._log_startup()
 
     @property
     def logging_settings(self) -> LoggingSettings:
-        """
-        Current logging settings.
+        """Define the Current logging settings.
 
         Returns
         -------
         LoggingSettings
             LoggingSettings object containing the current logging settings.
         """
         return self._logging_settings
 
     @logging_settings.setter
     def logging_settings(self, value: Tuple[SystemSettings, UserSettings]):
-        """
-        Setter for updating the logging settings.
+        """Define the Setter for updating the logging settings.
 
         Parameters
         ----------
         value : Tuple[SystemSettings, UserSettings]
             Tuple containing updated SystemSettings and UserSettings.
         """
         system_settings, user_settings = value
         self._logging_settings = LoggingSettings(
             user_settings=user_settings,
             system_settings=system_settings,
         )
 
     def _setup_handlers(self) -> HandlersManager:
-        """
-        Setup Logging Handlers.
+        """Set up Logging Handlers.
 
         Returns
         -------
         HandlersManager
             Handlers Manager object.
         """
         logger = logging.getLogger(__name__)
@@ -131,28 +129,32 @@
             "LOGFORMAT: %s%s",
             FormatterWithExceptions.LOGPREFIXFORMAT.replace("|", "-"),
             FormatterWithExceptions.LOGFORMAT.replace("|", "-"),
         )
 
         return handlers_manager
 
-    def _log_startup(self, route: Optional[str] = None) -> None:
-        """
-        Log startup information.
-        """
+    def _log_startup(
+        self,
+        route: Optional[str] = None,
+        custom_headers: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        """Log startup information."""
 
         def check_credentials_defined(credentials: Dict[str, Any]):
             class CredentialsDefinition(Enum):
                 defined = "defined"
                 undefined = "undefined"
 
             return {
-                c: CredentialsDefinition.defined.value
-                if credentials[c]
-                else CredentialsDefinition.undefined.value
+                c: (
+                    CredentialsDefinition.defined.value
+                    if credentials[c]
+                    else CredentialsDefinition.undefined.value
+                )
                 for c in credentials
             }
 
         logger = logging.getLogger(__name__)
         logger.info(
             "STARTUP: %s ",
             json.dumps(
@@ -161,29 +163,32 @@
                     "PREFERENCES": self._user_settings.preferences,
                     "KEYS": check_credentials_defined(
                         self._user_settings.credentials.model_dump()
                         if self._user_settings.credentials
                         else {}
                     ),
                     "SYSTEM": self._system_settings,
+                    "custom_headers": custom_headers,
                 },
                 default=to_jsonable_python,
             ),
         )
 
     def log(
         self,
         user_settings: UserSettings,
         system_settings: SystemSettings,
         route: str,
         func: Callable,
         kwargs: Dict[str, Any],
-        exec_info: Optional[
-            Tuple[Type[BaseException], BaseException, Optional[TracebackType]]
-        ] = None,
+        exec_info: Union[
+            Tuple[Type[BaseException], BaseException, TracebackType],
+            Tuple[None, None, None],
+        ],
+        custom_headers: Optional[Dict[str, Any]] = None,
     ):
         """
         Log command output and relevant information.
 
         Parameters
         ----------
         user_settings : UserSettings
@@ -204,15 +209,15 @@
         self._logging_settings = LoggingSettings(
             user_settings=self._user_settings,
             system_settings=self._system_settings,
         )
         self._handlers_manager.update_handlers(self._logging_settings)
 
         if "login" in route:
-            self._log_startup(route)
+            self._log_startup(route, custom_headers)
         else:
             logger = logging.getLogger(__name__)
 
             # Remove CommandContext if any
             kwargs.pop("cc", None)
 
             # Truncate kwargs if too long
@@ -226,14 +231,15 @@
             # Construct message
             message_label = "ERROR" if openbb_error else "CMD"
             log_message = json.dumps(
                 {
                     "route": route,
                     "input": kwargs,
                     "error": str(openbb_error.original) if openbb_error else None,
+                    "custom_headers": custom_headers,
                 },
                 default=to_jsonable_python,
             )
             log_message = f"{message_label}: {log_message}"
 
             log_level = logger.error if openbb_error else logger.info
             log_level(
```

### Comparing `openbb_core-1.2.0/openbb_core/app/logs/models/logging_settings.py` & `openbb_core-1.2.1/openbb_core/app/logs/models/logging_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+"""Logging settings."""
+
 from pathlib import Path
 from typing import List, Optional
 
 from openbb_core.app.logs.utils.utils import get_app_id, get_log_dir, get_session_id
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.app.model.user_settings import UserSettings
 
 
 # pylint: disable=too-many-instance-attributes
 class LoggingSettings:
+    """Logging settings."""
+
     def __init__(
         self,
         user_settings: Optional[UserSettings] = None,
         system_settings: Optional[SystemSettings] = None,
     ):
+        """Initialize the logging settings."""
         user_settings = user_settings or UserSettings()
         system_settings = system_settings or SystemSettings()
 
         user_data_directory = (
             str(Path.home() / "OpenBBUserData")
             if not user_settings.preferences
             else user_settings.preferences.data_directory
```

### Comparing `openbb_core-1.2.0/openbb_core/app/logs/utils/utils.py` & `openbb_core-1.2.1/openbb_core/app/logs/utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# IMPORT STANDARD
+"""Utility functions for logging."""
+
 import time
 import uuid
 import warnings
 from pathlib import Path, PosixPath
 
-# IMPORT THIRD-PARTY
-# IMPORT INTERNAL
-
 
 def get_session_id() -> str:
     """UUID of the current session."""
     session_id = str(uuid.uuid4()) + "-" + str(int(time.time()))
     return session_id
 
 
@@ -37,36 +35,40 @@
     logging_uuid = create_log_uuid_if_not_exists(log_dir)
     uuid_log_dir = create_uuid_dir_if_not_exists(log_dir, logging_uuid)
 
     return uuid_log_dir
 
 
 def create_log_dir_if_not_exists(contextual_user_data_directory: str) -> Path:
+    """Create a log directory for the current installation."""
     log_dir = Path(contextual_user_data_directory).joinpath("logs").absolute()
     if not log_dir.is_dir():
         log_dir.mkdir(parents=True, exist_ok=True)
 
     return log_dir
 
 
 def create_log_uuid_if_not_exists(log_dir: Path) -> str:
+    """Create a log id file for the current logging session."""
     log_id = get_log_id(log_dir)
     if not log_id.is_file():
         logging_id = f"{uuid.uuid4()}"
         log_id.write_text(logging_id, encoding="utf-8")
     else:
         logging_id = log_id.read_text(encoding="utf-8").rstrip()
 
     return logging_id
 
 
 def get_log_id(log_dir):
+    """Get the log id file."""
     return (log_dir / ".logid").absolute()
 
 
 def create_uuid_dir_if_not_exists(log_dir, logging_id) -> PosixPath:
+    """Create a directory for the current logging session."""
     uuid_log_dir = (log_dir / logging_id).absolute()
 
     if not uuid_log_dir.is_dir():
         uuid_log_dir.mkdir(parents=True, exist_ok=True)
 
     return uuid_log_dir
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/charts/chart.py` & `openbb_core-1.2.1/openbb_core/app/model/charts/chart.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+"""OpenBB Core Chart model."""
+
 from enum import Enum
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, ConfigDict, Field
 
 
 class ChartFormat(str, Enum):
+    """Chart format."""
+
     plotly = "plotly"
 
 
 class Chart(BaseModel):
+    """Model for Chart."""
+
     content: Optional[Dict[str, Any]] = Field(
         default=None,
         description="Raw textual representation of the chart.",
     )
     format: Optional[ChartFormat] = Field(
         default=ChartFormat.plotly,
         description="Complementary attribute to the `content` attribute. It specifies the format of the chart.",
@@ -21,10 +27,11 @@
         default=None,
         description="The figure object.",
         json_schema_extra={"exclude_from_api": True},
     )
     model_config = ConfigDict(validate_assignment=True)
 
     def __repr__(self) -> str:
+        """Return string representation."""
         return f"{self.__class__.__name__}\n\n" + "\n".join(
             f"{k}: {v}" for k, v in self.model_dump().items()
         )
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/charts/charting_settings.py` & `openbb_core-1.2.1/openbb_core/app/model/charts/charting_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+"""Charting settings."""
+
 from pathlib import Path
 from typing import Optional
 
 from openbb_core.app.logs.utils.utils import get_app_id
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.app.model.user_settings import UserSettings
 from openbb_core.env import Env
 
 
 # pylint: disable=too-many-instance-attributes
 class ChartingSettings:
+    """Charting settings."""
+
     def __init__(
         self,
         user_settings: Optional[UserSettings] = None,
         system_settings: Optional[SystemSettings] = None,
     ):
+        """Initialize charting settings."""
         user_settings = user_settings or UserSettings()
         system_settings = system_settings or SystemSettings()
 
         user_data_directory = (
             str(Path.home() / "OpenBBUserData")
             if not user_settings.preferences
             else user_settings.preferences.data_directory
@@ -25,15 +30,15 @@
 
         # System
         self.log_collect: bool = system_settings.log_collect
         self.version: str = system_settings.version
         self.python_version: str = system_settings.python_version
         self.test_mode = system_settings.test_mode
         self.app_id: str = get_app_id(user_data_directory)
-        self.debug_mode: bool = Env().DEBUG_MODE
+        self.debug_mode: bool = system_settings.debug_mode or Env().DEBUG_MODE
         self.headless: bool = system_settings.headless
         # User
         self.plot_enable_pywry: bool = user_settings.preferences.plot_enable_pywry
         self.plot_pywry_width: int = user_settings.preferences.plot_pywry_width
         self.plot_pywry_height: int = user_settings.preferences.plot_pywry_height
         self.plot_open_export: bool = user_settings.preferences.plot_open_export
         self.user_email: Optional[str] = getattr(
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/credentials.py` & `openbb_core-1.2.1/openbb_core/app/model/credentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+"""Credentials model and its utilities."""
+
 import traceback
 import warnings
 from typing import Dict, Optional, Set, Tuple
 
-from importlib_metadata import entry_points
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     SecretStr,
     create_model,
 )
 from pydantic.functional_serializers import PlainSerializer
 from typing_extensions import Annotated
 
+from openbb_core.app.extension_loader import ExtensionLoader
 from openbb_core.app.model.abstract.warning import OpenBBWarning
-from openbb_core.app.model.extension import Extension
 from openbb_core.app.provider_interface import ProviderInterface
 from openbb_core.env import Env
 
 
 class LoadingError(Exception):
     """Error loading extension."""
 
@@ -29,91 +30,89 @@
     PlainSerializer(
         lambda x: x.get_secret_value(), return_type=str, when_used="json-unless-none"
     ),
 ]
 
 
 class CredentialsLoader:
-    """Here we create the Credentials model"""
+    """Here we create the Credentials model."""
 
     credentials: Dict[str, Set[str]] = {}
 
     @staticmethod
     def prepare(
         credentials: Dict[str, Set[str]],
     ) -> Dict[str, Tuple[object, None]]:
-        """Prepare credentials map to be used in the Credentials model"""
+        """Prepare credentials map to be used in the Credentials model."""
         formatted: Dict[str, Tuple[object, None]] = {}
         for origin, creds in credentials.items():
             for c in creds:
                 # Not sure we should do this, if you require the same credential it breaks
                 # if c in formatted:
                 #     raise ValueError(f"Credential '{c}' already in use.")
                 formatted[c] = (
                     Optional[OBBSecretStr],
                     Field(
-                        default=None, description=origin
+                        default=None, description=origin, alias=c.upper()
                     ),  # register the credential origin (obbject, providers)
                 )
 
         return formatted
 
     def from_obbject(self) -> None:
-        """Load credentials from OBBject extensions"""
+        """Load credentials from OBBject extensions."""
         self.credentials["obbject"] = set()
-        for entry_point in sorted(entry_points(group="openbb_obbject_extension")):
+        for name, entry in ExtensionLoader().obbject_objects.items():
             try:
-                entry = entry_point.load()
-                if isinstance(entry, Extension):
-                    for c in entry.credentials:
-                        self.credentials["obbject"].add(c)
+                for c in entry.credentials:
+                    self.credentials["obbject"].add(c)
             except Exception as e:
-                msg = f"Error loading extension: {entry_point.name}\n"
+                msg = f"Error loading extension: {name}\n"
                 if Env().DEBUG_MODE:
                     traceback.print_exception(type(e), e, e.__traceback__)
                     raise LoadingError(msg + f"\033[91m{e}\033[0m") from e
                 warnings.warn(
                     message=msg,
                     category=OpenBBWarning,
                 )
 
     def from_providers(self) -> None:
-        """Load credentials from providers"""
+        """Load credentials from providers."""
         self.credentials["providers"] = set()
         for c in ProviderInterface().credentials:
             self.credentials["providers"].add(c)
 
     def load(self) -> BaseModel:
-        """Load credentials from providers"""
+        """Load credentials from providers."""
         # We load providers first to give them priority choosing credential names
         self.from_providers()
         self.from_obbject()
         return create_model(  # type: ignore
             "Credentials",
-            __config__=ConfigDict(validate_assignment=True),
+            __config__=ConfigDict(validate_assignment=True, populate_by_name=True),
             **self.prepare(self.credentials),
         )
 
 
 _Credentials = CredentialsLoader().load()
 
 
 class Credentials(_Credentials):  # type: ignore
-    """Credentials model used to store provider credentials"""
+    """Credentials model used to store provider credentials."""
 
     def __repr__(self) -> str:
-        """String representation of the credentials"""
+        """Define the string representation of the credentials."""
         return (
             self.__class__.__name__
             + "\n\n"
             + "\n".join([f"{k}: {v}" for k, v in sorted(self.__dict__.items())])
         )
 
     def show(self):
-        """Unmask credentials and print them"""
+        """Unmask credentials and print them."""
         print(  # noqa: T201
             self.__class__.__name__
             + "\n\n"
             + "\n".join(
                 [f"{k}: {v}" for k, v in sorted(self.model_dump(mode="json").items())]
             )
         )
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/extension.py` & `openbb_core-1.2.1/openbb_core/app/model/extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,79 @@
+"""Extension class for OBBject extensions."""
+
 import warnings
 from typing import Callable, List, Optional
 
 
 class Extension:
-    """Serves as extension entry point and must be created by each extension package.
+    """
+    Serves as OBBject extension entry point and must be created by each extension package.
 
-    See README.md for more information on how to create an extension.
+    See https://docs.openbb.co/platform/development/developer-guidelines/obbject_extensions.
     """
 
     def __init__(
         self,
         name: str,
         credentials: Optional[List[str]] = None,
+        description: Optional[str] = None,
     ) -> None:
         """Initialize the extension.
 
         Parameters
         ----------
         name : str
             Name of the extension.
         credentials : Optional[List[str]], optional
             List of required credentials, by default None
+        description: Optional[str]
+            Extension description.
         """
         self.name = name
         self.credentials = credentials or []
+        self.description = description
 
     @property
     def obbject_accessor(self) -> Callable:
         """Extend an OBBject, inspired by pandas."""
         # pylint: disable=import-outside-toplevel
         # Avoid circular imports
 
         from openbb_core.app.model.obbject import OBBject
 
         return self.register_accessor(self.name, OBBject)
 
     @staticmethod
     def register_accessor(name, cls) -> Callable:
-        """Register a custom accessor"""
+        """Register a custom accessor."""
 
         def decorator(accessor):
             if hasattr(cls, name):
                 warnings.warn(
                     f"registration of accessor '{repr(accessor)}' under name "
                     f"'{repr(name)}' for type '{repr(cls)}' is overriding a preexisting "
                     f"attribute with the same name.",
                     UserWarning,
                 )
             setattr(cls, name, CachedAccessor(name, accessor))
             # pylint: disable=protected-access
-            cls._accessors.add(name)
+            cls.accessors.add(name)
             return accessor
 
         return decorator
 
 
 class CachedAccessor:
-    """CachedAccessor"""
+    """CachedAccessor."""
 
     def __init__(self, name: str, accessor) -> None:
+        """Initialize the cached accessor."""
         self._name = name
         self._accessor = accessor
 
     def __get__(self, obj, cls):
+        """Get the cached accessor."""
         if obj is None:
             return self._accessor
         accessor_obj = self._accessor(obj)
         object.__setattr__(obj, self._name, accessor_obj)
         return accessor_obj
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/fast_api_settings.py` & `openbb_core-1.2.1/openbb_core/app/model/api_settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """FastAPI configuration settings model."""
-from typing import List
+
+from typing import Dict, List, Optional
 
 from pydantic import BaseModel, ConfigDict, Field, computed_field
 
 
 class Cors(BaseModel):
     """Cors model for FastAPI configuration."""
 
@@ -19,15 +20,15 @@
 
     model_config = ConfigDict(frozen=True)
 
     url: str = "http://localhost:8000"
     description: str = "Local OpenBB development server"
 
 
-class FastAPISettings(BaseModel):
+class APISettings(BaseModel):
     """Settings model for FastAPI configuration."""
 
     model_config = ConfigDict(frozen=True)
 
     version: str = "1"
     title: str = "OpenBB Platform API"
     description: str = "This is the OpenBB Platform API."
@@ -37,14 +38,17 @@
     contact_email: str = "hello@openbb.co"
     license_name: str = "MIT"
     license_url: str = (
         "https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/LICENSE"
     )
     servers: List[Servers] = Field(default_factory=lambda: [Servers()])
     cors: Cors = Field(default_factory=Cors)
+    custom_headers: Optional[Dict[str, str]] = Field(
+        default=None, description="Custom headers and respective default value."
+    )
 
     @computed_field  # type: ignore[misc]
     @property
     def prefix(self) -> str:
         """Return the API prefix."""
         return f"/api/v{self.version}"
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/metadata.py` & `openbb_core-1.2.1/openbb_core/app/model/metadata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,118 +1,141 @@
+"""Metadata model."""
+
 from datetime import datetime
 from inspect import isclass
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel, Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 
 
 class Metadata(BaseModel):
+    """Metadata of a command execution."""
+
     arguments: Dict[str, Any] = Field(
         default_factory=dict,
         description="Arguments of the command.",
     )
     duration: int = Field(
         description="Execution duration in nano second of the command."
     )
     route: str = Field(description="Route of the command.")
     timestamp: datetime = Field(description="Execution starting timestamp.")
 
     def __repr__(self) -> str:
+        """Return string representation."""
         return f"{self.__class__.__name__}\n\n" + "\n".join(
             f"{k}: {v}" for k, v in self.model_dump().items()
         )
 
     @field_validator("arguments")
     @classmethod
     def scale_arguments(cls, v):
         """Scale arguments.
+
         This function is meant to limit the size of the input arguments of a command.
         If the type is one of the following: `Data`, `List[Data]`, `DataFrame`, `List[DataFrame]`,
         `Series`, `List[Series]` or `ndarray`, the value of the argument is swapped by a dictionary
         containing the type and the columns. If the type is not one of the previous, the
         value is kept or trimmed to 80 characters.
         """
-        for arg, arg_val in v.items():
-            new_arg_val = None
-
-            # Data
-            if isclass(type(arg_val)) and issubclass(type(arg_val), Data):
-                new_arg_val = {
-                    "type": f"{type(arg_val).__name__}",
-                    "columns": list(arg_val.dict().keys()),
-                }
-
-            # List[Data]
-            if isinstance(arg_val, list) and issubclass(type(arg_val[0]), Data):
-                columns = [list(d.dict().keys()) for d in arg_val]
-                columns = (item for sublist in columns for item in sublist)  # flatten
-                new_arg_val = {
-                    "type": f"List[{type(arg_val[0]).__name__}]",
-                    "columns": list(set(columns)),
-                }
-
-            # DataFrame
-            elif isinstance(arg_val, pd.DataFrame):
-                columns = (
-                    list(arg_val.index.names) + arg_val.columns.tolist()
-                    if any(index is not None for index in list(arg_val.index.names))
-                    else arg_val.columns.tolist()
-                )
-                new_arg_val = {
-                    "type": f"{type(arg_val).__name__}",
-                    "columns": columns,
-                }
-
-            # List[DataFrame]
-            elif isinstance(arg_val, list) and issubclass(
-                type(arg_val[0]), pd.DataFrame
-            ):
-                columns = [
-                    list(df.index.names) + df.columns.tolist()
-                    if any(index is not None for index in list(df.index.names))
-                    else df.columns.tolist()
-                    for df in arg_val
-                ]
-                new_arg_val = {
-                    "type": f"List[{type(arg_val[0]).__name__}]",
-                    "columns": columns,
-                }
-
-            # Series
-            elif isinstance(arg_val, pd.Series):
-                new_arg_val = {
-                    "type": f"{type(arg_val).__name__}",
-                    "columns": list(arg_val.index.names) + [arg_val.name],
-                }
-
-            # List[Series]
-            elif isinstance(arg_val, list) and isinstance(arg_val[0], pd.Series):
-                columns = [
-                    list(series.index.names) + [series.name]
-                    if any(index is not None for index in list(series.index.names))
-                    else series.name
-                    for series in arg_val
-                ]
-                new_arg_val = {
-                    "type": f"List[{type(arg_val[0]).__name__}]",
-                    "columns": columns,
-                }
-
-            # ndarray
-            elif isinstance(arg_val, np.ndarray):
-                new_arg_val = {
-                    "type": f"{type(arg_val).__name__}",
-                    "columns": list(arg_val.dtype.names or []),
-                }
-
-            else:
-                str_repr_arg_val = str(arg_val)
-                if len(str_repr_arg_val) > 80:
-                    new_arg_val = str_repr_arg_val[:80]
+        arguments: Dict[str, Any] = {}
+        for item in ["provider_choices", "standard_params", "extra_params"]:
+            arguments[item] = {}
+            # The item could be class or it could a dictionary.
+            v_item = (
+                v.__dict__.get(item, {}) if not isinstance(v, dict) else v.get(item, {})
+            )
+            # The item might not be a dictionary yet.
+            v_item = v_item if isinstance(v_item, dict) else v_item.__dict__
+            for arg, arg_val in v_item.items():
+                new_arg_val: Optional[Union[str, dict[str, Sequence[Any]]]] = None
+
+                # Data
+                if isclass(type(arg_val)) and issubclass(type(arg_val), Data):
+                    new_arg_val = {
+                        "type": f"{type(arg_val).__name__}",
+                        "columns": list(arg_val.model_dump().keys()),
+                    }
+
+                # List[Data]
+                if isinstance(arg_val, list) and issubclass(type(arg_val[0]), Data):
+                    _columns = [list(d.model_dump().keys()) for d in arg_val]
+                    ld_columns = (
+                        item for sublist in _columns for item in sublist
+                    )  # flatten
+                    new_arg_val = {
+                        "type": f"List[{type(arg_val[0]).__name__}]",
+                        "columns": list(set(ld_columns)),
+                    }
+
+                # DataFrame
+                elif isinstance(arg_val, pd.DataFrame):
+                    df_columns = (
+                        list(arg_val.index.names) + arg_val.columns.tolist()
+                        if any(index is not None for index in list(arg_val.index.names))
+                        else arg_val.columns.tolist()
+                    )
+                    new_arg_val = {
+                        "type": f"{type(arg_val).__name__}",
+                        "columns": df_columns,
+                    }
+
+                # List[DataFrame]
+                elif isinstance(arg_val, list) and issubclass(
+                    type(arg_val[0]), pd.DataFrame
+                ):
+                    ldf_columns = [
+                        (
+                            list(df.index.names) + df.columns.tolist()
+                            if any(index is not None for index in list(df.index.names))
+                            else df.columns.tolist()
+                        )
+                        for df in arg_val
+                    ]
+                    new_arg_val = {
+                        "type": f"List[{type(arg_val[0]).__name__}]",
+                        "columns": ldf_columns,
+                    }
+
+                # Series
+                elif isinstance(arg_val, pd.Series):
+                    new_arg_val = {
+                        "type": f"{type(arg_val).__name__}",
+                        "columns": list(arg_val.index.names) + [arg_val.name],
+                    }
+
+                # List[Series]
+                elif isinstance(arg_val, list) and isinstance(arg_val[0], pd.Series):
+                    ls_columns = [
+                        (
+                            list(series.index.names) + [series.name]
+                            if any(
+                                index is not None for index in list(series.index.names)
+                            )
+                            else series.name
+                        )
+                        for series in arg_val
+                    ]
+                    new_arg_val = {
+                        "type": f"List[{type(arg_val[0]).__name__}]",
+                        "columns": ls_columns,
+                    }
+
+                # ndarray
+                elif isinstance(arg_val, np.ndarray):
+                    new_arg_val = {
+                        "type": f"{type(arg_val).__name__}",
+                        "columns": list(arg_val.dtype.names or []),
+                    }
+
+                else:
+                    str_repr_arg_val = str(arg_val)
+                    if len(str_repr_arg_val) > 80:
+                        new_arg_val = str_repr_arg_val[:80]
 
-            v[arg] = new_arg_val or arg_val
+                arguments[item][arg] = new_arg_val or arg_val
 
-        return v
+        return arguments
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/obbject.py` & `openbb_core-1.2.1/openbb_core/app/model/obbject.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 """The OBBject."""
-from re import sub
+
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     ClassVar,
     Dict,
     Generic,
+    Hashable,
     List,
     Literal,
     Optional,
     Set,
     TypeVar,
     Union,
 )
 
 import pandas as pd
 from numpy import ndarray
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, PrivateAttr
 
 from openbb_core.app.model.abstract.error import OpenBBError
 from openbb_core.app.model.abstract.tagged import Tagged
 from openbb_core.app.model.abstract.warning import Warning_
 from openbb_core.app.model.charts.chart import Chart
-from openbb_core.app.query import Query
 from openbb_core.app.utils import basemodel_to_df
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.data import Data
 
 if TYPE_CHECKING:
+    from openbb_core.app.query import Query
+
     try:
         from polars import DataFrame as PolarsDataFrame  # type: ignore
     except ImportError:
         PolarsDataFrame = None
 
 T = TypeVar("T")
 
 
 class OBBject(Tagged, Generic[T]):
     """OpenBB object."""
 
+    accessors: ClassVar[Set[str]] = set()
+    _user_settings: ClassVar[Optional[BaseModel]] = None
+    _system_settings: ClassVar[Optional[BaseModel]] = None
+
     results: Optional[T] = Field(
         default=None,
         description="Serializable results.",
     )
     provider: Optional[str] = Field(  # type: ignore
         default=None,
         description="Provider name.",
@@ -54,53 +62,37 @@
         default=None,
         description="Chart object.",
     )
     extra: Dict[str, Any] = Field(
         default_factory=dict,
         description="Extra info.",
     )
-    _credentials: ClassVar[Optional[BaseModel]] = None
-    _accessors: ClassVar[Set[str]] = set()
+    _route: str = PrivateAttr(
+        default=None,
+    )
+    _standard_params: Optional[Dict[str, Any]] = PrivateAttr(
+        default_factory=dict,
+    )
 
     def __repr__(self) -> str:
         """Human readable representation of the object."""
         items = [
             f"{k}: {v}"[:83] + ("..." if len(f"{k}: {v}") > 83 else "")
             for k, v in self.model_dump().items()
         ]
         return f"{self.__class__.__name__}\n\n" + "\n".join(items)
 
-    @classmethod
-    def results_type_repr(cls, params: Optional[Any] = None) -> str:
-        """Return the results type name."""
-        type_ = params[0] if params else cls.model_fields["results"].annotation
-        name = type_.__name__ if hasattr(type_, "__name__") else str(type_)
-        if "typing." in str(type_):
-            unpack_optional = sub(r"Optional\[(.*)\]", r"\1", str(type_))
-            name = sub(
-                r"(\w+\.)*(\w+)?(\, NoneType)?",
-                r"\2",
-                unpack_optional,
-            )
-
-        return name
-
-    @classmethod
-    def model_parametrized_name(cls, params: Any) -> str:
-        """Return the model name with the parameters."""
-        return f"OBBject[{cls.results_type_repr(params)}]"
-
     def to_df(
-        self, index: Optional[str] = None, sort_by: Optional[str] = None
+        self, index: Optional[Union[str, None]] = "date", sort_by: Optional[str] = None
     ) -> pd.DataFrame:
         """Alias for `to_dataframe`."""
         return self.to_dataframe(index=index, sort_by=sort_by)
 
     def to_dataframe(
-        self, index: Optional[str] = None, sort_by: Optional[str] = None
+        self, index: Optional[Union[str, None]] = "date", sort_by: Optional[str] = None
     ) -> pd.DataFrame:
         """Convert results field to pandas dataframe.
 
         Supports converting creating pandas DataFrames from the following
         serializable data formats:
 
         - List[BaseModel]
@@ -109,14 +101,17 @@
         - List[str]
         - List[int]
         - List[float]
         - Dict[str, Dict]
         - Dict[str, List]
         - Dict[str, BaseModel]
 
+        Other supported formats:
+        - str
+
         Parameters
         ----------
         index : Optional[str]
             Column name to use as index.
         sort_by : Optional[str]
             Column name to sort by.
 
@@ -146,33 +141,36 @@
             if isinstance(res, list) and len(res) == 1 and isinstance(res[0], dict):
                 r = res[0]
                 dict_of_df = {}
 
                 for k, v in r.items():
                     # Dict[str, List[BaseModel]]
                     if is_list_of_basemodel(v):
-                        dict_of_df[k] = basemodel_to_df(v, index or "date")
+                        dict_of_df[k] = basemodel_to_df(v, index)
                         sort_columns = False
                     # Dict[str, Any]
                     else:
                         dict_of_df[k] = pd.DataFrame(v)
 
                 df = pd.concat(dict_of_df, axis=1)
 
             # List[BaseModel]
             elif is_list_of_basemodel(res):
                 dt: Union[List[Data], Data] = res  # type: ignore
-                df = basemodel_to_df(dt, index or "date")
+                df = basemodel_to_df(dt, index)
                 sort_columns = False
+            # str
+            elif isinstance(res, str):
+                df = pd.DataFrame([res])
             # List[List | str | int | float] | Dict[str, Dict | List | BaseModel]
             else:
                 try:
-                    df = pd.DataFrame(res)
+                    df = pd.DataFrame(res)  # type: ignore[call-overload]
                     # Set index, if any
-                    if index and index in df.columns:
+                    if df is not None and index is not None and index in df.columns:
                         df.set_index(index, inplace=True)
 
                 except ValueError:
                     if isinstance(res, dict):
                         df = pd.DataFrame([res])
 
             if df is None:
@@ -207,106 +205,93 @@
         try:
             from polars import from_pandas  # type: ignore # pylint: disable=import-outside-toplevel
         except ImportError as exc:
             raise ImportError(
                 "Please install polars: `pip install polars pyarrow`  to use this method."
             ) from exc
 
-        return from_pandas(self.to_dataframe().reset_index())
+        return from_pandas(self.to_dataframe(index=None))
 
     def to_numpy(self) -> ndarray:
         """Convert results field to numpy array."""
-        return self.to_dataframe().reset_index().to_numpy()
+        return self.to_dataframe(index=None).to_numpy()
 
     def to_dict(
         self,
         orient: Literal[
             "dict", "list", "series", "split", "tight", "records", "index"
         ] = "list",
-    ) -> Dict[str, List]:
+    ) -> Union[Dict[Hashable, Any], List[Dict[Hashable, Any]]]:
         """Convert results field to a dictionary using any of pandas to_dict options.
 
         Parameters
         ----------
         orient : Literal["dict", "list", "series", "split", "tight", "records", "index"]
             Value to pass to `.to_dict()` method
 
 
         Returns
         -------
-        Dict[str, List]
-            Dictionary of lists.
+        Union[Dict[Hashable, Any], List[Dict[Hashable, Any]]]
+            Dictionary of lists or list of dictionaries if orient is "records".
         """
-        df = self.to_dataframe()  # type: ignore
-        transpose = False
-        if orient == "list":
-            transpose = True
-            if not isinstance(self.results, dict):
-                transpose = False
-            else:  # Only enter the loop if self.results is a dictionary
-                self.results: Dict[str, Any] = self.results  # type: ignore
-                for _, value in self.results.items():
-                    if not isinstance(value, dict):
-                        transpose = False
-                        break
-        if transpose:
+        df = self.to_dataframe(index=None)
+        if (
+            orient == "list"
+            and isinstance(self.results, dict)
+            and all(
+                isinstance(value, dict)
+                for value in self.results.values()  # pylint: disable=no-member
+            )
+        ):
             df = df.T
         results = df.to_dict(orient=orient)
-        if orient == "list" and "index" in results:
+        if isinstance(results, dict) and orient == "list" and "index" in results:
             del results["index"]
         return results
 
-    def to_chart(self, **kwargs):
-        """
-        Create or update the `Chart`.
-
-        This function assumes that the provided data is a time series, if it's not, it will
-        most likely result in an Exception.
-
-        Note that the `chart` attribute is composed by: `content`, `format` and `fig`.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to be passed to the charting extension.
-            This implies that the user has some knowledge on the charting extension API.
-            This is the case because the charting extension may vary on user preferences.
+    def to_llm(self) -> Union[Dict[Hashable, Any], List[Dict[Hashable, Any]]]:
+        """Convert results field to an LLM compatible output.
 
         Returns
         -------
-        chart.fig
-            The chart figure.
+        Union[Dict[Hashable, Any], List[Dict[Hashable, Any]]]
+            Dictionary of lists or list of dictionaries if orient is "records".
         """
-        #  pylint: disable=import-outside-toplevel
-        # Avoids circular import
-        from openbb_core.app.charting_service import ChartingService
+        df = self.to_dataframe(index=None)
 
-        cs = ChartingService()
-        kwargs["data"] = self.to_dataframe()
+        results = df.to_json(
+            orient="records",
+            date_format="iso",
+            date_unit="s",
+        )
 
-        self.chart = cs.to_chart(**kwargs)
-        return self.chart.fig
+        return results
 
-    def show(self):
+    def show(self, **kwargs: Any) -> None:
         """Display chart."""
+        # pylint: disable=no-member
         if not self.chart or not self.chart.fig:
-            raise OpenBBError(
-                "Chart not found. "
-                "Please compute the chart first by using the `chart=True` argument."
-            )
-        self.chart.fig.show()
+            raise OpenBBError("Chart not found.")
+        show_function: Callable = getattr(self.chart.fig, "show")
+        show_function(**kwargs)
 
     @classmethod
-    async def from_query(cls, query: Query) -> "OBBject":
+    async def from_query(cls, query: "Query") -> "OBBject":
         """Create OBBject from query.
 
         Parameters
         ----------
         query : Query
             Initialized query object.
 
         Returns
         -------
         OBBject[ResultsType]
             OBBject with results.
         """
-        return cls(results=await query.execute())
+        results = await query.execute()
+        if isinstance(results, AnnotatedResult):
+            return cls(
+                results=results.result, extra={"results_metadata": results.metadata}
+            )
+        return cls(results=results)
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/preferences.py` & `openbb_core-1.2.1/openbb_core/app/model/preferences.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+"""Preferences for the OpenBB platform."""
+
 from pathlib import Path
 from typing import Literal
 
 from pydantic import BaseModel, ConfigDict, Field, PositiveInt
 
 
 class Preferences(BaseModel):
-    data_directory: str = str(Path.home() / "OpenBBUserData")
-    export_directory: str = str(Path.home() / "OpenBBUserData" / "exports")
-    user_styles_directory: str = str(Path.home() / "OpenBBUserData" / "styles" / "user")
+    """Preferences for the OpenBB platform."""
+
     cache_directory: str = str(Path.home() / "OpenBBUserData" / "cache")
-    charting_extension: Literal["openbb_charting"] = "openbb_charting"
     chart_style: Literal["dark", "light"] = "dark"
+    data_directory: str = str(Path.home() / "OpenBBUserData")
+    export_directory: str = str(Path.home() / "OpenBBUserData" / "exports")
+    metadata: bool = True
+    output_type: Literal[
+        "OBBject", "dataframe", "polars", "numpy", "dict", "chart", "llm"
+    ] = Field(
+        default="OBBject",
+        description="Python default output type.",
+        validate_default=True,
+    )
     plot_enable_pywry: bool = True
-    plot_pywry_width: PositiveInt = 1400
-    plot_pywry_height: PositiveInt = 762
     plot_open_export: bool = (
         False  # Whether to open plot image exports after they are created
     )
+    plot_pywry_height: PositiveInt = 762
+    plot_pywry_width: PositiveInt = 1400
+    request_timeout: PositiveInt = 60
+    show_warnings: bool = True
     table_style: Literal["dark", "light"] = "dark"
-    request_timeout: PositiveInt = 15
-    metadata: bool = True
-    output_type: Literal[
-        "OBBject", "dataframe", "polars", "numpy", "dict", "chart"
-    ] = Field(default="OBBject", description="Python default output type.")
+    user_styles_directory: str = str(Path.home() / "OpenBBUserData" / "styles" / "user")
 
     model_config = ConfigDict(validate_assignment=True)
 
     def __repr__(self) -> str:
+        """Return a string representation of the model."""
         return f"{self.__class__.__name__}\n\n" + "\n".join(
             f"{k}: {v}" for k, v in self.model_dump().items()
         )
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/system_settings.py` & `openbb_core-1.2.1/openbb_core/app/model/system_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """The OpenBB Platform System Settings."""
+
 import json
 import platform as pl  # I do this so that the import doesn't conflict with the variable name
 from pathlib import Path
 from typing import List, Literal, Optional
 
 from pydantic import ConfigDict, Field, field_validator, model_validator
 
 from openbb_core.app.constants import (
     HOME_DIRECTORY,
     OPENBB_DIRECTORY,
     SYSTEM_SETTINGS_PATH,
     USER_SETTINGS_PATH,
 )
 from openbb_core.app.model.abstract.tagged import Tagged
-from openbb_core.app.model.fast_api_settings import FastAPISettings
-from openbb_core.app.version import VERSION
+from openbb_core.app.model.api_settings import APISettings
+from openbb_core.app.model.python_settings import PythonSettings
+from openbb_core.app.version import CORE_VERSION, VERSION
 
 
 class SystemSettings(Tagged):
     """System settings model."""
 
     # System section
     os: str = str(pl.system())
     python_version: str = str(pl.python_version())
     platform: str = str(pl.platform())
 
     # OpenBB section
     version: str = VERSION
+    core: str = CORE_VERSION
     home_directory: str = str(HOME_DIRECTORY)
     openbb_directory: str = str(OPENBB_DIRECTORY)
     user_settings_path: str = str(USER_SETTINGS_PATH)
     system_settings_path: str = str(SYSTEM_SETTINGS_PATH)
 
     # Logging section
     logging_app_name: Literal["platform"] = "platform"
@@ -40,17 +43,21 @@
     logging_rolling_clock: bool = False
     logging_verbosity: int = 20
     logging_sub_app: Literal["python", "api", "pro"] = "python"
     logging_suppress: bool = False
     log_collect: bool = True
 
     # API section
-    api_settings: FastAPISettings = Field(default_factory=FastAPISettings)
+    api_settings: APISettings = Field(default_factory=APISettings)
+
+    # Python section
+    python_settings: PythonSettings = Field(default_factory=PythonSettings)
 
     # Others
+    debug_mode: bool = False
     test_mode: bool = False
     headless: bool = False
 
     model_config = ConfigDict(validate_assignment=True, frozen=True)
 
     def __repr__(self) -> str:
         """Return a string representation of the model."""
@@ -82,15 +89,15 @@
         return values
 
     @model_validator(mode="after")  # type: ignore
     @classmethod
     def validate_posthog_handler(cls, values: "SystemSettings") -> "SystemSettings":
         """If the user has enabled log collection, then we need to add the Posthog."""
         if (
-            not any([values.test_mode, values.logging_suppress])
+            not any([values.test_mode, values.debug_mode, values.logging_suppress])
             and values.log_collect
             and "posthog" not in values.logging_handlers
         ):
             values.logging_handlers.append("posthog")
 
         return values
```

### Comparing `openbb_core-1.2.0/openbb_core/app/model/user_settings.py` & `openbb_core-1.2.1/openbb_core/app/model/user_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """User settings model."""
+
 from pydantic import Field
 
 from openbb_core.app.model.abstract.tagged import Tagged
 from openbb_core.app.model.credentials import Credentials
 from openbb_core.app.model.defaults import Defaults
 from openbb_core.app.model.preferences import Preferences
 from openbb_core.app.model.profile import Profile
@@ -14,12 +15,10 @@
     profile: Profile = Field(default_factory=Profile)
     credentials: Credentials = Field(default_factory=Credentials)
     preferences: Preferences = Field(default_factory=Preferences)
     defaults: Defaults = Field(default_factory=Defaults)
 
     def __repr__(self) -> str:
         """Human readable representation of the object."""
-        # We use the __dict__ because Credentials.model_dump() will use the serializer
-        # and unmask the credentials
         return f"{self.__class__.__name__}\n\n" + "\n".join(
             f"{k}: {v}" for k, v in self.model_dump().items()
         )
```

### Comparing `openbb_core-1.2.0/openbb_core/app/provider_interface.py` & `openbb_core-1.2.1/openbb_core/app/provider_interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 """Provider Interface."""
+
 from dataclasses import dataclass, make_dataclass
 from difflib import SequenceMatcher
-from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Type, Union
+from typing import (
+    Annotated,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
 
 from fastapi import Query
 from pydantic import (
-    AliasChoices,
     BaseModel,
     ConfigDict,
+    Discriminator,
     Field,
+    SerializeAsAny,
+    Tag,
     create_model,
 )
 from pydantic.fields import FieldInfo
 
 from openbb_core.app.model.abstract.singleton import SingletonMeta
+from openbb_core.app.model.obbject import OBBject
 from openbb_core.provider.query_executor import QueryExecutor
 from openbb_core.provider.registry_map import MapType, RegistryMap
 from openbb_core.provider.utils.helpers import to_snake_case
 
-TupleFieldType = Tuple[str, type, Any]
+TupleFieldType = Tuple[str, Optional[Type], Optional[Any]]
 
 
 @dataclass
 class DataclassField:
     """Dataclass field."""
 
     name: str
-    type_: type
-    default: Any
+    annotation: Optional[Type]
+    default: Optional[Any]
 
 
 @dataclass
 class StandardParams:
     """Standard params dataclass."""
 
 
@@ -88,20 +103,23 @@
         registry_map: Optional[RegistryMap] = None,
         query_executor: Optional[QueryExecutor] = None,
     ) -> None:
         """Initialize provider interface."""
         self._registry_map = registry_map or RegistryMap()
         self._query_executor = query_executor or QueryExecutor
 
-        self._map = self._registry_map.map
+        self._map = self._registry_map.standard_extra
         # TODO: Try these 4 methods in a single iteration
         self._model_providers_map = self._generate_model_providers_dc(self._map)
         self._params = self._generate_params_dc(self._map)
         self._data = self._generate_data_dc(self._map)
         self._return_schema = self._generate_return_schema(self._data)
+        self._return_annotations = self._generate_return_annotations(
+            self._registry_map.original_models
+        )
 
         self._available_providers = self._registry_map.available_providers
         self._provider_choices = self._get_provider_choices(self._available_providers)
 
     @property
     def map(self) -> MapType:
         """Dictionary of provider information."""
@@ -144,126 +162,165 @@
 
     @property
     def models(self) -> List[str]:
         """List of model names."""
         return self._registry_map.models
 
     @property
-    def return_map(self) -> Dict[str, Dict[str, Any]]:
+    def return_annotations(self) -> Dict[str, Type[OBBject]]:
         """Return map."""
-        return self._registry_map.return_map
+        return self._return_annotations
 
     def create_executor(self) -> QueryExecutor:
         """Get query executor."""
-        return self._query_executor(self._registry_map.registry)  # type: ignore
+        return self._query_executor(self._registry_map.registry)  # type: ignore[operator]
 
     @staticmethod
     def _merge_fields(
         current: DataclassField, incoming: DataclassField, query: bool = False
     ) -> DataclassField:
-        current_name = current.name
-        current_type = current.type_
-        current_desc = getattr(current.default, "description", "")
-
-        incoming_type = incoming.type_
-        incoming_desc = getattr(incoming.default, "description", "")
-
-        F: Union[Callable, object] = Query if query else FieldInfo
+        """Merge 2 dataclass fields."""
+        curr_name = current.name
+        curr_type: Optional[Type] = current.annotation
+        curr_desc = getattr(current.default, "description", "")
+        curr_json_schema_extra = getattr(current.default, "json_schema_extra", {})
+
+        inc_type: Optional[Type] = incoming.annotation
+        inc_desc = getattr(incoming.default, "description", "")
+        inc_json_schema_extra = getattr(incoming.default, "json_schema_extra", {})
 
         def split_desc(desc: str) -> str:
             """Split field description."""
             item = desc.split(" (provider: ")
             detail = item[0] if item else ""
             return detail
 
-        curr_detail = split_desc(current_desc)
-        inc_detail = split_desc(incoming_desc)
+        def merge_json_schema_extra(curr: dict, inc: dict) -> dict:
+            """Merge json schema extra."""
+            for key in curr.keys() & inc.keys():
+                # Merge keys that are in both dictionaries if both are lists
+                curr_value = curr[key]
+                inc_value = inc[key]
+                if isinstance(curr_value, list) and isinstance(inc_value, list):
+                    curr[key] = list(set(curr.get(key, []) + inc.get(key, [])))
+                    inc.pop(key)
+
+            # Add any remaining keys from inc to curr
+            curr.update(inc)
+            return curr
+
+        json_schema_extra: dict = merge_json_schema_extra(
+            curr=curr_json_schema_extra or {}, inc=inc_json_schema_extra or {}
+        )
 
-        providers = f"{current.default.title},{incoming.default.title}"
+        curr_detail = split_desc(curr_desc)
+        inc_detail = split_desc(inc_desc)
+
+        curr_title = getattr(current.default, "title", "")
+        inc_title = getattr(incoming.default, "title", "")
+        providers = ",".join([curr_title, inc_title])
         formatted_prov = providers.replace(",", ", ")
 
         if SequenceMatcher(None, curr_detail, inc_detail).ratio() > 0.8:
             new_desc = f"{curr_detail} (provider: {formatted_prov})"
         else:
-            new_desc = f"{current_desc};\n    {incoming_desc}"
+            new_desc = f"{curr_desc};\n    {inc_desc}"
 
-        merged_default = F(  # type: ignore
-            default=current.default.default,
+        QF: Callable = Query if query else FieldInfo  # type: ignore[assignment]
+        merged_default = QF(
+            default=getattr(current.default, "default", None),
             title=providers,
             description=new_desc,
+            json_schema_extra=json_schema_extra,
         )
 
-        merged_type = (
-            Union[current_type, incoming_type]
-            if current_type != incoming_type
-            else current_type
+        merged_type: Optional[Type] = (
+            Union[curr_type, inc_type]  # type: ignore[assignment]
+            if curr_type != inc_type
+            else curr_type
         )
 
-        return DataclassField(
-            name=current_name,
-            type_=merged_type,  # type: ignore
-            default=merged_default,
-        )
+        return DataclassField(curr_name, merged_type, merged_default)
 
     @staticmethod
     def _create_field(
         name: str,
         field: FieldInfo,
         provider_name: Optional[str] = None,
         query: bool = False,
         force_optional: bool = False,
-        alias_dict: Optional[Dict[str, List[str]]] = None,
     ) -> DataclassField:
-        alias_dict = alias_dict or {}
         new_name = name.replace(".", "_")
-        # field.type_ don't work for nested types
-        # field.outer_type_ don't work for Optional nested types
-        type_ = field.annotation
+        annotation = field.annotation
+
+        additional_description = ""
+        if extra := field.json_schema_extra:
+            providers = []
+            for p, v in extra.items():  # type: ignore[union-attr]
+                if isinstance(v, dict) and v.get("multiple_items_allowed"):
+                    providers.append(p)
+                elif isinstance(v, list) and "multiple_items_allowed" in v:
+                    # For backwards compatibility, before this was a list
+                    providers.append(p)
+
+            if providers:
+                if provider_name:
+                    additional_description += " Multiple comma separated items allowed."
+                else:
+                    additional_description += (
+                        " Multiple comma separated items allowed for provider(s): "
+                        + ", ".join(providers)  # type: ignore[arg-type]
+                        + "."
+                    )
 
         provider_field = (
             f"(provider: {provider_name})" if provider_name != "openbb" else ""
         )
         description = (
-            f"{field.description} {provider_field}"
+            f"{field.description}{additional_description} {provider_field}"
             if provider_name and field.description
-            else f"{field.description}"
+            else f"{field.description}{additional_description}"
         )
 
         if field.is_required():
             if force_optional:
-                type_ = Optional[type_]  # type: ignore
+                annotation = Optional[annotation]  # type: ignore
                 default = None
             else:
                 default = ...
         else:
             default = field.default
 
         if query:
-            # We need to use query if we want the field description to show up in the
-            # swagger, it's a fastapi limitation
-            default = Query(
-                default=default,
-                title=provider_name,
-                description=description,
-                alias=field.alias or None,
+            # We need to use query if we want the field description to show
+            # up in the swagger, it's a fastapi limitation
+            return DataclassField(
+                new_name,
+                annotation,
+                Query(
+                    default=default,
+                    title=provider_name,
+                    description=description,
+                    alias=field.alias or None,
+                    json_schema_extra=getattr(field, "json_schema_extra", None),
+                ),
             )
-        elif provider_name:
-            default: FieldInfo = Field(
-                default=default or None,
-                title=provider_name,
-                description=description,
-                validation_alias=AliasChoices(
-                    field.alias,
-                    *list(set(alias_dict.get(name, []))),
-                )
-                if alias_dict.get(name, [])
-                else None,
+        if provider_name:
+            return DataclassField(
+                new_name,
+                annotation,
+                Field(
+                    default=default or None,
+                    title=provider_name,
+                    description=description,
+                    json_schema_extra=field.json_schema_extra,
+                ),
             )
 
-        return DataclassField(new_name, type_, default)
+        return DataclassField(new_name, annotation, default)
 
     @classmethod
     def _extract_params(
         cls,
         providers: Any,
     ) -> Tuple[Dict[str, TupleFieldType], Dict[str, TupleFieldType]]:
         """Extract parameters from map."""
@@ -273,15 +330,15 @@
         for provider_name, model_details in providers.items():
             if provider_name == "openbb":
                 for name, field in model_details["QueryParams"]["fields"].items():
                     incoming = cls._create_field(name, field, query=True)
 
                     standard[incoming.name] = (
                         incoming.name,
-                        incoming.type_,
+                        incoming.annotation,
                         incoming.default,
                     )
             else:
                 for name, field in model_details["QueryParams"]["fields"].items():
                     if name not in providers["openbb"]["QueryParams"]["fields"]:
                         s_name = to_snake_case(name)
                         incoming = cls._create_field(
@@ -296,15 +353,15 @@
                             current = DataclassField(*extra[incoming.name])
                             updated = cls._merge_fields(current, incoming, query=True)
                         else:
                             updated = incoming
 
                         extra[updated.name] = (
                             updated.name,
-                            updated.type_,
+                            updated.annotation,
                             updated.default,
                         )
 
         return standard, extra
 
     @classmethod
     def _extract_data(
@@ -313,56 +370,64 @@
     ) -> Tuple[Dict[str, TupleFieldType], Dict[str, TupleFieldType]]:
         standard: Dict[str, TupleFieldType] = {}
         extra: Dict[str, TupleFieldType] = {}
 
         for provider_name, model_details in providers.items():
             if provider_name == "openbb":
                 for name, field in model_details["Data"]["fields"].items():
+                    if (
+                        name == "provider"
+                        and field.description == "The data provider for the data."
+                    ):  # noqa
+                        continue
                     incoming = cls._create_field(name, field, "openbb")
 
                     standard[incoming.name] = (
                         incoming.name,
-                        incoming.type_,
+                        incoming.annotation,
                         incoming.default,
                     )
             else:
-                alias_dict = model_details.get("Data", {}).get("alias_dict", {})
                 for name, field in model_details["Data"]["fields"].items():
                     if name not in providers["openbb"]["Data"]["fields"]:
+                        if (
+                            name == "provider"
+                            and field.description == "The data provider for the data."
+                        ):  # noqa
+                            continue
                         incoming = cls._create_field(
                             to_snake_case(name),
                             field,
                             provider_name,
                             force_optional=True,
-                            alias_dict=alias_dict,
                         )
 
                         if incoming.name in extra:
                             current = DataclassField(*extra[incoming.name])
                             updated = cls._merge_fields(current, incoming)
                         else:
                             updated = incoming
 
                         extra[updated.name] = (
                             updated.name,
-                            updated.type_,
+                            updated.annotation,
                             updated.default,
                         )
 
         return standard, extra
 
     def _generate_params_dc(
         self, map_: MapType
     ) -> Dict[str, Dict[str, Union[StandardParams, ExtraParams]]]:
         """Generate dataclasses for params.
 
         This creates a dictionary of dataclasses that can be injected as a FastAPI
         dependency.
 
-        Example:
+        Example
         -------
         @dataclass
         class CompanyNews(StandardParams):
             symbols: str = Query(...)
             page: int = Query(default=1)
 
         @dataclass
@@ -376,34 +441,34 @@
 
         for model_name, providers in map_.items():
             standard: dict
             extra: dict
             standard, extra = self._extract_params(providers)
 
             result[model_name] = {
-                "standard": make_dataclass(  # type: ignore
+                "standard": make_dataclass(
                     cls_name=model_name,
-                    fields=list(standard.values()),
+                    fields=list(standard.values()),  # type: ignore[arg-type]
                     bases=(StandardParams,),
                 ),
-                "extra": make_dataclass(  # type: ignore
+                "extra": make_dataclass(
                     cls_name=model_name,
-                    fields=list(extra.values()),
+                    fields=list(extra.values()),  # type: ignore[arg-type]
                     bases=(ExtraParams,),
                 ),
             }
         return result
 
     def _generate_model_providers_dc(self, map_: MapType) -> Dict[str, ProviderChoices]:
         """Generate dataclasses for provider choices by model.
 
         This creates a dictionary that maps model names to dataclasses that can be
         injected as a FastAPI dependency.
 
-        Example:
+        Example
         -------
         @dataclass
         class CompanyNews(ProviderChoices):
             provider: Literal["benzinga", "polygon"]
         """
         result: Dict = {}
 
@@ -429,15 +494,15 @@
     def _generate_data_dc(
         self, map_: MapType
     ) -> Dict[str, Dict[str, Union[StandardData, ExtraData]]]:
         """Generate dataclasses for data.
 
         This creates a dictionary of dataclasses.
 
-        Example:
+        Example
         -------
         class EquityHistoricalData(StandardData):
             date: date
             open: PositiveFloat
             high: PositiveFloat
             low: PositiveFloat
             close: PositiveFloat
@@ -447,22 +512,22 @@
         result: Dict = {}
 
         for model_name, providers in map_.items():
             standard: dict
             extra: dict
             standard, extra = self._extract_data(providers)
             result[model_name] = {
-                "standard": make_dataclass(  # type: ignore
+                "standard": make_dataclass(
                     cls_name=model_name,
-                    fields=list(standard.values()),
+                    fields=list(standard.values()),  # type: ignore[arg-type]
                     bases=(StandardData,),
                 ),
-                "extra": make_dataclass(  # type: ignore
+                "extra": make_dataclass(
                     cls_name=model_name,
-                    fields=list(extra.values()),
+                    fields=list(extra.values()),  # type: ignore[arg-type]
                     bases=(ExtraData,),
                 ),
             }
 
         return result
 
     def _generate_return_schema(
@@ -475,23 +540,24 @@
             standard = dataclasses["standard"]
             extra = dataclasses["extra"]
 
             fields = standard.model_fields.copy()
             fields.update(extra.model_fields)
 
             fields_dict: Dict[str, Tuple[Any, Any]] = {}
+
             for name, field in fields.items():
                 fields_dict[name] = (
                     field.annotation,
                     Field(
                         default=field.default,
                         title=field.title,
                         description=field.description,
                         alias=field.alias,
-                        validation_alias=field.validation_alias,
+                        json_schema_extra=field.json_schema_extra,
                     ),
                 )
 
             model_config = ConfigDict(extra="allow", populate_by_name=True)
 
             result[model_name] = create_model(  # type: ignore
                 model_name,
@@ -503,7 +569,64 @@
 
     def _get_provider_choices(self, available_providers: List[str]) -> type:
         return make_dataclass(
             cls_name="ProviderChoices",
             fields=[("provider", Literal[tuple(available_providers)])],  # type: ignore
             bases=(ProviderChoices,),
         )
+
+    def _generate_return_annotations(
+        self, original_models: Dict[str, Dict[str, Any]]
+    ) -> Dict[str, Type[OBBject]]:
+        """Generate return annotations for FastAPI.
+
+        Example
+        -------
+        class Data(BaseModel):
+            ...
+
+        class EquityData(Data):
+            price: float
+
+        class YFEquityData(EquityData):
+            yf_field: str
+
+        class AVEquityData(EquityData):
+            av_field: str
+
+        class OBBject(BaseModel):
+            results: List[
+                SerializeAsAny[
+                    Annotated[
+                        Union[
+                            Annotated[YFEquityData, Tag("yf")],
+                            Annotated[AVEquityData, Tag("av")],
+                        ],
+                        Discriminator(get_provider),
+                    ]
+                ]
+            ]
+        """
+
+        def get_provider(v: Type[BaseModel]):
+            """Callable to discriminate which BaseModel to use."""
+            return getattr(v, "_provider", None)
+
+        annotations = {}
+        for name, models in original_models.items():
+            outer = set()
+            args = set()
+            for provider, model in models.items():
+                data = model["data"]
+                outer.add(model["results_type"])
+                args.add(Annotated[data, Tag(provider)])
+                # We set the provider to use it in discriminator function
+                setattr(data, "_provider", provider)
+            meta = Discriminator(get_provider) if len(args) > 1 else None
+            inner = SerializeAsAny[Annotated[Union[tuple(args)], meta]]  # type: ignore[misc,valid-type]
+            full = Union[tuple((o[inner] if o else inner) for o in outer)]  # type: ignore[valid-type]
+            annotations[name] = create_model(
+                f"OBBject_{name}",
+                __base__=OBBject[full],  # type: ignore[valid-type]
+                __doc__=f"OBBject with results of type {name}",
+            )
+        return annotations
```

### Comparing `openbb_core-1.2.0/openbb_core/app/query.py` & `openbb_core-1.2.1/openbb_core/app/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
         query = extra_params.__class__.__name__
         fields = asdict(self.provider_interface.params[query]["extra"]())  # type: ignore
 
         for k, v in original.items():
             f = fields[k]
             providers = f.title.split(",") if hasattr(f, "title") else []
+
+            # We only filter/warn if the value is not the default, because fastapi
+            # Depends always sends the default value, even if it's not in the request.
             if v != f.default:
                 if provider_name in providers:
                     filtered[k] = v
                 else:
                     available = ", ".join(providers)
                     warnings.warn(
                         message=f"Parameter '{k}' is not supported by {provider_name}. Available for: {available}.",
```

### Comparing `openbb_core-1.2.0/openbb_core/app/router.py` & `openbb_core-1.2.1/openbb_core/app/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+"""OpenBB Router."""
+
 import traceback
 import warnings
 from functools import lru_cache, partial
 from inspect import Parameter, Signature, isclass, iscoroutinefunction, signature
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Mapping,
     Optional,
     Type,
-    Union,
     get_args,
     get_origin,
     get_type_hints,
     overload,
 )
 
 from fastapi import APIRouter, Depends
-from importlib_metadata import entry_points
 from pydantic import BaseModel
 from pydantic.v1.validators import find_validators
 from typing_extensions import Annotated, ParamSpec, _AnnotatedAlias
 
+from openbb_core.app.deprecation import DeprecationSummary, OpenBBDeprecationWarning
+from openbb_core.app.extension_loader import ExtensionLoader
 from openbb_core.app.model.abstract.warning import OpenBBWarning
 from openbb_core.app.model.command_context import CommandContext
+from openbb_core.app.model.example import filter_list
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.provider_interface import (
     ExtraParams,
     ProviderChoices,
     ProviderInterface,
     StandardParams,
 )
@@ -41,74 +44,81 @@
     """OpenBB Error Response."""
 
     detail: str
     error_kind: str
 
 
 class CommandValidator:
+    """Validate Command."""
+
     @staticmethod
     def is_standard_pydantic_type(value_type: Type) -> bool:
         """Check whether or not a parameter type is a valid Pydantic Standard Type."""
         try:
             func = next(
-                find_validators(value_type, config=dict(arbitrary_types_allowed=True))
+                find_validators(value_type, config=dict(arbitrary_types_allowed=True))  # type: ignore
             )
             valid_type = func.__name__ != "arbitrary_type_validator"
         except Exception:
             valid_type = False
 
         return valid_type
 
     @staticmethod
     def is_valid_pydantic_model_type(model_type: Type) -> bool:
+        """Check whether or not a parameter type is a valid Pydantic Model Type."""
         if not isclass(model_type):
             return False
 
         if issubclass(model_type, BaseModel):
             try:
                 model_type.model_json_schema()
                 return True
             except ValueError:
                 return False
         return False
 
     @classmethod
     def is_serializable_value_type(cls, value_type: Type) -> bool:
+        """Check whether or not a parameter type is a valid serializable type."""
         return cls.is_standard_pydantic_type(
             value_type=value_type
         ) or cls.is_valid_pydantic_model_type(model_type=value_type)
 
     @staticmethod
     def is_annotated_dc(annotation) -> bool:
+        """Check whether or not a parameter type is an annotated dataclass."""
         return isinstance(annotation, _AnnotatedAlias) and hasattr(
             annotation.__args__[0], "__dataclass_fields__"
         )
 
     @staticmethod
     def check_reserved_param(
         name: str,
         expected_annot: Any,
         parameter_map: Mapping[str, Parameter],
         func: Callable,
         sig: Signature,
     ):
+        """Check whether or not a parameter is reserved."""
         if name in parameter_map:
             annotation = getattr(parameter_map[name], "annotation", None)
             if annotation is not None and CommandValidator.is_annotated_dc(annotation):
                 annotation = annotation.__args__[0].__bases__[0]
             if not annotation == expected_annot:
                 raise TypeError(
                     f"The parameter `{name}` must be a {expected_annot}.\n"
                     f"module    = {func.__module__}\n"
                     f"function  = {func.__name__}\n"
                     f"signature = {sig}\n"
                 )
 
     @classmethod
     def check_parameters(cls, func: Callable):
+        """Check whether or not a parameter is a valid."""
         sig = signature(func)
         parameter_map = sig.parameters
 
         check_reserved = partial(
             cls.check_reserved_param, parameter_map=parameter_map, func=func, sig=sig
         )
         check_reserved("cc", CommandContext)
@@ -125,14 +135,15 @@
                     f"function  = {func.__name__}\n"
                     f"signature = {sig}\n"
                     f"parameter = {parameter}\n"
                 )
 
     @classmethod
     def check_return(cls, func: Callable):
+        """Check whether or not a return type is a valid."""
         sig = signature(func)
         return_type = sig.return_annotation
 
         valid_return_type = False
 
         if isclass(return_type) and issubclass(return_type, OBBject):
             results_type = return_type.__pydantic_generic_metadata__.get("args", [])[
@@ -158,76 +169,101 @@
                 "Allowed return type:"
                 f"    {func.__name__}(...) -> OBBject[T] :\n"
                 "If you need T = None, use an empty model instead.\n"
             )
 
     @classmethod
     def check(cls, func: Callable, model: str = ""):
+        """Check whether or not a function is valid."""
         if model and not iscoroutinefunction(func):
             raise TypeError(
                 f"Invalid function: {func.__module__}.{func.__name__}\n"
                 "Model is specified but function is not async.\n"
                 "\n\n"
                 '\033[92m@router.command(model="WorldNews")\n'
                 "async def world(\n"
                 "    cc: CommandContext,\n"
                 "    provider_choices: ProviderChoices,\n"
                 "    standard_params: StandardParams,\n"
                 "    extra_params: ExtraParams,\n"
-                ") -> OBBject[BaseModel]:\n"
+                ") -> OBBject:\n"
                 '    """World News. Global news data."""\n'
                 "    return await OBBject.from_query(Query(**locals()))\033[0m"
             )
 
         cls.check_return(func=func)
         cls.check_parameters(func=func)
 
 
 class Router:
+    """OpenBB Router Class."""
+
     @property
     def api_router(self) -> APIRouter:
+        """API Router."""
         return self._api_router
 
+    @property
+    def prefix(self) -> str:
+        """Prefix."""
+        return self._api_router.prefix
+
+    @property
+    def description(self) -> Optional[str]:
+        """Description."""
+        return self._description
+
+    @property
+    def routers(self) -> Dict[str, "Router"]:
+        """Routers nested within the Router, i.e. sub-routers."""
+        return self._routers
+
     def __init__(
         self,
         prefix: str = "",
+        description: Optional[str] = None,
     ) -> None:
+        """Initialize Router."""
         self._api_router = APIRouter(
             prefix=prefix,
             responses={404: {"description": "Not found"}},
         )
+        self._description = description
+        self._routers: Dict[str, Router] = {}
 
     @overload
     def command(self, func: Optional[Callable[P, OBBject]]) -> Callable[P, OBBject]:
         pass
 
     @overload
     def command(self, **kwargs) -> Callable:
         pass
 
     def command(
         self,
         func: Optional[Callable[P, OBBject]] = None,
         **kwargs,
     ) -> Optional[Callable]:
+        """Command decorator for routes."""
         if func is None:
             return lambda f: self.command(f, **kwargs)
 
         api_router = self._api_router
 
         model = kwargs.pop("model", "")
-        if model:
-            kwargs["response_model_exclude_unset"] = True
-            kwargs["openapi_extra"] = {"model": model}
 
-        func = SignatureInspector.complete_signature(func, model)
-
-        if func:
-            CommandValidator.check(func=func, model=model)
+        if func := SignatureInspector.complete(func, model):
 
+            kwargs["response_model_exclude_unset"] = True
+            kwargs["openapi_extra"] = kwargs.get("openapi_extra", {})
+            kwargs["openapi_extra"]["model"] = model
+            kwargs["openapi_extra"]["examples"] = filter_list(
+                examples=kwargs.pop("examples", []),
+                providers=ProviderInterface().available_providers,
+            )
             kwargs["operation_id"] = kwargs.get(
                 "operation_id", SignatureInspector.get_operation_id(func)
             )
             kwargs["path"] = kwargs.get("path", f"/{func.__name__}")
             kwargs["endpoint"] = func
             kwargs["methods"] = kwargs.get("methods", ["GET"])
             kwargs["response_model"] = kwargs.get(
@@ -249,36 +285,77 @@
                     500: {
                         "model": OpenBBErrorResponse,
                         "description": "Internal Error",
                     },
                 },
             )
 
+            # For custom deprecation
+            if kwargs.get("deprecated", False):
+                deprecation: OpenBBDeprecationWarning = kwargs.pop("deprecation")
+
+                kwargs["summary"] = DeprecationSummary(
+                    deprecation.long_message, deprecation
+                )
+
             api_router.add_api_route(**kwargs)
 
         return func
 
     def include_router(
         self,
         router: "Router",
         prefix: str = "",
     ):
-        tags = [prefix[1:]] if prefix else None
+        """Include router."""
+        tags = [prefix.strip("/")] if prefix else None
         self._api_router.include_router(
             router=router.api_router, prefix=prefix, tags=tags  # type: ignore
         )
+        name = prefix if prefix else router.prefix
+        self._routers[name.strip("/")] = router
+
+    def get_attr(self, path: str, attr: str) -> Any:
+        """Get router attribute from path.
+
+        Parameters
+        ----------
+        path : str
+            Path to the router or nested router.
+            E.g. "/equity" or "/equity/price".
+        attr : str
+            Attribute to get.
+
+        Returns
+        -------
+        Any
+            Attribute value.
+        """
+        return self._search_attr(self, path, attr)
+
+    @staticmethod
+    def _search_attr(router: "Router", path: str, attr: str) -> Any:
+        """Recursively search router attribute from path."""
+        path = path.strip("/")
+        first = path.split("/")[0]
+        if first in router.routers:
+            return Router._search_attr(
+                router.routers[first], "/".join(path.split("/")[1:]), attr
+            )
+        return getattr(router, attr, None)
 
 
 class SignatureInspector:
+    """Inspect function signature."""
+
     @classmethod
-    def complete_signature(
+    def complete(
         cls, func: Callable[P, OBBject], model: str
     ) -> Optional[Callable[P, OBBject]]:
         """Complete function signature."""
-
         if isclass(return_type := func.__annotations__["return"]) and not issubclass(
             return_type, OBBject
         ):
             return func
 
         provider_interface = ProviderInterface()
 
@@ -288,15 +365,14 @@
                     warnings.warn(
                         message=f"\nSkipping api route '/{func.__name__}'.\n"
                         f"Model '{model}' not found.\n\n"
                         "Check available models in ProviderInterface().models",
                         category=OpenBBWarning,
                     )
                 return None
-
             cls.validate_signature(
                 func,
                 {
                     "provider_choices": ProviderChoices,
                     "standard_params": StandardParams,
                     "extra_params": ExtraParams,
                 },
@@ -316,19 +392,19 @@
 
             func = cls.inject_dependency(
                 func=func,
                 arg="extra_params",
                 callable_=provider_interface.params[model]["extra"],
             )
 
-            func = cls.inject_return_type(
+            func = cls.inject_return_annotation(
                 func=func,
-                inner_type=provider_interface.return_schema[model],
-                outer_type=provider_interface.return_map[model],
+                annotation=provider_interface.return_annotations[model],
             )
+
         else:
             func = cls.polish_return_schema(func)
             if (
                 "provider_choices" in func.__annotations__
                 and func.__annotations__["provider_choices"] == ProviderChoices
             ):
                 func = cls.inject_dependency(
@@ -336,46 +412,28 @@
                     arg="provider_choices",
                     callable_=provider_interface.provider_choices,
                 )
 
         return func
 
     @staticmethod
-    def inject_return_type(
-        func: Callable[P, OBBject], inner_type: Any, outer_type: Any
-    ) -> Callable[P, OBBject]:
-        """Inject full return model into the function.
-        Also updates __name__ and __doc__ for API schemas."""
-        ReturnModel = inner_type
-        if get_origin(outer_type) == list:
-            ReturnModel = List[inner_type]  # type: ignore
-        elif get_origin(outer_type) == Union:
-            ReturnModel = Union[List[inner_type], inner_type]  # type: ignore
-
-        return_type = OBBject[ReturnModel]  # type: ignore
-        return_type.__name__ = f"OBBject[{inner_type.__name__}]"
-        return_type.__doc__ = f"OBBject with results of type '{inner_type.__name__}'."
-        return_type.model_rebuild(force=True)
-
-        func.__annotations__["return"] = return_type
-        return func
-
-    @staticmethod
     def polish_return_schema(func: Callable[P, OBBject]) -> Callable[P, OBBject]:
-        """Polish API schemas by filling __doc__ and __name__"""
+        """Polish API schemas by filling `__doc__` and `__name__`."""
         return_type = func.__annotations__["return"]
         is_list = False
 
         results_type = get_type_hints(return_type)["results"]
+        results_type_args = get_args(results_type)
         if not isinstance(results_type, type(None)):
-            results_type = get_args(results_type)[0]
+            results_type = results_type_args[0]
 
         is_list = get_origin(results_type) == list
-        args = get_args(results_type)
-        inner_type = args[0] if is_list and args else results_type
+        inner_type = (
+            results_type_args[0] if is_list and results_type_args else results_type
+        )
         inner_type_name = getattr(inner_type, "__name__", inner_type)
 
         func.__annotations__["return"].__doc__ = "OBBject"
         func.__annotations__["return"].__name__ = f"OBBject[{inner_type_name}]"
 
         return func
 
@@ -400,82 +458,105 @@
         func: Callable[P, OBBject], arg: str, callable_: Any
     ) -> Callable[P, OBBject]:
         """Annotate function with dependency injection."""
         func.__annotations__[arg] = Annotated[callable_, Depends()]  # type: ignore
         return func
 
     @staticmethod
+    def inject_return_annotation(
+        func: Callable[P, OBBject], annotation: Type[OBBject]
+    ) -> Callable[P, OBBject]:
+        """Annotate function with return annotation."""
+        func.__annotations__["return"] = annotation
+        return func
+
+    @staticmethod
     def get_description(func: Callable) -> str:
         """Get description from docstring."""
         doc = func.__doc__
         if doc:
             description = doc.split("    Parameters\n    ----------")[0]
             description = description.split("    Returns\n    -------")[0]
+            description = description.split("    Examples\n    -------")[0]
             description = "\n".join([line.strip() for line in description.split("\n")])
 
             return description
         return ""
 
     @staticmethod
-    def get_operation_id(func: Callable) -> str:
-        """Get operation id"""
+    def get_operation_id(func: Callable, sep: str = "_") -> str:
+        """Get operation id."""
         operation_id = [
             t.replace("_router", "").replace("openbb_", "")
             for t in func.__module__.split(".") + [func.__name__]
         ]
-        cleaned_id = "_".join({c: "" for c in operation_id if c}.keys())
+        cleaned_id = sep.join({c: "" for c in operation_id if c}.keys())
         return cleaned_id
 
 
 class CommandMap:
     """Matching Routes with Commands."""
 
     def __init__(
         self, router: Optional[Router] = None, coverage_sep: Optional[str] = None
     ) -> None:
+        """Initialize CommandMap."""
         self._router = router or RouterLoader.from_extensions()
         self._map = self.get_command_map(router=self._router)
-        self._provider_coverage = self.get_provider_coverage(
-            router=self._router, sep=coverage_sep
-        )
-        self._command_coverage = self.get_command_coverage(
-            router=self._router, sep=coverage_sep
-        )
-        self._commands_model = self.get_commands_model(
-            router=self._router, sep=coverage_sep
-        )
+        self._provider_coverage: Dict[str, List[str]] = {}
+        self._command_coverage: Dict[str, List[str]] = {}
+        self._commands_model: Dict[str, str] = {}
+        self._coverage_sep = coverage_sep
 
     @property
     def map(self) -> Dict[str, Callable]:
+        """Get command map."""
         return self._map
 
     @property
     def provider_coverage(self) -> Dict[str, List[str]]:
+        """Get provider coverage."""
+        if not self._provider_coverage:
+            self._provider_coverage = self.get_provider_coverage(
+                router=self._router, sep=self._coverage_sep
+            )
         return self._provider_coverage
 
     @property
     def command_coverage(self) -> Dict[str, List[str]]:
+        """Get command coverage."""
+        if not self._command_coverage:
+            self._command_coverage = self.get_command_coverage(
+                router=self._router, sep=self._coverage_sep
+            )
         return self._command_coverage
 
     @property
     def commands_model(self) -> Dict[str, str]:
+        """Get commands model."""
+        if not self._commands_model:
+            self._commands_model = self.get_commands_model(
+                router=self._router, sep=self._coverage_sep
+            )
         return self._commands_model
 
     @staticmethod
     def get_command_map(
         router: Router,
     ) -> Dict[str, Callable]:
+        """Get command map."""
         api_router = router.api_router
         command_map = {route.path: route.endpoint for route in api_router.routes}  # type: ignore
         return command_map
 
     @staticmethod
     def get_provider_coverage(
         router: Router, sep: Optional[str] = None
     ) -> Dict[str, List[str]]:
+        """Get provider coverage."""
         api_router = router.api_router
 
         mapping = ProviderInterface().map
 
         coverage_map: Dict[Any, Any] = {}
         for route in api_router.routes:
             openapi_extra = getattr(route, "openapi_extra")
@@ -498,14 +579,15 @@
 
         return coverage_map
 
     @staticmethod
     def get_command_coverage(
         router: Router, sep: Optional[str] = None
     ) -> Dict[str, List[str]]:
+        """Get command coverage."""
         api_router = router.api_router
 
         mapping = ProviderInterface().map
 
         coverage_map: Dict[Any, Any] = {}
         for route in api_router.routes:
             openapi_extra = getattr(route, "openapi_extra")
@@ -523,14 +605,15 @@
                         if route.path not in coverage_map:  # type: ignore
                             coverage_map[rp] = []
                         coverage_map[rp] = providers
         return coverage_map
 
     @staticmethod
     def get_commands_model(router: Router, sep: Optional[str] = None) -> Dict[str, str]:
+        """Get commands model."""
         api_router = router.api_router
 
         coverage_map: Dict[Any, Any] = {}
         for route in api_router.routes:
             openapi_extra = getattr(route, "openapi_extra")
             if openapi_extra:
                 model = openapi_extra.get("model", None)
@@ -540,34 +623,36 @@
                     )
                     if route.path not in coverage_map:  # type: ignore
                         coverage_map[rp] = []
                     coverage_map[rp] = model
         return coverage_map
 
     def get_command(self, route: str) -> Optional[Callable]:
+        """Get command from route."""
         return self._map.get(route, None)
 
 
 class LoadingError(Exception):
     """Error loading extension."""
 
 
 class RouterLoader:
+    """Router Loader."""
+
     @staticmethod
     @lru_cache
     def from_extensions() -> Router:
+        """Load routes from extensions."""
         router = Router()
 
-        for entry_point in sorted(entry_points(group="openbb_core_extension")):
+        for name, entry in ExtensionLoader().core_objects.items():
             try:
-                entry = entry_point.load()
-                if isinstance(entry, Router):
-                    router.include_router(router=entry, prefix=f"/{entry_point.name}")
+                router.include_router(router=entry, prefix=f"/{name}")
             except Exception as e:
-                msg = f"Error loading extension: {entry_point.name}\n"
+                msg = f"Error loading extension: {name}\n"
                 if Env().DEBUG_MODE:
                     traceback.print_exception(type(e), e, e.__traceback__)
                     raise LoadingError(msg + f"\033[91m{e}\033[0m") from e
                 warnings.warn(
                     message=msg,
                     category=OpenBBWarning,
                 )
```

### Comparing `openbb_core-1.2.0/openbb_core/app/service/auth_service.py` & `openbb_core-1.2.1/openbb_core/app/service/auth_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,72 @@
+"""Auth service."""
+
 import logging
 from importlib import import_module
 from types import ModuleType
 from typing import Awaitable, Callable, Optional
 
 from fastapi import APIRouter
-from importlib_metadata import entry_points
 from openbb_core.api.router.user import (
     auth_hook as default_auth_hook,
     router as default_router,
     user_settings_hook as default_user_settings_hook,
 )
+from openbb_core.app.extension_loader import ExtensionLoader
 from openbb_core.app.model.abstract.singleton import SingletonMeta
 from openbb_core.app.model.user_settings import UserSettings
 from openbb_core.env import Env
 
-EXT_GROUP = "openbb_core_extension"
 EXT_NAME = Env().API_AUTH_EXTENSION
 
 logger = logging.getLogger("uvicorn.error")
 
 
+class AuthServiceError(Exception):
+    """Authentication service error."""
+
+
 class AuthService(metaclass=SingletonMeta):
+    """Auth service."""
+
     def __init__(self, ext_name: Optional[str] = EXT_NAME) -> None:
-        """Initializes AuthService."""
+        """Initialize AuthService."""
         if not self._load_extension(ext_name):
             self._router = default_router
             self._auth_hook = default_auth_hook
             self._user_settings_hook = default_user_settings_hook
 
     @property
     def router(self) -> APIRouter:
-        """Gets router."""
+        """Get router."""
         return self._router
 
     @property
     def auth_hook(self) -> Callable[..., Awaitable[None]]:
-        """Gets general authentication hook."""
+        """Get general authentication hook."""
         return self._auth_hook
 
     @property
     def user_settings_hook(self) -> Callable[..., Awaitable[UserSettings]]:
-        """Gets user settings hook."""
+        """Get user settings hook."""
         return self._user_settings_hook
 
     @staticmethod
-    def _is_installed(ext_name: str, group: str = EXT_GROUP) -> bool:
-        """Checks if auth_extension is installed."""
-        return ext_name in [ext.name for ext in entry_points(group=group)]
+    def _is_installed(ext_name: str) -> bool:
+        """Check if auth_extension is installed."""
+        extension = ExtensionLoader().get_core_entry_point(ext_name) or False
+        return extension and ext_name == extension.name  # type: ignore
 
     @staticmethod
-    def _get_entry_mod(ext_name: str, group: str = EXT_GROUP) -> ModuleType:
+    def _get_entry_mod(ext_name: str) -> ModuleType:
         """Get the module of the given auth_extension."""
-        return import_module(entry_points(group=group)[ext_name].module)
+        extension = ExtensionLoader().get_core_entry_point(ext_name)
+        if not extension:
+            raise AuthServiceError(f"Extension '{ext_name}' is not installed.")
+        return import_module(extension.module)
 
     def _load_extension(self, ext_name: Optional[str]) -> bool:
         """Load auth extension."""
         if ext_name and self._is_installed(ext_name):
             entry_mod = self._get_entry_mod(ext_name)
             self._router = entry_mod.router
             self._auth_hook = entry_mod.auth_hook
```

### Comparing `openbb_core-1.2.0/openbb_core/app/service/hub_service.py` & `openbb_core-1.2.1/openbb_core/app/service/hub_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 """Hub manager class."""
+
 from typing import Optional
+from warnings import warn
 
 from fastapi import HTTPException
-from jose import JWTError
-from jose.exceptions import ExpiredSignatureError
-from jose.jwt import decode, get_unverified_header
+from jwt import ExpiredSignatureError, PyJWTError, decode, get_unverified_header
 from openbb_core.app.model.abstract.error import OpenBBError
 from openbb_core.app.model.credentials import Credentials
-from openbb_core.app.model.hub.features_keys import FeaturesKeys
 from openbb_core.app.model.hub.hub_session import HubSession
 from openbb_core.app.model.hub.hub_user_settings import HubUserSettings
 from openbb_core.app.model.profile import Profile
 from openbb_core.app.model.user_settings import UserSettings
 from openbb_core.env import Env
-from pydantic import SecretStr
 from requests import get, post, put
 
 
 class HubService:
     """Hub service class."""
 
     TIMEOUT = 10
+    # Mapping of V3 keys to V4 keys for backward compatibility
+    V3TOV4 = {
+        "API_KEY_ALPHAVANTAGE": "alpha_vantage_api_key",
+        "API_BIZTOC_TOKEN": "biztoc_api_key",
+        "API_FRED_KEY": "fred_api_key",
+        "API_KEY_FINANCIALMODELINGPREP": "fmp_api_key",
+        "API_INTRINIO_KEY": "intrinio_api_key",
+        "API_POLYGON_KEY": "polygon_api_key",
+        "API_KEY_QUANDL": "nasdaq_api_key",
+        "API_TRADIER_TOKEN": "tradier_api_key",
+    }
+    V4TOV3 = {v: k for k, v in V3TOV4.items()}
 
     def __init__(
         self,
         session: Optional[HubSession] = None,
         base_url: Optional[str] = None,
     ):
+        """Initialize Hub service."""
         self._base_url = base_url or Env().HUB_BACKEND
         self._session = session
+        self._hub_user_settings: Optional[HubUserSettings] = None
 
     @property
     def base_url(self) -> str:
         """Get base url."""
         return self._base_url
 
     @property
@@ -75,21 +87,18 @@
         raise OpenBBError(
             "No session found. Login or provide a 'HubSession' on initialization."
         )
 
     def pull(self) -> UserSettings:
         """Pull user settings from Hub."""
         if self._session:
-            hub_user_settings = self._get_user_settings(self._session)
-            if hub_user_settings:
-                profile = Profile(
-                    hub_session=self._session,
-                )
-                credentials = self.hub2platform(hub_user_settings)
-                return UserSettings(profile=profile, credentials=credentials)
+            self._hub_user_settings = self._get_user_settings(self._session)
+            profile = Profile(hub_session=self._session)
+            credentials = self.hub2platform(self._hub_user_settings)
+            return UserSettings(profile=profile, credentials=credentials)
         raise OpenBBError(
             "No session found. Login or provide a 'HubSession' on initialization."
         )
 
     def _get_session_from_email_password(self, email: str, password: str) -> HubSession:
         """Get session from email and password."""
         if not email:
@@ -124,15 +133,15 @@
         raise HTTPException(status_code, detail)
 
     def _get_session_from_platform_token(self, token: str) -> HubSession:
         """Get session from Platform personal access token."""
         if not token:
             raise OpenBBError("Platform personal access token not found.")
 
-        self.check_token_expiration(token)
+        self._check_token_expiration(token)
 
         response = post(
             url=self._base_url + "/sdk/login",
             json={
                 "token": token,
             },
             timeout=self.TIMEOUT,
@@ -210,61 +219,55 @@
 
         if response.status_code == 200:
             return True
         status_code = response.status_code
         detail = response.json().get("detail", None)
         raise HTTPException(status_code, detail)
 
-    @classmethod
-    def hub2platform(cls, settings: HubUserSettings) -> Credentials:
+    def hub2platform(self, settings: HubUserSettings) -> Credentials:
         """Convert Hub user settings to Platform models."""
-        # TODO: Hub is getting credentials from `all_api_keys.json`, which uses
-        # the terminal names conventions. We need to update it to use a file that
-        # lives here in the platform and maps the credential names between the two.
-        credentials = Credentials(
-            alpha_vantage_api_key=settings.features_keys.API_KEY_ALPHAVANTAGE,
-            biztoc_api_key=settings.features_keys.API_BIZTOC_TOKEN,
-            fred_api_key=settings.features_keys.API_FRED_KEY,
-            fmp_api_key=settings.features_keys.API_KEY_FINANCIALMODELINGPREP,
-            intrinio_api_key=settings.features_keys.API_INTRINIO_KEY,
-            polygon_api_key=settings.features_keys.API_POLYGON_KEY,
-            nasdaq_api_key=settings.features_keys.API_KEY_QUANDL,
-            ultima_api_key=settings.features_keys.API_ULTIMA_KEY,
-        )
-        return credentials
+        if any(k in settings.features_keys for k in self.V3TOV4):
+            deprecated = {
+                k: v for k, v in self.V3TOV4.items() if k in settings.features_keys
+            }
+            msg = ""
+            for k, v in deprecated.items():
+                msg += f"\n'{k}' -> '{v.upper()}', "
+            msg = msg.strip(", ")
+            warn(
+                message=f"\nDeprecated v3 credentials found.\n{msg}"
+                "\n\nYou can update them at https://my.openbb.co/app/platform/credentials.",
+            )
+        # We give priority to v4 keys over v3 keys if both are present
+        hub_credentials = {
+            self.V3TOV4.get(k, k): settings.features_keys.get(self.V3TOV4.get(k, k), v)
+            for k, v in settings.features_keys.items()
+        }
+        return Credentials(**hub_credentials)
 
-    @classmethod
-    def platform2hub(cls, credentials: Credentials) -> HubUserSettings:
+    def platform2hub(self, credentials: Credentials) -> HubUserSettings:
         """Convert Platform models to Hub user settings."""
-
-        def get_cred(cred: str) -> Optional[str]:
-            secret_str: Optional[SecretStr] = getattr(credentials, cred, None)
-            return secret_str.get_secret_value() if secret_str else None
-
-        features_keys = FeaturesKeys(
-            API_BIZTOC_TOKEN=get_cred("biztoc_api_key"),
-            API_FRED_KEY=get_cred("fred_api_key"),
-            API_INTRINIO_KEY=get_cred("intrinio_api_key"),
-            API_KEY_ALPHAVANTAGE=get_cred("alpha_vantage_api_key"),
-            API_KEY_FINANCIALMODELINGPREP=get_cred("fmp_api_key"),
-            API_POLYGON_KEY=get_cred("polygon_api_key"),
-            API_KEY_QUANDL=get_cred("nasdaq_api_key"),
-            API_ULTIMA_KEY=get_cred("ultima_api_key"),
-        )
-        hub_user_settings = HubUserSettings(features_keys=features_keys)
-        return hub_user_settings
+        # Dump mode json ensures SecretStr values are serialized as strings
+        credentials = credentials.model_dump(mode="json", exclude_none=True)
+        settings = self._hub_user_settings or HubUserSettings()
+        for v4_k, v in sorted(credentials.items()):
+            v3_k = self.V4TOV3.get(v4_k, None)
+            # If v3 key was in the hub already, we keep it
+            k = v3_k if v3_k in settings.features_keys else v4_k
+            settings.features_keys[k] = v
+        return settings
 
     @staticmethod
-    def check_token_expiration(token: str) -> None:
+    def _check_token_expiration(token: str) -> None:
         """Check token expiration, raises exception if expired."""
         try:
             header_data = get_unverified_header(token)
             decode(
                 token,
                 key="secret",
                 algorithms=[header_data["alg"]],
                 options={"verify_signature": False, "verify_exp": True},
             )
         except ExpiredSignatureError as e:
             raise OpenBBError("Platform personal access token expired.") from e
-        except JWTError as e:
+        except PyJWTError as e:
             raise OpenBBError("Failed to decode Platform token.") from e
```

### Comparing `openbb_core-1.2.0/openbb_core/app/service/system_service.py` & `openbb_core-1.2.1/openbb_core/app/service/system_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""System service."""
+
 import hashlib
 import json
 from pathlib import Path
 from typing import Optional
 
 from openbb_core.app.constants import SYSTEM_SETTINGS_PATH
 from openbb_core.app.model.abstract.singleton import SingletonMeta
@@ -14,24 +16,25 @@
     SYSTEM_SETTINGS_PATH = SYSTEM_SETTINGS_PATH
     SYSTEM_SETTINGS_ALLOWED_FIELD_SET = {
         "log_collect",
         "test_mode",
         "headless",
         "logging_sub_app",
         "api_settings",
+        "python_settings",
+        "debug_mode",
     }
 
-    PRO_VALIDATION_HASH = (
-        "300ac59fdcc8f899e0bc5c18cda8652220735da1a00e2af365efe9d8e5fe8306"
-    )
+    PRO_VALIDATION_HASH = "300ac59fdcc8f899e0bc5c18cda8652220735da1a00e2af365efe9d8e5fe8306"  # pragma: allowlist secret
 
     def __init__(
         self,
         **kwargs,
     ):
+        """Initialize system service."""
         self._system_settings = self._read_default_system_settings(
             path=self.SYSTEM_SETTINGS_PATH, **kwargs
         )
 
     @classmethod
     def _compare_hash(cls, input_value, existing_hash: Optional[str] = None):
         existing_hash = existing_hash or cls.PRO_VALIDATION_HASH
```

### Comparing `openbb_core-1.2.0/openbb_core/app/service/user_service.py` & `openbb_core-1.2.1/openbb_core/app/service/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """User service."""
+
 import json
 from functools import reduce
 from pathlib import Path
 from typing import Any, Dict, List, MutableMapping, Optional
 
 from openbb_core.app.constants import USER_SETTINGS_PATH
 from openbb_core.app.model.abstract.singleton import SingletonMeta
@@ -15,14 +16,15 @@
     USER_SETTINGS_PATH = USER_SETTINGS_PATH
     USER_SETTINGS_ALLOWED_FIELD_SET = {"credentials", "preferences", "defaults"}
 
     def __init__(
         self,
         default_user_settings: Optional[UserSettings] = None,
     ):
+        """Initialize user service."""
         self._default_user_settings = (
             default_user_settings or self.read_default_user_settings()
         )
 
     @classmethod
     def read_default_user_settings(cls, path: Optional[Path] = None) -> UserSettings:
         """Read default user settings."""
```

### Comparing `openbb_core-1.2.0/openbb_core/app/static/account.py` & `openbb_core-1.2.1/openbb_core/app/static/account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Account."""
+
 # pylint: disable=W0212:protected-access
 import json
 from functools import wraps
 from pathlib import Path
 from sys import exc_info
 from typing import TYPE_CHECKING, Optional
 
@@ -29,39 +30,42 @@
 
     def __init__(self, base_app: "BaseApp"):
         """Initialize account service."""
         self._base_app = base_app
         self._openbb_directory = (
             base_app._command_runner.system_settings.openbb_directory
         )
+        self._hub_service: Optional[HubService] = None
 
     def __repr__(self) -> str:
         """Human readable representation of the object."""
         return self.__doc__ or ""
 
     def _log_account_command(func):  # pylint: disable=E0213
         """Log account command."""
 
-        @wraps(func)
+        @wraps(func)  # type: ignore[arg-type]
         def wrapped(self, *args, **kwargs):
             try:
-                result = func(self, *args, **kwargs)  # pylint: disable=E1102
+                # pylint: disable=E1102
+                result = func(self, *args, **kwargs)  # type: ignore[operator]
             except Exception as e:
                 raise OpenBBError(e) from e
             finally:
                 user_settings = self._base_app._command_runner.user_settings
                 system_settings = self._base_app._command_runner.system_settings
                 ls = LoggingService(
                     user_settings=user_settings, system_settings=system_settings
                 )
                 ls.log(
                     user_settings=user_settings,
                     system_settings=system_settings,
-                    route=f"/account/{func.__name__}",  # pylint: disable=E1101
-                    func=func,
+                    # pylint: disable=E1101
+                    route=f"/account/{func.__name__}",  # type: ignore[attr-defined]
+                    func=func,  # type: ignore[arg-type]
                     kwargs={},  # don't want any credentials being logged by accident
                     exec_info=exc_info(),
                 )
 
             return result
 
         return wrapped
@@ -113,26 +117,28 @@
             Return user settings, by default False
 
         Returns
         -------
         Optional[UserSettings]
             User settings: profile, credentials, preferences
         """
-        hs = self._create_hub_service(email, password, pat)
-        incoming = hs.pull()
+        self._hub_service = self._create_hub_service(email, password, pat)
+        incoming = self._hub_service.pull()
         updated: UserSettings = UserService.update_default(incoming)
         self._base_app._command_runner.user_settings = updated
         if remember_me:
             Path(self._openbb_directory).mkdir(parents=False, exist_ok=True)
             session_file = Path(self._openbb_directory, self.SESSION_FILE)
             with open(session_file, "w") as f:
-                if not hs.session:
+                if not self._hub_service.session:
                     raise OpenBBError("Not connected to hub.")
 
-                json.dump(hs.session.model_dump(mode="json"), f, indent=4)
+                json.dump(
+                    self._hub_service.session.model_dump(mode="json"), f, indent=4
+                )
 
         if return_settings:
             return self._base_app._command_runner.user_settings
         return None
 
     @_log_account_command  # type: ignore
     def save(self, return_settings: bool = False) -> Optional[UserSettings]:
@@ -144,22 +150,20 @@
             Return user settings, by default False
 
         Returns
         -------
         Optional[UserSettings]
             User settings: profile, credentials, preferences
         """
-        hub_session = self._base_app._command_runner.user_settings.profile.hub_session
-        if not hub_session:
+        if not self._hub_service:
             UserService.write_default_user_settings(
                 self._base_app._command_runner.user_settings
             )
         else:
-            hs = HubService(hub_session)
-            hs.push(self._base_app._command_runner.user_settings)
+            self._hub_service.push(self._base_app._command_runner.user_settings)
 
         if return_settings:
             return self._base_app._command_runner.user_settings
         return None
 
     @_log_account_command  # type: ignore
     def refresh(self, return_settings: bool = False) -> Optional[UserSettings]:
@@ -171,22 +175,20 @@
             Return user settings, by default False
 
         Returns
         -------
         Optional[UserSettings]
             User settings: profile, credentials, preferences
         """
-        hub_session = self._base_app._command_runner.user_settings.profile.hub_session
-        if not hub_session:
+        if not self._hub_service:
             self._base_app._command_runner.user_settings = (
                 UserService.read_default_user_settings()
             )
         else:
-            hs = HubService(hub_session)
-            incoming = hs.pull()
+            incoming = self._hub_service.pull()
             updated: UserSettings = UserService.update_default(incoming)
             updated.id = self._base_app._command_runner.user_settings.id
             self._base_app._command_runner.user_settings = updated
 
         if return_settings:
             return self._base_app._command_runner.user_settings
         return None
@@ -201,20 +203,18 @@
             Return user settings, by default False
 
         Returns
         -------
         Optional[UserSettings]
             User settings: profile, credentials, preferences
         """
-        hub_session = self._base_app._command_runner.user_settings.profile.hub_session
-        if not hub_session:
+        if not self._hub_service:
             raise OpenBBError("Not connected to hub.")
 
-        hs = HubService(hub_session)
-        hs.disconnect()
+        self._hub_service.disconnect()
 
         session_file = Path(self._openbb_directory, self.SESSION_FILE)
         if session_file.exists():
             session_file.unlink()
 
         self._base_app._command_runner.user_settings = (
             UserService.read_default_user_settings()
```

### Comparing `openbb_core-1.2.0/openbb_core/app/static/app_factory.py` & `openbb_core-1.2.1/openbb_core/app/static/app_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """App factory."""
-from typing import Optional, Type, TypeVar
+
+from typing import Dict, Optional, Type, TypeVar
 
 from openbb_core.app.command_runner import CommandRunner
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.app.model.user_settings import UserSettings
 from openbb_core.app.static.account import Account
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.coverage import Coverage
+from openbb_core.app.static.reference_loader import ReferenceLoader
 from openbb_core.app.version import VERSION
 
 E = TypeVar("E", bound=Type[Container])
 BASE_DOC = f"""OpenBB Platform v{VERSION}
 
 Utilities:
     /account
@@ -20,17 +22,20 @@
 """
 
 
 class BaseApp:
     """Base app."""
 
     def __init__(self, command_runner: CommandRunner):
+        """Initialize the app."""
+        command_runner.init_logging_service()
         self._command_runner = command_runner
         self._account = Account(self)
         self._coverage = Coverage(self)
+        self._reference = ReferenceLoader().reference
 
     @property
     def account(self) -> Account:
         """Account menu."""
         return self._account
 
     @property
@@ -44,21 +49,23 @@
         return self._command_runner.system_settings
 
     @property
     def coverage(self) -> Coverage:
         """Coverage menu."""
         return self._coverage
 
+    @property
+    def reference(self) -> Dict[str, Dict]:
+        """Return reference data."""
+        return self._reference
+
 
 def create_app(extensions: Optional[E] = None) -> Type[BaseApp]:
     """Create the app."""
 
-    class EmptyClass:
-        pass
-
-    class App(BaseApp, extensions or EmptyClass):  # type: ignore
+    class App(BaseApp, extensions or object):  # type: ignore[misc]
         def __repr__(self) -> str:
             # pylint: disable=E1101
             ext_doc = extensions.__doc__ if extensions else ""
             return BASE_DOC + (ext_doc or "")
 
     return App(command_runner=CommandRunner())
```

### Comparing `openbb_core-1.2.0/openbb_core/app/static/coverage.py` & `openbb_core-1.2.1/openbb_core/app/static/coverage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """Coverage module."""
+
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from openbb_core.api.router.helpers.coverage_helpers import get_route_schema_map
 from openbb_core.app.provider_interface import ProviderInterface
 from openbb_core.app.router import CommandMap
+from openbb_core.app.static.reference_loader import ReferenceLoader
 
 if TYPE_CHECKING:
     from openbb_core.app.static.app_factory import BaseApp
 
 
 class Coverage:
     """Coverage class.
 
     /coverage
 
         providers
         commands
         command_model
         command_schemas
+        reference
     """
 
     def __init__(self, app: "BaseApp"):
         """Initialize coverage."""
         self._app = app
         self._command_map = CommandMap(coverage_sep=".")
         self._provider_interface = ProviderInterface()
+        self._reference_loader = ReferenceLoader()
 
     def __repr__(self) -> str:
         """Return docstring."""
         return self.__doc__ or ""
 
     @property
     def providers(self) -> Dict[str, List[str]]:
@@ -40,18 +44,21 @@
         """Return commands coverage."""
         return self._command_map.command_coverage
 
     @property
     def command_model(self) -> Dict[str, Dict[str, Dict[str, Dict[str, Any]]]]:
         """Return command to model mapping."""
         return {
-            command: self._provider_interface.map[
-                self._command_map.commands_model[command]
-            ]
-            for command in self._command_map.commands_model
+            command: self._provider_interface.map[value]
+            for command, value in self._command_map.commands_model.items()
         }
 
+    @property
+    def reference(self) -> Dict[str, Dict]:
+        """Return reference data."""
+        return self._reference_loader.reference
+
     def command_schemas(self, filter_by_provider: Optional[str] = None):
         """Return route schema for a command."""
         return get_route_schema_map(
             self._app, self._command_map.commands_model, filter_by_provider
         )
```

### Comparing `openbb_core-1.2.0/openbb_core/app/static/utils/linters.py` & `openbb_core-1.2.1/openbb_core/app/static/utils/linters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Linters for the package."""
+
 import shutil
 import subprocess
 from pathlib import Path
 from typing import (
     List,
     Literal,
     Optional,
```

### Comparing `openbb_core-1.2.0/openbb_core/app/utils.py` & `openbb_core-1.2.1/openbb_core/app/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+"""Utility functions for the OpenBB Core app."""
+
 import ast
 import json
-from typing import Dict, Iterable, List, Optional, Union
+from datetime import time
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from pydantic import ValidationError
 
+from openbb_core.app.model.abstract.error import OpenBBError
 from openbb_core.app.model.preferences import Preferences
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.provider.abstract.data import Data
 
 
 def basemodel_to_df(
     data: Union[List[Data], Data],
-    index: Optional[Union[str, Iterable]] = None,
+    index: Optional[str] = None,
 ) -> pd.DataFrame:
     """Convert list of BaseModel to a Pandas DataFrame."""
     if isinstance(data, list):
         df = pd.DataFrame([d.model_dump() for d in data])
     else:
         try:
             df = pd.DataFrame(data.model_dump())
@@ -25,39 +29,53 @@
             df = pd.DataFrame(data.model_dump(), index=["values"])
 
     if "is_multiindex" in df.columns:
         col_names = ast.literal_eval(df.multiindex_names.unique()[0])
         df = df.set_index(col_names)
         df = df.drop(["is_multiindex", "multiindex_names"], axis=1)
 
+    # If the date column contains dates only, convert them to a date to avoid encoding time data.
+    if "date" in df.columns:
+        df["date"] = df["date"].apply(pd.to_datetime)
+        if all(t.time() == time(0, 0) for t in df["date"]):
+            df["date"] = df["date"].apply(lambda x: x.date())
+
     if index and index in df.columns:
-        df = df.set_index(index)
-        # TODO: This should probably check if the index can be converted to a datetime instead of just assuming
-        if df.index.name == "date":
-            df.index = pd.to_datetime(df.index)
+        if index == "date":
+            df.set_index("date", inplace=True)
             df.sort_index(axis=0, inplace=True)
+        else:
+            df = df.set_index(index) if index and index in df.columns else df
 
     return df
 
 
 def df_to_basemodel(
     df: Union[pd.DataFrame, pd.Series], index: bool = False
 ) -> List[Data]:
     """Convert from a Pandas DataFrame to list of BaseModel."""
-    if index and not isinstance(df.index, pd.MultiIndex):
-        df = df.reset_index(drop=True)
+    is_multiindex = isinstance(df.index, pd.MultiIndex)
+
+    if not is_multiindex and (index or df.index.name):
+        df = df.reset_index()
     if isinstance(df, pd.Series):
         df = df.to_frame()
 
     # Check if df has multiindex.  If so, add the index names to the df and a boolean column
     if isinstance(df.index, pd.MultiIndex):
         df["is_multiindex"] = True
         df["multiindex_names"] = str(df.index.names)
         df = df.reset_index()
 
+    # Converting to JSON will add T00:00:00.000 to all dates with no time element unless we format it as a string first.
+    if "date" in df.columns:
+        df["date"] = df["date"].apply(pd.to_datetime)
+        if all(t.time() == time(0, 0) for t in df["date"]):
+            df["date"] = df["date"].apply(lambda x: x.date().strftime("%Y-%m-%d"))
+
     return [
         Data(**d) for d in json.loads(df.to_json(orient="records", date_format="iso"))
     ]
 
 
 def list_to_basemodel(data_list: List) -> List[Data]:
     """Convert a list to a list of BaseModel."""
@@ -116,27 +134,38 @@
         raise ValueError(
             f"Target column '{target}' not found in data. Choose from {choices}"
         )
     return df[target]
 
 
 def get_target_columns(df: pd.DataFrame, target_columns: List[str]) -> pd.DataFrame:
+    """Get target columns from time series data."""
     df_result = pd.DataFrame()
     for target in target_columns:
         df_result[target] = get_target_column(df, target).to_frame()
     return df_result
 
 
 def get_user_cache_directory() -> str:
+    """Get user cache directory."""
     file = SystemSettings().model_dump()["user_settings_path"]
     with open(file) as settings_file:
         contents = settings_file.read()
     try:
         settings = json.loads(contents)["preferences"]
     except KeyError:
         settings = None
     cache_dir = (
         settings["cache_directory"]
         if settings and "cache_directory" in settings
         else Preferences().cache_directory
     )
     return cache_dir
+
+
+def check_single_item(
+    value: Optional[str], message: Optional[str] = None
+) -> Optional[str]:
+    """Check that string contains a single item."""
+    if value and isinstance(value, str) and ("," in value or ";" in value):
+        raise OpenBBError(message if message else "multiple items not allowed")
+    return value
```

### Comparing `openbb_core-1.2.0/openbb_core/app/version.py` & `openbb_core-1.2.1/openbb_core/app/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Version script for the OpenBB Platform."""
+
 import shutil
 import subprocess
 from pathlib import Path
 
 import pkg_resources
 
 PACKAGE = "openbb"
@@ -43,11 +44,22 @@
             check=True,
         )
         return True
     except subprocess.CalledProcessError:
         return False
 
 
+def get_major_minor(version: str) -> tuple[int, int]:
+    """Retrieve the major and minor version from a version string."""
+    parts = version.split(".")
+    return (int(parts[0]), int(parts[1]))
+
+
 try:
     VERSION = get_package_version(PACKAGE)
 except pkg_resources.DistributionNotFound:
     VERSION = "unknown"
+
+try:
+    CORE_VERSION = get_package_version("openbb-core")
+except pkg_resources.DistributionNotFound:
+    CORE_VERSION = "unknown"
```

### Comparing `openbb_core-1.2.0/openbb_core/env.py` & `openbb_core-1.2.1/openbb_core/env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Environment variables."""
+
 import os
 from pathlib import Path
 from typing import Dict, Optional
 
 import dotenv
 
 from openbb_core.app.constants import OPENBB_DIRECTORY
@@ -10,60 +12,56 @@
 
 class Env(metaclass=SingletonMeta):
     """Environment variables."""
 
     _environ: Dict[str, str]
 
     def __init__(self) -> None:
+        """Initialize the environment."""
         dotenv.load_dotenv(Path(OPENBB_DIRECTORY, ".env"))
         self._environ = os.environ.copy()
 
     @property
     def API_AUTH(self) -> bool:
-        """API authentication: enables API endpoint authentication"""
+        """API authentication: enables API endpoint authentication."""
         return self.str2bool(self._environ.get("OPENBB_API_AUTH", False))
 
     @property
     def API_USERNAME(self) -> Optional[str]:
-        """API username: sets API username"""
+        """API username: sets API username."""
         return self._environ.get("OPENBB_API_USERNAME", None)
 
     @property
     def API_PASSWORD(self) -> Optional[str]:
-        """API password: sets API password"""
+        """API password: sets API password."""
         return self._environ.get("OPENBB_API_PASSWORD", None)
 
     @property
     def API_AUTH_EXTENSION(self) -> Optional[str]:
-        """Auth extension: specifies which authentication extension to use"""
+        """Auth extension: specifies which authentication extension to use."""
         return self._environ.get("OPENBB_API_AUTH_EXTENSION", None)
 
     @property
     def AUTO_BUILD(self) -> bool:
-        """Automatic build: enables automatic package build on import"""
+        """Automatic build: enables automatic package build on import."""
         return self.str2bool(self._environ.get("OPENBB_AUTO_BUILD", True))
 
     @property
-    def CHARTING_EXTENSION(self) -> str:
-        """Charting extension: specifies which charting extension to use"""
-        return self._environ.get("OPENBB_CHARTING_EXTENSION", "openbb_charting")
-
-    @property
     def DEBUG_MODE(self) -> bool:
-        """Debug mode: enables debug mode"""
+        """Debug mode: enables debug mode."""
         return self.str2bool(self._environ.get("OPENBB_DEBUG_MODE", False))
 
     @property
     def DEV_MODE(self) -> bool:
-        """Dev mode: enables development mode"""
+        """Dev mode: enables development mode."""
         return self.str2bool(self._environ.get("OPENBB_DEV_MODE", False))
 
     @property
     def HUB_BACKEND(self) -> str:
-        """Hub backend: sets the backend for the OpenBB Hub"""
+        """Hub backend: sets the backend for the OpenBB Hub."""
         return self._environ.get("OPENBB_HUB_BACKEND", "https://payments.openbb.co")
 
     @staticmethod
     def str2bool(value) -> bool:
         """Match a value to its boolean correspondent."""
         if isinstance(value, bool):
             return value
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/abstract/data.py` & `openbb_core-1.2.1/openbb_core/provider/abstract/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """The OpenBB Standardized Data Model."""
 
 from typing import Dict
 
 from pydantic import (
+    AliasGenerator,
     BaseModel,
     BeforeValidator,
     ConfigDict,
     alias_generators,
     model_validator,
 )
 from typing_extensions import Annotated
@@ -73,21 +74,24 @@
     def __repr__(self):
         """Return a string representation of the object."""
         return f"{self.__class__.__name__}({', '.join([f'{k}={v}' for k, v in super().model_dump().items()])})"
 
     model_config = ConfigDict(
         extra="allow",
         populate_by_name=True,
-        alias_generator=alias_generators.to_camel,
         strict=False,
+        alias_generator=AliasGenerator(
+            validation_alias=alias_generators.to_camel,
+            serialization_alias=alias_generators.to_snake,
+        ),
     )
 
     @model_validator(mode="before")
     @classmethod
     def _use_alias(cls, values):
         """Use alias for error locs."""
         # set the alias dict values keys
         aliases = {orig: alias for alias, orig in cls.__alias_dict__.items()}
-        if aliases:
+        if aliases and isinstance(values, dict):
             return {aliases.get(k, k): v for k, v in values.items()}
 
         return values
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/abstract/fetcher.py` & `openbb_core-1.2.1/openbb_core/provider/abstract/fetcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Abstract class for the fetcher."""
-# ruff: noqa: S101
-# pylint: disable=E1101
+
+# ruff: noqa: S101, E501
+# pylint: disable=E1101, C0301
 
 from typing import (
     Any,
     Dict,
     Generic,
     Optional,
     TypeVar,
+    Union,
     get_args,
     get_origin,
 )
 
 from pandas import DataFrame
 
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.helpers import maybe_coroutine, run_async
 
 Q = TypeVar("Q", bound=QueryParams)
 D = TypeVar("D", bound=Data)
 R = TypeVar("R")  # Return, usually List[D], but can be just D for example
@@ -51,38 +54,38 @@
         """Asynchronously extract the data from the provider."""
 
     @staticmethod
     def extract_data(query: Q, credentials: Optional[Dict[str, str]]) -> Any:
         """Extract the data from the provider."""
 
     @staticmethod
-    def transform_data(query: Q, data: Any, **kwargs) -> R:
+    def transform_data(query: Q, data: Any, **kwargs) -> Union[R, AnnotatedResult[R]]:
         """Transform the provider-specific data."""
         raise NotImplementedError
 
-    def __init_subclass__(cls, **kwargs):
+    def __init_subclass__(cls, *args, **kwargs):
         """Initialize the subclass."""
-        super().__init_subclass__(**kwargs)
+        super().__init_subclass__(*args, **kwargs)
 
         if cls.aextract_data != Fetcher.aextract_data:
-            cls.extract_data = cls.aextract_data
+            cls.extract_data = cls.aextract_data  # type: ignore[method-assign]
         elif cls.extract_data == Fetcher.extract_data:
             raise NotImplementedError(
                 "Fetcher subclass must implement either extract_data or aextract_data"
                 " method. If both are implemented, aextract_data will be used as the"
                 " default."
             )
 
     @classmethod
     async def fetch_data(
         cls,
         params: Dict[str, Any],
         credentials: Optional[Dict[str, str]] = None,
         **kwargs,
-    ) -> R:
+    ) -> Union[R, AnnotatedResult[R]]:
         """Fetch data from a provider."""
         query = cls.transform_query(params=params)
         data = await maybe_coroutine(
             cls.extract_data, query=query, credentials=credentials, **kwargs
         )
         return cls.transform_data(query=query, data=data, **kwargs)
 
@@ -134,75 +137,93 @@
         AssertionError
             If any of the tests fail.
         """
         query = cls.transform_query(params=params)
         data = run_async(
             cls.extract_data, query=query, credentials=credentials, **kwargs
         )
-        transformed_data = cls.transform_data(query=query, data=data, **kwargs)
+        result = cls.transform_data(query=query, data=data, **kwargs)
 
         # Class Assertions
-        assert isinstance(cls.require_credentials, bool)
+        assert isinstance(
+            cls.require_credentials, bool
+        ), "require_credentials must be a boolean."
 
         # Query Assertions
-        assert query
-        assert issubclass(type(query), cls.query_params_type)
-        assert all(getattr(query, key) == value for key, value in params.items())
+        assert query, "Query must not be None."
+        assert issubclass(
+            type(query), cls.query_params_type
+        ), f"Query type mismatch. Expected: {cls.query_params_type} Got: {type(query)}"
+        assert all(
+            getattr(query, key) == value for key, value in params.items()
+        ), f"Query must have the correct values. Expected: {params} Got: {query.__dict__}"
 
         # Data Assertions
         if not isinstance(data, DataFrame):
-            assert data
+            assert data, "Data must not be None."
         else:
-            assert not data.empty
+            assert not data.empty, "Data must not be empty."
         is_list = isinstance(data, list)
         if is_list:
             assert all(
                 field in data[0]
                 for field in cls.data_type.__fields__
                 if field in data[0]
-            )
+            ), f"Data must have the correct fields. Expected: {cls.data_type.__fields__} Got: {data[0].__dict__}"
             # This makes sure that the data is not transformed yet so that the
             # pipeline is implemented correctly. We can remove this assertion if we
             # want to be less strict.
-            assert issubclass(type(data[0]), cls.data_type) is False
+            assert (
+                issubclass(type(data[0]), cls.data_type) is False
+            ), f"Data must not be transformed yet. Expected: {cls.data_type} Got: {type(data[0])}"
         else:
             assert all(
                 field in data for field in cls.data_type.__fields__ if field in data
-            )
-            assert issubclass(type(data), cls.data_type) is False
+            ), f"Data must have the correct fields. Expected: {cls.data_type.__fields__} Got: {data.__dict__}"
+            assert (
+                issubclass(type(data), cls.data_type) is False
+            ), f"Data must not be transformed yet. Expected: {cls.data_type} Got: {type(data)}"
 
-        assert len(data) > 0
+        assert len(data) > 0, "Data must not be empty."
 
         # Transformed Data Assertions
-        assert transformed_data
+        transformed_data = (
+            result.result if isinstance(result, AnnotatedResult) else result
+        )
 
-        is_list = isinstance(transformed_data, list)
-        if is_list:
+        assert transformed_data, "Transformed data must not be None."
+
+        if isinstance(transformed_data, list):
             return_type_args = cls.return_type.__args__[0]
             return_type_is_dict = (
                 hasattr(return_type_args, "__origin__")
                 and return_type_args.__origin__ is dict
             )
             if return_type_is_dict:
                 return_type_fields = return_type_args.__args__[1].__args__[0].__fields__
                 return_type = return_type_args.__args__[1].__args__[0]
             else:
                 return_type_fields = return_type_args.__fields__
                 return_type = return_type_args
 
-            assert len(transformed_data) > 0  # type: ignore
+            assert len(transformed_data) > 0, "Transformed data must not be empty."  # type: ignore
             assert all(
-                field in transformed_data[0].__dict__  # type: ignore
-                for field in return_type_fields
-            )
-            assert issubclass(type(transformed_data[0]), cls.data_type)  # type: ignore
+                field in transformed_data[0].__dict__ for field in return_type_fields  # type: ignore
+            ), f"Transformed data must have the correct fields. Expected: {return_type_fields} Got: {transformed_data[0].__dict__}"  # type: ignore
             assert issubclass(
+                type(transformed_data[0]), cls.data_type  # type: ignore
+            ), f"Transformed data must be of the correct type. Expected: {cls.data_type} Got: {type(transformed_data[0])}"  # type: ignore
+            assert issubclass(  # type: ignore
                 type(transformed_data[0]),  # type: ignore
                 return_type,
-            )
+            ), f"Transformed data must be of the correct type. Expected: {return_type} Got: {type(transformed_data[0])}"  # type: ignore
         else:
             assert all(
                 field in transformed_data.__dict__
                 for field in cls.return_type.__fields__
-            )
-            assert issubclass(type(transformed_data), cls.data_type)
-            assert issubclass(type(transformed_data), cls.return_type)
+            ), f"Transformed data must have the correct fields. Expected: {cls.return_type.__fields__} Got: {transformed_data.__dict__}"
+            assert issubclass(
+                type(transformed_data), cls.data_type
+            ), f"Transformed data must be of the correct type. Expected: {cls.data_type} Got: {type(transformed_data)}"
+            assert issubclass(
+                type(transformed_data), cls.return_type
+            ), f"Transformed data must be of the correct type. Expected: {cls.return_type} Got: {type(transformed_data)}"
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/abstract/provider.py` & `openbb_core-1.2.1/openbb_core/provider/abstract/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,40 +4,53 @@
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 
 
 class Provider:
     """Serves as provider extension entry point and must be created by each provider."""
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         name: str,
         description: str,
         website: Optional[str] = None,
         credentials: Optional[List[str]] = None,
         fetcher_dict: Optional[Dict[str, Type[Fetcher]]] = None,
+        repr_name: Optional[str] = None,
+        v3_credentials: Optional[List[str]] = None,
+        instructions: Optional[str] = None,
     ) -> None:
         """Initialize the provider.
 
         Parameters
         ----------
         name : str
             Name of the provider.
         description : str
             Description of the provider.
         website : Optional[str]
             Website of the provider, by default None.
-        credentials : Optional[List[str]], optional
-            List of required credentials, by default None
+        credentials : Optional[List[str]]
+            List of required credentials, by default None.
         fetcher_dict : Optional[Dict[str, Type[Fetcher]]]
             Dictionary of fetchers, by default None.
+        repr_name: Optional[str]
+            Full name of the provider, by default None.
+        v3_credentials: Optional[List[str]]
+            List of corresponding v3 credentials, by default None.
+        instructions: Optional[str]
+            Instructions on how to setup the provider. For example, how to get an API key.
         """
         self.name = name
         self.description = description
         self.website = website
         self.fetcher_dict = fetcher_dict or {}
         if credentials is None:
             self.credentials: List = []
         else:
             self.credentials = []
             for c in credentials:
                 self.credentials.append(f"{self.name.lower()}_{c}")
+        self.repr_name = repr_name
+        self.v3_credentials = v3_credentials
+        self.instructions = instructions
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/query_executor.py` & `openbb_core-1.2.1/openbb_core/provider/query_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query executor module."""
+
 from typing import Any, Dict, Optional, Type
 
 from pydantic import SecretStr
 
 from openbb_core.app.model.abstract.error import OpenBBError
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.abstract.provider import Provider
@@ -88,12 +89,8 @@
             Query result.
         """
         provider = self.get_provider(provider_name)
         fetcher = self.get_fetcher(provider, model_name)
         filtered_credentials = self.filter_credentials(
             credentials, provider, fetcher.require_credentials
         )
-
-        try:
-            return await fetcher.fetch_data(params, filtered_credentials, **kwargs)
-        except Exception as e:
-            raise OpenBBError(e) from e
+        return await fetcher.fetch_data(params, filtered_credentials, **kwargs)
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/registry.py` & `openbb_core-1.2.1/openbb_core/provider/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Provider Registry Module."""
 
 import traceback
 import warnings
 from functools import lru_cache
 from typing import Dict
 
-from importlib_metadata import entry_points
-
+from openbb_core.app.extension_loader import ExtensionLoader
 from openbb_core.app.model.abstract.warning import OpenBBWarning
 from openbb_core.env import Env
 from openbb_core.provider.abstract.provider import Provider
 
 
 class Registry:
     """Maintain registry of providers."""
@@ -37,21 +36,20 @@
     """Load providers from entry points."""
 
     @staticmethod
     @lru_cache
     def from_extensions() -> Registry:
         """Load providers from entry points."""
         registry = Registry()
-        for entry_point in sorted(entry_points(group="openbb_provider_extension")):
+
+        for name, entry in ExtensionLoader().provider_objects.items():
             try:
-                entry = entry_point.load()
-                if isinstance(entry, Provider):
-                    registry.include_provider(provider=entry)
+                registry.include_provider(provider=entry)
             except Exception as e:
-                msg = f"Error loading extension: {entry_point.name}\n"
+                msg = f"Error loading extension: {name}\n"
                 if Env().DEBUG_MODE:
                     traceback.print_exception(type(e), e, e.__traceback__)
                     raise LoadingError(msg + f"\033[91m{e}\033[0m") from e
                 warnings.warn(
                     message=msg,
                     category=OpenBBWarning,
                 )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """AMERIBOR Standard Model."""
 
-
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/available_indices.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/available_indices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Available Indices Standard Model."""
 
-
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Balance Sheet Statement Growth Standard Model."""
 
-
 from datetime import date as dateType
 from typing import List, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -17,19 +16,18 @@
 class BalanceSheetGrowthQueryParams(QueryParams):
     """Balance Sheet Statement Growth Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
     limit: int = Field(default=10, description=QUERY_DESCRIPTIONS.get("limit", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    @classmethod
+    def to_upper(cls, v: str):
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class BalanceSheetGrowthData(Data):
     """Balance Sheet Statement Growth Data."""
 
     symbol: Optional[str] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
@@ -127,12 +125,13 @@
     growth_total_investments: float = Field(
         description="Growth rate of total investments."
     )
     growth_total_debt: float = Field(description="Growth rate of total debt.")
     growth_net_debt: float = Field(description="Growth rate of net debt.")
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    @classmethod
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)]) if v else None
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/bond_prices.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/bond_prices.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Bond Prices Standard Model."""
 
 from datetime import (
     date as dateType,
 )
 from typing import List, Optional, Union
 
-from pydantic import Field, field_validator
+from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 
 
 class BondPricesQueryParams(QueryParams):
     """Bond Prices Query."""
 
     country: Optional[str] = Field(
         default=None,
-        description="Country of the bond issuer. Matches partial name.",
+        description="The country to get data. Matches partial name.",
     )
     issuer_name: Optional[str] = Field(
         default=None,
         description="Name of the issuer.  Returns partial matches and is case insensitive.",
     )
     isin: Optional[Union[List, str]] = Field(
         default=None,
@@ -63,23 +63,14 @@
         description="Maximum yield to maturity of the bond.",
     )
     ytm_min: Optional[float] = Field(
         default=None,
         description="Minimum yield to maturity of the bond.",
     )
 
-    @field_validator("isin", "currency", "lei", mode="before", check_fields=False)
-    @classmethod
-    def validate_upper_case(cls, v):
-        """Convert the field to uppercase and convert a list to a query string."""
-        if isinstance(v, str):
-            return v.upper()
-        v = ",".join([symbol.upper() for symbol in list(v)])
-        return v if v else None
-
 
 class BondPricesData(Data):
     """Bond Prices Data."""
 
     isin: Optional[str] = Field(
         default=None,
         description="International Securities Identification Number of the bond.",
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/bond_reference.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/bond_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class BondReferenceQueryParams(QueryParams):
     """Bond Reference Query."""
 
     country: Optional[str] = Field(
         default=None,
-        description="Country of the bond issuer. Matches partial name.",
+        description="The country to get data. Matches partial name.",
     )
     issuer_name: Optional[str] = Field(
         default=None,
         description="Name of the issuer.  Returns partial matches and is case insensitive.",
     )
     isin: Optional[Union[List, str]] = Field(
         default=None,
@@ -61,16 +61,15 @@
 
     @field_validator("isin", "currency", "lei", mode="before", check_fields=False)
     @classmethod
     def validate_upper_case(cls, v):
         """Convert the field to uppercase and convert a list to a query string."""
         if isinstance(v, str):
             return v.upper()
-        v = ",".join([symbol.upper() for symbol in list(v)])
-        return v if v else None
+        return ",".join([symbol.upper() for symbol in list(v)]) if v else None
 
 
 class BondReferenceData(Data):
     """Bond Reference Search Data."""
 
     isin: Optional[str] = Field(
         default=None,
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/bond_trades.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/bond_trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class BondTradesQueryParams(QueryParams):
     """Bond Trades Query."""
 
     country: Optional[str] = Field(
         default=None,
-        description="Country of the bond issuer. Matches partial name.",
+        description="The country to get data. Matches partial name.",
     )
     isin: Optional[str] = Field(
         default=None,
         description="ISIN of the bond.",
     )
     issuer_type: Optional[Literal["government", "corporate", "municipal"]] = Field(
         default=None,
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Dividend Calendar Standard Model."""
 
-
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -24,20 +23,20 @@
         default=None, description=QUERY_DESCRIPTIONS.get("end_date", "")
     )
 
 
 class CalendarDividendData(Data):
     """Dividend Calendar Data."""
 
-    date: dateType = Field(
-        description=DATA_DESCRIPTIONS.get("date", "") + " (Ex-Dividend)"
+    ex_dividend_date: dateType = Field(
+        description="The ex-dividend date - the date on which the stock begins trading without rights to the dividend."
     )
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     amount: Optional[float] = Field(
-        default=None, description="Dividend amount, per-share."
+        default=None, description="The dividend amount per share."
     )
     name: Optional[str] = Field(default=None, description="Name of the entity.")
     record_date: Optional[dateType] = Field(
         default=None,
         description="The record date of ownership for eligibility.",
     )
     payment_date: Optional[dateType] = Field(
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Earnings Calendar Standard Model."""
 
-
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     )
     limit: Optional[int] = Field(
         description=QUERY_DESCRIPTIONS.get("limit", ""), default=100
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: str):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: str):
+        """Convert field to uppercase."""
         return v.upper() if v else None
 
     @field_validator("start_date", mode="before", check_fields=False)
     @classmethod
     def start_date_validate(cls, v):  # pylint: disable=E0213
         """Return the date as a datetime object."""
         return datetime.strftime(v, "%Y-%m-%d") if v else None
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Calendar Splits Standard Model."""
 
-
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/cash_flow.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,143 +1,151 @@
-"""Cash Flow Statement Standard Model."""
-
+"""Equity Info Standard Model."""
 
 from datetime import date as dateType
-from typing import List, Literal, Optional, Set, Union
+from typing import List, Optional, Set, Union
 
-from pydantic import Field, NonNegativeInt, StrictFloat, field_validator
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class CashFlowStatementQueryParams(QueryParams):
-    """Cash Flow Statement Query."""
+class EquityInfoQueryParams(QueryParams):
+    """Equity Info Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    period: Optional[Literal["annual", "quarter"]] = Field(
-        default="annual",
-        description=QUERY_DESCRIPTIONS.get("period", ""),
-    )
-    limit: Optional[NonNegativeInt] = Field(
-        default=5, description=QUERY_DESCRIPTIONS.get("limit", "")
-    )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        return v.split(",")[0].upper() if "," in v else v.upper()
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class CashFlowStatementData(Data):
-    """Cash Flow Statement Data."""
+class EquityInfoData(Data):
+    """Equity Info Data."""
 
-    symbol: Optional[str] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
-    )
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date" ""))
-    period: Optional[str] = Field(
-        default=None, description="Reporting period of the statement."
-    )
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    name: Optional[str] = Field(default=None, description="Common name of the company.")
     cik: Optional[str] = Field(
         default=None,
         description=DATA_DESCRIPTIONS.get("cik", ""),
     )
-
-    net_income: Optional[StrictFloat] = Field(default=None, description="Net income.")
-
-    depreciation_and_amortization: Optional[StrictFloat] = Field(
-        default=None, description="Depreciation and amortization."
+    cusip: Optional[str] = Field(
+        default=None, description="CUSIP identifier for the company."
     )
-    stock_based_compensation: Optional[StrictFloat] = Field(
-        default=None, description="Stock based compensation."
+    isin: Optional[str] = Field(
+        default=None, description="International Securities Identification Number."
     )
-    deferred_income_tax: Optional[StrictFloat] = Field(
-        default=None, description="Deferred income tax."
+    lei: Optional[str] = Field(
+        default=None, description="Legal Entity Identifier assigned to the company."
     )
-    other_non_cash_items: Optional[StrictFloat] = Field(
-        default=None, description="Other non-cash items."
+    legal_name: Optional[str] = Field(
+        default=None, description="Official legal name of the company."
     )
-    changes_in_operating_assets_and_liabilities: Optional[StrictFloat] = Field(
-        default=None, description="Changes in operating assets and liabilities."
+    stock_exchange: Optional[str] = Field(
+        default=None, description="Stock exchange where the company is traded."
     )
-
-    accounts_receivables: Optional[StrictFloat] = Field(
-        default=None, description="Accounts receivables."
+    sic: Optional[int] = Field(
+        default=None,
+        description="Standard Industrial Classification code for the company.",
     )
-    inventory: Optional[StrictFloat] = Field(default=None, description="Inventory.")
-    vendor_non_trade_receivables: Optional[StrictFloat] = Field(
-        default=None, description="Vendor non-trade receivables."
+    short_description: Optional[str] = Field(
+        default=None, description="Short description of the company."
     )
-    other_current_and_non_current_assets: Optional[StrictFloat] = Field(
-        default=None, description="Other current and non-current assets."
+    long_description: Optional[str] = Field(
+        default=None, description="Long description of the company."
     )
-    accounts_payables: Optional[StrictFloat] = Field(
-        default=None, description="Accounts payables."
+    ceo: Optional[str] = Field(
+        default=None, description="Chief Executive Officer of the company."
     )
-    deferred_revenue: Optional[StrictFloat] = Field(
-        default=None, description="Deferred revenue."
+    company_url: Optional[str] = Field(
+        default=None, description="URL of the company's website."
     )
-    other_current_and_non_current_liabilities: Optional[StrictFloat] = Field(
-        default=None, description="Other current and non-current liabilities."
+    business_address: Optional[str] = Field(
+        default=None, description="Address of the company's headquarters."
     )
-    net_cash_flow_from_operating_activities: Optional[StrictFloat] = Field(
-        default=None, description="Net cash flow from operating activities."
+    mailing_address: Optional[str] = Field(
+        default=None, description="Mailing address of the company."
     )
-
-    purchases_of_marketable_securities: Optional[StrictFloat] = Field(
-        default=None, description="Purchases of investments."
+    business_phone_no: Optional[str] = Field(
+        default=None, description="Phone number of the company's headquarters."
     )
-    sales_from_maturities_of_investments: Optional[StrictFloat] = Field(
-        default=None, description="Sales and maturities of investments."
+    hq_address1: Optional[str] = Field(
+        default=None, description="Address of the company's headquarters."
     )
-    investments_in_property_plant_and_equipment: Optional[StrictFloat] = Field(
-        default=None, description="Investments in property, plant, and equipment."
+    hq_address2: Optional[str] = Field(
+        default=None, description="Address of the company's headquarters."
     )
-    payments_from_acquisitions: Optional[StrictFloat] = Field(
-        default=None, description="Acquisitions, net of cash acquired, and other"
+    hq_address_city: Optional[str] = Field(
+        default=None, description="City of the company's headquarters."
     )
-    other_investing_activities: Optional[StrictFloat] = Field(
-        default=None, description="Other investing activities"
+    hq_address_postal_code: Optional[str] = Field(
+        default=None, description="Zip code of the company's headquarters."
     )
-    net_cash_flow_from_investing_activities: Optional[StrictFloat] = Field(
-        default=None, description="Net cash used for investing activities."
+    hq_state: Optional[str] = Field(
+        default=None, description="State of the company's headquarters."
     )
-
-    taxes_paid_on_net_share_settlement: Optional[StrictFloat] = Field(
-        default=None, description="Taxes paid on net share settlement of equity awards."
+    hq_country: Optional[str] = Field(
+        default=None, description="Country of the company's headquarters."
+    )
+    inc_state: Optional[str] = Field(
+        default=None, description="State in which the company is incorporated."
+    )
+    inc_country: Optional[str] = Field(
+        default=None, description="Country in which the company is incorporated."
+    )
+    employees: Optional[int] = Field(
+        default=None, description="Number of employees working for the company."
+    )
+    entity_legal_form: Optional[str] = Field(
+        default=None, description="Legal form of the company."
     )
-    dividends_paid: Optional[StrictFloat] = Field(
-        default=None, description="Payments for dividends and dividend equivalents"
+    entity_status: Optional[str] = Field(
+        default=None, description="Status of the company."
     )
-    common_stock_repurchased: Optional[StrictFloat] = Field(
-        default=None, description="Payments related to repurchase of common stock"
+    latest_filing_date: Optional[dateType] = Field(
+        default=None, description="Date of the company's latest filing."
     )
-    debt_proceeds: Optional[StrictFloat] = Field(
-        default=None, description="Proceeds from issuance of term debt"
+    irs_number: Optional[str] = Field(
+        default=None, description="IRS number assigned to the company."
     )
-    debt_repayment: Optional[StrictFloat] = Field(
-        default=None, description="Payments of long-term debt"
+    sector: Optional[str] = Field(
+        default=None, description="Sector in which the company operates."
     )
-    other_financing_activities: Optional[StrictFloat] = Field(
-        default=None, description="Other financing activities, net"
+    industry_category: Optional[str] = Field(
+        default=None, description="Category of industry in which the company operates."
     )
-    net_cash_flow_from_financing_activities: Optional[StrictFloat] = Field(
-        default=None, description="Net cash flow from financing activities."
+    industry_group: Optional[str] = Field(
+        default=None, description="Group of industry in which the company operates."
     )
-    net_change_in_cash: Optional[StrictFloat] = Field(
+    template: Optional[str] = Field(
         default=None,
-        description="Net increase (decrease) in cash, cash equivalents, and restricted cash",
+        description="Template used to standardize the company's financial statements.",
+    )
+    standardized_active: Optional[bool] = Field(
+        default=None, description="Whether the company is active or not."
+    )
+    first_fundamental_date: Optional[dateType] = Field(
+        default=None, description="Date of the company's first fundamental."
+    )
+    last_fundamental_date: Optional[dateType] = Field(
+        default=None, description="Date of the company's last fundamental."
+    )
+    first_stock_price_date: Optional[dateType] = Field(
+        default=None, description="Date of the company's first stock price."
+    )
+    last_stock_price_date: Optional[dateType] = Field(
+        default=None, description="Date of the company's last stock price."
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)]) if v else None
+        return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Cash Flow Statement Growth Standard Model."""
 
-
 from datetime import date as dateType
 from typing import List, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -17,19 +16,18 @@
 class CashFlowStatementGrowthQueryParams(QueryParams):
     """Cash Flow Statement Growth Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
     limit: int = Field(default=10, description=QUERY_DESCRIPTIONS.get("limit", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    @classmethod
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class CashFlowStatementGrowthData(Data):
     """Cash Flow Statement Growth Data."""
 
     symbol: Optional[str] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
@@ -114,12 +112,13 @@
     )
     growth_capital_expenditure: float = Field(
         description="Growth rate of capital expenditure."
     )
     growth_free_cash_flow: float = Field(description="Growth rate of free cash flow.")
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    @classmethod
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)]) if v else None
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/company_filings.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,54 @@
-"""Company Filings Standard Model."""
+"""Revenue by Geographic Segments Standard Model."""
 
-from datetime import (
-    date as dateType,
-    datetime,
-)
-from typing import List, Optional, Set, Union
+from datetime import date as dateType
+from typing import Dict, Literal, Optional
 
-from dateutil import parser
-from pydantic import Field, NonNegativeInt, field_validator
+from pydantic import Field, field_validator
 
-from openbb_core.provider.abstract.data import Data
+from openbb_core.provider.abstract.data import Data, ForceInt
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class CompanyFilingsQueryParams(QueryParams):
-    """Company Filings Query."""
+class RevenueGeographicQueryParams(QueryParams):
+    """Revenue by Geographic Segments Query."""
 
-    symbol: Optional[str] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("symbol", "")
-    )
-    form_type: Optional[str] = Field(
-        default=None,
-        description=(
-            "Filter by form type. Visit https://www.sec.gov/forms "
-            "for a list of supported form types."
-        ),
-    )
-    limit: NonNegativeInt = Field(
-        default=100, description=QUERY_DESCRIPTIONS.get("limit", "")
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    period: Literal["quarter", "annual"] = Field(
+        default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
     )
+    structure: Literal["hierarchical", "flat"] = Field(
+        default="flat", description="Structure of the returned data."
+    )  # should always be flat
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)]) if v else None
+    def to_upper(cls, v: str):
+        """Convert field to uppercase."""
+        return v.upper()
+
+    @field_validator("period", "structure", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
 
 
-class CompanyFilingsData(Data):
-    """Company Filings Data."""
+class RevenueGeographicData(Data):
+    """Revenue by Geographic Segments Data."""
 
-    symbol: Optional[str] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
+    period_ending: dateType = Field(description="The end date of the reporting period.")
+    fiscal_period: Optional[str] = Field(
+        default=None, description="The fiscal period of the reporting period."
     )
-    cik: Optional[str] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("cik", "")
+    fiscal_year: Optional[int] = Field(
+        default=None, description="The fiscal year of the reporting period."
+    )
+    filing_date: Optional[dateType] = Field(
+        default=None, description="The filing date of the report."
+    )
+    geographic_segment: Dict[str, ForceInt] = Field(
+        description="Dictionary of the revenue by geographic segment."
     )
-    filing_date: dateType = Field(description="Filing date of the SEC report.")
-    accepted_date: datetime = Field(description="Accepted date of the SEC report.")
-    report_type: str = Field(description="Type of the SEC report.")
-    filing_url: str = Field(description="URL to the filing page on the SEC site.")
-    report_url: str = Field(description="URL to the actual report on the SEC site.")
-
-    @field_validator("symbol", mode="before", check_fields=False)
-    @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)]) if v else None
-
-    @field_validator("date", "filing_date", mode="before", check_fields=False)
-    @classmethod
-    def convert_date(cls, v: str):
-        """Convert date to date type."""
-        return parser.parse(str(v)).date()
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/company_news.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/fred_series.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,42 @@
-"""Company News Standard Model."""
+"""FRED Series Standard Model."""
 
-
-from datetime import datetime
+from datetime import date as dateType
 from typing import Optional
 
-from pydantic import Field, NonNegativeInt, field_validator
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class CompanyNewsQueryParams(QueryParams):
-    """Company news Query."""
+class SeriesQueryParams(QueryParams):
+    """FRED Series Query."""
 
-    symbols: str = Field(
-        min_length=1,
-        description=QUERY_DESCRIPTIONS.get("symbols", "")
-        + " Here it is a separated list of symbols.",
+    symbol: str = Field(
+        description=QUERY_DESCRIPTIONS.get("symbol", ""),
+    )
+    start_date: Optional[dateType] = Field(
+        description=QUERY_DESCRIPTIONS.get("start_date", ""), default=None
+    )
+    end_date: Optional[dateType] = Field(
+        description=QUERY_DESCRIPTIONS.get("end_date", ""), default=None
     )
-    limit: Optional[NonNegativeInt] = Field(
-        default=20, description=QUERY_DESCRIPTIONS.get("limit", "")
+    limit: Optional[int] = Field(
+        description=QUERY_DESCRIPTIONS.get("limit", ""), default=100000
     )
 
-    @field_validator("symbols", mode="before")
+    @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def symbols_validate(cls, v: str):  # pylint: disable=E0213
-        """Validate the symbols."""
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
         return v.upper()
 
 
-class CompanyNewsData(Data):
-    """Company News Data."""
+class SeriesData(Data):
+    """FRED Series Data."""
 
-    symbols: str = Field(
-        min_length=1,
-        description=DATA_DESCRIPTIONS.get("symbols", "")
-        + " Here it is a separated list of symbols.",
-    )
-    date: datetime = Field(
-        description=DATA_DESCRIPTIONS.get("date", "")
-        + " Here it is the date of the news."
-    )
-    title: str = Field(description="Title of the news.")
-    image: Optional[str] = Field(default=None, description="Image URL of the news.")
-    text: Optional[str] = Field(default=None, description="Text/body of the news.")
-    url: str = Field(description="URL of the news.")
+    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/company_overview.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/company_overview.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Company Overview Standard Model."""
 
-
 from datetime import date
 from typing import List, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data, ForceInt
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -17,19 +16,17 @@
 class CompanyOverviewQueryParams(QueryParams):
     """Company Overview Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class CompanyOverviewData(Data):
     """Company Overview Data.
 
     Returns the profile of a given company.
     """
@@ -99,12 +96,12 @@
     is_etf: bool = Field(description="If the company is an ETF.")
     is_actively_trading: bool = Field(description="If the company is actively trading.")
     is_adr: bool = Field(description="If the company is an ADR.")
     is_fund: bool = Field(description="If the company is a fund.")
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/cot.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/cot_search.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/cot_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 
 
 class CotSearchQueryParams(QueryParams):
     """Commitment of Traders Reports Search Query."""
 
     query: str = Field(description="Search query.", default="")
+    use_cache: Optional[bool] = Field(
+        default=True,
+        description="Whether or not to use cache.",
+    )
 
 
 class CotSearchData(Data):
     """Commitment of Traders Reports Search Data."""
 
     code: str = Field(description="CFTC Code of the report.")
     name: str = Field(description="Name of the underlying asset.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/cp.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/economic_indicators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-"""Commercial Paper Standard Model."""
-from datetime import (
-    date as dateType,
-)
-from typing import Literal, Optional
+"""Economic Indicators Standard Model."""
+
+from datetime import date as dateType
+from typing import Optional, Union
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class CommercialPaperParams(QueryParams):
-    """Commercial Paper Query."""
+class EconomicIndicatorsQueryParams(QueryParams):
+    """Economic Indicators Query."""
 
-    start_date: Optional[dateType] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("start_date", ""),
+    symbol: str = Field(
+        description=QUERY_DESCRIPTIONS.get("symbol", "")
+        + " The base symbol for the indicator (e.g. GDP, CPI, etc.).",
     )
-    end_date: Optional[dateType] = Field(
+    country: Optional[str] = Field(
         default=None,
-        description=QUERY_DESCRIPTIONS.get("end_date", ""),
-    )
-    maturity: Literal["overnight", "7d", "15d", "30d", "60d", "90d"] = Field(
-        default="30d",
-        description="The maturity.",
+        description=QUERY_DESCRIPTIONS.get("country", "")
+        + " The country represented by the indicator, if available.",
     )
-    category: Literal["asset_backed", "financial", "nonfinancial"] = Field(
-        default="financial",
-        description="The category.",
+    start_date: Optional[dateType] = Field(
+        description=QUERY_DESCRIPTIONS.get("start_date", ""), default=None
     )
-    grade: Literal["aa", "a2_p2"] = Field(
-        default="aa",
-        description="The grade.",
+    end_date: Optional[dateType] = Field(
+        description=QUERY_DESCRIPTIONS.get("end_date", ""), default=None
     )
 
 
-class CommercialPaperData(Data):
-    """Commercial Paper Data."""
+class EconomicIndicatorsData(Data):
+    """Economic Indicators Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    rate: Optional[float] = Field(description="Commercial Paper Rate.")
+    symbol_root: Optional[str] = Field(
+        default=None, description="The root symbol for the indicator (e.g. GDP)."
+    )
+    symbol: Optional[str] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
+    )
+    country: Optional[str] = Field(
+        default=None, description="The country represented by the data."
+    )
+    value: Optional[Union[int, float]] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("value", "")
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/cpi.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/cpi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """CPI Standard Model."""
+
 from datetime import date as dateType
-from typing import List, Literal, Optional
+from typing import Literal, Optional
 
 from dateutil import parser
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
+from openbb_core.provider.utils.helpers import check_item
 
-CPI_COUNTRIES = Literal[
+CPI_COUNTRIES = [
     "australia",
     "austria",
     "belgium",
     "brazil",
     "bulgaria",
     "canada",
     "chile",
@@ -68,16 +70,17 @@
 
 CPI_FREQUENCY = Literal["monthly", "quarter", "annual"]
 
 
 class ConsumerPriceIndexQueryParams(QueryParams):
     """CPI Query."""
 
-    countries: List[CPI_COUNTRIES] = Field(
-        description=QUERY_DESCRIPTIONS.get("countries")
+    country: str = Field(
+        description=QUERY_DESCRIPTIONS.get("country"),
+        json_schema_extra={"choices": CPI_COUNTRIES},  # type: ignore[dict-item]
     )
     units: CPI_UNITS = Field(
         default="growth_same",
         description=QUERY_DESCRIPTIONS.get("units", "")
         + """
     Options:
     - `growth_previous`: Percent growth from the previous period.
@@ -98,14 +101,24 @@
     start_date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("start_date")
     )
     end_date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("end_date")
     )
 
+    @field_validator("country", mode="before", check_fields=False)
+    def validate_country(cls, c: str):  # pylint: disable=E0213
+        """Validate country."""
+        result = []
+        values = c.replace(" ", "_").split(",")
+        for v in values:
+            check_item(v.lower(), CPI_COUNTRIES)
+            result.append(v.lower())
+        return ",".join(result)
+
 
 class ConsumerPriceIndexData(Data):
     """CPI data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date"))
 
     @field_validator("date", mode="before")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Crypto Historical Price Standard Model."""
 
-
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import List, Optional, Set, Union
 
 from dateutil import parser
@@ -33,31 +32,35 @@
         default=None,
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def validate_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase and remove '-'."""
+        """Convert field to uppercase and remove '-'."""
         if isinstance(v, str):
             return v.upper().replace("-", "")
         return ",".join([symbol.upper().replace("-", "") for symbol in list(v)])
 
 
 class CryptoHistoricalData(Data):
     """Crypto Historical Price Data."""
 
-    date: datetime = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    date: Union[dateType, datetime] = Field(
+        description=DATA_DESCRIPTIONS.get("date", "")
+    )
     open: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("open", ""))
     high: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("high", ""))
     low: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("low", ""))
     close: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("close", ""))
     volume: float = Field(description=DATA_DESCRIPTIONS.get("volume", ""))
     vwap: Optional[PositiveFloat] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("vwap", "")
     )
 
     @field_validator("date", mode="before", check_fields=False)
     @classmethod
     def date_validate(cls, v):  # pylint: disable=E0213
         """Return formatted datetime."""
-        return parser.isoparse(str(v))
+        if ":" in str(v):
+            return parser.isoparse(str(v))
+        return parser.parse(str(v)).date()
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/crypto_search.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/crypto_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 
 
 class CryptoSearchQueryParams(QueryParams):
     """Crypto Search Query."""
 
-    query: Optional[str] = Field(description="Search query.", default="")
+    query: Optional[str] = Field(description="Search query.", default=None)
 
 
 class CryptoSearchData(Data):
     """Crypto Search Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", "") + " (Crypto)")
     name: Optional[str] = Field(description="Name of the crypto.", default=None)
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/currency_historical.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/currency_historical.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Currency Historical Price Standard Model."""
 
-
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import List, Optional, Set, Union
 
 from dateutil import parser
@@ -34,32 +33,36 @@
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     def validate_symbol(
         cls, v: Union[str, List[str], Set[str]]
     ):  # pylint: disable=E0213
-        """Convert symbol to uppercase and remove '-'."""
+        """Convert field to uppercase and remove '-'."""
         if isinstance(v, str):
             return v.upper().replace("-", "")
         return ",".join([symbol.upper().replace("-", "") for symbol in list(v)])
 
 
 class CurrencyHistoricalData(Data):
     """Currency Historical Price Data."""
 
-    date: datetime = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    date: Union[dateType, datetime] = Field(
+        description=DATA_DESCRIPTIONS.get("date", "")
+    )
     open: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("open", ""))
     high: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("high", ""))
     low: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("low", ""))
     close: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("close", ""))
     volume: Optional[float] = Field(
         description=DATA_DESCRIPTIONS.get("volume", ""), default=None
     )
     vwap: Optional[PositiveFloat] = Field(
         description=DATA_DESCRIPTIONS.get("vwap", ""), default=None
     )
 
     @field_validator("date", mode="before", check_fields=False)
     def date_validate(cls, v):  # pylint: disable=E0213
         """Return formatted datetime."""
-        return parser.isoparse(str(v))
+        if ":" in str(v):
+            return parser.isoparse(str(v))
+        return parser.parse(str(v)).date()
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Discount Window Primary Credit Rate Standard Model."""
+
 from datetime import (
     date as dateType,
 )
 from typing import Optional
 
 from pydantic import Field
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Earnings Call Transcript Standard Model."""
 
-
 from datetime import datetime
 from typing import List, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -18,30 +17,28 @@
     """Earnings Call Transcript rating Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
     year: int = Field(description="Year of the earnings call transcript.")
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class EarningsCallTranscriptData(Data):
     """Earnings Call Transcript Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     quarter: int = Field(description="Quarter of the earnings call transcript.")
     year: int = Field(description="Year of the earnings call transcript.")
     date: datetime = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     content: str = Field(description="Content of the earnings call transcript.")
 
     @field_validator("symbol", mode="before")
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-"""European Central Bank Interest Rates Standard Model."""
-from datetime import (
-    date as dateType,
-)
-from typing import Literal, Optional
+"""Short Term Interest Rates Standard Model."""
+
+from datetime import date as dateType
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class EuropeanCentralBankInterestRatesParams(QueryParams):
-    """European Central Bank Interest Rates Query."""
+class STIRQueryParams(QueryParams):
+    """Short Term Interest Rates Query."""
 
     start_date: Optional[dateType] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("start_date", ""),
+        default=None, description=QUERY_DESCRIPTIONS.get("start_date")
     )
     end_date: Optional[dateType] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("end_date", ""),
-    )
-    interest_rate_type: Literal["deposit", "lending", "refinancing"] = Field(
-        default="lending",
-        description="The type of interest rate.",
+        default=None, description=QUERY_DESCRIPTIONS.get("end_date")
     )
 
 
-class EuropeanCentralBankInterestRatesData(Data):
-    """European Central Bank Interest Rates Data."""
+class STIRData(Data):
+    """Short Term Interest Rates Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    rate: Optional[float] = Field(description="European Central Bank Interest Rate.")
+    date: Optional[dateType] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("date")
+    )
+    value: Optional[float] = Field(
+        default=None,
+        description="Interest rate (given as a whole number, i.e 10=10%)",
+    )
+    country: Optional[str] = Field(
+        default=None,
+        description="Country for which interest rate is given",
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Economic Calendar Standard Model."""
 
-
 from datetime import (
     date as dateType,
     datetime,
 )
-from typing import Literal, Optional, Union
+from typing import Optional, Union
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
@@ -33,34 +32,30 @@
 class EconomicCalendarData(Data):
     """Economic Calendar Data."""
 
     date: Optional[datetime] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("date", "")
     )
     country: Optional[str] = Field(default=None, description="Country of event.")
+    category: Optional[str] = Field(default=None, description="Category of event.")
     event: Optional[str] = Field(default=None, description="Event name.")
-    reference: Optional[str] = Field(
-        default=None,
-        description="Abbreviated period for which released data refers to.",
+    importance: Optional[str] = Field(
+        default=None, description="The importance level for the event."
     )
     source: Optional[str] = Field(default=None, description="Source of the data.")
-    sourceurl: Optional[str] = Field(default=None, description="Source URL.")
-    actual: Optional[Union[str, float]] = Field(
-        default=None, description="Latest released value."
+    currency: Optional[str] = Field(default=None, description="Currency of the data.")
+    unit: Optional[str] = Field(default=None, description="Unit of the data.")
+    consensus: Optional[Union[str, float]] = Field(
+        default=None,
+        description="Average forecast among a representative group of economists.",
     )
     previous: Optional[Union[str, float]] = Field(
         default=None,
         description="Value for the previous period after the revision (if revision is applicable).",
     )
-    consensus: Optional[Union[str, float]] = Field(
+    revised: Optional[Union[str, float]] = Field(
         default=None,
-        description="Average forecast among a representative group of economists.",
-    )
-    forecast: Optional[Union[str, float]] = Field(
-        default=None, description="Trading Economics projections"
+        description="Revised previous value, if applicable.",
     )
-    url: Optional[str] = Field(default=None, description="Trading Economics URL")
-    importance: Optional[Union[Literal[0, 1, 2, 3], str]] = Field(
-        default=None, description="Importance of the event. 1-Low, 2-Medium, 3-High"
+    actual: Optional[Union[str, float]] = Field(
+        default=None, description="Latest released value."
     )
-    currency: Optional[str] = Field(default=None, description="Currency of the data.")
-    unit: Optional[str] = Field(default=None, description="Unit of the data.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 class EquityFtdQueryParams(QueryParams):
     """Equity FTD Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: str):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: str):
+        """Convert field to uppercase."""
         return v.upper()
 
 
 class EquityFtdData(Data):
     """Equity FTD Data."""
 
     settlement_date: Optional[dateType] = Field(
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_historical.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_historical.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-"""Equity Historical Price Standard Model."""
-
+"""ETF Historical Price Standard Model."""
 
 from datetime import (
     date as dateType,
     datetime,
 )
-from typing import List, Optional, Set, Union
+from typing import Optional, Union
 
 from dateutil import parser
-from pydantic import Field, PositiveFloat, field_validator
+from pydantic import Field, NonNegativeInt, PositiveFloat, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class EquityHistoricalQueryParams(QueryParams):
-    """Equity Historical Price Query."""
+class EtfHistoricalQueryParams(QueryParams):
+    """ETF Historical Price Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    interval: Optional[str] = Field(
-        default="1d",
-        description=QUERY_DESCRIPTIONS.get("interval", ""),
-    )
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", "") + " (ETF)")
     start_date: Optional[dateType] = Field(
         default=None,
         description=QUERY_DESCRIPTIONS.get("start_date", ""),
     )
     end_date: Optional[dateType] = Field(
         default=None,
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase and remove '-'."""
+        return v.upper()
 
 
-class EquityHistoricalData(Data):
-    """Equity Historical Price Data."""
+class EtfHistoricalData(Data):
+    """ETF Historical Price Data."""
 
-    date: datetime = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    date: Union[dateType, datetime] = Field(
+        description=DATA_DESCRIPTIONS.get("date", "")
+    )
     open: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("open", ""))
     high: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("high", ""))
     low: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("low", ""))
     close: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("close", ""))
-    volume: Union[float, int] = Field(description=DATA_DESCRIPTIONS.get("volume", ""))
-    vwap: Optional[PositiveFloat] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("vwap", "")
+    volume: Optional[NonNegativeInt] = Field(
+        description=DATA_DESCRIPTIONS.get("volume", "")
     )
 
     @field_validator("date", mode="before", check_fields=False)
     def date_validate(cls, v):  # pylint: disable=E0213
         """Return formatted datetime."""
-        return parser.isoparse(str(v))
+        if ":" in str(v):
+            return parser.isoparse(str(v))
+        return parser.parse(str(v)).date()
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
     symbol: str = Field(
         description=QUERY_DESCRIPTIONS.get("symbol", ""),
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: str):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: str):
+        """Convert field to uppercase."""
         return v.upper()
 
 
 class EquityNBBOData(Data):
     """Equity NBBO Data."""
 
     ask_exchange: str = Field(
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Equity Ownership Standard Model."""
 
-
 from datetime import date as dateType
-from typing import List, Optional, Set, Union
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
@@ -30,19 +29,17 @@
     def time_validate(cls, v: str):
         """Validate the date."""
         if v is None:
             v = dateType.today()
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class EquityOwnershipData(Data):
     """Equity Ownership Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     cik: int = Field(description=DATA_DESCRIPTIONS.get("cik", ""))
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_peers.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_peers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Equity Peers Standard Model."""
 
-from typing import List, Set, Union
+from typing import List
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
@@ -12,19 +12,17 @@
 class EquityPeersQueryParams(QueryParams):
     """Equity Peers Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class EquityPeersData(Data):
     """Equity Peers Data."""
 
     peers_list: List[str] = Field(
         default_factory=list,
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_performance.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/index_search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,23 @@
-"""Equity Performance Standard Model."""
+"""Index Search Standard Model."""
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 
 
-class EquityPerformanceQueryParams(QueryParams):
-    """Equity Performance Query."""
+class IndexSearchQueryParams(QueryParams):
+    """Index Search Query."""
 
-    sort: str = Field(
-        default="desc",
-        description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'.",
+    query: str = Field(description="Search query.", default="")
+    is_symbol: bool = Field(
+        description="Whether to search by ticker symbol.", default=False
     )
 
 
-class EquityPerformanceData(Data):
-    """Equity Performance Data."""
+class IndexSearchData(Data):
+    """Index Search Data."""
 
-    symbol: str = Field(
-        description=DATA_DESCRIPTIONS.get("symbol", ""),
-    )
-    name: str = Field(
-        description="Name of the entity.",
-    )
-    price: float = Field(
-        description="Last price.",
-    )
-    change: float = Field(
-        description="Change in price value.",
-    )
-    percent_change: float = Field(
-        description="Percent change.",
-    )
-    volume: float = Field(
-        description=DATA_DESCRIPTIONS.get("volume", ""),
-    )
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    name: str = Field(description="Name of the index.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_quote.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/index_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-"""Equity Quote Standard Model."""
+"""Index Info Standard Model."""
 
-from datetime import datetime
-from typing import List, Optional, Set, Union
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class EquityQuoteQueryParams(QueryParams):
-    """Equity Quote Query."""
+class IndexInfoQueryParams(QueryParams):
+    """Index Info Query."""
 
-    symbol: str = Field(
-        description=QUERY_DESCRIPTIONS.get("symbol", "")
-        + " In this case, the comma separated list of symbols."
-    )
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
-    @field_validator("symbol", mode="before", check_fields=False)
+    @field_validator("symbol")
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class EquityQuoteData(Data):
-    """Equity Quote Data."""
-
-    day_low: Optional[float] = Field(
-        default=None,
-        description="Lowest price of the stock in the current trading day.",
+class IndexInfoData(Data):
+    """Index Info Data."""
+
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    name: str = Field(description="The name of the index.")
+    description: Optional[str] = Field(
+        description="The short description of the index.", default=None
+    )
+    methodology: Optional[str] = Field(
+        description="URL to the methodology document.", default=None
     )
-    day_high: Optional[float] = Field(
-        default=None,
-        description="Highest price of the stock in the current trading day.",
+    factsheet: Optional[str] = Field(
+        description="URL to the factsheet document.", default=None
     )
-    date: Optional[datetime] = Field(
-        description=DATA_DESCRIPTIONS.get("date", ""), default=None
+    num_constituents: Optional[int] = Field(
+        description="The number of constituents in the index.", default=None
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_screener.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_screener.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,12 +17,12 @@
     """Equity Screener Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     name: str = Field(description="Name of the company.")
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_search.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_search.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,20 @@
 class EquitySearchQueryParams(QueryParams):
     """Equity Search Query."""
 
     query: str = Field(description="Search query.", default="")
     is_symbol: bool = Field(
         description="Whether to search by ticker symbol.", default=False
     )
+    use_cache: Optional[bool] = Field(
+        default=True,
+        description="Whether to use the cache or not.",
+    )
 
 
 class EquitySearchData(Data):
     """Equity Search Data."""
 
     symbol: Optional[str] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
     )
-    name: str = Field(description="Name of the company.")
+    name: Optional[str] = Field(default=None, description="Name of the company.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Equity Short Interest Standard Model."""
 
-
 from datetime import date as dateType
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
@@ -12,18 +11,15 @@
     QUERY_DESCRIPTIONS,
 )
 
 
 class ShortInterestQueryParams(QueryParams):
     """Equity Short Interest Query."""
 
-    symbol: str = Field(
-        description=QUERY_DESCRIPTIONS.get("symbol", ""),
-        default=None,
-    )
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
 
 class ShortInterestData(Data):
     """Equity Short Interest Data."""
 
     settlement_date: dateType = Field(
         description=(
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Equity Valuation Multiples Standard Model."""
 
-from typing import List, Optional, Set, Union
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
@@ -15,19 +15,17 @@
 class EquityValuationMultiplesQueryParams(QueryParams):
     """Equity Valuation Multiples Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class EquityValuationMultiplesData(Data):
     """Equity Valuation Multiples Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     revenue_per_share_ttm: Optional[float] = Field(
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ESG Risk Rating Standard Model."""
 
-
 from typing import List, Literal, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
@@ -16,19 +15,17 @@
 class ESGRiskRatingQueryParams(QueryParams):
     """ESG Risk Rating Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class ESGRiskRatingData(Data):
     """ESG Risk Rating Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     cik: str = Field(description=DATA_DESCRIPTIONS.get("cik", ""))
@@ -38,12 +35,12 @@
     esg_risk_rating: Literal[
         "A+", "A", "A-", "B+", "B", "B-", "C+", "C", "C-", "D+", "D", "D-", "F"
     ] = Field(description="ESG risk rating of the company.")
     industry_rank: str = Field(description="Industry rank of the company.")
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/esg_score.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/esg_score.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ESG Score Standard Model."""
 
-
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import List, Set, Union
 
 from pydantic import Field, field_validator
@@ -20,19 +19,17 @@
 class ESGScoreQueryParams(QueryParams):
     """ESG Score Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class ESGScoreData(Data):
     """ESG Score Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     cik: str = Field(description=DATA_DESCRIPTIONS.get("cik", ""))
@@ -46,12 +43,12 @@
     social_score: float = Field(description="Social score of the company.")
     governance_score: float = Field(description="Governance score of the company.")
     esg_score: float = Field(description="ESG score of the company.")
     url: str = Field(description="URL of the company.")
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/esg_sector.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/esg_sector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ESG Sector Standard Model."""
 
-
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 
 
 class ESGSectorQueryParams(QueryParams):
     """ESG Sector Query.
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/estr_rates.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/estr_rates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ESTR Standard Model."""
 
-
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/etf_countries.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_countries.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """ETF Countries Standard Model."""
 
-from typing import List, Set, Union
-
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
 
 class EtfCountriesQueryParams(QueryParams):
     """ETF Countries Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", "") + " (ETF)")
 
     @field_validator("symbol")
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class EtfCountriesData(Data):
     """ETF Countries Data."""
 
     country: str = Field(
         description="The country of the exposure.  Corresponding values are normalized percentage points."
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/etf_historical.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/futures_historical.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-"""ETF Historical Price Standard Model."""
+"""Futures Historical Price Standard Model."""
 
-from datetime import date as dateType
-from typing import List, Optional, Set, Union
+from datetime import date, datetime
+from typing import Optional
 
 from dateutil import parser
-from pydantic import Field, NonNegativeInt, PositiveFloat, field_validator
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class EtfHistoricalQueryParams(QueryParams):
-    """ETF Historical Price Query."""
+class FuturesHistoricalQueryParams(QueryParams):
+    """Futures Historical Price Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", "") + " (ETF)")
-    start_date: Optional[dateType] = Field(
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    start_date: Optional[date] = Field(
         default=None,
         description=QUERY_DESCRIPTIONS.get("start_date", ""),
     )
-    end_date: Optional[dateType] = Field(
+    end_date: Optional[date] = Field(
         default=None,
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
+    expiration: Optional[str] = Field(
+        default=None,
+        description="Future expiry date with format YYYY-MM",
+    )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def validate_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase and remove '-'."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
-
-
-class EtfHistoricalData(Data):
-    """ETF Historical Price Data."""
-
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    open: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("open", ""))
-    high: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("high", ""))
-    low: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("low", ""))
-    close: PositiveFloat = Field(description=DATA_DESCRIPTIONS.get("close", ""))
-    volume: Optional[NonNegativeInt] = Field(
-        description=DATA_DESCRIPTIONS.get("volume", "")
-    )
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
+
 
-    @field_validator("date", mode="before", check_fields=False)
-    def date_validate(cls, v):  # pylint: disable=E0213
+class FuturesHistoricalData(Data):
+    """Futures Historical Price Data."""
+
+    date: datetime = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    open: float = Field(description=DATA_DESCRIPTIONS.get("open", ""))
+    high: float = Field(description=DATA_DESCRIPTIONS.get("high", ""))
+    low: float = Field(description=DATA_DESCRIPTIONS.get("low", ""))
+    close: float = Field(description=DATA_DESCRIPTIONS.get("close", ""))
+    volume: float = Field(description=DATA_DESCRIPTIONS.get("volume", ""))
+
+    @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
+    def date_validate(cls, v):
         """Return formatted datetime."""
         return parser.isoparse(str(v))
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """ETF Historical NAV model."""
 
 from datetime import date as dateType
-from typing import List, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
@@ -16,19 +15,17 @@
 class EtfHistoricalNavQueryParams(QueryParams):
     """ETF Historical NAV Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol")
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class EtfHistoricalNavData(Data):
     """ETF Historical NAV Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     nav: float = Field(description="The net asset value on the date.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,22 @@
-"""ETF Holdings Standard Model."""
+"""ETF Search Standard Model."""
 
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
-    QUERY_DESCRIPTIONS,
-)
+from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 
 
-class EtfHoldingsQueryParams(QueryParams):
-    """ETF Holdings Query."""
+class EtfSearchQueryParams(QueryParams):
+    """ETF Search Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", "") + " (ETF)")
+    query: Optional[str] = Field(description="Search query.", default="")
 
 
-class EtfHoldingsData(Data):
-    """ETF Holdings Data."""
+class EtfSearchData(Data):
+    """ETF Search Data."""
 
-    symbol: Optional[str] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("symbol", "") + " (ETF)"
-    )
-    name: Optional[str] = Field(
-        default=None,
-        description="Name of the ETF holding.",
-    )
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", "") + "(ETF)")
+    name: Optional[str] = Field(description="Name of the ETF.", default=None)
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/etf_info.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-"""ETF Info Standard Model."""
+"""ETF Sectors Standard Model."""
 
-from typing import List, Optional, Set, Union
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
-    QUERY_DESCRIPTIONS,
-)
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
 
-class EtfInfoQueryParams(QueryParams):
-    """ETF Info Query."""
+class EtfSectorsQueryParams(QueryParams):
+    """ETF Sectors Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", "") + " (ETF)")
 
     @field_validator("symbol")
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class EtfInfoData(Data):
-    """ETF Info Data."""
-
-    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", "") + " (ETF)")
-    name: Optional[str] = Field(description="Name of the ETF.")
-    inception_date: Optional[str] = Field(description="Inception date of the ETF.")
+class EtfSectorsData(Data):
+    """ETF Sectors Data."""
+
+    sector: str = Field(description="Sector of exposure.")
+    weight: Optional[float] = Field(
+        description="Exposure of the ETF to the sector in normalized percentage points."
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/etf_performance.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/cp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-"""ETF Performance Standard Model."""
-from datetime import date as dateType
+"""Commercial Paper Standard Model."""
 
-from pydantic import Field
+from datetime import (
+    date as dateType,
+)
+from typing import Literal, Optional
+
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class ETFPerformanceQueryParams(QueryParams):
-    """ETF Performance Query."""
-
-    sort: str = Field(
-        default="desc",
-        description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'.",
-    )
-    limit: int = Field(
-        default=10,
-        description=QUERY_DESCRIPTIONS.get("limit", ""),
-    )
-
-
-class ETFPerformanceData(Data):
-    """ETF Performance Data."""
+class CommercialPaperParams(QueryParams):
+    """Commercial Paper Query."""
 
-    symbol: str = Field(
-        description=DATA_DESCRIPTIONS.get("symbol", ""),
+    start_date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("start_date", ""),
     )
-    name: str = Field(
-        description="Name of the entity.",
+    end_date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
-    last_price: float = Field(
-        description="Last price.",
+    maturity: Literal["overnight", "7d", "15d", "30d", "60d", "90d"] = Field(
+        default="30d",
+        description="The maturity.",
     )
-    percent_change: float = Field(
-        description="Percent change.",
+    category: Literal["asset_backed", "financial", "nonfinancial"] = Field(
+        default="financial",
+        description="The category.",
     )
-    net_change: float = Field(
-        description="Net change.",
-    )
-    volume: float = Field(
-        description=DATA_DESCRIPTIONS.get("volume", ""),
-    )
-    date: dateType = Field(
-        description=DATA_DESCRIPTIONS.get("date", ""),
+    grade: Literal["aa", "a2_p2"] = Field(
+        default="aa",
+        description="The grade.",
     )
+
+    @field_validator("maturity", "category", "grade", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
+
+class CommercialPaperData(Data):
+    """Commercial Paper Data."""
+
+    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    rate: Optional[float] = Field(description="Commercial Paper Rate.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/cik_map.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""ETF Sectors Standard Model."""
+"""Cik Map Standard Model."""
 
-from typing import List, Optional, Set, Union
+from typing import Optional, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.descriptions import (
+    DATA_DESCRIPTIONS,
+    QUERY_DESCRIPTIONS,
+)
 
 
-class EtfSectorsQueryParams(QueryParams):
-    """ETF Sectors Query."""
+class CikMapQueryParams(QueryParams):
+    """CikMap Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", "") + " (ETF)")
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
-    @field_validator("symbol")
+    @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class EtfSectorsData(Data):
-    """ETF Sectors Data."""
-
-    sector: str = Field(description="Sector of exposure.")
-    weight: Optional[float] = Field(
-        description="Exposure of the ETF to the sector in normalized percentage points."
+class CikMapData(Data):
+    """CikMap Data."""
+
+    cik: Optional[Union[str, int]] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("cik", "")
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """Euro Area Yield Curve Standard Model."""
 
-
 from datetime import date as dateType
-from typing import Literal, Optional
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
 
 class EUYieldCurveQueryParams(QueryParams):
     """Euro Area Yield Curve Query."""
 
     date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("date", "")
     )
-    yield_curve_type: Literal[
-        "spot_rate", "instantaneous_forward", "par_yield"
-    ] = Field(
-        default="spot_rate",
-        description="The yield curve type.",
-    )
 
 
 class EUYieldCurveData(Data):
     """Euro Area Yield Curve Data."""
 
-    maturity: str = Field(description="Yield curve rate maturity.")
-    rate: Optional[float] = Field(description="Yield curve rate.", default=None)
+    maturity: Optional[float] = Field(description="Maturity, in years.", default=None)
+    rate: Optional[float] = Field(
+        description="Yield curve rate, as a normalized percent.",
+        default=None,
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/european_index_constituents.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,39 @@
-"""European Index Constituents Standard Model."""
+"""Historical Dividends Standard Model."""
 
-
-from typing import List, Set, Union
+from datetime import date as dateType
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class EuropeanIndexConstituentsQueryParams(QueryParams):
-    """European Index Constituents Query."""
+class HistoricalDividendsQueryParams(QueryParams):
+    """Historical Dividends Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    start_date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("start_date", "")
+    )
+    end_date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("end_date", "")
+    )
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    @classmethod
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class EuropeanIndexConstituentsData(Data):
-    """European Index Constituents Data."""
-
-    symbol: str = Field(
-        description=DATA_DESCRIPTIONS.get("symbol", "")
-        + " The symbol is the constituent company in the index."
-    )
-    price: float = Field(
-        description="Current price of the constituent company in the index."
-    )
-    open: float = Field(description=DATA_DESCRIPTIONS.get("open", ""))
-    high: float = Field(description=DATA_DESCRIPTIONS.get("high", ""))
-    low: float = Field(description=DATA_DESCRIPTIONS.get("low", ""))
-    close: float = Field(description=DATA_DESCRIPTIONS.get("close", ""))
-    volume: float = Field(description=DATA_DESCRIPTIONS.get("volume", ""))
+class HistoricalDividendsData(Data):
+    """Historical Dividends Data."""
 
-    @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    ex_dividend_date: dateType = Field(
+        description="The ex-dividend date - the date on which the stock begins trading without rights to the dividend."
+    )
+    amount: float = Field(description="The dividend amount per share.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/european_indices.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_performance.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,58 @@
-"""European Indices Standard Model."""
+"""ETF Performance Standard Model."""
 
-
-from datetime import (
-    date as dateType,
-    datetime,
-)
-from typing import List, Optional, Set, Union
+from datetime import date as dateType
+from typing import Literal, Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class EuropeanIndicesQueryParams(QueryParams):
-    """European Indices Query."""
+class ETFPerformanceQueryParams(QueryParams):
+    """ETF Performance Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    start_date: Optional[dateType] = Field(
-        description=QUERY_DESCRIPTIONS.get("start_date", ""), default=None
+    sort: Literal["asc", "desc"] = Field(
+        default="desc",
+        description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'.",
     )
-    end_date: Optional[dateType] = Field(
-        description=QUERY_DESCRIPTIONS.get("end_date", ""), default=None
+    limit: int = Field(
+        default=10,
+        description=QUERY_DESCRIPTIONS.get("limit", ""),
     )
 
-    @field_validator("symbol", mode="before", check_fields=False)
+    @field_validator("sort", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
 
 
-class EuropeanIndicesData(Data):
-    """European Indices Data."""
+class ETFPerformanceData(Data):
+    """ETF Performance Data."""
 
-    date: datetime = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    close: float = Field(description=DATA_DESCRIPTIONS.get("close", ""))
+    symbol: str = Field(
+        description=DATA_DESCRIPTIONS.get("symbol", ""),
+    )
+    name: str = Field(
+        description="Name of the entity.",
+    )
+    last_price: float = Field(
+        description="Last price.",
+    )
+    percent_change: float = Field(
+        description="Percent change.",
+    )
+    net_change: float = Field(
+        description="Net change.",
+    )
+    volume: float = Field(
+        description=DATA_DESCRIPTIONS.get("volume", ""),
+    )
+    date: dateType = Field(
+        description=DATA_DESCRIPTIONS.get("date", ""),
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_historical.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,66 @@
-"""Executive Compensation Standard Model."""
-
+"""Equity Historical Price Standard Model."""
 
 from datetime import (
     date as dateType,
     datetime,
 )
-from typing import List, Optional, Set, Union
+from typing import Optional, Union
 
-from pydantic import Field, NonNegativeFloat, field_validator
+from dateutil import parser
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class ExecutiveCompensationQueryParams(QueryParams):
-    """Executive Compensation Query."""
+class EquityHistoricalQueryParams(QueryParams):
+    """Equity Historical Price Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    interval: Optional[str] = Field(
+        default="1d",
+        description=QUERY_DESCRIPTIONS.get("interval", ""),
+    )
+    start_date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("start_date", ""),
+    )
+    end_date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("end_date", ""),
+    )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class ExecutiveCompensationData(Data):
-    """Executive Compensation Data."""
+class EquityHistoricalData(Data):
+    """Equity Historical Price Data."""
 
-    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
-    cik: Optional[str] = Field(
-        default=None,
-        description=DATA_DESCRIPTIONS.get("cik", ""),
+    date: Union[dateType, datetime] = Field(
+        description=DATA_DESCRIPTIONS.get("date", "")
     )
-    filing_date: dateType = Field(description="Date of the filing.")
-    accepted_date: datetime = Field(description="Date the filing was accepted.")
-    name_and_position: str = Field(description="Name and position of the executive.")
-    year: int = Field(description="Year of the compensation.")
-    salary: NonNegativeFloat = Field(description="Salary of the executive.")
-    bonus: NonNegativeFloat = Field(description="Bonus of the executive.")
-    stock_award: NonNegativeFloat = Field(description="Stock award of the executive.")
-    incentive_plan_compensation: NonNegativeFloat = Field(
-        description="Incentive plan compensation of the executive."
+    open: float = Field(description=DATA_DESCRIPTIONS.get("open", ""))
+    high: float = Field(description=DATA_DESCRIPTIONS.get("high", ""))
+    low: float = Field(description=DATA_DESCRIPTIONS.get("low", ""))
+    close: float = Field(description=DATA_DESCRIPTIONS.get("close", ""))
+    volume: Optional[Union[float, int]] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("volume", "")
     )
-    all_other_compensation: NonNegativeFloat = Field(
-        description="All other compensation of the executive."
+    vwap: Optional[float] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("vwap", "")
     )
-    total: NonNegativeFloat = Field(description="Total compensation of the executive.")
-    url: str = Field(description="URL of the filing data.")
 
-    @field_validator("symbol", mode="before", check_fields=False)
-    @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    @field_validator("date", mode="before", check_fields=False)
+    def date_validate(cls, v):  # pylint: disable=E0213
+        """Return formatted datetime."""
+        if ":" in str(v):
+            return parser.isoparse(str(v))
+        return parser.parse(str(v)).date()
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/fed_projections.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/fed_projections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """PROJECTION Standard Model."""
 
-
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/fed_rates.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/fed_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """FED Standard Model."""
 
-
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/ffrmc.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/ffrmc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Selected Treasury Constant Maturity Standard Model."""
+
 from datetime import (
     date as dateType,
 )
 from typing import Literal, Optional
 
-from pydantic import Field
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
@@ -26,14 +27,20 @@
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
     maturity: Optional[Literal["10y", "5y", "1y", "6m", "3m"]] = Field(
         default="10y",
         description="The maturity",
     )
 
+    @field_validator("maturity", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
 
 class SelectedTreasuryConstantMaturityData(Data):
     """Selected Treasury Constant Maturity Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     rate: Optional[float] = Field(
         description="Selected Treasury Constant Maturity Rate."
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/unemployment.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-"""Financial Attributes Standard Model."""
+"""Unemployment Standard Model."""
 
 from datetime import date as dateType
-from typing import Literal, Optional
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class FinancialAttributesQueryParams(QueryParams):
-    """Financial Attributes Query."""
+class UnemploymentQueryParams(QueryParams):
+    """Unemployment Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol"))
-    tag: str = Field(description=QUERY_DESCRIPTIONS.get("tag"))
-    period: Optional[Literal["annual", "quarter"]] = Field(
-        default="annual", description=QUERY_DESCRIPTIONS.get("period")
-    )
-    limit: Optional[int] = Field(
-        default=1000, description=QUERY_DESCRIPTIONS.get("limit")
-    )
-    type: Optional[str] = Field(
-        default=None, description="Filter by type, when applicable."
-    )
     start_date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("start_date")
     )
     end_date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("end_date")
     )
-    sort: Optional[Literal["asc", "desc"]] = Field(
-        default="desc", description="Sort order."
-    )
 
 
-class FinancialAttributesData(Data):
-    """Financial Attributes Data."""
+class UnemploymentData(Data):
+    """Unemployment Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date"))
-    value: Optional[float] = Field(default=None, description="The value of the data.")
+    date: Optional[dateType] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("date")
+    )
+    value: Optional[float] = Field(
+        default=None,
+        description="Unemployment rate (given as a whole number, i.e 10=10%)",
+    )
+    country: Optional[str] = Field(
+        default=None,
+        description="Country for which unemployment rate is given",
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/fred_search.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/fred_series.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-"""FRED Series Standard Model."""
-
+"""Long Term Interest Rates Standard Model."""
 
 from datetime import date as dateType
-from typing import List, Optional, Set, Union
+from typing import Optional
 
-from pydantic import Field, field_validator
+from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class SeriesQueryParams(QueryParams):
-    """FRED Series Query."""
+class LTIRQueryParams(QueryParams):
+    """Long Term Interest Rates Query."""
 
-    symbol: str = Field(
-        description=QUERY_DESCRIPTIONS.get("symbol", ""),
-    )
     start_date: Optional[dateType] = Field(
-        description=QUERY_DESCRIPTIONS.get("start_date", ""), default=None
+        default=None, description=QUERY_DESCRIPTIONS.get("start_date")
     )
     end_date: Optional[dateType] = Field(
-        description=QUERY_DESCRIPTIONS.get("end_date", ""), default=None
+        default=None, description=QUERY_DESCRIPTIONS.get("end_date")
     )
-    limit: Optional[int] = Field(
-        description=QUERY_DESCRIPTIONS.get("limit", ""), default=100000
-    )
-
-    @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
 
 
-class SeriesData(Data):
-    """FRED Series Data."""
+class LTIRData(Data):
+    """Long Term Interest Rates Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    date: Optional[dateType] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("date")
+    )
+    value: Optional[float] = Field(
+        default=None,
+        description="Interest rate (given as a whole number, i.e 10=10%)",
+    )
+    country: Optional[str] = Field(
+        default=None,
+        description="Country for which interest rate is given",
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/futures_curve.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/options_unusual.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-"""Futures Curve Standard Model."""
+"""Unusual Options Standard Model."""
 
-
-from datetime import date as dateType
-from typing import List, Optional, Set, Union
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class FuturesCurveQueryParams(QueryParams):
-    """Futures Curve Query."""
+class OptionsUnusualQueryParams(QueryParams):
+    """Unusual Options Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    date: Optional[dateType] = Field(
+    symbol: Optional[str] = Field(
         default=None,
-        description=QUERY_DESCRIPTIONS.get("date", ""),
+        description=QUERY_DESCRIPTIONS.get("symbol", "") + " (the underlying symbol)",
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    @classmethod
+    def to_upper(cls, v: str):
+        """Convert field to uppercase."""
+        return v.upper() if v else None
+
 
+class OptionsUnusualData(Data):
+    """Unusual Options Data."""
 
-class FuturesCurveData(Data):
-    """Futures Curve Data."""
-
-    expiration: str = Field(description="Futures expiration month.")
-    price: Optional[float] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("close", "")
+    underlying_symbol: Optional[str] = Field(
+        description=DATA_DESCRIPTIONS.get("symbol", "") + " (the underlying symbol)",
+        default=None,
     )
+    contract_symbol: str = Field(description="Contract symbol for the option.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/futures_historical.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/index_historical.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,76 @@
-"""Futures Historical Price Standard Model."""
+"""Index Historical Standard Model."""
 
-
-from datetime import date, datetime
-from typing import List, Optional, Set, Union
+from datetime import (
+    date as dateType,
+    datetime,
+)
+from typing import Optional, Union
 
 from dateutil import parser
-from pydantic import Field, field_validator
+from pydantic import Field, StrictFloat, field_validator
 
-from openbb_core.provider.abstract.data import Data
+from openbb_core.provider.abstract.data import Data, ForceInt
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class FuturesHistoricalQueryParams(QueryParams):
-    """Futures Historical Price Query."""
+class IndexHistoricalQueryParams(QueryParams):
+    """Index Historical Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    start_date: Optional[date] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("start_date", ""),
-    )
-    end_date: Optional[date] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("end_date", ""),
-    )
-    expiration: Optional[str] = Field(
-        default=None,
-        description="Future expiry date with format YYYY-MM",
+    start_date: Optional[dateType] = Field(
+        description=QUERY_DESCRIPTIONS.get("start_date", ""), default=None
+    )
+    end_date: Optional[dateType] = Field(
+        description=QUERY_DESCRIPTIONS.get("end_date", ""), default=None
+    )
+    interval: Optional[str] = Field(
+        default="1d",
+        description=QUERY_DESCRIPTIONS.get("interval", ""),
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
-
-
-class FuturesHistoricalData(Data):
-    """Futures Historical Price Data."""
-
-    date: datetime = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    open: float = Field(description=DATA_DESCRIPTIONS.get("open", ""))
-    high: float = Field(description=DATA_DESCRIPTIONS.get("high", ""))
-    low: float = Field(description=DATA_DESCRIPTIONS.get("low", ""))
-    close: float = Field(description=DATA_DESCRIPTIONS.get("close", ""))
-    volume: float = Field(description=DATA_DESCRIPTIONS.get("volume", ""))
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
-    @field_validator("symbol", mode="before", check_fields=False)
+    @field_validator("sort", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
+
+class IndexHistoricalData(Data):
+    """Index Historical Data."""
+
+    date: Union[dateType, datetime] = Field(
+        description=DATA_DESCRIPTIONS.get("date", "")
+    )
+    open: Optional[StrictFloat] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("open", "")
+    )
+    high: Optional[StrictFloat] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("high", "")
+    )
+    low: Optional[StrictFloat] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("low", "")
+    )
+    close: Optional[StrictFloat] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("close", "")
+    )
+    volume: Optional[ForceInt] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("volume", "")
+    )
+
+    @field_validator("date", mode="before", check_fields=False)
     @classmethod
     def date_validate(cls, v):
         """Return formatted datetime."""
-        return parser.isoparse(str(v))
+        if ":" in str(v):
+            return parser.isoparse(str(v))
+        return parser.parse(str(v)).date()
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Forecast GDP Standard Model."""
+
 from datetime import date as dateType
 from typing import Literal, Optional
 
-from pydantic import Field
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
@@ -27,14 +28,20 @@
         default=None, description=QUERY_DESCRIPTIONS.get("end_date")
     )
     type: Literal["nominal", "real"] = Field(
         default="real",
         description="Type of GDP to get forecast of. Either nominal or real.",
     )
 
+    @field_validator("period", "type", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
 
 class GdpForecastData(Data):
     """Forecast GDP Data."""
 
     date: Optional[dateType] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("date")
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-"""Nominal GDP Standard Model."""
-from datetime import date as dateType
+"""ICE BofA US Corporate Bond Indices Standard Model."""
+
+from datetime import (
+    date as dateType,
+)
 from typing import Literal, Optional
 
-from pydantic import Field
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class GdpNominalQueryParams(QueryParams):
-    """Nominal GDP Query."""
+class ICEBofAQueryParams(QueryParams):
+    """ICE BofA US Corporate Bond Indices Query."""
 
-    units: Literal["usd", "usd_cap"] = Field(
-        default="usd",
-        description=QUERY_DESCRIPTIONS.get("units", "")
-        + " Units to get nominal GDP in. Either usd or usd_cap indicating per capita.",
-    )
     start_date: Optional[dateType] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("start_date")
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("start_date", ""),
     )
     end_date: Optional[dateType] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("end_date")
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("end_date", ""),
+    )
+    index_type: Literal["yield", "yield_to_worst", "total_return", "spread"] = Field(
+        default="yield",
+        description="The type of series.",
     )
 
+    @field_validator("index_type", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
 
-class GdpNominalData(Data):
-    """Nominal GDP Data."""
 
-    date: Optional[dateType] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("date")
-    )
-    value: Optional[float] = Field(
-        default=None, description="Nominal GDP value on the date."
+class ICEBofAData(Data):
+    """ICE BofA US Corporate Bond Indices Data."""
+
+    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    rate: Optional[float] = Field(
+        description="ICE BofA US Corporate Bond Indices Rate."
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/gdp_real.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/gdp_real.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Real GDP Standard Model."""
+
 from datetime import date as dateType
 from typing import Literal, Optional
 
-from pydantic import Field
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
@@ -25,14 +26,20 @@
     start_date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("start_date")
     )
     end_date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("end_date")
     )
 
+    @field_validator("units", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
 
 class GdpRealData(Data):
     """Real GDP Data."""
 
     date: Optional[dateType] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("date")
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-"""Historical Attributes Standard Model."""
+"""Search Financial Attributes Standard Model."""
 
-from datetime import date as dateType
-from typing import Literal, Optional
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
-    QUERY_DESCRIPTIONS,
-)
-
-
-class HistoricalAttributesQueryParams(QueryParams):
-    """Historical Attributes Query."""
-
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol"))
-    tag: str = Field(description="Intrinio data tag ID or code.")
-    start_date: Optional[dateType] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("start_date")
-    )
-    end_date: Optional[dateType] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("end_date")
-    )
-    frequency: Optional[
-        Literal["daily", "weekly", "monthly", "quarterly", "yearly"]
-    ] = Field(default="yearly", description=QUERY_DESCRIPTIONS.get("frequency"))
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+
+
+class SearchFinancialAttributesQueryParams(QueryParams):
+    """Search Financial Attributes Query."""
+
+    query: str = Field(description="Query to search for.")
     limit: Optional[int] = Field(
         default=1000, description=QUERY_DESCRIPTIONS.get("limit")
     )
-    type: Optional[str] = Field(
-        default=None, description="Filter by type, when applicable."
-    )
-    sort: Optional[Literal["asc", "desc"]] = Field(
-        default="desc", description="Sort order."
-    )
 
 
-class HistoricalAttributesData(Data):
-    """Historical Attributes Data."""
+class SearchFinancialAttributesData(Data):
+    """Search Financial Attributes Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date"))
-    value: Optional[float] = Field(default=None, description="The value of the data.")
+    id: str = Field(description="ID of the financial attribute.")
+    name: str = Field(description="Name of the financial attribute.")
+    tag: str = Field(description="Tag of the financial attribute.")
+    statement_code: str = Field(description="Code of the financial statement.")
+    statement_type: Optional[str] = Field(
+        default=None, description="Type of the financial statement."
+    )
+    parent_name: Optional[str] = Field(
+        default=None, description="Parent's name of the financial attribute."
+    )
+    sequence: Optional[int] = Field(
+        default=None, description="Sequence of the financial statement."
+    )
+    factor: Optional[str] = Field(
+        default=None, description="Unit of the financial attribute."
+    )
+    transaction: Optional[str] = Field(
+        default=None,
+        description="Transaction type (credit/debit) of the financial attribute.",
+    )
+    type: Optional[str] = Field(
+        default=None, description="Type of the financial attribute."
+    )
+    unit: Optional[str] = Field(
+        default=None, description="Unit of the financial attribute."
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/historical_splits.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,43 @@
-"""Historical Dividends Standard Model."""
-
+"""Historical Splits Standard Model."""
 
 from datetime import date as dateType
-from typing import List, Set, Union
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class HistoricalDividendsQueryParams(QueryParams):
-    """Historical Dividends Query."""
+class HistoricalSplitsQueryParams(QueryParams):
+    """Historical Splits Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):  # pylint: disable=E0213
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    @classmethod
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class HistoricalDividendsData(Data):
-    """Historical Dividends Data."""
+class HistoricalSplitsData(Data):
+    """Historical Splits Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    dividend: float = Field(description="Dividend of the historical dividends.")
+    numerator: Optional[float] = Field(
+        default=None,
+        description="Numerator of the split.",
+    )
+    denominator: Optional[float] = Field(
+        default=None,
+        description="Denominator of the split.",
+    )
+    split_ratio: Optional[str] = Field(
+        default=None,
+        description="Split ratio.",
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/historical_employees.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/historical_employees.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 class HistoricalEmployeesQueryParams(QueryParams):
     """Historical Employees Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class HistoricalEmployeesData(Data):
     """Historical Employees Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     cik: int = Field(description=DATA_DESCRIPTIONS.get("cik", ""))
@@ -64,12 +62,12 @@
     @classmethod
     def filing_date_validate(cls, v):  # pylint: disable=E0213
         """Validate filing date."""
         return datetime.strptime(v, "%Y-%m-%d")
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/historical_eps.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/historical_eps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Historical EPS Standard Model."""
 
-
 from datetime import date as dateType
-from typing import List, Optional, Set, Union
+from typing import Optional
 
 from dateutil import parser
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
@@ -18,19 +17,17 @@
 class HistoricalEpsQueryParams(QueryParams):
     """Historical EPS Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class HistoricalEpsData(Data):
     """Historical EPS Data."""
 
     date: dateType = Field(default=None, description=DATA_DESCRIPTIONS.get("date", ""))
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/historical_splits.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,49 @@
-"""Historical Splits Standard Model."""
-
+"""Balance Sheet Standard Model."""
 
 from datetime import date as dateType
-from typing import List, Set, Union
+from typing import Optional
 
-from pydantic import Field, field_validator
+from pydantic import Field, NonNegativeInt, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class HistoricalSplitsQueryParams(QueryParams):
-    """Historical Splits Query."""
+class BalanceSheetQueryParams(QueryParams):
+    """Balance Sheet Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    period: str = Field(
+        default="annual",
+        description=QUERY_DESCRIPTIONS.get("period", ""),
+    )
+    limit: Optional[NonNegativeInt] = Field(
+        default=5, description=QUERY_DESCRIPTIONS.get("limit", "")
+    )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str):
+        """Convert field to uppercase."""
+        return v.upper()
 
+    @field_validator("period", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
 
-class HistoricalSplitsData(Data):
-    """Historical Splits Data."""
-
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    label: str = Field(description="Label of the historical stock splits.")
-    numerator: float = Field(description="Numerator of the historical stock splits.")
-    denominator: float = Field(
-        description="Denominator of the historical stock splits."
+
+class BalanceSheetData(Data):
+    """Balance Sheet Data."""
+
+    period_ending: dateType = Field(description="The end date of the reporting period.")
+    fiscal_period: Optional[str] = Field(
+        description="The fiscal period of the report.", default=None
+    )
+    fiscal_year: Optional[int] = Field(
+        description="The fiscal year of the fiscal period.", default=None
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/hqm.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/hqm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """High Quality Market Corporate Bond Standard Model."""
+
 from datetime import (
     date as dateType,
 )
 from typing import Literal, Optional
 
-from pydantic import Field
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
@@ -22,14 +23,20 @@
         description=QUERY_DESCRIPTIONS.get("date", ""),
     )
     yield_curve: Literal["spot", "par"] = Field(
         default="spot",
         description="The yield curve type.",
     )
 
+    @field_validator("yield_curve", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
 
 class HighQualityMarketCorporateBondData(Data):
     """High Quality Market Corporate Bond Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     rate: Optional[float] = Field(description="HighQualityMarketCorporateBond Rate.")
     maturity: str = Field(description="Maturity.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-"""ICE BofA US Corporate Bond Indices Standard Model."""
-from datetime import (
-    date as dateType,
-)
-from typing import Literal, Optional
+"""Composite Leading Indicator Standard Model."""
+
+from datetime import date as dateType
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class ICEBofAQueryParams(QueryParams):
-    """ICE BofA US Corporate Bond Indices Query."""
+class CLIQueryParams(QueryParams):
+    """Composite Leading Indicator Query."""
 
     start_date: Optional[dateType] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("start_date", ""),
+        default=None, description=QUERY_DESCRIPTIONS.get("start_date")
     )
     end_date: Optional[dateType] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("end_date", ""),
-    )
-    index_type: Literal["yield", "yield_to_worst", "total_return", "spread"] = Field(
-        default="yield",
-        description="The type of series.",
+        default=None, description=QUERY_DESCRIPTIONS.get("end_date")
     )
 
 
-class ICEBofAData(Data):
-    """ICE BofA US Corporate Bond Indices Data."""
+class CLIData(Data):
+    """Composite Leading Indicator Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    rate: Optional[float] = Field(
-        description="ICE BofA US Corporate Bond Indices Rate."
+    date: Optional[dateType] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("date")
+    )
+    value: Optional[float] = Field(default=None, description="CLI value")
+    country: Optional[str] = Field(
+        default=None,
+        description="Country for which CLI is given",
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/income_statement.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/equity_quote.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,156 +1,152 @@
-"""Income Statement Standard Model."""
+"""Equity Quote Standard Model."""
 
+from datetime import datetime
+from typing import List, Optional, Union
 
-from datetime import date as dateType
-from typing import List, Literal, Optional, Set, Union
-
-from pydantic import Field, NonNegativeInt, StrictFloat, field_validator
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class IncomeStatementQueryParams(QueryParams):
-    """Income Statement Query."""
+class EquityQuoteQueryParams(QueryParams):
+    """Equity Quote Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    period: Optional[Literal["annual", "quarter"]] = Field(
-        default="annual",
-        description=QUERY_DESCRIPTIONS.get("period", ""),
-    )
-    limit: Optional[NonNegativeInt] = Field(
-        default=5, description=QUERY_DESCRIPTIONS.get("limit", "")
-    )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        return v.split(",")[0].upper() if "," in v else v.upper()
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class IncomeStatementData(Data):
-    """Income Statement Data."""
+class EquityQuoteData(Data):
+    """Equity Quote Data."""
 
-    symbol: Optional[str] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
-    )
-    date: dateType = Field(
-        description=DATA_DESCRIPTIONS.get("date", "")
-        + " In this case, the date of the income statement."
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    asset_type: Optional[str] = Field(
+        default=None, description="Type of asset - i.e, stock, ETF, etc."
     )
-    period: Optional[str] = Field(
-        default=None, description="Period of the income statement."
+    name: Optional[str] = Field(
+        default=None, description="Name of the company or asset."
     )
-    cik: Optional[str] = Field(
+    exchange: Optional[str] = Field(
         default=None,
-        description=DATA_DESCRIPTIONS.get("cik", ""),
+        description="The name or symbol of the venue where the data is from.",
     )
-
-    revenue: Optional[StrictFloat] = Field(default=None, description="Revenue.")
-    cost_of_revenue: Optional[StrictFloat] = Field(
-        default=None, description="Cost of revenue."
+    bid: Optional[float] = Field(
+        default=None, description="Price of the top bid order."
     )
-    gross_profit: Optional[StrictFloat] = Field(
-        default=None, description="Gross profit."
+    bid_size: Optional[int] = Field(
+        default=None,
+        description="This represents the number of round lot orders at the given price."
+        + " The normal round lot size is 100 shares."
+        + " A size of 2 means there are 200 shares available at the given price.",
     )
-    cost_and_expenses: Optional[StrictFloat] = Field(
-        default=None, description="Cost and expenses."
+    bid_exchange: Optional[str] = Field(
+        default=None,
+        description="The specific trading venue where the purchase order was placed.",
     )
-    gross_profit_ratio: Optional[float] = Field(
-        default=None, description="Gross profit ratio."
+    ask: Optional[float] = Field(
+        default=None, description="Price of the top ask order."
     )
-
-    research_and_development_expenses: Optional[StrictFloat] = Field(
-        default=None, description="Research and development expenses."
+    ask_size: Optional[int] = Field(
+        default=None,
+        description="This represents the number of round lot orders at the given price."
+        + " The normal round lot size is 100 shares."
+        + " A size of 2 means there are 200 shares available at the given price.",
     )
-    general_and_administrative_expenses: Optional[StrictFloat] = Field(
-        default=None, description="General and administrative expenses."
+    ask_exchange: Optional[str] = Field(
+        default=None,
+        description="The specific trading venue where the sale order was placed.",
     )
-    selling_and_marketing_expenses: Optional[float] = Field(
-        default=None, description="Selling and marketing expenses."
+    quote_conditions: Optional[Union[str, int, List[str], List[int]]] = Field(
+        default=None,
+        description="Conditions or condition codes applicable to the quote.",
     )
-    selling_general_and_administrative_expenses: Optional[StrictFloat] = Field(
-        default=None, description="Selling, general and administrative expenses."
+    quote_indicators: Optional[Union[str, int, List[str], List[int]]] = Field(
+        default=None,
+        description="Indicators or indicator codes applicable to the participant"
+        + " quote related to the price bands for the issue, or the affect the quote has"
+        + " on the NBBO.",
     )
-    other_expenses: Optional[StrictFloat] = Field(
-        default=None, description="Other expenses."
+    sales_conditions: Optional[Union[str, int, List[str], List[int]]] = Field(
+        default=None,
+        description="Conditions or condition codes applicable to the sale.",
     )
-    operating_expenses: Optional[StrictFloat] = Field(
-        default=None, description="Operating expenses."
+    sequence_number: Optional[int] = Field(
+        default=None,
+        description="The sequence number represents the sequence in which message events happened."
+        + " These are increasing and unique per ticker symbol,"
+        + " but will not always be sequential (e.g., 1, 2, 6, 9, 10, 11).",
     )
-
-    depreciation_and_amortization: Optional[StrictFloat] = Field(
-        default=None, description="Depreciation and amortization."
+    market_center: Optional[str] = Field(
+        default=None,
+        description="The ID of the UTP participant that originated the message.",
     )
-    ebit: Optional[StrictFloat] = Field(
+    participant_timestamp: Optional[datetime] = Field(
         default=None,
-        description="Earnings before interest, and taxes.",
+        description="Timestamp for when the quote was generated by the exchange.",
     )
-    ebitda: Optional[StrictFloat] = Field(
+    trf_timestamp: Optional[datetime] = Field(
         default=None,
-        description="Earnings before interest, taxes, depreciation and amortization.",
+        description="Timestamp for when the TRF (Trade Reporting Facility) received the message.",
     )
-    ebitda_ratio: Optional[float] = Field(
+    sip_timestamp: Optional[datetime] = Field(
         default=None,
-        description="Earnings before interest, taxes, depreciation and amortization ratio.",
+        description="Timestamp for when the SIP (Security Information Processor)"
+        + " received the message from the exchange.",
     )
-    operating_income: Optional[StrictFloat] = Field(
-        default=None, description="Operating income."
+    last_price: Optional[float] = Field(
+        default=None, description="Price of the last trade."
     )
-    operating_income_ratio: Optional[float] = Field(
-        default=None, description="Operating income ratio."
+    last_tick: Optional[str] = Field(
+        default=None, description="Whether the last sale was an up or down tick."
     )
-
-    interest_income: Optional[StrictFloat] = Field(
-        default=None, description="Interest income."
+    last_size: Optional[int] = Field(
+        default=None, description="Size of the last trade."
     )
-    interest_expense: Optional[StrictFloat] = Field(
-        default=None, description="Interest expense."
+    last_timestamp: Optional[datetime] = Field(
+        default=None, description="Date and Time when the last price was recorded."
     )
-    total_other_income_expenses_net: Optional[StrictFloat] = Field(
-        default=None, description="Total other income expenses net."
+    open: Optional[float] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("open", "")
     )
-
-    income_before_tax: Optional[StrictFloat] = Field(
-        default=None, description="Income before tax."
+    high: Optional[float] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("high", "")
     )
-    income_before_tax_ratio: Optional[float] = Field(
-        default=None, description="Income before tax ratio."
+    low: Optional[float] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("low", "")
     )
-    income_tax_expense: Optional[StrictFloat] = Field(
-        default=None, description="Income tax expense."
+    close: Optional[float] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("close", "")
     )
-
-    net_income: Optional[StrictFloat] = Field(default=None, description="Net income.")
-    net_income_ratio: Optional[float] = Field(
-        default=None, description="Net income ratio."
+    volume: Optional[Union[int, float]] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("volume", "")
     )
-    eps: Optional[float] = Field(default=None, description="Earnings per share.")
-    eps_diluted: Optional[float] = Field(
-        default=None, description="Earnings per share diluted."
+    exchange_volume: Optional[Union[int, float]] = Field(
+        default=None,
+        description="Volume of shares exchanged during the trading day on the specific exchange.",
     )
-    weighted_average_shares_outstanding: Optional[StrictFloat] = Field(
-        default=None, description="Weighted average shares outstanding."
+    prev_close: Optional[float] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("prev_close", "")
     )
-    weighted_average_shares_outstanding_dil: Optional[StrictFloat] = Field(
-        default=None, description="Weighted average shares outstanding diluted."
+    change: Optional[float] = Field(
+        default=None, description="Change in price from previous close."
     )
-    link: Optional[str] = Field(
-        default=None, description="Link to the income statement."
+    change_percent: Optional[float] = Field(
+        default=None,
+        description="Change in price as a normalized percentage.",
+        json_schema_extra={"x-frontendmultiply": 100},
     )
-    final_link: Optional[str] = Field(
-        default=None, description="Final link to the income statement."
+    year_high: Optional[float] = Field(
+        default=None, description="The one year high (52W High)."
+    )
+    year_low: Optional[float] = Field(
+        default=None, description="The one year low (52W Low)."
     )
-
-    @field_validator("symbol", mode="before", check_fields=False)
-    @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)]) if v else None
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Income Statement Growth Standard Model."""
 
-
 from datetime import date as dateType
 from typing import List, Literal, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -21,19 +20,23 @@
     limit: int = Field(default=10, description=QUERY_DESCRIPTIONS.get("limit", ""))
     period: Literal["annual", "quarter"] = Field(
         default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
+
+    @field_validator("period", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
 
 
 class IncomeStatementGrowthData(Data):
     """Income Statement Growth Data."""
 
     symbol: Optional[str] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
@@ -109,12 +112,12 @@
     )
     growth_weighted_average_shs_out_dil: float = Field(
         description="Growth rate of diluted weighted average shares outstanding."
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)]) if v else None
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/index_constituents.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,43 @@
-"""Index Constituents Standard Model."""
+"""ETF Equity Exposure Standard Model."""
 
-
-from datetime import date
-from typing import List, Literal, Optional, Set, Union
+from typing import Optional, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
 
-class IndexConstituentsQueryParams(QueryParams):
-    """Index Constituents Query."""
+class EtfEquityExposureQueryParams(QueryParams):
+    """ETF Equity Exposure Query Params."""
 
-    index: Literal["nasdaq", "sp500", "dowjones"] = Field(
-        default="dowjones",
-        description="Index for which we want to fetch the constituents.",
-    )
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", "") + " (Stock)")
+
+    @field_validator("symbol")
+    @classmethod
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class IndexConstituentsData(Data):
-    """Index Constituents Data."""
+class EtfEquityExposureData(Data):
+    """ETF Equity Exposure Data."""
 
-    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
-    name: str = Field(description="Name of the constituent company in the index.")
-    sector: str = Field(
-        description="Sector the constituent company in the index belongs to."
+    equity_symbol: str = Field(description="The symbol of the equity requested.")
+    etf_symbol: str = Field(
+        description="The symbol of the ETF with exposure to the requested equity."
     )
-    sub_sector: Optional[str] = Field(
+    shares: Optional[float] = Field(
         default=None,
-        description="Sub-sector the constituent company in the index belongs to.",
+        description="The number of shares held in the ETF.",
     )
-    headquarter: Optional[str] = Field(
+    weight: Optional[float] = Field(
         default=None,
-        description="Location of the headquarter of the constituent company in the index.",
+        description="The weight of the equity in the ETF, as a normalized percent.",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
-    date_first_added: Optional[Union[date, str]] = Field(
-        default=None, description="Date the constituent company was added to the index."
-    )
-    cik: int = Field(
-        description=DATA_DESCRIPTIONS.get("cik", ""),
-    )
-    founded: Optional[Union[date, str]] = Field(
+    market_value: Optional[Union[int, float]] = Field(
         default=None,
-        description="Founding year of the constituent company in the index.",
+        description="The market value of the equity position in the ETF.",
     )
-
-    @field_validator("symbol", mode="before", check_fields=False)
-    @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/index_info.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/futures_curve.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,38 @@
-"""Index Info Standard Model."""
+"""Futures Curve Standard Model."""
 
-from typing import List, Optional, Set, Union
+from datetime import date as dateType
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class IndexInfoQueryParams(QueryParams):
-    """Index Info Query."""
+class FuturesCurveQueryParams(QueryParams):
+    """Futures Curve Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("date", ""),
+    )
 
-    @field_validator("symbol")
+    @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
-class IndexInfoData(Data):
-    """Index Info Data."""
-
-    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
-    name: str = Field(description="The name of the index.")
-    description: Optional[str] = Field(
-        description="The short description of the index.", default=None
-    )
-    methodology: Optional[str] = Field(
-        description="URL to the methodology document.", default=None
-    )
-    factsheet: Optional[str] = Field(
-        description="URL to the factsheet document.", default=None
-    )
-    num_constituents: Optional[int] = Field(
-        description="The number of constituents in the index.", default=None
+class FuturesCurveData(Data):
+    """Futures Curve Data."""
+
+    expiration: str = Field(description="Futures expiration month.")
+    price: Optional[float] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("close", "")
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/index_search.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/top_retail.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-"""Index Search Standard Model."""
+"""Top Retail Standard Model."""
+
+from datetime import date as DateType
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
+from openbb_core.provider.utils.descriptions import (
+    DATA_DESCRIPTIONS,
+    QUERY_DESCRIPTIONS,
+)
 
 
-class IndexSearchQueryParams(QueryParams):
-    """Index Search Query."""
+class TopRetailQueryParams(QueryParams):
+    """Top Retail Search Query."""
 
-    query: str = Field(description="Search query.", default="")
-    is_symbol: bool = Field(
-        description="Whether to search by ticker symbol.", default=False
-    )
+    limit: int = Field(description=QUERY_DESCRIPTIONS.get("limit", ""), default=5)
 
 
-class IndexSearchData(Data):
-    """Index Search Data."""
+class TopRetailData(Data):
+    """Top Retail Search Data."""
 
+    date: DateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
-    name: str = Field(description="Name of the index.")
+    activity: float = Field(description="Activity of the symbol.")
+    sentiment: float = Field(
+        description="Sentiment of the symbol. 1 is bullish, -1 is bearish."
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/index_sectors.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/index_sectors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Index Sectors Standard Model."""
 
-from typing import List, Set, Union
-
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
 
 class IndexSectorsQueryParams(QueryParams):
     """Index Sectors Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol")
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class IndexSectorsData(Data):
     """Index Sectors Data."""
 
     sector: str = Field(description="The sector name.")
     weight: float = Field(description="The weight of the sector in the index.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Index Snapshots Standard Model."""
 
-from typing import Literal, Optional
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 
 
 class IndexSnapshotsQueryParams(QueryParams):
     """Index Snapshots Query."""
 
-    region: Optional[Literal["US", "EU"]] = Field(
-        description="The region to return. Currently supports US and EU.", default="US"
+    region: str = Field(
+        default="us", description="The region of focus for the data - i.e., us, eu."
     )
 
 
 class IndexSnapshotsData(Data):
     """Index Snapshots Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
@@ -34,14 +34,20 @@
     )
     low: Optional[float] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("low", "")
     )
     close: Optional[float] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("close", "")
     )
+    volume: Optional[int] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("volume", "")
+    )
     prev_close: Optional[float] = Field(
-        default=None, description="Previous closing price of the index."
+        default=None, description=DATA_DESCRIPTIONS.get("prev_close", "")
+    )
+    change: Optional[float] = Field(
+        default=None, description="Change in value of the index."
     )
-    change: Optional[float] = Field(default=None, description="Change of the index.")
     change_percent: Optional[float] = Field(
-        default=None, description="Change percent of the index."
+        default=None,
+        description="Change, in normalized percentage points, of the index.",
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/industry_pe.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/insider_trading.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/insider_trading.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """Insider Trading Standard Model."""
 
-from datetime import date, datetime, time
-from typing import List, Optional, Set, Union
+from datetime import (
+    date as dateType,
+    datetime,
+    time,
+)
+from typing import Optional, Union
 
 from dateutil import parser
 from pydantic import Field, StrictInt, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
@@ -21,67 +25,70 @@
     limit: StrictInt = Field(
         default=500,
         description=QUERY_DESCRIPTIONS.get("limit", ""),
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class InsiderTradingData(Data):
     """Insider Trading Data."""
 
-    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
-    company_cik: int = Field(description="Company CIK of the insider trading.")
-    filing_date: datetime = Field(description="Filing date of the insider trading.")
-    transaction_date: Optional[date] = Field(
-        default=None, description="Transaction date of the insider trading."
+    symbol: Optional[str] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
+    )
+    company_cik: Optional[Union[int, str]] = Field(
+        default=None, description="CIK number of the company."
+    )
+    filing_date: Optional[Union[dateType, datetime]] = Field(
+        default=None, description="Filing date of the trade."
+    )
+    transaction_date: Optional[dateType] = Field(
+        default=None, description="Date of the transaction."
+    )
+    owner_cik: Optional[Union[int, str]] = Field(
+        default=None, description="Reporting individual's CIK."
+    )
+    owner_name: Optional[str] = Field(
+        default=None, description="Name of the reporting individual."
     )
-    owner_cik: int = Field(description="Reporting CIK of the insider trading.")
-    owner_name: str = Field(description="Reporting name of the insider trading.")
     owner_title: Optional[str] = Field(
-        default=None, description="Designation of owner of the insider trading."
+        default=None, description="The title held by the reporting individual."
     )
-    transaction_type: str = Field(
-        description="Transaction type of the insider trading."
+    transaction_type: Optional[str] = Field(
+        default=None, description="Type of transaction being reported."
     )
     acquisition_or_disposition: Optional[str] = Field(
-        default=None,
-        description="Acquisition or disposition of the insider trading.",
+        default=None, description="Acquisition or disposition of the shares."
     )
     security_type: Optional[str] = Field(
-        default=None, description="Security type of the insider trading."
+        default=None, description="The type of security transacted."
     )
     securities_owned: Optional[float] = Field(
-        default=None, description="Number of securities owned in the insider trading."
+        default=None,
+        description="Number of securities owned by the reporting individual.",
     )
     securities_transacted: Optional[float] = Field(
-        default=None, description="Securities transacted of the insider trading."
+        default=None,
+        description="Number of securities transacted by the reporting individual.",
     )
     transaction_price: Optional[float] = Field(
-        default=None,
-        description="Price of the insider trading.",
+        default=None, description="The price of the transaction."
     )
-    filing_url: str = Field(description="Link of the insider trading.")
+    filing_url: Optional[str] = Field(default=None, description="Link to the filing.")
 
-    @field_validator("symbol", mode="before", check_fields=False)
-    @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
-
-    @field_validator("filing_date", mode="before", check_fields=False)
+    @field_validator(
+        "filing_date", "transaction_date", mode="before", check_fields=False
+    )
     @classmethod
     def date_validate(cls, v):  # pylint: disable=E0213
         """Return formatted datetime."""
-        filing_date = parser.isoparse(str(v))
-
-        if filing_date.time() == time(0, 0):
-            return datetime.combine(filing_date.date(), time(0, 0, 0))
-        return filing_date
+        if v:
+            filing_date = parser.isoparse(str(v))
+            if filing_date.time() == time(0, 0):
+                return filing_date.date()
+            return filing_date
+        return None
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Institutional Ownership Standard Model."""
 
-
 from datetime import date as dateType
 from typing import List, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -17,31 +16,29 @@
 class InstitutionalOwnershipQueryParams(QueryParams):
     """Institutional Ownership Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class InstitutionalOwnershipData(Data):
     """Institutional Ownership Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     cik: Optional[str] = Field(
         default=None,
         description=DATA_DESCRIPTIONS.get("cik", ""),
     )
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/key_executives.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/key_executives.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Key Executives Standard Model."""
 
-from typing import List, Optional, Set, Union
+from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data, ForceInt
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
@@ -12,19 +12,17 @@
 class KeyExecutivesQueryParams(QueryParams):
     """Key Executives Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class KeyExecutivesData(Data):
     """Key Executives Data."""
 
     title: str = Field(description="Designation of the key executive.")
     name: str = Field(description="Name of the key executive.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/key_metrics.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-"""Key Metrics Standard Model."""
+"""Latest Attributes Standard Model."""
 
-from typing import List, Literal, Optional, Set, Union
+from typing import List, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class KeyMetricsQueryParams(QueryParams):
-    """Key Metrics Query."""
+class LatestAttributesQueryParams(QueryParams):
+    """Latest Attributes Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    period: Optional[Literal["annual", "quarter"]] = Field(
-        default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
-    )
-    limit: Optional[int] = Field(
-        default=100, description=QUERY_DESCRIPTIONS.get("limit", "")
-    )
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol"))
+    tag: str = Field(description="Intrinio data tag ID or code.")
 
-    @field_validator("symbol", mode="before", check_fields=False)
+    @field_validator("tag", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def multiple_tags(cls, v: Union[str, List[str], Set[str]]):
+        """Accept a comma-separated string or list of tags."""
         if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+            return v.lower()
+        return ",".join([tag.lower() for tag in list(v)])
 
+    @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
-class KeyMetricsData(Data):
-    """Key Metrics Data."""
 
-    symbol: Optional[str] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
-    )
-    market_cap: Optional[float] = Field(
-        default=None, description="Market capitalization"
+class LatestAttributesData(Data):
+    """Latest Attributes Data."""
+
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol"))
+    tag: Optional[str] = Field(
+        default=None, description="Tag name for the fetched data."
     )
-    pe_ratio: Optional[float] = Field(
-        default=None, description="Price-to-earnings ratio (P/E ratio)"
+    value: Optional[Union[str, float]] = Field(
+        default=None, description="The value of the data."
     )
-
-    @field_validator("symbol", mode="before", check_fields=False)
-    @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)]) if v else None
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-"""Latest Attributes Standard Model."""
+"""SOFR Standard Model."""
 
-from typing import Optional, Union
+from datetime import date as dateType
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.descriptions import (
+    DATA_DESCRIPTIONS,
+    QUERY_DESCRIPTIONS,
+)
 
 
-class LatestAttributesQueryParams(QueryParams):
-    """Latest Attributes Query."""
-
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol"))
-    tag: str = Field(description="Intrinio data tag ID or code.")
+class SOFRQueryParams(QueryParams):
+    """SOFR Query."""
+
+    start_date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("start_date", ""),
+    )
+    end_date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("end_date", ""),
+    )
 
 
-class LatestAttributesData(Data):
-    """Latest Attributes Data."""
+class SOFRData(Data):
+    """SOFR Data."""
 
-    value: Optional[Union[str, float]] = Field(
-        default=None, description="The value of the data."
-    )
+    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    rate: Optional[float] = Field(description="SOFR rate.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/market_indices.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/market_indices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Market Indices Standard Model."""
 
 from datetime import (
     date as dateType,
     datetime,
 )
-from typing import List, Optional, Set, Union
+from typing import Optional
 
 from dateutil import parser
 from pydantic import Field, StrictFloat, field_validator
 
 from openbb_core.provider.abstract.data import Data, ForceInt
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
@@ -26,19 +26,17 @@
     )
     end_date: Optional[dateType] = Field(
         description=QUERY_DESCRIPTIONS.get("end_date", ""), default=None
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class MarketIndicesData(Data):
     """Market Indices Data."""
 
     date: datetime = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     open: Optional[StrictFloat] = Field(
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/market_movers.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Market Snapshots Standard Model."""
 
 from typing import Optional
 
 from pydantic import Field
 
-from openbb_core.provider.abstract.data import Data
+from openbb_core.provider.abstract.data import Data, ForceInt
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 
 
 class MarketSnapshotsQueryParams(QueryParams):
     """Market Snapshots Query."""
 
 
 class MarketSnapshotsData(Data):
     """Market Snapshots Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
-
     open: Optional[float] = Field(
         description=DATA_DESCRIPTIONS.get("open", ""),
         default=None,
     )
     high: Optional[float] = Field(
         description=DATA_DESCRIPTIONS.get("high", ""),
         default=None,
@@ -30,17 +29,23 @@
         description=DATA_DESCRIPTIONS.get("low", ""),
         default=None,
     )
     close: Optional[float] = Field(
         description=DATA_DESCRIPTIONS.get("close", ""),
         default=None,
     )
+    volume: Optional[ForceInt] = Field(
+        description=DATA_DESCRIPTIONS.get("volume", ""), default=None
+    )
     prev_close: Optional[float] = Field(
-        description="The previous closing price of the stock.", default=None
+        description=DATA_DESCRIPTIONS.get("prev_close", ""),
+        default=None,
     )
-    change: Optional[float] = Field(description="The change in price.", default=None)
-    change_percent: Optional[float] = Field(
-        description="The change, as a percent.", default=None
+    change: Optional[float] = Field(
+        description="The change in price from the previous close.",
+        default=None,
     )
-    volume: Optional[int] = Field(
-        description=DATA_DESCRIPTIONS.get("volume", ""), default=None
+    change_percent: Optional[float] = Field(
+        description="The change in price from the previous close, as a normalized percent.",
+        default=None,
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/money_measures.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/money_measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Money Measures Standard Model."""
 
-
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/moody.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/moody.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Moody Corporate Bond Index Standard Model."""
 
 from datetime import (
     date as dateType,
 )
 from typing import Literal, Optional
 
-from pydantic import Field
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
@@ -27,13 +27,19 @@
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
     index_type: Literal["aaa", "baa"] = Field(
         default="aaa",
         description="The type of series.",
     )
 
+    @field_validator("index_type", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
 
 class MoodyCorporateBondIndexData(Data):
     """Moody Corporate Bond Index Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     rate: Optional[float] = Field(description="Moody Corporate Bond Index Rate.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/options_unusual.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/etf_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-"""Unusual Options Standard Model."""
+"""ETF Info Standard Model."""
 
 from typing import Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class OptionsUnusualQueryParams(QueryParams):
-    """Unusual Options Query."""
+class EtfInfoQueryParams(QueryParams):
+    """ETF Info Query."""
 
-    symbol: Optional[str] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("symbol", "") + " (the underlying symbol)",
-    )
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", "") + " (ETF)")
+
+    @field_validator("symbol")
+    @classmethod
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
-    @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: str):
-        """Convert symbol to uppercase."""
-        return v.upper() if v else None
 
+class EtfInfoData(Data):
+    """ETF Info Data."""
 
-class OptionsUnusualData(Data):
-    """Unusual Options Data."""
-
-    underlying_symbol: Optional[str] = Field(
-        description=DATA_DESCRIPTIONS.get("symbol", "") + " (the underlying symbol)",
-        default=None,
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", "") + " (ETF)")
+    name: Optional[str] = Field(description="Name of the ETF.")
+    description: Optional[str] = Field(
+        default=None, description="Description of the fund."
     )
-    contract_symbol: str = Field(description="Contract symbol for the option.")
+    inception_date: Optional[str] = Field(description="Inception date of the ETF.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """OTC Aggregate Standard Model."""
 
-
 from datetime import date as dateType
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
 
 class OTCAggregateQueryParams(QueryParams):
     """OTC Aggregate Query."""
 
-    symbol: str = Field(
+    symbol: Optional[str] = Field(
         description=QUERY_DESCRIPTIONS.get("symbol", ""),
         default=None,
     )
 
 
 class OTCAggregateData(Data):
     """OTC Aggregate Data."""
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/price_target.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,93 @@
-"""Price Target Standard Model."""
+"""LBMA Fixing Standard Model."""
 
-
-from datetime import datetime
-from typing import List, Optional, Set, Union
+from datetime import (
+    date as dateType,
+    datetime,
+)
+from typing import Literal, Optional
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class PriceTargetQueryParams(QueryParams):
-    """Price Target Query."""
+class LbmaFixingQueryParams(QueryParams):
+    """
+    LBMA Fixing Query.
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    Source: https://www.lbma.org.uk/prices-and-data/precious-metal-prices#/table
+    """
 
-    @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    asset: Literal["gold", "silver"] = Field(
+        description="The metal to get price fixing rates for.",
+        default="gold",
+    )
+    start_date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("start_date", ""),
+    )
+    end_date: Optional[dateType] = Field(
+        default=None,
+        description=QUERY_DESCRIPTIONS.get("end_date", ""),
+    )
 
+    @field_validator("asset", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
 
-class PriceTargetData(Data):
-    """Price Target Data."""
 
-    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
-    published_date: datetime = Field(description="Published date of the price target.")
-    news_url: Optional[str] = Field(
-        default=None, description="News URL of the price target."
+class LbmaFixingData(Data):
+    """LBMA Fixing Data.  Historical fixing prices in USD, GBP and EUR."""
+
+    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    usd_am: Optional[float] = Field(
+        default=None,
+        description="AM fixing price in USD.",
+    )
+    usd_pm: Optional[float] = Field(
+        default=None,
+        description="PM fixing price in USD.",
+    )
+    gbp_am: Optional[float] = Field(
+        default=None,
+        description="AM fixing price in GBP.",
+    )
+    gbp_pm: Optional[float] = Field(
+        default=None,
+        description="PM fixing price in GBP.",
     )
-    news_title: Optional[str] = Field(
-        default=None, description="News title of the price target."
+    euro_am: Optional[float] = Field(
+        default=None,
+        description="AM fixing price in EUR.",
     )
-    analyst_name: Optional[str] = Field(default=None, description="Analyst name.")
-    analyst_company: Optional[str] = Field(default=None, description="Analyst company.")
-    price_target: Optional[float] = Field(default=None, description="Price target.")
-    adj_price_target: Optional[float] = Field(
-        default=None, description="Adjusted price target."
+    euro_pm: Optional[float] = Field(
+        default=None,
+        description="PM fixing price in EUR.",
     )
-    price_when_posted: Optional[float] = Field(
-        default=None, description="Price when posted."
+    usd: Optional[float] = Field(
+        default=None,
+        description="Daily fixing price in USD.",
     )
-    news_publisher: Optional[str] = Field(
-        default=None, description="News publisher of the price target."
+    gbp: Optional[float] = Field(
+        default=None,
+        description="Daily fixing price in GBP.",
     )
-    news_base_url: Optional[str] = Field(
-        default=None, description="News base URL of the price target."
+    eur: Optional[float] = Field(
+        default=None,
+        description="Daily fixing price in EUR.",
     )
 
-    @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    @field_validator("date", mode="before", check_fields=False)
+    @classmethod
+    def validate_date(cls, v) -> dateType:
+        """Validate date."""
+        if isinstance(v, datetime):
+            return v.date()
+        return datetime.strptime(v, "%Y-%m-%d").date()
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Price Target Consensus Standard Model."""
 
-
 from typing import List, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
@@ -12,40 +11,43 @@
     QUERY_DESCRIPTIONS,
 )
 
 
 class PriceTargetConsensusQueryParams(QueryParams):
     """Price Target Consensus Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    symbol: Optional[str] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("symbol", "")
+    )
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    @classmethod
+    def to_upper(cls, v):
+        """Convert field to uppercase."""
+        return v.upper() if v else None
 
 
 class PriceTargetConsensusData(Data):
     """Price Target Consensus Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    name: Optional[str] = Field(default=None, description="The company name")
     target_high: Optional[float] = Field(
         default=None, description="High target of the price target consensus."
     )
     target_low: Optional[float] = Field(
         default=None, description="Low target of the price target consensus."
     )
     target_consensus: Optional[float] = Field(
         default=None, description="Consensus target of the price target consensus."
     )
     target_median: Optional[float] = Field(
         default=None, description="Median target of the price target consensus."
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    @classmethod
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/cash_flow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-"""Revenue by Business Line Standard Model."""
-
+"""Cash Flow Statement Standard Model."""
 
 from datetime import date as dateType
-from typing import Dict, List, Literal, Set, Union
+from typing import Optional
 
-from pydantic import Field, field_validator
+from pydantic import Field, NonNegativeInt, field_validator
 
-from openbb_core.provider.abstract.data import Data, ForceInt
+from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
-    QUERY_DESCRIPTIONS,
-)
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
 
-class RevenueBusinessLineQueryParams(QueryParams):
-    """Revenue by Business Line Query."""
+class CashFlowStatementQueryParams(QueryParams):
+    """Cash Flow Statement Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    period: Literal["quarter", "annual"] = Field(
-        default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
+    period: str = Field(
+        default="annual",
+        description=QUERY_DESCRIPTIONS.get("period", ""),
+    )
+    limit: Optional[NonNegativeInt] = Field(
+        default=5, description=QUERY_DESCRIPTIONS.get("limit", "")
     )
-    structure: Literal["hierarchical", "flat"] = Field(
-        default="flat", description="Structure of the returned data."
-    )  # should always be flat
 
     @field_validator("symbol", mode="before", check_fields=False)
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
-
-
-class RevenueBusinessLineData(Data):
-    """Revenue by Business Line Data."""
-
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    business_line: Dict[str, ForceInt] = Field(
-        description="Day level data containing the revenue of the business line."
+    @classmethod
+    def to_upper(cls, v: str):
+        """Convert field to uppercase."""
+        return v.upper()
+
+    @field_validator("period", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
+
+class CashFlowStatementData(Data):
+    """Cash Flow Statement Data."""
+
+    period_ending: dateType = Field(description="The end date of the reporting period.")
+    fiscal_period: Optional[str] = Field(
+        description="The fiscal period of the report.", default=None
+    )
+    fiscal_year: Optional[int] = Field(
+        description="The fiscal year of the fiscal period.", default=None
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,69 @@
-"""Revenue by Geographic Segments Standard Model."""
-
+"""Historical Attributes Standard Model."""
 
 from datetime import date as dateType
-from typing import Dict, List, Literal, Optional, Set, Union
+from typing import List, Literal, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
-from openbb_core.provider.abstract.data import Data, ForceInt
+from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class RevenueGeographicQueryParams(QueryParams):
-    """Revenue by Geographic Segments Query."""
+class HistoricalAttributesQueryParams(QueryParams):
+    """Historical Attributes Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    period: Literal["quarter", "annual"] = Field(
-        default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
-    )
-    structure: Literal["hierarchical", "flat"] = Field(
-        default="flat", description="Structure of the returned data."
-    )  # should always be flat
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol"))
+    tag: str = Field(description="Intrinio data tag ID or code.")
+    start_date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("start_date")
+    )
+    end_date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("end_date")
+    )
+    frequency: Optional[
+        Literal["daily", "weekly", "monthly", "quarterly", "yearly"]
+    ] = Field(default="yearly", description=QUERY_DESCRIPTIONS.get("frequency"))
+    limit: Optional[int] = Field(
+        default=1000, description=QUERY_DESCRIPTIONS.get("limit")
+    )
+    tag_type: Optional[str] = Field(
+        default=None, description="Filter by type, when applicable."
+    )
+    sort: Optional[Literal["asc", "desc"]] = Field(
+        default="desc", description="Sort order."
+    )
 
-    @field_validator("symbol", mode="before", check_fields=False)
+    @field_validator("tag", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def multiple_tags(cls, v: Union[str, List[str], Set[str]]):
+        """Accept a comma-separated string or list of tags."""
         if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+            return v.lower()
+        return ",".join([tag.lower() for tag in list(v)])
 
+    @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
-class RevenueGeographicData(Data):
-    """Revenue by Geographic Segments Data."""
+    @field_validator("frequency", "sort", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    geographic_segment: Dict[str, ForceInt] = Field(
-        description="Day level data containing the revenue of the geographic segment."
-    )
-    americas: Optional[ForceInt] = Field(
-        default=None, description="Revenue from the the American segment."
-    )
-    europe: Optional[ForceInt] = Field(
-        default=None, description="Revenue from the the European segment."
-    )
-    greater_china: Optional[ForceInt] = Field(
-        default=None, description="Revenue from the the Greater China segment."
-    )
-    japan: Optional[ForceInt] = Field(
-        default=None, description="Revenue from the the Japan segment."
-    )
-    rest_of_asia_pacific: Optional[ForceInt] = Field(
-        default=None, description="Revenue from the the Rest of Asia Pacific segment."
+
+class HistoricalAttributesData(Data):
+    """Historical Attributes Data."""
+
+    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date"))
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol"))
+    tag: Optional[str] = Field(
+        default=None, description="Tag name for the fetched data."
     )
+    value: Optional[float] = Field(default=None, description="The value of the data.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/risk_premium.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/risk_premium.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Risk Premium Standard Model."""
 
-
 from typing import Optional
 
 from pydantic import Field, NonNegativeFloat, PositiveFloat
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/search_attributes.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/sector_news.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,31 @@
-"""Sector News Standard Model."""
+"""Trailing Dividend Yield Standard Model."""
 
+from datetime import date as dateType
+from typing import Optional
 
-from datetime import datetime
-from typing import Dict, List, Optional
-
-from pydantic import Field, NonNegativeInt
+from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class SectorNewsQueryParams(QueryParams):
-    """Sector News Query."""
-
-    sectors: str = Field(
-        min_length=1,
-        description="A coma separated list of sectors.",
-    )
+class TrailingDivYieldQueryParams(QueryParams):
+    """Trailing Dividend Yield Query."""
 
-    limit: NonNegativeInt = Field(
-        default=20,
-        description=QUERY_DESCRIPTIONS.get("limit", "")
-        + " Here it is the no. of articles to return.",
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    limit: Optional[int] = Field(
+        default=252,
+        description=f"{QUERY_DESCRIPTIONS.get('limit', '')}"
+        " Default is 252, the number of trading days in a year.",
     )
 
 
-class SectorNewsData(Data):
-    """Sector News Data."""
+class TrailingDivYieldData(Data):
+    """Trailing Dividend Yield Data."""
 
-    date: datetime = Field(
-        description=DATA_DESCRIPTIONS.get("date", "")
-        + " Here it is the published date of the news."
-    )
-    title: str = Field(description="Title of the news.")
-    images: Optional[List[Dict[str, str]]] = Field(
-        default=None, description="Images associated with the news."
-    )
-    text: Optional[str] = Field(default=None, description="Text/body of the news.")
-    url: Optional[str] = Field(default=None, description="URL of the news.")
+    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
+    trailing_dividend_yield: float = Field(description="Trailing dividend yield.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/sector_pe.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/share_statistics.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/share_statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Share Statistics Standard Model."""
 
-
 from datetime import date as dateType
 from typing import List, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -17,19 +16,17 @@
 class ShareStatisticsQueryParams(QueryParams):
     """Share Statistics Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    def to_upper(cls, v: str) -> str:
+        """Convert field to uppercase."""
+        return v.upper()
 
 
 class ShareStatisticsData(Data):
     """Share Statistics Data."""
 
     symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
     date: Optional[dateType] = Field(
@@ -48,12 +45,12 @@
     )
     source: Optional[str] = Field(
         default=None, description="Source of the received data."
     )
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def upper_symbol(cls, v: Union[str, List[str], Set[str]]):
-        """Convert symbol to uppercase."""
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
         if isinstance(v, str):
             return v.upper()
         return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/short_volume.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/short_volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Short Volume Standard Model."""
+
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
@@ -11,15 +12,15 @@
     QUERY_DESCRIPTIONS,
 )
 
 
 class ShortVolumeQueryParams(QueryParams):
     """Short Volume Query."""
 
-    symbol: str = Field(default=None, description=QUERY_DESCRIPTIONS.get("symbol"))
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol"))
 
 
 class ShortVolumeData(Data):
     """Short Volume Data."""
 
     date: Optional[dateType] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("date")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-"""SOFR Standard Model."""
-
+"""SONIA Standard Model."""
 
 from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class SOFRQueryParams(QueryParams):
-    """SOFR Query."""
+class SONIAQueryParams(QueryParams):
+    """SONIA Query."""
 
     start_date: Optional[dateType] = Field(
         default=None,
         description=QUERY_DESCRIPTIONS.get("start_date", ""),
     )
     end_date: Optional[dateType] = Field(
         default=None,
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
 
 
-class SOFRData(Data):
-    """SOFR Data."""
+class SONIAData(Data):
+    """SONIA Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    rate: Optional[float] = Field(description="SOFR rate.")
+    rate: Optional[float] = Field(description="SONIA rate.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/spot.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/company_news.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,76 @@
-"""Spot Rate Standard Model."""
+"""Company News Standard Model."""
+
 from datetime import (
     date as dateType,
+    datetime,
 )
-from typing import List, Literal, Optional
+from typing import Dict, List, Optional
 
-from pydantic import Field, field_validator
+from dateutil.relativedelta import relativedelta
+from pydantic import Field, NonNegativeInt, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class SpotRateQueryParams(QueryParams):
-    """Spot Rate Query."""
+class CompanyNewsQueryParams(QueryParams):
+    """Company news Query."""
 
-    start_date: Optional[dateType] = Field(
+    symbol: Optional[str] = Field(
         default=None,
-        description=QUERY_DESCRIPTIONS.get("start_date", ""),
+        description=QUERY_DESCRIPTIONS.get("symbol", ""),
     )
-    end_date: Optional[dateType] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("end_date", ""),
+    start_date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("start_date", "")
     )
-    maturity: List[float] = Field(
-        default=[10.0], description="The maturities in years."
+    end_date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("end_date", "")
     )
-    category: List[Literal["par_yield", "spot_rate"]] = Field(
-        default=["spot_rate"],
-        description="The category.",
+    limit: Optional[NonNegativeInt] = Field(
+        default=2500, description=QUERY_DESCRIPTIONS.get("limit", "")
     )
 
-    @field_validator("maturity")
+    @field_validator("symbol", mode="before")
+    @classmethod
+    def symbols_validate(cls, v):
+        """Validate the symbols."""
+        return v.upper() if v else None
+
+    @field_validator("start_date", mode="before")
+    @classmethod
+    def start_date_validate(cls, v) -> dateType:  # pylint: disable=E0213
+        """Populate start date if empty."""
+        if not v:
+            now = datetime.now().date()
+            v = now - relativedelta(weeks=16)
+        return v
+
+    @field_validator("end_date", mode="before")
     @classmethod
-    def maturity_validate(cls, v):
-        """Validate maturity."""
-        for i in v:
-            if not isinstance(i, float):
-                raise ValueError("`maturity` must be a float")
-            if not 1 <= i <= 100:
-                raise ValueError("`maturity` must be between 1 and 100")
+    def end_date_validate(cls, v) -> dateType:  # pylint: disable=E0213
+        """Populate end date if empty."""
+        if not v:
+            v = datetime.now().date()
         return v
 
 
-class SpotRateData(Data):
-    """Spot Rate Data."""
+class CompanyNewsData(Data):
+    """Company News Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    rate: Optional[float] = Field(description="Spot Rate.")
+    date: datetime = Field(
+        description=DATA_DESCRIPTIONS.get("date", "")
+        + " Here it is the published date of the article."
+    )
+    title: str = Field(description="Title of the article.")
+    text: Optional[str] = Field(default=None, description="Text/body of the article.")
+    images: Optional[List[Dict[str, str]]] = Field(
+        default=None, description="Images associated with the article."
+    )
+    url: str = Field(description="URL to the article.")
+    symbols: Optional[str] = Field(
+        default=None, description="Symbols associated with the article."
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/tbffr.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/tbffr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Selected Treasury Bill Standard Model."""
+
 from datetime import (
     date as dateType,
 )
 from typing import Literal, Optional
 
-from pydantic import Field
+from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
@@ -26,13 +27,19 @@
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
     )
     maturity: Optional[Literal["3m", "6m"]] = Field(
         default="3m",
         description="The maturity",
     )
 
+    @field_validator("maturity", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
+
 
 class SelectedTreasuryBillData(Data):
     """Selected Treasury Bill Data."""
 
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
     rate: Optional[float] = Field(description="SelectedTreasuryBill Rate.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/tmc.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-"""Treasury Constant Maturity Model."""
-from datetime import (
-    date as dateType,
-)
-from typing import Literal, Optional
+"""US Yield Curve Standard Model."""
+
+from datetime import date as dateType
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
-    QUERY_DESCRIPTIONS,
-)
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 
 
-class TreasuryConstantMaturityQueryParams(QueryParams):
-    """Treasury Constant Maturity Query."""
+class USYieldCurveQueryParams(QueryParams):
+    """US Yield Curve Query."""
 
-    start_date: Optional[dateType] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("start_date", ""),
-    )
-    end_date: Optional[dateType] = Field(
+    date: Optional[dateType] = Field(
         default=None,
-        description=QUERY_DESCRIPTIONS.get("end_date", ""),
+        description=QUERY_DESCRIPTIONS.get("date", "")
+        + " Defaults to the most recent FRED entry.",
     )
-    maturity: Optional[Literal["3m", "2y"]] = Field(
-        default="3m",
-        description="The maturity",
+    inflation_adjusted: Optional[bool] = Field(
+        default=False, description="Get inflation adjusted rates."
     )
 
 
-class TreasuryConstantMaturityData(Data):
-    """Treasury Constant Maturity Data."""
+class USYieldCurveData(Data):
+    """US Yield Curve Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    rate: Optional[float] = Field(description="TreasuryConstantMaturity Rate.")
+    maturity: float = Field(description="Maturity of the treasury rate in years.")
+    rate: float = Field(
+        description="Associated rate given in decimal form (0.05 is 5%)"
+    )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/currency_pairs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-"""Trailing Dividend Yield Standard Model."""
+"""Currency Available Pairs Standard Model."""
 
-
-from datetime import date as dateType
+from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
-    QUERY_DESCRIPTIONS,
-)
+from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 
 
-class TrailingDivYieldQueryParams(QueryParams):
-    """Trailing Dividend Yield Query."""
+class CurrencyPairsQueryParams(QueryParams):
+    """Currency Available Pairs Query."""
 
-    symbol: str = Field(default=None, description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    query: Optional[str] = Field(
+        default=None, description="Query to search for currency pairs."
+    )
 
 
-class TrailingDivYieldData(Data):
-    """Trailing Dividend Yield Data."""
+class CurrencyPairsData(Data):
+    """Currency Available Pairs Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    trailing_dividend_yield: float = Field(description="Trailing dividend yield.")
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    name: Optional[str] = Field(default=None, description="Name of the currency pair.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         description=QUERY_DESCRIPTIONS.get("end_date", "") + " The default is today.",
     )
 
     @model_validator(mode="before")
     @classmethod
     def validate_dates(cls, values) -> dict:
         """Validate the query parameters."""
+        if not isinstance(values, dict):
+            return values
+
         if values.get("start_date") is None:
             values["start_date"] = (datetime.now() - timedelta(days=90)).strftime(
                 "%Y-%m-%d"
             )
         if values.get("end_date") is None:
             values["end_date"] = datetime.now().strftime("%Y-%m-%d")
         return values
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,68 @@
-"""Treasury Prices Standard Model."""
-
+"""Forward Sales Estimates Standard Model."""
 
 from datetime import date as dateType
 from typing import Optional
 
-from pydantic import Field
+from pydantic import Field, field_validator
 
-from openbb_core.provider.abstract.data import Data
+from openbb_core.provider.abstract.data import Data, ForceInt
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class USTreasuryPricesQueryParams(QueryParams):
-    """US Treasury Prices Query."""
+class ForwardSalesEstimatesQueryParams(QueryParams):
+    """Forward Sales Estimates Query Parameters."""
 
-    date: Optional[dateType] = Field(
-        description=QUERY_DESCRIPTIONS.get("date", "")
-        + " No date will return the current posted data.",
+    symbol: Optional[str] = Field(
         default=None,
+        description=QUERY_DESCRIPTIONS["symbol"],
     )
 
+    @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
+    def to_upper(cls, v):
+        """Convert field to uppercase."""
+        return v.upper() if v else None
+
 
-class USTreasuryPricesData(Data):
-    """US Treasury Prices Data."""
+class ForwardSalesEstimatesData(Data):
+    """Forward Sales Estimates Data."""
 
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    name: Optional[str] = Field(default=None, description="Name of the entity.")
     date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    cusip: str = Field(description="CUSIP of the security.")
-    security_type: str = Field(
-        description="The type of US Treasury security. Bill, Note, Bond, TIPS, FRN."
+    fiscal_year: Optional[int] = Field(
+        default=None, description="Fiscal year for the estimate."
     )
-    rate: Optional[float] = Field(
-        description="The annualized interest rate or coupon of the security.",
-        default=None,
+    fiscal_period: Optional[str] = Field(
+        default=None, description="Fiscal quarter for the estimate."
+    )
+    calendar_year: Optional[int] = Field(
+        default=None, description="Calendar year for the estimate."
+    )
+    calendar_period: Optional[str] = Field(
+        default=None, description="Calendar quarter for the estimate."
     )
-    maturity_date: dateType = Field(description="The maturity date of the security.")
-    call_date: Optional[dateType] = Field(
-        description="The call date of the security.", default=None
+    low_estimate: Optional[ForceInt] = Field(
+        default=None, description="The sales estimate low for the period."
     )
-    bid: Optional[float] = Field(
-        description="The bid price of the security.", default=None
+    high_estimate: Optional[ForceInt] = Field(
+        default=None, description="The sales estimate high for the period."
     )
-    offer: Optional[float] = Field(
-        description="The offer price of the security.", default=None
+    mean: Optional[ForceInt] = Field(
+        default=None, description="The sales estimate mean for the period."
     )
-    eod_price: Optional[float] = Field(
-        description="The end-of-day price of the security.", default=None
+    median: Optional[ForceInt] = Field(
+        default=None, description="The sales estimate median for the period."
+    )
+    standard_deviation: Optional[ForceInt] = Field(
+        default=None,
+        description="The sales estimate standard deviation for the period.",
+    )
+    number_of_analysts: Optional[int] = Field(
+        default=None,
+        description="Number of analysts providing estimates for the period.",
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/index_constituents.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-"""US Yield Curve Standard Model."""
+"""Index Constituents Standard Model."""
 
-from datetime import date as dateType
 from typing import Optional
 
 from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.descriptions import (
+    DATA_DESCRIPTIONS,
+    QUERY_DESCRIPTIONS,
+)
 
 
-class USYieldCurveQueryParams(QueryParams):
-    """US Yield Curve Query."""
+class IndexConstituentsQueryParams(QueryParams):
+    """Index Constituents Query."""
 
-    date: Optional[dateType] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("date", "")
-        + " Defaults to the most recent FRED entry.",
-    )
-    inflation_adjusted: Optional[bool] = Field(
-        default=False, description="Get inflation adjusted rates."
-    )
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
 
-class USYieldCurveData(Data):
-    """US Yield Curve Data."""
+class IndexConstituentsData(Data):
+    """Index Constituents Data."""
 
-    maturity: float = Field(description="Maturity of the treasury rate in years.")
-    rate: float = Field(
-        description="Associated rate given in decimal form (0.05 is 5%)"
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    name: Optional[str] = Field(
+        default=None, description="Name of the constituent company in the index."
     )
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/standard_models/world_news.py` & `openbb_core-1.2.1/openbb_core/provider/standard_models/available_indicators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-"""World News Standard Model."""
+"""Available Indicators Standard Model."""
 
+from typing import Optional
 
-from datetime import datetime
-from typing import Dict, List, Optional
-
-from pydantic import Field, NonNegativeInt
+from pydantic import Field
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
-    QUERY_DESCRIPTIONS,
-)
+from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 
 
-class WorldNewsQueryParams(QueryParams):
-    """World News Query."""
+class AvailableIndicesQueryParams(QueryParams):
+    """Available Indicators Query."""
 
-    limit: NonNegativeInt = Field(
-        default=20,
-        description=QUERY_DESCRIPTIONS.get("limit", "")
-        + " Here its the no. of articles to return.",
-    )
 
+class AvailableIndicatorsData(Data):
+    """Available Indicators Data.
 
-class WorldNewsData(Data):
-    """World News Data."""
+    Returns the list of available economic indicators from a provider.
+    """
 
-    date: datetime = Field(
-        description=DATA_DESCRIPTIONS.get("date", "")
-        + " Here it is the published date of the news."
+    symbol_root: Optional[str] = Field(
+        default=None, description="The root symbol representing the indicator."
+    )
+    symbol: Optional[str] = Field(
+        default=None,
+        description=DATA_DESCRIPTIONS.get("symbol", "")
+        + " The root symbol with additional codes.",
+    )
+    country: Optional[str] = Field(
+        default=None,
+        description="The name of the country, region, or entity represented by the symbol.",
+    )
+    iso: Optional[str] = Field(
+        default=None,
+        description="The ISO code of the country, region, or entity represented by the symbol.",
+    )
+    description: Optional[str] = Field(
+        default=None, description="The description of the indicator."
     )
-    title: str = Field(description="Title of the news.")
-    images: Optional[List[Dict[str, str]]] = Field(
-        default=None, description="Images associated with the news."
+    frequency: Optional[str] = Field(
+        default=None, description="The frequency of the indicator data."
     )
-    text: Optional[str] = Field(default=None, description="Text/body of the news.")
-    url: Optional[str] = Field(default=None, description="URL of the news.")
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/utils/client.py` & `openbb_core-1.2.1/openbb_core/provider/utils/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Aiohttp client."""
+
 # pylint: disable=protected-access,invalid-overridden-method
 import asyncio
 import random
 import re
 import warnings
 import zlib
 from typing import Any, Dict, Type, Union
@@ -36,14 +37,15 @@
     return random.choice(user_agent_strings)  # nosec # noqa: S311
 
 
 class ClientResponse(aiohttp.ClientResponse):
     """Client response class."""
 
     def __init__(self, *args, **kwargs):
+        """Initialize the response."""
         kwargs["request_info"] = self.obfuscate_request_info(kwargs["request_info"])
         super().__init__(*args, **kwargs)
 
     @classmethod
     def obfuscate_request_info(
         cls, request_info: aiohttp.RequestInfo
     ) -> aiohttp.RequestInfo:
@@ -56,18 +58,21 @@
 
     async def json(self, **kwargs) -> Union[dict, list]:
         """Return the json response."""
         return await super().json(**kwargs)
 
 
 class ClientSession(aiohttp.ClientSession):
+    """Client session."""
+
     _response_class: Type[ClientResponse]
     _session: "ClientSession"
 
     def __init__(self, *args, **kwargs):
+        """Initialize the session."""
         kwargs["connector"] = kwargs.get(
             "connector", aiohttp.TCPConnector(ttl_dns_cache=300)
         )
         kwargs["response_class"] = kwargs.get("response_class", ClientResponse)
         kwargs["auto_decompress"] = kwargs.get("auto_decompress", False)
 
         super().__init__(*args, **kwargs)
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/utils/descriptions.py` & `openbb_core-1.2.1/openbb_core/provider/utils/descriptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "symbol": "Symbol to get data for.",
     "start_date": "Start date of the data, in YYYY-MM-DD format.",
     "end_date": "End date of the data, in YYYY-MM-DD format.",
     "interval": "Time interval of the data to return.",
     "period": "Time period of the data to return.",
     "date": "A specific date to get data for.",
     "limit": "The number of data entries to return.",
+    "country": "The country to get data.",
     "countries": "The country or countries to get data.",
     "units": "The unit of measurement for the data.",
     "frequency": "The frequency of the data.",
 }
 
 DATA_DESCRIPTIONS = {
     "symbol": "Symbol representing the entity requested in the data.",
@@ -20,8 +21,9 @@
     "open": "The open price.",
     "high": "The high price.",
     "low": "The low price.",
     "close": "The close price.",
     "volume": "The trading volume.",
     "adj_close": "The adjusted close price.",
     "vwap": "Volume Weighted Average Price over the period.",
+    "prev_close": "The previous close price.",
 }
```

### Comparing `openbb_core-1.2.0/openbb_core/provider/utils/helpers.py` & `openbb_core-1.2.1/openbb_core/provider/utils/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,68 @@
 """Provider helpers."""
+
 import asyncio
+import os
 import re
+from datetime import date, datetime, timedelta, timezone
+from difflib import SequenceMatcher
 from functools import partial
 from inspect import iscoroutinefunction
-from typing import Awaitable, Callable, List, Literal, Optional, TypeVar, Union, cast
+from typing import (
+    Awaitable,
+    Callable,
+    List,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import requests
 from anyio import start_blocking_portal
 from typing_extensions import ParamSpec
 
+from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.utils.client import (
     ClientResponse,
     ClientSession,
     get_user_agent,
 )
 
 T = TypeVar("T")
 P = ParamSpec("P")
+D = TypeVar("D", bound="Data")
+
+
+def check_item(item: str, allowed: List[str], threshold: float = 0.75) -> None:
+    """Check if an item is in a list of allowed items and raise an error if not.
+
+    Parameters
+    ----------
+    item : str
+        The item to check.
+    allowed : List[str]
+        The list of allowed items.
+    threshold : float, optional
+        The similarity threshold for the error message, by default 0.75
+
+    Raises
+    ------
+    ValueError
+        If the item is not in the allowed list.
+    """
+    if item not in allowed:
+        similarities = map(
+            lambda c: (c, SequenceMatcher(None, item, c).ratio()), allowed
+        )
+        similar, score = max(similarities, key=lambda x: x[1])
+        if score > threshold:
+            raise ValueError(f"'{item}' is not available. Did you mean '{similar}'?")
+        raise ValueError(f"'{item}' is not available.")
 
 
 def get_querystring(items: dict, exclude: List[str]) -> str:
     """Turn a dictionary into a querystring, excluding the keys in the exclude list.
 
     Parameters
     ----------
@@ -58,16 +100,16 @@
     method: Literal["GET", "POST"] = "GET",
     timeout: int = 10,
     response_callback: Optional[
         Callable[[ClientResponse, ClientSession], Awaitable[Union[dict, List[dict]]]]
     ] = None,
     **kwargs,
 ) -> Union[dict, List[dict]]:
-    """Abstract helper to make requests from a url with potential headers and params.
-
+    """
+    Abstract helper to make requests from a url with potential headers and params.
 
     Parameters
     ----------
     url : str
         Url to make the request to
     method : str, optional
         HTTP method to use.  Can be "GET" or "POST", by default "GET"
@@ -142,21 +184,21 @@
         for result in await asyncio.gather(
             *[amake_request(url, session=session, **kwargs) for url in urls],
             return_exceptions=True,
         ):
             is_exception = isinstance(result, Exception)
 
             if is_exception and kwargs.get("raise_for_status", False):
-                raise result
+                raise result  # type: ignore[misc]
 
             if is_exception or not result:
                 continue
 
-            results.extend(  # type: ignore
-                result if isinstance(result, list) else [result]
+            results.extend(
+                result if isinstance(result, list) else [result]  # type: ignore[list-item]
             )
 
         return results
 
     finally:
         await session.close()
 
@@ -227,27 +269,57 @@
     )
 
 
 async def maybe_coroutine(
     func: Callable[P, Union[T, Awaitable[T]]], /, *args: P.args, **kwargs: P.kwargs
 ) -> T:
     """Check if a function is a coroutine and run it accordingly."""
-
     if not iscoroutinefunction(func):
         return cast(T, func(*args, **kwargs))
 
     return await func(*args, **kwargs)
 
 
 def run_async(
     func: Callable[P, Awaitable[T]], /, *args: P.args, **kwargs: P.kwargs
 ) -> T:
     """Run a coroutine function in a blocking context."""
-
     if not iscoroutinefunction(func):
         return cast(T, func(*args, **kwargs))
 
     with start_blocking_portal() as portal:
         try:
             return portal.call(partial(func, *args, **kwargs))
         finally:
             portal.call(portal.stop)
+
+
+def filter_by_dates(
+    data: List[D], start_date: Optional[date] = None, end_date: Optional[date] = None
+) -> List[D]:
+    """Filter data by dates."""
+    if start_date is None and end_date is None:
+        return data
+
+    def _filter(d: Data) -> bool:
+        _date = getattr(d, "date", None)
+        dt = _date.date() if _date and isinstance(_date, datetime) else _date
+        if dt:
+            if start_date and end_date:
+                return start_date <= dt <= end_date
+            if start_date:
+                return dt >= start_date
+            if end_date:
+                return dt <= end_date
+            return True
+        return False
+
+    return list(filter(_filter, data))
+
+
+def safe_fromtimestamp(
+    timestamp: Union[float, int], tz: Optional[timezone] = None
+) -> datetime:
+    """datetime.fromtimestamp alternative which supports negative timestamps on Windows platform."""
+    if os.name == "nt" and timestamp < 0:
+        return datetime(1970, 1, 1, tzinfo=tz) + timedelta(seconds=timestamp)
+    return datetime.fromtimestamp(timestamp, tz)
```

### Comparing `openbb_core-1.2.0/pyproject.toml` & `openbb_core-1.2.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "openbb-core"
-version = "1.2.0"
+version = "1.2.1"
 description = "OpenBB package with core functionality"
 authors = ["OpenBB Team <hello@openbb.co>"]
+license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_core" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 uvicorn = "^0.24"
 websockets = "^12.0"
 pandas = ">=1.5.3"
 html5lib = "^1.1"
-fastapi = "^0.104.1"
-python-jose = "^3.3.0"
+fastapi = "^0.111.0"
 uuid7 = "^0.1.0"
-posthog = "^3.0.1"
-python-multipart = "^0.0.6"
+posthog = "^3.3.1"
+python-multipart = "^0.0.7"
 pydantic = "^2.5.1"
 requests = "^2.31.0"
 importlib-metadata = "^6.8.0"
 python-dotenv = "^1.0.0"
-aiohttp = "^3.9.0"
+aiohttp = "^3.9.5"
 ruff = "^0.1.6"
+pyjwt = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 pytest-subtests = "^0.11.0"
 pytest-recorder = "^0.2.4"
 pytest-asyncio = "^0.23.2"
-black = "^23.11.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openbb_core-1.2.0/PKG-INFO` & `openbb_core-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-core
-Version: 1.2.0
+Version: 1.2.1
 Summary: OpenBB package with core functionality
+License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.9.0,<4.0.0)
-Requires-Dist: fastapi (>=0.104.1,<0.105.0)
+Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0)
 Requires-Dist: pandas (>=1.5.3)
-Requires-Dist: posthog (>=3.0.1,<4.0.0)
+Requires-Dist: posthog (>=3.3.1,<4.0.0)
 Requires-Dist: pydantic (>=2.5.1,<3.0.0)
+Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: python-jose (>=3.3.0,<4.0.0)
-Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
+Requires-Dist: python-multipart (>=0.0.7,<0.0.8)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruff (>=0.1.6,<0.2.0)
 Requires-Dist: uuid7 (>=0.1.0,<0.2.0)
 Requires-Dist: uvicorn (>=0.24,<0.25)
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
```

