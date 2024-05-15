# Comparing `tmp/tdda-2.1.2.tar.gz` & `tmp/tdda-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdda-2.1.2.tar", last modified: Tue Apr 30 16:28:19 2024, max compression
+gzip compressed data, was "tdda-2.1.5.tar", last modified: Wed May 15 18:00:34 2024, max compression
```

## Comparing `tdda-2.1.2.tar` & `tdda-2.1.5.tar`

### file list

```diff
@@ -1,237 +1,248 @@
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.022753 tdda-2.1.2/
--rw-r--r--   0 njr        (501) staff       (20)     1100 2022-04-01 21:00:40.000000 tdda-2.1.2/LICENSE.txt
--rw-r--r--   0 njr        (501) staff       (20)       38 2022-04-01 21:00:40.000000 tdda-2.1.2/MANIFEST.in
--rw-r--r--   0 njr        (501) staff       (20)     4616 2024-04-30 16:28:19.022669 tdda-2.1.2/PKG-INFO
--rw-r--r--   0 njr        (501) staff       (20)     4233 2024-04-30 15:44:51.000000 tdda-2.1.2/README.md
--rw-r--r--   0 njr        (501) staff       (20)      438 2024-04-30 16:23:26.000000 tdda-2.1.2/pyproject.toml
--rw-r--r--   0 njr        (501) staff       (20)      200 2024-04-30 16:28:19.022986 tdda-2.1.2/setup.cfg
--rw-r--r--   0 njr        (501) staff       (20)     2309 2024-02-12 09:13:47.000000 tdda-2.1.2/setup.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.995695 tdda-2.1.2/tdda/
--rw-r--r--   0 njr        (501) staff       (20)    28592 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/CHANGES.py
--rw-r--r--   0 njr        (501) staff       (20)      987 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/__init__.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.998339 tdda-2.1.2/tdda/constraints/
--rw-r--r--   0 njr        (501) staff       (20)      455 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)    36493 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/base.py
--rw-r--r--   0 njr        (501) staff       (20)    24998 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/baseconstraints.py
--rw-r--r--   0 njr        (501) staff       (20)     8001 2024-02-19 15:49:06.000000 tdda-2.1.2/tdda/constraints/console.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.999360 tdda-2.1.2/tdda/constraints/db/
--rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/db/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)    17342 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/constraints.py
--rw-r--r--   0 njr        (501) staff       (20)     2754 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/detect.py
--rw-r--r--   0 njr        (501) staff       (20)     2934 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/discover.py
--rw-r--r--   0 njr        (501) staff       (20)    30601 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/drivers.py
--rw-r--r--   0 njr        (501) staff       (20)     1444 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/extension.py
--rw-r--r--   0 njr        (501) staff       (20)    13836 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/testdbconstraints.py
--rw-r--r--   0 njr        (501) staff       (20)     2491 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/verify.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.001838 tdda-2.1.2/tdda/constraints/examples/
--rw-r--r--   0 njr        (501) staff       (20)     7336 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/README.md
--rw-r--r--   0 njr        (501) staff       (20)     4700 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts25k.tdda
--rw-r--r--   0 njr        (501) staff       (20)      326 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_detect_25k_against_1k.py
--rw-r--r--   0 njr        (501) staff       (20)      327 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_discover_1k.py
--rw-r--r--   0 njr        (501) staff       (20)      223 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_1k.py
--rw-r--r--   0 njr        (501) staff       (20)      226 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_25k.py
--rw-r--r--   0 njr        (501) staff       (20)      236 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_25k_against_1k.py
--rw-r--r--   0 njr        (501) staff       (20)      398 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_25k_against_1k_feather.py
--rw-r--r--   0 njr        (501) staff       (20)      264 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_25k_to_frame.py
--rw-r--r--   0 njr        (501) staff       (20)     2800 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements118.tdda
--rw-r--r--   0 njr        (501) staff       (20)      326 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_detect_118_against_92.py
--rw-r--r--   0 njr        (501) staff       (20)      327 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_discover_92.py
--rw-r--r--   0 njr        (501) staff       (20)      226 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_verify_118.py
--rw-r--r--   0 njr        (501) staff       (20)      236 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_verify_118_against_92.py
--rw-r--r--   0 njr        (501) staff       (20)      398 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_verify_118_against_92_feather.py
--rw-r--r--   0 njr        (501) staff       (20)      223 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_verify_92.py
--rw-r--r--   0 njr        (501) staff       (20)    13795 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/files_extension.py
--rw-r--r--   0 njr        (501) staff       (20)     1078 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/simple_discovery.py
--rw-r--r--   0 njr        (501) staff       (20)     2176 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/simple_verification.py
--rw-r--r--   0 njr        (501) staff       (20)      373 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/simple_verify_fail.py
--rw-r--r--   0 njr        (501) staff       (20)      316 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/simple_verify_pass.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.003691 tdda-2.1.2/tdda/constraints/examples/testdata/
--rw-r--r--   0 njr        (501) staff       (20)  1723312 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/accounts.zip
--rw-r--r--   0 njr        (501) staff       (20)     4881 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/accounts1k.tdda
--rw-r--r--   0 njr        (501) staff       (20)      703 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/ddd.csv
--rw-r--r--   0 njr        (501) staff       (20)     2709 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/ddd.tdda
--rw-r--r--   0 njr        (501) staff       (20)    13780 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements118.csv
--rw-r--r--   0 njr        (501) staff       (20)    19560 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements118.feather
--rw-r--r--   0 njr        (501) staff       (20)    15835 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements118.pmm
--rw-r--r--   0 njr        (501) staff       (20)    11460 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements92.csv
--rw-r--r--   0 njr        (501) staff       (20)     2954 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements92.tdda
--rw-r--r--   0 njr        (501) staff       (20)      511 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/examples.py
--rw-r--r--   0 njr        (501) staff       (20)    14680 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/extension.py
--rw-r--r--   0 njr        (501) staff       (20)     9008 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/flags.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.004597 tdda-2.1.2/tdda/constraints/pd/
--rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/pd/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)    53538 2024-04-30 15:49:32.000000 tdda-2.1.2/tdda/constraints/pd/constraints.py
--rw-r--r--   0 njr        (501) staff       (20)     3261 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/detect.py
--rw-r--r--   0 njr        (501) staff       (20)     2987 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/discover.py
--rw-r--r--   0 njr        (501) staff       (20)     1364 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/extension.py
--rw-r--r--   0 njr        (501) staff       (20)    73648 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/testpdconstraints.py
--rw-r--r--   0 njr        (501) staff       (20)     2926 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/verify.py
--rw-r--r--   0 njr        (501) staff       (20)      130 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/pdconstraints.py
--rw-r--r--   0 njr        (501) staff       (20)      128 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/pddiscover.py
--rw-r--r--   0 njr        (501) staff       (20)      126 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/pdverify.py
--rw-r--r--   0 njr        (501) staff       (20)     9858 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/tdda_json_file_format.md
--rw-r--r--   0 njr        (501) staff       (20)     6805 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/testbase.py
--rw-r--r--   0 njr        (501) staff       (20)      641 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/testconstraints.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.009089 tdda-2.1.2/tdda/constraints/testdata/
--rw-r--r--   0 njr        (501) staff       (20)      703 2024-01-29 09:44:59.000000 tdda-2.1.2/tdda/constraints/testdata/d.csv
--rw-r--r--   0 njr        (501) staff       (20)      703 2024-01-29 09:59:11.000000 tdda-2.1.2/tdda/constraints/testdata/ddd.csv
--rw-r--r--   0 njr        (501) staff       (20)     2601 2024-01-29 09:59:11.000000 tdda-2.1.2/tdda/constraints/testdata/ddd.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5007 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline-interleaved.csv
--rw-r--r--   0 njr        (501) staff       (20)     5116 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline.csv
--rw-r--r--   0 njr        (501) staff       (20)     5111 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline2.csv
--rw-r--r--   0 njr        (501) staff       (20)      207 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/detect_dups.df
--rw-r--r--   0 njr        (501) staff       (20)    13780 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.csv
--rw-r--r--   0 njr        (501) staff       (20)     2158 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.df
--rw-r--r--   0 njr        (501) staff       (20)    19560 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.feather
--rw-r--r--   0 njr        (501) staff       (20)    16972 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.parquet
--rw-r--r--   0 njr        (501) staff       (20)    15835 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.pmm
--rw-r--r--   0 njr        (501) staff       (20)     3278 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.tdda
--rw-r--r--   0 njr        (501) staff       (20)     2778 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_csv.csv
--rw-r--r--   0 njr        (501) staff       (20)     2773 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_feather.csv
--rw-r--r--   0 njr        (501) staff       (20)      688 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_feather.feather
--rw-r--r--   0 njr        (501) staff       (20)     5713 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118oldrex-3.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5949 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118oldrex.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5770 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex-3.tdda
--rw-r--r--   0 njr        (501) staff       (20)     2277 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex.df
--rw-r--r--   0 njr        (501) staff       (20)     5770 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex.tdda
--rw-r--r--   0 njr        (501) staff       (20)      173 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect.csv
--rw-r--r--   0 njr        (501) staff       (20)      666 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect.df
--rw-r--r--   0 njr        (501) staff       (20)     2994 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect_perc.csv
--rw-r--r--   0 njr        (501) staff       (20)    11460 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92.csv
--rw-r--r--   0 njr        (501) staff       (20)    15459 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/testdata/elements92.parquet
--rw-r--r--   0 njr        (501) staff       (20)     2954 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92.tdda
--rw-r--r--   0 njr        (501) staff       (20)     3458 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92_pandas.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5376 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92oldrex.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5332 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92rex.tdda
--rw-r--r--   0 njr        (501) staff       (20)    14504 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/example.csv
--rw-r--r--   0 njr        (501) staff       (20)    24576 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/example.db
--rw-r--r--   0 njr        (501) staff       (20)     1940 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/example.sql
--rw-r--r--   0 njr        (501) staff       (20)     3632 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/ref-accounts1k.tdda
--rw-r--r--   0 njr        (501) staff       (20)     3414 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/ref-accounts25k.tdda
--rw-r--r--   0 njr        (501) staff       (20)      907 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/ref-detect25k-failures.txt
--rw-r--r--   0 njr        (501) staff       (20)       51 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/sqlite.conn
--rw-r--r--   0 njr        (501) staff       (20)     2617 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/examples.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.009223 tdda-2.1.2/tdda/gentest/
--rw-r--r--   0 njr        (501) staff       (20)        0 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/__init__.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.009592 tdda-2.1.2/tdda/gentest/examples/
--rw-r--r--   0 njr        (501) staff       (20)     1915 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/README.md
--rw-r--r--   0 njr        (501) staff       (20)      311 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/example2.sh
--rw-r--r--   0 njr        (501) staff       (20)       11 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/hey
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.011363 tdda-2.1.2/tdda/gentest/examples/r-examples/
--rw-r--r--   0 njr        (501) staff       (20)      541 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/0-set-variables.R
--rw-r--r--   0 njr        (501) staff       (20)       54 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/00-install.R
--rw-r--r--   0 njr        (501) staff       (20)      389 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/1-compute-weighted-average-tolerance-values.R
--rw-r--r--   0 njr        (501) staff       (20)     1725 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/2-compute-cumulative-percentiles.R
--rw-r--r--   0 njr        (501) staff       (20)     2750 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/3-parametric-regression.R
--rw-r--r--   0 njr        (501) staff       (20)     1778 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/4-non-parametric-regression.R
--rw-r--r--   0 njr        (501) staff       (20)     7686 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/README.md
--rw-r--r--   0 njr        (501) staff       (20)     5426 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/env.data.or.txt
--rw-r--r--   0 njr        (501) staff       (20)    19410 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/env.data.txt
--rw-r--r--   0 njr        (501) staff       (20)   199154 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/site.species.or.txt
--rw-r--r--   0 njr        (501) staff       (20)   354013 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/site.species.txt
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.013789 tdda-2.1.2/tdda/referencetest/
--rw-r--r--   0 njr        (501) staff       (20)     6515 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)     3260 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/basecomparison.py
--rw-r--r--   0 njr        (501) staff       (20)     1131 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/captureoutput.py
--rw-r--r--   0 njr        (501) staff       (20)    40454 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/checkfiles.py
--rw-r--r--   0 njr        (501) staff       (20)    22759 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/checkpandas.py
--rw-r--r--   0 njr        (501) staff       (20)     4328 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/diffrex.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.014228 tdda-2.1.2/tdda/referencetest/examples/
--rw-r--r--   0 njr        (501) staff       (20)     4851 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/README.md
--rw-r--r--   0 njr        (501) staff       (20)      888 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/dataframes.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.993083 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.014880 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/
--rw-r--r--   0 njr        (501) staff       (20)      478 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/conftest.py
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/expected.html
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/generators.py
--rw-r--r--   0 njr        (501) staff       (20)      489 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/test_all.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.015493 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/
--rw-r--r--   0 njr        (501) staff       (20)      476 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/conftest.py
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/expected.html
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/generators.py
--rw-r--r--   0 njr        (501) staff       (20)      654 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/test_all.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.993258 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.015938 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/expected.html
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/generators.py
--rw-r--r--   0 njr        (501) staff       (20)      606 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/test_all.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.016377 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/expected.html
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/generators.py
--rw-r--r--   0 njr        (501) staff       (20)      887 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/test_all.py
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/generators.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.016662 tdda-2.1.2/tdda/referencetest/examples/pytest/
--rw-r--r--   0 njr        (501) staff       (20)      631 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/pytest/conftest.py
--rw-r--r--   0 njr        (501) staff       (20)     5785 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/pytest/test_using_referencepytest.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.017192 tdda-2.1.2/tdda/referencetest/examples/reference/
--rw-r--r--   0 njr        (501) staff       (20)      530 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/reference/dataframe_result.csv
--rw-r--r--   0 njr        (501) staff       (20)     1096 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/reference/dataframe_result2.csv
--rw-r--r--   0 njr        (501) staff       (20)     1570 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/reference/file_result.html
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/reference/string_result.html
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.017332 tdda-2.1.2/tdda/referencetest/examples/unittest/
--rw-r--r--   0 njr        (501) staff       (20)     6643 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/unittest/test_using_referencetestcase.py
--rw-r--r--   0 njr        (501) staff       (20)      556 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/examples.py
--rw-r--r--   0 njr        (501) staff       (20)    55226 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/gentest.py
--rw-r--r--   0 njr        (501) staff       (20)      962 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/gentest_boilerplate.py
--rw-r--r--   0 njr        (501) staff       (20)     3962 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/pddates.py
--rw-r--r--   0 njr        (501) staff       (20)     1500 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/pytestconfig.py
--rw-r--r--   0 njr        (501) staff       (20)    10499 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/referencepytest.py
--rw-r--r--   0 njr        (501) staff       (20)    36641 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/referencetest.py
--rw-r--r--   0 njr        (501) staff       (20)    11082 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/referencetestcase.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.018080 tdda-2.1.2/tdda/referencetest/tests/
--rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)      484 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/alltests.py
--rw-r--r--   0 njr        (501) staff       (20)     1701 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testbase.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.019447 tdda-2.1.2/tdda/referencetest/tests/testdata/
--rw-r--r--   0 njr        (501) staff       (20)     4389 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/colours.txt
--rw-r--r--   0 njr        (501) staff       (20)       28 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/double.txt
--rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/empty.txt
--rw-r--r--   0 njr        (501) staff       (20)      219 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/frames_fail1.txt
--rw-r--r--   0 njr        (501) staff       (20)       64 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/frames_fail2.txt
--rw-r--r--   0 njr        (501) staff       (20)       66 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/frames_fail3.txt
--rw-r--r--   0 njr        (501) staff       (20)      218 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/left.txt
--rw-r--r--   0 njr        (501) staff       (20)      171 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/ref.txt
--rw-r--r--   0 njr        (501) staff       (20)      198 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/removals.txt
--rw-r--r--   0 njr        (501) staff       (20)       14 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/single.txt
--rw-r--r--   0 njr        (501) staff       (20)       14 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/single2.txt
--rw-r--r--   0 njr        (501) staff       (20)    15273 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testfiles.py
--rw-r--r--   0 njr        (501) staff       (20)     6971 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/tests/testpandas.py
--rw-r--r--   0 njr        (501) staff       (20)     2113 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testregeneration.py
--rw-r--r--   0 njr        (501) staff       (20)    11656 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/teststrings.py
--rw-r--r--   0 njr        (501) staff       (20)     2610 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/utils.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.020643 tdda-2.1.2/tdda/rexpy/
--rw-r--r--   0 njr        (501) staff       (20)      176 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/__init__.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.021164 tdda-2.1.2/tdda/rexpy/examples/
--rw-r--r--   0 njr        (501) staff       (20)     1126 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/examples/agents9.txt
--rw-r--r--   0 njr        (501) staff       (20)       44 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/examples/headed-ids.txt
--rw-r--r--   0 njr        (501) staff       (20)      230 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/examples/ids.py
--rw-r--r--   0 njr        (501) staff       (20)      364 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/examples/pandas_ids.py
--rw-r--r--   0 njr        (501) staff       (20)      465 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/rexpy/examples.py
--rw-r--r--   0 njr        (501) staff       (20)       50 2023-03-27 07:08:57.000000 tdda-2.1.2/tdda/rexpy/quality.py
--rw-r--r--   0 njr        (501) staff       (20)      412 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/relib.py
--rw-r--r--   0 njr        (501) staff       (20)    91873 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/rexpy/rexpy.py
--rw-r--r--   0 njr        (501) staff       (20)     3230 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/seq.py
--rw-r--r--   0 njr        (501) staff       (20)     1033 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/testhypo.py
--rw-r--r--   0 njr        (501) staff       (20)    74007 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/rexpy/testrexpy.py
--rw-r--r--   0 njr        (501) staff       (20)      716 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/rexpy/testseq.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.022202 tdda-2.1.2/tdda/serial/
--rw-r--r--   0 njr        (501) staff       (20)       93 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)     6088 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/base.py
--rw-r--r--   0 njr        (501) staff       (20)     1449 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/cli.py
--rw-r--r--   0 njr        (501) staff       (20)    11284 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/csvw.py
--rw-r--r--   0 njr        (501) staff       (20)     1478 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/pandasio.py
--rw-r--r--   0 njr        (501) staff       (20)     4948 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/reader.py
--rw-r--r--   0 njr        (501) staff       (20)    17656 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/testserialmetadata.py
--rw-r--r--   0 njr        (501) staff       (20)     1484 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/utils.py
--rw-r--r--   0 njr        (501) staff       (20)     1090 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/testconfig.py
--rw-r--r--   0 njr        (501) staff       (20)      753 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/testtdda.py
--rw-r--r--   0 njr        (501) staff       (20)      246 2024-04-30 16:26:42.000000 tdda-2.1.2/tdda/version.py
--rw-r--r--   0 njr        (501) staff       (20)    10442 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/writabletestcase.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.022424 tdda-2.1.2/tdda.egg-info/
--rw-r--r--   0 njr        (501) staff       (20)     4616 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/PKG-INFO
--rw-r--r--   0 njr        (501) staff       (20)     8561 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/SOURCES.txt
--rw-r--r--   0 njr        (501) staff       (20)        1 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/dependency_links.txt
--rw-r--r--   0 njr        (501) staff       (20)       85 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/entry_points.txt
--rw-r--r--   0 njr        (501) staff       (20)        1 2023-02-10 16:16:28.000000 tdda-2.1.2/tdda.egg-info/not-zip-safe
--rw-r--r--   0 njr        (501) staff       (20)       28 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/requires.txt
--rw-r--r--   0 njr        (501) staff       (20)        5 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/top_level.txt
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.169322 tdda-2.1.5/
+-rw-r--r--   0 njr        (501) staff       (20)     1100 2022-04-01 21:00:40.000000 tdda-2.1.5/LICENSE.txt
+-rw-r--r--   0 njr        (501) staff       (20)       38 2022-04-01 21:00:40.000000 tdda-2.1.5/MANIFEST.in
+-rw-r--r--   0 njr        (501) staff       (20)     4616 2024-05-15 18:00:34.169257 tdda-2.1.5/PKG-INFO
+-rw-r--r--   0 njr        (501) staff       (20)     4233 2024-05-03 08:00:27.000000 tdda-2.1.5/README.md
+-rw-r--r--   0 njr        (501) staff       (20)      438 2024-05-15 17:52:10.000000 tdda-2.1.5/pyproject.toml
+-rw-r--r--   0 njr        (501) staff       (20)      200 2024-05-15 18:00:34.169542 tdda-2.1.5/setup.cfg
+-rw-r--r--   0 njr        (501) staff       (20)     2309 2024-02-12 09:13:47.000000 tdda-2.1.5/setup.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.134995 tdda-2.1.5/tdda/
+-rw-r--r--   0 njr        (501) staff       (20)    28592 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/CHANGES.py
+-rw-r--r--   0 njr        (501) staff       (20)      987 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/__init__.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.138480 tdda-2.1.5/tdda/constraints/
+-rw-r--r--   0 njr        (501) staff       (20)      455 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)    36493 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/base.py
+-rw-r--r--   0 njr        (501) staff       (20)    24998 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/baseconstraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     8001 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/console.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.139616 tdda-2.1.5/tdda/constraints/db/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/db/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)    17342 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/db/constraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     2754 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/db/detect.py
+-rw-r--r--   0 njr        (501) staff       (20)     2934 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/db/discover.py
+-rw-r--r--   0 njr        (501) staff       (20)    30601 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/db/drivers.py
+-rw-r--r--   0 njr        (501) staff       (20)     1444 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/db/extension.py
+-rw-r--r--   0 njr        (501) staff       (20)    13836 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/db/testdbconstraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     2491 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/db/verify.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.142119 tdda-2.1.5/tdda/constraints/examples/
+-rw-r--r--   0 njr        (501) staff       (20)     7336 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/README.md
+-rw-r--r--   0 njr        (501) staff       (20)      326 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/accounts_detect_25k_against_1k.py
+-rw-r--r--   0 njr        (501) staff       (20)      327 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/accounts_discover_1k.py
+-rw-r--r--   0 njr        (501) staff       (20)      223 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/accounts_verify_1k.py
+-rw-r--r--   0 njr        (501) staff       (20)      188 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/accounts_verify_25k.py
+-rw-r--r--   0 njr        (501) staff       (20)      207 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/accounts_verify_25k_against_1k.py
+-rw-r--r--   0 njr        (501) staff       (20)      368 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/accounts_verify_25k_against_1k_parquet.py
+-rw-r--r--   0 njr        (501) staff       (20)      264 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/accounts_verify_25k_to_frame.py
+-rw-r--r--   0 njr        (501) staff       (20)    16972 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/elements118.parquet
+-rw-r--r--   0 njr        (501) staff       (20)    15459 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/elements92.parquet
+-rw-r--r--   0 njr        (501) staff       (20)      326 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/elements_detect_118_against_92.py
+-rw-r--r--   0 njr        (501) staff       (20)      327 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/elements_discover_92.py
+-rw-r--r--   0 njr        (501) staff       (20)      226 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/elements_verify_118.py
+-rw-r--r--   0 njr        (501) staff       (20)      236 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/elements_verify_118_against_92.py
+-rw-r--r--   0 njr        (501) staff       (20)      368 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/elements_verify_118_against_92_parquet.py
+-rw-r--r--   0 njr        (501) staff       (20)      223 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/elements_verify_92.py
+-rw-r--r--   0 njr        (501) staff       (20)    13795 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/files_extension.py
+-rw-r--r--   0 njr        (501) staff       (20)     1078 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/simple_discovery.py
+-rw-r--r--   0 njr        (501) staff       (20)     2176 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/simple_verification.py
+-rw-r--r--   0 njr        (501) staff       (20)      373 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/simple_verify_fail.py
+-rw-r--r--   0 njr        (501) staff       (20)      316 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/simple_verify_pass.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.145750 tdda-2.1.5/tdda/constraints/examples/testdata/
+-rw-r--r--   0 njr        (501) staff       (20)  1723312 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/testdata/accounts.zip
+-rw-r--r--   0 njr        (501) staff       (20)     4881 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/testdata/accounts1k.tdda
+-rw-r--r--   0 njr        (501) staff       (20)  2174703 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/testdata/accounts25k.parquet
+-rw-r--r--   0 njr        (501) staff       (20)      703 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/testdata/ddd.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2709 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/testdata/ddd.tdda
+-rw-r--r--   0 njr        (501) staff       (20)    13780 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/testdata/elements118.csv
+-rw-r--r--   0 njr        (501) staff       (20)    19560 2024-05-15 17:51:54.000000 tdda-2.1.5/tdda/constraints/examples/testdata/elements118.feather
+-rw-r--r--   0 njr        (501) staff       (20)    16972 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/testdata/elements118.parquet
+-rw-r--r--   0 njr        (501) staff       (20)    15835 2024-05-15 17:52:05.000000 tdda-2.1.5/tdda/constraints/examples/testdata/elements118.pmm
+-rw-r--r--   0 njr        (501) staff       (20)     5736 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/testdata/elements118.tdda
+-rw-r--r--   0 njr        (501) staff       (20)    11460 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/testdata/elements92.csv
+-rw-r--r--   0 njr        (501) staff       (20)    15459 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/examples/testdata/elements92.parquet
+-rw-r--r--   0 njr        (501) staff       (20)     2954 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/examples/testdata/elements92.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      511 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/examples.py
+-rw-r--r--   0 njr        (501) staff       (20)    14680 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/extension.py
+-rw-r--r--   0 njr        (501) staff       (20)     8998 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/flags.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.146615 tdda-2.1.5/tdda/constraints/pd/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/pd/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)    52770 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/pd/constraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     2977 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/pd/detect.py
+-rw-r--r--   0 njr        (501) staff       (20)     2716 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/pd/discover.py
+-rw-r--r--   0 njr        (501) staff       (20)     1364 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/pd/extension.py
+-rw-r--r--   0 njr        (501) staff       (20)    73648 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/constraints/pd/testpdconstraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     2673 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/constraints/pd/verify.py
+-rw-r--r--   0 njr        (501) staff       (20)      130 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/pdconstraints.py
+-rw-r--r--   0 njr        (501) staff       (20)      128 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/pddiscover.py
+-rw-r--r--   0 njr        (501) staff       (20)      126 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/pdverify.py
+-rw-r--r--   0 njr        (501) staff       (20)     9858 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/tdda_json_file_format.md
+-rw-r--r--   0 njr        (501) staff       (20)     6805 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/testbase.py
+-rw-r--r--   0 njr        (501) staff       (20)      641 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/constraints/testconstraints.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.155123 tdda-2.1.5/tdda/constraints/testdata/
+-rw-r--r--   0 njr        (501) staff       (20)      703 2024-01-29 09:44:59.000000 tdda-2.1.5/tdda/constraints/testdata/d.csv
+-rw-r--r--   0 njr        (501) staff       (20)      703 2024-01-29 09:59:11.000000 tdda-2.1.5/tdda/constraints/testdata/ddd.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2601 2024-01-29 09:59:11.000000 tdda-2.1.5/tdda/constraints/testdata/ddd.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5007 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/detect-els-cmdline-interleaved.csv
+-rw-r--r--   0 njr        (501) staff       (20)     5116 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/detect-els-cmdline.csv
+-rw-r--r--   0 njr        (501) staff       (20)     5111 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/detect-els-cmdline2.csv
+-rw-r--r--   0 njr        (501) staff       (20)      207 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/detect_dups.df
+-rw-r--r--   0 njr        (501) staff       (20)    13780 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2158 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118.df
+-rw-r--r--   0 njr        (501) staff       (20)    19560 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118.feather
+-rw-r--r--   0 njr        (501) staff       (20)    16972 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/constraints/testdata/elements118.parquet
+-rw-r--r--   0 njr        (501) staff       (20)    15835 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118.pmm
+-rw-r--r--   0 njr        (501) staff       (20)     3278 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     2778 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118_detect_from_csv.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2773 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118_detect_from_feather.csv
+-rw-r--r--   0 njr        (501) staff       (20)      688 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118_detect_from_feather.feather
+-rw-r--r--   0 njr        (501) staff       (20)     5713 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118oldrex-3.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5949 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118oldrex.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5770 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118rex-3.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     2277 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118rex.df
+-rw-r--r--   0 njr        (501) staff       (20)     5770 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118rex.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      173 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118rex_detect.csv
+-rw-r--r--   0 njr        (501) staff       (20)      666 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118rex_detect.df
+-rw-r--r--   0 njr        (501) staff       (20)     2994 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements118rex_detect_perc.csv
+-rw-r--r--   0 njr        (501) staff       (20)    11460 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements92.csv
+-rw-r--r--   0 njr        (501) staff       (20)    15459 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/constraints/testdata/elements92.parquet
+-rw-r--r--   0 njr        (501) staff       (20)     2954 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements92.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     3458 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements92_pandas.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5376 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements92oldrex.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5332 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/elements92rex.tdda
+-rw-r--r--   0 njr        (501) staff       (20)    14504 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/example.csv
+-rw-r--r--   0 njr        (501) staff       (20)    24576 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/example.db
+-rw-r--r--   0 njr        (501) staff       (20)     1940 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/example.sql
+-rw-r--r--   0 njr        (501) staff       (20)     3632 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/ref-accounts1k.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     3414 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/ref-accounts25k.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      907 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/ref-detect25k-failures.txt
+-rw-r--r--   0 njr        (501) staff       (20)       51 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/constraints/testdata/sqlite.conn
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.155314 tdda-2.1.5/tdda/deprecated/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/deprecated/__init__.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.155733 tdda-2.1.5/tdda/deprecated/examples/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/deprecated/examples/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)     3698 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/deprecated/examples/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)     3197 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/deprecated/examples/test_using_writabletestcase.py
+-rw-r--r--   0 njr        (501) staff       (20)     1404 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/deprecated/featherfiles.py
+-rw-r--r--   0 njr        (501) staff       (20)     2617 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/examples.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.155957 tdda-2.1.5/tdda/gentest/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/__init__.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.156249 tdda-2.1.5/tdda/gentest/examples/
+-rw-r--r--   0 njr        (501) staff       (20)     1915 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/README.md
+-rw-r--r--   0 njr        (501) staff       (20)      323 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/gentest/examples/example2.sh
+-rw-r--r--   0 njr        (501) staff       (20)       11 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/hey
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.157591 tdda-2.1.5/tdda/gentest/examples/r-examples/
+-rw-r--r--   0 njr        (501) staff       (20)      541 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/0-set-variables.R
+-rw-r--r--   0 njr        (501) staff       (20)       54 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/00-install.R
+-rw-r--r--   0 njr        (501) staff       (20)      389 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/1-compute-weighted-average-tolerance-values.R
+-rw-r--r--   0 njr        (501) staff       (20)     1725 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/2-compute-cumulative-percentiles.R
+-rw-r--r--   0 njr        (501) staff       (20)     2750 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/3-parametric-regression.R
+-rw-r--r--   0 njr        (501) staff       (20)     1778 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/4-non-parametric-regression.R
+-rw-r--r--   0 njr        (501) staff       (20)     7686 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/README.md
+-rw-r--r--   0 njr        (501) staff       (20)     5426 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/env.data.or.txt
+-rw-r--r--   0 njr        (501) staff       (20)    19410 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/env.data.txt
+-rw-r--r--   0 njr        (501) staff       (20)   199154 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/site.species.or.txt
+-rw-r--r--   0 njr        (501) staff       (20)   354013 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/gentest/examples/r-examples/site.species.txt
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.160033 tdda-2.1.5/tdda/referencetest/
+-rw-r--r--   0 njr        (501) staff       (20)     6515 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)     3260 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/basecomparison.py
+-rw-r--r--   0 njr        (501) staff       (20)     1131 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/captureoutput.py
+-rw-r--r--   0 njr        (501) staff       (20)    40454 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/checkfiles.py
+-rw-r--r--   0 njr        (501) staff       (20)    22759 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/referencetest/checkpandas.py
+-rw-r--r--   0 njr        (501) staff       (20)     4328 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/diffrex.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.160354 tdda-2.1.5/tdda/referencetest/examples/
+-rw-r--r--   0 njr        (501) staff       (20)     4851 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/README.md
+-rw-r--r--   0 njr        (501) staff       (20)      888 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/dataframes.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.129895 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.160812 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise1/
+-rw-r--r--   0 njr        (501) staff       (20)      478 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise1/conftest.py
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise1/expected.html
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise1/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)      489 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise1/test_all.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.161340 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise2/
+-rw-r--r--   0 njr        (501) staff       (20)      476 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise2/conftest.py
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise2/expected.html
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise2/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)      654 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise2/test_all.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.130115 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.161930 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise1/
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise1/expected.html
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise1/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)      606 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise1/test_all.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.162342 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise2/
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise2/expected.html
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise2/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)      887 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise2/test_all.py
+-rw-r--r--   0 njr        (501) staff       (20)     3991 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/referencetest/examples/generators.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.162635 tdda-2.1.5/tdda/referencetest/examples/pytest/
+-rw-r--r--   0 njr        (501) staff       (20)      631 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/pytest/conftest.py
+-rw-r--r--   0 njr        (501) staff       (20)     5785 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/pytest/test_using_referencepytest.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.163128 tdda-2.1.5/tdda/referencetest/examples/reference/
+-rw-r--r--   0 njr        (501) staff       (20)      530 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/reference/dataframe_result.csv
+-rw-r--r--   0 njr        (501) staff       (20)     1096 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/reference/dataframe_result2.csv
+-rw-r--r--   0 njr        (501) staff       (20)     1570 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/reference/file_result.html
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/reference/string_result.html
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.163245 tdda-2.1.5/tdda/referencetest/examples/unittest/
+-rw-r--r--   0 njr        (501) staff       (20)     6643 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/examples/unittest/test_using_referencetestcase.py
+-rw-r--r--   0 njr        (501) staff       (20)      556 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/examples.py
+-rw-r--r--   0 njr        (501) staff       (20)    55226 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/gentest.py
+-rw-r--r--   0 njr        (501) staff       (20)      962 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/gentest_boilerplate.py
+-rw-r--r--   0 njr        (501) staff       (20)     3962 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/referencetest/pddates.py
+-rw-r--r--   0 njr        (501) staff       (20)     1500 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/pytestconfig.py
+-rw-r--r--   0 njr        (501) staff       (20)    10499 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/referencepytest.py
+-rw-r--r--   0 njr        (501) staff       (20)    36641 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/referencetest/referencetest.py
+-rw-r--r--   0 njr        (501) staff       (20)    11082 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/referencetest/referencetestcase.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.164039 tdda-2.1.5/tdda/referencetest/tests/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)      484 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/alltests.py
+-rw-r--r--   0 njr        (501) staff       (20)     1701 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testbase.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.165383 tdda-2.1.5/tdda/referencetest/tests/testdata/
+-rw-r--r--   0 njr        (501) staff       (20)     4389 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/colours.txt
+-rw-r--r--   0 njr        (501) staff       (20)       28 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/double.txt
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/empty.txt
+-rw-r--r--   0 njr        (501) staff       (20)      219 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/frames_fail1.txt
+-rw-r--r--   0 njr        (501) staff       (20)       64 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/frames_fail2.txt
+-rw-r--r--   0 njr        (501) staff       (20)       66 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/frames_fail3.txt
+-rw-r--r--   0 njr        (501) staff       (20)      218 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/left.txt
+-rw-r--r--   0 njr        (501) staff       (20)      171 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/ref.txt
+-rw-r--r--   0 njr        (501) staff       (20)      198 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/removals.txt
+-rw-r--r--   0 njr        (501) staff       (20)       14 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/single.txt
+-rw-r--r--   0 njr        (501) staff       (20)       14 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testdata/single2.txt
+-rw-r--r--   0 njr        (501) staff       (20)    15273 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testfiles.py
+-rw-r--r--   0 njr        (501) staff       (20)     6971 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/referencetest/tests/testpandas.py
+-rw-r--r--   0 njr        (501) staff       (20)     2113 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/testregeneration.py
+-rw-r--r--   0 njr        (501) staff       (20)    11656 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/referencetest/tests/teststrings.py
+-rw-r--r--   0 njr        (501) staff       (20)     2677 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/referencetest/utils.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.167107 tdda-2.1.5/tdda/rexpy/
+-rw-r--r--   0 njr        (501) staff       (20)      176 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/rexpy/__init__.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.167561 tdda-2.1.5/tdda/rexpy/examples/
+-rw-r--r--   0 njr        (501) staff       (20)     1126 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/rexpy/examples/agents9.txt
+-rw-r--r--   0 njr        (501) staff       (20)       44 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/rexpy/examples/headed-ids.txt
+-rw-r--r--   0 njr        (501) staff       (20)      230 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/rexpy/examples/ids.py
+-rw-r--r--   0 njr        (501) staff       (20)      364 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/rexpy/examples/pandas_ids.py
+-rw-r--r--   0 njr        (501) staff       (20)      465 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/rexpy/examples.py
+-rw-r--r--   0 njr        (501) staff       (20)       50 2023-03-27 07:08:57.000000 tdda-2.1.5/tdda/rexpy/quality.py
+-rw-r--r--   0 njr        (501) staff       (20)      412 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/rexpy/relib.py
+-rw-r--r--   0 njr        (501) staff       (20)    91873 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/rexpy/rexpy.py
+-rw-r--r--   0 njr        (501) staff       (20)     3230 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/rexpy/seq.py
+-rw-r--r--   0 njr        (501) staff       (20)     1033 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/rexpy/testhypo.py
+-rw-r--r--   0 njr        (501) staff       (20)    74007 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/rexpy/testrexpy.py
+-rw-r--r--   0 njr        (501) staff       (20)      716 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/rexpy/testseq.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.168732 tdda-2.1.5/tdda/serial/
+-rw-r--r--   0 njr        (501) staff       (20)       93 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/serial/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)     6088 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/serial/base.py
+-rw-r--r--   0 njr        (501) staff       (20)     1449 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/serial/cli.py
+-rw-r--r--   0 njr        (501) staff       (20)    11284 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/serial/csvw.py
+-rw-r--r--   0 njr        (501) staff       (20)     1478 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/serial/pandasio.py
+-rw-r--r--   0 njr        (501) staff       (20)     4948 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/serial/reader.py
+-rw-r--r--   0 njr        (501) staff       (20)    17656 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/serial/testserialmetadata.py
+-rw-r--r--   0 njr        (501) staff       (20)     1484 2024-04-30 15:41:12.000000 tdda-2.1.5/tdda/serial/utils.py
+-rw-r--r--   0 njr        (501) staff       (20)     1090 2022-04-01 21:00:40.000000 tdda-2.1.5/tdda/testconfig.py
+-rw-r--r--   0 njr        (501) staff       (20)      793 2024-05-15 17:52:10.000000 tdda-2.1.5/tdda/testtdda.py
+-rw-r--r--   0 njr        (501) staff       (20)      246 2024-05-15 17:53:12.000000 tdda-2.1.5/tdda/version.py
+-rw-r--r--   0 njr        (501) staff       (20)    10442 2024-02-12 09:13:47.000000 tdda-2.1.5/tdda/writabletestcase.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-05-15 18:00:34.169016 tdda-2.1.5/tdda.egg-info/
+-rw-r--r--   0 njr        (501) staff       (20)     4616 2024-05-15 18:00:34.000000 tdda-2.1.5/tdda.egg-info/PKG-INFO
+-rw-r--r--   0 njr        (501) staff       (20)     8974 2024-05-15 18:00:34.000000 tdda-2.1.5/tdda.egg-info/SOURCES.txt
+-rw-r--r--   0 njr        (501) staff       (20)        1 2024-05-15 18:00:34.000000 tdda-2.1.5/tdda.egg-info/dependency_links.txt
+-rw-r--r--   0 njr        (501) staff       (20)       85 2024-05-15 18:00:34.000000 tdda-2.1.5/tdda.egg-info/entry_points.txt
+-rw-r--r--   0 njr        (501) staff       (20)        1 2023-02-10 16:16:28.000000 tdda-2.1.5/tdda.egg-info/not-zip-safe
+-rw-r--r--   0 njr        (501) staff       (20)       28 2024-05-15 18:00:34.000000 tdda-2.1.5/tdda.egg-info/requires.txt
+-rw-r--r--   0 njr        (501) staff       (20)        5 2024-05-15 18:00:34.000000 tdda-2.1.5/tdda.egg-info/top_level.txt
```

### Comparing `tdda-2.1.2/LICENSE.txt` & `tdda-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/PKG-INFO` & `tdda-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdda
-Version: 2.1.2
+Version: 2.1.5
 Home-page: http://www.stochasticsolutions.com
 Download-URL: https://github.com/tdda/tdda
 Author: Simon Brown
 Author-email: Nick Radcliffe <njr@stochasticsolutions.com>
 License: MIT
 Keywords: tdda constraint referencetest rexpy
 Requires-Python: >=3.8
