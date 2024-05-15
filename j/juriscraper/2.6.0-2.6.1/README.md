# Comparing `tmp/juriscraper-2.6.0.tar.gz` & `tmp/juriscraper-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juriscraper-2.6.0.tar", last modified: Thu Apr  4 01:09:20 2024, max compression
+gzip compressed data, was "juriscraper-2.6.1.tar", last modified: Wed May 15 18:07:33 2024, max compression
```

## Comparing `juriscraper-2.6.0.tar` & `juriscraper-2.6.1.tar`

### file list

```diff
@@ -1,447 +1,447 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.011596 juriscraper-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-04 01:09:07.000000 juriscraper-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 01:09:07.000000 juriscraper-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 01:09:07.000000 juriscraper-2.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-04 01:09:20.011596 juriscraper-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-04-04 01:09:07.000000 juriscraper-2.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.943596 juriscraper-2.6.0/juriscraper/
--rw-r--r--   0 runner    (1001) docker     (127)    17359 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/AbstractSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/DeferringList.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OpinionSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OpinionSiteLinear.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OpinionSiteLinearWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OpinionSiteWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OralArgumentSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OralArgumentSiteLinear.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OralArgumentSiteLinearWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/WebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.947597 juriscraper-2.6.0/juriscraper/fdsys/
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/fdsys/FDSysSite.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/fdsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/fdsys/scrape_court_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.947597 juriscraper-2.6.0/juriscraper/fdsys/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/fdsys/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/fdsys/utils/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/fdsys/utils/get_xpath_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.947597 juriscraper-2.6.0/juriscraper/lasc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lasc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lasc/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lasc/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.947597 juriscraper-2.6.0/juriscraper/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/cookie_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/diff_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/judge_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/log_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26813 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.951597 juriscraper-2.6.0/juriscraper/opinions/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/opinion_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.951597 juriscraper-2.6.0/juriscraper/opinions/united_states/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.951597 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/asbca.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/bia.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/bva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/mspb_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/mspb_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/olc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.955597 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca11_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca11_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca2_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca2_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca3_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca3_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca7.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca9_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca9_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cafc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_relating.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.955597 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.955597 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/dcd.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/ed_louisiana.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.959596 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/acca_memorandum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/acca_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/acca_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/afcca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/ag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/armfor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/cavc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/cit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/fisc.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/fiscr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/nmcca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscgcoca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.991596 juriscraper-2.6.0/juriscraper/opinions/united_states/state/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ala.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/alacivapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/alacrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/alaska.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/alaskactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ariz.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/arizctapp_div_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/arizctapp_div_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ark.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/arkctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/cal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calag.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_4th_div1.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_4th_div2.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_4th_div3.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_5th.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_6th.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_app_div.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/colo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/coloctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/conn.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/connappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/dc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/delaware.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/delch.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/delctcompl.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/delsuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fla.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/gactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/haw.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/haw_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/hawapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idaho_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idaho_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idahoctapp_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idahoctapp_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idahoctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/illappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ind.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/indctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/indtc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/iowa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/iowactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kan_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kan_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kanctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kanctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ky.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kyctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/la.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/lactapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/massappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/massappct_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/masslandct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mdag.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mdctspecapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/me.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mesuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mich.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/michctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/minn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnag.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/miss.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/miss_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/missctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mo.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/moctapp_eastern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/moctapp_southern.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/moctapp_western.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mont.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nc.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ncctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/neb.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nebctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nev.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nevapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nj.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/njsuperctappdiv_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/njsuperctappdiv_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/njtaxct_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/njtaxct_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nm.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nmctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ny.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_4th.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappterm_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappterm_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nycityct.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nycivct.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyclaimsct.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nycountyct.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nycrimct.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nydistct.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyfamct.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyjustct.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nysupct.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nysupct_commercial.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nysurct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nytrial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohio.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_11.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_12.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_7.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_9.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctcl.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/okla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklaag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklacivapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklacrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/or.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/orctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/pa.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/pacommwct.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/pasuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ri_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ri_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/sc.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/scctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/sd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/tenn.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/tenncrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/tennctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/tex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texag.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_11.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_12.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_13.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_7.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_9.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texcrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/utah.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/utahctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/va.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vactapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vactapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vt.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vt_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vtsuperct_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vtsuperct_environmental.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vtsuperct_family.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vtsuperct_probate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/washctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/washctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wva.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wvactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wyo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.991596 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/as.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/guam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/nmariana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/prapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/prsupreme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/virginislands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/visuper_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/visuper_u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.991596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.991596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.995596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.995596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.999596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2011.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.999596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/cal_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/indctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/indtc.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/me.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/me_2013.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ny.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/sd.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.003596 juriscraper-2.6.0/juriscraper/oral_args/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/oral_argument_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.003596 juriscraper-2.6.0/juriscraper/oral_args/united_states/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.003596 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca11.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca7.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca9.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/cadc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/cafc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/scotus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.003596 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_1st_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_2nd_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_3rd_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_4th_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_5th_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_workers_comp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/md.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.007596 juriscraper-2.6.0/juriscraper/pacer/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/acms_docket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/appellate_attachment_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    30499 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/appellate_docket.py
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/attachment_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/case_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/case_query_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/claims_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/claims_register.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/docket_history_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    63103 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/docket_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/docket_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/download_confirmation_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    34933 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/email.py
--rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/free_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/hidden_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/internet_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/list_of_creditors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/mobile_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/rss_feeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacerdocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.007596 juriscraper-2.6.0/juriscraper/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.007596 juriscraper-2.6.0/juriscraper/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.007596 juriscraper-2.6.0/juriscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22388 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-04 01:09:08.000000 juriscraper-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 01:09:08.000000 juriscraper-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-04 01:09:20.011596 juriscraper-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-04 01:09:08.000000 juriscraper-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.421362 juriscraper-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-15 18:07:24.000000 juriscraper-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 18:07:24.000000 juriscraper-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 18:07:24.000000 juriscraper-2.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-15 18:07:33.421362 juriscraper-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-05-15 18:07:24.000000 juriscraper-2.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.353362 juriscraper-2.6.1/juriscraper/
+-rw-r--r--   0 runner    (1001) docker     (127)    17359 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/AbstractSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/DeferringList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/OpinionSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/OpinionSiteLinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/OpinionSiteLinearWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/OpinionSiteWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/OralArgumentSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/OralArgumentSiteLinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/OralArgumentSiteLinearWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/WebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.353362 juriscraper-2.6.1/juriscraper/fdsys/
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/fdsys/FDSysSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/fdsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/fdsys/scrape_court_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.357362 juriscraper-2.6.1/juriscraper/fdsys/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/fdsys/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/fdsys/utils/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/fdsys/utils/get_xpath_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.357362 juriscraper-2.6.1/juriscraper/lasc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lasc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lasc/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lasc/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.357362 juriscraper-2.6.1/juriscraper/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/cookie_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/diff_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/judge_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/log_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26813 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.357362 juriscraper-2.6.1/juriscraper/opinions/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/opinion_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.357362 juriscraper-2.6.1/juriscraper/opinions/united_states/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.361362 juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/asbca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/bia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/bva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/mspb_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/mspb_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/olc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.361362 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca11_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca11_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca2_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca2_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca3_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca3_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca9_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca9_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/cadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/cadc_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/cafc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/scotus_relating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.365362 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_bankruptcy/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_bankruptcy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.365362 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_district/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_district/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_district/dcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_district/ed_louisiana.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.365362 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/acca_memorandum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/acca_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/acca_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/afcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/ag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/armfor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/cavc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/cit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/fisc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/fiscr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/nmcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscfc_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscgcoca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.401362 juriscraper-2.6.1/juriscraper/opinions/united_states/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ala.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/alacivapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/alacrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/alaska.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/alaskactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ariz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/arizctapp_div_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/arizctapp_div_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/arkctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_4th_div1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_4th_div2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_4th_div3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_5th.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_6th.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_app_div.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/calctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/colo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/coloctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/connappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/delaware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/delch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/delctcompl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/delsuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/fla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/gactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/haw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/haw_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/hawapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/idaho_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/idaho_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/idahoctapp_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/idahoctapp_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/idahoctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/illappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/indctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/indtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/iowa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/iowactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/kan_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/kan_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/kanctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/kanctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ky.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/kyctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/la.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/lactapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/massappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/massappct_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/masslandct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/mdag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/mdctspecapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/mesuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/mich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/michctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/minn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/minnag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/minnctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/minnctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/miss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/miss_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/missctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/moctapp_eastern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/moctapp_southern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/moctapp_western.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/mont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ncctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nebctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nevapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/njsuperctappdiv_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/njsuperctappdiv_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/njtaxct_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/njtaxct_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nmctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyappdiv_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyappdiv_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyappdiv_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyappdiv_4th.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyappterm_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyappterm_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nycityct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nycivct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyclaimsct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nycountyct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nycrimct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nydistct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyfamct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyjustct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nysupct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nysupct_commercial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nysurct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/nytrial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctapp_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/okla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/oklaag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/oklacivapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/oklacrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/or.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/orctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/pa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/pacommwct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/pasuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ri_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/ri_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/scctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/sd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/tenn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/tenncrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/tennctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/tex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texapp_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/texcrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/utah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/utahctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/va.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/vactapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/vactapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/vt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/vt_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/vtsuperct_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/vtsuperct_environmental.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/vtsuperct_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/vtsuperct_probate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/wash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/washctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/washctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/wis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/wva.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/wvactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/state/wyo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.401362 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/as.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/guam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/nmariana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/prapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/prsupreme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/virginislands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/visuper_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states/territories/visuper_u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.405362 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.405362 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/administrative_agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.405362 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.405362 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.409362 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-15 18:07:24.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.413362 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/cal_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/illappct_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/illappct_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/illappct_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/illappct_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/illappct_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/ind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/indctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/indtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/me.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/me_2013.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/ny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/sd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.413362 juriscraper-2.6.1/juriscraper/oral_args/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/oral_argument_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.413362 juriscraper-2.6.1/juriscraper/oral_args/united_states/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.413362 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/cadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/cafc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/scotus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.417362 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/illappct_1st_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/illappct_2nd_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/illappct_3rd_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/illappct_4th_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/illappct_5th_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/illappct_workers_comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/oral_args/united_states/state/md.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.421362 juriscraper-2.6.1/juriscraper/pacer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/acms_docket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/appellate_attachment_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30499 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/appellate_docket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/attachment_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/case_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/case_query_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/claims_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/claims_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/docket_history_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63103 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/docket_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/docket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/download_confirmation_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35043 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/free_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/hidden_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/internet_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/list_of_creditors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/mobile_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/rss_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacer/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/pacerdocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.421362 juriscraper-2.6.1/juriscraper/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.421362 juriscraper-2.6.1/juriscraper/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:25.000000 juriscraper-2.6.1/juriscraper/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:07:33.421362 juriscraper-2.6.1/juriscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-15 18:07:33.000000 juriscraper-2.6.1/juriscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22388 2024-05-15 18:07:33.000000 juriscraper-2.6.1/juriscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:07:33.000000 juriscraper-2.6.1/juriscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 18:07:33.000000 juriscraper-2.6.1/juriscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 18:07:33.000000 juriscraper-2.6.1/juriscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-15 18:07:25.000000 juriscraper-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 18:07:25.000000 juriscraper-2.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 18:07:33.421362 juriscraper-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-15 18:07:25.000000 juriscraper-2.6.1/setup.py
```

### Comparing `juriscraper-2.6.0/LICENSE` & `juriscraper-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/PKG-INFO` & `juriscraper-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juriscraper
-Version: 2.6.0
+Version: 2.6.1
 Summary: An API to scrape American court websites for metadata.
 Home-page: https://github.com/freelawproject/juriscraper
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 License: BSD
```

### Comparing `juriscraper-2.6.0/README.rst` & `juriscraper-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/AbstractSite.py` & `juriscraper-2.6.1/juriscraper/AbstractSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/DeferringList.py` & `juriscraper-2.6.1/juriscraper/DeferringList.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/OpinionSite.py` & `juriscraper-2.6.1/juriscraper/OpinionSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/OpinionSiteLinear.py` & `juriscraper-2.6.1/juriscraper/OpinionSiteLinear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/OralArgumentSite.py` & `juriscraper-2.6.1/juriscraper/OralArgumentSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/OralArgumentSiteLinear.py` & `juriscraper-2.6.1/juriscraper/OralArgumentSiteLinear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/WebDriven.py` & `juriscraper-2.6.1/juriscraper/WebDriven.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/fdsys/FDSysSite.py` & `juriscraper-2.6.1/juriscraper/fdsys/FDSysSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/fdsys/scrape_court_names.py` & `juriscraper-2.6.1/juriscraper/fdsys/scrape_court_names.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/fdsys/utils/get_metadata.py` & `juriscraper-2.6.1/juriscraper/fdsys/utils/get_metadata.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/fdsys/utils/get_xpath_results.py` & `juriscraper-2.6.1/juriscraper/fdsys/utils/get_xpath_results.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lasc/fetch.py` & `juriscraper-2.6.1/juriscraper/lasc/fetch.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lasc/http.py` & `juriscraper-2.6.1/juriscraper/lasc/http.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/cookie_utils.py` & `juriscraper-2.6.1/juriscraper/lib/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/date_utils.py` & `juriscraper-2.6.1/juriscraper/lib/date_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/diff_tools.py` & `juriscraper-2.6.1/juriscraper/lib/diff_tools.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/exceptions.py` & `juriscraper-2.6.1/juriscraper/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/html_utils.py` & `juriscraper-2.6.1/juriscraper/lib/html_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/importer.py` & `juriscraper-2.6.1/juriscraper/lib/importer.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/judge_parsers.py` & `juriscraper-2.6.1/juriscraper/lib/judge_parsers.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/log_tools.py` & `juriscraper-2.6.1/juriscraper/lib/log_tools.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/network_utils.py` & `juriscraper-2.6.1/juriscraper/lib/network_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/string_utils.py` & `juriscraper-2.6.1/juriscraper/lib/string_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/test_utils.py` & `juriscraper-2.6.1/juriscraper/lib/test_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/lib/utils.py` & `juriscraper-2.6.1/juriscraper/lib/utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/opinion_template.py` & `juriscraper-2.6.1/juriscraper/opinions/opinion_template.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/asbca.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/asbca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/bia.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/bia.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/bva.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/bva.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/mspb_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/mspb_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/mspb_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/administrative_agency/mspb_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca1.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca10.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca11_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca11_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca11_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca11_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca2_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca2_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca2_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca2_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca3_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca3_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca4.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca4.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca5.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca6.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca6.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca7.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca7.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca8.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca8.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca9_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca9_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca9_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/ca9_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/cadc_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cafc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/cafc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/dcd.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_district/dcd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/acca_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/acca_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/afcca.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/ag.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-"""Scraper for the Air Force Court of Criminal Appeals
-CourtID: afcca
-Court Short Name: Air Force Court of Criminal Appeals
-Reviewer: mlr
-History:
-    15 Sep 2014: Created by Jon Andersen
+"""Scraper for the United States Department of Justice Attorney General
+CourtID: ag
+Court Short Name: United States Attorney General
 """
-
-from datetime import date
-
 from juriscraper.OpinionSiteLinear import OpinionSiteLinear
 
 
 class Site(OpinionSiteLinear):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        self.url_base = "http://afcca.law.af.mil/content/opinions_date_%d.html"
-        self.url = self.url_base % date.today().year
-        self.disable_certificate_verification()
+        self.url = "https://www.justice.gov/olc/opinions?items_per_page=40"
+        self.status = "Published"
 
     def _process_html(self):
-        for row in self.html.xpath(".//img[contains(@src, 'pdf.gif')]/../..")[
-            :-1
-        ]:
-            status = row.xpath(".//td")[3].text_content()
-            if status != "Published":
-                status = "Unpublished"
+        for row in self.html.xpath(".//article"):
+            name = row.xpath(".//h2")[0].text_content().strip()
+            url = row.xpath(".//a/@href")[0]
+            date = row.xpath(".//time")[0].text_content()
+            if not name:
+                continue
+            summary = row.xpath(".//p")[0].text_content()
             self.cases.append(
                 {
-                    "url": row.xpath(".//td/a/@href")[0],
-                    "docket": row.xpath(".//td")[2].text_content(),
-                    "name": row.xpath(".//td/a")[0].text_content(),
-                    "date": row.xpath(".//td")[4].text_content(),
-                    "status": status,
+                    "date": date,
+                    "name": name,
+                    "url": url,
+                    "summary": summary,
+                    "docket": "",  # Docket numbers don't appear to exist.
                 }
             )
```

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/ag.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/vactapp_u.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-"""Scraper for the United States Department of Justice Attorney General
-CourtID: ag
-Court Short Name: United States Attorney General
-"""
 from juriscraper.OpinionSiteLinear import OpinionSiteLinear
 
 
 class Site(OpinionSiteLinear):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        self.url = "https://www.justice.gov/olc/opinions?items_per_page=40"
-        self.status = "Published"
+        self.url = "https://www.vacourts.gov/wpcau.htm"
+        self.status = "Unpublished"
 
     def _process_html(self):
-        for row in self.html.xpath(".//article"):
-            name = row.xpath(".//h2")[0].text_content().strip()
-            url = row.xpath(".//a/@href")[0]
-            date = row.xpath(".//time")[0].text_content()
+        for row in self.html.xpath("//p"):
+            links = row.xpath(".//a")
+            name = row.xpath(".//b/text()")
             if not name:
                 continue
-            summary = row.xpath(".//p")[0].text_content()
+            date, disposition, *_ = row.text_content().splitlines()
+            date = date.split(name[0])[1]
             self.cases.append(
                 {
-                    "date": date,
-                    "name": name,
-                    "url": url,
-                    "summary": summary,
-                    "docket": "",  # Docket numbers don't appear to exist.
+                    "name": name[0].strip(),
+                    "docket": links[0].get("href").split("/")[-1][:-4],
+                    "url": links[0].get("href"),
+                    "disposition": disposition,
+                    "date": date.strip(),
                 }
             )
```

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/armfor.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/armfor.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/cavc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/cavc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/cit.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/cit.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/fisc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/fisc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/nmcca.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/nmcca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/tax.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/tax.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscfc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscfc_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscgcoca.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/federal_special/uscgcoca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/__init__.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/__init__.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ala.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ala.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/alaska.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/alaska.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ariz.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ariz.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/arizctapp_div_2.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/arizctapp_div_2.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ark.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ark.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/cal.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,72 @@
-import re
+"""
+Scraper for Indiana Supreme Court archive before 6/6/2005
+CourtID: ind
+Court Short Name: Ind.
+Auth: Mike Lissner <mike@freelawproject.org>
+Reviewer:
+History:
+    2014-09-03: Renamed to ind_2005.py by janderse
+"""
+import time
+from datetime import date
+
+from lxml import html
 
-from juriscraper.lib.string_utils import convert_date_string
 from juriscraper.OpinionSite import OpinionSite
 
 
 class Site(OpinionSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.url = "http://www.in.gov/judiciary/opinions/previous/archsup.html"
         self.court_id = self.__module__
-        self.court_code = "S"
-
-    def _download(self, request_dict={}):
-        if not self.test_mode_enabled():
-            self.url = self.build_url()
-        return super()._download(request_dict)
-
-    def build_url(self):
-        return (
-            "http://www.courts.ca.gov/cms/opinions.htm?Courts=%s"
-            % self.court_code
-        )
 
     def _get_case_names(self):
-        case_names = []
-        for cell in self.html.xpath("//table/tr/td[3]"):
-            name = cell.text_content()
-            date_regex = re.compile(r" \d\d?/\d\d?/\d\d| filed")
-            if "P. v. " in date_regex.split(name)[0]:
-                case_names.append(
-                    date_regex.split(name)[0].replace("P. ", "People ")
+        return [e for e in self.html.xpath("//table/tr/td[1]/font/a/text()")]
+
+    def _get_case_dates(self):
+        dates = []
+        for link_string in self.html.xpath("//table/tr/td[4]/font/a/@href"):
+            date_string = link_string.split("/")[-1].split(".")[0][:-2]
+            if date_string == "12319701-fs":
+                # special case (there's always *one*)
+                dates.append(
+                    date.fromtimestamp(
+                        time.mktime(time.strptime("123197", "%m%d%y"))
+                    )
+                )
+            elif len(date_string) == 4:
+                dates.append(
+                    date.fromtimestamp(
+                        time.mktime(
+                            time.strptime(f"{date_string}98", "%m%d%y")
+                        )
+                    )
+                )
+            elif len(date_string) == 5:
+                dates.append(
+                    date.fromtimestamp(
+                        time.mktime(time.strptime(f"0{date_string}", "%m%d%y"))
+                    )
+                )
+            elif len(date_string) == 6:
+                dates.append(
+                    date.fromtimestamp(
+                        time.mktime(time.strptime(date_string, "%m%d%y"))
+                    )
                 )
             else:
-                case_names.append(date_regex.split(name)[0])
-        return case_names
+                print(date_string)
+        return dates
 
     def _get_download_urls(self):
-        return [
-            t
-            for t in self.html.xpath(
-                "//table/tr/td[2]/a/@href[contains(.,'PDF')]"
-            )
-        ]
+        return [s for s in self.html.xpath("//table/tr/td[4]/font/a/@href")]
 
-    def _get_case_dates(self):
-        path = "//table/tr/td[1]/text()"
+    def _get_docket_numbers(self):
         return [
-            convert_date_string(date_string)
-            for date_string in self.html.xpath(path)
+            html.tostring(e, method="text")
+            for e in self.html.xpath("//table/tr/td[2]")
         ]
 
-    def _get_docket_numbers(self):
-        return [t for t in self.html.xpath("//table/tr/td[2]/text()[1]")]
-
     def _get_precedential_statuses(self):
         return ["Published"] * len(self.case_names)
```

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/calag.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/calag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_1st.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,26 @@
-# Scraper for California's First District Court of Appeal
-# CourtID: calctapp_1st
-# Court Short Name: Cal. Ct. App.
+"""Backscraper for Dept of Justice Office of Legal Counsel
+CourtID: olc
+Court Short Name: OLC
+Author: William E. Palin
+History:
+    2022-01-14: Created by William E. Palin
+"""
 
-from juriscraper.opinions.united_states.state import cal
+from juriscraper.opinions.united_states.administrative_agency import olc
 
 
-class Site(cal.Site):
+class Site(olc.Site):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        self.court_code = "A"
-        self.division = "1st App. Dist."
-        self.url = self.build_url()
+        self.back_scrape_iterable = range(1, 36)
 
-    def _get_divisions(self):
-        return [self.division] * len(self.case_names)
+    def _download_backwards(self, page: int) -> None:
+        """Download backwards over the volume links in the DOJ OLC website.
+
+        :param page: The page index for the URL
+        :return: None
+        """
+        self.url = f"https://www.justice.gov/olc/opinions?items_per_page=40&page={page}"
+        self.html = self._download()
+        self._process_html()
```

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/colo.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/colo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/coloctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/coloctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/conn.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/conn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/connappct.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/connappct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/dc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/dc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/delaware.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/delaware.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/fla.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/pa.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,77 @@
-# Scraper for Florida Supreme Court
-# CourtID: fla
-# Court Short Name: fla
-
-from datetime import datetime
+"""
+Scraper for Pennsylvania Supreme Court
+CourtID: pa
+Court Short Name: pa
+"""
+import re
 
+from juriscraper.lib.html_utils import get_xml_parsed_text
 from juriscraper.lib.string_utils import convert_date_string
-from juriscraper.OpinionSite import OpinionSite
+from juriscraper.OpinionSiteLinear import OpinionSiteLinear
 
 
-class Site(OpinionSite):
+class Site(OpinionSiteLinear):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        today = datetime.today().strftime("%m/%d/%Y")
-        this_year = datetime.today().year
-        last_year = this_year - 1
-        today_last_year = today.replace(str(this_year), str(last_year))
-        # Get 50 most recent opinions from past year--even though you can
-        # put whatever number you want as limit, 50 seems to be max
-        self.url = (
-            "https://www.floridasupremecourt.org/search/?searchtype=opinions&limit=50&startdate=%s&enddate=%s"
-            % (today_last_year, today)
+        self.regex = False
+        self.url = "https://www.pacourts.us/Rss/Opinions/Supreme/"
+        self.set_regex(r"(.*)(?:[,-]?\s+Nos?\.)(.*)")
+        self.base = (
+            "//item[not(contains(title/text(), 'Judgment List'))]"
+            "[not(contains(title/text(), 'Reargument Table'))]"
+            "[not(contains(title/text(), 'Order Amending Rules'))]"
+            "[contains(title/text(), 'No.')]"
         )
-        self.path_cell = '//div[@class="search-results"]//tr/td[%d]'
         self.cases = []
 
-    def _download(self, request_dict={}):
-        html = super()._download(request_dict)
-        self._extract_cases_from_html(html)
-        return html
-
-    def _extract_cases_from_html(self, html):
-        path = '//div[@class="search-results"]//tbody/tr'
-        for row in html.xpath(path):
-            cells = row.xpath("./td")
-            url = cells[4].xpath("./a/@href")
-            if not url:
-                # Skip rows without PDFs
-                continue
+    def _make_html_tree(self, text):
+        return get_xml_parsed_text(text)
+
+    def _process_html(self):
+        for item in self.html.xpath(self.base):
+            judges = item.xpath(
+                "./dc:creator/text()", namespaces=self.html.nsmap
+            )
+            pubdate = item.xpath("./pubDate/text()")[0]
+            title = item.xpath("./title/text()")[0]
+            search = self.regex.search(title)
+            url = item.xpath("./atom:link/@href", namespaces=self.html.nsmap)[
+                0
+            ]
+            if search:
+                name = search.group(1)
+                docket = search.group(2)
+            else:
+                name = title
+                docket = ""
             self.cases.append(
                 {
-                    "url": url[0],
-                    "name": cells[2].text_content(),
-                    "docket": cells[1].text_content(),
-                    "date": convert_date_string(cells[0].text_content()),
+                    "name": name,
+                    "date": convert_date_string(pubdate),
+                    "docket": docket,
+                    "judge": judges[0] if judges else "",
+                    "url": url,
                 }
             )
 
     def _get_case_names(self):
         return [case["name"] for case in self.cases]
 
     def _get_download_urls(self):
         return [case["url"] for case in self.cases]
 
     def _get_case_dates(self):
         return [case["date"] for case in self.cases]
 
+    def _get_precedential_statuses(self):
+        return ["Published"] * len(self.cases)
+
     def _get_docket_numbers(self):
         return [case["docket"] for case in self.cases]
 
-    def _get_precedential_statuses(self):
-        return ["Published"] * len(self.cases)
+    def _get_judges(self):
+        return [case["judge"] for case in self.cases]
+
+    def set_regex(self, pattern):
+        self.regex = re.compile(pattern)
```

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_5.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/fladistctapp_5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ga.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ga.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/gactapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/gactapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/haw.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/haw.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/haw_beginningofyear.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/haw_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/idaho_civil.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/idaho_civil.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/idahoctapp_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/idahoctapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ind.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ind.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/iowa.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/iowa.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/iowactapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/iowactapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/kan_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/kan_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ky.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ky.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/kyctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/kyctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/la.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/la.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/lactapp_1.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/lactapp_1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mass.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/mass.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/massappct_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/massappct_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/masslandct.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/masslandct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/md.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/md.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mdag.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/mdag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mdctspecapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/mdctspecapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/me.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/me.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mesuperct.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/mesuperct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mich.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/mich.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/michctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/michctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/minn.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/minn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnag.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/minnag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnctapp_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/minnctapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/miss.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/miss.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/miss_beginningofyear.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/miss_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mo.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/mo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/moctapp_southern.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/moctapp_southern.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mont.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/mont.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ncctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ncctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nd.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/neb.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/neb.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nev.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nev.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nevapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nevapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nh.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nh.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nj.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nj.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nm.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nm.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ny.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ny.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyag.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_1st.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nyappdiv_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nytrial.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/nytrial.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohio.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohio.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/okla.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/okla.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklaag.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/oklaag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklacivapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/oklacivapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklacrimapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/oklacrimapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/orctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/orctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/pa.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/wyo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,60 @@
+"""Scraper for Wyoming Supreme Court
+CourtID: wyo
+Court Short Name: Wyo.
+History:
+ - 2014-07-02: mlr: Created new version when court got new website.
+ - 2015-07-06: m4h7: Updated to use JSON!
+ - 2016-06-09: arderyp: Updated because json endpoint moved and was changed
 """
-Scraper for Pennsylvania Supreme Court
-CourtID: pa
-Court Short Name: pa
-"""
+
 import re
