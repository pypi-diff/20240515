# Comparing `tmp/openbb_fmp-1.1.5.tar.gz` & `tmp/openbb_fmp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fmp-1.1.5.tar", max compression
+gzip compressed data, was "openbb_fmp-1.2.0.tar", max compression
```

## Comparing `openbb_fmp-1.1.5.tar` & `openbb_fmp-1.2.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      478 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/README.md
--rw-r--r--   0        0        0     8255 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6076 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5308 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6768 2024-04-19 13:09:31.739184 openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2780 2024-04-19 13:09:31.739184 openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3607 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-04-19 13:10:31.744034 openbb_fmp-1.1.5/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5050 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2270 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10603 2024-04-19 13:10:31.744034 openbb_fmp-1.1.5/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3938 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     6297 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3521 2024-04-19 13:09:31.739184 openbb_fmp-1.1.5/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3270 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/py.typed
--rw-r--r--   0        0        0       17 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4246 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0      433 2024-04-19 16:41:18.207237 openbb_fmp-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 openbb_fmp-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      351 2024-05-15 14:25:41.787335 openbb_fmp-1.2.0/README.md
+-rw-r--r--   0        0        0     9101 2024-05-14 15:30:05.613337 openbb_fmp-1.2.0/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-29 11:03:36.842842 openbb_fmp-1.2.0/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-10 10:40:27.292197 openbb_fmp-1.2.0/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-04-08 12:02:16.633618 openbb_fmp-1.2.0/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-04-08 12:02:16.633789 openbb_fmp-1.2.0/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-04-08 12:02:16.633907 openbb_fmp-1.2.0/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-04-08 12:02:16.634020 openbb_fmp-1.2.0/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-04-08 12:02:16.634152 openbb_fmp-1.2.0/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-04-02 11:35:59.449553 openbb_fmp-1.2.0/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-04-08 12:02:16.634306 openbb_fmp-1.2.0/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-04-08 12:02:16.634395 openbb_fmp-1.2.0/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-04-08 12:02:16.634510 openbb_fmp-1.2.0/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2961 2024-05-10 10:40:27.292367 openbb_fmp-1.2.0/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-04-02 11:35:59.450137 openbb_fmp-1.2.0/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5908 2024-05-10 11:33:20.067768 openbb_fmp-1.2.0/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-04-08 12:02:16.634839 openbb_fmp-1.2.0/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5901 2024-05-10 11:33:20.067963 openbb_fmp-1.2.0/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     3208 2024-05-09 15:04:29.070919 openbb_fmp-1.2.0/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6082 2024-05-10 10:40:27.293022 openbb_fmp-1.2.0/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-04-02 11:35:59.451189 openbb_fmp-1.2.0/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-04-08 12:02:16.635270 openbb_fmp-1.2.0/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     5073 2024-05-14 15:30:05.613556 openbb_fmp-1.2.0/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5924 2024-05-10 10:40:27.293165 openbb_fmp-1.2.0/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-04-02 11:35:59.451669 openbb_fmp-1.2.0/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-04-08 12:02:16.635574 openbb_fmp-1.2.0/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6114 2024-05-10 10:40:27.293312 openbb_fmp-1.2.0/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5314 2024-05-10 10:40:27.293457 openbb_fmp-1.2.0/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-04-02 11:35:59.452060 openbb_fmp-1.2.0/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6499 2024-05-10 10:40:27.293618 openbb_fmp-1.2.0/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3452 2024-05-10 10:40:27.293766 openbb_fmp-1.2.0/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3162 2024-05-10 10:40:27.293941 openbb_fmp-1.2.0/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6772 2024-05-09 15:04:29.071085 openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-04-02 11:35:59.452710 openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2780 2024-04-23 10:22:39.667379 openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3623 2024-05-10 10:40:27.294092 openbb_fmp-1.2.0/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-04-08 12:02:16.636814 openbb_fmp-1.2.0/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-04-02 11:35:59.453264 openbb_fmp-1.2.0/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4304 2024-05-10 10:40:27.294266 openbb_fmp-1.2.0/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-04-08 12:02:16.637030 openbb_fmp-1.2.0/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5056 2024-05-10 10:40:27.294412 openbb_fmp-1.2.0/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-04-08 12:02:16.637259 openbb_fmp-1.2.0/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-04-02 11:35:59.453743 openbb_fmp-1.2.0/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-04-02 11:35:59.453824 openbb_fmp-1.2.0/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-04-02 11:35:59.453905 openbb_fmp-1.2.0/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-04-08 12:02:16.637445 openbb_fmp-1.2.0/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-04-02 11:35:59.454171 openbb_fmp-1.2.0/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-04-08 12:02:16.637552 openbb_fmp-1.2.0/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5832 2024-05-10 10:40:27.294557 openbb_fmp-1.2.0/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-04-02 11:35:59.454433 openbb_fmp-1.2.0/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-04-02 11:35:59.454534 openbb_fmp-1.2.0/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2270 2024-04-23 10:22:39.667606 openbb_fmp-1.2.0/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10619 2024-05-10 10:40:27.294661 openbb_fmp-1.2.0/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3938 2024-04-23 10:22:39.667724 openbb_fmp-1.2.0/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     6297 2024-04-23 10:22:39.667856 openbb_fmp-1.2.0/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3527 2024-05-10 10:40:27.294808 openbb_fmp-1.2.0/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4238 2024-05-10 10:40:27.295370 openbb_fmp-1.2.0/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3276 2024-05-10 10:40:27.295527 openbb_fmp-1.2.0/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847376 openbb_fmp-1.2.0/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-04-08 12:02:16.638378 openbb_fmp-1.2.0/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-04-08 12:02:16.638491 openbb_fmp-1.2.0/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-04-02 11:35:59.455545 openbb_fmp-1.2.0/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-04-02 11:35:59.455637 openbb_fmp-1.2.0/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-04-08 12:02:16.638589 openbb_fmp-1.2.0/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-04-08 12:02:16.638702 openbb_fmp-1.2.0/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847941 openbb_fmp-1.2.0/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-04-23 10:22:39.668253 openbb_fmp-1.2.0/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-08 12:02:16.638823 openbb_fmp-1.2.0/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-04-23 10:22:39.668404 openbb_fmp-1.2.0/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.848164 openbb_fmp-1.2.0/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0      459 2024-05-15 16:06:42.123564 openbb_fmp-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 openbb_fmp-1.2.0/PKG-INFO
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/analyst_estimates.py` & `openbb_fmp-1.2.0/openbb_fmp/models/analyst_estimates.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class FMPAnalystEstimatesQueryParams(AnalystEstimatesQueryParams):
     """FMP Analyst Estimates Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/analyst-estimates-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     period: Literal["quarter", "annual"] = Field(
         default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
     )
     limit: Optional[int] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("limit", "")
     )
@@ -56,15 +56,15 @@
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         symbols = query.symbol.split(",")  # type: ignore
 
-        results = []
+        results: List[dict] = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
             url = create_url(
                 3, f"analyst-estimates/{symbol}", api_key, query, ["symbol"]
             )
             result = await amake_request(
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/available_indices.py` & `openbb_fmp-1.2.0/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/balance_sheet.py` & `openbb_fmp-1.2.0/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/balance_sheet_growth.py` & `openbb_fmp-1.2.0/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/calendar_dividend.py` & `openbb_fmp-1.2.0/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/calendar_earnings.py` & `openbb_fmp-1.2.0/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/calendar_splits.py` & `openbb_fmp-1.2.0/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/cash_flow.py` & `openbb_fmp-1.2.0/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/cash_flow_growth.py` & `openbb_fmp-1.2.0/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/company_filings.py` & `openbb_fmp-1.2.0/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/company_news.py` & `openbb_fmp-1.2.0/openbb_fmp/models/company_news.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class FMPCompanyNewsQueryParams(CompanyNewsQueryParams):
     """FMP Company News Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/stock-news-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     page: Optional[int] = Field(
         default=0,
         description="Page number of the results. Use in combination with limit.",
     )
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/company_overview.py` & `openbb_fmp-1.2.0/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/crypto_historical.py` & `openbb_fmp-1.2.0/openbb_fmp/models/crypto_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     FMP Crypto Historical Price Query.
 
     Source:
     https://site.financialmodelingprep.com/developer/docs/cryptocurrency-historical-data-api/#Historical-Daily-Prices
     """
 
     __alias_dict__ = {"start_date": "from", "end_date": "to"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
 
 
 class FMPCryptoHistoricalData(CryptoHistoricalData):
@@ -96,15 +96,15 @@
         base_url = "https://financialmodelingprep.com/api/v3"
         query_str = get_querystring(query.model_dump(), ["symbol"])
 
         def get_url_params(symbol: str) -> str:
             url_params = f"{symbol}?{query_str}&apikey={api_key}"
             url = f"{base_url}/historical-chart/{interval}/{url_params}"
             if interval == "1day":
-                url = f"{base_url}/historical-price-full/crypto/{url_params}"
+                url = f"{base_url}/historical-price-full/{url_params}"
             return url
 
         symbols = query.symbol.split(",")
 
         results = []
         messages = []
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/crypto_search.py` & `openbb_fmp-1.2.0/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/currency_historical.py` & `openbb_fmp-1.2.0/openbb_fmp/models/currency_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class FMPCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """FMP Currency Historical Price Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Historical-Forex-Price
     """
 
     __alias_dict__ = {"start_date": "from", "end_date": "to"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
 
 
 class FMPCurrencyHistoricalData(CurrencyHistoricalData):
@@ -94,29 +94,26 @@
         base_url = "https://financialmodelingprep.com/api/v3"
         query_str = get_querystring(query.model_dump(), ["symbol"])
 
         def get_url_params(symbol: str) -> str:
             url_params = f"{symbol}?{query_str}&apikey={api_key}"
             url = f"{base_url}/historical-chart/{interval}/{url_params}"
             if interval == "1day":
-                url = f"{base_url}/historical-price-full/forex/{url_params}"
+                url = f"{base_url}/historical-price-full/{url_params}"
             return url
 
         symbols = query.symbol.split(",")
 
         results = []
         messages = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
-
             url = get_url_params(symbol)
-
             data = []
-
             response = await amake_request(url, **kwargs)
 
             if isinstance(response, dict) and response.get("Error Message"):
                 message = f"Error fetching data for {symbol}: {response.get('Error Message', '')}"
                 warn(message)
                 messages.append(message)
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/currency_snapshots.py` & `openbb_fmp-1.2.0/openbb_fmp/models/currency_snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class FMPCurrencySnapshotsQueryParams(CurrencySnapshotsQueryParams):
     """FMP Currency Snapshots Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs#exchange-prices-quote
     """
 
-    __json_schema_extra__ = {"base": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"base": {"multiple_items_allowed": True}}
 
 
 class FMPCurrencySnapshotsData(CurrencySnapshotsData):
     """FMP Currency Snapshots Data."""
 
     __alias_dict__ = {
         "last_rate": "price",
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/discovery_filings.py` & `openbb_fmp-1.2.0/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/earnings_call_transcript.py` & `openbb_fmp-1.2.0/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/equity_historical.py` & `openbb_fmp-1.2.0/openbb_fmp/models/equity_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class FMPEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """FMP Equity Historical Price Query.
 
     Source: https://financialmodelingprep.com/developer/docs/#Stock-Historical-Price
     """
 
     __alias_dict__ = {"start_date": "from", "end_date": "to"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
 
 
 class FMPEquityHistoricalData(EquityHistoricalData):
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/equity_ownership.py` & `openbb_fmp-1.2.0/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/equity_peers.py` & `openbb_fmp-1.2.0/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/equity_profile.py` & `openbb_fmp-1.2.0/openbb_fmp/models/equity_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class FMPEquityProfileQueryParams(EquityInfoQueryParams):
     """FMP Equity Profile Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/companies-key-stats-free-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEquityProfileData(EquityInfoData):
     """FMP Equity Profile Data."""
 
     __alias_dict__ = {
         "name": "companyName",
@@ -44,15 +44,15 @@
         "hq_country": "country",
         "business_phone_no": "phone",
         "industry_category": "industry",
         "employees": "fullTimeEmployees",
         "long_description": "description",
         "first_stock_price_date": "ipoDate",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     is_etf: bool = Field(description="If the symbol is an ETF.")
     is_actively_trading: bool = Field(description="If the company is actively trading.")
     is_adr: bool = Field(description="If the stock is an ADR.")
     is_fund: bool = Field(description="If the company is a fund.")
     image: Optional[str] = Field(default=None, description="Image of the company.")
     currency: Optional[str] = Field(
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/equity_quote.py` & `openbb_fmp-1.2.0/openbb_fmp/models/equity_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class FMPEquityQuoteQueryParams(EquityQuoteQueryParams):
     """FMP Equity Quote Query.
 
     Source: https://financialmodelingprep.com/developer/docs/#Stock-Historical-Price
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEquityQuoteData(EquityQuoteData):
     """FMP Equity Quote Data."""
 
     __alias_dict__ = {
         "price_avg50": "priceAvg50",
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/equity_screener.py` & `openbb_fmp-1.2.0/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_fmp-1.2.0/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class FMPEquityValuationMultiplesQueryParams(EquityValuationMultiplesQueryParams):
     """FMP Equity Valuation Multiples Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Company-Key-Metrics
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEquityValuationMultiplesData(EquityValuationMultiplesData):
     """FMP Equity Valuation Multiples Data."""
 
     __alias_dict__ = {
         "revenue_per_share_ttm": "revenuePerShareTTM",
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/etf_countries.py` & `openbb_fmp-1.2.0/openbb_fmp/models/etf_countries.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_fmp.utils.helpers import create_url, response_callback
 from pandas import DataFrame
 
 
 class FMPEtfCountriesQueryParams(EtfCountriesQueryParams):
     """FMP ETF Countries Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEtfCountriesData(EtfCountriesData):
     """FMP ETF Countries Data."""
 
 
 class FMPEtfCountriesFetcher(
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/etf_equity_exposure.py` & `openbb_fmp-1.2.0/openbb_fmp/models/etf_equity_exposure.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class FMPEtfEquityExposureQueryParams(EtfEquityExposureQueryParams):
     """
     FMP ETF Equity Exposure Query Params.
 
     Source: https://site.financialmodelingprep.com/developer/docs/etf-stock-exposure-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEtfEquityExposureData(EtfEquityExposureData):
     """FMP ETF Equity Exposure Data."""
 
     __alias_dict__ = {
         "equity_symbol": "assetExposure",
@@ -60,15 +60,15 @@
         query: FMPEtfEquityExposureQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         symbols = query.symbol.split(",")
-        results = []
+        results: List[dict] = []
 
         async def get_one(symbol):
             """Get one symbol."""
             url = f"https://financialmodelingprep.com/api/v3/etf-stock-exposure/{symbol}?apikey={api_key}"
             response = await amake_request(
                 url, response_callback=response_callback, **kwargs
             )
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings.py` & `openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         alias="valUsd",
         default=None,
     )
     weight: Optional[float] = Field(
         description="The weight of the holding, as a normalized percent.",
         alias="pctVal",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     payoff_profile: Optional[str] = Field(
         description="The payoff profile of the holding.",
         alias="payoffProfile",
         default=None,
     )
     asset_category: Optional[str] = Field(
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings_date.py` & `openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings_performance.py` & `openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/etf_info.py` & `openbb_fmp-1.2.0/openbb_fmp/models/etf_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_core.provider.utils.helpers import amake_request
 from pydantic import Field
 
 
 class FMPEtfInfoQueryParams(EtfInfoQueryParams):
     """FMP ETF Info Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEtfInfoData(EtfInfoData):
     """FMP ETF Info Data."""
 
     issuer: Optional[str] = Field(
         default=None, description="Company of the ETF.", alias="etfCompany"
@@ -39,15 +39,15 @@
     )
     nav_currency: Optional[str] = Field(
         default=None, description="Currency of the ETF's net asset value."
     )
     expense_ratio: Optional[float] = Field(
         default=None,
         description="The expense ratio, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     holdings_count: Optional[int] = Field(
         default=None, description="Number of holdings."
     )
     avg_volume: Optional[float] = Field(
         default=None, description="Average daily trading volume."
     )
@@ -72,15 +72,15 @@
         query: FMPEtfInfoQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         symbols = query.symbol.split(",")
-        results = []
+        results: List = []
 
         async def get_one(symbol):
             """Get one symbol."""
             url = f"https://financialmodelingprep.com/api/v4/etf-info?symbol={symbol}&apikey={api_key}"
             response = await amake_request(url)
             if not response:
                 warn(f"No results found for {symbol}.")
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/etf_search.py` & `openbb_fmp-1.2.0/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/etf_sectors.py` & `openbb_fmp-1.2.0/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/executive_compensation.py` & `openbb_fmp-1.2.0/openbb_fmp/models/executive_compensation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class FMPExecutiveCompensationQueryParams(ExecutiveCompensationQueryParams):
     """FMP Executive Compensation Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/executive-compensation-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     year: Optional[int] = Field(default=None, description="Year of the compensation.")
 
 
 class FMPExecutiveCompensationData(ExecutiveCompensationData):
     """FMP Executive Compensation Data."""
 
@@ -82,15 +82,15 @@
 
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         base_url = "https://financialmodelingprep.com/api/v4/"
 
         symbols = query.symbol.split(",")
 
-        results = []
+        results: List[dict] = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
 
             url = f"{base_url}/governance/executive_compensation?symbol={symbol}&apikey={api_key}"
             result = await amake_request(
                 url, response_callback=response_callback, **kwargs
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/financial_ratios.py` & `openbb_fmp-1.2.0/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/forward_eps_estimates.py` & `openbb_fmp-1.2.0/openbb_fmp/models/forward_eps_estimates.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class FMPForwardEpsEstimatesQueryParams(ForwardEpsEstimatesQueryParams):
     """FMP Forward EPS Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/analyst-estimates-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     __alias_dict__ = {"fiscal_period": "period"}
 
     fiscal_period: Literal["annual", "quarter"] = Field(
         default="annual",
         description="The future fiscal period to retrieve estimates for.",
     )
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/historical_dividends.py` & `openbb_fmp-1.2.0/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/historical_employees.py` & `openbb_fmp-1.2.0/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/historical_eps.py` & `openbb_fmp-1.2.0/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/historical_splits.py` & `openbb_fmp-1.2.0/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/income_statement.py` & `openbb_fmp-1.2.0/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/income_statement_growth.py` & `openbb_fmp-1.2.0/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/index_constituents.py` & `openbb_fmp-1.2.0/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/index_historical.py` & `openbb_fmp-1.2.0/openbb_fmp/models/index_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class FMPIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """FMP Index Historical Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/historical-index-price-api/
     """
 
     __alias_dict__ = {"start_date": "from", "end_date": "to"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
 
 
 class FMPIndexHistoricalData(IndexHistoricalData):
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/insider_trading.py` & `openbb_fmp-1.2.0/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/institutional_ownership.py` & `openbb_fmp-1.2.0/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/key_executives.py` & `openbb_fmp-1.2.0/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/key_metrics.py` & `openbb_fmp-1.2.0/openbb_fmp/models/key_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class FMPKeyMetricsQueryParams(KeyMetricsQueryParams):
     """FMP Key Metrics Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/company-key-metrics-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     with_ttm: Optional[bool] = Field(
         default=False, description="Include trailing twelve months (TTM) data."
     )
 
 
 class FMPKeyMetricsData(KeyMetricsData):
@@ -118,15 +118,15 @@
     interest_coverage: Optional[float] = Field(
         default=None, description="Interest coverage"
     )
     income_quality: Optional[float] = Field(default=None, description="Income quality")
     dividend_yield: Optional[float] = Field(
         default=None,
         description="Dividend yield, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     payout_ratio: Optional[float] = Field(default=None, description="Payout ratio")
     sales_general_and_administrative_to_revenue: Optional[float] = Field(
         default=None,
         description="Sales general and administrative expenses-to-revenue ratio",
     )
     research_and_development_to_revenue: Optional[float] = Field(
@@ -225,15 +225,15 @@
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         base_url = "https://financialmodelingprep.com/api/v3"
 
         symbols = query.symbol.split(",")
 
-        results = []
+        results: List = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
 
             url = f"{base_url}/key-metrics/{symbol}?period={query.period}&limit={query.limit}&apikey={api_key}"
 
             result = await amake_request(
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/market_indices.py` & `openbb_fmp-1.2.0/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/market_snapshots.py` & `openbb_fmp-1.2.0/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/price_performance.py` & `openbb_fmp-1.2.0/openbb_fmp/models/price_performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class FMPPricePerformanceQueryParams(RecentPerformanceQueryParams):
     """FMP Price Performance Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/stock-split-calendar-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPPricePerformanceData(RecentPerformanceData):
     """FMP Price Performance Data."""
 
     symbol: str = Field(description="The ticker symbol.")
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/price_target.py` & `openbb_fmp-1.2.0/openbb_fmp/models/price_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class FMPPriceTargetQueryParams(PriceTargetQueryParams):
     """FMP Price Target Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Price-Target
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     with_grade: bool = Field(
         False,
         description="Include upgrades and downgrades in the response.",
     )
 
 
@@ -85,15 +85,15 @@
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         endpoint = "upgrades-downgrades" if query.with_grade else "price-target"
 
         symbols = query.symbol.split(",")  # type: ignore
 
-        results = []
+        results: List[dict] = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
             url = create_url(4, endpoint, api_key, query, exclude=["limit", "symbol"])
             url += f"&symbol={symbol}"
             result = await amake_request(
                 url, response_callback=response_callback, **kwargs
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/price_target_consensus.py` & `openbb_fmp-1.2.0/openbb_fmp/models/price_target_consensus.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class FMPPriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """FMP Price Target Consensus Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/price-target-consensus-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def check_symbol(cls, value):
         """Check the symbol."""
         if not value:
             raise RuntimeError("Error: Symbol is a required field for FMP.")
```

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/revenue_business_line.py` & `openbb_fmp-1.2.0/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/revenue_geographic.py` & `openbb_fmp-1.2.0/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/risk_premium.py` & `openbb_fmp-1.2.0/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/share_statistics.py` & `openbb_fmp-1.2.0/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/treasury_rates.py` & `openbb_fmp-1.2.0/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/models/world_news.py` & `openbb_fmp-1.2.0/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/utils/definitions.py` & `openbb_fmp-1.2.0/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/openbb_fmp/utils/helpers.py` & `openbb_fmp-1.2.0/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.5/PKG-INFO` & `openbb_fmp-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-fmp
-Version: 1.1.5
+Version: 1.2.0
 Summary: FMP extension for OpenBB
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
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Financial Modeling Prep Provider
 
 This extension integrates the [Financial Modeling Prep](https://site.financialmodelingprep.com/) data provider into the OpenBB Platform.
 
 ## Installation
 
 To install the extension:
 
 ```bash
 pip install openbb-fmp
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