```

### Comparing `tdda-2.1.2/README.md` & `tdda-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/setup.py` & `tdda-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/CHANGES.py` & `tdda-2.1.5/tdda/CHANGES.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/__init__.py` & `tdda-2.1.5/tdda/__init__.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/base.py` & `tdda-2.1.5/tdda/constraints/base.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/baseconstraints.py` & `tdda-2.1.5/tdda/constraints/baseconstraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/console.py` & `tdda-2.1.5/tdda/constraints/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """
 Command line interface for constraint discovery and verification.
 
 If pandas is available, constraints can be discovered and verified on
-.csv files and saved .feather dataframe files.
+.csv files and saved .parquet dataframe files.
 
 If supported database drivers are available, constraints can be discovered
 and verified on tables in databases.
 
 Constraint discovery and verification may be available for other data
 sources too, via any extensions specified in the `TDDA_EXTENSIONS`
 environment variable, if these are loadable using the normal Python module
```

### Comparing `tdda-2.1.2/tdda/constraints/db/constraints.py` & `tdda-2.1.5/tdda/constraints/db/constraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/db/detect.py` & `tdda-2.1.5/tdda/constraints/db/detect.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/db/discover.py` & `tdda-2.1.5/tdda/constraints/db/discover.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/db/drivers.py` & `tdda-2.1.5/tdda/constraints/db/drivers.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/db/extension.py` & `tdda-2.1.5/tdda/constraints/db/extension.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/db/testdbconstraints.py` & `tdda-2.1.5/tdda/constraints/db/testdbconstraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/db/verify.py` & `tdda-2.1.5/tdda/constraints/db/verify.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/README.md` & `tdda-2.1.5/tdda/constraints/examples/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/accounts25k.tdda` & `tdda-2.1.5/tdda/constraints/examples/testdata/accounts1k.tdda`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8922526041666666%*

 * *Differences: {"'creation_metadata'": "{'local_time': '2019-03-07 11:11:14', 'utc_time': '2019-03-07 11:11:14', "*

 * *                        "'source': 'testdata/accounts1k.csv', 'dataset': 'accounts1k.csv', "*

 * *                        "'n_records': 1000, 'n_selected': 1000, 'tddafile': "*

 * *                        "'testdata/accounts1k.tdda'}",*

 * * "'fields'": "{'account_number': {'min': 10000801, 'max': 12994290}, 'open_date': {'min': "*

 * *             "'2002-10-02 00:00:00', 'max': '2018-11-17 00:00:00'}, 'close_date': {'min': "*

 * *   […]*

```diff
@@ -1,50 +1,49 @@
 {
     "creation_metadata": {
         "creator": "TDDA 1.0.21",
-        "dataset": "accounts25k.csv",
+        "dataset": "accounts1k.csv",
         "host": "teacsa.local",
-        "local_time": "2019-03-07 11:11:17",
-        "n_records": 25000,
-        "n_selected": 25000,
-        "source": "testdata/accounts25k.csv",
-        "tddafile": "accounts25k.tdda",
+        "local_time": "2019-03-07 11:11:14",
+        "n_records": 1000,
+        "n_selected": 1000,
+        "source": "testdata/accounts1k.csv",
+        "tddafile": "testdata/accounts1k.tdda",
         "user": "simon",
-        "utc_time": "2019-03-07 11:11:17"
+        "utc_time": "2019-03-07 11:11:14"
     },
     "fields": {
         "account_number": {
-            "max": 12999930,
+            "max": 12994290,
             "max_nulls": 0,
-            "min": 10000191,
+            "min": 10000801,
             "no_duplicates": true,
             "sign": "positive",
             "type": "int"
         },
         "account_type": {
             "allowed_values": [
                 "basic",
                 "current",
                 "current+",
-                "no longer valid",
                 "offset",
                 "premium"
             ],
-            "max_length": 15,
+            "max_length": 8,
+            "max_nulls": 0,
             "min_length": 5,
             "rex": [
                 "^[a-z]{5,7}$",
-                "^current\\+$",
-                "^no longer valid$"
+                "^current\\+$"
             ],
             "type": "string"
         },
         "address1": {
             "max_length": 25,
-            "max_nulls": 1,
+            "max_nulls": 0,
             "min_length": 7,
             "rex": [
                 "^\\d{1,3} [A-Z][a-z]+ $",
                 "^\\d{1,3} Yellow Brick $",
                 "^\\d{1,3} [A-Z][a-z]+ [A-Z][a-z]+$",
                 "^\\d{1,3} [A-Z][a-z]{9}\\'s $",
                 "^\\d{1,3} Yellow Brick [A-Z][a-z]+$",
@@ -52,39 +51,42 @@
             ],
             "type": "string"
         },
         "cash_card_number": {
             "max_length": 19,
             "max_nulls": 0,
             "min_length": 19,
+            "no_duplicates": true,
             "rex": [
-                "^\\d{4} \\d{4} \\d{4} \\d{4}$"
+                "^1202 \\d{4} \\d{4} \\d{4}$"
             ],
             "type": "string"
         },
         "city": {
             "max_length": 18,
+            "max_nulls": 0,
             "min_length": 4,
             "rex": [
                 "^[A-Z][a-z]+$",
                 "^St Albans$",
                 "^Welwyn Garden City$",
                 "^Ashby de la Zouch$"
             ],
             "type": "string"
         },
         "close_date": {
-            "max": "2018-11-19 00:00:00",
-            "min": "1990-03-09 00:00:00",
+            "max": "2018-11-14 00:00:00",
+            "min": "2003-08-12 00:00:00",
             "type": "date"
         },
         "email": {
-            "max_length": 39,
+            "max_length": 37,
             "max_nulls": 0,
             "min_length": 14,
+            "no_duplicates": true,
             "rex": [
                 "^[a-z0-9]+\\@[a-z]+\\.com$",
                 "^[a-z0-9]+[\\.\\@][a-z0-9]+[\\.\\@][a-z]+\\.[a-z]{2,3}$",
                 "^[a-z]+\\.[a-z0-9]+\\@[a-z]+\\.co\\.uk$"
             ],
             "type": "string"
         },
@@ -95,14 +97,15 @@
             "rex": [
                 "^[A-Z][a-z]+$"
             ],
             "type": "string"
         },
         "home_tel": {
             "max_length": 13,
+            "max_nulls": 0,
             "min_length": 13,
             "no_duplicates": true,
             "rex": [
                 "^\\d{4} \\d{3} \\d{4}$"
             ],
             "type": "string"
         },
@@ -112,37 +115,40 @@
             "rex": [
                 "^[A-Z][a-z]+$"
             ],
             "type": "string"
         },
         "mobile_tel": {
             "max_length": 13,
+            "max_nulls": 0,
             "min_length": 13,
+            "no_duplicates": true,
             "rex": [
                 "^\\d{4} \\d{3} \\d{4}$"
             ],
             "type": "string"
         },
         "open_date": {
-            "max": "2018-11-19 00:00:00",
+            "max": "2018-11-17 00:00:00",
             "max_nulls": 0,
-            "min": "1970-01-01 00:00:00",
+            "min": "2002-10-02 00:00:00",
             "type": "date"
         },
         "overdraft_limit": {
             "max": 20000,
             "max_nulls": 0,
             "min": 0,
             "sign": "non-negative",
             "type": "int"
         },
         "postcode": {
             "max_length": 8,
-            "max_nulls": 1,
+            "max_nulls": 0,
             "min_length": 7,
+            "no_duplicates": true,
             "rex": [
                 "^[A-Z]{2}\\d{1,2} \\d[A-Z]{2}$"
             ],
             "type": "string"
         },
         "surname": {
             "max_length": 10,
```

### Comparing `tdda-2.1.2/tdda/constraints/examples/elements118.tdda` & `tdda-2.1.5/tdda/constraints/examples/testdata/elements92.tdda`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9658854166666666%*

 * *Differences: {"'fields'": "{'Z': {'max': 92}, 'Name': {'max_length': 12}, 'Symbol': {'max_length': 2}, "*

 * *             "'AtomicWeight': {'max': 238.028914, 'max_nulls': 0}, 'Etymology': {'max_length': 39, "*

 * *             "'max_nulls': 0}, 'RelativeAtomicMass': {'max': 238.028914, 'max_nulls': 0}, "*

 * *             "'MeltingPointC': {'max_nulls': 1}, 'MeltingPointKelvin': {'max_nulls': 1}, "*

 * *             "'BoilingPointC': {'max_nulls': 0}, 'BoilingPointF': {'max_nulls': 0}, 'Density': "*

 * *             "{'max': 22.610001, 'max_n […]*

```diff
@@ -1,23 +1,25 @@
 {
     "fields": {
         "AtomicWeight": {
-            "max": 294.0,
-            "max_nulls": 1,
+            "max": 238.028914,
+            "max_nulls": 0,
             "min": 1.007946,
             "sign": "positive",
             "type": "real"
         },
         "BoilingPointC": {
             "max": 5596.0,
+            "max_nulls": 0,
             "min": -268.93,
             "type": "real"
         },
         "BoilingPointF": {
             "max": 10105.0,
+            "max_nulls": 0,
             "min": -452.07,
             "type": "real"
         },
         "ChemicalSeries": {
             "allowed_values": [
                 "Actinoid",
                 "Alkali metal",
@@ -37,77 +39,80 @@
         },
         "Colour": {
             "max_length": 80,
             "min_length": 4,
             "type": "string"
         },
         "Density": {
-            "max": 41.0,
+            "max": 22.610001,
+            "max_nulls": 0,
             "min": 8.9e-05,
             "sign": "positive",
             "type": "real"
         },
         "Description": {
             "max_length": 83,
             "min_length": 1,
             "type": "string"
         },
         "Etymology": {
-            "max_length": 53,
-            "max_nulls": 1,
+            "max_length": 39,
+            "max_nulls": 0,
             "min_length": 4,
             "type": "string"
         },
         "Group": {
             "max": 18,
             "min": 1,
             "sign": "positive",
             "type": "int"
         },
         "MeltingPointC": {
             "max": 3675.0,
+            "max_nulls": 1,
             "min": -258.975,
             "type": "real"
         },
         "MeltingPointKelvin": {
             "max": 3948.0,
+            "max_nulls": 1,
             "min": 14.2,
             "sign": "positive",
             "type": "real"
         },
         "Name": {
-            "max_length": 13,
+            "max_length": 12,
             "max_nulls": 0,
             "min_length": 3,
             "no_duplicates": true,
             "type": "string"
         },
         "Period": {
             "max": 7,
             "max_nulls": 0,
             "min": 1,
             "sign": "positive",
             "type": "int"
         },
         "RelativeAtomicMass": {
-            "max": 294.0,
-            "max_nulls": 1,
+            "max": 238.028914,
+            "max_nulls": 0,
             "min": 1.007946,
             "sign": "positive",
             "type": "real"
         },
         "Symbol": {
-            "max_length": 3,
+            "max_length": 2,
             "max_nulls": 0,
             "min_length": 1,
             "no_duplicates": true,
             "type": "string"
         },
         "Z": {
-            "max": 118,
+            "max": 92,
             "max_nulls": 0,
             "min": 1,
             "no_duplicates": true,
             "sign": "positive",
             "type": "int"
         }
     }
```

### Comparing `tdda-2.1.2/tdda/constraints/examples/files_extension.py` & `tdda-2.1.5/tdda/constraints/examples/files_extension.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/simple_discovery.py` & `tdda-2.1.5/tdda/constraints/examples/simple_discovery.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/simple_verification.py` & `tdda-2.1.5/tdda/constraints/examples/simple_verification.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/testdata/accounts.zip` & `tdda-2.1.5/tdda/constraints/examples/testdata/accounts.zip`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/testdata/ddd.csv` & `tdda-2.1.5/tdda/constraints/examples/testdata/ddd.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/testdata/ddd.tdda` & `tdda-2.1.5/tdda/constraints/examples/testdata/ddd.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/testdata/elements118.csv` & `tdda-2.1.5/tdda/constraints/examples/testdata/elements118.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/testdata/elements118.feather` & `tdda-2.1.5/tdda/constraints/examples/testdata/elements118.feather`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/testdata/elements118.pmm` & `tdda-2.1.5/tdda/constraints/examples/testdata/elements118.pmm`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/testdata/elements92.csv` & `tdda-2.1.5/tdda/constraints/examples/testdata/elements92.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/examples/testdata/elements92.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements92.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/extension.py` & `tdda-2.1.5/tdda/constraints/extension.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/flags.py` & `tdda-2.1.5/tdda/constraints/flags.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
       Specify original columns to write out.
   * --interleave
       In the output, place the verification fields immediately after
       the original field to which they correspond.
   * --index
       Include a row-number index in the output file.
       The row number is automatically included if no output fields are
-      specified. Rows are usually numbered from 1, unless the (feather)
+      specified. Rows are usually numbered from 1, unless the
       input file already has an index.
 
 '''
 
 def discover_parser(usage=''):
     formatter = argparse.RawDescriptionHelpFormatter
     parser = argparse.ArgumentParser(prog='tdda discover',
```

### Comparing `tdda-2.1.2/tdda/constraints/pd/constraints.py` & `tdda-2.1.5/tdda/constraints/pd/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,32 +26,24 @@
 import datetime
 import os
 import re
 import sys
 
 from collections import OrderedDict
 
+from tdda.deprecated.featherfiles import read_feather_file, write_feather_file
+
 try:
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 import numpy as np
 import pandas as pd
 
-try:
-    from pmmif import featherpmm
-except ImportError:
-    featherpmm = None
-
-try:
-    import feather as feather
-except ImportError:
-    feather = None
-
 from tdda.constraints.base import (
     STANDARD_FIELD_CONSTRAINTS,
     STANDARD_CONSTRAINT_SUFFIXES,
     CONSTRAINT_SUFFIX_MAP,
     native_definite,
     DatasetConstraints,
     Verification,
@@ -1166,23 +1158,15 @@
     exists = os.path.exists(os.path.expanduser(path))
     stem, ext = os.path.splitext(path)
     lcstem, ext = stem.lower(), ext.lower()
 
     if ext == '.parquet':
         return pd.read_parquet(path)
     elif ext == '.feather':
-        if featherpmm and feather:
-            ds = featherpmm.read_dataframe(path)
-            return ds.df
-        elif feather:
-            return feather.read_dataframe(path)
-        else:
-            raise Exception('The Python feather module is not installed.\n'
-                            'Use:\n    pip install feather-format\n'
-                            'to add capability.\n')
+        return read_feather_file(path)
 
     if mdpath is None:
         md_type, _ = find_metadata_type_from_path(path)
         if md_type:
             # path is a metadata file of a known type
             # load the metadata from it and get the file path, if any
             # from the metadata file
@@ -1218,25 +1202,18 @@
         print(default_csv_writer(df, None, index=index))
     else:
         fmt = file_format(path)
     if fmt == 'parquet':
         df.to_parquet(path=path, index=False)
     elif fmt in ('csv', 'psv', 'tsv', 'txt'):
         default_csv_writer(df, path, index=index)
-    elif fmt != 'feather':
-        raise Exception(f'Unknown output format: {fmt}')
-    elif featherpmm and feather:
-        featherpmm.write_dataframe(featherpmm.Dataset(df, name='verification'),
-                                   path)
-    elif feather:
-        feather.write_dataframe(df, path)
+    elif fmt == 'feather':
+        write_feather_file(df, path, name='verification')
     else:
-        raise Exception('The Python feather module is not installed.\n'
-                        'Use:\n    pip install feather-format\n'
-                        'to add capability.\n')
+        raise Exception(f'Unknown output format: {fmt}')
 
 
 def unique_column_name(df, name):
     """
     Generate a column name that is not already present in the dataframe.
     """
     i = 1
```

### Comparing `tdda-2.1.2/tdda/constraints/pd/detect.py` & `tdda-2.1.5/tdda/constraints/pd/detect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # -*- coding: utf-8 -*-
 
 """
 Support for Pandas constraint detection from the command-line tool
 
 Detect constraints using CSV files, or Pandas or R DataFrames saved as