+from datetime import date, datetime
 
-from juriscraper.lib.html_utils import get_xml_parsed_text
-from juriscraper.lib.string_utils import convert_date_string
-from juriscraper.OpinionSiteLinear import OpinionSiteLinear
+from juriscraper.OpinionSite import OpinionSite
 
 
-class Site(OpinionSiteLinear):
+class Site(OpinionSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        self.regex = False
-        self.url = "https://www.pacourts.us/Rss/Opinions/Supreme/"
-        self.set_regex(r"(.*)(?:[,-]?\s+Nos?\.)(.*)")
-        self.base = (
-            "//item[not(contains(title/text(), 'Judgment List'))]"
-            "[not(contains(title/text(), 'Reargument Table'))]"
-            "[not(contains(title/text(), 'Order Amending Rules'))]"
-            "[contains(title/text(), 'No.')]"
+        self.base_url = "http://www.courts.state.wy.us"
+        self.download_base = "https://documents.courts.state.wy.us/Opinions"
+        self.url = (
+            "https://opinions.courts.state.wy.us/Home/GetOpinions?StartDate=1%2F1%2F"
+            + str(date.today().year)
         )
-        self.cases = []
-
-    def _make_html_tree(self, text):
-        return get_xml_parsed_text(text)
-
-    def _process_html(self):
-        for item in self.html.xpath(self.base):
-            judges = item.xpath(
-                "./dc:creator/text()", namespaces=self.html.nsmap
-            )
-            pubdate = item.xpath("./pubDate/text()")[0]
-            title = item.xpath("./title/text()")[0]
-            search = self.regex.search(title)
-            url = item.xpath("./atom:link/@href", namespaces=self.html.nsmap)[
-                0
-            ]
-            if search:
-                name = search.group(1)
-                docket = search.group(2)
-            else:
-                name = title
-                docket = ""
-            self.cases.append(
-                {
-                    "name": name,
-                    "date": convert_date_string(pubdate),
-                    "docket": docket,
-                    "judge": judges[0] if judges else "",
-                    "url": url,
-                }
-            )
 
     def _get_case_names(self):
-        return [case["name"] for case in self.cases]
+        return [
+            f"{opinion['Appellant']} v. {opinion['Appellee']}"
+            for opinion in self.html
+        ]
 
     def _get_download_urls(self):
-        return [case["url"] for case in self.cases]
+        download_urls = []
+        for record in self.html:
+            pdf_file_name = record["DocumentName"]
+            if pdf_file_name[:5] == "../..":
+                pdf_file_name = pdf_file_name[5:]
+            url = f"{self.download_base}/{pdf_file_name}".replace(" ", "%20")
+            download_urls.append(url)
+        return download_urls
 
     def _get_case_dates(self):
-        return [case["date"] for case in self.cases]
-
-    def _get_precedential_statuses(self):
-        return ["Published"] * len(self.cases)
+        case_dates = []
+        date_re = re.compile(r"^/Date\((\d+)\)/$")
+        for record in self.html:
+            match = date_re.match(record["date_heard"])
+            if match:
+                timestamp = int(match.group(1)) / 1000
+                case_dates.append(datetime.fromtimestamp(timestamp).date())
+        return case_dates
 
     def _get_docket_numbers(self):
-        return [case["docket"] for case in self.cases]
+        return [opinion["DocketNumber"] for opinion in self.html]
 
-    def _get_judges(self):
-        return [case["judge"] for case in self.cases]
+    def _get_citations(self):
+        return [opinion["OpinionID"] for opinion in self.html]
 
-    def set_regex(self, pattern):
-        self.regex = re.compile(pattern)
+    def _get_precedential_statuses(self):
+        return ["Published"] * len(self.case_names)
```

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/pacommwct.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/pacommwct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ri_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ri_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ri_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/ri_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/sc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/sc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/scctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/scctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/sd.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/sd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/tenn.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/tenn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/tex.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/tex.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/texag.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/texag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/utah.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/utah.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/utahctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/utahctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/va.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/va.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/vactapp_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/vactapp_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/vactapp_u.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/territories/visuper_p.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,41 @@
+# Scraper for Superior Court of the Virgin Islands (published)
+# CourtID: visuper_p
+
 from juriscraper.OpinionSiteLinear import OpinionSiteLinear
 
 
 class Site(OpinionSiteLinear):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        self.url = "https://www.vacourts.gov/wpcau.htm"
-        self.status = "Unpublished"
+        self.url = (
+            "https://superior.vicourts.org/court_opinions/published_opinions"
+        )
+        self.status = "Published"
+
+    def _process_html(self) -> None:
+        """Parse HTML into case objects
 
-    def _process_html(self):
-        for row in self.html.xpath("//p"):
-            links = row.xpath(".//a")
-            name = row.xpath(".//b/text()")
-            if not name:
-                continue
-            date, disposition, *_ = row.text_content().splitlines()
-            date = date.split(name[0])[1]
+        :return: None
+        """
+        row_xpath = ".//tbody//tr[.//a[text() and not(@title='Summary')]]"
+        for row in self.html.xpath(row_xpath):
+            (
+                case_name,
+                date_filed,
+                docket_number,
+                judge,
+                citation,
+                _summary,
+            ) = row.xpath(".//td//text()")
+            url = row.xpath(".//td/a")[0].get("href")
             self.cases.append(
                 {
-                    "name": name[0].strip(),
-                    "docket": links[0].get("href").split("/")[-1][:-4],
-                    "url": links[0].get("href"),
-                    "disposition": disposition,
-                    "date": date.strip(),
+                    "date": date_filed,
+                    "docket": docket_number,
+                    "name": case_name,
+                    "url": url,
+                    "judge": judge,
+                    "citation": citation,
                 }
             )
```

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/vt.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/vt.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/wash.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/wash.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/washctapp_p.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/washctapp_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/wis.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/wis.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/wva.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/state/wva.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/state/wyo.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/cadc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,62 @@
-"""Scraper for Wyoming Supreme Court
-CourtID: wyo
-Court Short Name: Wyo.
-History:
- - 2014-07-02: mlr: Created new version when court got new website.
- - 2015-07-06: m4h7: Updated to use JSON!
- - 2016-06-09: arderyp: Updated because json endpoint moved and was changed
+"""Scraper for D.C. Circuit of Appeals
+CourtID: cadc
+Court Short Name: cadc
+Author: Andrei Chelaru
+Reviewer: mlr
+Date created: 18 July 2014
 """
 
-import re
 from datetime import date, datetime
 
-from juriscraper.OpinionSite import OpinionSite
+from juriscraper.OralArgumentSite import OralArgumentSite
 
 
-class Site(OpinionSite):
+class Site(OralArgumentSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        self.base_url = "http://www.courts.state.wy.us"
-        self.download_base = "https://documents.courts.state.wy.us/Opinions"
-        self.url = (
-            "https://opinions.courts.state.wy.us/Home/GetOpinions?StartDate=1%2F1%2F"
-            + str(date.today().year)
+        d = date.today()
+        # d = date(month=5, day=1, year=2014)
+        self.url = "http://www.cadc.uscourts.gov/recordings/recordings.nsf/DocsByRDate?OpenView&count=100&SKey={yearmo}".format(
+            yearmo=d.strftime("%Y%m")
         )
-
-    def _get_case_names(self):
-        return [
-            f"{opinion['Appellant']} v. {opinion['Appellee']}"
-            for opinion in self.html
+        self.back_scrape_iterable = [
+            "%s%02d" % (year, month)
+            for year in range(2007, d.year + 1)
+            for month in range(1, 13)
         ]
 
+    def _download(self, **kwargs):
+        # The certificate on their site has expired.
+        return super()._download(request_dict={"verify": False})
+
     def _get_download_urls(self):
-        download_urls = []
-        for record in self.html:
-            pdf_file_name = record["DocumentName"]
-            if pdf_file_name[:5] == "../..":
-                pdf_file_name = pdf_file_name[5:]
-            url = f"{self.download_base}/{pdf_file_name}".replace(" ", "%20")
-            download_urls.append(url)
-        return download_urls
+        path = "id('ViewBody')//div[contains(concat(' ',@class,' '),' row-entry')]//@href"
+        return list(self.html.xpath(path))
+
+    def _get_case_names(self):
+        path = "id('ViewBody')//*[contains(concat(' ',@class,' '),' column-two')]/div[1]/text()"
+        return list(self.html.xpath(path))
 
     def _get_case_dates(self):
-        case_dates = []
-        date_re = re.compile(r"^/Date\((\d+)\)/$")
-        for record in self.html:
-            match = date_re.match(record["date_heard"])
-            if match:
-                timestamp = int(match.group(1)) / 1000
-                case_dates.append(datetime.fromtimestamp(timestamp).date())
-        return case_dates
+        path = "id('ViewBody')//date/text()"
+        return list(map(self._return_case_date, self.html.xpath(path)))
 
-    def _get_docket_numbers(self):
-        return [opinion["DocketNumber"] for opinion in self.html]
+    @staticmethod
+    def _return_case_date(e):
+        e = "".join(e.split())
+        return datetime.strptime(e, "%m/%d/%Y").date()
 
-    def _get_citations(self):
-        return [opinion["OpinionID"] for opinion in self.html]
+    def _get_docket_numbers(self):
+        path = "id('ViewBody')//*[contains(concat(' ',@class,' '),' row-entry')]//a//text()"
+        return list(self.html.xpath(path))
 
-    def _get_precedential_statuses(self):
-        return ["Published"] * len(self.case_names)
+    def _get_judges(self):
+        path = '//div[span[contains(., "Judges")]]/text()'
+        return [" ".join(s.split()) for s in self.html.xpath(path)]
+
+    def _download_backwards(self, yearmo):
+        self.url = "http://www.cadc.uscourts.gov/recordings/recordings.nsf/DocsByRDate?OpenView&count=100&SKey={yearmo}".format(
+            yearmo=yearmo,
+        )
+        self.html = self._download()
```

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/guam.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/territories/guam.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/nmariana.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/territories/nmariana.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/prapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/territories/prapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/prsupreme.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/territories/prsupreme.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/virginislands.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states/territories/virginislands.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ill.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ind.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/ind.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/indctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/indctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/me.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/me.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/me_2013.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/me_2013.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nd.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/nd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/sd.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/sd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py` & `juriscraper-2.6.1/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/oral_argument_template.py` & `juriscraper-2.6.1/juriscraper/oral_args/oral_argument_template.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca1.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca10.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca11.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca11.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca2.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca2.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca3.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca4.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca4.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca5.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca6.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca6.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca7.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca7.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca8.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca8.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca9.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/ca9.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/cadc.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/scotus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,55 @@
-"""Scraper for D.C. Circuit of Appeals
-CourtID: cadc
-Court Short Name: cadc
-Author: Andrei Chelaru
-Reviewer: mlr
-Date created: 18 July 2014
+"""Scraper for Supreme Court of U.S.
+CourtID: scotus
+Court Short Name: scotus
+History:
+ - 2014-07-20 - Created by Andrei Chelaru, reviewed by MLR
+ - 2017-10-09 - Updated by MLR.
 """
 
-from datetime import date, datetime
+from datetime import datetime
 
 from juriscraper.OralArgumentSite import OralArgumentSite
 
 
 class Site(OralArgumentSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        d = date.today()
-        # d = date(month=5, day=1, year=2014)
-        self.url = "http://www.cadc.uscourts.gov/recordings/recordings.nsf/DocsByRDate?OpenView&count=100&SKey={yearmo}".format(
-            yearmo=d.strftime("%Y%m")
+        self.url = (
+            "http://www.supremecourt.gov/oral_arguments/argument_audio.aspx"
         )
-        self.back_scrape_iterable = [
-            "%s%02d" % (year, month)
-            for year in range(2007, d.year + 1)
-            for month in range(1, 13)
-        ]
-
-    def _download(self, **kwargs):
-        # The certificate on their site has expired.
-        return super()._download(request_dict={"verify": False})
+        self.back_scrape_iterable = list(range(2010, 2015))
 
     def _get_download_urls(self):
-        path = "id('ViewBody')//div[contains(concat(' ',@class,' '),' row-entry')]//@href"
-        return list(self.html.xpath(path))
+        path = "id('list')//tr//a/text()"
+        return list(map(self._return_download_url, self.html.xpath(path)))
+
+    @staticmethod
+    def _return_download_url(d):
+        file_type = "mp3"  # or 'wma' is also available for any case.
+        download_url = "http://www.supremecourt.gov/media/audio/{type}files/{docket_number}.{type}".format(
+            type=file_type, docket_number=d
+        )
+        return download_url
 
     def _get_case_names(self):
-        path = "id('ViewBody')//*[contains(concat(' ',@class,' '),' column-two')]/div[1]/text()"
-        return list(self.html.xpath(path))
+        path = "id('list')//tr/td/span/text()"
+        return [s.lstrip(". ") for s in self.html.xpath(path)]
 
     def _get_case_dates(self):
-        path = "id('ViewBody')//date/text()"
-        return list(map(self._return_case_date, self.html.xpath(path)))
-
-    @staticmethod
-    def _return_case_date(e):
-        e = "".join(e.split())
-        return datetime.strptime(e, "%m/%d/%Y").date()
+        path = "id('list')//tr/td[2]//text()"
+        return [
+            datetime.strptime(s, "%m/%d/%y").date()
+            for s in self.html.xpath(path)
+            if not "Date" in s
+        ]
 
     def _get_docket_numbers(self):
-        path = "id('ViewBody')//*[contains(concat(' ',@class,' '),' row-entry')]//a//text()"
+        path = "id('list')//tr//a/text()"
         return list(self.html.xpath(path))
 
-    def _get_judges(self):
-        path = '//div[span[contains(., "Judges")]]/text()'
-        return [" ".join(s.split()) for s in self.html.xpath(path)]
-
-    def _download_backwards(self, yearmo):
-        self.url = "http://www.cadc.uscourts.gov/recordings/recordings.nsf/DocsByRDate?OpenView&count=100&SKey={yearmo}".format(
-            yearmo=yearmo,
+    def _download_backwards(self, year):
+        self.url = (
+            f"http://www.supremecourt.gov/oral_arguments/argument_audio/{year}"
         )
         self.html = self._download()
```

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/cafc.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/federal_appellate/cafc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/state/ill.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_1st_dist.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/state/illappct_1st_dist.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/oral_args/united_states/state/md.py` & `juriscraper-2.6.1/juriscraper/oral_args/united_states/state/md.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/__init__.py` & `juriscraper-2.6.1/juriscraper/pacer/__init__.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/acms_docket.py` & `juriscraper-2.6.1/juriscraper/pacer/acms_docket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/appellate_attachment_page.py` & `juriscraper-2.6.1/juriscraper/pacer/appellate_attachment_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/appellate_docket.py` & `juriscraper-2.6.1/juriscraper/pacer/appellate_docket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/attachment_page.py` & `juriscraper-2.6.1/juriscraper/pacer/attachment_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/case_query.py` & `juriscraper-2.6.1/juriscraper/pacer/case_query.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/case_query_advanced.py` & `juriscraper-2.6.1/juriscraper/pacer/case_query_advanced.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/claims_activity.py` & `juriscraper-2.6.1/juriscraper/pacer/claims_activity.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/claims_register.py` & `juriscraper-2.6.1/juriscraper/pacer/claims_register.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/docket_history_report.py` & `juriscraper-2.6.1/juriscraper/pacer/docket_history_report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/docket_report.py` & `juriscraper-2.6.1/juriscraper/pacer/docket_report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/docket_utils.py` & `juriscraper-2.6.1/juriscraper/pacer/docket_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/download_confirmation_page.py` & `juriscraper-2.6.1/juriscraper/pacer/download_confirmation_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/email.py` & `juriscraper-2.6.1/juriscraper/pacer/email.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,15 +538,15 @@
             # In: 6:22-bk-13643-SY Request for courtesy Notice of Electronic Filing (NEF)
             # Out: Request for courtesy Notice of Electronic Filing (NEF)
             short_description = subject.split(docket_number)[-1]
 
             # Remove docket number traces "-AAA"
             regex = r"^-.*?\s"
             short_description = re.sub(regex, "", short_description)
-        elif self.court_id in ["njb", "dcb", "vaeb", "paeb"]:
+        elif self.court_id in ["njb", "dcb", "vaeb", "paeb", "mdb"]:
             # In: Ch-11 19-27439-MBK Determination of Adjournment Request - Hollister Construc
             # Out: Determination of Adjournment Request
             short_description = subject.split(docket_number)[-1]
             # Remove docket number traces "-AAA"
             # Remove CH after docket and BK after short description for dcb
             regex = r"^-.*?\s|C[Hh][\s\d]+|[ (]?B[Kk]( Other)?[) ]?"
             short_description = re.sub(regex, "", short_description)
@@ -561,18 +561,20 @@
             # Remove strings starting with "Ch" followed by a number
             regex = r"\bCh\d+\b"
             short_description = re.sub(regex, "", short_description)
 
             # Remove docket number traces "-AAA"
             regex = r"^-.*?\s"
             short_description = re.sub(regex, "", short_description)
-        elif self.court_id in ["pawb", "ndb"]:
+        elif self.court_id in ["pawb", "ndb", "deb"]:
             # In: Ch-7 22-20823-GLT U LOCK INC Reply
             # Out: Reply
-            short_description = subject.split(case_name)[-1]
+            if case_name in subject:
+                # See deb_2.txt for need of this check
+                short_description = subject.split(case_name)[-1]
         else:
             logger.error(
                 "Short description has no parsing for bankruptcy court '%s'",
                 self.court_id,
                 extra={
                     "fingerprint": [
                         f"{self.court_id}-not-parsing-short-description"
```

### Comparing `juriscraper-2.6.0/juriscraper/pacer/free_documents.py` & `juriscraper-2.6.1/juriscraper/pacer/free_documents.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/hidden_api.py` & `juriscraper-2.6.1/juriscraper/pacer/hidden_api.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/http.py` & `juriscraper-2.6.1/juriscraper/pacer/http.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/internet_archive.py` & `juriscraper-2.6.1/juriscraper/pacer/internet_archive.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/list_of_creditors.py` & `juriscraper-2.6.1/juriscraper/pacer/list_of_creditors.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/mobile_query.py` & `juriscraper-2.6.1/juriscraper/pacer/mobile_query.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/reports.py` & `juriscraper-2.6.1/juriscraper/pacer/reports.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/rss_feeds.py` & `juriscraper-2.6.1/juriscraper/pacer/rss_feeds.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacer/utils.py` & `juriscraper-2.6.1/juriscraper/pacer/utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/pacerdocket.py` & `juriscraper-2.6.1/juriscraper/pacerdocket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper/report.py` & `juriscraper-2.6.1/juriscraper/report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/juriscraper.egg-info/PKG-INFO` & `juriscraper-2.6.1/juriscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juriscraper
-Version: 2.6.0
+Version: 2.6.1
 Summary: An API to scrape American court websites for metadata.
 Home-page: https://github.com/freelawproject/juriscraper
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 License: BSD
```

### Comparing `juriscraper-2.6.0/juriscraper.egg-info/SOURCES.txt` & `juriscraper-2.6.1/juriscraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.0/setup.py` & `juriscraper-2.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 import os
 import unittest
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-VERSION = "2.6.0"
+VERSION = "2.6.1"
 AUTHOR = "Free Law Project"
 EMAIL = "info@free.law"
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 
 reqs_path = f"{HERE}/requirements.txt"
 with open(reqs_path) as reqs_file:
```

