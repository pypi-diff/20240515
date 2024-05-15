# Comparing `tmp/graas-observability-utility-1.6.5.tar.gz` & `tmp/graas-observability-utility-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graas-observability-utility-1.6.5.tar", last modified: Tue May 14 08:18:22 2024, max compression
+gzip compressed data, was "graas-observability-utility-1.6.6.tar", last modified: Wed May 15 12:08:56 2024, max compression
```

## Comparing `graas-observability-utility-1.6.5.tar` & `graas-observability-utility-1.6.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-05-14 08:18:22.397628 graas-observability-utility-1.6.5/
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       43 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/MANIFEST.in
--rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-05-14 08:18:22.397628 graas-observability-utility-1.6.5/PKG-INFO
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      565 2023-11-02 10:15:21.000000 graas-observability-utility-1.6.5/README.md
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-05-14 08:18:22.365627 graas-observability-utility-1.6.5/graas_observability_utility.egg-info/
--rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-05-14 08:18:22.000000 graas-observability-utility-1.6.5/graas_observability_utility.egg-info/PKG-INFO
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4531 2024-05-14 08:18:22.000000 graas-observability-utility-1.6.5/graas_observability_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        1 2024-05-14 08:18:22.000000 graas-observability-utility-1.6.5/graas_observability_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       11 2024-05-14 08:18:22.000000 graas-observability-utility-1.6.5/graas_observability_utility.egg-info/requires.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       16 2024-05-14 08:18:22.000000 graas-observability-utility-1.6.5/graas_observability_utility.egg-info/top_level.txt
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-05-14 08:18:22.365627 graas-observability-utility-1.6.5/graas_utilities/
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-05-14 08:18:22.397628 graas-observability-utility-1.6.5/graas_utilities/Schema/
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4031 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2438 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5106 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5005 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3585 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3548 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3482 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1873 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2962 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1561 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2631 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2226 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2188 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1488 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3619 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5556 2024-05-14 08:17:20.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1694 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5961 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     9612 2024-04-02 10:30:41.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3743 2024-05-14 05:17:27.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4668 2024-04-16 08:59:10.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3926 2024-04-16 08:59:10.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3505 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3208 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1833 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1229 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1628 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1251 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2994 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1148 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2001 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1095 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5893 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6341 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6202 2024-05-14 05:26:30.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2479 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1429 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     8522 2024-04-05 10:52:26.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3500 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1531 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2362 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3318 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4650 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4115 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/__init__.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      577 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/amount_currency_code_object.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1785 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_amazon_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1301 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_flipkart_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1306 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1794 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_deals_overview_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2318 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_deals_trends_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1294 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_offsite_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1499 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_onsite_keywords.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2141 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_product_campaign_performance.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2700 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_shop_stats_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1554 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2454 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1330 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1851 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-11-27 05:46:40.000000 graas-observability-utility-1.6.5/graas_utilities/__init__.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5651 2024-04-16 09:00:32.000000 graas-observability-utility-1.6.5/graas_utilities/configs.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      751 2024-03-26 06:37:57.000000 graas-observability-utility-1.6.5/graas_utilities/ref_Resolver.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3986 2024-05-02 07:03:39.000000 graas-observability-utility-1.6.5/graas_utilities/validation.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       38 2024-05-14 08:18:22.397628 graas-observability-utility-1.6.5/setup.cfg
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1306 2024-05-14 08:17:31.000000 graas-observability-utility-1.6.5/setup.py
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-05-15 12:08:56.687487 graas-observability-utility-1.6.6/
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       43 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/MANIFEST.in
+-rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-05-15 12:08:56.687487 graas-observability-utility-1.6.6/PKG-INFO
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      565 2023-11-02 10:15:21.000000 graas-observability-utility-1.6.6/README.md
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-05-15 12:08:56.639487 graas-observability-utility-1.6.6/graas_observability_utility.egg-info/
+-rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-05-15 12:08:56.000000 graas-observability-utility-1.6.6/graas_observability_utility.egg-info/PKG-INFO
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4531 2024-05-15 12:08:56.000000 graas-observability-utility-1.6.6/graas_observability_utility.egg-info/SOURCES.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        1 2024-05-15 12:08:56.000000 graas-observability-utility-1.6.6/graas_observability_utility.egg-info/dependency_links.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       11 2024-05-15 12:08:56.000000 graas-observability-utility-1.6.6/graas_observability_utility.egg-info/requires.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       16 2024-05-15 12:08:56.000000 graas-observability-utility-1.6.6/graas_observability_utility.egg-info/top_level.txt
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-05-15 12:08:56.639487 graas-observability-utility-1.6.6/graas_utilities/
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-05-15 12:08:56.683487 graas-observability-utility-1.6.6/graas_utilities/Schema/
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4031 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2438 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5106 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5005 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3585 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3548 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3482 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1873 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2962 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1561 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2631 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2226 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2188 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1488 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3619 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5556 2024-05-14 08:17:20.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1694 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5961 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     9612 2024-04-02 10:30:41.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3743 2024-05-14 05:17:27.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4668 2024-04-16 08:59:10.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3926 2024-04-16 08:59:10.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3505 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3208 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1833 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1229 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1628 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1251 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2994 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1148 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2001 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1095 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5893 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6341 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6202 2024-05-14 05:26:30.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2479 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1429 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     8522 2024-04-05 10:52:26.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3500 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1531 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2362 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3318 2024-04-16 08:59:15.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4650 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4115 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/__init__.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      577 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/amount_currency_code_object.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1785 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_amazon_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1301 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_flipkart_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1306 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1794 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_deals_overview_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2318 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_deals_trends_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1294 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_offsite_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1499 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_onsite_keywords.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2141 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_product_campaign_performance.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2700 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_shop_stats_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1554 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2454 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1330 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1851 2023-12-24 13:53:23.000000 graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-11-27 05:46:40.000000 graas-observability-utility-1.6.6/graas_utilities/__init__.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5651 2024-04-16 09:00:32.000000 graas-observability-utility-1.6.6/graas_utilities/configs.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      751 2024-03-26 06:37:57.000000 graas-observability-utility-1.6.6/graas_utilities/ref_Resolver.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4598 2024-05-15 12:08:24.000000 graas-observability-utility-1.6.6/graas_utilities/validation.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       38 2024-05-15 12:08:56.687487 graas-observability-utility-1.6.6/setup.cfg
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1306 2024-05-15 12:08:27.000000 graas-observability-utility-1.6.6/setup.py
```

### Comparing `graas-observability-utility-1.6.5/PKG-INFO` & `graas-observability-utility-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graas-observability-utility
-Version: 1.6.5
+Version: 1.6.6
 Summary: A small wrapper around data observability
 Home-page: https://bitbucket.org/shoptimizeanalytics/graas-observability-utility
 Author: Graas
 Author-email: priyanka.patel@graas.ai
 Keywords: utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `graas-observability-utility-1.6.5/README.md` & `graas-observability-utility-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_observability_utility.egg-info/PKG-INFO` & `graas-observability-utility-1.6.6/graas_observability_utility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graas-observability-utility
-Version: 1.6.5
+Version: 1.6.6
 Summary: A small wrapper around data observability
 Home-page: https://bitbucket.org/shoptimizeanalytics/graas-observability-utility
 Author: Graas
 Author-email: priyanka.patel@graas.ai
 Keywords: utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `graas-observability-utility-1.6.5/graas_observability_utility.egg-info/SOURCES.txt` & `graas-observability-utility-1.6.6/graas_observability_utility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/amount_currency_code_object.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/amount_currency_code_object.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_amazon_campaigns.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_amazon_campaigns.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_flipkart_campaigns.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_flipkart_campaigns.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_deals_overview_daily.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_deals_overview_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_deals_trends_daily.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_deals_trends_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_offsite_campaigns.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_offsite_campaigns.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_onsite_keywords.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_onsite_keywords.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_product_campaign_performance.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_product_campaign_performance.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_shop_stats_daily.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_shop_stats_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json` & `graas-observability-utility-1.6.6/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/configs.py` & `graas-observability-utility-1.6.6/graas_utilities/configs.py`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/graas_utilities/ref_Resolver.py` & `graas-observability-utility-1.6.6/graas_utilities/ref_Resolver.py`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.6.5/setup.py` & `graas-observability-utility-1.6.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 	'Programming Language :: Python :: 3.3', 
 	'Programming Language :: Python :: 3.4', 
 	'Programming Language :: Python :: 3.8', 
 	]
 
 # calling the setup function 
 setup(name='graas-observability-utility', 
-	version='1.6.5', 
+	version='1.6.6', 
 	description='A small wrapper around data observability', 
 	# long_description=long_description, 
 	url='https://bitbucket.org/shoptimizeanalytics/graas-observability-utility', 
 	author='Graas', 
 	author_email='priyanka.patel@graas.ai', 
 	# license='MIT',
     packages=find_packages(),
```