-feather files, against a constraints from .tdda JSON constraints file.
+parquet files, against a constraints from .tdda JSON constraints file.
 """
 
 USAGE = '''
 
 Parameters:
 
   * input is one of:
 
       - a csv file
       - a .parquet file
-      - a feather file containing a Pandas or R DataFrame (deprecated(
       - any of the other supported data sources
 
   * constraints.tdda, if provided, is a JSON .tdda file constaining
     constraints.
 
-  * name of output file (.csv,  .parqet or .feather (deprecated))
+  * name of output file (.csv, .parqet)
     where detection results are to be written.
     Can be - (or missing) to write to standard output.
 
 '''
 
 import os
 import sys
@@ -34,23 +33,14 @@
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 import pandas as pd
 import numpy as np
 
-try:
-    from pmmif import featherpmm
-except ImportError:
-    featherpmm = None
-    try:
-        import feather as feather
-    except ImportError:
-        feather = None
-
 from tdda import __version__
 from tdda.constraints.flags import detect_parser, detect_flags
 from tdda.constraints.pd.constraints import detect_df, load_df, file_format
 
 
 def detect_df_from_file(df_path, constraints_path, outpath,
                         verbose=True, **kwargs):
@@ -71,15 +61,15 @@
     if verbose and outpath is not None and outpath != '-':
         print(v)
     return v
 
 
 def pd_detect_parser():
     parser = detect_parser(USAGE)
-    parser.add_argument('input', help='CSV, parquet or feather file')
+    parser.add_argument('input', help='CSV, parquet')
     parser.add_argument('constraints', nargs='?',
                         help='constraints file to verify against')
     parser.add_argument('outpath', nargs='?',
                         help='file to write detection results to')
     return parser
```

### Comparing `tdda-2.1.2/tdda/constraints/pd/discover.py` & `tdda-2.1.5/tdda/constraints/pd/discover.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 # -*- coding: utf-8 -*-
 
 """
 Support for Pandas constraint discovery from the command-line tool
 
 Discover TDDA constraints for CSV files, and for Pandas or R DataFrames saved
-as feather files, and save the generated constraints as a .tdda JSON file.
+as parquetfiles, and save the generated constraints as a .tdda JSON file.
 """
 
 USAGE = '''
 
 Parameters:
 
   * input is one of:
 
     - a csv file
     - a .parquet file
-    - a .feather file containing a saved Pandas or R DataFrame (deprecated)
     - any of the other supported data sources
 
   * constraints.tdda, if provided, specifies the name of a file to
     which the generated constraints will be written.  Can be - (or missing)
     to write to standard output.
 
 '''
 
 import os
 import sys
 
 try:
-    from pmmif import featherpmm
-except ImportError:
-    featherpmm = None
-    try:
-        import feather as feather
-    except ImportError:
-        feather = None
-
-try:
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 from tdda import __version__
 from tdda.constraints.flags import discover_parser, discover_flags
 from tdda.constraints.pd.constraints import discover_df, load_df
@@ -65,15 +55,15 @@
         print(output)
     return output
 
 
 def pd_discover_parser():
     parser = discover_parser(USAGE)
     parser.add_argument('input', nargs=1,
-                        help='CSV, parquet (or feather, deprecated) file')
+                        help='CSV or parquet file')
     parser.add_argument('constraints', nargs='?',
                         help='name of constraints file to create')
     return parser
 
 
 def pd_discover_params(args):
     parser = pd_discover_parser()
```

### Comparing `tdda-2.1.2/tdda/constraints/pd/extension.py` & `tdda-2.1.5/tdda/constraints/pd/extension.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,18 +27,18 @@
             if (ext in ('.csv', '.psv', '.tsv', '.parquet', '.feather'
                         '.json', '.yaml')):
                 return True
         return False
 
     def help(self, stream=sys.stdout):
         print('  - Flat files (filename.csv)', file=stream)
-        print('  - Pandas DataFrames (filename.feather)', file=stream)
+        print('  - Pandas DataFrames (filename.parquet)', file=stream)
 
     def spec(self):
-        return 'a CSV file or a .feather file'
+        return 'a CSV file or a .parquet file'
 
     def discover(self):
         return PandasDiscoverer(self.argv, verbose=self.verbose).discover()
 
     def verify(self):
         return PandasVerifier(self.argv, verbose=self.verbose).verify()
```

### Comparing `tdda-2.1.2/tdda/constraints/pd/testpdconstraints.py` & `tdda-2.1.5/tdda/constraints/pd/testpdconstraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/pd/verify.py` & `tdda-2.1.5/tdda/constraints/pd/verify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 
 """
 Support for Pandas constraint verification from the command-line tool
 
 Verify constraints using CSV files, or Pandas or R DataFrames saved as
-feather files, against a constraints from .tdda JSON constraints file.
+parquet files, against a constraints from .tdda JSON constraints file.
 """
 
 USAGE = '''
 
 Parameters:
 
   * input is one of:
 
       - a csv file. Can be - to read from standard input.
       - a parquet file
-      - a feather file containing a Pandas or R DataFrame (deprecated).
       - any of the other supported data sources
 
   * constraints.tdda, if provided, is a JSON .tdda file constaining
     constraints.
 
 If no constraints file is provided, a file with the same path as the
 input file, with a .tdda extension will be tried.
@@ -33,23 +32,14 @@
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 import pandas as pd
 import numpy as np
 
-try:
-    from pmmif import featherpmm
-except ImportError:
-    featherpmm = None
-    try:
-        import feather as feather
-    except ImportError:
-        feather = None
-
 from tdda import __version__
 from tdda.constraints.flags import verify_parser, verify_flags
 from tdda.constraints.pd.constraints import verify_df, load_df
 
 
 def verify_df_from_file(df_path, constraints_path, verbose=True, **kwargs):
     if df_path == '-' or df_path is None:
@@ -66,15 +56,15 @@
     if verbose:
         print(v)
     return v
 
 
 def pd_verify_parser():
     parser = verify_parser(USAGE)
-    parser.add_argument('input', nargs=1, help='CSV, parquet, or feather file')
+    parser.add_argument('input', nargs=1, help='CSV or parquet file')
     parser.add_argument('constraints', nargs='?',
                         help='constraints file to verify against')
     return parser
 
 
 def pd_verify_params(args):
     parser = pd_verify_parser()
```

### Comparing `tdda-2.1.2/tdda/constraints/tdda_json_file_format.md` & `tdda-2.1.5/tdda/constraints/tdda_json_file_format.md`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testbase.py` & `tdda-2.1.5/tdda/constraints/testbase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testconstraints.py` & `tdda-2.1.5/tdda/constraints/testconstraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/d.csv` & `tdda-2.1.5/tdda/constraints/testdata/d.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/ddd.csv` & `tdda-2.1.5/tdda/constraints/testdata/ddd.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/ddd.tdda` & `tdda-2.1.5/tdda/constraints/testdata/ddd.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline-interleaved.csv` & `tdda-2.1.5/tdda/constraints/testdata/detect-els-cmdline-interleaved.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline.csv` & `tdda-2.1.5/tdda/constraints/testdata/detect-els-cmdline.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline2.csv` & `tdda-2.1.5/tdda/constraints/testdata/detect-els-cmdline2.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118.csv` & `tdda-2.1.5/tdda/constraints/testdata/elements118.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118.df` & `tdda-2.1.5/tdda/constraints/testdata/elements118.df`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118.feather` & `tdda-2.1.5/tdda/constraints/testdata/elements118.feather`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118.parquet` & `tdda-2.1.5/tdda/constraints/examples/elements118.parquet`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118.pmm` & `tdda-2.1.5/tdda/constraints/testdata/elements118.pmm`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements118.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_csv.csv` & `tdda-2.1.5/tdda/constraints/testdata/elements118_detect_from_csv.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_feather.csv` & `tdda-2.1.5/tdda/constraints/testdata/elements118_detect_from_feather.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_feather.feather` & `tdda-2.1.5/tdda/constraints/testdata/elements118_detect_from_feather.feather`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118oldrex-3.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements118oldrex-3.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118oldrex.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements118oldrex.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118rex-3.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements118rex-3.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118rex.df` & `tdda-2.1.5/tdda/constraints/testdata/elements118rex.df`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118rex.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements118rex.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect.df` & `tdda-2.1.5/tdda/constraints/testdata/elements118rex_detect.df`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect_perc.csv` & `tdda-2.1.5/tdda/constraints/testdata/elements118rex_detect_perc.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements92.csv` & `tdda-2.1.5/tdda/constraints/testdata/elements92.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements92.parquet` & `tdda-2.1.5/tdda/constraints/examples/elements92.parquet`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements92_pandas.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements92_pandas.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements92oldrex.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements92oldrex.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/elements92rex.tdda` & `tdda-2.1.5/tdda/constraints/testdata/elements92rex.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/example.csv` & `tdda-2.1.5/tdda/constraints/testdata/example.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/example.db` & `tdda-2.1.5/tdda/constraints/testdata/example.db`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/example.sql` & `tdda-2.1.5/tdda/constraints/testdata/example.sql`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/ref-accounts1k.tdda` & `tdda-2.1.5/tdda/constraints/testdata/ref-accounts1k.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/ref-accounts25k.tdda` & `tdda-2.1.5/tdda/constraints/testdata/ref-accounts25k.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/constraints/testdata/ref-detect25k-failures.txt` & `tdda-2.1.5/tdda/constraints/testdata/ref-detect25k-failures.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/examples.py` & `tdda-2.1.5/tdda/examples.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/README.md` & `tdda-2.1.5/tdda/gentest/examples/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/0-set-variables.R` & `tdda-2.1.5/tdda/gentest/examples/r-examples/0-set-variables.R`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/2-compute-cumulative-percentiles.R` & `tdda-2.1.5/tdda/gentest/examples/r-examples/2-compute-cumulative-percentiles.R`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/3-parametric-regression.R` & `tdda-2.1.5/tdda/gentest/examples/r-examples/3-parametric-regression.R`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/4-non-parametric-regression.R` & `tdda-2.1.5/tdda/gentest/examples/r-examples/4-non-parametric-regression.R`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/README.md` & `tdda-2.1.5/tdda/gentest/examples/r-examples/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/env.data.or.txt` & `tdda-2.1.5/tdda/gentest/examples/r-examples/env.data.or.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/env.data.txt` & `tdda-2.1.5/tdda/gentest/examples/r-examples/env.data.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/site.species.or.txt` & `tdda-2.1.5/tdda/gentest/examples/r-examples/site.species.or.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/gentest/examples/r-examples/site.species.txt` & `tdda-2.1.5/tdda/gentest/examples/r-examples/site.species.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/__init__.py` & `tdda-2.1.5/tdda/referencetest/__init__.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/basecomparison.py` & `tdda-2.1.5/tdda/referencetest/basecomparison.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/captureoutput.py` & `tdda-2.1.5/tdda/referencetest/captureoutput.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/checkfiles.py` & `tdda-2.1.5/tdda/referencetest/checkfiles.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/checkpandas.py` & `tdda-2.1.5/tdda/referencetest/checkpandas.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/diffrex.py` & `tdda-2.1.5/tdda/referencetest/diffrex.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/README.md` & `tdda-2.1.5/tdda/referencetest/examples/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/dataframes.py` & `tdda-2.1.5/tdda/referencetest/examples/dataframes.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/expected.html` & `tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise1/expected.html`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/generators.py` & `tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise1/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/expected.html` & `tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise2/expected.html`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/generators.py` & `tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise2/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/test_all.py` & `tdda-2.1.5/tdda/referencetest/examples/exercises-pytest/exercise2/test_all.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/expected.html` & `tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise1/expected.html`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/generators.py` & `tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise1/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/test_all.py` & `tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise1/test_all.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/expected.html` & `tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise2/expected.html`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/generators.py` & `tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise2/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/test_all.py` & `tdda-2.1.5/tdda/referencetest/examples/exercises-unittest/exercise2/test_all.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/generators.py` & `tdda-2.1.5/tdda/referencetest/examples/generators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-# -*- coding: utf-8 -*-
 """
 generators.py: Trivial result generation functions for illustrating
                tdda.referencetest
 
 Source repository: http://github.com/tdda/tdda
 
 License: MIT
 
-Copyright (c) Stochastic Solutions Limited 2016
+Copyright (c) Stochastic Solutions Limited 2016-2024
 """
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
-
 import datetime
 import math
 
+
 def generate_string():
     """
     Returns an HTML string that should display identically to the result
     stored in tdda/examples/reference/string_result, but which has
     four (non-semantic) differences:
         - The Copyright line is different
         - The version number line is different
         - It has a newline at the top, unlike the reference file.
         - It is missing a newline at the end of the string, which the
           reference file includes.
     """
     version = '1.0.0'
-    copyright_year = '2016'
+    copyright_year = str(datetime.date.today().year)
     inc_gendate = False
     date = datetime.datetime.now().strftime('    %Y-%m-%dT%H:%M:%S')
     generation_date = date if inc_gendate else ''
     spiral = generate_spiral()
 
     return """<!DOCTYPE html>
 <html>
@@ -65,19 +61,20 @@
   </div>
 </body>
 </html>
 """ % locals()
 
 
 def generate_file(path):
+    year = str(datetime.date.today().year)
     html = '''<!DOCTYPE html>
 <html>
   <head>
     <!--
-    Copyright (c) Stochastic Solutions, 2016
+    Copyright (c) Stochastic Solutions, %s
     Version 1.0.0
     -->
     <meta charset="UTF-8"/>
     <style type="text/css">
       body {font-family: Palatino, "Palatino Linotype", Times;
             text-align: center;}
       h1 {font-size: large; text-align: center;}
@@ -109,15 +106,15 @@
   </svg>
 
   <div>
     It will serve to illustrate tdda.referencetest.
   </div>
 </body>
 </html>
-'''
+''' % year
     with open(path, 'w') as f:
         f.write(html)
 
 
 def generate_spiral():
     points = ' '.join('%d %d L' % (t / 20 * math.cos(t * 2 * math.pi / 100),
                                    t / 20 * math.sin(t * 2 * math.pi / 100))
```

### Comparing `tdda-2.1.2/tdda/referencetest/examples/pytest/conftest.py` & `tdda-2.1.5/tdda/referencetest/examples/pytest/conftest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/pytest/test_using_referencepytest.py` & `tdda-2.1.5/tdda/referencetest/examples/pytest/test_using_referencepytest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/reference/dataframe_result.csv` & `tdda-2.1.5/tdda/referencetest/examples/reference/dataframe_result.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/reference/dataframe_result2.csv` & `tdda-2.1.5/tdda/referencetest/examples/reference/dataframe_result2.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/reference/file_result.html` & `tdda-2.1.5/tdda/referencetest/examples/reference/file_result.html`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/reference/string_result.html` & `tdda-2.1.5/tdda/referencetest/examples/reference/string_result.html`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples/unittest/test_using_referencetestcase.py` & `tdda-2.1.5/tdda/referencetest/examples/unittest/test_using_referencetestcase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/examples.py` & `tdda-2.1.5/tdda/referencetest/examples.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/gentest.py` & `tdda-2.1.5/tdda/referencetest/gentest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/gentest_boilerplate.py` & `tdda-2.1.5/tdda/referencetest/gentest_boilerplate.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/pddates.py` & `tdda-2.1.5/tdda/referencetest/pddates.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/pytestconfig.py` & `tdda-2.1.5/tdda/referencetest/pytestconfig.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/referencepytest.py` & `tdda-2.1.5/tdda/referencetest/referencepytest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/referencetest.py` & `tdda-2.1.5/tdda/referencetest/referencetest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/referencetestcase.py` & `tdda-2.1.5/tdda/referencetest/referencetestcase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/tests/testbase.py` & `tdda-2.1.5/tdda/referencetest/tests/testbase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/tests/testdata/colours.txt` & `tdda-2.1.5/tdda/referencetest/tests/testdata/colours.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/tests/testfiles.py` & `tdda-2.1.5/tdda/referencetest/tests/testfiles.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/tests/testpandas.py` & `tdda-2.1.5/tdda/referencetest/tests/testpandas.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/tests/testregeneration.py` & `tdda-2.1.5/tdda/referencetest/tests/testregeneration.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/tests/teststrings.py` & `tdda-2.1.5/tdda/referencetest/tests/teststrings.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/referencetest/utils.py` & `tdda-2.1.5/tdda/referencetest/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     filetype = filetype or FileType(path)
     if filetype.binary:
         return
     enc = filetype.encoding if filetype else None
     try:
         with open(path, encoding=enc) as f:
             return f.readlines()
+        if filetype.is_unknown():
+            filetype.text = True
     except UnicodeDecodeError:
         if filetype.text:  # really was expecting text
             try:
                 with open(path, encoding='iso-8859-1') as f:
                     lines = f.readlines()
                     filetype.encoding = 'iso-8859-1'
                     return lines
```

### Comparing `tdda-2.1.2/tdda/rexpy/examples/agents9.txt` & `tdda-2.1.5/tdda/rexpy/examples/agents9.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/rexpy/rexpy.py` & `tdda-2.1.5/tdda/rexpy/rexpy.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/rexpy/seq.py` & `tdda-2.1.5/tdda/rexpy/seq.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/rexpy/testhypo.py` & `tdda-2.1.5/tdda/rexpy/testhypo.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/rexpy/testrexpy.py` & `tdda-2.1.5/tdda/rexpy/testrexpy.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/rexpy/testseq.py` & `tdda-2.1.5/tdda/rexpy/testseq.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/serial/base.py` & `tdda-2.1.5/tdda/serial/base.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/serial/cli.py` & `tdda-2.1.5/tdda/serial/cli.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/serial/csvw.py` & `tdda-2.1.5/tdda/serial/csvw.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/serial/pandasio.py` & `tdda-2.1.5/tdda/serial/pandasio.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/serial/reader.py` & `tdda-2.1.5/tdda/serial/reader.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/serial/testserialmetadata.py` & `tdda-2.1.5/tdda/serial/testserialmetadata.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/serial/utils.py` & `tdda-2.1.5/tdda/serial/utils.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/testconfig.py` & `tdda-2.1.5/tdda/testconfig.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda/testtdda.py` & `tdda-2.1.5/tdda/testtdda.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,12 +21,13 @@
     print('Performing configuration tests (reporting)', file=sys.stderr)
     from tdda.testconfig import *
 else:
     pass
 
 
 def testall(module=None, argv=None):
+    os.environ['TDDA_TESTING'] = 'TRUE'
     ReferenceTestCase.main(module=module, argv=argv)
 
 
 if __name__ == '__main__':
     testall(argv=sys.argv)
```

### Comparing `tdda-2.1.2/tdda/writabletestcase.py` & `tdda-2.1.5/tdda/writabletestcase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.1.2/tdda.egg-info/PKG-INFO` & `tdda-2.1.5/tdda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdda
-Version: 2.1.2
+Version: 2.1.5
 Home-page: http://www.stochasticsolutions.com
 Download-URL: https://github.com/tdda/tdda
 Author: Simon Brown
 Author-email: Nick Radcliffe <njr@stochasticsolutions.com>
 License: MIT
 Keywords: tdda constraint referencetest rexpy
 Requires-Python: >=3.8
```

### Comparing `tdda-2.1.2/tdda.egg-info/SOURCES.txt` & `tdda-2.1.5/tdda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,42 +36,46 @@
 tdda/constraints/db/detect.py
 tdda/constraints/db/discover.py
 tdda/constraints/db/drivers.py
 tdda/constraints/db/extension.py
 tdda/constraints/db/testdbconstraints.py
 tdda/constraints/db/verify.py
 tdda/constraints/examples/README.md
-tdda/constraints/examples/accounts25k.tdda
 tdda/constraints/examples/accounts_detect_25k_against_1k.py
 tdda/constraints/examples/accounts_discover_1k.py
 tdda/constraints/examples/accounts_verify_1k.py
 tdda/constraints/examples/accounts_verify_25k.py
 tdda/constraints/examples/accounts_verify_25k_against_1k.py
-tdda/constraints/examples/accounts_verify_25k_against_1k_feather.py
+tdda/constraints/examples/accounts_verify_25k_against_1k_parquet.py
 tdda/constraints/examples/accounts_verify_25k_to_frame.py
-tdda/constraints/examples/elements118.tdda
+tdda/constraints/examples/elements118.parquet
+tdda/constraints/examples/elements92.parquet
 tdda/constraints/examples/elements_detect_118_against_92.py
 tdda/constraints/examples/elements_discover_92.py
 tdda/constraints/examples/elements_verify_118.py
 tdda/constraints/examples/elements_verify_118_against_92.py
-tdda/constraints/examples/elements_verify_118_against_92_feather.py
+tdda/constraints/examples/elements_verify_118_against_92_parquet.py
 tdda/constraints/examples/elements_verify_92.py
 tdda/constraints/examples/files_extension.py
 tdda/constraints/examples/simple_discovery.py
 tdda/constraints/examples/simple_verification.py
 tdda/constraints/examples/simple_verify_fail.py
 tdda/constraints/examples/simple_verify_pass.py
 tdda/constraints/examples/testdata/accounts.zip
 tdda/constraints/examples/testdata/accounts1k.tdda
+tdda/constraints/examples/testdata/accounts25k.parquet
 tdda/constraints/examples/testdata/ddd.csv
 tdda/constraints/examples/testdata/ddd.tdda
 tdda/constraints/examples/testdata/elements118.csv
 tdda/constraints/examples/testdata/elements118.feather
+tdda/constraints/examples/testdata/elements118.parquet
 tdda/constraints/examples/testdata/elements118.pmm
+tdda/constraints/examples/testdata/elements118.tdda
 tdda/constraints/examples/testdata/elements92.csv
+tdda/constraints/examples/testdata/elements92.parquet
 tdda/constraints/examples/testdata/elements92.tdda
 tdda/constraints/pd/__init__.py
 tdda/constraints/pd/constraints.py
 tdda/constraints/pd/detect.py
 tdda/constraints/pd/discover.py
 tdda/constraints/pd/extension.py
 tdda/constraints/pd/testpdconstraints.py
@@ -109,14 +113,19 @@
 tdda/constraints/testdata/example.csv
 tdda/constraints/testdata/example.db
 tdda/constraints/testdata/example.sql
 tdda/constraints/testdata/ref-accounts1k.tdda
 tdda/constraints/testdata/ref-accounts25k.tdda
 tdda/constraints/testdata/ref-detect25k-failures.txt
 tdda/constraints/testdata/sqlite.conn
+tdda/deprecated/__init__.py
+tdda/deprecated/featherfiles.py
+tdda/deprecated/examples/__init__.py
+tdda/deprecated/examples/generators.py
+tdda/deprecated/examples/test_using_writabletestcase.py
 tdda/gentest/__init__.py
 tdda/gentest/examples/README.md
 tdda/gentest/examples/example2.sh
 tdda/gentest/examples/hey
 tdda/gentest/examples/r-examples/0-set-variables.R
 tdda/gentest/examples/r-examples/00-install.R
 tdda/gentest/examples/r-examples/1-compute-weighted-average-tolerance-values.R
```

