# Comparing `tmp/slip39-9.0.4.tar.gz` & `tmp/slip39-9.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slip39-9.0.4.tar", last modified: Sun Oct  2 13:17:51 2022, max compression
+gzip compressed data, was "slip39-9.1.2.tar", last modified: Mon Oct 17 22:28:22 2022, max compression
```

## Comparing `slip39-9.0.4.tar` & `slip39-9.1.2.tar`

### file list

```diff
@@ -1,81 +1,101 @@
-drwxrwxr-x   0 perry     (1002) kundert   (1004)        0 2022-10-02 13:17:51.496258 slip39-9.0.4/
--rw-rw-r--   0 perry     (1002) kundert   (1004)    35147 2021-12-27 14:01:50.000000 slip39-9.0.4/COPYING
--rw-rw-r--   0 perry     (1002) kundert   (1004)     1154 2021-12-27 14:01:50.000000 slip39-9.0.4/LICENSE
--rw-rw-r--   0 perry     (1002) kundert   (1004)      176 2022-02-12 14:07:55.000000 slip39-9.0.4/MANIFEST.in
--rw-rw-r--   0 perry     (1002) kundert   (1004)    10734 2022-10-02 13:17:51.496258 slip39-9.0.4/PKG-INFO
--rw-rw-r--   0 perry     (1002) kundert   (1004)    88509 2022-10-02 13:03:13.000000 slip39-9.0.4/README.org
--rw-rw-r--   0 perry     (1002) kundert   (1004)   876808 2022-10-02 13:03:13.000000 slip39-9.0.4/README.pdf
--rw-rw-r--   0 perry     (1002) kundert   (1004)   103599 2022-10-02 13:03:13.000000 slip39-9.0.4/README.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      104 2021-12-27 14:01:50.000000 slip39-9.0.4/pyproject.toml
--rw-rw-r--   0 perry     (1002) kundert   (1004)       78 2022-03-11 11:33:27.000000 slip39-9.0.4/requirements-dev.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)       20 2022-02-12 14:07:55.000000 slip39-9.0.4/requirements-gui.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)       16 2022-02-12 14:07:55.000000 slip39-9.0.4/requirements-serial.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)       14 2022-02-24 17:42:09.000000 slip39-9.0.4/requirements-tests.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)       48 2022-02-24 17:42:09.000000 slip39-9.0.4/requirements-wallet.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      183 2022-10-02 13:03:13.000000 slip39-9.0.4/requirements.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)       38 2022-10-02 13:17:51.496258 slip39-9.0.4/setup.cfg
--rw-rw-r--   0 perry     (1002) kundert   (1004)    15950 2022-10-02 13:03:13.000000 slip39-9.0.4/setup.py
-drwxrwxr-x   0 perry     (1002) kundert   (1004)        0 2022-10-02 13:17:51.488258 slip39-9.0.4/slip39/
--rw-rw-r--   0 perry     (1002) kundert   (1004)      174 2022-10-02 13:03:10.000000 slip39-9.0.4/slip39/__init__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)       55 2021-12-27 14:01:50.000000 slip39-9.0.4/slip39/__main__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)    39673 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/api.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)    10100 2022-02-12 14:07:55.000000 slip39-9.0.4/slip39/api_passphrase_test.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)    16493 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/api_test.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)     4298 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/defaults.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)     5918 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/dependency_test.py
-drwxrwxr-x   0 perry     (1002) kundert   (1004)        0 2022-10-02 13:17:51.488258 slip39-9.0.4/slip39/generator/
--rw-rw-r--   0 perry     (1002) kundert   (1004)    10640 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/generator/__init__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)       55 2022-02-12 14:07:55.000000 slip39-9.0.4/slip39/generator/__main__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)    16830 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/generator/main.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)     4272 2022-10-02 13:03:10.000000 slip39-9.0.4/slip39/generator_test.py
-drwxrwxr-x   0 perry     (1002) kundert   (1004)        0 2022-10-02 13:17:51.492258 slip39-9.0.4/slip39/gui/
--rw-rw-r--   0 perry     (1002) kundert   (1004)     3188 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/SLIP-39-AS-BIP.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     1847 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/SLIP-39-CRYPTO.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      716 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/SLIP-39-CS.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     1613 2022-03-11 11:33:27.000000 slip39-9.0.4/slip39/gui/SLIP-39-G-NAME.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     1460 2022-03-11 11:33:27.000000 slip39-9.0.4/slip39/gui/SLIP-39-G.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     2986 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/SLIP-39-LO.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     2223 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/SLIP-39-PASSPHRASE.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      611 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/SLIP-39-PF.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     4433 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/SLIP-39-SD.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     1719 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/SLIP-39-SE.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      215 2022-03-11 11:33:27.000000 slip39-9.0.4/slip39/gui/SLIP-39-THRESHOLD.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     2491 2022-03-11 11:33:27.000000 slip39-9.0.4/slip39/gui/SLIP-39-WALLET.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      834 2022-04-10 22:49:46.000000 slip39-9.0.4/slip39/gui/SLIP-39.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)        0 2022-02-12 14:07:55.000000 slip39-9.0.4/slip39/gui/__init__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)       55 2022-02-12 14:07:55.000000 slip39-9.0.4/slip39/gui/__main__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)    66936 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/gui/main.py
-drwxrwxr-x   0 perry     (1002) kundert   (1004)        0 2022-10-02 13:17:51.492258 slip39-9.0.4/slip39/layout/
--rw-rw-r--   0 perry     (1002) kundert   (1004)       68 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/layout/1x1-ffffff3f.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)       68 2022-02-24 17:42:09.000000 slip39-9.0.4/slip39/layout/1x1-ffffff54.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)       68 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/layout/1x1-ffffffbf.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)    40663 2022-03-11 11:33:27.000000 slip39-9.0.4/slip39/layout/BNB.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)    27493 2022-02-24 17:42:09.000000 slip39-9.0.4/slip39/layout/BTC.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)      989 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/layout/COVER-BIP-39.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      710 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/layout/COVER-SLIP-39.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)     1140 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/layout/COVER.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)    44316 2022-03-11 11:33:27.000000 slip39-9.0.4/slip39/layout/CRO.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)    22020 2022-02-24 17:42:09.000000 slip39-9.0.4/slip39/layout/DOGE.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)    30750 2022-02-24 17:42:09.000000 slip39-9.0.4/slip39/layout/ETH.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)    21913 2022-02-24 17:42:09.000000 slip39-9.0.4/slip39/layout/LTC.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)   111308 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/layout/SLIP-39.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)    43289 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/layout/XRP.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)    48335 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/layout/__init__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)   274581 2022-02-24 17:42:09.000000 slip39-9.0.4/slip39/layout/paper-wallet-background.png
--rw-rw-r--   0 perry     (1002) kundert   (1004)     9669 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/main.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)     2590 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/output_test.py
-drwxrwxr-x   0 perry     (1002) kundert   (1004)        0 2022-10-02 13:17:51.492258 slip39-9.0.4/slip39/recovery/
--rw-rw-r--   0 perry     (1002) kundert   (1004)     5180 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/recovery/__init__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)       55 2022-10-02 13:03:10.000000 slip39-9.0.4/slip39/recovery/__main__.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)     6193 2022-10-02 13:16:47.000000 slip39-9.0.4/slip39/recovery/main.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)    14683 2022-10-02 13:03:13.000000 slip39-9.0.4/slip39/recovery_test.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)     5358 2022-10-02 13:03:10.000000 slip39-9.0.4/slip39/util.py
--rw-rw-r--   0 perry     (1002) kundert   (1004)       88 2022-10-02 13:16:47.000000 slip39-9.0.4/slip39/version.py
-drwxrwxr-x   0 perry     (1002) kundert   (1004)        0 2022-10-02 13:17:51.496258 slip39-9.0.4/slip39.egg-info/
--rw-rw-r--   0 perry     (1002) kundert   (1004)    10734 2022-10-02 13:17:51.000000 slip39-9.0.4/slip39.egg-info/PKG-INFO
--rw-rw-r--   0 perry     (1002) kundert   (1004)     1810 2022-10-02 13:17:51.000000 slip39-9.0.4/slip39.egg-info/SOURCES.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)        1 2022-10-02 13:17:51.000000 slip39-9.0.4/slip39.egg-info/dependency_links.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      168 2022-10-02 13:17:51.000000 slip39-9.0.4/slip39.egg-info/entry_points.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)      352 2022-10-02 13:17:51.000000 slip39-9.0.4/slip39.egg-info/requires.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)        7 2022-10-02 13:17:51.000000 slip39-9.0.4/slip39.egg-info/top_level.txt
--rw-rw-r--   0 perry     (1002) kundert   (1004)        1 2022-03-02 20:34:41.000000 slip39-9.0.4/slip39.egg-info/zip-safe
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2022-10-17 22:28:22.537156 slip39-9.1.2/
+-rw-rw-r--   0 perry      (501) staff       (20)    35147 2021-12-22 19:42:56.000000 slip39-9.1.2/COPYING
+-rw-rw-r--   0 perry      (501) staff       (20)     1154 2021-12-22 23:18:16.000000 slip39-9.1.2/LICENSE
+-rw-rw-r--   0 perry      (501) staff       (20)      176 2022-02-17 12:55:48.000000 slip39-9.1.2/MANIFEST.in
+-rw-rw-r--   0 perry      (501) staff       (20)    10734 2022-10-17 22:28:22.536534 slip39-9.1.2/PKG-INFO
+-rw-rw-r--   0 perry      (501) staff       (20)    90871 2022-10-17 22:27:51.000000 slip39-9.1.2/README.org
+-rw-rw-r--   0 perry      (501) staff       (20)   875826 2022-10-17 22:27:51.000000 slip39-9.1.2/README.pdf
+-rw-rw-r--   0 perry      (501) staff       (20)   101382 2022-10-17 22:27:51.000000 slip39-9.1.2/README.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      104 2021-12-22 20:43:01.000000 slip39-9.1.2/pyproject.toml
+-rw-rw-r--   0 perry      (501) staff       (20)       87 2022-10-17 22:27:51.000000 slip39-9.1.2/requirements-dev.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       20 2022-10-17 22:27:51.000000 slip39-9.1.2/requirements-gui.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       16 2022-02-01 19:41:34.000000 slip39-9.1.2/requirements-serial.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       14 2022-02-16 23:41:11.000000 slip39-9.1.2/requirements-tests.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       46 2022-10-17 22:27:51.000000 slip39-9.1.2/requirements-wallet.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      184 2022-10-17 22:27:51.000000 slip39-9.1.2/requirements.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       38 2022-10-17 22:28:22.537315 slip39-9.1.2/setup.cfg
+-rw-rw-r--   0 perry      (501) staff       (20)    15980 2022-10-17 22:27:51.000000 slip39-9.1.2/setup.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2022-10-17 22:28:22.456977 slip39-9.1.2/slip39/
+-rw-rw-r--   0 perry      (501) staff       (20)      941 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)       55 2021-12-22 13:15:21.000000 slip39-9.1.2/slip39/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)    40978 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/api.py
+-rw-rw-r--   0 perry      (501) staff       (20)    10100 2022-02-04 15:11:13.000000 slip39-9.1.2/slip39/api_passphrase_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)    16493 2022-05-27 14:53:53.000000 slip39-9.1.2/slip39/api_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)     4923 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/defaults.py
+-rw-rw-r--   0 perry      (501) staff       (20)     5918 2022-04-20 00:55:26.000000 slip39-9.1.2/slip39/dependency_test.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2022-10-17 22:28:22.458936 slip39-9.1.2/slip39/generator/
+-rw-rw-r--   0 perry      (501) staff       (20)    10640 2022-05-27 14:53:53.000000 slip39-9.1.2/slip39/generator/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)       55 2022-01-26 20:35:06.000000 slip39-9.1.2/slip39/generator/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)    16830 2022-05-27 14:53:53.000000 slip39-9.1.2/slip39/generator/main.py
+-rw-rw-r--   0 perry      (501) staff       (20)     3861 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/generator_test.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2022-10-17 22:28:22.485695 slip39-9.1.2/slip39/gui/
+-rw-rw-r--   0 perry      (501) staff       (20)     3958 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-AS-BIP.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     2489 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-CRYPTO.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     1082 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-CS.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     2087 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-G-NAME.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     1602 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-G.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     3702 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-LO.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     4096 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-PASSPHRASE.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      985 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-PF.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     6036 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-SD.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      561 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-SE-SIGS.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     2356 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-SE.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      215 2022-10-17 13:47:37.000000 slip39-9.1.2/slip39/gui/SLIP-39-THRESHOLD.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     3015 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/SLIP-39-WALLET.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      834 2022-03-25 12:35:10.000000 slip39-9.1.2/slip39/gui/SLIP-39.txt
+-rw-rw-r--   0 perry      (501) staff       (20)        0 2022-02-04 14:13:36.000000 slip39-9.1.2/slip39/gui/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)       55 2022-02-04 14:13:36.000000 slip39-9.1.2/slip39/gui/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)    80076 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/gui/main.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2022-10-17 22:28:22.509525 slip39-9.1.2/slip39/layout/
+-rw-rw-r--   0 perry      (501) staff       (20)       68 2022-05-27 14:53:53.000000 slip39-9.1.2/slip39/layout/1x1-ffffff3f.png
+-rw-rw-r--   0 perry      (501) staff       (20)       68 2022-02-16 23:41:11.000000 slip39-9.1.2/slip39/layout/1x1-ffffff54.png
+-rw-rw-r--   0 perry      (501) staff       (20)       68 2022-05-27 14:53:53.000000 slip39-9.1.2/slip39/layout/1x1-ffffffbf.png
+-rw-rw-r--   0 perry      (501) staff       (20)    40663 2022-03-10 21:58:35.000000 slip39-9.1.2/slip39/layout/BNB.png
+-rw-r--r--   0 perry      (501) staff       (20)    27493 2022-02-17 14:41:02.000000 slip39-9.1.2/slip39/layout/BTC.png
+-rw-rw-r--   0 perry      (501) staff       (20)     1318 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/COVER-BIP-39.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     1169 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/COVER-SLIP-39.txt
+-rw-rw-r--   0 perry      (501) staff       (20)     1140 2022-05-27 14:53:53.000000 slip39-9.1.2/slip39/layout/COVER.txt
+-rw-rw-r--   0 perry      (501) staff       (20)    44316 2022-03-10 21:58:35.000000 slip39-9.1.2/slip39/layout/CRO.png
+-rw-r--r--   0 perry      (501) staff       (20)    22020 2022-02-17 14:41:12.000000 slip39-9.1.2/slip39/layout/DOGE.png
+-rw-rw-r--   0 perry      (501) staff       (20)    30750 2022-03-10 16:46:20.000000 slip39-9.1.2/slip39/layout/ETH.png
+-rw-r--r--   0 perry      (501) staff       (20)    21913 2022-02-17 14:41:05.000000 slip39-9.1.2/slip39/layout/LTC.png
+-rw-rw-r--   0 perry      (501) staff       (20)   111308 2022-05-27 14:53:53.000000 slip39-9.1.2/slip39/layout/SLIP-39.png
+-rw-rw-r--   0 perry      (501) staff       (20)    43289 2022-04-17 12:53:56.000000 slip39-9.1.2/slip39/layout/XRP.png
+-rw-rw-r--   0 perry      (501) staff       (20)      879 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)    20369 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/components.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2022-10-17 22:28:22.527539 slip39-9.1.2/slip39/layout/font/
+-rw-rw-r--   0 perry      (501) staff       (20)   331992 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/DejaVuSansMono-Bold.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   253580 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/DejaVuSansMono-BoldOblique.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   251932 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/DejaVuSansMono-Oblique.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   340712 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/DejaVuSansMono.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)    98260 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/Inconsolata-Bold.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)    97864 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/Inconsolata-Regular.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   383496 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/NotoSansMono-Bold.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   383844 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/NotoSansMono-Regular.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   179804 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/OverpassMono-Bold.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   179880 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/OverpassMono-Regular.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   119648 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/SourceCodePro-Bold.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   101188 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/SourceCodePro-BoldItalic.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   101260 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/SourceCodePro-Italic.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   119788 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/font/SourceCodePro-Regular.ttf
+-rw-rw-r--   0 perry      (501) staff       (20)   274581 2022-02-16 23:41:11.000000 slip39-9.1.2/slip39/layout/paper-wallet-background.png
+-rw-rw-r--   0 perry      (501) staff       (20)    32000 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/pdf.py
+-rw-rw-r--   0 perry      (501) staff       (20)     4350 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/layout/printer.py
+-rw-rw-r--   0 perry      (501) staff       (20)    10635 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/main.py
+-rw-rw-r--   0 perry      (501) staff       (20)     2590 2022-05-27 14:53:53.000000 slip39-9.1.2/slip39/output_test.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2022-10-17 22:28:22.530894 slip39-9.1.2/slip39/recovery/
+-rw-rw-r--   0 perry      (501) staff       (20)     6178 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/recovery/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)      822 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/recovery/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)    53541 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/recovery/entropy.py
+-rw-rw-r--   0 perry      (501) staff       (20)     7210 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/recovery/main.py
+-rw-rw-r--   0 perry      (501) staff       (20)    52443 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/recovery_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)    10692 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/util.py
+-rw-rw-r--   0 perry      (501) staff       (20)       88 2022-10-17 22:27:51.000000 slip39-9.1.2/slip39/version.py
+drwxrwxr-x   0 perry      (501) staff       (20)        0 2022-10-17 22:28:22.535508 slip39-9.1.2/slip39.egg-info/
+-rw-rw-r--   0 perry      (501) staff       (20)    10734 2022-10-17 22:28:22.000000 slip39-9.1.2/slip39.egg-info/PKG-INFO
+-rw-rw-r--   0 perry      (501) staff       (20)     2589 2022-10-17 22:28:22.000000 slip39-9.1.2/slip39.egg-info/SOURCES.txt
+-rw-rw-r--   0 perry      (501) staff       (20)        1 2022-10-17 22:28:22.000000 slip39-9.1.2/slip39.egg-info/dependency_links.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      168 2022-10-17 22:28:22.000000 slip39-9.1.2/slip39.egg-info/entry_points.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      361 2022-10-17 22:28:22.000000 slip39-9.1.2/slip39.egg-info/requires.txt
+-rw-rw-r--   0 perry      (501) staff       (20)        7 2022-10-17 22:28:22.000000 slip39-9.1.2/slip39.egg-info/top_level.txt
+-rw-rw-r--   0 perry      (501) staff       (20)        1 2022-10-17 22:28:21.000000 slip39-9.1.2/slip39.egg-info/zip-safe
```

### Comparing `slip39-9.0.4/COPYING` & `slip39-9.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/LICENSE` & `slip39-9.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/PKG-INFO` & `slip39-9.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slip39
-Version: 9.0.4
+Version: 9.1.2
 Summary: Standards-compliant SLIP-39 cryptocurrency seed generation and recovery, compatible with Trezor hardware wallets
 Home-page: https://github.com/pjkundert/python-slip39
 Author: Perry Kundert
 Author-email: perry@dominionrnd.com
 License: Dual License; GPLv3 and Proprietary
 Project-URL: Bug Tracker, https://github.com/pjkundert/python-slip39/issues
 Keywords: Ethereum Bitcoin Dogecoin Litecoin cryptocurrency SLIP-39 BIP-39 seed recovery PDF BIP-38 paper wallet
```

### Comparing `slip39-9.0.4/README.org` & `slip39-9.1.2/README.org`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #+author: Perry Kundert
 #+email: perry@kundert.ca
 #+date: 2021-12-20 10:55:00
 #+draft: false
 #+EXPORT_FILE_NAME: README.pdf
 #+STARTUP: org-startup-with-inline-images inlineimages
 #+STARTUP: org-latex-tables-centered nil
-
 #+OPTIONS: ^:nil # Disable sub/superscripting with bare _; _{...} still works
 #+OPTIONS: toc:nil
 
 #+LATEX_HEADER: \usepackage[margin=1.333in]{geometry}
 
 #+BEGIN_SRC emacs-lisp :noweb no-export :exports results
 ;; Tables not centered
@@ -186,21 +185,22 @@
     #+LATEX: {\scriptsize
     #+BEGIN_SRC bash :exports both :results output
     slip39 -c ETH -c BTC -c DOGE -c LTC --secret ffffffffffffffffffffffffffffffff \
         --no-card --wallet password --wallet-hint 'bad:pass...' 2>&1
     #+END_SRC
 
     #+RESULTS:
-    : 2022-06-10 06:25:39 slip39           It is recommended to not use '-s|--secret <hex>'; specify '-' to read from input
-    : 2022-06-10 06:25:39 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
-    : 2022-06-10 06:25:39 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
-    : 2022-06-10 06:25:39 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
-    : 2022-06-10 06:25:39 slip39.layout    DOGE   m/44'/3'/0'/0/0     : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
-    : 2022-06-10 06:25:39 slip39.layout    LTC    m/84'/2'/0'/0/0     : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
-    : 2022-06-10 06:25:43 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-06-10+06.25.40-ETH-0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1.pdf
+    : 2022-10-05 15:32:42 slip39           It is recommended to not use '-s|--secret <hex>'; specify '-' to read from input
+    : 2022-10-05 15:32:42 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
+    : 2022-10-05 15:32:42 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
+    : 2022-10-05 15:32:42 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
+    : 2022-10-05 15:32:42 slip39.layout    DOGE   m/44'/3'/0'/0/0     : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
+    : 2022-10-05 15:32:42 slip39.layout    LTC    m/84'/2'/0'/0/0     : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
+    : 2022-10-05 15:32:47 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-10-05+15.32.44-ETH-0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1.pdf
+
     #+LATEX: }
 
     And what they look like:
     
     #+CAPTION: Paper Wallets (from =--secret ffff...=)
     #+ATTR_LATEX: :width 5in :options angle=0
     [[./images/slip39-wallets.png]]
@@ -213,17 +213,18 @@
     slip39-recovery -v \
 	--mnemonic "material leaf acrobat romp charity capital omit skunk change firm eclipse crush fancy best tracks flip grownup plastic chew peanut" \
         --mnemonic "material leaf beard romp disaster duke flame uncover group slice guest blue gums duckling total suitable trust guitar payment platform" \
 	2>&1
     #+END_SRC
 
     #+RESULTS:
-    : 2022-06-10 06:26:00 slip39.recovery  Recovered 128-bit SLIP-39 Seed Entropy with 2 (all) of 2 supplied mnemonics; Seed decoded from SLIP-39 Mnemonics w/ passphrase
-    : 2022-06-10 06:26:00 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
+    : 2022-10-05 15:33:13 slip39.recovery  Recovered 128-bit SLIP-39 Seed Entropy with 2 (all) of 2 supplied mnemonics; Seed decoded from SLIP-39 Mnemonics w/ passphrase
+    : 2022-10-05 15:33:13 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
     : ffffffffffffffffffffffffffffffff
+
     #+LATEX: }
 
     You can run this as a command-line pipeline.  Here, we use some SLIP-39 Mnemonics that encode the =ffff...= Seed Entropy;
     note that the wallets match those output above:
     
     #+LATEX: {\scriptsize
     #+BEGIN_SRC bash :exports both :results output
@@ -232,20 +233,21 @@
         --mnemonic "material leaf beard romp disaster duke flame uncover group slice guest blue gums duckling total suitable trust guitar payment platform" \
     | slip39 -c ETH -c BTC -c DOGE -c LTC --secret - \
         --no-card --wallet password --wallet-hint 'bad:pass...' \
 	2>&1
     #+END_SRC
 
     #+RESULTS:
-    : 2022-06-10 06:26:04 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
-    : 2022-06-10 06:26:04 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
-    : 2022-06-10 06:26:04 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
-    : 2022-06-10 06:26:04 slip39.layout    DOGE   m/44'/3'/0'/0/0     : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
-    : 2022-06-10 06:26:04 slip39.layout    LTC    m/84'/2'/0'/0/0     : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
-    : 2022-06-10 06:26:08 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-06-10+06.26.05-ETH-0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1.pdf
+    : 2022-10-05 15:33:38 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
+    : 2022-10-05 15:33:38 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
+    : 2022-10-05 15:33:38 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
+    : 2022-10-05 15:33:38 slip39.layout    DOGE   m/44'/3'/0'/0/0     : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
+    : 2022-10-05 15:33:38 slip39.layout    LTC    m/84'/2'/0'/0/0     : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
+    : 2022-10-05 15:33:42 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-10-05+15.33.39-ETH-0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1.pdf
+
     #+LATEX: }
 
 *** Supported Cryptocurrencies
 
     While the SLIP-39 Seed is not cryptocurrency-specific (any wallet for any cryptocurrency can be
     derived from it), each type of cryptocurrency has its own standard derivation path
     (eg. =m/44'/3'/0'/0/0= for DOGE), and its own address representation (eg. Bech32 at
@@ -332,15 +334,15 @@
     : 
     : Create and output SLIP-39 encoded Seeds and Paper Wallets to a PDF file.
     : 
     : positional arguments:
     :   names                 Account names to produce; if --secret Entropy is
     :                         supplied, only one is allowed.
     : 
-    : optional arguments:
+    : options:
     :   -h, --help            show this help message and exit
     :   -v, --verbose         Display logging information.
     :   -q, --quiet           Reduce logging output.
     :   -o OUTPUT, --output OUTPUT
     :                         Output PDF to file or '-' (stdout); formatting w/
     :                         name, date, time, crypto, path, address allowed
     :   -t THRESHOLD, --threshold THRESHOLD
@@ -391,14 +393,15 @@
     :                         business)
     :   --no-card             Disable PDF SLIP-39 mnemonic card output
     :   --paper PAPER         Paper size (default: Letter)
     :   --cover               Produce PDF SLIP-39 cover page
     :   --no-cover            Disable PDF SLIP-39 cover page
     :   --text                Enable textual SLIP-39 mnemonic output to stdout
     #+end_example
+
     #+LATEX: }
 
 ** Recovery & Re-Creation
 
   Later, if you need to recover the wallet seed, keep entering SLIP-39 mnemonics into
   =slip39-recovery= until the secret is recovered (invalid/duplicate mnemonics will be ignored):
 
@@ -420,19 +423,20 @@
 
   #+LATEX: {\scriptsize
   #+BEGIN_SRC bash :exports both :results output
   slip39 --secret 383597fd63547e7c9525575decd413f7 --wallet password --wallet-hint bad:pass... 2>&1
   #+END_SRC
 
   #+RESULTS:
-  : 2022-06-10 06:26:22 slip39           It is recommended to not use '-s|--secret <hex>'; specify '-' to read from input
-  : 2022-06-10 06:26:22 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
-  : 2022-06-10 06:26:23 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xb44A2011A99596671d5952CdC22816089f142FB3
-  : 2022-06-10 06:26:23 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qcupw7k8enymvvsa7w35j5hq4ergtvus3zk8a8s
-  : 2022-06-10 06:26:25 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-06-10+06.26.23-ETH-0xb44A2011A99596671d5952CdC22816089f142FB3.pdf
+  : 2022-10-05 16:36:32 slip39           It is recommended to not use '-s|--secret <hex>'; specify '-' to read from input
+  : 2022-10-05 16:36:32 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
+  : 2022-10-05 16:36:32 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xb44A2011A99596671d5952CdC22816089f142FB3
+  : 2022-10-05 16:36:32 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qcupw7k8enymvvsa7w35j5hq4ergtvus3zk8a8s
+  : 2022-10-05 16:36:35 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-10-05+16.36.33-ETH-0xb44A2011A99596671d5952CdC22816089f142FB3.pdf
+
   #+LATEX: }
 
 *** =slip39.recovery= Synopsis
 
     #+LATEX: {\scriptsize
     #+BEGIN_SRC bash :exports both :results output
     slip39-recovery --help 2>&1                | sed 's/^/: /' # (just for output formatting)
@@ -441,15 +445,15 @@
     #+RESULTS:
     #+begin_example
     : usage: slip39-recovery [-h] [-v] [-q] [-m MNEMONIC] [-e] [-b] [-u]
     :                        [-p PASSPHRASE]
     : 
     : Recover and output secret Seed from SLIP-39 or BIP-39 Mnemonics
     : 
-    : optional arguments:
+    : options:
     :   -h, --help            show this help message and exit
     :   -v, --verbose         Display logging information.
     :   -q, --quiet           Reduce logging output.
     :   -m MNEMONIC, --mnemonic MNEMONIC
     :                         Supply another SLIP-39 (or a BIP-39) mnemonic phrase
     :   -e, --entropy         Return the BIP-39 Mnemonic Seed Entropy instead of the
     :                         generated Seed (default: False)
@@ -482,14 +486,15 @@
     : stored in SLIP-39 -- not the *input* 128-, 160-, 192-, 224-, or 256-bit entropy used to create the
     : original BIP-39 mnemonic phrase.
     : 
     : 2) The original BIP-39 12- or 24-word, 128- to 256-bit Seed Entropy can be recovered by supplying
     : --entropy.  This modifies the BIP-39 recovery to return the original BIP-39 Mnemonic Entropy, before
     : decryption and seed generation.  It has no effect for SLIP-39 recovery.
     #+end_example
+
     #+LATEX: }
 
 *** Pipelining =slip39.recovery | slip39 --secret -=
 
    The tools can be used in a pipeline to avoid printing the secret.  Here we generate some
    mnemonics, sorting them in reverse order so we need more than just the first couple to recover.
    Observe the Ethereum wallet address generated.
@@ -501,20 +506,22 @@
    #+BEGIN_SRC bash :exports both :results output
    ( python3 -m slip39 --text --no-card \
        | ( sort -r  ; echo "...later..." 1>&2 ) \
        | python3 -m slip39.recovery \
        | python3 -m slip39 --secret - --no-card \
     ) 2>&1
    #+END_SRC
+
    #+RESULTS:
-   : 2022-06-10 06:26:37 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xD1701483AC2bDe364C01D8C2A04D1F59fb80aAA0
-   : 2022-06-10 06:26:37 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qktmcplw5yazvpzsrmxdfrppvkdw4w0r8qmxfqe
+   : 2022-10-05 16:36:16 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x252B6C41bCE5f580054fb54b6de539433C58B86D
+   : 2022-10-05 16:36:16 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qpksxy2n5ct67du5wjytgntuw9dl99uwews2wg5
    : ...later...
-   : 2022-06-10 06:26:37 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xD1701483AC2bDe364C01D8C2A04D1F59fb80aAA0
-   : 2022-06-10 06:26:37 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qktmcplw5yazvpzsrmxdfrppvkdw4w0r8qmxfqe
+   : 2022-10-05 16:36:16 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x252B6C41bCE5f580054fb54b6de539433C58B86D
+   : 2022-10-05 16:36:16 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qpksxy2n5ct67du5wjytgntuw9dl99uwews2wg5
+
    #+LATEX: }
 
 ** Generation of Addresses
 
    For systems that require a stream of groups of wallet Addresses (eg. for preparing invoices for
    clients, with a choice of cryptocurrency payment options), =slip-generator= can produce a stream
    of groups of addresses.
@@ -532,15 +539,15 @@
     :                         [-c CRYPTOCURRENCY] [--path PATH] [-d DEVICE]
     :                         [--baudrate BAUDRATE] [-e ENCRYPT] [--decrypt ENCRYPT]
     :                         [--enumerated] [--no-enumerate] [--receive]
     :                         [--corrupt CORRUPT]
     : 
     : Generate public wallet address(es) from a secret seed
     : 
-    : optional arguments:
+    : options:
     :   -h, --help            show this help message and exit
     :   -v, --verbose         Display logging information.
     :   -q, --quiet           Reduce logging output.
     :   -s SECRET, --secret SECRET
     :                         Use the supplied 128-, 256- or 512-bit hex value as
     :                         the secret seed; '-' (default) reads it from stdin
     :                         (eg. output from slip39.recover)
@@ -583,14 +590,15 @@
     : 
     : Since the receiver requires the nonce to decrypt, and we do not want to separately transmit the
     : nonce and supply it to the receiver, the first record emitted when --encrypt is specified is the
     : random nonce, encrypted with the password, itself with a known nonce of all 0 bytes.  The plaintext
     : data is random, while the nonce is not, but since this construction is only used once, it should be
     : satisfactory.  This first nonce record is transmitted with an enumeration prefix of "nonce".
     #+end_example
+
     #+LATEX: }
 
 *** Producing Addresses
 
     Addresses can be produced in plaintext or encrypted, and output to stdout or to a serial port.
 
     #+LATEX: {\scriptsize
@@ -599,14 +607,15 @@
     #+END_SRC
 
     #+RESULTS:
     :     0: [["ETH", "m/44'/60'/0'/0/0", "0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1"], ["BTC", "m/84'/0'/0'/0/0", "bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl"]]
     :     1: [["ETH", "m/44'/60'/0'/0/1", "0x8D342083549C635C0494d3c77567860ee7456963"], ["BTC", "m/84'/0'/0'/0/1", "bc1qnec684yvuhfrmy3q856gydllsc54p2tx9w955c"]]
     :     2: [["ETH", "m/44'/60'/0'/0/2", "0x52787E24965E1aBd691df77827A3CfA90f0166AA"], ["BTC", "m/84'/0'/0'/0/2", "bc1q2snj0zcg23dvjpw7m9lxtu0ap0hfl5tlddq07j"]]
     :     3: [["ETH", "m/44'/60'/0'/0/3", "0xc2442382Ae70c77d6B6840EC6637dB2422E1D44e"], ["BTC", "m/84'/0'/0'/0/3", "bc1qxwekjd46aa5n0s3dtsynvtsjwsne7c5f5w5dsd"]]
+
     #+LATEX: }
 
     To produce accounts from a BIP-39 or SLIP-39 seed, recover it using slip39-recovery.
 
     Here's an example of recovering a test BIP-39 seed; note that it yields the well-known ETH
     =0xfc20...1B5E= and BTC =bc1qk0...gnn2= accounts associated with this test Mnemonic:
 
@@ -617,33 +626,35 @@
     #+END_SRC
 
     #+RESULTS:
     :     0: [["ETH", "m/44'/60'/0'/0/0", "0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E"], ["BTC", "m/84'/0'/0'/0/0", "bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2"]]
     :     1: [["ETH", "m/44'/60'/0'/0/1", "0xd1a7451beB6FE0326b4B78e3909310880B781d66"], ["BTC", "m/84'/0'/0'/0/1", "bc1qkd33yck74lg0kaq4tdcmu3hk4yruhjayxpe9ug"]]
     :     2: [["ETH", "m/44'/60'/0'/0/2", "0x578270B5E5B53336baC354756b763b309eCA90Ef"], ["BTC", "m/84'/0'/0'/0/2", "bc1qvr7e5aytd0hpmtaz2d443k364hprvqpm3lxr8w"]]
     :     3: [["ETH", "m/44'/60'/0'/0/3", "0x909f59835A5a120EafE1c60742485b7ff0e305da"], ["BTC", "m/84'/0'/0'/0/3", "bc1q6t9vhestkcfgw4nutnm8y2z49n30uhc0kyjl0d"]]
+
     #+LATEX: }
 
     We can encrypt the output, to secure the sequence (and due to integrated MACs, ensures no errors
     occur over an insecure channel like a serial cable):
 
     #+LATEX: {\scriptsize
     #+BEGIN_SRC bash :exports both :results output
     ( slip39-recovery --bip39 --mnemonic 'zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong' \
         | slip39-generator --secret - --path '../-3' --encrypt 'password' ) 2>&1
     #+END_SRC
 
     #+RESULTS:
     : 
     : 
-    : nonce: 6fcc59c2edec925c2bce6d7cd24b78f475dee0e13b5aadebd8f6b5ad
-    :     0: 722d48835b80062aaa41db839cc010c41a9b3b27044b4d7640c02ad14cc49c2451d0f696610a5e913c939776fb10f0a40a7de2ba62b5ada9de955cee8c5b40344d729779719aa2f9d25756eb91e24bf6a7d2418f8d3feaff854c1f0fa603c8dc974b33fbf68b2eb416583be0bb85b24e7cbc4a07d3bde11377febf503b4a708bd79faa8f8ebbc533ee16beee920dd78c0ecd8433cdb9f906b8b658561e2fccc4bdcd666e5e
-    :     1: 617f1ad0862f25c16f826b9bc23830142d03f6afca8efffa93848490646fab5e3afff8d43773a8354726e0e7cb7e3f4d835dab2b71718d2cda5fda76e311e390d46ddd56f02472c19cfd7fe298377fdae0b39454604ee4450933b5022485d85d6ab69e2828bc6d3365e6781681bc80d67cf2fdecd49f2f69a405dd9c80e586bd2262d4041c2cbca1b584ef1c1ec6c8d6eb16fbaabcedc18bd2101b3e5025e68e9988315654
-    :     2: c3644f4d71b9050aadba90bdd13e0ca4c7cf353c565b783155c87417ef08bf4a9420e0648e8bc03e329c85bca62632e206df5d2a2916b140e915c2119b3b477bdc941e2898f32fe9255d68e06f5cc6e9f52a6e0c0be25344ad21cc30f32aa0cfcb085b83c4d587df39f42b58b8e3f8ae1d1af033668ee263ca3214f8c899532db72413a4db2eb11f5dfa41689296880cd5222fda23ff418e1df800e669a3296a56bf44b187
-    :     3: 8730fc53e9aef587f10f3e13554536a58dea7c2459c57485fd2ac95a6309acac8f3f603f5fdc94fd1df93d98715924a9ebb48e73ba068113ff69cb19117b25fe5ff68487d96eabe02c584b2406e781d8105744497a819ee9eaa66ca3881248166a4e5c2c6972b23ff6df2314474a04d38f3e8c787a4b20aeeab9fd029f479f553fdd878c6a14f0d3f3be02d4851e8af89bda113f9fb189db06f634e45eff2b34997308b647
+    : nonce: 530f5d2784b872e16c1f25912891866ab380b4eb767f15312f0a60ae
+    :     0: 3a33abe5b4ed567e238b059576059067795fa7b4760ac80d29a42796c213296dcbde47c75826f2adc0c8821da6e438d9ef7271f5285239e6c5208f409001dfe4888169282a3f4a13953e7a9dab74e724e2447ed7413e92836b5f0ff100eaa5bb80dd933ce76dae58324957c427b6228fdbe46c06fdc114394954a1843e7358d651f30ffcf5aa3bf66db776d3ae7eb265bcb5a8fc3aeb4fed73da27c4d94a7ad6fe893de526
+    :     1: 8fe5a59696c32d3e096930a905fc7474c1987a9d5582ddbd1b82ebe62118a36d81a8e210f50b0345c3fc2c83b84628208ea45e46397133476c04d1ffca48b246c2547f2ea912fd12cc9b334215b745675d2fd65bd90d9e7805195d7a66f493305d2c3ca364c9dfdd73097f1898cd193720a9410f66efed79ea9fb5537cc9aafda3ae211fc5e9f30a1de24df012ad846ab3b17a6e0dd4d07d4c6fecf2593cf7290f35a5875d
+    :     2: 534fa3352e576be04f749f57a56101d7fc723cdc1cf9a205ea3127a088625957b1dee1495f9622223a7c13e1535f1e1f20da4cdd79d3704fe27d796aec4b07f1a0a8088bd4422271d7d3b851eaa410d6bae5d25fe22d20fb29477a2e83a6eb15145efa019a4f74e729932f469428e3c7864faa797448374aa8a916547f9b3021e9074ef8611470999dba241f66969632a0d8a57641f3fa7e675ab57c3b05892069c8aa1ad0
+    :     3: d0488b4808f1028f57792c2dd147eb347bada39175f7be38d9fa0ef770ffedd2cea664f91a8fd94b761e0d726e33d9983aaab2c25906b0c0092f0e71505a9cae086841d8c5b95de65f9dd890f5d6eac2c59c913159ce9c26f76d5a17390958589a38d756679de00d3f547c9b4c4234845273fafa5af8560456e1871304895d9991d0a54ffc9e9fd190ef2a688530d380ee725daebaa948e4072237dfdde965f098ba8eac5f
+
     #+LATEX: }
 
     On the receiving computer, we can decrypt and recover the stream of accounts from the wallet
     seed; any rows with errors are ignored:
     #+LATEX: {\scriptsize
     #+BEGIN_SRC bash :exports both :results output
     ( slip39-recovery --bip39 --mnemonic 'zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong' \
@@ -652,14 +663,15 @@
     #+END_SRC
 
     #+RESULTS:
     :     0: [["ETH", "m/44'/60'/0'/0/0", "0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E"], ["BTC", "m/84'/0'/0'/0/0", "bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2"]]
     :     1: [["ETH", "m/44'/60'/0'/0/1", "0xd1a7451beB6FE0326b4B78e3909310880B781d66"], ["BTC", "m/84'/0'/0'/0/1", "bc1qkd33yck74lg0kaq4tdcmu3hk4yruhjayxpe9ug"]]
     :     2: [["ETH", "m/44'/60'/0'/0/2", "0x578270B5E5B53336baC354756b763b309eCA90Ef"], ["BTC", "m/84'/0'/0'/0/2", "bc1qvr7e5aytd0hpmtaz2d443k364hprvqpm3lxr8w"]]
     :     3: [["ETH", "m/44'/60'/0'/0/3", "0x909f59835A5a120EafE1c60742485b7ff0e305da"], ["BTC", "m/84'/0'/0'/0/3", "bc1q6t9vhestkcfgw4nutnm8y2z49n30uhc0kyjl0d"]]
+
     #+LATEX: }
 
 ** The =slip39= module API
    
    Provide SLIP-39 Mnemonic set creation from a 128-bit master secret, and recovery of the secret
    from a subset of the provided Mnemonic set.
    
@@ -692,17 +704,18 @@
     | accounts        | Resultant list of groups of accounts               |
     | using_bip39     | Seed produced from entropy using BIP-39 generation |
     #+LATEX: }
 
     This is immediately usable to pass to =slip39.output=.
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     import codecs
     import random
+    from tabulate import tabulate
 
     #
     # NOTE:
     #
     # We turn off randomness here during SLIP-39 generation to get deterministic phrases;
     # during normal operation, secure entropy is used during mnemonic generation, yielding
     # random phrases, even when the same seed is used multiple times.
@@ -714,30 +727,28 @@
 
     cryptopaths         = [("ETH","m/44'/60'/0'/0/-2"), ("BTC","m/44'/0'/0'/0/-2")]
     master_secret       = b'\xFF' * 16
     passphrase          = b""
     create_details      = slip39.create(
         "Test", 2, { "Mine": (1,1), "Fam": (2,3) },
         master_secret=master_secret, passphrase=passphrase, cryptopaths=cryptopaths )
-    [
+
+    print( tabulate( [
         [
             f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" if l_n == 0 else ""
         ] + words
         for g_name,(g_of,g_mnems) in create_details.groups.items()
         for g_n,mnem in enumerate( g_mnems )
         for l_n,(line,words) in enumerate(slip39.organize_mnemonic(
                 mnem, label=f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" ))
-    ]
+      ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[1]:
-    | 0             | 1          | 2           | 3           |
-    |---------------+------------+-------------+-------------|
     | Mine(1/1) #1: | 1 academic | 8 safari    | 15 standard |
     |               | 2 acid     | 9 drug      | 16 angry    |
     |               | 3 acrobat  | 10 browser  | 17 similar  |
     |               | 4 easy     | 11 trash    | 18 aspect   |
     |               | 5 change   | 12 fridge   | 19 smug     |
     |               | 6 injury   | 13 busy     | 20 violence |
     |               | 7 painting | 14 finger   |             |
@@ -764,27 +775,24 @@
     |               | 7 discuss  | 14 sunlight |             |
     :end:
     #+LATEX: }
 
     Add the resultant HD Wallet addresses:
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
-    [
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
+    print( tabulate( [
         [ account.path, account.address ]
         for group in create_details.accounts
         for account in group
-    ]
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[2]:
-    | 0                | 1                                          |
-    |------------------+--------------------------------------------|
     | m/44'/60'/0'/0/0 | 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1 |
     | m/44'/0'/0'/0/0  | bc1qm5ua96hx30snwrwsfnv97q96h53l86ded7wmjl |
     | m/44'/60'/0'/0/1 | 0x8D342083549C635C0494d3c77567860ee7456963 |
     | m/44'/0'/0'/0/1  | bc1qwz6v9z49z8mk5ughj7r78hjsp45jsxgzh29lnh |
     | m/44'/60'/0'/0/2 | 0x52787E24965E1aBd691df77827A3CfA90f0166AA |
     | m/44'/0'/0'/0/2  | bc1q690m430qu29auyefarwfrvfumncunvyw6v53n9 |
     :end:
@@ -807,34 +815,31 @@
     #+LATEX: }
 
     Layout and produce a PDF containing all the SLIP-39 details on cards for the crypto accounts, on
     the paper_format provided.  Returns the paper (orientation,format) used, the FPDF, and passes
     through the supplied cryptocurrency accounts derived.
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     (paper_format,orientation),pdf,accounts = slip39.produce_pdf( *create_details )
     pdf_binary = pdf.output()
-    [
+    print( tabulate( [
         [ "Orientation:",	orientation ],
         [ "Paper:",		paper_format ],
         [ "PDF Pages:",		pdf.pages_count ],
         [ "PDF Size:",		len( pdf_binary )],
-    ]
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[4]:
-    | 0            | 1         |
-    |--------------+-----------|
     | Orientation: | landscape |
-    | Paper:       | Letter    |
-    | PDF Pages:   | 1         |
-    | PDF Size:    | 13028     |
+    | Paper:       |    Letter |
+    | PDF Pages:   |         1 |
+    | PDF Size:    |     13137 |
     :end:
 
     #+LATEX: }
 
 *** =slip39.write_pdfs=
 
     #+LATEX: {\scriptsize
@@ -892,40 +897,37 @@
     |-------------+----------------------------------------------------|
     | mnemonics   | ["<mnemonics>", ...]                               |
     | passphrase  | Optional passphrase to decrypt secret Seed Entropy |
     | using_bip39 | Use BIP-39 Seed generation from recover Entropy    |
     #+LATEX: }
     
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     # Recover with the wrong password (on purpose, as a decoy wallet w/ a small amount)
     recoverydecoy       = slip39.recover(
         create_details.groups['Mine'][1][:] + create_details.groups['Fam'][1][:2],
         passphrase=b"wrong!"
     )
     recoverydecoy_hex   = codecs.encode( recoverydecoy, 'hex_codec' ).decode( 'ascii' )
 
     # But, recovering w/ correct passphrase yields our original Seed Entropy
     recoveryvalid       = slip39.recover(
         create_details.groups['Mine'][1][:] + create_details.groups['Fam'][1][:2],
         passphrase=passphrase
     )
     recoveryvalid_hex   = codecs.encode( recoveryvalid, 'hex_codec' ).decode( 'ascii' )
 
-    [
+    print( tabulate( [
       [ f"{len(recoverydecoy)*8}-bit secret (decoy):", f"{recoverydecoy_hex}" ],
       [ f"{len(recoveryvalid)*8}-bit secret recovered:", f"{recoveryvalid_hex}" ]
-    ]
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[5]:
-    | 0                         | 1                                |
-    |---------------------------+----------------------------------|
     | 128-bit secret (decoy):   | 2e522cea2b566840495c220cf79c756e |
     | 128-bit secret recovered: | ffffffffffffffffffffffffffffffff |
     :end:
     #+LATEX: }
 
 *** =slip39.recover_bip39=
 
@@ -947,15 +949,15 @@
     #+LATEX: {\scriptsize
     | Key      | Description                                                 |
     |----------+-------------------------------------------------------------|
     | entropy  | The =bytes= of Seed Entropy                                 |
     | strength | Or, the number of bits of Entropy to produce (Default: 128) |
     | language | Default is "english"                                        |
     #+LATEX: }
-    
+
 * Conversion from BIP-39 to SLIP-39
 
   If we already have a BIP-39 wallet, it would certainly be nice to be able to create nice, safe
   SLIP-39 mnemonics for it, and discard the unsafe BIP-39 mnemonics we have lying around, just
   waiting to be accidentally discovered and the account compromised!
 
   Fortunately, *we can* do this!  It takes a bit of practice to become comfortable with the process,
@@ -983,108 +985,99 @@
     BIP-39 uses a single set of 12, 15, 18, 21 or 24 BIP-39 words to carefully preserve a specific
     128 to 256 bits of initial Seed Entropy.  Here's a 128-bit (12-word) example using some fixed
     "entropy" =0xFFFF..FFFF=.  You'll note that, from the BIP-39 Mnemonic, we can either recover the
     original 128-bit Seed Entropy, *or* we can generate the resultant 512-bit Seed w/ the correct
     passphrase:
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     from mnemonic import Mnemonic
     bip39_english       = Mnemonic("english")
     entropy             = b'\xFF' * 16
     entropy_hex		= codecs.encode( entropy, 'hex_codec' ).decode( 'ascii' )
     entropy_mnemonic    = bip39_english.to_mnemonic( entropy )
 
     recovered		= slip39.recover_bip39( entropy_mnemonic, as_entropy=True )
     recovered_hex	= codecs.encode( recovered, 'hex_codec' ).decode( 'ascii' )
 
     recovered_seed	= slip39.recover_bip39( entropy_mnemonic, passphrase=passphrase )
     recovered_seed_hex	= codecs.encode( recovered_seed, 'hex_codec' ).decode( 'ascii' )
     
-    [
-     [ "Original Entropy", entropy_hex ],
-     [ "BIP-39 Mnemonic", entropy_mnemonic ],
-     [ "Recovered Entropy", recovered_hex ],
-     [ "Recovered Seed", f"{recovered_seed_hex:.50}..." ],
-    ]
+    print( tabulate( [
+        [ "Original Entropy", entropy_hex ],
+        [ "BIP-39 Mnemonic", entropy_mnemonic ],
+        [ "Recovered Entropy", recovered_hex ],
+        [ "Recovered Seed", f"{recovered_seed_hex:.50}..." ],
+    ], tablefmt='orgtbl'))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[6]:
-    | 0                 | 1                                                     |
-    |-------------------+-------------------------------------------------------|
     | Original Entropy  | ffffffffffffffffffffffffffffffff                      |
     | BIP-39 Mnemonic   | zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong     |
     | Recovered Entropy | ffffffffffffffffffffffffffffffff                      |
     | Recovered Seed    | b6a6d8921942dd9806607ebc2750416b289adea669198769f2... |
     :end:
     #+LATEX: }
 
-    Each word is one of a corpus of 2048 words; therefore, each word encodes 11 bits (2048 == 2**11)
-    of entropy.  So, we provided 128 bits, but 12*11 == 132.  So where does the extra 4 bits of data
+    Each word is one of a corpus of 2048 words; therefore, each word encodes 11 bits (2048 = 2**11)
+    of entropy.  So, we provided 128 bits, but 12*11 = 132.  So where does the extra 4 bits of data
     come from?
 
     It comes from the first few bits of a SHA256 hash of the entropy, which is added to the end of
-    the supplied 128 bits, to reach the required 132 bits: 132 / 11 == 12 words.
+    the supplied 128 bits, to reach the required 132 bits: 132 / 11 = 12 words.
 
     This last 4 bits (up to 8 bits, for a 256-bit 24-word BIP-39) is checked, when validating the
     BIP-39 mnemonic.  Therefore, making up a random BIP-39 mnemonic will succeed only 1 / 16 times on
-    average, due to an incorrect checksum 4-bit (16 == 2**4) .  Lets check:
+    average, due to an incorrect checksum 4-bit (16 = 2**4) .  Lets check:
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     def random_words( n, count=100 ):
         for _ in range( count ):
             yield ' '.join( random.choice( bip39_english.wordlist ) for _ in range( n ))
 
     successes           = sum(
         bip39_english.check( m )
         for i,m in enumerate( random_words( 12, 10000 ))) / 100
 
-    [
+    print( tabulate( [
       [ "Valid random 12-word mnemonics:", f"{successes}%" ],
       [ "Or, about: ", f"1 / {100/successes:.3}" ],
-    ]
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[7]:
-    | 0                               | 1        |
-    |---------------------------------+----------|
-    | Valid random 12-word mnemonics: | 6.34%    |
-    | Or, about:                      | 1 / 15.8 |
+    | Valid random 12-word mnemonics: |    6.26% |
+    | Or, about:                      | 1 / 16.0 |
     :end:
     #+LATEX: }
 
     Sure enough, about 1/16 random 12-word phrases are valid BIP-39 mnemonics.  OK, we've got the
     contents of the BIP-39 phrase dialed in.  How is it used to generate accounts?
 
 *** BIP-39 Mnemonic to Seed
 
     Unfortunately, BIP-39 does *not* use the carefully preserved 128-bit entropy to generate the wallet!
     Nope, it is stretched to a 512-bit seed using PBKDF2 HMAC SHA512.  The normalized *text* (/not
     the Entropy bytes/) of the 12-word mnemonic is then used (with a salt of "mnemonic" plus an
     optional passphrase, "" by default), to obtain the 512-bit seed:
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     seed                = bip39_english.to_seed( entropy_mnemonic )
     seed_hex            = codecs.encode( seed, 'hex_codec' ).decode( 'ascii' )
-    [
+    print( tabulate( [
      [ f"{len(seed)*8}-bit seed:", f"{seed_hex:.50}..." ]
-    ]
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[8]:
-    | 0             | 1                                                     |
-    |---------------+-------------------------------------------------------|
     | 512-bit seed: | b6a6d8921942dd9806607ebc2750416b289adea669198769f2... |
     :end:
     #+LATEX: }
 
 *** BIP-39 Seed to Address
 
     Finally, this 512-bit seed is used to derive HD wallet(s).  The HD Wallet key derivation process
@@ -1092,29 +1085,26 @@
     with a prefix of b"Bitcoin seed" to stretch the supplied seed entropy to 64 bytes (512 bits).
     Then, the HD Wallet *path* segments are iterated through, permuting the first 32 bytes of this
     material as the key with the second 32 bytes of material as the chain node, until finally the
     32-byte (256-bit) Ethereum account private key is produced.  We then use this private key to
     compute the rest of the Ethereum account details, such as its public address.
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     path                = "m/44'/60'/0'/0/0"
     bip39_eth_hd        = slip39.account( seed, 'ETH', path )
-    [
+    print( tabulate( [
      [ f"{len(bip39_eth_hd.key)*4}-bit derived key path:", f"{path}" ],
      [ "Produces private key: ", f"{bip39_eth_hd.key}" ],
      [ "Yields Ethereum address:", f"{bip39_eth_hd.address}" ],
-    ]
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[9]:
-    | 0                         | 1                                                                |
-    |---------------------------+------------------------------------------------------------------|
     | 256-bit derived key path: | m/44'/60'/0'/0/0                                                 |
     | Produces private key:     | 7af65ba4dd53f23495dcb04995e96f47c243217fc279f10795871b725cd009ae |
     | Yields Ethereum address:  | 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E                       |
     :end:
     #+LATEX: }
 
     Thus, we see that while the 12-word BIP-39 mnemonic careful preserves the original 128-bit
@@ -1125,31 +1115,28 @@
 *** SLIP-39 Entropy to Mnemonic
 
     Just like BIP-39 carefully preserves the original 128-bit Seed Entropy bytes in a single 12-word
     mnemonic phrase, SLIP-39 preserves the original 128- or 256-bit Seed Entropy in a /set/ of 20-
     or 33-word Mnemonic phrases.
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     name,thrs,grps,acct,ub39 = slip39.create(
         "Test", 2, { "Mine": (1,1), "Fam": (2,3) }, entropy )
-    [
-     [ f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" if l_n == 0 else "" ] + words
-     for g_name,(g_of,g_mnems) in grps.items()
-     for g_n,mnem in enumerate( g_mnems )
-     for l_n,(line,words) in enumerate(slip39.organize_mnemonic(
-             mnem, rows=7, cols=3, label=f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" ))
-    ]
+    print( tabulate( [
+        [ f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" if l_n == 0 else "" ] + words
+        for g_name,(g_of,g_mnems) in grps.items()
+        for g_n,mnem in enumerate( g_mnems )
+        for l_n,(line,words) in enumerate(slip39.organize_mnemonic(
+                mnem, rows=7, cols=3, label=f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" ))
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[10]:
-    | 0             | 1          | 2           | 3           |
-    |---------------+------------+-------------+-------------|
     | Mine(1/1) #1: | 1 academic | 8 safari    | 15 standard |
     |               | 2 acid     | 9 drug      | 16 angry    |
     |               | 3 acrobat  | 10 browser  | 17 similar  |
     |               | 4 easy     | 11 trash    | 18 aspect   |
     |               | 5 change   | 12 fridge   | 19 smug     |
     |               | 6 injury   | 13 busy     | 20 violence |
     |               | 7 painting | 14 finger   |             |
@@ -1179,30 +1166,26 @@
 
     Since there is some randomness used in the SLIP-39 mnemonics generation process, we would get a
     *different* set of words each time for the fixed "entropy" =0xFFFF..FF= used in this example (if
     we hadn't manually disabled entropy for =shamir_mnemonic=, above), but we will *always* derive
     the same Ethereum account =0x824b..19a1= at the specified HD Wallet derivation path.
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
-    [
-     [ "Crypto", "HD Wallet Path:", "Ethereum Address:" ]
-    ] + [
-     [ account.crypto, account.path, account.address ]
-     for group in create_details.accounts
-     for account in group
-    ]
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
+    print( tabulate( [
+        [ account.crypto, account.path, account.address ]
+        for group in create_details.accounts
+        for account in group
+    ], tablefmt='orgtbl', headers=[ "Crypto", "HD Wallet Path:", "Ethereum Address:" ] ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[11]:
-    | 0      | 1                | 2                                          |
-    |--------+------------------+--------------------------------------------|
     | Crypto | HD Wallet Path:  | Ethereum Address:                          |
+    |--------+------------------+--------------------------------------------|
     | ETH    | m/44'/60'/0'/0/0 | 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1 |
     | BTC    | m/44'/0'/0'/0/0  | bc1qm5ua96hx30snwrwsfnv97q96h53l86ded7wmjl |
     | ETH    | m/44'/60'/0'/0/1 | 0x8D342083549C635C0494d3c77567860ee7456963 |
     | BTC    | m/44'/0'/0'/0/1  | bc1qwz6v9z49z8mk5ughj7r78hjsp45jsxgzh29lnh |
     | ETH    | m/44'/60'/0'/0/2 | 0x52787E24965E1aBd691df77827A3CfA90f0166AA |
     | BTC    | m/44'/0'/0'/0/2  | bc1q690m430qu29auyefarwfrvfumncunvyw6v53n9 |
     :end:
@@ -1211,53 +1194,47 @@
 *** SLIP-39 Mnemonic to Seed
 
     Lets prove that we can actually recover the *original* Seed Entropy from the SLIP-39 recovery
     Mnemonics; in this case, we've specified a SLIP-39 group_threshold of 2 groups, so we'll use 1
     Mnemonic from Mine, and 2 from the Fam group:
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     _,mnem_mine         = grps['Mine']
     _,mnem_fam          = grps['Fam']
     recseed             = slip39.recover( mnem_mine + mnem_fam[:2] )
     recseed_hex         = codecs.encode( recseed, 'hex_codec' ).decode( 'ascii' )
-    [
-     [ f"{len(recseed)*8}-bit Seed:", f"{recseed_hex}" ]
-    ]
+    print( tabulate( [
+        [ f"{len(recseed)*8}-bit Seed:", f"{recseed_hex}" ]
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[12]:
-    | 0             | 1                                |
-    |---------------+----------------------------------|
     | 128-bit Seed: | ffffffffffffffffffffffffffffffff |
     :end:
     #+LATEX: }
 
 *** SLIP-39 Seed to Address
 
     And we'll use the same style of code as for the BIP-39 example above, to derive the Ethereum
     address *directly* from this recovered 128-bit seed:
 
     #+LATEX: {\scriptsize
-    #+BEGIN_SRC ipython :session :exports both :results raw drawer
+    #+BEGIN_SRC ipython :session :exports both :results output raw drawer
     slip39_eth_hd       = slip39.account( recseed, 'ETH', path )
-    [
-     [ f"{len(slip39_eth_hd.key)*4}-bit derived key path:", f"{path}" ],
-     [ "Produces private key: ", f"{slip39_eth_hd.key}" ],
-     [ "Yields Ethereum address:", f"{slip39_eth_hd.address}" ],
-    ]
+    print( tabulate( [
+        [ f"{len(slip39_eth_hd.key)*4}-bit derived key path:", f"{path}" ],
+        [ "Produces private key: ", f"{slip39_eth_hd.key}" ],
+        [ "Yields Ethereum address:", f"{slip39_eth_hd.address}" ],
+    ], tablefmt='orgtbl' ))
     #+END_SRC
 
     #+RESULTS:
     :results:
-    # Out[13]:
-    | 0                         | 1                                                                |
-    |---------------------------+------------------------------------------------------------------|
     | 256-bit derived key path: | m/44'/60'/0'/0/0                                                 |
     | Produces private key:     | 6a2ec39aab88ec0937b79c8af6aaf2fd3c909e9a56c3ddd32ab5354a06a21a2b |
     | Yields Ethereum address:  | 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1                       |
     :end:
     #+LATEX: }
 
     And we see that we obtain the same Ethereum address =0x824b..1a2b= as we originally got from
@@ -1329,34 +1306,34 @@
     ( python3 -m slip39.recovery --bip39 \
         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
       | python3 -m slip39 --secret - --no-card -v
     ) 2>&1 | tail -20
     #+END_SRC
     #+RESULTS:
     #+begin_example
-    2022-06-10 06:28:24 slip39                7 salary    19 visual    31 extend    43 impulse   55 quarter   
-    2022-06-10 06:28:24 slip39                8 aluminum  20 evoke     32 failure   44 fitness   56 cylinder  
-    2022-06-10 06:28:24 slip39                9 estimate  21 ladybug   33 junior    45 behavior  57 have      
-    2022-06-10 06:28:24 slip39               10 work      22 else      34 hour      46 frost     58 grumpy    
-    2022-06-10 06:28:24 slip39               11 space     23 laundry   35 entrance  47 avoid     59 expand    
-    2022-06-10 06:28:24 slip39               12 peaceful  24 unknown   36 paper     48 kitchen   
-    2022-06-10 06:28:24 slip39           6th  1 remove    13 game      25 discuss   37 gray      49 metric    
-    2022-06-10 06:28:24 slip39                2 steady    14 index     26 daisy     38 hunting   50 slice     
-    2022-06-10 06:28:24 slip39                3 decision  15 ivory     27 problem   39 breathe   51 lair      
-    2022-06-10 06:28:24 slip39                4 spider    16 exotic    28 beaver    40 equip     52 view      
-    2022-06-10 06:28:24 slip39                5 acne      17 cricket   29 reaction  41 glance    53 ounce     
-    2022-06-10 06:28:24 slip39                6 luxury    18 screw     30 slush     42 random    54 glad      
-    2022-06-10 06:28:24 slip39                7 says      19 therapy   31 ultimate  43 increase  55 victim    
-    2022-06-10 06:28:24 slip39                8 depart    20 drove     32 dive      44 senior    56 vampire   
-    2022-06-10 06:28:24 slip39                9 very      21 strike    33 ajar      45 scroll    57 brave     
-    2022-06-10 06:28:24 slip39               10 listen    22 steady    34 ending    46 depart    58 rebuild   
-    2022-06-10 06:28:24 slip39               11 invasion  23 climate   35 lying     47 dough     59 engage    
-    2022-06-10 06:28:24 slip39               12 treat     24 verify    36 scroll    48 very      
-    2022-06-10 06:28:24 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
-    2022-06-10 06:28:24 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
+    2022-10-05 16:34:32 slip39                7 rescue    19 exchange  31 solution  43 increase  55 slap      
+    2022-10-05 16:34:32 slip39                8 jump      20 lunar     32 check     44 rapids    56 lungs     
+    2022-10-05 16:34:32 slip39                9 news      21 fawn      33 income    45 density   57 nervous   
+    2022-10-05 16:34:32 slip39               10 detailed  22 plastic   34 image     46 sack      58 bracelet  
+    2022-10-05 16:34:32 slip39               11 spit      23 lying     35 criminal  47 maximum   59 loyalty   
+    2022-10-05 16:34:32 slip39               12 pajamas   24 morning   36 belong    48 radar     
+    2022-10-05 16:34:32 slip39           6th  1 large     13 method    25 license   37 snapshot  49 medical   
+    2022-10-05 16:34:32 slip39                2 training  14 pile      26 license   38 chubby    50 provide   
+    2022-10-05 16:34:32 slip39                3 decision  15 envy      27 leaves    39 hairy     51 tolerate  
+    2022-10-05 16:34:32 slip39                4 spider    16 dictate   28 gesture   40 literary  52 climate   
+    2022-10-05 16:34:32 slip39                5 academic  17 roster    29 lawsuit   41 revenue   53 adapt     
+    2022-10-05 16:34:32 slip39                6 texture   18 verify    30 chew      42 furl      54 counter   
+    2022-10-05 16:34:32 slip39                7 total     19 endless   31 glasses   43 race      55 surprise  
+    2022-10-05 16:34:32 slip39                8 judicial  20 jacket    32 soul      44 making    56 husband   
+    2022-10-05 16:34:32 slip39                9 racism    21 elegant   33 jewelry   45 mason     57 elite     
+    2022-10-05 16:34:32 slip39               10 mansion   22 building  34 tenant    46 ruin      58 insect    
+    2022-10-05 16:34:32 slip39               11 hearing   23 museum    35 manual    47 switch    59 cylinder  
+    2022-10-05 16:34:32 slip39               12 sharp     24 ticket    36 realize   48 ounce     
+    2022-10-05 16:34:32 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
+    2022-10-05 16:34:32 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
     #+end_example
     #+LATEX: }
     
     This =0xfc20..1B5E= address is the same Ethereum address as is recovered on a Trezor using this
     BIP-39 mnemonic phrase.  Thus, we can generate "Paper Wallets" for the desired Cryptocurrency
     accounts, and recover the funds.
 
@@ -1398,16 +1375,16 @@
     #+LATEX: {\scriptsize3
     #+BEGIN_SRC bash :exports both :results output
     ( python3 -m slip39.recovery --bip39 --entropy -v \
         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" 
     ) 2>&1
     #+END_SRC
     #+RESULTS:
-    : 2022-06-10 06:28:39 slip39.recovery  Recovered 128-bit BIP-39 secret from english mnemonic
-    : 2022-06-10 06:28:39 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
+    : 2022-10-05 16:34:49 slip39.recovery  Recovered 128-bit BIP-39 secret from english mnemonic
+    : 2022-10-05 16:34:49 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
     : ffffffffffffffffffffffffffffffff
     #+LATEX: }
 
     Now we generate SLIP-39 Mnemonics to recover the 128-bit Seed Entropy.  Note that these are
     20-word Mnemonics.  However, these are *NOT* the wallets we expected!  These are the well-known
     native SLIP-39 wallets from the =0xFFFF...FF= Seed Entropy; not the well-known native BIP-39
     wallets from that Seed Entropy, which generate the Ethereum wallet address =0xfc20..1B5E=!  Why
@@ -1418,34 +1395,34 @@
     ( python3 -m slip39.recovery --bip39 --entropy \
         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
       | python3 -m slip39 --secret - --no-card -v
     ) 2>&1 | tail -20
     #+END_SRC
     #+RESULTS:
     #+begin_example
-    2022-06-10 06:28:43 slip39                4 skin      11 sheriff   18 dynamic   
-    2022-06-10 06:28:43 slip39                5 document  12 album     19 diminish  
-    2022-06-10 06:28:43 slip39                6 station   13 overall   20 metric    
-    2022-06-10 06:28:43 slip39                7 smear     14 depend    
-    2022-06-10 06:28:43 slip39           5th  1 desert     8 gather    15 auction   
-    2022-06-10 06:28:43 slip39                2 pipeline   9 living    16 finger    
-    2022-06-10 06:28:43 slip39                3 decision  10 view      17 work      
-    2022-06-10 06:28:43 slip39                4 snake     11 public    18 organize  
-    2022-06-10 06:28:43 slip39                5 dish      12 predator  19 beard     
-    2022-06-10 06:28:43 slip39                6 crucial   13 withdraw  20 health    
-    2022-06-10 06:28:43 slip39                7 extra     14 clock     
-    2022-06-10 06:28:43 slip39           6th  1 desert     8 bracelet  15 game      
-    2022-06-10 06:28:43 slip39                2 pipeline   9 muscle    16 blanket   
-    2022-06-10 06:28:43 slip39                3 decision  10 holiday   17 element   
-    2022-06-10 06:28:43 slip39                4 spider    11 flexible  18 birthday  
-    2022-06-10 06:28:43 slip39                5 buyer     12 acne      19 manager   
-    2022-06-10 06:28:43 slip39                6 minister  13 judicial  20 agency    
-    2022-06-10 06:28:43 slip39                7 pink      14 agency    
-    2022-06-10 06:28:43 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
-    2022-06-10 06:28:43 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
+    2022-10-05 16:34:52 slip39                4 skin      11 very      18 vitamins  
+    2022-10-05 16:34:52 slip39                5 brave     12 treat     19 leaves    
+    2022-10-05 16:34:52 slip39                6 rapids    13 fortune   20 valuable  
+    2022-10-05 16:34:52 slip39                7 therapy   14 script    
+    2022-10-05 16:34:52 slip39           5th  1 length     8 explain   15 reward    
+    2022-10-05 16:34:52 slip39                2 merit      9 usual     16 news      
+    2022-10-05 16:34:52 slip39                3 decision  10 starting  17 receiver  
+    2022-10-05 16:34:52 slip39                4 snake     11 deliver   18 scramble  
+    2022-10-05 16:34:52 slip39                5 briefing  12 grocery   19 wits      
+    2022-10-05 16:34:52 slip39                6 downtown  13 dragon    20 solution  
+    2022-10-05 16:34:52 slip39                7 daisy     14 hamster   
+    2022-10-05 16:34:52 slip39           6th  1 length     8 involve   15 vexed     
+    2022-10-05 16:34:52 slip39                2 merit      9 payment   16 argue     
+    2022-10-05 16:34:52 slip39                3 decision  10 dismiss   17 terminal  
+    2022-10-05 16:34:52 slip39                4 spider    11 shadow    18 clinic    
+    2022-10-05 16:34:52 slip39                5 activity  12 general   19 stilt     
+    2022-10-05 16:34:52 slip39                6 finance   13 nuclear   20 ecology   
+    2022-10-05 16:34:52 slip39                7 oven      14 rhyme     
+    2022-10-05 16:34:52 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
+    2022-10-05 16:34:52 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
     #+end_example
     #+LATEX: }
 
     Because we must tell =slip39= to that we're using the BIP-39 Mnemonic and Seed generation
     process to derived the wallet addresses from the Seed Entropy (not the SLIP-39 standard).  So,
     we add the =-using-bip39= option:
 
@@ -1454,34 +1431,34 @@
     ( python3 -m slip39.recovery --bip39 --entropy \
         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
       | python3 -m slip39 --secret - --no-card -v --using-bip39
     ) 2>&1 | tail -20
     #+END_SRC
     #+RESULTS:
     #+begin_example
-    2022-06-10 06:28:50 slip39                4 skin      11 grill     18 national  
-    2022-06-10 06:28:50 slip39                5 being     12 brother   19 capture   
-    2022-06-10 06:28:50 slip39                6 election  13 royal     20 switch    
-    2022-06-10 06:28:50 slip39                7 ivory     14 juice     
-    2022-06-10 06:28:50 slip39           5th  1 guitar     8 punish    15 ivory     
-    2022-06-10 06:28:50 slip39                2 training   9 fantasy   16 born      
-    2022-06-10 06:28:50 slip39                3 decision  10 therapy   17 survive   
-    2022-06-10 06:28:50 slip39                4 snake     11 patrol    18 garden    
-    2022-06-10 06:28:50 slip39                5 demand    12 that      19 axle      
-    2022-06-10 06:28:50 slip39                6 camera    13 unusual   20 deploy    
-    2022-06-10 06:28:50 slip39                7 revenue   14 home      
-    2022-06-10 06:28:50 slip39           6th  1 guitar     8 flip      15 relate    
-    2022-06-10 06:28:50 slip39                2 training   9 scandal   16 square    
-    2022-06-10 06:28:50 slip39                3 decision  10 spew      17 rocky     
-    2022-06-10 06:28:50 slip39                4 spider    11 style     18 deploy    
-    2022-06-10 06:28:50 slip39                5 answer    12 playoff   19 ugly      
-    2022-06-10 06:28:50 slip39                6 entrance  13 lift      20 intimate  
-    2022-06-10 06:28:50 slip39                7 timely    14 promise   
-    2022-06-10 06:28:50 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
-    2022-06-10 06:28:50 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
+    2022-10-05 16:34:55 slip39                4 skin      11 biology   18 chest     
+    2022-10-05 16:34:55 slip39                5 album     12 subject   19 dough     
+    2022-10-05 16:34:55 slip39                6 merit     13 capacity  20 frequent  
+    2022-10-05 16:34:55 slip39                7 warn      14 canyon    
+    2022-10-05 16:34:55 slip39           5th  1 funding    8 axle      15 reward    
+    2022-10-05 16:34:55 slip39                2 upstairs   9 domestic  16 oral      
+    2022-10-05 16:34:55 slip39                3 decision  10 dynamic   17 canyon    
+    2022-10-05 16:34:55 slip39                4 snake     11 plastic   18 drug      
+    2022-10-05 16:34:55 slip39                5 deadline  12 total     19 primary   
+    2022-10-05 16:34:55 slip39                6 bracelet  13 mother    20 closet    
+    2022-10-05 16:34:55 slip39                7 evidence  14 brother   
+    2022-10-05 16:34:55 slip39           6th  1 funding    8 satisfy   15 black     
+    2022-10-05 16:34:55 slip39                2 upstairs   9 velvet    16 crush     
+    2022-10-05 16:34:55 slip39                3 decision  10 lend      17 lawsuit   
+    2022-10-05 16:34:55 slip39                4 spider    11 radar     18 zero      
+    2022-10-05 16:34:55 slip39                5 bucket    12 license   19 hunting   
+    2022-10-05 16:34:55 slip39                6 class     13 infant    20 voice     
+    2022-10-05 16:34:55 slip39                7 stay      14 year      
+    2022-10-05 16:34:55 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
+    2022-10-05 16:34:55 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
     #+end_example
     #+LATEX: }
 
     And, there we have it -- we've recovered exactly the same Ethereum and Bitcoin wallets as would
     a native BIP-39 hardware wallet like a Ledger Nano.
 
 **** Using SLIP-39 App "Backup" Controls
@@ -1566,14 +1543,82 @@
     : $ git clone git@github.com:pjkundert/python-slip39.git
 
 **** Code Signing    
 
      The MMC (Microsoft Management Console) is used to store your code-signing certificates.  
      See [[https://stackoverflow.com/questions/19879812/signing-exe-with-cer-file-what-is-my-certificates-name-that-signtool-exe-is][stackoverflow.com]] for how to enable its Certificate management.
 
+* Licensing
+
+  Each installation of the SLIP-39 App requires an Ed25519 "Agent" identity, and cryptographically
+  signed license(s) to activate various python-slip39 features.  No license is required to use basic
+  features; advanced features require a license.
+
+** Create an Ed25519 "Agent" Key
+
+   The Ed25519 signing "Agent" identity is loaded at start-up, and (if necessary) is created
+   automatically on first execution.  This is similar to the =ssh-keygen -t ed25519= procedure.
+
+   Each separate installation must have a ~/.crypto-licensing/python-slip39.crypto-keypair.  This
+   contains the licensing "Agent" credentials: a passphrase-encrypted Ed25519 private key, and a
+   self-signed public key.  This shows that we actually had access to the private key and used it to
+   create a signature for the claimed public key and the supplied encrypted private key -- proving
+   that the public key is valid, and associated with the encrypted private key.
+
+** Validating an Advanced Feature License
+
+   When an advanced feature is used, all available =python-slip39.crypto-license= files are loaded.
+   They are examined, and if a license is found that is:
+
+     - Assigned to this Agent and Machine-ID
+     - Contains the required license authorizations
+
+   then the functionality is allowed to proceed.
+
+   If no license is found, instructions on how to obtain a license for this Agent on this Machine-ID
+   will be displayed.
+
+   If you've already obtained a "master" license on your primary machine's SLIP-39 installation, you
+   can use it to issue a sub-license to this installation (eg. for your air-gapped cryptocurrency
+   management machine).
+
+   Otherwise, a URL is displayed at which the required "master" license can be issued.
+
+*** Get a sub-license From Your "master" License
+
+    Typically, you'll be using python-slip39's advanced features on an air-gapped computer.  You do
+    not want to visit websites from this computer.  So, you obtain a sub-license from your primary
+    computer's python-slip39 installation, and place it on your secure air-gapped computer
+    (eg. using a USB stick).
+
+    Take note of the secondary machine's Agent ID (pubkey) and Machine ID.  On your primary
+    computer (with the "master" license), run:
+    : python3 -m slip39.sublicense <agent-pubkey> <machine-id>
+
+    Take the output, and place it in the file =~/.crypto-licensing/python-slip39.crypto-license= on
+    your air-gapped computer.
+    
+*** Obtaining an Advanced Feature "master" License
+
+    On your primary computer, open the provided URL in a browser.  The URL contains the details of
+    the advanced feature desired.
+
+    This URL's web page will request an Ed25519 "Agent" public key to issue your "master" license
+    to.  This should be your primary user account's Ed25519 "Agent" public key -- this master
+    "Agent" will be issuing sub-licenses to any of your other SLIP-39 installations.  You will be
+    redirected to a URL that is unique to the advanced feature plus your Agent ID.
+
+    An invoice will be generated with unique Bitcoin, Ethereum and perhaps other cryptocurrency
+    addresses.  Pay the required amount of cryptocurrency to one of the provided wallet addresses.
+    Within a few seconds, the cryptocurrency transfer will be confirmed.
+
+    Once the payment for the advanced feature is confirmed, the URL including your agent ID will
+    always allow you to re-download the license.  It is only usable by your Agent ID to issue
+    sub-licenses to your python-slip39 installations on your machines.
+
 * Dependencies
 
   Internally, python-slip39 project uses Trezor's [[https://gihub.com/trezor/python-shamir-mnemonic.git][python-shamir-mnemonic]] to encode the seed data to
   SLIP-39 phrases, [[https://github.com/meherett/python-hdwallet.git][python-hdwallet]] to convert seeds to ETH, BTC, LTC and DOGE wallets, and the
   Ethereum project's [[https://github.com/ethereum/eth-account][eth-account]] to produce encrypted JSON wallets for specified Ethereum accounts.
 
 ** The =python-shamir-mnemonic= API
```

### Comparing `slip39-9.0.4/README.pdf` & `slip39-9.1.2/README.pdf`

 * *Files 14% similar despite different names*

#### Comparing `slip39-9.0.4/README.pdf` & `slip39-9.1.2/README.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: 'Perry Kundert'
-CreationDate: "D:20220610063947-06'00'"
-Creator: 'Emacs 28.1 (Org mode 9.5.2)'
+CreationDate: "D:20221005170130-06'00'"
+Creator: 'Emacs 28.2 (Org mode 9.5.2)'
 Keywords: ''
-ModDate: "D:20220610063947-06'00'"
+ModDate: "D:20221005170130-06'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.24 (TeX Live 2022/Homebrew) kpathsea version 6.3.4'
 Producer: 'pdfTeX-1.40.24'
 Subject: ''
 Title: 'Ethereum SLIP-39 Account Generation'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -98,41 +98,41 @@
 16
 17
 17
 18
 18
 19
 20
+20
 21
 21
 21
 22
-23
 
 4 Building & Installing
 4.1 The slip39 Module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 4.2 The slip39 GUI . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 4.2.1 The macOS/win32 SLIP-39.app GUI . . . . . . . . . . . . . . . .
 4.2.2 The Windows 10 SLIP-39 GUI . . . . . . . . . . . . . . . . . . . .
 
 25
 25
-26
-26
+25
+25
 26
 
 2
 
 5 Dependencies
 5.1 The python-shamir-mnemonic API . . . . . . . . . . . . . . . . . . . . . .
 
 1
 
-27
-27
+26
+26
 
 Security with Availability
 
 For both BIP-39 and SLIP-39, a 128- or 256-bit random "seed" is the source of an unlimited sequence of Ethereum and Bitcoin HD (Heirarchical Deterministic) derived Wallet
 accounts. Anyone who can obtain this seed gains control of all Ethereum, Bitcoin (and
 other) accounts derived from it, so it must be securely stored.
 Losing this seed means that all of the HD Wallet accounts are permanently lost. It
@@ -265,21 +265,21 @@
 browser, for example?
 The slip39.gui (and the macOS/win32 SLIP-39.App) support output of standard
 BIP-38 encrypted wallets for Bitcoin-like cryptocurrencies such as BTC, LTC and DOGE.
 It also outputs encrypted Ethereum JSON wallets for ETH. Here is how to produce them
 (from a test secret Seed; exclude --secret ffff... for yours!):
 slip39 -c ETH -c BTC -c DOGE -c LTC --secret ffffffffffffffffffffffffffffffff \
 --no-card --wallet password --wallet-hint ’bad:pass...’ 2>&1
-2022-06-10 06:39:13 slip39
-2022-06-10 06:39:13 slip39
-2022-06-10 06:39:14 slip39.layout
-2022-06-10 06:39:14 slip39.layout
-2022-06-10 06:39:14 slip39.layout
-2022-06-10 06:39:14 slip39.layout
-2022-06-10 06:39:17 slip39.layout
+2022-10-05 17:01:01 slip39
+2022-10-05 17:01:01 slip39
+2022-10-05 17:01:01 slip39.layout
+2022-10-05 17:01:01 slip39.layout
+2022-10-05 17:01:01 slip39.layout
+2022-10-05 17:01:01 slip39.layout
+2022-10-05 17:01:05 slip39.layout
 
 It is recommended to not use ’-s|--secret <hex>’; specify ’-’ to read from input
 It is recommended to not use ’-w|--wallet <password>’; specify ’-’ to read from input
 ETH
 m/44’/60’/0’/0/0
 : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
 BTC
@@ -287,50 +287,50 @@
 : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
 DOGE
 m/44’/3’/0’/0/0
 : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
 LTC
 m/84’/2’/0’/0/0
 : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
-Writing SLIP39-encoded wallet for ’SLIP39’ to: SLIP39-2022-06-10+06.39.15-ETH-0x824b1
+Writing SLIP39-encoded wallet for ’SLIP39’ to: SLIP39-2022-10-05+17.01.02-ETH-0x824b1
 
 And what they look like:
 To recover your real SLIP-39 Seed Entropy and print wallets, use the SLIP-39 App’s
 "Recover" Controls, or to do so on the command-line, use slip39-recover:
 
 slip39-recovery -v \
 --mnemonic "material leaf acrobat romp charity capital omit skunk change firm eclipse crush fancy best tracks flip grownup
 --mnemonic "material leaf beard romp disaster duke flame uncover group slice guest blue gums duckling total suitab
 2>&1
 
 5
 
 Figure 2: Paper Wallets (from --secret ffff...)
-2022-06-10 06:39:18 slip39.recovery
-2022-06-10 06:39:18 slip39.recovery
+2022-10-05 17:01:05 slip39.recovery
+2022-10-05 17:01:05 slip39.recovery
 ffffffffffffffffffffffffffffffff
 
 Recovered 128-bit SLIP-39 Seed Entropy with 2 (all) of 2 supplied mnemonics; Seed dec
 Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39
 
 You can run this as a command-line pipeline. Here, we use some SLIP-39 Mnemonics
 that encode the ffff... Seed Entropy; note that the wallets match those output above:
 
 slip39-recovery \
 --mnemonic "material leaf acrobat romp charity capital omit skunk change firm eclipse crush fancy best tracks flip grownup
 --mnemonic "material leaf beard romp disaster duke flame uncover group slice guest blue gums duckling total suitab
 | slip39 -c ETH -c BTC -c DOGE -c LTC --secret - \
 --no-card --wallet password --wallet-hint ’bad:pass...’ \
 2>&1
-2022-06-10 06:39:18 slip39
-2022-06-10 06:39:18 slip39.layout
-2022-06-10 06:39:18 slip39.layout
-2022-06-10 06:39:18 slip39.layout
-2022-06-10 06:39:18 slip39.layout
-2022-06-10 06:39:22 slip39.layout
+2022-10-05 17:01:06 slip39
+2022-10-05 17:01:06 slip39.layout
+2022-10-05 17:01:06 slip39.layout
+2022-10-05 17:01:06 slip39.layout
+2022-10-05 17:01:06 slip39.layout
+2022-10-05 17:01:10 slip39.layout
 
 2.1.2
 
 It is recommended to not use ’-w|--wallet <password>’; specify ’-’ to read from input
 ETH
 m/44’/60’/0’/0/0
 : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
@@ -339,15 +339,15 @@
 : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
 DOGE
 m/44’/3’/0’/0/0
 : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
 LTC
 m/84’/2’/0’/0/0
 : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
-Writing SLIP39-encoded wallet for ’SLIP39’ to: SLIP39-2022-06-10+06.39.19-ETH-0x824b1
+Writing SLIP39-encoded wallet for ’SLIP39’ to: SLIP39-2022-10-05+17.01.07-ETH-0x824b1
 
 Supported Cryptocurrencies
 
 While the SLIP-39 Seed is not cryptocurrency-specific (any wallet for any cryptocurrency
 can be derived from it), each type of cryptocurrency has its own standard derivation path
 (eg. m/44’/3’/0’/0/0 for DOGE), and its own address representation (eg. Bech32 at
 m/84’/0’/0’/0/0 for BTC eg. bc1qcupw7k8enymvvsa7w35j5hq4ergtvus3zk8a8s.
@@ -472,15 +472,15 @@
 : positional arguments:
 :
 names
 Account names to produce; if --secret Entropy is
 :
 supplied, only one is allowed.
 :
-: optional arguments:
+: options:
 :
 -h, --help
 show this help message and exit
 :
 -v, --verbose
 Display logging information.
 :
@@ -620,45 +620,45 @@
 Enter 4th SLIP-39 mnemonic: veteran guilt beard romp dragon island merit burden aluminum worthy ...
 2021-12-25 11:03:33 slip39.recovery Recovered SLIP-39 secret; Use: python3 -m slip39 --secret ...
 383597fd63547e7c9525575decd413f7
 
 Finally, re-create the wallet seed, perhaps including an encrypted JSON Paper Wallet for import of some accounts into a software wallet (use --json password to output
 encrypted Ethereum JSON wallet files):
 slip39 --secret 383597fd63547e7c9525575decd413f7 --wallet password --wallet-hint bad:pass... 2>&1
-2022-06-10 06:39:23 slip39
-2022-06-10 06:39:23 slip39
-2022-06-10 06:39:23 slip39.layout
-2022-06-10 06:39:23 slip39.layout
-2022-06-10 06:39:26 slip39.layout
+2022-10-05 17:01:11 slip39
+2022-10-05 17:01:11 slip39
+2022-10-05 17:01:11 slip39.layout
+2022-10-05 17:01:11 slip39.layout
+2022-10-05 17:01:13 slip39.layout
 
 2.4.1
 
 It is recommended to not use ’-s|--secret <hex>’; specify ’-’ to read from input
 It is recommended to not use ’-w|--wallet <password>’; specify ’-’ to read from input
 ETH
 m/44’/60’/0’/0/0
 : 0xb44A2011A99596671d5952CdC22816089f142FB3
 BTC
 m/84’/0’/0’/0/0
 : bc1qcupw7k8enymvvsa7w35j5hq4ergtvus3zk8a8s
-Writing SLIP39-encoded wallet for ’SLIP39’ to: SLIP39-2022-06-10+06.39.24-ETH-0xb44A2
+Writing SLIP39-encoded wallet for ’SLIP39’ to: SLIP39-2022-10-05+17.01.12-ETH-0xb44A2
 
 slip39.recovery Synopsis
 
 slip39-recovery --help 2>&1
 
 | sed ’s/^/: /’ # (just for output formatting)
 
 : usage: slip39-recovery [-h] [-v] [-q] [-m MNEMONIC] [-e] [-b] [-u]
 :
 [-p PASSPHRASE]
 :
 : Recover and output secret Seed from SLIP-39 or BIP-39 Mnemonics
 :
-: optional arguments:
+: options:
 
 9
 
 :
 -h, --help
 show this help message and exit
 :
@@ -729,37 +729,37 @@
 Then, we recover the master secret seed in hex with slip39-recovery, and finally
 send it to slip39 --secret - to re-generate the same wallet as we originally created.
 ( python3 -m slip39 --text --no-card \
 | ( sort -r ; echo "...later..." 1>&2 ) \
 | python3 -m slip39.recovery \
 | python3 -m slip39 --secret - --no-card \
 ) 2>&1
-2022-06-10 06:39:27 slip39.layout
-2022-06-10 06:39:27 slip39.layout
+2022-10-05 17:01:14 slip39.layout
+2022-10-05 17:01:14 slip39.layout
 ...later...
-2022-06-10 06:39:27 slip39.layout
-2022-06-10 06:39:27 slip39.layout
+2022-10-05 17:01:14 slip39.layout
+2022-10-05 17:01:14 slip39.layout
 
 ETH
 BTC
 
 m/44’/60’/0’/0/0
 m/84’/0’/0’/0/0
 
-: 0xbda76fEBb9CFafd3d603b840a29b1CC91C34057B
-: bc1qh8uthcv23kr4j6f0n4q9pvlmndhwaqv4n6x2ur
+: 0x9c0a51d69303A9e6596B5AD5560cB4ed23fcC66F
+: bc1q2dadecuwl5f5ruferhuvdzmpek8rcmlr367lry
 
 ETH
 BTC
 
 m/44’/60’/0’/0/0
 m/84’/0’/0’/0/0
 
-: 0xbda76fEBb9CFafd3d603b840a29b1CC91C34057B
-: bc1qh8uthcv23kr4j6f0n4q9pvlmndhwaqv4n6x2ur
+: 0x9c0a51d69303A9e6596B5AD5560cB4ed23fcC66F
+: bc1q2dadecuwl5f5ruferhuvdzmpek8rcmlr367lry
 
 10
 
 2.5
 
 Generation of Addresses
 
@@ -781,15 +781,15 @@
 :
 [--enumerated] [--no-enumerate] [--receive]
 :
 [--corrupt CORRUPT]
 :
 : Generate public wallet address(es) from a secret seed
 :
-: optional arguments:
+: options:
 :
 -h, --help
 show this help message and exit
 :
 -v, --verbose
 Display logging information.
 :
@@ -906,19 +906,19 @@
 3: [["ETH", "m/44’/60’/0’/0/3", "0x909f59835A5a120EafE1c60742485b7ff0e305da"], ["BTC", "m/84’/0’/0’/0/3", "bc1q6t9vhestkcf
 
 We can encrypt the output, to secure the sequence (and due to integrated MACs,
 ensures no errors occur over an insecure channel like a serial cable):
 ( slip39-recovery --bip39 --mnemonic ’zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong’ \
 | slip39-generator --secret - --path ’../-3’ --encrypt ’password’ ) 2>&1
 
-nonce: 123214ca926b596e14e25ed56da59a4b76bd2be887ab499ccd751655
-0: 13400570d94908a968d160811a0623bd0c41ea721f0a8cc0145e962b062ad0948760e21e12fcbac490f059fecb1f86e089410df97858dc5ec7a
-1: dfb0417ebff97df188f1893a7b49be5230a413d47d4c11bbb6b6b73f170f04be77717644356b799096f7bacf2d997aec10ab398fab9ec851a0f
-2: 880c4f69df01433b9a3486f9678c080ca920ba04e3e182172aea90d3174a2855fc412cc6a3729ac4dd99aeec8d32eda03bcf8b869e800834ddb
-3: 1bd122669988362bbd06fec202cdbe4de7fa3c00841487118706a9fe735e0587d33f1912ca28db37fff1c91a2634cef9dd6c4725e4f71407fbd
+nonce: aecf9408c46fdbbfb681b439e4eb2819970767d97467a087bccccb82
+0: 9770d26000a922248a84769d37366b62f8122a5a0c25e3a35aacd5b68b410895a94d8bbb87d6eb4815eafc57e7df7c261faeca4329e3eefcf6e
+1: 5e98935234787dd65345efc605204378b88fb4cd437b2a9762024ca53d887c5afca60e0fde00bad9ac2dad37900eaae3657ee0f1f3125222a2d
+2: 73417b3e3c0bce95cdc5816eacc29ce914761530b78f9893aad650250d2e5731decb160617e7382d92c5763f56fc02d1810e829b2a846f55a21
+3: ff886225ad75264ccad761789b946404ec44ff4d01cdc9c5aa3e099cf2cbc0c8541bc9dbaff582ca40ed16c71ff091a9fafb971780663c9d41f
 
 On the receiving computer, we can decrypt and recover the stream of accounts from
 the wallet seed; any rows with errors are ignored:
 ( slip39-recovery --bip39 --mnemonic ’zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong’ \
 | slip39-generator --secret - --path ’../-3’ --encrypt ’password’ \
 | slip39-generator --receive --decrypt ’password’ ) 2>&1
 
@@ -976,14 +976,15 @@
 Like groups, w/ <members> = ["<mnemonics>", . . . ]
 Resultant list of groups of accounts
 Seed produced from entropy using BIP-39 generation
 
 This is immediately usable to pass to slip39.output.
 import codecs
 import random
+from tabulate import tabulate
 
 #
 # NOTE:
 #
 # We turn off randomness here during SLIP-39 generation to get deterministic phrases;
 # during normal operation, secure entropy is used during mnemonic generation, yielding
 # random phrases, even when the same seed is used multiple times.
@@ -997,30 +998,28 @@
 = b’\xFF’ * 16
 passphrase
 = b""
 create_details
 = slip39.create(
 "Test", 2, { "Mine": (1,1), "Fam": (2,3) },
 master_secret=master_secret, passphrase=passphrase, cryptopaths=cryptopaths )
-[
+print( tabulate( [
 [
 f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" if l_n == 0 else ""
 ] + words
 for g_name,(g_of,g_mnems) in create_details.groups.items()
 for g_n,mnem in enumerate( g_mnems )
 for l_n,(line,words) in enumerate(slip39.organize_mnemonic(
 mnem, label=f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" ))
-]
+], tablefmt=’orgtbl’ ))
 
 13
 
-0
-Mine(1/1) #1:
+Mine(1/1) #1:
 
-1
 1 academic
 2 acid
 3 acrobat
 4 easy
 5 change
 6 injury
 7 painting
@@ -1048,15 +1047,14 @@
 
 Fam(2/3) #1:
 
 Fam(2/3) #2:
 
 Fam(2/3) #3:
 
-2
 8 safari
 9 drug
 10 browser
 11 trash
 12 fridge
 13 busy
 14 finger
@@ -1078,15 +1076,14 @@
 9 invasion
 10 bumpy
 11 identify
 12 anxiety
 13 august
 14 sunlight
 
-3
 15 standard
 16 angry
 17 similar
 18 aspect
 19 smug
 20 violence
 15 dwarf
@@ -1105,30 +1102,28 @@
 16 satoshi
 17 hobo
 18 ounce
 19 both
 20 award
 
 Add the resultant HD Wallet addresses:
-[
+print( tabulate( [
 [ account.path, account.address ]
 for group in create_details.accounts
 for account in group
-]
-0
+], tablefmt=’orgtbl’ ))
 m/44’/60’/0’/0/0
 m/44’/0’/0’/0/0
 m/44’/60’/0’/0/1
 m/44’/0’/0’/0/1
 m/44’/60’/0’/0/2
 m/44’/0’/0’/0/2
 
 2.6.2
 
-1
 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
 bc1qm5ua96hx30snwrwsfnv97q96h53l86ded7wmjl
 0x8D342083549C635C0494d3c77567860ee7456963
 bc1qwz6v9z49z8mk5ughj7r78hjsp45jsxgzh29lnh
 0x52787E24965E1aBd691df77827A3CfA90f0166AA
 bc1q690m430qu29auyefarwfrvfumncunvyw6v53n9
 
@@ -1155,38 +1150,36 @@
 ’Letter’, . . .
 Force an orientation (default: portrait, landscape)
 Produce a cover page w/ the text (and BIP-39 Phrase if using_bip39)
 
 Layout and produce a PDF containing all the SLIP-39 details on cards for the crypto
 accounts, on the paper_format provided. Returns the paper (orientation,format) used,
 the FPDF, and passes through the supplied cryptocurrency accounts derived.
+(paper_format,orientation),pdf,accounts = slip39.produce_pdf( *create_details )
+pdf_binary = pdf.output()
 
 14
 
-(paper_format,orientation),pdf,accounts = slip39.produce_pdf( *create_details )
-pdf_binary = pdf.output()
-[
+print( tabulate( [
 [ "Orientation:",orientation ],
 [ "Paper:",paper_format ],
 [ "PDF Pages:",pdf.pages_count ],
 [ "PDF Size:",len( pdf_binary )],
-]
-0
+], tablefmt=’orgtbl’ ))
 Orientation:
 Paper:
 PDF Pages:
 PDF Size:
 
 2.6.3
 
-1
 landscape
 Letter
 1
-13028
+13137
 
 slip39.write_pdfs
 
 Key
 names
 master_secret
 passphrase
@@ -1242,21 +1235,20 @@
 
 Takes a number of SLIP-39 mnemonics, and if sufficient group_threshold groups’ mnemonics are present (and the options passphrase is supplied), the master_secret is recovered.
 This can be used with slip39.accounts to directly obtain any Account data.
 Note that the SLIP-39 passphrase is not checked; entering a different passphrase for
 the same set of mnemonics will recover a different wallet! This is by design; it allows
 the holder of the SLIP-39 mnemonic phrases to recover a "decoy" wallet by supplying a
 specific passphrase, while protecting the "primary" wallet.
-
-15
-
-Therefore, it is essential to remember any non-default (non-empty) passphrase used,
+Therefore, it is essential to remember any non-default (non-empty) passphrase used,
 separately and securely. Take great care in deciding if you wish to use a passphrase with
 your SLIP-39 wallet!
-Key
+15
+
+Key
 mnemonics
 passphrase
 using_bip39
 
 Description
 ["<mnemonics>", . . . ]
 Optional passphrase to decrypt secret Seed Entropy
@@ -1274,25 +1266,23 @@
 recoveryvalid
 = slip39.recover(
 create_details.groups[’Mine’][1][:] + create_details.groups[’Fam’][1][:2],
 passphrase=passphrase
 )
 recoveryvalid_hex
 = codecs.encode( recoveryvalid, ’hex_codec’ ).decode( ’ascii’ )
-[
+print( tabulate( [
 [ f"{len(recoverydecoy)*8}-bit secret (decoy):", f"{recoverydecoy_hex}" ],
 [ f"{len(recoveryvalid)*8}-bit secret recovered:", f"{recoveryvalid_hex}" ]
-]
-0
+], tablefmt=’orgtbl’ ))
 128-bit secret (decoy):
 128-bit secret recovered:
 
 2.6.5
 
-1
 2e522cea2b566840495c220cf79c756e
 ffffffffffffffffffffffffffffffff
 
 slip39.recover_bip39
 
 Generate the 512-bit Seed from a BIP-39 Mnemonic + passphrase. Or, return the original
 128- to 256-bit Seed Entropy, if as_entropy is specified.
@@ -1327,14 +1317,15 @@
 
 If we already have a BIP-39 wallet, it would certainly be nice to be able to create nice,
 safe SLIP-39 mnemonics for it, and discard the unsafe BIP-39 mnemonics we have lying
 around, just waiting to be accidentally discovered and the account compromised!
 Fortunately, we can do this! It takes a bit of practice to become comfortable with
 the process, but once you do – you can confidently discard your original insecure and
 unreliable BIP-39 Mnemonic backups.
+
 16
 
 3.1
 
 BIP-39 vs. SLIP-39 Incompatibility
 
 Unfortunately, it is not possible to cleanly convert a BIP-39 generated wallet Seed into
@@ -1367,61 +1358,56 @@
 entropy_hex = codecs.encode( entropy, ’hex_codec’ ).decode( ’ascii’ )
 entropy_mnemonic
 = bip39_english.to_mnemonic( entropy )
 recovered = slip39.recover_bip39( entropy_mnemonic, as_entropy=True )
 recovered_hex = codecs.encode( recovered, ’hex_codec’ ).decode( ’ascii’ )
 recovered_seed = slip39.recover_bip39( entropy_mnemonic, passphrase=passphrase )
 recovered_seed_hex = codecs.encode( recovered_seed, ’hex_codec’ ).decode( ’ascii’ )
-[
+print( tabulate( [
 [ "Original Entropy", entropy_hex ],
 [ "BIP-39 Mnemonic", entropy_mnemonic ],
 [ "Recovered Entropy", recovered_hex ],
 [ "Recovered Seed", f"{recovered_seed_hex:.50}..." ],
-]
-0
+], tablefmt=’orgtbl’))
 Original Entropy
 BIP-39 Mnemonic
 Recovered Entropy
 Recovered Seed
 
-1
 ffffffffffffffffffffffffffffffff
 zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong
 ffffffffffffffffffffffffffffffff
 b6a6d8921942dd9806607ebc2750416b289adea669198769f2. . .
 
-Each word is one of a corpus of 2048 words; therefore, each word encodes 11 bits (2048 =
-2**11) of entropy. So, we provided 128 bits, but 12*11 = 132. So where does
-the extra 4 bits of data come from?
+Each word is one of a corpus of 2048 words; therefore, each word encodes 11 bits (2048
+= 2**11) of entropy. So, we provided 128 bits, but 12*11 = 132. So where does the extra
+4 bits of data come from?
 It comes from the first few bits of a SHA256 hash of the entropy, which is added to
-the end of the supplied 128 bits, to reach the required 132 bits: 132 / 11 == 12 words.
+the end of the supplied 128 bits, to reach the required 132 bits: 132 / 11 = 12 words.
 17
 
 This last 4 bits (up to 8 bits, for a 256-bit 24-word BIP-39) is checked, when validating
 the BIP-39 mnemonic. Therefore, making up a random BIP-39 mnemonic will succeed
-only 1 / 16 times on average, due to an incorrect checksum 4-bit (16 == 2**4) . Lets
-check:
+only 1 / 16 times on average, due to an incorrect checksum 4-bit (16 = 2**4) . Lets check:
 def random_words( n, count=100 ):
 for _ in range( count ):
 yield ’ ’.join( random.choice( bip39_english.wordlist ) for _ in range( n ))
 successes
 = sum(
 bip39_english.check( m )
 for i,m in enumerate( random_words( 12, 10000 ))) / 100
-[
+print( tabulate( [
 [ "Valid random 12-word mnemonics:", f"{successes}%" ],
 [ "Or, about: ", f"1 / {100/successes:.3}" ],
-]
-0
+], tablefmt=’orgtbl’ ))
 Valid random 12-word mnemonics:
 Or, about:
 
-1
-6.25%
-1 / 16.0
+6.27%
+1 / 15.9
 
 Sure enough, about 1/16 random 12-word phrases are valid BIP-39 mnemonics. OK,
 we’ve got the contents of the BIP-39 phrase dialed in. How is it used to generate accounts?
 3.1.2
 
 BIP-39 Mnemonic to Seed
 
@@ -1430,53 +1416,49 @@
 normalized text (not the Entropy bytes) of the 12-word mnemonic is then used (with a
 salt of "mnemonic" plus an optional passphrase, "" by default), to obtain the 512-bit
 seed:
 seed
 = bip39_english.to_seed( entropy_mnemonic )
 seed_hex
 = codecs.encode( seed, ’hex_codec’ ).decode( ’ascii’ )
-[
+print( tabulate( [
 [ f"{len(seed)*8}-bit seed:", f"{seed_hex:.50}..." ]
-]
-0
+], tablefmt=’orgtbl’ ))
 512-bit seed:
 
 3.1.3
 
-1
 b6a6d8921942dd9806607ebc2750416b289adea669198769f2. . .
 
 BIP-39 Seed to Address
 
 Finally, this 512-bit seed is used to derive HD wallet(s). The HD Wallet key derivation
 process consumes whatever seed entropy is provided (512 bits in the case of BIP-39),
 and uses HMAC SHA512 with a prefix of b"Bitcoin seed" to stretch the supplied seed
 entropy to 64 bytes (512 bits). Then, the HD Wallet path segments are iterated through,
 permuting the first 32 bytes of this material as the key with the second 32 bytes of
 material as the chain node, until finally the 32-byte (256-bit) Ethereum account private
 key is produced. We then use this private key to compute the rest of the Ethereum
 account details, such as its public address.
-
-18
-
-path
+path
 = "m/44’/60’/0’/0/0"
 bip39_eth_hd
 = slip39.account( seed, ’ETH’, path )
-[
+print( tabulate( [
 [ f"{len(bip39_eth_hd.key)*4}-bit derived key path:", f"{path}" ],
-[ "Produces private key: ", f"{bip39_eth_hd.key}" ],
+
+18
+
+[ "Produces private key: ", f"{bip39_eth_hd.key}" ],
 [ "Yields Ethereum address:", f"{bip39_eth_hd.address}" ],
-]
-0
+], tablefmt=’orgtbl’ ))
 256-bit derived key path:
 Produces private key:
 Yields Ethereum address:
 
-1
 m/44’/60’/0’/0/0
 7af65ba4dd53f23495dcb04995e96f47c243217fc279f10795871b725cd009ae
 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
 
 Thus, we see that while the 12-word BIP-39 mnemonic careful preserves the original
 128-bit entropy, this data is not directly used to derive the wallet private key and address.
 Also, since an irreversible hash is used to derive the Seed from the Mnemonic, we can’t
@@ -1486,34 +1468,29 @@
 SLIP-39 Entropy to Mnemonic
 
 Just like BIP-39 carefully preserves the original 128-bit Seed Entropy bytes in a single
 12-word mnemonic phrase, SLIP-39 preserves the original 128- or 256-bit Seed Entropy
 in a set of 20- or 33-word Mnemonic phrases.
 name,thrs,grps,acct,ub39 = slip39.create(
 "Test", 2, { "Mine": (1,1), "Fam": (2,3) }, entropy )
-[
+print( tabulate( [
 [ f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" if l_n == 0 else "" ] + words
 for g_name,(g_of,g_mnems) in grps.items()
 for g_n,mnem in enumerate( g_mnems )
 for l_n,(line,words) in enumerate(slip39.organize_mnemonic(
 mnem, rows=7, cols=3, label=f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" ))
-]
-
-19
-
-0
+], tablefmt=’orgtbl’ ))
 Mine(1/1) #1:
 
 Fam(2/3) #1:
 
 Fam(2/3) #2:
 
 Fam(2/3) #3:
 
-1
 1 academic
 2 acid
 3 acrobat
 4 easy
 5 change
 6 injury
 7 painting
@@ -1535,15 +1512,14 @@
 2 acid
 3 beard
 4 entrance
 5 alarm
 6 health
 7 discuss
 
-2
 8 safari
 9 drug
 10 browser
 11 trash
 12 fridge
 13 busy
 14 finger
@@ -1565,15 +1541,14 @@
 9 invasion
 10 bumpy
 11 identify
 12 anxiety
 13 august
 14 sunlight
 
-3
 15 standard
 16 angry
 17 similar
 18 aspect
 19 smug
 20 violence
 15 dwarf
@@ -1593,110 +1568,100 @@
 17 hobo
 18 ounce
 19 both
 20 award
 
 Since there is some randomness used in the SLIP-39 mnemonics generation process,
 we would get a different set of words each time for the fixed "entropy" 0xFFFF..FF used
-in this example (if we hadn’t manually disabled entropy for shamir_mnemonic, above),
+19
+
+in this example (if we hadn’t manually disabled entropy for shamir_mnemonic, above),
 but we will always derive the same Ethereum account 0x824b..19a1 at the specified HD
 Wallet derivation path.
-[
-[ "Crypto", "HD Wallet Path:", "Ethereum Address:" ]
-] + [
+print( tabulate( [
 [ account.crypto, account.path, account.address ]
 for group in create_details.accounts
 for account in group
-]
-0
+], tablefmt=’orgtbl’, headers=[ "Crypto", "HD Wallet Path:", "Ethereum Address:" ] ))
 Crypto
 ETH
 BTC
 ETH
 BTC
 ETH
 BTC
 
 3.1.5
 
-1
 HD Wallet Path:
 m/44’/60’/0’/0/0
 m/44’/0’/0’/0/0
 m/44’/60’/0’/0/1
 m/44’/0’/0’/0/1
 m/44’/60’/0’/0/2
 m/44’/0’/0’/0/2
 
-2
 Ethereum Address:
 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
 bc1qm5ua96hx30snwrwsfnv97q96h53l86ded7wmjl
 0x8D342083549C635C0494d3c77567860ee7456963
 bc1qwz6v9z49z8mk5ughj7r78hjsp45jsxgzh29lnh
 0x52787E24965E1aBd691df77827A3CfA90f0166AA
 bc1q690m430qu29auyefarwfrvfumncunvyw6v53n9
 
 SLIP-39 Mnemonic to Seed
 
 Lets prove that we can actually recover the original Seed Entropy from the SLIP-39
 recovery Mnemonics; in this case, we’ve specified a SLIP-39 group_threshold of 2 groups,
 so we’ll use 1 Mnemonic from Mine, and 2 from the Fam group:
 _,mnem_mine
-
 = grps[’Mine’]
-
-20
-
-_,mnem_fam
+_,mnem_fam
 = grps[’Fam’]
 recseed
 = slip39.recover( mnem_mine + mnem_fam[:2] )
 recseed_hex
 = codecs.encode( recseed, ’hex_codec’ ).decode( ’ascii’ )
-[
+print( tabulate( [
 [ f"{len(recseed)*8}-bit Seed:", f"{recseed_hex}" ]
-]
-0
+], tablefmt=’orgtbl’ ))
 128-bit Seed:
 
 3.1.6
 
-1
 ffffffffffffffffffffffffffffffff
 
 SLIP-39 Seed to Address
 
 And we’ll use the same style of code as for the BIP-39 example above, to derive the
 Ethereum address directly from this recovered 128-bit seed:
 slip39_eth_hd
 = slip39.account( recseed, ’ETH’, path )
-[
+print( tabulate( [
 [ f"{len(slip39_eth_hd.key)*4}-bit derived key path:", f"{path}" ],
 [ "Produces private key: ", f"{slip39_eth_hd.key}" ],
 [ "Yields Ethereum address:", f"{slip39_eth_hd.address}" ],
-]
-0
+], tablefmt=’orgtbl’ ))
 256-bit derived key path:
 Produces private key:
 Yields Ethereum address:
 
-1
 m/44’/60’/0’/0/0
 6a2ec39aab88ec0937b79c8af6aaf2fd3c909e9a56c3ddd32ab5354a06a21a2b
 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
 
 And we see that we obtain the same Ethereum address 0x824b..1a2b as we originally got from slip39.create above. However, this is not the same Ethereum wallet
 address obtained from BIP-39 with exactly the same 0xFFFF...FF Seed Entropy, which
 was 0xfc20..1B5E!
 This is due to the fact that BIP-39 does not use the recovered Seed Entropy to produce
 the seed like SLIP-39 does, but applies additional one-way hashing of the Mnemonic to
 produce a 512-bit Seed.
+20
 
-3.2
+3.2
 
 BIP-39 vs SLIP-39 Key Derivation Summary
 
 At no time in BIP-39 account derivation is the original 128-bit Seed Entropy used (directly) in the derivation of the wallet key. This differs from SLIP-39, which directly uses
 the 128-bit Seed Entropy recovered from the SLIP-39 Shamir’s Secret Sharing System
 recovery process to generate each HD Wallet account’s private key.
 Furthermore, there is no point in the BIP-39 Seed Entropy to account generation
@@ -1707,18 +1672,15 @@
 
 3.3
 
 BIP-39 Backup via SLIP-39
 
 Here are the two available methods for backing up insecure and unreliable BIP-39 Mnemonic
 phrases, using SLIP-39.
-
-21
-
-The first "Emergency Recovery" method allows you to recover your BIP-39 generated
+The first "Emergency Recovery" method allows you to recover your BIP-39 generated
 wallets without the passphrase, but does not support recovery using hardware wallets;
 you must output "Paper Wallets" and use them to recover the Cryptocurrency funds.
 The second "Best Recovery: Using BIP-39" allows us to recover the accounts to any
 standard BIP-39 hardware wallet! However, the SLIP-39 Mnemonics are not compatible
 with standard SLIP-39 wallets like the Trezor "Model T" – you have to use the recovered
 BIP-39 Mnemonic phrase to recover the hardware wallet.
 3.3.1
@@ -1734,129 +1696,129 @@
 BIP-39 mnemonic + passphrase – without abandoning your existing BIP-39 wallets.
 We’ll use slip39.recovery --bip39 ... to recover the 512-bit stretched seed from
 BIP-39:
 ( python3 -m slip39.recovery --bip39 -v \
 --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong"
 ) 2>&1
 
-2022-06-10 06:39:37 slip39.recovery Recovered 512-bit BIP-39 secret from english mnemonic
-2022-06-10 06:39:37 slip39.recovery Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39
+2022-10-05 17:01:23 slip39.recovery Recovered 512-bit BIP-39 secret from english mnemonic
+2022-10-05 17:01:23 slip39.recovery Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39
 b6a6d8921942dd9806607ebc2750416b289adea669198769f2e15ed926c3aa92bf88ece232317b4ea463e84b0fcd3b53577812ee449ccc448eb45e6f54
 
 Then we can generate a 59-word SLIP-39 mnemonic set from the 512-bit secret:
-( python3 -m slip39.recovery --bip39 \
+
+21
+
+( python3 -m slip39.recovery --bip39 \
 --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
 | python3 -m slip39 --secret - --no-card -v
 ) 2>&1 | tail -20
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39
-2022-06-10 06:39:37 slip39.layout
-2022-06-10 06:39:37 slip39.layout
-
-7 tendency 19 clogs
-31 teacher
-43 husband
-55 symbolic
-8 sidewalk 20 syndrome 32 platform 44 join
-56 lying
-9 prevent
-21 hesitate 33 alarm
-45 gravity
-57 answer
-10 pancake
-22 album
-34 wildlife 46 shelter
-58 evening
-11 fridge
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39
+2022-10-05 17:01:23 slip39.layout
+2022-10-05 17:01:23 slip39.layout
+
+7 percent
+19 slavery
+31 elder
+43 grant
+55 radar
+8 endorse
+20 erode
+32 check
+44 aunt
+56 medical
+9 pulse
+21 knit
+33 theory
+45 judicial 57 analysis
+10 pants
+22 crucial
+34 tricycle 46 stadium
+58 cultural
+11 view
 23 guest
-35 fatal
-47 metric
-59 prayer
-12 relate
-24 multiple 36 debris
-48 gasoline
-6th 1 flea
-13 pumps
-25 afraid
-37 desktop
-49 kernel
-2 roster
-14 petition 26 campus
-38 density
-50 steady
-3 decision 15 unknown
-27 silver
-39 jump
-51 ordinary
+35 omit
+47 document 59 webcam
+12 manual
+24 royal
+36 upstairs 48 smear
+6th 1 making
+13 lair
+25 taxi
+37 tricycle 49 cover
+2 regret
+14 faint
+26 emission 38 chemical 50 email
+3 decision 15 kitchen
+27 exact
+39 disease
+51 receiver
 4 spider
-16 huge
-28 crisis
-40 library
-52 shaped
+16 trend
+28 findings 40 ticket
+52 counter
 5 acne
-17 wavy
-29 weapon
-41 thorn
-53 huge
-6 temple
-18 custody
-30 warmth
-42 trust
-54 forward
-7 gums
-19 forbid
-31 afraid
-43 forecast 55 orbit
-8 literary 20 fishing
-32 wealthy
-44 rebuild
-56 image
-9 order
-21 timber
-33 rainbow
-45 fantasy
-57 should
-10 prize
-22 license
-34 privacy
-46 slice
-58 stadium
-11 crunch
-23 military 35 soul
-47 agency
-59 should
-12 crazy
-24 elevator 36 arcade
-48 become
+17 desire
+29 lizard
+41 penalty
+53 being
+6 mixture
+18 gravity
+30 pitch
+42 inside
+54 empty
+7 gray
+19 warmth
+31 rhyme
+43 trend
+55 username
+8 crucial
+20 budget
+32 buyer
+44 petition 56 liquid
+9 terminal 21 modify
+33 database 45 wrist
+57 findings
+10 rumor
+22 regret
+34 garlic
+46 garden
+58 glance
+11 helpful
+23 judicial 35 problem
+47 standard 59 juice
+12 drift
+24 center
+36 mother
+48 similar
 ETH
 m/44’/60’/0’/0/0
 : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
 BTC
 m/84’/0’/0’/0/0
 : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
 
-22
-
-This 0xfc20..1B5E address is the same Ethereum address as is recovered on a Trezor
+This 0xfc20..1B5E address is the same Ethereum address as is recovered on a Trezor
 using this BIP-39 mnemonic phrase. Thus, we can generate "Paper Wallets" for the
 desired Cryptocurrency accounts, and recover the funds.
 So, this does the job:
 • Uses our original BIP-39 Mnemonic
 • Does not require remembering the BIP-39 passphrase
 • Preserves all of the original wallets
 But:
@@ -1870,211 +1832,204 @@
 
 Best Recovery: Using Recovered BIP-39 Mnemonic Phrase
 
 The best solution is to use SLIP-39 to back up the original BIP-39 Seed Entropy (not the
 generated Seed), and then later recover that Seed Entropy and re-generate the BIP-39
 Mnemonic phrase. You will continue to need to remember and use your original BIP-39
 passphrase:
+22
 
-First, observe that we can recover the 128-bit Seed Entropy from the BIP-39 Mnemonic
+First, observe that we can recover the 128-bit Seed Entropy from the BIP-39 Mnemonic
 phrase (not the 512-bit generated Seed): 3
 ( python3 -m slip39.recovery --bip39 --entropy -v \
 --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong"
 ) 2>&1
-2022-06-10 06:39:42 slip39.recovery
-2022-06-10 06:39:42 slip39.recovery
+2022-10-05 17:01:25 slip39.recovery
+2022-10-05 17:01:25 slip39.recovery
 ffffffffffffffffffffffffffffffff
 
 Recovered 128-bit BIP-39 secret from english mnemonic
 Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39
 
-23
-
-Now we generate SLIP-39 Mnemonics to recover the 128-bit Seed Entropy. Note that
+Now we generate SLIP-39 Mnemonics to recover the 128-bit Seed Entropy. Note that
 these are 20-word Mnemonics. However, these are NOT the wallets we expected! These
 are the well-known native SLIP-39 wallets from the 0xFFFF...FF Seed Entropy; not the
 well-known native BIP-39 wallets from that Seed Entropy, which generate the Ethereum
 wallet address 0xfc20..1B5E! Why not?
 3
 ( python3 -m slip39.recovery --bip39 --entropy \
 --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
 | python3 -m slip39 --secret - --no-card -v
 ) 2>&1 | tail -20
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39
-2022-06-10 06:39:42 slip39.layout
-2022-06-10 06:39:42 slip39.layout
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39
+2022-10-05 17:01:25 slip39.layout
+2022-10-05 17:01:25 slip39.layout
 
 5th
 
 6th
 
 ETH
 BTC
 
 4 skin
-11 fake
-18 pile
-5 carpet
-12 center
-19 slap
-6 epidemic 13 blimp
-20 terminal
-7 holiday
-14 desire
-1 rich
-8 river
-15 vitamins
-2 hush
-9 valuable 16 flame
-3 decision 10 hanger
-17 transfer
+11 river
+18 smirk
+5 crowd
+12 guitar
+19 jewelry
+6 skin
+13 ocean
+20 pitch
+7 drug
+14 adjust
+1 dynamic
+8 findings 15 wildlife
+2 guilt
+9 chest
+16 birthday
+3 decision 10 explain
+17 evening
 4 snake
-11 wildlife 18 together
-5 cause
-12 buyer
-19 pupal
-6 lizard
-13 painting 20 decision
-7 nail
-14 sheriff
-1 rich
-8 umbrella 15 decent
-2 hush
-9 born
-16 mansion
-3 decision 10 forbid
-17 either
+11 adorn
+18 system
+5 duke
+12 quick
+19 crystal
+6 group
+13 dryer
+20 owner
+7 taste
+14 twice
+1 dynamic
+8 taught
+15 frequent
+2 guilt
+9 warn
+16 carve
+3 decision 10 intend
+17 mansion
 4 spider
-11 review
-18 recover
-5 demand
-12 born
-19 ancient
-6 budget
-13 vitamins 20 ranked
-7 pecan
-14 rumor
+11 fatal
+18 shadow
+5 briefing 12 roster
+19 spirit
+6 patent
+13 pitch
+20 chubby
+7 flame
+14 very
 m/44’/60’/0’/0/0
 : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
 m/84’/0’/0’/0/0
 : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
 
 Because we must tell slip39 to that we’re using the BIP-39 Mnemonic and Seed
 generation process to derived the wallet addresses from the Seed Entropy (not the SLIP39 standard). So, we add the -using-bip39 option:
 3
-( python3 -m slip39.recovery --bip39 --entropy \
+
+23
+
+( python3 -m slip39.recovery --bip39 --entropy \
 --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
 | python3 -m slip39 --secret - --no-card -v --using-bip39
 ) 2>&1 | tail -20
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39
+2022-10-05 17:01:26 slip39.layout
+2022-10-05 17:01:26 slip39.layout
 
 5th
 
 6th
 
-4 skin
-5 brave
-6 install
-7 campus
-1 steady
-2 upstairs
-3 decision
-4 snake
-5 drove
-6 stay
-7 union
-1 steady
-2 upstairs
-3 decision
-4 spider
-5 cowboy
-6 safari
-
-24
-
-11 ugly
-12 husky
-13 costume
-14 wisdom
-8 diet
-9 hawk
-10 system
-11 pregnant
-12 genuine
-13 pupal
-14 woman
-8 lizard
-9 aunt
-10 fused
-11 dance
-12 disease
-13 texture
-
-18 decrease
-19 olympic
-20 chest
-15 ladybug
-16 alien
-17 multiple
-18 platform
-19 hanger
-20 timely
-15 market
-16 plunge
-17 relate
-18 depart
-19 emperor
-20 boring
-
-2022-06-10 06:39:43 slip39
-2022-06-10 06:39:43 slip39.layout
-2022-06-10 06:39:43 slip39.layout
-
 ETH
 BTC
 
-7 unwrap
-14 rich
+4 skin
+11 quarter
+18 organize
+5 camera
+12 herd
+19 indicate
+6 flame
+13 game
+20 usher
+7 believe
+14 finance
+1 sprinkle
+8 company
+15 receiver
+2 cause
+9 wisdom
+16 paper
+3 decision 10 exotic
+17 formal
+4 snake
+11 response 18 demand
+5 decorate 12 ancient
+19 browser
+6 flash
+13 picture
+20 swimming
+7 ting
+14 subject
+1 sprinkle
+8 imply
+15 exhaust
+2 cause
+9 exact
+16 pregnant
+3 decision 10 analysis 17 decision
+4 spider
+11 quick
+18 ocean
+5 agree
+12 response 19 airline
+6 pupal
+13 snake
+20 emphasis
+7 knife
+14 lobe
 m/44’/60’/0’/0/0
-m/84’/0’/0’/0/0
-
 : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
+m/84’/0’/0’/0/0
 : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
 
 And, there we have it – we’ve recovered exactly the same Ethereum and Bitcoin wallets
 as would a native BIP-39 hardware wallet like a Ledger Nano.
 1. Using SLIP-39 App "Backup" Controls
 In the SLIP-39 App, the default Controls presented are to "Backup" a BIP-39
 recovery phrase.
@@ -2091,15 +2046,17 @@
 . . . vote" 24-word phrase) until you’re confident. Then, back up your real BIP-39
 recovery phrase.
 Once you’re convinced you can securely and reliably recover your BIP-39 phrase
 any time you need it, we recommend that you destroy your original BIP-39 recovery
 phrase backup(s). They are dangerous and unreliable, and only serve to make your
 Cryptocurrency accounts less secure!
 
-4
+24
+
+4
 
 Building & Installing
 
 The python-slip39 project is tested under both homebrew:
 $ brew install python-tk@3.9
 and using the official python.org/downloads installer.
 Either of these methods will get you a python3 executable running version 3.9+,
@@ -2108,18 +2065,15 @@
 4.1
 
 The slip39 Module
 
 To build the wheel and install slip39 manually:
 $ git clone git@github.com:pjkundert/python-slip39.git
 $ make -C python-slip39 install
-
-25
-
-To install from Pypi, including the optional requirements to run the PySimpleGUI/tkinter
+To install from Pypi, including the optional requirements to run the PySimpleGUI/tkinter
 GUI, support serial I/O, and to support creating encrypted BIP-38 and Ethereum JSON
 Paper Wallets:
 $ python3 -m pip install slip39[gui,paper,serial]
 
 4.2
 
 The slip39 GUI
@@ -2139,15 +2093,18 @@
 
 You can build the native macOS and win32 SLIP-39.app App.
 This requires the official python.org/downloads installer; the homebrew python-tk@3.9
 will not work for building the native app using either PyInstaller. (The py2app approach
 doesn’t work in either version of Python).
 $ git clone git@github.com:pjkundert/python-slip39.git
 $ make -C python-slip39 app
-4.2.2
+
+25
+
+4.2.2
 
 The Windows 10 SLIP-39 GUI
 
 Install Python from https://python.org/downloads, and the Microsoft C++ Build
 Tools via the Visual Studio Installer (required for installing some slip39 package dependencies).
 To run the GUI, just install slip39 package from Pypi using pip, including the gui
 and wallet options. Building the Windows SLIP-39 executable GUI application requires
@@ -2157,17 +2114,15 @@
 from git-scm.com. Once installed, run "Git bash", and
 $ ssh-keygen.exe -t ed25519
 to create an id_ed25519.pub SSH identity, and import it into your Git Settings SSH
 keys. Then,
 $ mkdir src
 $ cd src
 $ git clone git@github.com:pjkundert/python-slip39.git
-26
-
-1. Code Signing
+1. Code Signing
 The MMC (Microsoft Management Console) is used to store your code-signing certificates. See stackoverflow.com for how to enable its Certificate management.
 
 5
 
 Dependencies
 
 Internally, python-slip39 project uses Trezor’s python-shamir-mnemonic to encode the
@@ -2189,15 +2144,18 @@
 merit aluminum beard romp briefing email member flavor disaster exercise cinema subject perfect facility genius bike inclu
 Group 3 of 4 - 2 of 5 shares required:
 merit aluminum ceramic roster already cinema knit cultural agency intimate result ivory makeup lobe jerky theory garlic en
 merit aluminum ceramic scared beam findings expand broken smear cleanup enlarge coding says destroy agency emperor hairy d
 merit aluminum ceramic shadow cover smith idle vintage mixture source dish squeeze stay wireless likely privacy impulse to
 merit aluminum ceramic sister duke relate elite ruler focus leader skin machine mild envelope wrote amazing justice mornin
 merit aluminum ceramic smug buyer taxi amazing marathon treat clinic rainbow destroy unusual keyboard thumb story literary
-Group 4 of 4 - 3 of 6 shares required:
+
+26
+
+Group 4 of 4 - 3 of 6 shares required:
 merit aluminum decision round bishop wrote belong anatomy spew hour index fishing lecture disease cage thank fantasy extra
 merit aluminum decision scatter carpet spine ruin location forward priest cage security careful emerald screw adult jerky
 merit aluminum decision shaft arcade infant argue elevator imply obesity oral venture afraid slice raisin born nervous uni
 merit aluminum decision skin already fused tactics skunk work floral very gesture organize puny hunting voice python trial
 merit aluminum decision snake cage premium aide wealthy viral chemical pharmacy smoking inform work cubic ancestor clay ge
 merit aluminum decision spider boundary lunar staff inside junior tendency sharp editor trouble legal visual tricycle auct
```

### Comparing `slip39-9.0.4/README.txt` & `slip39-9.1.2/README.txt`

 * *Files 5% similar despite different names*

```diff
@@ -267,23 +267,24 @@
 
   ┌────
   │     slip39 -c ETH -c BTC -c DOGE -c LTC --secret ffffffffffffffffffffffffffffffff \
   │         --no-card --wallet password --wallet-hint 'bad:pass...' 2>&1
   └────
 
   ┌────
-  │ 2022-06-10 06:40:11 slip39           It is recommended to not use '-s|--secret <hex>'; specify '-' to read from input
-  │ 2022-06-10 06:40:11 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
-  │ 2022-06-10 06:40:11 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
-  │ 2022-06-10 06:40:11 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
-  │ 2022-06-10 06:40:11 slip39.layout    DOGE   m/44'/3'/0'/0/0     : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
-  │ 2022-06-10 06:40:11 slip39.layout    LTC    m/84'/2'/0'/0/0     : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
-  │ 2022-06-10 06:40:15 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-06-10+06.40.12-ETH-0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1.pdf
+  │ 2022-10-05 16:59:07 slip39           It is recommended to not use '-s|--secret <hex>'; specify '-' to read from input
+  │ 2022-10-05 16:59:07 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
+  │ 2022-10-05 16:59:07 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
+  │ 2022-10-05 16:59:07 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
+  │ 2022-10-05 16:59:07 slip39.layout    DOGE   m/44'/3'/0'/0/0     : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
+  │ 2022-10-05 16:59:07 slip39.layout    LTC    m/84'/2'/0'/0/0     : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
+  │ 2022-10-05 16:59:10 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-10-05+16.59.08-ETH-0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1.pdf
   └────
 
+
   And what they look like:
 
   <./images/slip39-wallets.png>
 
   To recover your real SLIP-39 Seed Entropy and print wallets, use the
   SLIP-39 App's "Recover" Controls, or to do so on the command-line, use
   `slip39-recover':
@@ -292,39 +293,40 @@
   │     slip39-recovery -v \
   │ 	--mnemonic "material leaf acrobat romp charity capital omit skunk change firm eclipse crush fancy best tracks flip grownup plastic chew peanut" \
   │         --mnemonic "material leaf beard romp disaster duke flame uncover group slice guest blue gums duckling total suitable trust guitar payment platform" \
   │ 	2>&1
   └────
 
   ┌────
-  │ 2022-06-10 06:40:15 slip39.recovery  Recovered 128-bit SLIP-39 Seed Entropy with 2 (all) of 2 supplied mnemonics; Seed decoded from SLIP-39 Mnemonics w/ passphrase
-  │ 2022-06-10 06:40:15 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
+  │ 2022-10-05 16:59:11 slip39.recovery  Recovered 128-bit SLIP-39 Seed Entropy with 2 (all) of 2 supplied mnemonics; Seed decoded from SLIP-39 Mnemonics w/ passphrase
+  │ 2022-10-05 16:59:11 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
   │ ffffffffffffffffffffffffffffffff
   └────
 
+
   You can run this as a command-line pipeline.  Here, we use some
   SLIP-39 Mnemonics that encode the `ffff...' Seed Entropy; note that
   the wallets match those output above:
 
   ┌────
   │     slip39-recovery \
   │ 	--mnemonic "material leaf acrobat romp charity capital omit skunk change firm eclipse crush fancy best tracks flip grownup plastic chew peanut" \
   │         --mnemonic "material leaf beard romp disaster duke flame uncover group slice guest blue gums duckling total suitable trust guitar payment platform" \
   │     | slip39 -c ETH -c BTC -c DOGE -c LTC --secret - \
   │         --no-card --wallet password --wallet-hint 'bad:pass...' \
   │ 	2>&1
   └────
 
   ┌────
-  │ 2022-06-10 06:40:16 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
-  │ 2022-06-10 06:40:16 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
-  │ 2022-06-10 06:40:16 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
-  │ 2022-06-10 06:40:16 slip39.layout    DOGE   m/44'/3'/0'/0/0     : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
-  │ 2022-06-10 06:40:16 slip39.layout    LTC    m/84'/2'/0'/0/0     : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
-  │ 2022-06-10 06:40:20 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-06-10+06.40.17-ETH-0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1.pdf
+  │ 2022-10-05 16:59:11 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
+  │ 2022-10-05 16:59:11 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
+  │ 2022-10-05 16:59:11 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
+  │ 2022-10-05 16:59:11 slip39.layout    DOGE   m/44'/3'/0'/0/0     : DN8PNN3dipSJpLmyxtGe4EJH38EhqF8Sfy
+  │ 2022-10-05 16:59:11 slip39.layout    LTC    m/84'/2'/0'/0/0     : ltc1qe5m2mst9kjcqtfpapaanaty40qe8xtusmq4ake
+  │ 2022-10-05 16:59:14 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-10-05+16.59.12-ETH-0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1.pdf
   └────
 
 
 2.1.2 Supported Cryptocurrencies
 ╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌
 
   While the SLIP-39 Seed is not cryptocurrency-specific (any wallet for
@@ -444,15 +446,15 @@
   │     : 
   │     : Create and output SLIP-39 encoded Seeds and Paper Wallets to a PDF file.
   │     : 
   │     : positional arguments:
   │     :   names                 Account names to produce; if --secret Entropy is
   │     :                         supplied, only one is allowed.
   │     : 
-  │     : optional arguments:
+  │     : options:
   │     :   -h, --help            show this help message and exit
   │     :   -v, --verbose         Display logging information.
   │     :   -q, --quiet           Reduce logging output.
   │     :   -o OUTPUT, --output OUTPUT
   │     :                         Output PDF to file or '-' (stdout); formatting w/
   │     :                         name, date, time, crypto, path, address allowed
   │     :   -t THRESHOLD, --threshold THRESHOLD
@@ -531,19 +533,19 @@
   files):
 
   ┌────
   │   slip39 --secret 383597fd63547e7c9525575decd413f7 --wallet password --wallet-hint bad:pass... 2>&1
   └────
 
   ┌────
-  │ 2022-06-10 06:40:21 slip39           It is recommended to not use '-s|--secret <hex>'; specify '-' to read from input
-  │ 2022-06-10 06:40:21 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
-  │ 2022-06-10 06:40:21 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xb44A2011A99596671d5952CdC22816089f142FB3
-  │ 2022-06-10 06:40:21 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qcupw7k8enymvvsa7w35j5hq4ergtvus3zk8a8s
-  │ 2022-06-10 06:40:23 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-06-10+06.40.22-ETH-0xb44A2011A99596671d5952CdC22816089f142FB3.pdf
+  │ 2022-10-05 16:59:16 slip39           It is recommended to not use '-s|--secret <hex>'; specify '-' to read from input
+  │ 2022-10-05 16:59:16 slip39           It is recommended to not use '-w|--wallet <password>'; specify '-' to read from input
+  │ 2022-10-05 16:59:16 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xb44A2011A99596671d5952CdC22816089f142FB3
+  │ 2022-10-05 16:59:16 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qcupw7k8enymvvsa7w35j5hq4ergtvus3zk8a8s
+  │ 2022-10-05 16:59:18 slip39.layout    Writing SLIP39-encoded wallet for 'SLIP39' to: SLIP39-2022-10-05+16.59.17-ETH-0xb44A2011A99596671d5952CdC22816089f142FB3.pdf
   └────
 
 
 2.4.1 `slip39.recovery' Synopsis
 ╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌
 
   ┌────
@@ -552,15 +554,15 @@
 
   ┌────
   │     : usage: slip39-recovery [-h] [-v] [-q] [-m MNEMONIC] [-e] [-b] [-u]
   │     :                        [-p PASSPHRASE]
   │     : 
   │     : Recover and output secret Seed from SLIP-39 or BIP-39 Mnemonics
   │     : 
-  │     : optional arguments:
+  │     : options:
   │     :   -h, --help            show this help message and exit
   │     :   -v, --verbose         Display logging information.
   │     :   -q, --quiet           Reduce logging output.
   │     :   -m MNEMONIC, --mnemonic MNEMONIC
   │     :                         Supply another SLIP-39 (or a BIP-39) mnemonic phrase
   │     :   -e, --entropy         Return the BIP-39 Mnemonic Seed Entropy instead of the
   │     :                         generated Seed (default: False)
@@ -614,20 +616,21 @@
   ┌────
   │    ( python3 -m slip39 --text --no-card \
   │        | ( sort -r  ; echo "...later..." 1>&2 ) \
   │        | python3 -m slip39.recovery \
   │        | python3 -m slip39 --secret - --no-card \
   │     ) 2>&1
   └────
+
   ┌────
-  │ 2022-06-10 06:40:25 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xAba3B0d3142e9856D866578B717D6a3a3DFCbd20
-  │ 2022-06-10 06:40:25 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q8wmn4g6qcx8pjz9357x5ct8uu06ye0vje08fqg
+  │ 2022-10-05 16:59:19 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xbEc417E880c805908ae43A3bE1915549E2a58C0d
+  │ 2022-10-05 16:59:19 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qt7chyzr557ytzvch8lknujkl8puvjg783fkt4a
   │ ...later...
-  │ 2022-06-10 06:40:25 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xAba3B0d3142e9856D866578B717D6a3a3DFCbd20
-  │ 2022-06-10 06:40:25 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q8wmn4g6qcx8pjz9357x5ct8uu06ye0vje08fqg
+  │ 2022-10-05 16:59:19 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xbEc417E880c805908ae43A3bE1915549E2a58C0d
+  │ 2022-10-05 16:59:19 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qt7chyzr557ytzvch8lknujkl8puvjg783fkt4a
   └────
 
 
 2.5 Generation of Addresses
 ───────────────────────────
 
   For systems that require a stream of groups of wallet Addresses
@@ -648,15 +651,15 @@
   │     :                         [-c CRYPTOCURRENCY] [--path PATH] [-d DEVICE]
   │     :                         [--baudrate BAUDRATE] [-e ENCRYPT] [--decrypt ENCRYPT]
   │     :                         [--enumerated] [--no-enumerate] [--receive]
   │     :                         [--corrupt CORRUPT]
   │     : 
   │     : Generate public wallet address(es) from a secret seed
   │     : 
-  │     : optional arguments:
+  │     : options:
   │     :   -h, --help            show this help message and exit
   │     :   -v, --verbose         Display logging information.
   │     :   -q, --quiet           Reduce logging output.
   │     :   -s SECRET, --secret SECRET
   │     :                         Use the supplied 128-, 256- or 512-bit hex value as
   │     :                         the secret seed; '-' (default) reads it from stdin
   │     :                         (eg. output from slip39.recover)
@@ -718,14 +721,15 @@
   ┌────
   │ 0: [["ETH", "m/44'/60'/0'/0/0", "0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1"], ["BTC", "m/84'/0'/0'/0/0", "bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl"]]
   │ 1: [["ETH", "m/44'/60'/0'/0/1", "0x8D342083549C635C0494d3c77567860ee7456963"], ["BTC", "m/84'/0'/0'/0/1", "bc1qnec684yvuhfrmy3q856gydllsc54p2tx9w955c"]]
   │ 2: [["ETH", "m/44'/60'/0'/0/2", "0x52787E24965E1aBd691df77827A3CfA90f0166AA"], ["BTC", "m/84'/0'/0'/0/2", "bc1q2snj0zcg23dvjpw7m9lxtu0ap0hfl5tlddq07j"]]
   │ 3: [["ETH", "m/44'/60'/0'/0/3", "0xc2442382Ae70c77d6B6840EC6637dB2422E1D44e"], ["BTC", "m/84'/0'/0'/0/3", "bc1qxwekjd46aa5n0s3dtsynvtsjwsne7c5f5w5dsd"]]
   └────
 
+
   To produce accounts from a BIP-39 or SLIP-39 seed, recover it using
   slip39-recovery.
 
   Here's an example of recovering a test BIP-39 seed; note that it
   yields the well-known ETH `0xfc20...1B5E' and BTC `bc1qk0...gnn2'
   accounts associated with this test Mnemonic:
 
@@ -737,33 +741,35 @@
   ┌────
   │ 0: [["ETH", "m/44'/60'/0'/0/0", "0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E"], ["BTC", "m/84'/0'/0'/0/0", "bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2"]]
   │ 1: [["ETH", "m/44'/60'/0'/0/1", "0xd1a7451beB6FE0326b4B78e3909310880B781d66"], ["BTC", "m/84'/0'/0'/0/1", "bc1qkd33yck74lg0kaq4tdcmu3hk4yruhjayxpe9ug"]]
   │ 2: [["ETH", "m/44'/60'/0'/0/2", "0x578270B5E5B53336baC354756b763b309eCA90Ef"], ["BTC", "m/84'/0'/0'/0/2", "bc1qvr7e5aytd0hpmtaz2d443k364hprvqpm3lxr8w"]]
   │ 3: [["ETH", "m/44'/60'/0'/0/3", "0x909f59835A5a120EafE1c60742485b7ff0e305da"], ["BTC", "m/84'/0'/0'/0/3", "bc1q6t9vhestkcfgw4nutnm8y2z49n30uhc0kyjl0d"]]
   └────
 
+
   We can encrypt the output, to secure the sequence (and due to
   integrated MACs, ensures no errors occur over an insecure channel like
   a serial cable):
 
   ┌────
   │     ( slip39-recovery --bip39 --mnemonic 'zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong' \
   │         | slip39-generator --secret - --path '../-3' --encrypt 'password' ) 2>&1
   └────
 
   ┌────
   │ 
   │ 
-  │ nonce: 2a7714516d6e91616ce02219dd70ab6575dc5e81bd1e520e4dce061d
-  │     0: 9b335ce5720ab37790089cad98c8253d331ce2f4563dc00e5e5c5c7d7f0e56022ce0ed6ad9ba38ed0e01a520036d87e3fc822b278129820a8fde8fe6152987e1bfd785e188189c6dec88de39eda24364608ddfee663fedd34b5be71f173b3c56d352f69138ec78b042356916c8373783374fbddd75d27bb2236aa27cffb024b64f01c7a2ff2309d7c1dcfc76bc42373fc08b7a8d2f559bfffb4314980da5616dc4f9f9e4c6
-  │     1: d0873123353726537bcf97b57efea591a3e52cd9511c5b8117e68d89b3e76f03b8c94033ccabe8ffd4d2dc611820bc0e893a94b3ba0c95fe66f539875b92d399071167052ebda7c7ab47ecef7faa9fbc523987964fc1d0e211cff5411ad04bf7e0b1feab77eaf71f4efaffe7e639f2e72ba88711864cdf149b273d7301c6308098d96760b638daa98ff2a5a3103068b828bbe022de1c53fcd47d36ff37c866bc27bce08332
-  │     2: 368a0c9c6ecffba3aa2e8afefb0f072814f5f8fede96dbb6f97f36eed602dd3c4820cab527c45c91189b995ad6ace3aa5fcff1d5529f03aa008657c91041c13807d6fcbfe5c8e98c0f42599f33d416ff6c3c64cfd4aef1accb5521f98e80f86912f4d0dd73763c667746ff88e3ccd9a014efb94f075852374fc9d7ae17c477bdd72334e04303ffe55e30ec21961b7cf4e5f0d4fb1c49dfc8637a25912860fdd70790b5b710
-  │     3: 6af0cd1c6938e1b21f6dbdd5ef38c60502ac2389014227476257efa9af3ccd49c31cf4e93de30083d9b3456da24cdac495d2fddcec6bb9b55c884549aa4b337b8c5d1ee528e916168e5b8ed8af112ac48eb443d08344408ec3337c4d71e34ad01961e2888ae6a283fec3aa95daf436fff2dda83a47ddb224559ac0b830ea6da87c494118516067f65d4d01276975e7e3083d2a035ffbd2a5cc4903a9f249313821292100b4
+  │ nonce: 6a24e975d704af3333c8f0d57a1dd4a9036d21cff82863daae5b36ff
+  │     0: e3992c21f7acadcff23bffad8ac0cd6cfbce94c1c50202413f2a59a27fa299a189d6b3385dd377be4fa8bf7ac0af20f1bde6f35d47b74cc05954e5f41c530f487df1f0f6b42362a5d72933a1c19018df9151f2f3c7b4acb4b52b7d8024ea76cbcd6c102c268ff3a1bca6167988fa540ca48d98456b77fff04a6a84174e02f76c339c192ec11cb2960829d14898a00977def64686c1dd2ad6ca63aed9342cb4ea89052ca16e
+  │     1: 6fda42f388ad2c6b1a263c7414897f1b7a88c793db4ecbb190ddb6df2574305c85cdc5b2ff0ee7542820e5af8dec35a26fd588ed60aa340d202e3c3a0520e2e5607a9e57152c39e8ab8447b78b38c003e94efe0a8352844d65e91efe382386453080532e40ae724e83f53712291afc3d08bea3e08c6df568feff8f4693ccfc5030d4a9c61ce2537353f216fd8fb7975fa4af96013ea97ad2459f7ac85e19d5066a6f3bbbc5
+  │     2: 78d2d59863d97c826a494e28132d227b9112bf133341757f0ca37707d18792fb13615678b2077af68725c318dec856c4968cc73d2bd2b17e7fd378e5c906186230ed99aba8e93b165ba1d78d04283db291c74796282b6323d0ec45eb672e9c665efac574356097998471dd613bc90dad5c9f615dc48d4e18348cbd4e08d542fd0a9a763227e01b0f4c5bef8a35bd79f49e50d67798e44e09c18eac4b23361f0d2ece953b79
+  │     3: 4ad67ce28d53503459c858d1471b3ede4b625c9b2c79cb44126a085966aee8839d6e7b7f70fc471b4e56643ebd525a316bdc62a37b1c36004ee1c4ee830989c22b48689ce6f8c497025f1f3725f5cf48767dc479fc3e56e531f0010a98a5fd1432fc3aa5d53a2e6e2a9e075f377611c112ea4e98c5d03775c23cb9570809289436e9d89962671437485f87d954d08c7f00a03437224d16a5d1387bbded0c27e1bbfdee1566
   └────
 
+
   On the receiving computer, we can decrypt and recover the stream of
   accounts from the wallet seed; any rows with errors are ignored:
   ┌────
   │     ( slip39-recovery --bip39 --mnemonic 'zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong' \
   │         | slip39-generator --secret - --path '../-3' --encrypt 'password' \
   │         | slip39-generator --receive --decrypt 'password' ) 2>&1
   └────
@@ -812,15 +818,19 @@
    accounts         Resultant list of groups of accounts               
    using_bip39      Seed produced from entropy using BIP-39 generation 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   This is immediately usable to pass to `slip39.output'.
 
   ┌────
   │     import codecs
+  │     import logging
   │     import random
+  │     from tabulate import tabulate
+  │ 
+  │     logging.basicConfig( level=logging.WARNING, format="%(message)s" )
   │ 
   │     #
   │     # NOTE:
   │     #
   │     # We turn off randomness here during SLIP-39 generation to get deterministic phrases;
   │     # during normal operation, secure entropy is used during mnemonic generation, yielding
   │     # random phrases, even when the same seed is used multiple times.
@@ -832,28 +842,27 @@
   │ 
   │     cryptopaths         = [("ETH","m/44'/60'/0'/0/-2"), ("BTC","m/44'/0'/0'/0/-2")]
   │     master_secret       = b'\xFF' * 16
   │     passphrase          = b""
   │     create_details      = slip39.create(
   │         "Test", 2, { "Mine": (1,1), "Fam": (2,3) },
   │         master_secret=master_secret, passphrase=passphrase, cryptopaths=cryptopaths )
-  │     [
+  │ 
+  │     print( tabulate( [
   │         [
   │             f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" if l_n == 0 else ""
   │         ] + words
   │         for g_name,(g_of,g_mnems) in create_details.groups.items()
   │         for g_n,mnem in enumerate( g_mnems )
   │         for l_n,(line,words) in enumerate(slip39.organize_mnemonic(
   │                 mnem, label=f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" ))
-  │     ]
+  │       ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0              1           2            3           
-  ─────────────────────────────────────────────────────
    Mine(1/1) #1:  1 academic  8 safari     15 standard 
                   2 acid      9 drug       16 angry    
                   3 acrobat   10 browser   17 similar  
                   4 easy      11 trash     18 aspect   
                   5 change    12 fridge    19 smug     
                   6 injury    13 busy      20 violence 
                   7 painting  14 finger                
@@ -878,24 +887,22 @@
                   5 alarm     12 anxiety   19 both     
                   6 health    13 august    20 award    
                   7 discuss   14 sunlight              
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   Add the resultant HD Wallet addresses:
 
   ┌────
-  │     [
+  │     print( tabulate( [
   │         [ account.path, account.address ]
   │         for group in create_details.accounts
   │         for account in group
-  │     ]
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0                                                          1 
-  ──────────────────────────────────────────────────────────────
    m/44'/60'/0'/0/0  0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1 
    m/44'/0'/0'/0/0   bc1qm5ua96hx30snwrwsfnv97q96h53l86ded7wmjl 
    m/44'/60'/0'/0/1  0x8D342083549C635C0494d3c77567860ee7456963 
    m/44'/0'/0'/0/1   bc1qwz6v9z49z8mk5ughj7r78hjsp45jsxgzh29lnh 
    m/44'/60'/0'/0/2  0x52787E24965E1aBd691df77827A3CfA90f0166AA 
    m/44'/0'/0'/0/2   bc1q690m430qu29auyefarwfrvfumncunvyw6v53n9 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
@@ -921,29 +928,27 @@
   for the crypto accounts, on the paper_format provided.  Returns the
   paper (orientation,format) used, the FPDF, and passes through the
   supplied cryptocurrency accounts derived.
 
   ┌────
   │     (paper_format,orientation),pdf,accounts = slip39.produce_pdf( *create_details )
   │     pdf_binary = pdf.output()
-  │     [
+  │     print( tabulate( [
   │         [ "Orientation:",	orientation ],
   │         [ "Paper:",		paper_format ],
   │         [ "PDF Pages:",		pdf.pages_count ],
   │         [ "PDF Size:",		len( pdf_binary )],
-  │     ]
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━
-   0                     1 
-  ─────────────────────────
    Orientation:  landscape 
    Paper:           Letter 
    PDF Pages:            1 
-   PDF Size:         13028 
+   PDF Size:         13137 
   ━━━━━━━━━━━━━━━━━━━━━━━━━
 
 
 2.6.3 `slip39.write_pdfs'
 ╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
@@ -1017,23 +1022,21 @@
   │     # But, recovering w/ correct passphrase yields our original Seed Entropy
   │     recoveryvalid       = slip39.recover(
   │         create_details.groups['Mine'][1][:] + create_details.groups['Fam'][1][:2],
   │         passphrase=passphrase
   │     )
   │     recoveryvalid_hex   = codecs.encode( recoveryvalid, 'hex_codec' ).decode( 'ascii' )
   │ 
-  │     [
+  │     print( tabulate( [
   │       [ f"{len(recoverydecoy)*8}-bit secret (decoy):", f"{recoverydecoy_hex}" ],
   │       [ f"{len(recoveryvalid)*8}-bit secret recovered:", f"{recoveryvalid_hex}" ]
-  │     ]
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0                          1                                
-  ─────────────────────────────────────────────────────────────
    128-bit secret (decoy):    2e522cea2b566840495c220cf79c756e 
    128-bit secret recovered:  ffffffffffffffffffffffffffffffff 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 
 
 2.6.5 `slip39.recover_bip39'
 ╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌
@@ -1120,63 +1123,58 @@
   │ 
   │     recovered		= slip39.recover_bip39( entropy_mnemonic, as_entropy=True )
   │     recovered_hex	= codecs.encode( recovered, 'hex_codec' ).decode( 'ascii' )
   │ 
   │     recovered_seed	= slip39.recover_bip39( entropy_mnemonic, passphrase=passphrase )
   │     recovered_seed_hex	= codecs.encode( recovered_seed, 'hex_codec' ).decode( 'ascii' )
   │     
-  │     [
-  │      [ "Original Entropy", entropy_hex ],
-  │      [ "BIP-39 Mnemonic", entropy_mnemonic ],
-  │      [ "Recovered Entropy", recovered_hex ],
-  │      [ "Recovered Seed", f"{recovered_seed_hex:.50}..." ],
-  │     ]
+  │     print( tabulate( [
+  │         [ "Original Entropy", entropy_hex ],
+  │         [ "BIP-39 Mnemonic", entropy_mnemonic ],
+  │         [ "Recovered Entropy", recovered_hex ],
+  │         [ "Recovered Seed", f"{recovered_seed_hex:.50}..." ],
+  │     ], tablefmt='orgtbl'))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0                  1                                                   
-  ────────────────────────────────────────────────────────────────────────
    Original Entropy   ffffffffffffffffffffffffffffffff                    
    BIP-39 Mnemonic    zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong   
    Recovered Entropy  ffffffffffffffffffffffffffffffff                    
    Recovered Seed     b6a6d8921942dd9806607ebc2750416b289adea669198769f2… 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   Each word is one of a corpus of 2048 words; therefore, each word
-      encodes 11 bits (2048 `= 2**11) of entropy.  So, we provided 128
-      bits, but 12*11 =' 132.  So where does the extra 4 bits of data
-      come from?
+  encodes 11 bits (2048 = 2**11) of entropy.  So, we provided 128 bits,
+  but 12*11 = 132.  So where does the extra 4 bits of data come from?
 
   It comes from the first few bits of a SHA256 hash of the entropy,
   which is added to the end of the supplied 128 bits, to reach the
-  required 132 bits: 132 / 11 == 12 words.
+  required 132 bits: 132 / 11 = 12 words.
 
   This last 4 bits (up to 8 bits, for a 256-bit 24-word BIP-39) is
   checked, when validating the BIP-39 mnemonic.  Therefore, making up a
   random BIP-39 mnemonic will succeed only 1 / 16 times on average, due
-  to an incorrect checksum 4-bit (16 == 2**4) .  Lets check:
+  to an incorrect checksum 4-bit (16 = 2**4) .  Lets check:
 
   ┌────
   │     def random_words( n, count=100 ):
   │         for _ in range( count ):
   │             yield ' '.join( random.choice( bip39_english.wordlist ) for _ in range( n ))
   │ 
   │     successes           = sum(
   │         bip39_english.check( m )
   │         for i,m in enumerate( random_words( 12, 10000 ))) / 100
   │ 
-  │     [
+  │     print( tabulate( [
   │       [ "Valid random 12-word mnemonics:", f"{successes}%" ],
   │       [ "Or, about: ", f"1 / {100/successes:.3}" ],
-  │     ]
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0                                       1 
-  ───────────────────────────────────────────
-   Valid random 12-word mnemonics:     6.19% 
+   Valid random 12-word mnemonics:     6.17% 
    Or, about:                       1 / 16.2 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   Sure enough, about 1/16 random 12-word phrases are valid BIP-39
   mnemonics.  OK, we've got the contents of the BIP-39 phrase dialed in.
   How is it used to generate accounts?
 
 
@@ -1189,22 +1187,20 @@
   Entropy bytes/) of the 12-word mnemonic is then used (with a salt of
   "mnemonic" plus an optional passphrase, "" by default), to obtain the
   512-bit seed:
 
   ┌────
   │     seed                = bip39_english.to_seed( entropy_mnemonic )
   │     seed_hex            = codecs.encode( seed, 'hex_codec' ).decode( 'ascii' )
-  │     [
+  │     print( tabulate( [
   │      [ f"{len(seed)*8}-bit seed:", f"{seed_hex:.50}..." ]
-  │     ]
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-               0                                                    1 
-  ────────────────────────────────────────────────────────────────────
    512-bit seed:  b6a6d8921942dd9806607ebc2750416b289adea669198769f2… 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 
 
 3.1.3 BIP-39 Seed to Address
 ╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌
 
@@ -1218,27 +1214,25 @@
   32-byte (256-bit) Ethereum account private key is produced.  We then
   use this private key to compute the rest of the Ethereum account
   details, such as its public address.
 
   ┌────
   │     path                = "m/44'/60'/0'/0/0"
   │     bip39_eth_hd        = slip39.account( seed, 'ETH', path )
-  │     [
+  │     print( tabulate( [
   │      [ f"{len(bip39_eth_hd.key)*4}-bit derived key path:", f"{path}" ],
   │      [ "Produces private key: ", f"{bip39_eth_hd.key}" ],
   │      [ "Yields Ethereum address:", f"{bip39_eth_hd.address}" ],
-  │     ]
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0                                                                                         1 
-  ─────────────────────────────────────────────────────────────────────────────────────────────
-   256-bit derived key path:                                                  m/44'/60'/0'/0/0 
+   256-bit derived key path:  m/44'/60'/0'/0/0                                                 
    Produces private key:      7af65ba4dd53f23495dcb04995e96f47c243217fc279f10795871b725cd009ae 
-   Yields Ethereum address:                         0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E 
+   Yields Ethereum address:   0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E                       
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   Thus, we see that while the 12-word BIP-39 mnemonic careful preserves
   the original 128-bit entropy, this data is not directly used to derive
   the wallet private key and address.  Also, since an irreversible hash
   is used to derive the Seed from the Mnemonic, we can't reverse the
   process on the seed to arrive back at the BIP-39 mnemonic phrase.
 
@@ -1250,26 +1244,24 @@
   bytes in a single 12-word mnemonic phrase, SLIP-39 preserves the
   original 128- or 256-bit Seed Entropy in a /set/ of 20- or 33-word
   Mnemonic phrases.
 
   ┌────
   │     name,thrs,grps,acct,ub39 = slip39.create(
   │         "Test", 2, { "Mine": (1,1), "Fam": (2,3) }, entropy )
-  │     [
-  │      [ f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" if l_n == 0 else "" ] + words
-  │      for g_name,(g_of,g_mnems) in grps.items()
-  │      for g_n,mnem in enumerate( g_mnems )
-  │      for l_n,(line,words) in enumerate(slip39.organize_mnemonic(
-  │              mnem, rows=7, cols=3, label=f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" ))
-  │     ]
+  │     print( tabulate( [
+  │         [ f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" if l_n == 0 else "" ] + words
+  │         for g_name,(g_of,g_mnems) in grps.items()
+  │         for g_n,mnem in enumerate( g_mnems )
+  │         for l_n,(line,words) in enumerate(slip39.organize_mnemonic(
+  │                 mnem, rows=7, cols=3, label=f"{g_name}({g_of}/{len(g_mnems)}) #{g_n+1}:" ))
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0              1           2            3           
-  ─────────────────────────────────────────────────────
    Mine(1/1) #1:  1 academic  8 safari     15 standard 
                   2 acid      9 drug       16 angry    
                   3 acrobat   10 browser   17 similar  
                   4 easy      11 trash     18 aspect   
                   5 change    12 fridge    19 smug     
                   6 injury    13 busy      20 violence 
                   7 painting  14 finger                
@@ -1299,27 +1291,24 @@
   generation process, we would get a *different* set of words each time
   for the fixed "entropy" `0xFFFF..FF' used in this example (if we
   hadn't manually disabled entropy for `shamir_mnemonic', above), but we
   will *always* derive the same Ethereum account `0x824b..19a1' at the
   specified HD Wallet derivation path.
 
   ┌────
-  │     [
-  │      [ "Crypto", "HD Wallet Path:", "Ethereum Address:" ]
-  │     ] + [
-  │      [ account.crypto, account.path, account.address ]
-  │      for group in create_details.accounts
-  │      for account in group
-  │     ]
+  │     print( tabulate( [
+  │         [ account.crypto, account.path, account.address ]
+  │         for group in create_details.accounts
+  │         for account in group
+  │     ], tablefmt='orgtbl', headers=[ "Crypto", "HD Wallet Path:", "Ethereum Address:" ] ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0       1                                                          2 
+   Crypto  HD Wallet Path:   Ethereum Address:                          
   ──────────────────────────────────────────────────────────────────────
-   Crypto  HD Wallet Path:                            Ethereum Address: 
    ETH     m/44'/60'/0'/0/0  0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1 
    BTC     m/44'/0'/0'/0/0   bc1qm5ua96hx30snwrwsfnv97q96h53l86ded7wmjl 
    ETH     m/44'/60'/0'/0/1  0x8D342083549C635C0494d3c77567860ee7456963 
    BTC     m/44'/0'/0'/0/1   bc1qwz6v9z49z8mk5ughj7r78hjsp45jsxgzh29lnh 
    ETH     m/44'/60'/0'/0/2  0x52787E24965E1aBd691df77827A3CfA90f0166AA 
    BTC     m/44'/0'/0'/0/2   bc1q690m430qu29auyefarwfrvfumncunvyw6v53n9 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
@@ -1334,48 +1323,44 @@
   Mine, and 2 from the Fam group:
 
   ┌────
   │     _,mnem_mine         = grps['Mine']
   │     _,mnem_fam          = grps['Fam']
   │     recseed             = slip39.recover( mnem_mine + mnem_fam[:2] )
   │     recseed_hex         = codecs.encode( recseed, 'hex_codec' ).decode( 'ascii' )
-  │     [
-  │      [ f"{len(recseed)*8}-bit Seed:", f"{recseed_hex}" ]
-  │     ]
+  │     print( tabulate( [
+  │         [ f"{len(recseed)*8}-bit Seed:", f"{recseed_hex}" ]
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-               0                                 1 
-  ─────────────────────────────────────────────────
    128-bit Seed:  ffffffffffffffffffffffffffffffff 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 
 
 3.1.6 SLIP-39 Seed to Address
 ╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌
 
   And we'll use the same style of code as for the BIP-39 example above,
   to derive the Ethereum address *directly* from this recovered 128-bit
   seed:
 
   ┌────
   │     slip39_eth_hd       = slip39.account( recseed, 'ETH', path )
-  │     [
-  │      [ f"{len(slip39_eth_hd.key)*4}-bit derived key path:", f"{path}" ],
-  │      [ "Produces private key: ", f"{slip39_eth_hd.key}" ],
-  │      [ "Yields Ethereum address:", f"{slip39_eth_hd.address}" ],
-  │     ]
+  │     print( tabulate( [
+  │         [ f"{len(slip39_eth_hd.key)*4}-bit derived key path:", f"{path}" ],
+  │         [ "Produces private key: ", f"{slip39_eth_hd.key}" ],
+  │         [ "Yields Ethereum address:", f"{slip39_eth_hd.address}" ],
+  │     ], tablefmt='orgtbl' ))
   └────
 
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-   0                                                                                         1 
-  ─────────────────────────────────────────────────────────────────────────────────────────────
-   256-bit derived key path:                                                  m/44'/60'/0'/0/0 
+   256-bit derived key path:  m/44'/60'/0'/0/0                                                 
    Produces private key:      6a2ec39aab88ec0937b79c8af6aaf2fd3c909e9a56c3ddd32ab5354a06a21a2b 
-   Yields Ethereum address:                         0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1 
+   Yields Ethereum address:   0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1                       
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   And we see that we obtain the same Ethereum address `0x824b..1a2b' as
   we originally got from `slip39.create' above.  However, this is *not
   the same* Ethereum wallet address obtained from BIP-39 with exactly
   the same `0xFFFF...FF' Seed Entropy, which was `0xfc20..1B5E'!
 
   This is due to the fact that BIP-39 does not use the recovered Seed
@@ -1438,49 +1423,49 @@
 
   ┌────
   │     ( python3 -m slip39.recovery --bip39 -v \
   │         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" 
   │     ) 2>&1
   └────
   ┌────
-  │ 2022-06-10 06:40:35 slip39.recovery  Recovered 512-bit BIP-39 secret from english mnemonic
-  │ 2022-06-10 06:40:35 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
+  │ 2022-10-05 16:59:34 slip39.recovery  Recovered 512-bit BIP-39 secret from english mnemonic
+  │ 2022-10-05 16:59:34 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
   │ b6a6d8921942dd9806607ebc2750416b289adea669198769f2e15ed926c3aa92bf88ece232317b4ea463e84b0fcd3b53577812ee449ccc448eb45e6f544e25b6
   └────
 
   Then we can generate a 59-word SLIP-39 mnemonic set from the 512-bit
   secret:
 
   ┌────
   │     ( python3 -m slip39.recovery --bip39 \
   │         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
   │       | python3 -m slip39 --secret - --no-card -v
   │     ) 2>&1 | tail -20
   └────
   ┌────
-  │     2022-06-10 06:40:35 slip39                7 dynamic   19 fatal     31 spider    43 yelp      55 ancient   
-  │     2022-06-10 06:40:35 slip39                8 reunion   20 family    32 eraser    44 review    56 expect    
-  │     2022-06-10 06:40:35 slip39                9 garlic    21 guest     33 overall   45 intimate  57 dish      
-  │     2022-06-10 06:40:35 slip39               10 smear     22 transfer  34 security  46 estate    58 marvel    
-  │     2022-06-10 06:40:35 slip39               11 spray     23 perfect   35 froth     47 modify    59 ceramic   
-  │     2022-06-10 06:40:35 slip39               12 ladle     24 nail      36 lyrics    48 idle      
-  │     2022-06-10 06:40:35 slip39           6th  1 sister    13 universe  25 river     37 glance    49 spend     
-  │     2022-06-10 06:40:35 slip39                2 steady    14 grin      26 manual    38 rhythm    50 award     
-  │     2022-06-10 06:40:35 slip39                3 decision  15 uncover   27 prospect  39 salon     51 very      
-  │     2022-06-10 06:40:35 slip39                4 spider    16 preach    28 luck      40 script    52 switch    
-  │     2022-06-10 06:40:35 slip39                5 acquire   17 patent    29 fantasy   41 satoshi   53 spew      
-  │     2022-06-10 06:40:35 slip39                6 jerky     18 steady    30 phantom   42 society   54 rival     
-  │     2022-06-10 06:40:35 slip39                7 ambition  19 science   31 phrase    43 argue     55 fridge    
-  │     2022-06-10 06:40:35 slip39                8 course    20 fishing   32 finger    44 says      56 space     
-  │     2022-06-10 06:40:35 slip39                9 ceramic   21 crystal   33 garbage   45 privacy   57 nervous   
-  │     2022-06-10 06:40:35 slip39               10 employer  22 curly     34 taxi      46 blessing  58 envy      
-  │     2022-06-10 06:40:35 slip39               11 august    23 username  35 romantic  47 believe   59 award     
-  │     2022-06-10 06:40:35 slip39               12 kind      24 purchase  36 acquire   48 location  
-  │     2022-06-10 06:40:35 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
-  │     2022-06-10 06:40:35 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
+  │     2022-10-05 16:59:35 slip39                7 erode     19 cowboy    31 merit     43 anxiety   55 fumes     
+  │     2022-10-05 16:59:35 slip39                8 funding   20 river     32 various   44 prayer    56 tadpole   
+  │     2022-10-05 16:59:35 slip39                9 client    21 primary   33 undergo   45 sunlight  57 losing    
+  │     2022-10-05 16:59:35 slip39               10 apart     22 remember  34 depict    46 galaxy    58 famous    
+  │     2022-10-05 16:59:35 slip39               11 amuse     23 thunder   35 example   47 diagnose  59 careful   
+  │     2022-10-05 16:59:35 slip39               12 hawk      24 distance  36 devote    48 usual     
+  │     2022-10-05 16:59:35 slip39           6th  1 teaspoon  13 soldier   25 building  37 gray      49 beaver    
+  │     2022-10-05 16:59:35 slip39                2 steady    14 regret    26 deal      38 desire    50 geology   
+  │     2022-10-05 16:59:35 slip39                3 decision  15 fluff     27 champion  39 parking   51 clock     
+  │     2022-10-05 16:59:35 slip39                4 spider    16 ladybug   28 garlic    40 leaf      52 sheriff   
+  │     2022-10-05 16:59:35 slip39                5 academic  17 reject    29 crunch    41 expand    53 cage      
+  │     2022-10-05 16:59:35 slip39                6 source    18 educate   30 treat     42 garlic    54 staff     
+  │     2022-10-05 16:59:35 slip39                7 system    19 minister  31 nuclear   43 check     55 public    
+  │     2022-10-05 16:59:35 slip39                8 petition  20 improve   32 lamp      44 invasion  56 pulse     
+  │     2022-10-05 16:59:35 slip39                9 peaceful  21 glance    33 academic  45 evil      57 lungs     
+  │     2022-10-05 16:59:35 slip39               10 society   22 pajamas   34 depart    46 family    58 trial     
+  │     2022-10-05 16:59:35 slip39               11 repeat    23 declare   35 impact    47 hesitate  59 percent   
+  │     2022-10-05 16:59:35 slip39               12 render    24 research  36 item      48 pharmacy  
+  │     2022-10-05 16:59:35 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
+  │     2022-10-05 16:59:35 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
   └────
   This `0xfc20..1B5E' address is the same Ethereum address as is
   recovered on a Trezor using this BIP-39 mnemonic phrase.  Thus, we can
   generate "Paper Wallets" for the desired Cryptocurrency accounts, and
   recover the funds.
 
   So, this does the job:
@@ -1515,16 +1500,16 @@
   BIP-39 Mnemonic phrase (not the 512-bit generated Seed):
   ┌────
   │     ( python3 -m slip39.recovery --bip39 --entropy -v \
   │         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" 
   │     ) 2>&1
   └────
   ┌────
-  │ 2022-06-10 06:40:37 slip39.recovery  Recovered 128-bit BIP-39 secret from english mnemonic
-  │ 2022-06-10 06:40:37 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
+  │ 2022-10-05 16:59:37 slip39.recovery  Recovered 128-bit BIP-39 secret from english mnemonic
+  │ 2022-10-05 16:59:37 slip39.recovery  Recovered BIP-39 secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -
   │ ffffffffffffffffffffffffffffffff
   └────
 
   Now we generate SLIP-39 Mnemonics to recover the 128-bit Seed Entropy.
   Note that these are 20-word Mnemonics.  However, these are *NOT* the
   wallets we expected!  These are the well-known native SLIP-39 wallets
   from the `0xFFFF...FF' Seed Entropy; not the well-known native BIP-39
@@ -1534,67 +1519,67 @@
   ┌────
   │     ( python3 -m slip39.recovery --bip39 --entropy \
   │         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
   │       | python3 -m slip39 --secret - --no-card -v
   │     ) 2>&1 | tail -20
   └────
   ┌────
-  │     2022-06-10 06:40:37 slip39                4 skin      11 tricycle  18 install   
-  │     2022-06-10 06:40:37 slip39                5 argue     12 necklace  19 alto      
-  │     2022-06-10 06:40:37 slip39                6 deny      13 extra     20 dining    
-  │     2022-06-10 06:40:37 slip39                7 living    14 flea      
-  │     2022-06-10 06:40:37 slip39           5th  1 strike     8 clinic    15 hanger    
-  │     2022-06-10 06:40:37 slip39                2 guilt      9 crowd     16 umbrella  
-  │     2022-06-10 06:40:37 slip39                3 decision  10 shelter   17 withdraw  
-  │     2022-06-10 06:40:37 slip39                4 snake     11 story     18 evil      
-  │     2022-06-10 06:40:37 slip39                5 amazing   12 ending    19 software  
-  │     2022-06-10 06:40:37 slip39                6 quarter   13 video     20 hazard    
-  │     2022-06-10 06:40:37 slip39                7 transfer  14 maximum   
-  │     2022-06-10 06:40:37 slip39           6th  1 strike     8 grownup   15 sugar     
-  │     2022-06-10 06:40:37 slip39                2 guilt      9 cinema    16 society   
-  │     2022-06-10 06:40:37 slip39                3 decision  10 elephant  17 elevator  
-  │     2022-06-10 06:40:37 slip39                4 spider    11 olympic   18 says      
-  │     2022-06-10 06:40:37 slip39                5 diploma   12 bundle    19 escape    
-  │     2022-06-10 06:40:37 slip39                6 index     13 resident  20 military  
-  │     2022-06-10 06:40:37 slip39                7 scholar   14 spelling  
-  │     2022-06-10 06:40:37 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
-  │     2022-06-10 06:40:37 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
+  │     2022-10-05 16:59:37 slip39                4 skin      11 remove    18 quarter   
+  │     2022-10-05 16:59:37 slip39                5 bracelet  12 axis      19 squeeze   
+  │     2022-10-05 16:59:37 slip39                6 fitness   13 smirk     20 miracle   
+  │     2022-10-05 16:59:37 slip39                7 indicate  14 pharmacy  
+  │     2022-10-05 16:59:37 slip39           5th  1 security   8 keyboard  15 dish      
+  │     2022-10-05 16:59:37 slip39                2 cause      9 memory    16 improve   
+  │     2022-10-05 16:59:37 slip39                3 decision  10 garlic    17 unfair    
+  │     2022-10-05 16:59:37 slip39                4 snake     11 step      18 acrobat   
+  │     2022-10-05 16:59:37 slip39                5 branch    12 building  19 merchant  
+  │     2022-10-05 16:59:37 slip39                6 desktop   13 evoke     20 object    
+  │     2022-10-05 16:59:37 slip39                7 trip      14 eyebrow   
+  │     2022-10-05 16:59:37 slip39           6th  1 security   8 crunch    15 class     
+  │     2022-10-05 16:59:37 slip39                2 cause      9 cylinder  16 vexed     
+  │     2022-10-05 16:59:37 slip39                3 decision  10 burning   17 faint     
+  │     2022-10-05 16:59:37 slip39                4 spider    11 curly     18 firm      
+  │     2022-10-05 16:59:37 slip39                5 cubic     12 receiver  19 upstairs  
+  │     2022-10-05 16:59:37 slip39                6 crush     13 lyrics    20 unkind    
+  │     2022-10-05 16:59:37 slip39                7 smith     14 amazing   
+  │     2022-10-05 16:59:37 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0x824b174803e688dE39aF5B3D7Cd39bE6515A19a1
+  │     2022-10-05 16:59:37 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1q9yscq3l2yfxlvnlk3cszpqefparrv7tk24u6pl
   └────
   Because we must tell `slip39' to that we're using the BIP-39 Mnemonic
   and Seed generation process to derived the wallet addresses from the
   Seed Entropy (not the SLIP-39 standard).  So, we add the
   `-using-bip39' option:
 
   ┌────
   │     ( python3 -m slip39.recovery --bip39 --entropy \
   │         --mnemonic "zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo zoo wrong" \
   │       | python3 -m slip39 --secret - --no-card -v --using-bip39
   │     ) 2>&1 | tail -20
   └────
   ┌────
-  │     2022-06-10 06:40:38 slip39                4 skin      11 easy      18 afraid    
-  │     2022-06-10 06:40:38 slip39                5 crystal   12 beaver    19 lily      
-  │     2022-06-10 06:40:38 slip39                6 superior  13 vocal     20 guitar    
-  │     2022-06-10 06:40:38 slip39                7 acid      14 cover     
-  │     2022-06-10 06:40:38 slip39           5th  1 increase   8 ladybug   15 decent    
-  │     2022-06-10 06:40:38 slip39                2 taxi       9 wealthy   16 process   
-  │     2022-06-10 06:40:38 slip39                3 decision  10 corner    17 multiple  
-  │     2022-06-10 06:40:38 slip39                4 snake     11 merit     18 safari    
-  │     2022-06-10 06:40:38 slip39                5 beam      12 deadline  19 frozen    
-  │     2022-06-10 06:40:38 slip39                6 charity   13 intend    20 enjoy     
-  │     2022-06-10 06:40:38 slip39                7 theater   14 video     
-  │     2022-06-10 06:40:38 slip39           6th  1 increase   8 alive     15 orange    
-  │     2022-06-10 06:40:38 slip39                2 taxi       9 believe   16 being     
-  │     2022-06-10 06:40:38 slip39                3 decision  10 sunlight  17 adequate  
-  │     2022-06-10 06:40:38 slip39                4 spider    11 width     18 beam      
-  │     2022-06-10 06:40:38 slip39                5 blind     12 museum    19 animal    
-  │     2022-06-10 06:40:38 slip39                6 beaver    13 marvel    20 failure   
-  │     2022-06-10 06:40:38 slip39                7 exchange  14 busy      
-  │     2022-06-10 06:40:38 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
-  │     2022-06-10 06:40:38 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
+  │     2022-10-05 16:59:38 slip39                4 skin      11 olympic   18 worthy    
+  │     2022-10-05 16:59:38 slip39                5 duration  12 disease   19 champion  
+  │     2022-10-05 16:59:38 slip39                6 hazard    13 receiver  20 unusual   
+  │     2022-10-05 16:59:38 slip39                7 clock     14 crisis    
+  │     2022-10-05 16:59:38 slip39           5th  1 desire     8 lift      15 ecology   
+  │     2022-10-05 16:59:38 slip39                2 echo       9 graduate  16 hairy     
+  │     2022-10-05 16:59:38 slip39                3 decision  10 artwork   17 slap      
+  │     2022-10-05 16:59:38 slip39                4 snake     11 pacific   18 spend     
+  │     2022-10-05 16:59:38 slip39                5 benefit   12 rich      19 grownup   
+  │     2022-10-05 16:59:38 slip39                6 cricket   13 lips      20 brother   
+  │     2022-10-05 16:59:38 slip39                7 sprinkle  14 flip      
+  │     2022-10-05 16:59:38 slip39           6th  1 desire     8 phrase    15 axis      
+  │     2022-10-05 16:59:38 slip39                2 echo       9 forecast  16 inform    
+  │     2022-10-05 16:59:38 slip39                3 decision  10 patent    17 realize   
+  │     2022-10-05 16:59:38 slip39                4 spider    11 spray     18 object    
+  │     2022-10-05 16:59:38 slip39                5 axis      12 founder   19 python    
+  │     2022-10-05 16:59:38 slip39                6 news      13 idea      20 finger    
+  │     2022-10-05 16:59:38 slip39                7 paper     14 decision  
+  │     2022-10-05 16:59:38 slip39.layout    ETH    m/44'/60'/0'/0/0    : 0xfc2077CA7F403cBECA41B1B0F62D91B5EA631B5E
+  │     2022-10-05 16:59:38 slip39.layout    BTC    m/84'/0'/0'/0/0     : bc1qk0a9hr7wjfxeenz9nwenw9flhq0tmsf6vsgnn2
   └────
   And, there we have it – we've recovered exactly the same Ethereum and
   Bitcoin wallets as would a native BIP-39 hardware wallet like a Ledger
   Nano.
 
 
 ◊ 3.3.2.1 Using SLIP-39 App "Backup" Controls
```

### Comparing `slip39-9.0.4/setup.py` & `slip39-9.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,16 @@
     "slip39.gui":		"./slip39/gui",
 }
 
 package_data			= {
     'slip39': [
         'layout/*.png',
         'layout/*.txt',
-        'gui/*.txt'
+        'layout/font/*.ttf',
+        'gui/*.txt',
     ],
 }
 
 long_description_content_type	= 'text/markdown'
 long_description		= """\
 Creating Ethereum, Bitcoin and other accounts is complex and fraught
 with potential for loss of funds.
```

### Comparing `slip39-9.0.4/slip39/api.py` & `slip39-9.1.2/slip39/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+
+#
+# Python-slip39 -- Ethereum SLIP-39 Account Generation and Recovery
+#
+# Copyright (c) 2022, Dominion Research & Development Corp.
+#
+# Python-slip39 is free software: you can redistribute it and/or modify it under
+# the terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.  It is also available under alternative (eg. Commercial) licenses, at
+# your option.  See the LICENSE file at the top of the source tree.
+#
+# Python-slip39 is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+
 import base58
 import codecs
 import hashlib
 import itertools
 import json
 import logging
 import math
@@ -15,15 +32,15 @@
 
 from shamir_mnemonic	import generate_mnemonics
 
 import hdwallet
 from hdwallet		import cryptocurrencies
 
 from .defaults		import BITS_DEFAULT, BITS, MNEM_ROWS_COLS, GROUP_REQUIRED_RATIO, CRYPTO_PATHS
-from .util		import ordinal
+from .util		import ordinal, commas
 from .recovery		import produce_bip39, recover_bip39
 
 log				= logging.getLogger( __package__ )
 
 # Support for private key encryption via BIP-38 and Ethereum JSON wallet is optional; pip install slip39[wallet]
 paper_wallet_issues		= []
 try:
@@ -222,15 +239,15 @@
         p2pkh_btc	= super( XRPHDWallet, self ).p2pkh_address()
         p2pkh		= base58.b58decode_check( p2pkh_btc )
         return base58.b58encode_check( p2pkh, base58.RIPPLE_ALPHABET ).decode( 'UTF-8' )
 
 
 class Account:
     """A Cryptocurrency "Account" / Wallet, based on a variety of underlying Python crypto-asset
-    support modules.  Presently, only meherett/python-hdwallet is used
+    support modules.  Presently, only meherett/python-hdwallet is used.
 
     An appropriate hdwallet-like wrapper is built, for any crypto-asset supported using another
     module.  The required hdwallet API calls are:
 
       .from_seed	-- start deriving from the provided seed
       .from_mnemonic	-- start deriving from the provided seed via BIP-39 mnemonic
       .clean_derivation	-- forget any prior derivation path
@@ -343,15 +360,15 @@
         """Return the default derivation path for the given crypto, based on its currently selected default
         address format.
 
         """
         crypto			= cls.supported( crypto )
         format			= format.lower() if format else cls.address_format( crypto )
         if format not in cls.CRYPTO_FORMAT_PATH[crypto]:
-            raise ValueError( f"{format} not supported for {crypto}; specify one of {', '.join( cls.CRYPTO_FORMAT_PATH[crypto].keys() )}" )
+            raise ValueError( f"{format} not supported for {crypto}; specify one of {commas( cls.CRYPTO_FORMAT_PATH[crypto].keys() )}" )
         return cls.CRYPTO_FORMAT_PATH[crypto][format]
 
     @classmethod
     def address_format( cls, crypto, format=None ):
         """Get or set the desired default address format for the specified supported crypto.  Future
         instances of Address created for the crypto will use the specified address format and its
         default derivation path.
@@ -359,30 +376,30 @@
         """
         crypto			= cls.supported( crypto )
         if format is None:
             return cls.CRYPTO_FORMAT[crypto]
 
         format			= format.lower() if format else None
         if format not in cls.FORMATS:
-            raise ValueError( f"{crypto} address format {format!r} not recognized; specify one of {', '.join( cls.FORMATS )}" )
+            raise ValueError( f"{crypto} address format {format!r} not recognized; specify one of {commas( cls.FORMATS )}" )
         cls.CRYPTO_FORMAT[crypto]	= format
 
     @classmethod
     def supported( cls, crypto ):
         """Validates that the specified cryptocurrency is supported and returns the normalized short name
         for it, or raises an a ValueError.  Eg. "Ethereum" --> "ETH"
 
         """
         validated		= cls.CRYPTO_NAMES.get(
             crypto.lower(),
             crypto.upper() if crypto.upper() in cls.CRYPTOCURRENCIES else None
         )
         if validated:
             return validated
-        raise ValueError( f"{crypto} not presently supported; specify {', '.join( cls.CRYPTOCURRENCIES )}" )
+        raise ValueError( f"{crypto} not presently supported; specify {commas( cls.CRYPTOCURRENCIES )}" )
 
     def __str__( self ):
         """Until from_seed/from_path are invoked, may not have an address or derivation path."""
         address			= None
         try:
             address		= self.address
         except Exception:
@@ -437,19 +454,23 @@
             from_path		= path_edit( from_path, path )
         self.hdwallet.clean_derivation()
         self.hdwallet.from_path( from_path )
         return self
 
     @property
     def address( self ):
-        if self.format == "legacy":
+        """Returns the 1..., 3... or bc1... address, depending on whether format is legacy, segwit or bech32"""
+        return self.formatted_address()
+
+    def formatted_address( self, format=None ):
+        if ( format or self.format or '' ).lower() == "legacy":
             return self.legacy_address()
-        elif self.format == "segwit":
+        elif ( format or self.format or '' ).lower() == "segwit":
             return self.segwit_address()
-        elif self.format == "bech32":
+        elif ( format or self.format or '' ).lower() == "bech32":
             return self.bech32_address()
         raise ValueError( f"Unknown addresses semantic: {self.format}" )
 
     def substitute_symbol( method ):
         """For some locally-defined cryptocurrencies, the python-hdwallet code specifically checks
         for "ETH" and represents the address in the standard Ethereum 0x... format.  For those
         cryptocurrencies that need the underlying hdwallet._cryptocurrency.symbol adjusted during
@@ -492,17 +513,26 @@
         return self.hdwallet.path()
 
     @property
     def key( self ):
         return self.hdwallet.private_key()
 
     @property
+    def xkey( self ):
+        return self.hdwallet.xprivate_key()
+
+    @property
     def pubkey( self ):
         return self.hdwallet.public_key()
 
+    @property
+    def xpubkey( self ):
+        """Returns the xpub, ypub or zpub, depending on whether format is legacy, segwit or bech32"""
+        return self.hdwallet.xpublic_key()
+
     def from_private_key( self, private_key ):
         self.hdwallet.from_private_key( private_key )
         return self
 
     def encrypted( self, passphrase ):
         """Output the appropriately encrypted private key for this cryptocurrency.  Ethereum uses
         encrypted JSON wallet standard, Bitcoin et.al. use BIP-38 encrypted private keys."""
@@ -871,15 +901,15 @@
         g_name: (g_of, g_mnems)
         for (g_name,(g_of, _),g_mnems) in zip( g_names, g_dims, mnems )
     }
     if log.isEnabledFor( logging.INFO ):
         group_reqs			= list(
             f"{g_nam}({g_of}/{len(g_mns)})" if g_of != len(g_mns) else f"{g_nam}({g_of})"
             for g_nam,(g_of,g_mns) in groups.items() )
-        requires		= f"Recover w/ {group_threshold} of {len(groups)} groups {', '.join(group_reqs)}"
+        requires		= f"Recover w/ {group_threshold} of {len(groups)} groups {commas( group_reqs )}"
         for g_n,(g_name,(g_of,g_mnems)) in enumerate( groups.items() ):
             log.info( f"{g_name}({g_of}/{len(g_mnems)}): {requires}" )
             for mn_n,mnem in enumerate( g_mnems ):
                 for line,_ in organize_mnemonic( mnem, label=f"{ordinal(mn_n+1)} " ):
                     log.info( f"{line}" )
 
     return Details(name, group_threshold, groups, accts, using_bip39)
@@ -898,15 +928,15 @@
 
     """
     if master_secret is None:
         assert strength in BITS, f"Invalid {strength}-bit secret length specified"
         master_secret		= random_secret( strength // 8 )
     if len( master_secret ) * 8 not in BITS:
         raise ValueError(
-            f"Only {', '.join( f'{b}-' for b in BITS )}bit seeds supported; {len(master_secret)*8}-bit master_secret supplied" )
+            f"Only {commas( BITS, final_and=True )}-bit seeds supported; {len(master_secret)*8}-bit seed supplied" )
     return generate_mnemonics(
         group_threshold	= group_threshold,
         groups		= groups,
         master_secret	= master_secret,
         passphrase	= passphrase,
         iteration_exponent = iteration_exponent )
 
@@ -972,16 +1002,16 @@
         ],
         ...
 
     """
     yield from zip( *[
         accounts(
             master_secret	= master_secret,
-            paths		= paths,
             crypto		= crypto,
+            paths		= paths,
             allow_unbounded	= allow_unbounded,
         )
         for crypto,paths in cryptopaths_parser( cryptopaths )
     ])
 
 
 def address(
```

### Comparing `slip39-9.0.4/slip39/api_passphrase_test.py` & `slip39-9.1.2/slip39/api_passphrase_test.py`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/api_test.py` & `slip39-9.1.2/slip39/api_test.py`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/defaults.py` & `slip39-9.1.2/slip39/defaults.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 
 #
 # Python-slip39 -- Ethereum SLIP-39 Account Generation and Recovery
 #
-# Copyright (c) 2021, Dominion Research & Development Corp.
+# Copyright (c) 2022, Dominion Research & Development Corp.
 #
 # Python-slip39 is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
-# version. See the LICENSE file at the top of the source tree.
+# version.  It is also available under alternative (eg. Commercial) licenses, at
+# your option.  See the LICENSE file at the top of the source tree.
 #
 # Python-slip39 is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 
+__author__                      = "Perry Kundert"
+__email__                       = "perry@dominionrnd.com"
+__copyright__                   = "Copyright (c) 2022 Dominion Research & Development Corp."
+__license__                     = "Dual License: GPLv3 (or later) and Commercial (see LICENSE)"
+
 #
 # HD Wallet Derivation Paths (Standard BIP-44 / Trezor)
 #
 #     https://wolovim.medium.com/ethereum-201-hd-wallets-11d0c93c87f7
 #
 # BIP-44 defines the purpose of each depth level:
 #    m / purpose’ / coin_type’ / account’ / change / address_index
@@ -34,15 +40,15 @@
     "Fam(4)",
     "Frens3/6"
 ]
 
 THEME				= 'DarkAmber'   # PySimpleGUI Theme
 FONTS				= dict(
     sans	= 'helvetica',
-    mono	= 'courier',
+    mono	= 'sourcecode',  # UTF-8 monospaced w/ "━": dejavu, inconsolata, noto, overpass, sourcecode
 )
 
 #                                  Y      X       Margin
 BUSINESS_CARD			= (2,     3+1/2), 1/32  # noqa: E241
 CREDIT_CARD			= (2+1/4, 3+3/8), 1/32
 INDEX_CARD			= (3,     5),     1/16  # noqa: E241
 HALF_LETTER			= (13.5/3,8),     1/8   # noqa: E241 (actually, 2/letter, 3/legal)
@@ -92,16 +98,17 @@
     'Pro',
 ]
 LAYOUT_BAK			= 0
 LAYOUT_CRE			= 1
 LAYOUT_REC			= 2
 LAYOUT_PRO			= 3
 
-BITS				= (128, 256, 512)
 BITS_DEFAULT			= 128
+BITS				= (128, 256, 512)
+BITS_BIP39			= BITS + (160, 192, 224)
 
 MNEM_ROWS_COLS			= {
     20:	( 7, 3),		# 128-bit seed
     33:	(11, 3),		# 256-bit seed
     59:	(12, 5),		# 512-bit seed, eg. from BIP-39 (Unsupported on Trezor)
 }
 
@@ -118,14 +125,16 @@
 
 FILENAME_KEYWORDS		= ['name', 'date', 'time', 'crypto', 'path', 'address']
 FILENAME_FORMAT			= "{name}-{date}+{time}-{crypto}-{address}.pdf"
 
 # Default Crypto accounts (and optional paths) to generate
 CRYPTO_PATHS			= ('ETH', 'BTC')
 
+__d				= "55"
+__m				= "88"
 __o				= "BB"
 __h				= "DD"
 __f				= "FF"
 COLOR				= [
     # Primary
     f"0x{__o}{__o}{__f}",  # Blue
     f"0x{__o}{__f}{__o}",  # Green
@@ -141,9 +150,12 @@
     f"0x{__h}{__o}{__f}",  # Violet
     f"0x{__h}{__f}{__o}",  # Lime
     f"0x{__f}{__h}{__o}",  # Orange
     # Other
     f"0x{__o}{__h}{__h}",  # Light Cyan
     f"0x{__h}{__o}{__h}",  # Light Magenta
     f"0x{__h}{__h}{__o}",  # Light Yellow
+    # Greys
     f"0x{__h}{__h}{__h}",  # Light grey,
+    f"0x{__m}{__m}{__m}",  # Medium grey,
+    f"0x{__d}{__d}{__d}",  # Dark grey,
 ]
```

### Comparing `slip39-9.0.4/slip39/dependency_test.py` & `slip39-9.1.2/slip39/dependency_test.py`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/generator/__init__.py` & `slip39-9.1.2/slip39/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/generator/main.py` & `slip39-9.1.2/slip39/generator/main.py`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/generator_test.py` & `slip39-9.1.2/slip39/generator_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -121,21 +121,7 @@
     ser				= SerialEOF( slave_name, timeout=1)
     for group in accountgroups_input(
         cipher		= chacha20poly1305( password=password ),
         encoding	= 'UTF-8',
         file		= ser
     ):
         logging.info( f"Receive: {group}" )
-
-
-# def transmitter():
-
-
-#     yield from addresses(
-#         master_secret			= b"\xFF" * 16,
-#         paths
-
-
-# def test_serial_xonxoff():
-#     """Ensure that flow-control works.  The idealy secure solution is to use hardware RTS/CTS flow
-#     control, with no tx circuit.  However, even a regular serial link with software XON/XOFF flow
-#     control is much more secure than a network-connected peer."""
```

### Comparing `slip39-9.0.4/slip39/gui/SLIP-39.txt` & `slip39-9.1.2/slip39/gui/SLIP-39.txt`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/gui/main.py` & `slip39-9.1.2/slip39/gui/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import subprocess
 
 from itertools import islice
 
 import PySimpleGUI as sg
 
 from ..api		import Account, create, group_parser, random_secret, cryptopaths_parser, paper_wallet_available
-from ..recovery		import recover, recover_bip39, produce_bip39
-from ..util		import log_level, log_cfg, ordinal, chunker, hue_shift
+from ..recovery		import recover, recover_bip39, produce_bip39, scan_entropy, display_entropy
+from ..util		import log_level, log_cfg, ordinal, commas, chunker, hue_shift, rate_dB, entropy_rating_dB, timing, avg
 from ..layout		import write_pdfs, printers_available
 from ..defaults		import (
-    GROUPS, GROUP_THRESHOLD_RATIO, MNEM_PREFIX, CRYPTO_PATHS, BITS, BITS_DEFAULT,
+    GROUPS, GROUP_THRESHOLD_RATIO, MNEM_PREFIX, CRYPTO_PATHS, BITS, BITS_BIP39, BITS_DEFAULT,
     CARD_SIZES, CARD, PAPER_FORMATS, PAPER, WALLET_SIZES, WALLET, MNEM_CONT, THEME,
     LAYOUT, LAYOUT_OPTIONS, LAYOUT_BAK, LAYOUT_CRE, LAYOUT_REC, LAYOUT_PRO
 )
 
 log				= logging.getLogger( __package__ )
 
 
@@ -29,29 +29,51 @@
 BIP39_EXAMPLE_256		= "zoo " * 23 + "vote"
 SLIP39_EXAMPLE_128              = "academic acid acrobat romp change injury painting safari drug browser" \
                                   " trash fridge busy finger standard angry similar overall prune ladybug" \
                                   "\n" \
                                   "academic acid beard romp believe impulse species holiday demand building" \
                                   " earth warn lunar olympic clothes piece campus alpha short endless"
 
+SD_SEED_FRAME			= 'Seed Source: Create your Seed Entropy here'
+SE_SEED_FRAME			= 'Seed Extra Randomness'
+SS_SEED_FRAME			= 'Seed Secret & SLIP-39 Recovery Groups'
 
 def theme_color( thing, theme=None ):
     """Get the currency configured PySimpleGUI Theme color for thing == eg. "TEXT", "BACKGROUND.
     """
     if theme is None:
         theme			= sg.CURRENT_LOOK_AND_FEEL
     return sg.LOOK_AND_FEEL_TABLE[theme][thing]
 
+# Try to pick a font; Use something like this to see what's available (ya, this sucks):
+# 
+#     from tkinter import Tk, font
+#     root = Tk()
+#     font_tuple = font.families()
+#     #Creates a Empty list to hold font names
+#     FontList=[]
+#     fonts = [font.Font(family=f) for f in font.families()]
+#     monospace = [f for f in fonts if f.metrics("fixed")]
+#     for font in monospace:
+#         FontList.append(font.actual('family'))
+#     root.destroy()
+#     print( '\n'.join( FontList ))
+if sys.platform == 'darwin':
+    font_name			= 'Source Code Pro'
+elif sys.platform == 'win32':
+    font_name			= 'Consolas'
+else:  # assume linux
+    font_name			= 'DejaVu Sans Mono'
 
 font_points			= 14
-font				= ('Courier', font_points+0)
-font_dense			= ('Courier', font_points-2)
-font_small			= ('Courier', font_points-4)
-font_big			= ('Courier', font_points+2)
-font_bold			= ('Courier', font_points+2, 'bold italic')
+font				= (font_name, font_points+0)
+font_dense			= (font_name, font_points-2)
+font_small			= (font_name, font_points-4)
+font_big			= (font_name, font_points+2)
+font_bold			= (font_name, font_points+2, 'bold italic')
 
 I_kwds				= dict(
     change_submits	= True,
     font		= font,
 )
 I_kwds_small			= dict(
     change_submits	= True,
@@ -207,29 +229,28 @@
                     ] )
                 ]
             ],                                          key='-OUTPUT-F-',                       **F_kwds_big ),
         ],
     ] + [
         [
             # SLIP-39 only available in Recovery; SLIP-39 Passphrase only in Pro; BIP-39 and Fixed Hex only in Pro
-            sg.Frame( 'Seed Source: Input or Create your Seed Entropy here', [
+            sg.Frame( SD_SEED_FRAME, [
                 [
                     sg.Text( "Random:" if not LO_BAK else "Source:",            visible=LO_CRE, **T_hue( T_kwds, 0/20 )),
                     sg.Radio( "128-bit",          "SD", key='-SD-128-RND-',     default=LO_CRE,
                                                                                 visible=LO_CRE, **T_hue( B_kwds, 0/20 )),
                     sg.Radio( "256-bit",          "SD", key='-SD-256-RND-',     visible=LO_CRE, **T_hue( B_kwds, 0/20 )),
                     sg.Radio( "512-bit",          "SD", key='-SD-512-RND-',     visible=LO_PRO, **T_hue( B_kwds, 0/20 )),
                     sg.Text( "Recover:",                                        visible=LO_BAK, **T_hue( T_kwds, 2/20 )),
                     sg.Radio( "SLIP-39",          "SD", key='-SD-SLIP-',        visible=LO_REC, **T_hue( B_kwds, 2/20 )),
                     sg.Radio( "BIP-39",           "SD", key='-SD-BIP-',         default=LO_BAK,
                                                                                 visible=LO_BAK or LO_CRE,
                                                                                                 **T_hue( B_kwds, 2/20 )),
                     sg.Radio( "BIP-39 Seed",      "SD", key='-SD-BIP-SEED-',    visible=LO_PRO, **T_hue( B_kwds, 2/20 )),
-                    sg.Checkbox( 'Passphrase',
-                                                        key='-SD-PASS-C-',      visible=False,  **T_hue( B_kwds, 2/20 )),
+                    sg.Checkbox( 'Passphrase',          key='-SD-PASS-C-',      visible=False,  **T_hue( B_kwds, 2/20 )),
                 ],
                 [
                     sg.Text("Fixed: ",                                          visible=LO_PRO, **T_hue( T_kwds, 1/20 )),
                 ] + [
                     sg.Radio( f"{b}-bit",  "SD", key=f"-SD-{b}-FIX-",           visible=LO_PRO, **T_hue( B_kwds, 1/20 ))
                     for b in BITS
                 ] + [
@@ -239,34 +260,38 @@
                             sg.Input( "",               key='-SD-PASS-',        size=inputs,    **I_kwds ),
                         ],
                     ],                                  key='-SD-PASS-F-',      visible=False,  **F_kwds ),
                 ],
                 [
                     sg.Frame( 'From Mnemonic(s):', [
                         [
-                            sg.Multiline( "",           key='-SD-DATA-',        size=mnemos,    **I_kwds_small ),
+                            sg.Multiline( "",           key='-SD-DATA-',        size=mnemos,
+                                          no_scrollbar=True,                                    **I_kwds_small ),
                         ],
                     ],                                  key='-SD-DATA-F-',      visible=False,  **F_kwds ),
                 ],
                 [
                     sg.Text( "Seed Raw Data: ",                                 visible=LO_REC,
                                                                                 size=prefix,    **T_kwds ),
                     sg.Text( "",                        key='-SD-SEED-',        visible=LO_REC,
                                                                                 size=inlong,    **T_kwds ),
                 ],
             ],                                          key='-SD-SEED-F-',                      **F_kwds_big ),
         ],
     ] + [
+
         [
-            sg.Frame( 'Seed Extra Randomness (Trust but Verify ;-)', [
+            sg.Frame( SE_SEED_FRAME, [
                 [
                     sg.Radio( "None",             "SE", key='-SE-NON-',         visible=LO_REC,
                                                                                 default=True,   **B_kwds ),
                     sg.Radio( "Hex",              "SE", key='-SE-HEX-',         visible=LO_PRO, **B_kwds ),
                     sg.Radio( "Die rolls, ... (SHA-512)", "SE", key='-SE-SHA-', visible=LO_REC, **B_kwds ),
+                    sg.Checkbox( 'Ignore Bad Entropy', key='-SE-SIGS-C-', 	visible=LO_REC or LO_PRO,
+				 						disabled=False, **T_hue( B_kwds, 3/20 )),
                 ],
                 [
                     sg.Frame( 'Entropy', [
                         [
                             sg.Text( "Hex digits: ",    key='-SE-DATA-T-',      size=prefix,    **T_kwds ),
                             sg.Input( "",               key='-SE-DATA-',        size=inlong,    **I_kwds ),
                         ],
@@ -278,40 +303,46 @@
                     sg.Text( "",                        key='-SE-SEED-',        visible=LO_REC,
                                                                                 size=inlong,    **T_kwds ),
                 ],
             ],                                          key='-SE-SEED-F-',      visible=LO_CRE, **F_kwds_big ),
         ]
     ] + [
         [
-            sg.Frame( 'Seed Secret & SLIP-39 Recovery Groups', [
+            sg.Frame( SS_SEED_FRAME, [
                 [
                     sg.Text( "Seed Secret: ",                                   size=prefix,    **T_kwds ),
                     sg.Text( "",                        key='-SEED-',           size=inlong,    **T_kwds ),
                 ],
                 [
                     sg.Checkbox( "Using BIP-39:",       key='-AS-BIP-CB-',      default=True,
                                                                                 size=prefix,    **T_hue( B_kwds, -1/20 )),
                     sg.Text( '',                        key='-AS-BIP-',         visible=True,   **T_hue( T_kwds_dense, -1/20 )),
                 ],
                 [
                     sg.Column( [
                         [
-                            sg.Text( "Passphrase:",     key='-PASSPHRASE-L-',   size=prefix,    **T_kwds ),
-                            sg.Input( f"{passphrase or ''}",    key='-PASSPHRASE-',     size=inputs,    **I_kwds ),
+                            sg.Frame( "BIP-39 Passphrase", [
+                                [
+                                    sg.Text( "Passphrase (encrypt):",                           **T_kwds ),
+                                    sg.Input( f"{passphrase or ''}",
+                                                        key='-PASSPHRASE-',     size=inputs,    **I_kwds ),
+                                ],
+                            ],                          key='-PASSPHRASE-F-',   visible=True,   **F_kwds ),
                         ],
                         [
                             sg.Text( "Recovery needs: ",                        size=prefix,    **T_kwds ),
                             sg.Input( f"{group_threshold}", key='-THRESHOLD-',  size=tiny,      **I_kwds ),
                             sg.Text( f"of {len(groups)}", key='-RECOVERY-',                     **T_kwds ),
                             sg.Button( '+', **B_kwds ),
                             sg.Text( "Mnemonic Card Groups",                                    **T_kwds ),
                         ],
                         group_body,
                     ] ),
-                    sg.Multiline( "",                   key='-INSTRUCTIONS-',   size=(80,15),   **T_kwds_dense ),
+                    sg.Multiline( "",                   key='-INSTRUCTIONS-',   size=(80,15),
+                                  no_scrollbar=True, horizontal_scroll=LO_PRO or LO_REC,        **T_kwds_dense ),
                 ],
             ],                                          key='-GROUPS-F-',                       **F_kwds_big ),
         ],
     ] + [
         [
             sg.Frame( 'Cryptocurrencies and Paper Wallets', [
                 [
@@ -451,118 +482,145 @@
     """Respond to changes in the desired Seed Data source, and recover/generate and update the
     -SD-SEED- text, which is a Text field (not in values), and defines the size of the Seed in hex
     nibbles.  If invalid, we will fill it with the appropriate number of '---...'.
 
     Stores the last known state of the -SD-... radio buttons, and saves/restores the user data being
     supplied on for BIP/SLIP/FIX.  If event indicates one of our radio-buttons is re-selectedd, then
     also re-generate the random data.  If a system event occurs (eg. after a Controls change),
-    restores our last-known radio button and data.
+    restores our last-known radio button and data.  Since we cannot know if/when our main window is
+    going to disappear and be replaced, we constantly save the current state.
 
+    Reports the quality of the Seed Data in the frame label.
     """
+    SD_CONTROLS			= [
+        '-SD-128-RND-',
+        '-SD-256-RND-',
+        '-SD-512-RND-',
+        '-SD-128-FIX-',
+        '-SD-256-FIX-',
+        '-SD-512-FIX-',
+        '-SD-BIP-',			# Recover 128- to 256-bit Mnemonic Seed Entropy
+        '-SD-BIP-SEED-',		# Recover 512-bit Generated Seed w/ passphrase
+        '-SD-SLIP-',
+    ]
     changed			= False
-    if not event.startswith( '-' ) and update_seed_data.src and window[update_seed_data.src].visible:
-        # Some system event; restore where we left off (if known, and if the remembered control is visible).
-        data, pswd		= update_seed_data.was.get( update_seed_data.src, ('','') )
-        seed			= None
-        values[update_seed_data.src] = True
-        window[update_seed_data.src].update( True )
-        update_seed_data.src	= None
+    # Some system event (eg. __TIMEOUT__ immediately after a new main window is created, or due to
+    # scheduled callback); restore where we left off if known, and if the remembered control is
+    # visible.  This allows continuation between major screen changes w/ full controls regeneration.
+    # As long as the new screen contains the current visible control, we'll continue editing our Seed
+    # Data wherever we left off.  If the new screen has different controls, we'll get whatever is
+    # there, instead.
+    if not event.startswith( '-' ):
+        log.warning( f"Restoring Seed Source w/ event {event} from saved {update_seed_data.src}"
+                     f" data/password{' (none saved)' if update_seed_data.src not in update_seed_data.was else ''}" )
+        if not values[update_seed_data.src]:
+            # Something else has been selected (probably due to a major display change).
+            if window[update_seed_data.src].visible:
+                # And its still visible; switch back to where we were...
+                for src in SD_CONTROLS:
+                    values[src]	= False
+                values[update_seed_data.src] = True
+                window[update_seed_data.src].update( True )
+            else:
+                # And it isn't available; switch to newly available default...
+                update_seed_data.src, = ( src for src in SD_CONTROLS if values[src] )
+            changed		= True  # and force controls visiblity update
+        data, pswd, seed	= update_seed_data.was.get( update_seed_data.src, ('', '', None) )
+    elif not values[update_seed_data.src]:
+        # A controls selection change.
+        update_seed_data.src,	= ( src for src in SD_CONTROLS if values[src] )
+        changed			= True  # and force controls visiblity update
+        data, pswd, seed	= update_seed_data.was.get( update_seed_data.src, ('', '', None) )
     else:
-        data, pswd		= values['-SD-DATA-'], values['-SD-PASS-']
-        seed			= window['-SD-SEED-'].get()
-    for src in [
-            '-SD-128-RND-',
-            '-SD-256-RND-',
-            '-SD-512-RND-',
-            '-SD-128-FIX-',
-            '-SD-256-FIX-',
-            '-SD-512-FIX-',
-            '-SD-BIP-',			# Recover 128- to 256-bit Mnemonic Seed Entropy
-            '-SD-BIP-SEED-',		# Recover 512-bit Generated Seed w/ passphrase
-            '-SD-SLIP-',
-    ]:
-        # See what we got for -SD-DATA-, for this -SD-... radio button selection
-        if values[src] and update_seed_data.src != src:
-            # If selected radio-button for Seed Data source changed, save last source's working data
-            # and restore what was, last time we were working on this source.  If the triggering
-            # event is not one of ours (eg. __TIMEOUT__), then don't overwrite memory.
-            if update_seed_data.src and event.startswith( '-' ):
-                #log.warning( f"Switching Seed Source w/ event {event} to {src}: saving {update_seed_data.src}: {data!r:.10}..., {pswd!r}" )
-                update_seed_data.was[update_seed_data.src] = data, pswd
-            changed		= True
-            update_seed_data.src = src
-            data, pswd		= update_seed_data.was.get( src, ('','') )
-            seed		= None
-            window['-SD-DATA-'].update( data )
-            values['-SD-DATA-'] = data
-            window['-SD-PASS-'].update( pswd )
-            # And change visibility of Seed Data source controls
-            if 'FIX' in update_seed_data.src:
-                window['-SD-DATA-F-'].update( "Hex data: " )
-                window['-SD-DATA-F-'].update( visible=True  )
-                window['-SD-PASS-C-'].update( visible=False )
-                window['-SD-PASS-F-'].update( visible=False )
-            elif 'BIP-SEED' in update_seed_data.src:
-                window['-SD-DATA-F-'].update( "BIP-39 Mnemonic (for 512-bit Seed Recovery): " )
-                window['-SD-DATA-F-'].update( visible=True )
-                window['-SD-PASS-C-'].update( visible=True )
-                window['-SD-PASS-F-'].update(
-                    "BIP-39 passphrase (won't be needed for Recovery)",
-                    visible=values['-SD-PASS-C-']
-                )
-            elif 'BIP' in update_seed_data.src:
-                window['-SD-DATA-F-'].update( "BIP-39 Mnemonic: " )
-                window['-SD-DATA-F-'].update( visible=True )
-                window['-SD-PASS-C-'].update( visible=False )
-                window['-SD-PASS-F-'].update(
-                    visible=False
-                )
-            elif 'SLIP' in update_seed_data.src:
-                window['-SD-DATA-F-'].update( "SLIP-39 Mnemonics: " )
-                window['-SD-DATA-F-'].update( visible=True )
-                window['-SD-PASS-C-'].update( visible=True )
-                window['-SD-PASS-F-'].update(
-                    passphrase_trezor_incompatible,
-                    visible=values['-SD-PASS-C-']
-                )
-            elif 'RND' in update_seed_data.src:
-                window['-SD-DATA-F-'].update( visible=False )
-                window['-SD-PASS-C-'].update( visible=False )
-                window['-SD-PASS-F-'].update( visible=False )
-        elif event == update_seed_data.src == src:
+        # A normal user-initiated window event, w/ no controls change; get updated value/window data
+        if event == update_seed_data.src:
             # Same radio-button re-selected; just force an update (eg. re-generate random)
-            changed		= True
-    if not seed:
-        seed		= '-' * ( BITS_DEFAULT // 4 )
+            log.info( f"Seed Data update forced due to event: {event!r}" )
+            changed		= True  # and force controls visiblity update
+        data, pswd, seed	= values['-SD-DATA-'], values['-SD-PASS-'], window['-SD-SEED-'].get()
+
+    # Now that we've recovered which Seed Data control was previously in play (and any data/pswd),
+    # update window/value content and other controls' visibility for this -SD-...  selection.
+    window['-SD-DATA-'].update( data )
+    values['-SD-DATA-']		= data
+    window['-SD-PASS-'].update( pswd )
+    if 'FIX' in update_seed_data.src:
+        window['-SD-DATA-F-'].update( "Hex data: " )
+        window['-SD-DATA-F-'].update( visible=True  )
+        window['-SD-PASS-C-'].update( visible=False )
+        window['-SD-PASS-F-'].update( visible=False )
+    elif 'BIP-SEED' in update_seed_data.src:
+        # We're recovering the (decrypted) BIP-39 Seed, so we require the Passphrase!
+        window['-SD-DATA-F-'].update( "BIP-39 Mnemonic (for 512-bit Seed Recovery): " )
+        window['-SD-DATA-F-'].update( visible=True )
+        window['-SD-PASS-C-'].update( visible=True )
+        window['-SD-PASS-F-'].update(
+            "BIP-39 passphrase (won't be needed for Recovery)",
+            visible=values['-SD-PASS-C-']
+        )
+    elif 'BIP' in update_seed_data.src:
+        # We're recovering the BIP-39 Seed Phrase *Entropy*, NOT the derived (decrypted) 512-bit
+        # Seed Data!  So, we don't deal in Passphrases, here.  The Passphrase (to encrypt the Seed,
+        # when "Using BIP-39") is only required to display the correct wallet addresses.
+        window['-SD-DATA-F-'].update( "BIP-39 Mnemonic: " )
+        window['-SD-DATA-F-'].update( visible=True )
+        window['-SD-PASS-C-'].update( visible=False )
+        window['-SD-PASS-F-'].update( visible=False )
+    elif 'SLIP' in update_seed_data.src:
+        window['-SD-DATA-F-'].update( "SLIP-39 Mnemonics: " )
+        window['-SD-DATA-F-'].update( visible=True )
+        window['-SD-PASS-C-'].update( visible=True )
+        window['-SD-PASS-F-'].update(
+            passphrase_trezor_incompatible,
+            visible=values['-SD-PASS-C-']
+        )
+    elif 'RND' in update_seed_data.src:
+        window['-SD-DATA-F-'].update( visible=False )
+        window['-SD-PASS-C-'].update( visible=False )
+        window['-SD-PASS-F-'].update( visible=False )
 
     # We got our working -SD-DATA- into 'data' (maybe from last time 'round), compute seed.
     status			= None
     bits			= None
+    if not seed:
+        seed		= '-' * ( BITS_DEFAULT // 4 )
     if 'BIP' in update_seed_data.src:
         # When recovering from BIP-39 for use in SLIP-39, we always recover the ORIGINAL 128- or
-        # 256-bit Entropy used to create the BIP-39 Mnemonic.  This is what we want to back up --
-        # NOT the 512-bit Seed output from the processing the BIP-39 Mnemonic + passphrase; thus, we
-        # can always re-produce the BIP-39 mnemonic.  Later, (when producing wallets) we'll see if
-        # the desired target device seed will be transmitted via BIP-39 + passphrase, or SLIP-39, and
-        # produce the correct Seed for deriving predicted wallet addresses.
-        window['-SD-PASS-F-'].update( visible=values['-SD-PASS-C-'] )
+        # 256-bit Entropy used to create the BIP-39 Mnemonic (other sizes of BIP-39 Entropy are not
+        # supported).  This is what we want to back up -- NOT the 512-bit Seed output from the
+        # processing the BIP-39 Mnemonic + passphrase; thus, we can always re-produce the BIP-39
+        # mnemonic.  Later, (when producing wallets) we'll see if the desired target device seed
+        # will be transmitted via BIP-39 + passphrase, or SLIP-39, and produce the correct Seed for
+        # deriving predicted wallet addresses.
         try:
-            # No passphrase allowed/required, to get original BIP-39 Mnemonic Entropy
-            # Only needed (later) for Account generation
-            passphrase		= pswd.strip().encode( 'UTF-8' )
+            # No passphrase allowed/required, to get original BIP-39 Mnemonic Entropy Only needed
+            # (later) for Account generation.  This *may* produce a number of bits NOT in
+            # default.BITS!  (eg. from a 160- or 192-bit BIP-39 Mnemonics). This is allowable,
+            # because if as_entropy is True, we'll be BIP-39-encrypting the Seed Data to generate a
+            # 512-bit seed.
             as_entropy		= 'BIP-SEED' not in update_seed_data.src
+            if as_entropy:
+                if pswd:
+                    log.warning( f"BIP-39 Seed Passphrase (decrypt) ignored; using Seed Phrase Entropy, not decrypted Seed!" )
+                passphrase	= b""
+            else:
+                if pswd.strip() != pswd:
+                    log.warning( f"BIP-39 Seed Passphrase (decrypt) contains leading/trailing whitespace; are you certain this is correct?" ) 
+                passphrase	= pswd.encode( 'UTF-8' )
             seed		= recover_bip39(
                 mnemonic	= data.strip(),
-                passphrase	= b"" if as_entropy else passphrase,
+                passphrase	= passphrase,
                 as_entropy	= as_entropy,
             )
             bits		= len( seed ) * 8
+            assert bits in BITS_allowed( values ), \
+                f"Only {commas(BITS, final_and=True)}-bit BIP-39 Mnemonics supported, unless 'Using BIP-39' selected"
         except Exception as exc:
-            log.warning( f"BIP-39 recovery failed w/{data!r}: {exc}" )
             status		= f"Invalid BIP-39 recovery mnemonic: {exc}"
+            log.warning( status )
     elif 'SLIP' in update_seed_data.src:
         window['-SD-PASS-F-'].update( visible=values['-SD-PASS-C-'] )
         try:
             passphrase		= pswd.strip().encode( 'UTF-8' )
             seed		= recover(
                 mnemonics	= list( mnemonic_continuation( data.strip().split( '\n' ))),
                 passphrase	= passphrase,
@@ -571,52 +629,84 @@
         except Exception as exc:
             log.warning( f"SLIP-39 recovery failed w/ {data!r}: {exc}" )
             status		= f"Invalid SLIP-39 recovery mnemonics: {exc}"
     elif 'FIX' in update_seed_data.src:
         bits			= int( update_seed_data.src.split( '-' )[2] )
         try:
             # 0-fill and truncate any supplied hex data to the desired bit length
-            data		= f"{data:<0{bits // 4}.{bits // 4}}"
-            seed 		= codecs.decode( data, 'hex_codec' )
+            data_filled		= f"{data:<0{bits // 4}.{bits // 4}}"
+            seed 		= codecs.decode( data_filled, 'hex_codec' )
         except Exception as exc:
             log.warning( f"Fixed hex recovery failed w/ {data!r}: {exc}" )
             status		= f"Invalid Hex for {bits}-bit fixed seed: {exc}"
-    elif changed:  # Random.  Regenerated each time changed, or not valid
+    elif changed or not seed:  # RND.  Regenerated each time changed, or not valid
         bits			= int( update_seed_data.src.split( '-' )[2] )
         seed			= random_secret( bits // 8 )
 
     # Compute any newly computed/recovered binary Seed Data bytes as hex. Must be 128-, 256- or
-    # 512-bit hex data.
-    try:
-        if type(seed) is not str:
-            seed		= codecs.encode( seed, 'hex_codec' ).decode( 'ascii' )
-        if bits is None:  # For previously defined seed_data, compute length
-            bits		= len( seed ) * 4
-        assert len( seed ) * 4 == bits, \
-            f"{len(seed)*4}-bit data recovered; expected {bits} bits: {seed}"
-        assert bits in BITS, \
-            f"Invalid {bits}-bit data size: {seed}"
-    except Exception as exc:
-        status			= f"Invalid seed data: {exc}"
+    # 512-bit hex data.  Do a final comparison against current -SD-SEED- to detect changes.
+    if status:
+        status			= f"Invalid Seed Data: {status}"
+    else:
+        try:
+            if type(seed) is not str:
+                seed		= codecs.encode( seed, 'hex_codec' ).decode( 'ascii' )
+            if bits is None:  # For previously defined seed_data, compute length
+                bits		= len( seed ) * 4
+            assert len( seed ) * 4 == bits, \
+                f"{len(seed)*4}-bit data recovered; expected {bits} bits: {seed}"
+            assert bits in BITS_allowed( values ), \
+                f"Invalid {bits}-bit data size: {seed}"
+        except Exception as exc:
+            status			= f"Invalid Seed Data: {exc}"
+    if status:
         if not bits:
             bits		= BITS_DEFAULT
         seed			= '-' * (bits // 4)
+    if window['-SD-SEED-'].get() != seed:
+        update_seed_data.deficiencies = ()
+        changed			= True
+
+    # Analyze the seed for Signal harmonic or Shannon entropy failures, if we're in a __TIMEOUT__
+    # (between keystrokes or after a major controls change).  Otherwise, if the seed's changed,
+    # request a __TIMEOUT__; when it invokes, perform the entropy analysis.
+    if status is None:
+        if event == '__TIMEOUT__':
+            seed_bytes		= codecs.decode( seed, 'hex_codec' )
+            scan_dur,(sigs,shan) = timing( scan_entropy, instrument=True )( seed_bytes, show_details=True )  # could be (None,None)
+            sigs_rate		= f"{rate_dB( max( sigs ).dB if sigs else None, what='Harmonics')}"
+            shan_rate		= f"{rate_dB( max( shan ).dB if shan else None, what='Shannon Entropy')}"
+            window['-SD-SEED-F-'].update( f"{SD_SEED_FRAME}; {sigs_rate}, {shan_rate}" )
+            disp_dur,analysis	= timing( display_entropy, instrument=True )( sigs, shan, what=f"{len(seed_bytes)*8}-bit Seed Source" )
+            update_seed_data.deficiencies = (sigs, shan)
+            update_seed_data.analysis = analysis or '(No entropy analysis deficiencies found in Seed Data)'
+            log.debug( f"Seed Data  Entropy Analysis took {scan_dur:.3f}s + {disp_dur:.3f}s == {scan_dur+disp_dur:.3f}s: {analysis}" )
+        elif changed:
+            log.info( f"Seed Data requests __TIMEOUT__ w/ current source: {update_seed_data.src!r}" )
+            values['__TIMEOUT__'] = .5
+    else:
+        window['-SD-SEED-F-'].update( f"{SD_SEED_FRAME}; Invalid" )
 
     # Since a window[...].update() doesn't show up to a .get() 'til the next cycle of the display,
     # we'll communicate updates to successive functions via values.
     values['-SD-SEED-'] 	= seed
     window['-SD-SEED-'].update( seed )
+
+    # Finally, remember what data/pswd/seed we're working on, in case we get a major controls change.
+    update_seed_data.was[update_seed_data.src] = data, pswd, seed
     return status
 
-update_seed_data.src		= None  # noqa: E305
+update_seed_data.src		= '-SD-BIP-'  # noqa: E305
 update_seed_data.was		= {
-    '-SD-BIP-':		(BIP39_EXAMPLE_128,""),
-    '-SD-BIP-SEED-':	(BIP39_EXAMPLE_128,""),
-    '-SD-SLIP-':	(SLIP39_EXAMPLE_128,""),
+    '-SD-BIP-':		(BIP39_EXAMPLE_128,  "", None),
+    '-SD-BIP-SEED-':	(BIP39_EXAMPLE_128,  "", None),
+    '-SD-SLIP-':	(SLIP39_EXAMPLE_128, "", None),
 }
+update_seed_data.deficiencies	= ()
+update_seed_data.analysis	= ''
 
 
 def stretch_seed_entropy( entropy, n, bits, encoding=None ):
     """To support the generation of a number of Seeds, each subsequent seed *must* be independent of
     the prior seed.  The Seed Data supplied (ie. recovered from BIP/SLIP-39 Mnemonics, or from fixed/random
     data) is of course unchanging for the subsequent seeds to be produced; only the "extra" Seed Entropy
     is useful for producing multiple sequential Seeds.  Returns the designated number of bits
@@ -648,71 +738,152 @@
         entropy			= hashlib.sha512( entropy ).digest()
     octets			= ( bits + 7 ) // 8
     assert len( entropy ) >= octets, \
         "Insufficient extra Seed Entropy provided for {ordinal(n+1)} {bits}-bit Seed"
     return entropy[:octets]
 
 
-def update_seed_entropy( window, values ):
+def update_seed_entropy( event, window, values ):
     """Respond to changes in the extra Seed Entropy, and recover/generate the -SE-SEED-.  It is
     expected to be exactly the same size as the -SD-SEED- data.  Stores the last known state of the
-    -SE-... radio buttons, updating visibilties on change.
+    -SE-... radio buttons, updating visibilities on change.
 
+    We analyze the entropy of the *input* data (as UTF-8), not the resultant entropy.
     """
-    dat				 = values['-SE-DATA-']
-    for src in [
+    SE_CONTROLS			= [
         '-SE-NON-',
         '-SE-HEX-',
         '-SE-SHA-',
-    ]:
+    ]
+    data			= values['-SE-DATA-']
+    try:
+        data_bytes		= data.encode( 'UTF-8' )
+    except Exception as exc:
+        status			= f"Invalid data {data!r}: {exc}"
+
+    for src in SE_CONTROLS:
         if values[src] and update_seed_entropy.src != src:
             # If selected radio-button for Seed Entropy source changed, save last source's working
             # data and restore what was, last time we were working on this source.
-            if update_seed_entropy.src:
-                update_seed_entropy.was[update_seed_entropy.src] = dat
-            dat			= update_seed_entropy.was.get( src, '' )
+            data		= update_seed_entropy.was.get( src, '' )
             update_seed_entropy.src = src
-            window['-SE-DATA-'].update( dat )
-            values['-SE-DATA-']	= dat
+            window['-SE-DATA-'].update( data )
+            values['-SE-DATA-']	= data
             if 'HEX' in update_seed_entropy.src:
                 window['-SE-DATA-T-'].update( "Hex digits: " )
             else:
                 window['-SE-DATA-T-'].update( "Die rolls, etc.: " )
 
+    # Evaluate the nature of the extra entropy, and place interpretation to analyze in data_bytes.
+    # Binary "hex" data should be neutral harmonically and in Shannon entropy.  However, some data
+    # such as dice rolls may exhibit restricted symbol values; try to deduce this case, restricting
+    # Shannon Entropy 'N' to binary (coin-flip) or 4, 6 and 10-sided dice.
     status			= None
-    seed_data			= values.get( '-SD-SEED-', window['-SD-SEED-'].get() )
-    bits			= len( seed_data ) * 4
-    log.debug( f"Computing Extra Entropy, for {bits}-bit Seed Data: {seed_data!r}" )
+    seed			= values.get( '-SD-SEED-', window['-SD-SEED-'].get() )
+    bits			= len( seed ) * 4
+
+    strides			= 8
+    overlap			= False
+    ignore_dc			= True
+    N				= None
+    interpretation		= 'Trust but Verify ;-'
+    log.debug( f"Computing Extra Entropy, for {bits}-bit Seed Data: {seed!r}" )
     if 'NON' in update_seed_entropy.src:
         window['-SE-DATA-F-'].update( visible=False )
         extra_entropy		= b''
     elif 'HEX' in update_seed_entropy.src:
         window['-SE-DATA-F-'].update( visible=True )
         try:
-            # 0-fill and truncate any supplied hex data to the desired bit length
-            extra_entropy	= stretch_seed_entropy( dat, n=0, bits=bits, encoding='hex_codec' )
+            # 0-fill and truncate any supplied hex data to the desired bit length, SHA-512 stretch
+            extra_entropy	= stretch_seed_entropy( data, n=0, bits=bits, encoding='hex_codec' )
         except Exception as exc:
-            status		= f"Invalid Hex {dat!r} for {bits}-bit extra seed entropy: {exc}"
+            status		= f"Invalid Hex {data!r} for {bits}-bit extra seed entropy: {exc}"
+        else:
+            data_bytes		= codecs.decode( f"{data:<0{bits // 4}.{bits // 4}}", 'hex_codec' )
+            interpretation	= "Hexadecimal Data"
+            strides		= None
+            overlap		= True
+            ignore_dc		= False
     else:
         window['-SE-DATA-F-'].update( visible=True )
         try:
             # SHA-512 stretch and possibly truncate supplied Entropy (show for 1st Seed)
-            extra_entropy	= stretch_seed_entropy( dat, n=0, bits=bits, encoding='UTF-8' )
+            extra_entropy	= stretch_seed_entropy( data, n=0, bits=bits, encoding='UTF-8' )
         except Exception as exc:
-            status		= f"Invalid data {dat!r} for {bits}-bit extra seed entropy: {exc}"
+            status		= f"Invalid data {data!r} for {bits}-bit extra seed entropy: {exc}"
+        if data and all( '0' <= c <= '9' for c in data ):
+            N			= {
+                '0':  2, '1':  2,				# Coin flips
+                '2':  6, '3':  6, '4':  6, '5':  6, '6':  6,    # 6-sided (regular) dice
+                '7': 10, '8': 10, '9': 10, 		 	# 10-sided (enter 0 for the 10 side)
+            }[max( data )]
+            interpretation	= f"{N}-sided Dice" if N > 2 else "Coin-flips/Binary"
 
-    # Compute the Seed Entropy as hex.  Will be 128-, 256- or 512-bit hex data.
+    # Compute the Seed Entropy as hex.  Will be 128-, 256- or 512-bit hex data.  Ensure
+    # extra_{bytes,entropy} are bytes and ASCII (hex, or -) respectively.
     if status or not extra_entropy:
-        extra_entropy		= '-' * (bits // 4)
+        extra_entropy		= '-' * ( bits // 4 )
+        extra_bytes		= b''
     elif type( extra_entropy ) is bytes:
-        extra_entropy		= codecs.encode( extra_entropy, 'hex_codec' ).decode( 'ascii' )
+        extra_bytes		= extra_entropy
+        extra_entropy		= codecs.encode( extra_bytes, 'hex_codec' ).decode( 'ascii' )
+    else:
+        extra_bytes		= codecs.decode( extra_entropy, 'hex_codec' )
+
+    if window['-SE-SEED-'].get() != extra_entropy:
+        update_seed_entropy.deficiencies = ()
+
+    se_seed_frame		= f"{SE_SEED_FRAME} ({interpretation})"
+    if status is None and len( data_bytes ) >= 8 and not update_seed_entropy.deficiencies:
+        if event == '__TIMEOUT__':
+            scan_dur,(sigs,shan) = timing( scan_entropy, instrument=True )(  # could be (None,None)
+                data_bytes,
+                strides		= strides,
+                overlap		= overlap,
+                ignore_dc	= ignore_dc,
+                N		= N,
+                signal_threshold = 300/100,
+                shannon_threshold = 10/100,
+                show_details	= True
+            )
+            sigs_rate		= f"{rate_dB( max( sigs ).dB if sigs else None, what='Harmonics')}"
+            shan_rate		= f"{rate_dB( max( shan ).dB if shan else None, what='Shannon Entropy')}"
+            window['-SE-SEED-F-'].update( f"{se_seed_frame}: {sigs_rate}, {shan_rate}" )
+            disp_dur,analysis	= timing( display_entropy, instrument=True )( sigs, shan, what=f"{len(extra_bytes)*8}-bit Extra Seed Entropy" )
+            update_seed_entropy.deficiencies = (sigs, shan)
+            update_seed_entropy.analysis = analysis or '(No entropy analysis deficiencies found in Extra Seed Entropy)'
+            log.debug( f"Seed Extra Entropy Analysis took {scan_dur:.3f}s + {disp_dur:.3f}s == {scan_dur+disp_dur:.3f}s: {analysis}" )
+        else:
+            log.info( f"Seed Extra requests __TIMEOUT__ w/ current source: {update_seed_entropy.src!r}" )
+            values['__TIMEOUT__'] = .5
+    elif status:
+        window['-SE-SEED-F-'].update( f"{se_seed_frame}: Invalid" )
+        update_seed_entropy.analysis = f"{se_seed_frame}: {status}"
+    elif len( data_bytes ) < 8:
+        window['-SE-SEED-F-'].update( f"{se_seed_frame}" )
+        update_seed_entropy.analysis = f"{se_seed_frame}: {'None Provided' if values['-SE-NON-'] else 'Insufficient for analysis'}"
+
     values['-SE-SEED-']		= extra_entropy
     window['-SE-SEED-'].update( extra_entropy )
-update_seed_entropy.src	= None  # noqa: E305
+
+    update_seed_entropy.was[update_seed_entropy.src] = data
+    return status
+
+update_seed_entropy.src	= '-SE-NON-'  # noqa: E305
 update_seed_entropy.was = {}
+update_seed_entropy.deficiencies = ()
+update_seed_entropy.analysis = ''
+
+
+def using_BIP39( values ):
+    return values['-AS-BIP-CB-']
+
+
+def BITS_allowed( values ):
+    return BITS_BIP39 if using_BIP39( values ) else BITS
 
 
 def compute_master_secret( window, values, n=0 ):
     """Validate the Seed Data and Seed Entropy, and compute the n'th master secret seed.  This is a
     simple XOR of the Seed Data, and any extra Seed Entropy -- so that the user can VISUALLY OBSERVE
     that the purported Seed Data and their provided extra Seed Entropy leads to the final master
     secret seed.  We are resilient to '-' in incoming seed_data (eg. from an incomplete BIP/SLIP-39
@@ -722,15 +893,15 @@
     cryptocurrency seed generation algorithm!
 
     This function must have knowledge of the extra Seed Entropy settings, so it inspects the
     -SE-{NON/HEX}- checkbox values.
     """
     seed_data_hex		= values.get( '-SD-SEED-', window['-SD-SEED-'].get() )
     bits			= len( seed_data_hex ) * 4
-    assert bits in BITS, \
+    assert bits in BITS_allowed( values ), \
         f"Invalid {bits}-bit Seed size: {seed_data_hex}"
     try:
         seed_data		= codecs.decode( seed_data_hex.replace( '-', '0' ), 'hex_codec' )
     except Exception as exc:
         raise ValueError( f"Invalid Seed hex data: {seed_data_hex}" ) from exc
     if values['-SE-NON-']:
         assert n == 0, \
@@ -862,15 +1033,15 @@
             for g in group or GROUPS
         )
     assert groups and all( isinstance( k, str ) and len( v ) == 2 for k,v in groups.items() ), \
         f"Each group member specification must be a '<group>': (<needs>, <size>) pair, not {type(next(groups.items()))}"
 
     group_threshold		= int( threshold ) if threshold else math.ceil( len( groups ) * GROUP_THRESHOLD_RATIO )
 
-    sg.CURRENT_LOOK_AND_FEEL = sg.theme( THEME )  # Why?  This module global should have updated...
+    sg.CURRENT_LOOK_AND_FEEL	= sg.theme( THEME )  # Why?  This module global should have updated...
 
     # Try to set a sane initial CWD (for saving generated files).  If we start up in the standard
     # macOS App's "Container" directory for this App, ie.:
     #
     #    /Users/<somebody>/Library/Containers/ca.kundert.perry.SLIP39/Data
     #
     # then we'll move upwards to the user's home directory.  If we change the macOS App's Bundle ID,
@@ -898,17 +1069,18 @@
     status_error		= False
     event			= False
     events_termination		= (sg.WIN_CLOSED, 'Exit',)
     events_ignored		= ('-MNEMONICS-'+sg.WRITE_ONLY_KEY,)
     master_secret		= None		# default to produce randomly
     details			= None		# The SLIP-39 details produced from groups; make None to force SLIP-39 Mnemonic update
     cryptopaths			= None
-    timeout			= 0		# First time thru; refresh immediately
+    timeout			= 0		# First time thru; refresh immediately; functions req. refresh may adjust via values['__TIMEOUT__']
     instructions		= ''		# The last instructions .txt payload found
     instructions_kwds		= dict()        # .. and its colors
+    values			= dict()
     while event not in events_termination:
         # A Controls layout selection, eg. '-LO-2-'; closes and re-generates window layout
         if event and event.startswith( '-LO-' ):
             controls		= int( event.split( '-' )[2] )
             window.close()
             window		= None
 
@@ -932,72 +1104,44 @@
                 printers	= None
 
             layout		= groups_layout(
                 names		= names,
                 group_threshold	= group_threshold,
                 groups		= groups,
                 cryptocurrency	= cryptocurrency,
-                passphrase	= passphrase,
+                passphrase	= passphrase.decode( 'UTF-8' ) if passphrase else None,
                 wallet_pwd	= wallet_pwd,
                 wallet_pwd_hint	= wallet_pwd_hint,
                 wallet_derive	= wallet_derive,
                 controls	= controls,
                 printers	= printers,
             )
             window		= sg.Window(
                 f"{', '.join( names )} SLIP-39 Mnemonic Cards",
                 layout,
                 finalize	= True,
                 grab_anywhere	= True,
                 no_titlebar	= no_titlebar,
                 scaling		= scaling,
             )
-            timeout		= 0 		# First time through w/ new window, refresh immediately
+            values['__TIMEOUT__'] = 0 		# First time through w/ new window, refresh immediately
 
-        # Block (except for first loop) and obtain current event and input values. Until we get a
-        # new event, retain the current status
+        # Block (except for first loop, or if someone requested a __TIMEOUT__) and obtain current
+        # event and input values. Until we get a new event, retain the current status
+        timeout			= values.get( '__TIMEOUT__', None )  # Subsequently, default; block indefinitely (functions may adjust...)
+        if timeout:
+            logging.debug( f"A __TIMEOUT__ was requested: {timeout!r}" )
         event, values		= window.read( timeout=timeout )
-        timeout			= None 		# Subsequently, default; block indefinitely
         logging.debug( f"{event}, {values}" )
         if not values or event in events_termination or event in events_ignored:
             continue
 
         status			= None
         status_error		= True
 
-        # See if there are any instructional 'SLIP-39-<event>.txt' for the last event.  If so, load
-        # it into the '-INSTRUCTIONS-' Multiline.  We'll split each event on its component '-', and
-        # look for eg. SLIP-39-LO.txt, when we see event == '-LO-1-'.  We'll select the most
-        # specific instructional .txt we can load.  Only if the current instructions is empty will
-        # we go all the way back to load the generic SLIP-39.txt.  If the event corresponds to an
-        # object with text/backround_color, use it in the instructional text.
-        txt_segs		= ( event or '' ).strip('-').split( '-' )
-        for txt_i in range( len( txt_segs ), 0 if instructions else -1, -1 ):
-            txt_name		= '-'.join( [ 'SLIP', '39' ] + txt_segs[:txt_i] ) + '.txt'
-            txt_path		= os.path.join( os.path.dirname( __file__ ), txt_name )
-            try:
-                with open( txt_path, 'r', encoding='utf-8' ) as txt_f:
-                    txt		= txt_f.read()
-                    if txt:
-                        instructions = txt
-                        break
-            except FileNotFoundError:
-                pass
-        if event.startswith( '-' ):  # One of our events (ie. not __TIMEOUT__, etc.)...
-            try:
-                event_element	= window.find_element( event, silent_on_error=True )
-                instructions_kwds.update(
-                    text_color	= event_element.TextColor,
-                    background_color= event_element.BackgroundColor,
-                )
-            except Exception as exc:
-                log.debug( f"Couldn't update instructions text color: {exc}" )
-                pass
-        window['-INSTRUCTIONS-'].update( instructions, **instructions_kwds )
-
         if event == '+' and len( groups ) < 16:
             # Add a SLIP39 Groups row (if not already at limit)
             g			= len( groups )
             name		= f"Group{g+1}"
             needs		= (2,3)
             groups[name] 	= needs
             window.close()
@@ -1023,31 +1167,113 @@
 
         # Attempt to compute the 1st Master Secret Seed, collecting any failure status detected.
         # Compute the Master Secret Seed, from the supplied Seed Data and any extra Seed Entropy.
         # We are displaying the 1st extra Seed Entropy, used to produce the first Seed, for the
         # first SLIP-39 encoding.
         master_secret_was	= window['-SEED-'].get()
         status_sd		= update_seed_data( event, window, values )
-        status_se		= update_seed_entropy( window, values )
+        status_se		= update_seed_entropy( event, window, values )
         status_ms		= None
         try:
             master_secret	= compute_master_secret( window, values, n=0 )
         except Exception as exc:
             status_ms		= f"Error computing master_secret: {exc}"
             logging.exception( f"{status}" )
             master_secret	= '-' * len( values['-SD-SEED-'] )
         if type(master_secret) is bytes:
             master_secret	= codecs.encode( master_secret, 'hex_codec' ).decode( 'ascii' )
 
+        # We've now calculated any supplied Seed Data or Seed Extra Randomness (and detected any
+        # Entropy Analysis deficiencies, which may be included in some instruction formats); see if
+        # there are any instructional 'SLIP-39-<event>.txt' for the last event.  If so, load it into
+        # the '-INSTRUCTIONS-' Multiline.  We'll split each event on its component '-', and look for
+        # eg. SLIP-39-LO.txt, when we see event == '-LO-1-'.  We'll select the most specific
+        # instructional .txt we can load.  Only if the current instructions is empty will we go all
+        # the way back to load the generic SLIP-39.txt.  If the event corresponds to an object with
+        # text/backround_color, use it in the instructional text.
+        txt_segs		= ( event or '' ).strip( '-' ).split( '-' )
+        instructions_path	= ''
+        for txt_i in range( len( txt_segs ), 0 if instructions else -1, -1 ):
+            txt_name		= '-'.join( [ 'SLIP', '39' ] + txt_segs[:txt_i] ) + '.txt'
+            txt_path		= os.path.join( os.path.dirname( __file__ ), txt_name )
+            try:
+                with open( txt_path, 'r', encoding='UTF-8' ) as txt_f:
+                    txt		= txt_f.read()
+                    if txt:
+                        instructions = txt
+                        instructions_path = txt_path
+                        break
+            except FileNotFoundError:
+                pass
+
+        # If there are {...} entries in the loaded text, we'll assume they are formatting options.
+        # These files form part of the program, and therefore can know about the names of internal
+        # variables.  If someone can exploit these .txt files, they can just as easily exploit the
+        # Python code of the program...  Let's provide access to an aggregate summary of the Entropy
+        # Analysis of the Seed Data and Seed Extra Randomness, here.  If we have some poor Seed
+        # Data, but provide good Seed Extra Randomness, or provide a BIP/SLIP-39 passphrase, then
+        # we'll let that go.  In other words, poor Seed Data with a Passphrase is considered more
+        # secure (still not recommended).  But, really bad Seed Data entropy can still overwhelm it.
+        def deficiency( *deficiencies ):
+            """Entropy analysis deficiencies may consists of eg. (,), (None,[]) or ([],[]).  Yields
+            the largest (first item) from each, if any.  Convert to a deficiency sequence.
+
+            """
+            for alist in deficiencies:
+                if alist:
+                    yield alist[0]
+        dB_defic		= []
+        sd_defic		= list( deficiency( *update_seed_data.deficiencies ))
+        if sd_defic:
+            # There is a Seed Data entropy deficit!
+            dB_defic.append( max( sd_defic ).dB )
+        if 'NON' not in update_seed_entropy.src:
+            # There is Seed Extra Randomness; is it also in entropy deficit?
+            se_defic		= list( deficiency( *update_seed_entropy.deficiencies ))
+            if dB_defic or se_defic:
+                # Some good Seed Extra Randomness dilutes poor Seed Data entropy deficit...
+                dB_defic.append( max( se_defic ).dB if se_defic else -1.0 )
+        if dB_defic and window['-PASSPHRASE-'].get():
+            # There's a deficit, but they're using an encryption Passphrase...
+            dB_defic.append( -1.0 )
+        # If None, "excellent", otherwise rating is avg of worst of Seed Data / Extra Entropy, net a
+        # reduction for passphrase and good Extra Entropy.  If entropy_dB is None (excellent), or <
+        # 0.0dB (ok), this is considered acceptable.
+        entropy_dB		= avg( dB_defic ) if dB_defic else None
+        entropy_rating		= rate_dB( entropy_dB )
+        ( log.warning if dB_defic else log.info )( f"Overall entropy deficiency: {entropy_rating}, from: {commas(dB_defic)}" )
+
+        window['-GROUPS-F-'].update( f"{SS_SEED_FRAME}: Overall entropy deficiency: {entropy_rating}" )
+        instructions_fmtd	= instructions
+        if '{' in instructions:
+            try:
+                kwds		= globals()
+                kwds.update( locals() )
+                instructions_fmtd = instructions.format( **kwds )
+            except KeyError as exc:
+                log.warning( f"Failed to format instructions {instructions_path}: Local variable {exc} not found." )
+
+        if event.startswith( '-' ):  # One of our events (ie. not __TIMEOUT__, etc.)...
+            try:
+                event_element	= window.find_element( event, silent_on_error=True )
+                instructions_kwds.update(
+                    text_color	= event_element.TextColor,
+                    background_color= event_element.BackgroundColor,
+                )
+            except Exception as exc:
+                log.debug( f"Couldn't update instructions text color: {exc}" )
+                pass
+        window['-INSTRUCTIONS-'].update( instructions_fmtd, **instructions_kwds )
+
         # See if we should display/use the BIP-39 version of the Master Secret Seed.  Also, re-labels
         # the -PASSPHRASE-... between SLIP-39 and BIP-39.  We only support one Passphrase, even if
         # SLIP-39 is encoding the entropy in a BIP-39 Mnemonic; If BIP-39 is selected, the
         # Passphrase is assumed to be encrypting the BIP-39 Mnemonic to generate the Seed; the same
         # Passphrase must be entered on the hardware wallet along with the Mnemonic.
-        using_bip39		= values['-AS-BIP-CB-']  # Also triggers BIP-39 Seed generation, below
+        using_bip39		= using_BIP39( values )  # Also triggers BIP-39 Seed generation, below
 
         # From this point forward, detect if we have seen any change in the computed Master Seed, or
         # in the SLIP-39 groups recovered; avoid unnecessary update of the SLIP-39 Mnemonics.  And,
         # if any status was reported in the computation of Seed Data, extra Seed Entropy or Master
         # Secret, report it now.  We'll also force this if someone clicks "Using BIP-39".  Remember
         # -- the BIP-39 Mnemonic encodes only the original Seed Entropy, so there is no concept of a
         # Passphrase.  Later, when we use the Entropy to produce wallets -- if "Using BIP-39" is
@@ -1074,16 +1300,16 @@
                 # The seed is BIP-39 compatible; give the option to indicating they're using BIP-39
                 window['-AS-BIP-CB-'].update( disabled=False )
             details		= None
 
         # Recover any passphrase, discarding any details on change.  The empty passphrase b'' is the
         # default for both SLIP-39 and BIP-39.
         window['-AS-BIP-'].update( visible=values['-AS-BIP-CB-'] )
-        window['-PASSPHRASE-L-'].update(
-            'BIP-39 passphrase:' if using_bip39 else 'SLIP-39 passphrase:' )
+        window['-PASSPHRASE-F-'].update(
+            'BIP-39 Passphrase' if using_bip39 else passphrase_trezor_incompatible )
         passphrase_now		= values['-PASSPHRASE-'].strip().encode( 'UTF-8' )
         if passphrase != passphrase_now:
             passphrase		= passphrase_now
             details		= None
 
         status			= status_sd or status_se or status_ms
         if status:
@@ -1246,25 +1472,32 @@
         # We have a complete SLIP-39 Mnemonic set.  If we get here, no failure status has been
         # detected, and SLIP39 mnemonic and account details { "name": <details> } have been created;
         # we can now save the PDFs; converted details is now { "<filename>": <details> })
         if wallet_pwd is not False:
             # And, if Paper Wallets haven't been disabled completely, remember our password/hint
             wallet_pwd		= values['-WALLET-PASS-']  # Produces Paper Wallet(s) iff set
             wallet_pwd_hint	= values['-WALLET-HINT-']
+
         if event in ('-SAVE-', '-PRINT-'):
             # A -SAVE- target directory has been selected; use it, if possible.  This is where any
             # output will be written.  It should usually be a removable volume, but we do not check.
             # An empty path implies the current directory.
             filepath,printer	= None,None
             if event == '-SAVE-':
                 filepath	= values['-SAVE-']
                 log.info( f"Saving to {filepath!r}..." )
             if event == '-PRINT-':
                 printer		= values['-PRINTER-']
                 log.info( f"Printing to {printer!r}..." )
+                # A bad Entropy Analysis results in a watermark, warning that the SLIP-39 Mnemonic Seed may
+                # be insecure.
+            if entropy_dB is None or entropy_dB < 0:
+                watermark	= None
+            else:
+                watermark	= f"Seed Entropy: {entropy_rating_dB( entropy_dB )}"
             try:
                 card_format	= next( c for c in CARD_SIZES if values[f"-CS-{c}-"] )
                 paper_format	= next( pf for pn,pf in PAPER_FORMATS.items() if values[f"-PF-{pn}-"] )
                 details		= write_pdfs(
                     names		= details,
                     using_bip39		= using_bip39,
                     card_format		= card_format,
@@ -1272,14 +1505,15 @@
                     cryptocurrency	= cryptocurrency,
                     edit		= edit,
                     wallet_pwd		= wallet_pwd,
                     wallet_pwd_hint	= wallet_pwd_hint,
                     wallet_format	= next( (f for f in WALLET_SIZES if values.get( f"-WALLET-SIZE-{f}-" )), None ),
                     filepath		= filepath,
                     printer		= printer,
+                    watermark		= watermark,
                 )
             except Exception as exc:
                 status		= f"Error saving PDF(s): {exc}"
                 logging.exception( f"{status}" )
                 continue
             name_len		= max( len( name ) for name in details )
             status		= '\n'.join(
```

### Comparing `slip39-9.0.4/slip39/layout/BNB.png` & `slip39-9.1.2/slip39/layout/BNB.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/BTC.png` & `slip39-9.1.2/slip39/layout/BTC.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/COVER-BIP-39.txt` & `slip39-9.1.2/slip39/layout/COVER-BIP-39.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-                             ______________
-
-                              USING BIP-39
-                             ______________
+                      ━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+                       SEED RECOVERY USING BIP-39
+                      ━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 
 
 SLIP-39 supports Hardware Wallets that require BIP-39 Mnemonics for Seed
 recovery, such as your Ledger Nano, etc.  Recover your BIP-39 Mnemonic
-phrase from these SLIP-39 cards using the App whenever you need it, to
+phrase from these cards using the SLIP-39 App whenever you need it, to
 restore your Cryptocurrency accounts to your hardware wallet.
 
-- Open the SLIP-39 App, and set Controls to "Recover"
-- In "Seed Source", use "SLIP-39" and input Mnemonics, with sufficient:
-  - Different Groups to satisfy Recovery Card Groups threshold
-  - Cards in each Group to meet each groups' recovery minimums
-- In "Seed & SLIP-39 Recover Groups", click "Using BIP-39"
-  - The BIP-39 Mnemonic will be recovered and displayed
-- Restore your Cryptocurrency accounts to your hardware wallet by
+• Open the SLIP-39 App, and set Controls to "Recover"
+• In "Seed Source", use "SLIP-39" and input Mnemonics, with sufficient:
+  • Different Groups to satisfy Recovery Card Groups threshold
+  • Cards in each Group to meet each groups' recovery minimums
+• In "Seed & SLIP-39 Recover Groups", click "Using BIP-39"
+  • The BIP-39 Mnemonic will be recovered and displayed
+• Restore your Cryptocurrency accounts to your hardware wallet by
   entering the BIP-39 Mnemonic phrase.
-- Tear off and Destroy this BIP-39 Mnemonic backup, once you are
+• Cut off and *destroy* this BIP-39 Mnemonic backup, once you are
   confident you can recover it at will!
+
+      NOTE: You cannot enter these SLIP-39 Mnemonics directly on a
+      BIP-39 Hardware Wallet to recover the Seed.  Use the SLIP-39
+      App to recover the BIP-39 Seed Phrase.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slip39-9.0.4/slip39/layout/COVER.txt` & `slip39-9.1.2/slip39/layout/COVER.txt`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/CRO.png` & `slip39-9.1.2/slip39/layout/CRO.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/DOGE.png` & `slip39-9.1.2/slip39/layout/DOGE.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/ETH.png` & `slip39-9.1.2/slip39/layout/ETH.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/LTC.png` & `slip39-9.1.2/slip39/layout/LTC.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/SLIP-39.png` & `slip39-9.1.2/slip39/layout/SLIP-39.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/XRP.png` & `slip39-9.1.2/slip39/layout/XRP.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/layout/__init__.py` & `slip39-9.1.2/slip39/recovery/entropy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1137 +1,1299 @@
-import ast
-import io
-import json
+# -*- mode: python ; coding: utf-8 -*-
+#
+# Python-slip39 -- Ethereum SLIP-39 Account Generation and Recovery
+#
+# Copyright (c) 2022, Dominion Research & Development Corp.
+#
+# Python-slip39 is free software: you can redistribute it and/or modify it under
+# the terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.  It is also available under alternative (eg. Commercial) licenses, at
+# your option.  See the LICENSE file at the top of the source tree.
+#
+# Python-slip39 is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+
+import cmath
+import codecs
 import logging
 import math
-import os
-import re
-import subprocess
-import sys
-import warnings
-
-from datetime		import datetime
-from collections	import namedtuple
-from collections.abc	import Callable
-
-from typing		import Dict, List, Tuple, Optional, Sequence, Any
-import qrcode
-from fpdf		import FPDF, FlexTemplate
-
-from ..api		import Account, cryptopaths_parser, create, enumerate_mnemonic, group_parser
-from ..util		import ordinal, chunker
-from ..recovery		import recover, produce_bip39
-from ..defaults		import (
-    FONTS, MNEM_ROWS_COLS, CARD, CARD_SIZES, PAPER, PAGE_MARGIN, MM_IN, PT_IN,
-    WALLET, WALLET_SIZES, COLOR,
-    GROUPS, GROUP_THRESHOLD_RATIO,
-    FILENAME_FORMAT,
-)
 
-# Optionally support output of encrypted JSON files
-eth_account			= None
 try:
-    import eth_account
+    from numpy		import fft as np_fft
 except ImportError:
-    pass
-
-log				= logging.getLogger( __package__ )
+    np_fft			= None
 
+from collections	import namedtuple, defaultdict
+from typing		import List, Union, Tuple, Optional, Callable, Sequence
 
-class Region:
-    """Takes authority for a portion of another Region, and places things in it, relative to its
-    upper-left and lower-right corners.
-
-    Attempts to create a sane priority hierarchy, because fpdf2's FlexTemplate sorts based on it.
-    If a specific priority is provided, it will be used.  However, if no priority is given, 0 will
-    be automatically assigned by FlexTemplate.  If sorting is unstable, this may result in an
-    unspecified ordering.
+from ..util		import mixed_fraction, ordinal, commas, is_power_of_2, avg, rms
 
-    """
-    def __init__( self, name, x1=None, y1=None, x2=None, y2=None, rotate=None, priority=None ):
-        self.name		= name
-        self.x1			= x1		# could represent positions, offsets or ratios
-        self.y1			= y1
-        self.x2			= x2
-        self.y2			= y2
-        self.rotate		= rotate
-        self.priority		= priority
-        self.regions		= []
-
-    @property
-    def h( self ):
-        return self.y2 - self.y1
-
-    @property
-    def w( self ):
-        return self.x2 - self.x1
-
-    def element( self ):
-        "Converts to mm.  Optionally returns a specified priority."
-        d			= dict(
-            name	= self.name,
-            x1		= self.x1 * MM_IN,
-            y1		= self.y1 * MM_IN,
-            x2		= self.x2 * MM_IN,
-            y2		= self.y2 * MM_IN,
-            rotate	= self.rotate or 0.0
-        )
-        if self.priority:
-            d['priority']	= self.priority
-        return d
+log				= logging.getLogger( __package__ )
 
-    def __str__( self ):
-        return f"({self.name:16}: ({float(self.x1):8}, {float( self.y1):8}) - ({float(self.x2):8} - {float(self.y2):8})"
 
-    def add_region( self, region ):
-        region.x1		= self.x1 if region.x1 is None else region.x1
-        region.y1		= self.y1 if region.y1 is None else region.y1
-        region.x2		= self.x2 if region.x2 is None else region.x2
-        region.y2		= self.y2 if region.y2 is None else region.y2
-        self.regions.append( region )
-        return region
-
-    def add_region_relative( self, region ):
-        region.x1		= self.x1 + ( region.x1 or 0 )
-        region.y1		= self.y1 + ( region.y1 or 0 )
-        region.x2		= self.x2 + ( region.x2 or 0 )
-        region.y2		= self.y2 + ( region.y2 or 0 )
-        self.regions.append( region )
-        return region
-
-    def add_region_proportional( self, region ):
-        region.x1		= self.x1 + self.w * ( 0 if region.x1 is None else region.x1 )
-        region.y1		= self.y1 + self.h * ( 0 if region.y1 is None else region.y1 )
-        region.x2		= self.x1 + self.w * ( 1 if region.x2 is None else region.x2 )
-        region.y2		= self.y1 + self.h * ( 1 if region.y2 is None else region.y2 )
-        self.regions.append( region )
-        return region
-
-    def square( self, maximum=None, justify=None ):
-        """Make a region square (of 'maximum' size), justifying it L/C/R, and/or T/M/B; default is Center/Middle"""
-        dims			= min( self.w, self.h )
-        if maximum:
-            dims		= min( dims, maximum )
-        justify			= ( justify or '' ).upper()
-        if 'L' in justify:
-            self.x2		= self.x1 + dims
-        elif 'R' in justify:
-            self.x1		= self.x2 - dims
-        else:  # 'C' is default
-            self.x1, self.x2	= self.x1 + ( self.w - dims ) / 2, self.x2 - ( self.w - dims ) / 2
-        if 'T' in justify:
-            self.y2		= self.y1 + dims
-        elif 'B' in justify:
-            self.y1		= self.y2 - dims
-        else:  # 'M' is default
-            self.y1, self.y2	= self.y1 + ( self.h - dims ) / 2, self.y2 - ( self.h - dims ) / 2
-        return self
-
-    def mm( self ):
-        "Dimensions as Coordinate( x, y ) in mm."
-        return Coordinate( self.w * MM_IN, self.h * MM_IN )
-
-    dimensions 			= mm
-
-    def elements( self ):
-        """Yield a sequence of { 'name': "...", 'x1': #,  ... }."""
-        if self.__class__ != Region:
-            yield self.element()
-        for r in self.regions:
-            for d in r.elements():
-                yield d
-
-
-class Text( Region ):
-    SIZE_RATIO			= 3/4
-
-    def __init__( self, *args, font=None, text=None, size=None, size_ratio=None, align=None, multiline=None,
-                  foreground=None, background=None, bold=None, italic=None, underline=None,
-                  **kwds ):
-        self.font		= font
-        self.text		= text
-        self.multiline		= multiline
-        self.size		= size
-        self.size_ratio		= size_ratio or self.SIZE_RATIO
-        self.align		= align
-        self.foreground		= foreground
-        self.background		= background
-        self.bold		= bold
-        self.italic		= italic
-        self.underline		= underline
-        super().__init__( *args, **kwds )
-
-    def element( self ):
-        d			= super().element()
-        d['type']		= 'T'
-        d['font']		= FONTS.get( self.font ) or self.font or FONTS.get( 'sans' )
-        line_height		= self.h * PT_IN  # Postscript point == 1/72 inch
-        d['size']		= self.size or ( line_height * self.size_ratio )  # No need for int(round(..))
-        if self.text is not None:
-            d['text']		= self.text
-        if self.bold:
-            d['bold']		= True
-        if self.italic:
-            d['italic']		= True
-        if self.underline:
-            d['underline']	= True
-        if self.align is not None:
-            d['align']		= self.align
-        if self.multiline is not None:
-            d['multiline']	= bool( self.multiline )
-        if self.foreground is not None:
-            d['foreground']	= self.foreground
-        if self.background is not None:
-            d['background']	= self.background
-        return d
-
-
-class Image( Region ):
-    def __init__( self, *args, font=None, text=None, size=None, **kwds ):
-        self.font		= font
-        self.text		= text
-        self.size		= None
-        super().__init__( *args, **kwds )
-
-    def element( self ):
-        d			= super().element()
-        d['type']		= 'I'
-        return d
-
-
-class Line( Region ):
-    def emit( self, d, *args, **kwds ):
-        d['type']		= 'L'
-        super().emit( *args, **kwds )
-
-
-class Box( Region ):
-    def element( self ):
-        d			= super().element()
-        d['type']		= 'B'
-        return d
-
-
-Coordinate			= namedtuple( 'Coordinate', ('x', 'y') )
-
-
-def layout_card(
-    card_size: Coordinate,
-    card_margin: int,
-    num_mnemonics: int	= 20,
-):
-    card			= Box( 'card', 0, 0, card_size.x, card_size.y )
-    card_interior		= card.add_region_relative(
-        Region( 'card-interior', x1=+card_margin, y1=+card_margin, x2=-card_margin, y2=-card_margin )
-    )
-    for c_n in range( 16 ):  # SLIP-39 supports up to 16 groups
-        card_interior.add_region_proportional( Text(
-            f'card-g{c_n}', x1=1/8, y1=-1/16, x2=7/8, y2=5/16,
-            foreground	= int( COLOR[c_n % len( COLOR )], 16 ),
-            rotate	= -45,
-        ))
-    card_interior.add_region_proportional( Text(
-        'card-link', x1=2/8, y1=-2/32, x2=8/8, y2=4/32,
-        foreground	= int( COLOR[-1], 16 ),
-        rotate		= -45,
-        align		= 'C'
-    ))
-    card_top			= card_interior.add_region_proportional(
-        Region( 'card-top', x1=0, y1=0, x2=1, y2=1/4 )
-    )
-    card_bottom			= card_interior.add_region_proportional(
-        Region( 'card-bottom', x1=0, y1=1/4, x2=1, y2=1 )
-    )
-    card_mnemonics		= card_bottom.add_region_proportional(
-        Region( 'card-mnemonics', x1=0, y1=0, x2=13/16, y2=1 )
-    )
+def fft( x ):
+    """Computes frequency bin amplitude (real) and phase (imaginary) for N/2 frequency bins
+    0,..,Nyquist, for an N-sampled signal.  Uses numpy.fft.fft if available, otherwise, pfft where N
+    is a power of 2, dft for other N.
 
-    # QR codes sqaare, and anchored to top and bottom of card.
-    card_bottom.add_region_proportional(
-        Image( 'card-qr1', x1=13/16, y1=0, x2=1, y2=1/2 )
-    ).square( justify='TR' )
-    card_bottom.add_region_proportional(
-        Image( 'card-qr2', x1=13/16, y1=1/2, x2=1, y2=1 )
-    ).square( justify='BR' )
+    """
+    if np_fft:
+        return [ complex(b) for b in np_fft.fft( x ) ]
+    N				= len( x )
+    if not is_power_of_2( N ):
+        return dft( x )
+    return pfft( x )
+
+
+def ifft( y: List[complex] ) -> List[complex]:
+    """Compute inverse FFT for any complex bins N (ideally a power of 2, or multiple of 2."""
+    if np_fft:
+        return [ complex(s) for s in np_fft.ifft( y ) ]
+    return idft( y )
+
+
+def pfft( x ):
+    """A simple pure-python FFT"""
+    N				= len( x )
+    if N <= 1:
+        return x
+    even			= pfft( x[0::2] )
+    odd				= pfft( x[1::2] )
+    T				= [ cmath.exp( -2j * cmath.pi * k / N ) * odd[k] for k in range( N//2 ) ]
+    return [even[k] + T[k] for k in range(N//2)] + \
+           [even[k] - T[k] for k in range(N//2)]
+
+
+def dft( x: List[Union[int, float, complex]] ) -> List[complex]:
+    """Takes N either real or complex signal samples, yields complex DFT bins.  Assuming the input
+    waveform is filtered to only contain signals in the bandwidth B range -B/2:+B/2 around baseband
+    frequency MID, and is frequency shifted (divided by) your baseband frequency MID, and is sampled
+    at the Nyquist rate R: given N samples, the result contains N signal frequency component bins:
+
+        index:      0                 N/2-1      N/2      N/2+1       N-1
+        baseband:  [MID+] [MID+] ... [MID+]    [MID+/-]  [MID+]  ... [MID+]
+        frequency:  DC     1B/N   (N/2-1)B/N   (N/2)B/N  (1-N/2)B/N  -1B/N
 
-    card_top.add_region_proportional(
-        Text( 'card-title', x1=0, y1=0, x2=1, y2=40/100, bold=True )
-    )
-    card_top.add_region_proportional(
-        Text( 'card-requires', x1=0, y1=40/100, x2=1, y2=66/100, align='C', italic=True )
-    )
-    card_top.add_region_proportional(
-        Text( 'card-crypto1', x1=0, y1=66/100, x2=1, y2=83/100, align='R' )
-    )
-    card_top.add_region_proportional(
-        Text( 'card-crypto2', x1=0, y1=83/100, x2=1, y2=100/100, align='R' )
-    )
+    """
+    N				= len( x )
+    result			= []
+    for k in range( N ):
+        r			= 0
+        for n in range( N ):
+            t			= -2j * cmath.pi * k * n / N
+            r		       += x[n] * cmath.exp( t )
+        result.append( r )
+    return result
 
-    assert num_mnemonics in MNEM_ROWS_COLS, \
-        f"Invalid SLIP-39 mnemonic word count: {num_mnemonics}"
-    rows,cols		= MNEM_ROWS_COLS[num_mnemonics]
-    for r in range( rows ):
-        for c in range( cols ):
-            card_mnemonics.add_region_proportional(
-                Text(
-                    f"mnem-{c * rows + r}",
-                    x1		= c/cols,
-                    y1		= r/rows,
-                    x2		= (c+1)/cols,
-                    y2		= (r+1)/rows,
-                    font	= 'mono',
-                    size_ratio	= 9/16,
-                )
-            )
 
-    return card
+def idft( y: List[complex] ) -> List[complex]:
+    """Inverse DFT on complex frequency bins.  Very slow O(N^2), so use ... carefully.
 
+    Since we're likely to use this a lot for the same values of N, we'll memoize the constants we
+    use for multiplying.
 
-def layout_wallet(
-    wallet_size: Coordinate,
-    wallet_margin: int,
-):
-    """Produce a template format for a Paper Wallet.
-
-    Sets priority:
-      -3     : Hindmost backgrounds
-      -2     : Things atop background, but beneath contrast-enhancement
-      -1     : Contrast-enhancing partially transparent images
-       0     : Text, etc. (the default)
     """
-    prio_backing		= -3
-    prio_normal			= -2
-    prio_contrast		= -1
-
-    wallet			= Box( 'wallet', 0, 0, wallet_size.x, wallet_size.y )
-    wallet_background		= wallet.add_region_proportional(  # noqa: F841
-        Image( 'wallet-bg', priority=prio_backing ),
-    )
-
-    # Most of the Paper Wallet is visible (contains public address information).  The right-most
-    # portion can be folded over, and displays private key information
-    show			= wallet.add_region_proportional(
-        Region( 'wallet-show', x2=5/8 )
-    )
-    fold			= wallet.add_region_proportional(
-        Box( 'wallet-fold', x1=5/8 )
-    )
+    N				= len( y )
+    #assert N <= 170, f"idft: {N=} too large."  # 512-bit entropy as 3-bit symbols
+    e_sk_N			= idft.e_sk.setdefault( N, [] )
+    if e_sk_N:
+        e_sk_N_i		= iter( e_sk_N )
+        result			= [
+            sum(
+                y_k * e_sk
+                for y_k,e_sk in zip( y, e_sk_N_i )
+            ) / N+0j
+            for n in range( N )
+        ]
+    else:
+        #print( f"idft: Memoizing {N=} multiplication factors" )
+        result			= []
+        for n in range( N ):
+            r			= 0
+            s			= 2j * cmath.pi * n / N
+            for k in range( N ):
+                e_sk		= cmath.exp( s * k )
+                e_sk_N.append( e_sk )
+                r	       += y[k] * e_sk
+            r		       /= N+0j
+            result.append( r )
+    return result
+idft.e_sk			= {}  # noqa: E305
+
+
+def dft_magnitude( bins: Sequence[complex] ) -> List[float]:
+    return [ abs( b ) for b in bins ]
+
+
+def dft_normalize( bins: Sequence[complex] ) -> List[float]:
+    N				= len( bins )
+    assert N % 2 == 0, \
+        "Only even numbers of DFT bins are supported, not {len(x)}"
+    scale			= math.log( N, 2 )
+    return [ b / scale for b in bins ]
+
+
+def dft_to_rms_mags( bins: List[complex] ) -> List[float]:
+    """Compute the real-valued magnitudes of the provided complex-valued DFT bins.  Since real samples
+    cannot distinguish between a +1Hz and a -1Hz signal, the bins assigned to all intervening
+    frequencies between the DC and max bins must be combined.
+
+    Only even numbers of bins are supported.  The resultant number of DFT bins is N/2+1, ordered
+    from DC to max.
+
+    And, while we're at it, we'll normalize the scale so that DFTs of one number of bins is
+    comparable to another; they are scaled at a rate of sqrt(N).  This makes the RMS energy and
+    magnitudes on DFTs of different sizes comparable with eachother.
 
-    public			= show.add_region_relative(
-        Region( 'wallet-public', x1=+wallet_margin, y1=+wallet_margin, x2=-wallet_margin, y2=-wallet_margin )
-    )
-    private			= fold.add_region_relative(
-        Region( 'wallet-private', x1=+wallet_margin, y1=+wallet_margin, x2=-wallet_margin, y2=-wallet_margin )
-    )
+    """
+    N				= len( bins )
+    mags			= dft_magnitude( bins )
+    norm			= dft_normalize( mags )
+    nrms			= rms( norm )
+    for i in range( 1, N//2 ):
+        norm[i]		       += norm[-i]
+        norm[-i]		= 0.0
+    return nrms, norm[:N//2+1]
+
+
+def dft_on_real( bins ):
+    nrms, mags			= dft_to_rms_mags( bins )
+    return mags
+
+
+def denoise_mags( mags, threshold, middle=None, stride=8 ):
+    """Look for top signals within the given magnitudes.  This involves finding a noise floor within the
+    magnitude bins w/ a signal level threshold x above the noise floor.  We'll compute the SNR of
+    each signal by iteratively scaling the largest signals down to the average, and then look for
+    new signals that have risen above the new (lower) noise-floor avg.  Stops when the remaining
+    bins are below the avg * threshold.
 
-    # Assign each different Crypto name a different color, in template labels crypto-{f,b}1, crypto-{f,b}2, ...
-    for c_n in range( len( COLOR )):
-        public.add_region_proportional(
-            Text( f'crypto-f{c_n}', x1=1/8, y1=-1/16, x2=7/8, y2=7/16, foreground=int( COLOR[c_n], 16 ), rotate=-45, priority=prio_normal )
-        )
-        private.add_region_proportional(
-            Text( f'crypto-b{c_n}', x1=2/8, y1=-1/16, x2=7/8, y2=7/16, foreground=int( COLOR[c_n], 16 ), rotate=-45, priority=prio_normal )
-        )
+    Returns the noise threshold target, and list of the top mags: (target, [ (snr,index), ... ])
 
-    # The background rosette and cryptocurrency symbol in the center
-    public_center_size		= min( public.w, public.h )
-    public.add_region(
-        Image(
-            'center',
-            x1		= public.x1 + public.w * 2/3 - public_center_size / 3,
-            y1		= public.y1 + public.h * 1/2 - public_center_size / 3,
-            x2		= public.x1 + public.w * 2/3 + public_center_size / 3,
-            y2		= public.y1 + public.h * 1/2 + public_center_size / 3,
-        )
-    )
+    """
+    snrs			= set()
+    curs			= mags[:]
+    cavg			= avg( curs ) if middle is None else middle( curs )
+    target			= cavg * threshold
+    while peaks := set(
+            i
+            for i,m in enumerate( curs )
+            if i not in snrs and m >= target
+    ):
+        # There are 1 or more new peaks above the middle curs 'cavg' value.  Note that they are
+        # candidate signals in snrs.
+        snrs.update( peaks )
+        # Replace each signal with the current cavg * threshold 'target'.  This lowers the "avg"
+        # noise level by removing the signal portion of the now recognized signal bins; only the
+        # remaining non-signal portion of the signal candidate bins and the remaining non-gisnal
+        # bins influence the new cavg.
+        curs			= [
+            target if i in snrs else b
+            for i, b in enumerate( mags )
+        ]
+        cavg			= avg( curs ) if middle is None else middle( curs )
+        target			= cavg * threshold
+        #print( f"dnoi: {' '.join( f'{c:{stride}.1f}({mags[i] / target:{stride-2}.1f})' for i,c in enumerate( curs ))}: {target=:7.1f}" )
+
+    # Return the noise threshold target magnitude deduced, and the index,SNR for each signal bin,
+    # sorted by SNR
+    return target, sorted( ( (i, mags[i] / target) for i in snrs ), key=lambda e: e[1], reverse=True )
+
+
+def signal_recover_real( dfts, scale=None, integer=False, amplify=None ):
+    """Recover a real signal from the provided DFT output.  Optionally, scale the DFT before
+    recovering the signal.  Optionally, round the values to integer (eg. if the original signal was
+    integer).
 
-    # Public addresses are vertical on left- and right-hand of public Region.  In order to fit the
-    # longer ETH addresses into a space with a fixed-width font, we know that the ratio of the width
-    # to the height has to be about 1/20.  Rotation is downward around upper-left corner; so,
-    # lower-left corner will shift 1 height leftward and upward; so start 1 height right and down.
-    address_length		= public.h
-    address_height		= address_length * 1/20
-    public.add_region(
-        Image(
-            'address-l-bg',
-            x1		= public.x1 + address_height,
-            y1		= public.y1,
-            x2		= public.x1 + address_height + address_length,
-            y2		= public.y1 + address_height,
-            rotate	= -90,
-            priority	= prio_contrast,
-        )
-    ).add_region(
-        Text(
-            'address-l',
-            font	= 'mono',
-            rotate	= -90,
-        )
-    )
+    """
+    #print( "dfts: " + ' '.join( f"{d:{stride*2}.1f}" for d in dfts ))
+    assert scale in (None, 0, 1) or scale % 2 == 0, \
+        f"Only even multiples of a DFT are valid, not x{scale}"
+    while ( scale or 1 ) >= 2:
+        scale		      //= 2
+        N			= len( dfts )
+        # When doubling the length of a DFT, we have to scale each entry by 2x
+        dfts			= [d*2 for d in dfts]
+        # Insert N entries in the middle
+        dfts			= dfts[:N//2] + [0j] * N + dfts[N//2:]
+        # Split the high-frequency bin from the old DFT between the 2 new lower frequency bins.  Was
+        # in position [N//2+1], or also [-N//2]; now is stil in the position [-N//2], since N is
+        # still the old DFT size!  The corresponding location is at dft[N//2]; this will always be a
+        # freshly added 0+0j bin.
+        dfts[-N//2]	       /= 2
+        dfts[N//2]	       += dfts[-N//2]
+    #print( "dfts: " + ' '.join( f"{d:{stride*2}.1f}" for d in dfts ))
+    sigR			= ifft( dfts )
+    #print( "sigR: " + ' '.join( f"{s:{stride*2}.1f}" for s in sigR ))
+    sigR			= [ s.real for s in sigR ]
+    #print( "sigR: " + ' '.join( f"{s:{stride*2}.1f}" for s in sigR ))
+    if amplify:
+        sigR			= [s * amplify for s in sigR]
+    if integer:
+        sigR			= list( map( int, map( round, sigR )))
+        #print( "sigR: " + ' '.join( f"{s:{stride*2}}" for s in sigR ))
+    return sigR
+
+
+def signal_draw( s, scale=None, neg=None, pos=None ):
+    """Draws a single-line signed waveform if pos/neg is None, or the +'ve/-'ve half
+    of a waveform.  Default scale is 1 signed byte.
+
+        default:    "'‾~_.,._~‾'
+        pos:                     ,._~‾'"'‾~_.,
+        neg:        "'‾~_.,._~‾'"
 
-    # Rotation is upward around the upper-left corner, so lower-left corner will shift 1 height
-    # upward and right; so start 1 height leftward and down.
-    public.add_region(
-        Image(
-            'address-r-bg',
-            x1		= public.x2 - address_height,
-            y1		= public.y2,
-            x2		= public.x2 - address_height + address_length,
-            y2		= public.y2 + address_height,
-            rotate	= +90,
-            priority	= prio_contrast,
-        )
-    ).add_region(
-        Text(
-            'address-r',
-            font	= 'mono',
-            rotate	= +90,
-        )
-    )
+    """
+    if neg is True or pos is False:
+        return " \"'‾~_.,"[max( -1, min( 6, int( (-s-1) * 7 // ( scale or 128 )))) + 1]
+    elif pos is True or neg is False:
+        return " ,._~‾'\""[max( -1, min( 6, int(   s    * 7 // ( scale or 128 )))) + 1]
+    else:
+        return ",._~‾'\"" [max( -3, min( 3, round( s    * 7  / ( scale or 256 )))) + 3]
 
-    # Wallet name, amount
-    public.add_region_proportional(
-        Text( 'name-label',	x1=1/16, y1=0/16, x2=4/16, y2=1/16 )
-    )
-    public.add_region_proportional(
-        Image( 'name-bg',	x1=4/16, y1=0/16, x2=15/16, y2=1/16, priority=prio_contrast )
-    )
-    public.add_region_proportional(
-        Text( 'name',		x1=4/16, y1=0/16, x2=15/16, y2=1/16 )
-    )
 
-    public.add_region_proportional(
-        Text( 'amount-label',	x1=1/16, y1=3/16, x2=4/16, y2=1/16 )
-    )
-    public.add_region_proportional(
-        Image( 'amount-bg',	x1=4/16, y1=0/16, x2=15/16, y2=1/16, priority=prio_contrast )
-    )
-    public.add_region_proportional(
-        Text( 'amount',		x1=4/16, y1=0/16, x2=15/16, y2=1/16 )
-    )
+if __name__ == "__main__":
+    x				= [ 2, 3, 5, 7, 11 ]
+    print( "vals:   " + ' '.join( f"{f:11.2f}" for f in x ))
+    y				= fft( x )
+    print( "DFT:    " + ' '.join( f"{f:11.2f}" for f in y ))
+    z				= ifft( y )
+    print( "inverse:" + ' '.join( f"{f:11.2f}" for f in z ))
+    print( " - real:" + ' '.join( f"{f.real:11.2f}" for f in z ))
+
+    N				= 8
+    print( f"Complex signals, 1-4 cycles in {N} samples; energy into successive DFT bins" )
+    for rot in (0, 1, 2, 3, -4, -3, -2, -1):  # cycles; and bins in ascending index order
+        if rot > N/2:
+            print( "Signal change frequency exceeds sample rate and will result in artifacts" )
+        sigs                    = [
+            # unit-magnitude complex samples, rotated through 2Pi 'rot' times, in N steps
+            cmath.rect(
+                1, cmath.pi*2*rot/N*i
+            )
+            for i in range( N )
+        ]
+        print( f"{rot:2} cycle" + ' '.join( f"{f:11.2f}" for f in sigs ))
+        dfts                    = fft( sigs )
+        print( "  DFT:  " + ' '.join( f"{f:11.2f}" for f in dfts ))
+        print( "   ABS: " + ' '.join( f"{abs(f):11.2f}" for f in dfts ))
+
+
+# dB <-> ratio calculations.  Default dB definitions are in terms of
+# power.  However, most measured values are of fields (eg. voltages).
+dB_type_kwds = {
+    'power': {              # eg. Antenna dBi gain
+        'base':   10.0,
+        'factor': 10.0,
+    },
+    'field': {              # eg. Amplifier voltage gain
+        'base':   10.0,
+        'factor': 20.0,
+    },
+    'sensed':  {            # eg. Loudness sensation gain
+        'base':    2.0,
+        'factor': 10.0,
+    },
+}
+
+
+# dB <-> ratio (for power, by default).  If reference is 1 (default),
+# then the value is a ratio.  Otherwise, the 'dB' of the 'value'
+# vs. the 'reference' value is computed.  This is the definition of
+# dB, so deals in terms of Power (Energy) values by default.
+def value_from_dB( dB, reference=1, base=10.0, factor=10.0 ):
+    return base ** ( dB / factor ) * reference
+
+
+def dB_from_value( ratio, reference=1, base=10.0, factor=10.0 ):
+    """Convert a ratio [0,oo) into a dB range (-oo,oo), where the ratio 1.0 == 0.0dB.  A -'ve or 0
+    is invalid, and tends to -oo (negative infinity).
 
-    # Make Public QR Code square w/ min of height, width, anchored at lower-left corner
-    public.add_region_proportional(
-        Text( 'address-qr-t',	x1=1/16, y1=5/16, x2=1, y2=6/16 )
-    )
-    public_qr			= public.add_region_proportional(
-        Image( 'address-qr-bg',	x1=1/16, y1=6/16, x2=1, y2=15/16 )
-    ).square( justify='BL' )
-    public_qr.add_region(
-        Image( 'address-qr' )
-    )
+    """
+    if reference and reference != 1:
+        ratio		       /= reference
+    if ratio > 0:
+        return factor * math.log( ratio, base )
+    return -math.inf
 
-    public.add_region_proportional(
-        Text( 'address-qr-b',	x1=1/16, y1=15/16, x2=1, y2=16/16 )
-    )
-    public_qr_r			= public.add_region_proportional(
-        Text( 'address-qr-r',	x1=1/16, y1=6/16, x2=1, y2=7/16, rotate=-90 )
-    )
-    public_qr_r.x1	       += public_qr.w + public_qr_r.h
-    public_qr_r.x2	       += public_qr.w
 
-    # Private region
+# dB <-> value (for field values, by default).  This is the practical
+# dB, so by default deals in measured values, which are usually Field
+# strength measurements (eg. Voltage, Sound Pressure, ...)
+def from_dB( dB, reference=1, dB_type='field' ):
+    return value_from_dB( dB=dB, reference=reference, **dB_type_kwds[dB_type] )
 
-    private.add_region_proportional(
-        Text( 'private-qr-t',	x1=0/16, y1=5/16, x2=1, y2=6/16 )
-    )
-    # QR code at most 5/8 the width, to retain sufficient space for large Ethereum encrypted JSON
-    # wallet private keys
-    private_qr			= private.add_region_proportional(
-        Image( 'private-qr-bg',	x1=0/16, y1=6/16, x2=1, y2=15/16, priority=prio_contrast )
-    ).square( maximum=private.w * 5 / 8, justify='BL' )
-    private_qr.add_region(
-        Image( 'private-qr' )
-    )
-    private.add_region_proportional(
-        Text( 'private-qr-b',	x1=0/16, y1=15/16, x2=1, y2=16/16 )
-    )
 
-    # Hint above; but same computed width as private_qr
-    private_h_t			= private.add_region_proportional(
-        Text( 'private-hint-t',	x1=0/16, y1=0/16, x2=1, y2=1/16 )
-    )
-    private_h_t.x2		= private_qr.x2
-    private_h_bg		= private.add_region_proportional(
-        Image( 'private-hint-bg',x1=0/16, y1=1/16, x2=1, y2=4/16, priority=prio_contrast )
-    )
-    private_h_bg.x2		= private_qr.x2
-    private_h			= private.add_region_proportional(
-        Text( 'private-hint',	x1=0/16, y1=1/16, x2=1, y2=3/16 )
-    )
-    private_h.x2		= private_qr.x2
+def into_dB( ratio, reference=1, dB_type='field' ):
+    return dB_from_value( ratio=ratio, reference=reference, **dB_type_kwds[dB_type] )
 
-    # We'll use the right side of the private region, each line rotated 90 degrees down and right.
-    # So, we need the upper-left corner of the private-bg anchored at the upper-right corner of
-    # private.
-    private_length		= private.h                     # line length is y-height
-    private_fontsize		= 6.5				# points == 1/72 inch
-    private_height		= private.x2 - private_qr.x2 - .05
-    private_lineheight		= private_fontsize / PT_IN / Text.SIZE_RATIO * .9  # in.
-
-    private.add_region(
-        Image(
-            'private-bg',
-            x1		= private.x2,
-            y1		= private.y1,
-            x2		= private.x2 + private_length,
-            y2		= private.y1 + private_height,
-            rotate	= -90,
-            priority	= prio_contrast,
-        )
-    )
-    # Now, add private key lines down the edge from right to left, rotating each into place
-    for ln in range( int( private_height // private_lineheight )):
-        private.add_region(
-            Text(
-                f"private-{ln}",
-                font	= 'mono',
-                x1	= private.x2 - private_lineheight * ln,
-                y1	= private.y1,
-                x2	= private.x2 + private_length,
-                y2	= private.y1 + private_lineheight,
-                size	= private_fontsize,
-                rotate	= -90,
-            )
-        )
 
-    return wallet
+class Signal( namedtuple('Signal', [ 'dB', 'stride', 'symbols', 'offset', 'details' ] )):
+    """Provide details on the location of symbols that seem to indicate a reduction in entropy.
 
+    dB:		signal to noise ratio; higher indicates worse entropy (more signal or pattern)
+    details:	A textual description of the signal
+    """
+    def __str__( self ):
+        return f"{self.dB:7.2f}dB, at {self.offset=:3}: {self.symbols:2} x {self.stride:2} bits/symbol: {self.details}"
 
-def layout_components(
-    pdf: FPDF,
-    comp_dim: Coordinate,
-    page_margin_mm: float	= .25 * MM_IN,   # 1/4" in mm.
-) -> Tuple[int, Callable[[int],[int, Coordinate]]]:
-    """Compute the number of components per pdf page, and a function returning the page # and
-    component (x,y) for the num'th component."""
-
-    # FPDF().epw/.eph is *without* page margins, but *with* re-orienting for portrait/landscape
-    # Allow 5% bleed over into page margins (to allow for slight error in paper vs. comp sizes)
-    comp_cols			= int(( pdf.epw - page_margin_mm * 2 * 95/100 ) // comp_dim.x )
-    comp_rows			= int(( pdf.eph - page_margin_mm * 2 * 95/100 ) // comp_dim.y )
-    comps_pp			= comp_rows * comp_cols
-
-    def page_xy( num ):
-        """Returns the page, and the coordinates within that page of the num'th component"""
-        page,nth		= divmod( num, comps_pp )
-        page_rows,page_cols	= divmod( nth, comp_cols )
-        offsetx			= page_margin_mm + page_cols * comp_dim.x
-        offsety			= page_margin_mm + page_rows * comp_dim.y
-        log.debug( f"{ordinal(num)} {comp_dim.x:7.5f}mm x {comp_dim.y:7.5f}mm component on page {page}, offset {offsetx:7.5f}mm x {offsety:7.5f}mm" )
-        return (page, Coordinate( x=offsetx, y=offsety ))
-
-    return (comps_pp, page_xy)
-
-
-def layout_pdf(
-        card_dim: Coordinate,                   # mm.
-        page_margin_mm: float	= .25 * MM_IN,  # 1/4" in mm.
-        orientation: str	= 'portrait',
-        paper_format: Any	= PAPER         # Can be a paper name (Letter) or (x, y) dimensions in mm.
-) -> Tuple[int, str, Callable[[int],[int, Coordinate]], FPDF]:
-    """Find the ideal orientation for the most cards of the given dimensions.  Returns the number of
-    cards per page, the FPDF, and a function useful for laying out templates on the pages of the
-    PDF."""
-    pdf				= FPDF(
-        orientation	= orientation,
-        format		= paper_format,
-    )
-    pdf.set_margin( 0 )
 
-    cards_pp,page_xy		= layout_components(
-        pdf, comp_dim=card_dim, page_margin_mm=page_margin_mm
-    )
-    return cards_pp, orientation, page_xy, pdf
+def entropy_bin_ints( entropy_bin, offset, symbols, stride, cancel_dc=None ):
+    length			= len( entropy_bin )
+    bits			= [
+        entropy_bin[off:off+stride]
+        for off in range( offset, length - stride + 1, stride )
+    ][:symbols]
+    ints			= [ int( b, 2 )  for b in bits ]
+    if cancel_dc:
+        ints			= [ r - 2**(stride-1) for r in ints ]
+    # print( "bits: " + ' '.join( f"{b:{stride*2}}" for b in bits ))
+    # print( "ints: " + ' '.join( f"{r:{stride*2}}" for r in ints ))
+    return ints
+
+
+def entropy_bin_dfts( entropy_bin, offset, symbols, stride, cancel_dc=True ):
+    """Compute the frequency bin magnitudes for 'stride'-bits x symbols starting at bit 'offset'.
+    If cancel_dc, shifts the numeric zero from bit value '00...' to '10...'; if the values are
+    randomly distributed, the DC offset should be cancelled out.
 
+    """
+    sigs			= entropy_bin_ints( entropy_bin, offset=offset, symbols=symbols, stride=stride,
+                                                    cancel_dc=cancel_dc )
+    #print( "sigs: " + ' '.join( f"{s:{stride*2}}" for s in sigs ))
+    dfts			= fft( sigs )
+
+    # See if we can observe any signal/noise ratio on any frequency
+    #print( "dfts: " + ' '.join( f"{d:{stride*2}.1f}" for d in dfts ))
+    return dfts
+
+
+def int_decode( c, stride=8 ):
+    """Output the decimal (if possible) and decoded view of the integer datum 'c'"""
+    if stride == 6:  # base-64 URL-safe
+        return f"{'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_'[c]:<{stride}}"
+    if stride == 5:  # base-32
+        return f"{'ABCDEFGHIJKLMNOPQRSTUVWXYZ234567'[c]:<{stride}}"
+    if stride == 4:  # hex nibbles
+        return f"x{'0123456789ABCDEF'[c]:<{stride-1}}"
+    if stride == 3:  # octal digits
+        return f"o{'01234567'[c]:<{stride-1}}"
+    if 1 <= stride <= 2:  # bits / base-4
+        return f"{'0123'[c]:<{stride}}"
+    if stride <= 8 and 32 <= c < 127:
+        s		= ("'" + chr( c ) + "'")
+        return f"{s:<{stride}}"
+    hex			= f"{c:0{(stride+3)//4}X}"
+    return f"{hex:<{stride}}" if stride <= len( hex ) + 2 else f"0x{hex:<{stride-2}}"
+
+
+def signal_entropy(
+    entropy: bytes,
+    stride: int			= 8,		# bits per symbol
+    symbols: Optional[int]	= None,		# symbols per DFT; default to ~128 bits and a power of 2, but < length
+    overlap: bool		= False,        # sweep across n-1 bits for symbol start
+    threshold: Optional[float]	= None,		# Default: must be a known length/stride/symbols
+    ignore_dc: bool		= False,        # For eg. character data, we know there'll be a big DC component
+    show_details: bool		= True,		# include signal details (incl. expensive ifft)
+    middle: Optional[Callable[List[float],float]] = None,  # default to normalized RMS energy, or eg. statistics.median on bin magnitudes
+    harmonics_max: int		= 2,		# maximum harmonics to represent
+) -> Optional[Signal]:
+    """Checks for signals in the supplied entropy.  If n-bit 'stride' or 'base'-n symbols are found
+    to exhibit significant signal pattern over the average noise, then the pattern will be reported.
+
+    Returns the Signal w/ dB signal multiple by which the greatest signal exceeded the threshold
+    noise floor (defaults to RMS average energy), and its bit stride and offset from start of
+    entropy.
+
+    Therefore, if a signal is found w/ power above the threshold (0.0dB), it will have a +'ve dB.
+    Acceptable (low signal strength == high entropy) signals below the threshold will have a -'ve
+    dB.  Using something like statistics.median is problematic for low-noise signals, because if a
+    sufficient number of bins have 0 energy, the noise will be 0, and a "default" SNR (signal/noise
+    *ratio*) of 1.0 will be used (0.0 dB), allowing any more legitimate signal to be used instead of
+    the unlikely "perfect" noise-free signal.
 
-def output_pdf( *args, **kwds ):
-    warnings.warn(
-        "output_pdf() is deprecated; use produce_pdf instead.",
-        PendingDeprecationWarning,
-    )
-    _,pdf,accounts		= produce_pdf( *args, **kwds )
-    return pdf,accounts
+    So, the result can be sorted by greatest power, and if any power is found to be > 0.0dB, the
+    entropy can be rejected as having too much "signal" vs "noise" (entropy).
 
+    """
+    entropy_hex			= codecs.encode( entropy, 'hex_codec' ).decode( 'ascii' )
+    entropy_bin			= ''.join( f"{int(h,16):0>4b}" for h in entropy_hex )
+    length			= len( entropy_bin )
+    assert not overlap or not ignore_dc, \
+        "Cannot specify both overlap and ignore_dc (intended for handling fixed-location symbols)"
+    if symbols is None:
+        # Default to the largest even-numbered amount of symbols that will fit in the signal, except
+        # if 'overlap' is specified, ensure we sweep across all bit-offsets of the symbol once.
+        symbols			= length // ( stride * 2 ) * 2
+        if overlap and length - symbols * stride < stride - 1:
+            symbols	       -= 2
+    assert symbols // 2 * 2 == symbols, \
+        f"An even number of symbols must be specified, not {symbols=}"
+    assert symbols * stride <= length, \
+        f"{symbols} x {stride}-bit symbols is beyond signal {length=}"
+    if threshold is None:
+        threshold		= signal_entropy.signal_limits.get(
+            overlap, {} ).get(
+                length, {} ).get(
+                    stride, {} ).get(
+                        symbols )
+    assert threshold and ( 0 < threshold ), \
+        f"A small +'ve ratio threshold of Signal energy (0,...) is required for {length}-bit entropy w/ {stride}-bit symbols eg. 300%, not {threshold=!r}"
+    #print( f"signal_entropy: {length:3}-bit entropy w/ {symbols:3} x {stride:2}-bit symbols ({ignore_dc=:5}): {threshold=:f}" )
+    dc				= 0+0j
+    strongest			= None
+    mags_all			= []
+    for symb in range(0, length - symbols * stride + 1, stride ):
+        for slip in range( stride if overlap else 1 ):  # noqa: E111
+            offset		= symb + slip
+            #print( f"=> {symb=:3} + {slip=:3} == {offset}" )
+            if length - offset < symbols * stride:
+                break
+            dfts		= entropy_bin_dfts( entropy_bin, offset, symbols, stride, cancel_dc=not ignore_dc )
+            #print( f"dfts: {' '.join( f'{b:{stride*2}.1f}' for b in dfts )}" )
+            dc			= dfts[0]
+            if ignore_dc:
+                dfts[0]		= 0+0j
+            nrms, mags		= dft_to_rms_mags( dfts )  # abs energy bins, from DC to max freq
+            mags_all.append( mags )
+            #print( f"mags: {' '.join( f'{m:{stride*2}.1f}' for m in mags )}: {sum(mags):7.2f} sum, {avg(mags):7.2f} avg, {nrms:7.2f} RMS; dc: {dc:11.1f} == {abs(dc):7.2f} abs" )
+            target, snrs	= denoise_mags( mags, threshold )
+            snrd		= dict( snrs )  # i: snr
+            #print( f"snrs: {' '.join( f'{snrd[i]:{stride*2}.1f}' if i in snrd else (' ' * stride*2) for i in range( len( mags )))}: {target=:7.1f}" )
+
+            # mid			= nrms if middle is None else middle( mags )
+            # target		= mid * threshold
+            # # Find the magnitude, offset of the top magnitudes exceeding target, sorted high to low
+            # tops		= sorted( ( (m,i) for i,m in enumerate( mags ) if m > target ), reverse=True )
+            # # Compute total signal dB SNR vs. target.  If all mags are 0 (all sigs were 0), then top
+            # # and target will all be 0.  However, this means that the signal is totally predictable
+            # # (contains infinitely strong signal), so pick an small but non-passing snr (1.0 ==
+            # # 0.0dB), so that any other more "legitimate" non-passing signals will likely be chosen
+            # # as strongest.  If no signal; report how far below the target our strongest bin is.
+
+            # When we have multiple signals, a Signal with several strong signals should have an SNR
+            # higher than something with fewer/weaker signals.  However, only the portion *above*
+            # the target threshold count.  So, sum the tops, and compute the overall Signal SNR.
+            if snrd:
+                peak		= target + sum( mags[i] - target for i in snrd )
+            else:
+                peak		= max( mags )  # No signals; SNR is greatest bin vs. threshold target
+            snr			= ( peak / target ) if target else 1.0
+            snr_dB		= into_dB( snr )
+            #print( f"tops: {offset=:3}, {peak=:7.2f}, {threshold=:7.2f}, {target=:7.2f}, {snr=:7.2f}, {snr_dB=:7.2f}" )
+            if strongest and snr_dB <= strongest.dB:
+                continue
+            if snr_dB < 0 or not show_details:
+                strongest	= Signal( dB=snr_dB, stride=stride, symbols=symbols, offset=offset, details='' )
+                continue
 
-def produce_pdf(
-    name: str,
-    group_threshold: int,			# SLIP-39 Group Threshold required
-    groups: Dict[str,Tuple[int,List[str]]],     # SLIP-39 Groups {<name>: (<need>,[<mnemonic>,...])
-    accounts: Sequence[Sequence[Account]],      # The crypto account(s); at least 1 of each required
-    using_bip39: bool,				# Using BIP-39 wallets Seed generation
-    card_format: str		= CARD,		# 'index' or '(<h>,<w>),<margin>'
-    paper_format: Any		= None,		# 'Letter', (x,y) dimensions in mm.
-    orientations: Sequence[str]	= None,		# available orientations; default portrait, landscape
-    cover_text: Optional[str]	= None,		# Any Cover Page text; we'll append BIP-39 if 'using_bip39'
-) -> Tuple[Tuple[str,str], FPDF, Sequence[Sequence[Account]]]:
-    """Produces an FPDF containing the specified SLIP-39 Mnemonics group recovery cards.
+            # Find the strongest signal frequency bin.  The max frequency (last) bin indicates some
+            # pattern sensed in every second symbol (the Nyquist rate, sampled at 2x the max
+            # frequency detectable).  The min frequency (first) bin indicates a DC offset (symbol
+            # values not centered around zero).  For N symbols, there are N/2+1 bins, [DC], [min],
+            # ..., [max]: the intervening N/2 bins [min], ..., [max] contain evenly spaced
+            # frequencies; eg. for N==8, N/2+1==5 bins, N/2==4 min-max bins where:
+            #
+            #     For symbols ==  8 ==>  64 bits 	For symbols == 16 ==> 128 bits
+            #     ------------------------------        ------------------------------
+            #     [0](DC)  ==> 8*8== 64 bits/beat       [0](DC)  ==>16*8==128 bits/beat
+            #     [1](min) ==> 4*8== 32 bits/beat       [1](min) ==> 8*8== 64 bits/beat
+            #     [2]          3*8== 24                 [2]          7*8== 56
+            #     [3]          2*8== 16                 [3]          6*8== 48
+            #     [4](max) ==> 1*8==  8 bits/beat       [4]          5*8== 40
+            #                                           [5]          4*8== 32
+            #                                           [6]          3*8== 24
+            #                                           [7]          2*8== 16
+            #                                           [8](max) ==> 1*8==  8 bits/beat
+            #
+
+            # Draw the signal area of interest over 'symbols' of the 'stride'-bit symbols beginning at bit 'offset'.
+            details		= '\n'
+            offpref		= ''
+            if offset > 8:
+                details	       += f"...x{offset:<3}>{entropy_bin[offset:]}\n"
+                offpref		= ' ' * 8
+            else:
+                details	       += f"{entropy_bin}\n"
+                offpref		= ' ' * offset
+            details	       += offpref + ''.join(
+                '-_'[(( i-offset ) // stride ) % 2] if ( offset <= i < ( offset + symbols * stride )) else ' '
+                for i in range( offset, length )
+            ) + '\n'
+
+            if stride >= 4:
+                details	       += offpref + ''.join(
+                    f"{c:<{stride}}"
+                    for c in entropy_bin_ints( entropy_bin, offset=offset, symbols=symbols, stride=stride, cancel_dc=not ignore_dc )
+                ) + ' decimal\n'
+            details	       += offpref + ''.join(
+                int_decode( c, stride=stride )
+                for c in entropy_bin_ints( entropy_bin, offset=offset, symbols=symbols, stride=stride )
+            ) + f" base-{2**(4 if stride >= 7 else stride)}" + ("/ASCII" if stride >= 7 else "") + " decoding\n"
+
+            # Select the one or two highest energy harmonics, and scale the waveform (which is
+            # denominated in stride-bit chunks) to the extent needed to cover the binary version of the
+            # entropy (then decimate to fit exactly).  So, if the 8-bit signal values are being
+            # recovered, we can scale the waveform by 8x.  Also, scale the amplitude by the (removed) DC
+            # component; this counteracts the reduction in dynamic range inherent to typical ASCII
+            # values (eg. the digits 0-9 are only 8% of the full ASCII range).
+            dfts_rec		= [0+0j] * len( dfts)
+            harmonic		= []
+            for max_i in snrd:
+                if harmonics_max and harmonic and len( harmonic ) >= harmonics_max:
+                    break
+                # The 0'th bin is DC, 1st is the base frequency, and then for eg. 16 symbols, we get
+                # DC + 8 bins, where each bin represents a harmonic frequency component repeating
+                # every 16/1==16, 16/2==8, 16/3==5+1/3, 16/4==4, 16/5==3+1/5, ..., 16/8==2 (the max
+                # Nyquist frequency) symbols.
+                harmonic.append( max_i )
+                dfts_rec[max_i]	= dfts[max_i]
+                if 0 < max_i < len(mags)-1:
+                    dfts_rec[-max_i] = dfts[-max_i]		# ... and its symmetrical bin, if not max freq.
+            harmonic_freq	= [
+                mixed_fraction( len( dfts ), h )
+                for h in harmonic
+                if h > 0
+            ]
+
+            dc_amplify		= None
+            if ignore_dc:
+                # scale the signal by the ratio of the removed DC to the largest other signal.  Since we know that
+                # the other signals were DC "higher" in the original signal, amplifying the signal by this ratio
+                # shouldn't exceed the maximum dynamic range of the eg. integer signal values.
+                dc_amplify	= 1 + abs( dc ) / max( abs( b ) for b in dfts )
+
+            # Compute the resolution for the inverse DFT required to properly cover the binary
+            # entropy.  However, limit size of the resultant DFT, as idft is O(N^2).  For a 512-bit
+            # entropy split into 3-bit symbols, results in a N=170 DFT.  That's the 28,900
+            # multiplications to produce an inverse-DFT.  That's the absolute largest we want to
+            # deal with, and we don't want to produce anything bigger than an N=128 DFT, because we
+            # don't need greater resolution than that to produce a smooth function graph in text.
+            scale_signal	= 1
+            scale_stride	= stride
+            while scale_stride > 2 and len( dfts_rec ) * scale_signal * 2 <= 128:
+                scale_stride   /= 2
+                scale_signal   *= 2
+            sigs		= signal_recover_real( dfts_rec, scale=scale_signal, integer=True, amplify=dc_amplify )
+
+            pos			= ''
+            neg			= ''
+            o			= 0
+            for i in range( symbols * stride ):
+                o			= int( i / scale_stride )
+                #print( f" - {i=:3} --> {o=:3} ==> {sigs[o]:7}" )
+                pos	       += signal_draw( sigs[o], pos=True )
+                neg	       += signal_draw( sigs[o], neg=True )
+            harmonic_dBs	= [ f"{ordinal(h) if h else 'DC'} {into_dB(mags[h]/target):.1f}dB" for h in harmonic ]
+            details	       += f"{offpref}{pos} {len(harmonic)} harmonics: {commas( harmonic_dBs, final_and=True )}\n"
+            details	       += f"{offpref}{neg}  - "
+            if 0 in harmonic:
+                details	       += "DC offset"
+            if 0 in harmonic and harmonic_freq:
+                details	       += " and "
+            if harmonic_freq:
+                details	       += f"every {commas( harmonic_freq, final_and=True )} symbols"
+            details	       += "\n"
+            strongest		= Signal( dB=snr_dB, stride=stride, symbols=symbols, offset=offset, details=details )
+    #mags_avgs			= [sum(col)/len(mags_all) for col in zip(*mags_all)]
+    #print( f"avgs: {' '.join( f'{m:{stride*2}.1f}' for m in mags_avgs )}: {sum(mags_avgs):7.2f}" )
+    return strongest
+
+signal_entropy.signal_limits	= {  # noqa: E305
+    False: {
+        128: {
+            3: {
+                40: 3.7959290562900327,
+                42: 3.647561915551939
+            },
+            4: {
+                30: 3.8431997942042178,
+                32: 3.8749244192110694
+            },
+            5: {
+                22: 4.01132938746108,
+                24: 3.855818706529049
+            },
+            6: {
+                18: 3.9821710568269393,
+                20: 4.10175893691386
+            },
+            7: {
+                16: 3.9998153373627243,
+                18: 3.86288147813215
+            },
+            8: {
+                14: 4.035389231470121,
+                16: 3.85295803340856
+            }
+        },
+        160: {
+            3: {
+                50: 3.768307059766632,
+                52: 3.657642158466681
+            },
+            4: {
+                38: 3.927175392223398,
+                40: 3.644644794089787
+            },
+            5: {
+                30: 4.004859915596088,
+                32: 3.723428336867249
+            },
+            6: {
+                24: 3.921311891749215,
+                26: 3.7484305351772997
+            },
+            7: {
+                20: 4.053741462343345,
+                22: 3.7022202971931337
+            },
+            8: {
+                18: 3.902181587171419,
+                20: 3.682978660449477
+            }
+        },
+        192: {
+            3: {
+                62: 3.78844766566635,
+                64: 3.6289494114027234
+            },
+            4: {
+                46: 3.9167065596553523,
+                48: 3.6393513794634913
+            },
+            5: {
+                36: 3.8915275898547788,
+                38: 3.7473928123694793
+            },
+            6: {
+                30: 3.9132919286186874,
+                32: 3.904575332226886
+            },
+            7: {
+                24: 4.18637617875428,
+                26: 3.8093336871612897
+            },
+            8: {
+                22: 4.046780450578674,
+                24: 3.766307067356347
+            }
+        },
+        224: {
+            3: {
+                72: 3.6989229751871116,
+                74: 3.858442530730556
+            },
+            4: {
+                54: 3.868023231802504,
+                56: 3.821289665038688
+            },
+            5: {
+                42: 3.9244827423261506,
+                44: 3.7255928738074235
+            },
+            6: {
+                34: 3.9796568789267033,
+                36: 3.8424176850637064
+            },
+            7: {
+                30: 3.884348278904745,
+                32: 3.7274499501787015
+            },
+            8: {
+                26: 3.9286076413465723,
+                28: 3.8212509511408332
+            }
+        },
+        256: {
+            3: {
+                82: 3.874105542934525,
+                84: 3.8031640175138075
+            },
+            4: {
+                62: 3.8535667393555895,
+                64: 3.6702455043197517
+            },
+            5: {
+                48: 3.966192695309544,
+                50: 3.810215205319617
+            },
+            6: {
+                40: 3.780615203182523,
+                42: 3.7166374907758537
+            },
+            7: {
+                34: 3.7632487952840674,
+                36: 3.820508681003472
+            },
+            8: {
+                30: 3.851962569866387,
+                32: 3.79387401596316
+            }
+        },
+        512: {
+            3: {
+                168: 3.8510228062858536,
+                170: 3.6930501052854368
+            },
+            4: {
+                126: 3.8739687818152095,
+                128: 3.8390294681049797
+            },
+            5: {
+                100: 3.8944436960232816,
+                102: 3.8213977750827777
+            },
+            6: {
+                82: 3.8651467331943445,
+                84: 4.00628842914143
+            },
+            7: {
+                70: 3.8977031690387087,
+                72: 3.7538315552341635
+            },
+            8: {
+                62: 3.956950350574148,
+                64: 3.7809092998228437
+            }
+        }
+    },
+    True: {
+        128: {
+            3: {
+                40: 4.015412815647333,
+                42: 4.049142728796211
+            },
+            4: {
+                30: 4.084354511564386,
+                32: 3.651281177941025
+            },
+            5: {
+                22: 4.190848444589507,
+                24: 4.358983589533379
+            },
+            6: {
+                18: 4.433227305912341,
+                20: 4.300266280446989
+            },
+            7: {
+                16: 4.63348257265716,
+                18: 4.251514929567565
+            },
+            8: {
+                14: 4.539487223257121,
+                16: 3.8298375269653464
+            }
+        },
+        160: {
+            3: {
+                50: 4.102991330499331,
+                52: 3.9201904890263806
+            },
+            4: {
+                38: 3.9660043286866316,
+                40: 3.8885457864057296
+            },
+            5: {
+                30: 4.1534554695112424,
+                32: 3.875257196943185
+            },
+            6: {
+                24: 4.314705804221271,
+                26: 4.276913496937379
+            },
+            7: {
+                20: 4.484017655351361,
+                22: 4.1891981747029154
+            },
+            8: {
+                18: 4.403790052686062,
+                20: 3.8171358828247257
+            }
+        },
+        192: {
+            3: {
+                62: 3.946957410520236,
+                64: 3.707417210141612
+            },
+            4: {
+                46: 4.243992805910835,
+                48: 3.5294430695860983
+            },
+            5: {
+                36: 4.307388423581146,
+                38: 3.8978305998977363
+            },
+            6: {
+                30: 4.296222571278912,
+                32: 3.666087989048472
+            },
+            7: {
+                24: 4.483230938800909,
+                26: 4.2688078347472285
+            },
+            8: {
+                22: 4.3975014624329,
+                24: 3.9299336762739103
+            }
+        },
+        224: {
+            3: {
+                72: 4.020867167290543,
+                74: 4.115472579780688
+            },
+            4: {
+                54: 4.155505881349097,
+                56: 3.611932501064818
+            },
+            5: {
+                42: 4.296142369450004,
+                44: 4.075549039418728
+            },
+            6: {
+                34: 4.339759784005132,
+                36: 4.199962133110188
+            },
+            7: {
+                30: 4.323936203605842,
+                32: 4.029221841050185
+            },
+            8: {
+                26: 4.470823290289282,
+                28: 3.8214418599675444
+            }
+        },
+        256: {
+            3: {
+                82: 3.9159493966982546,
+                84: 3.9052586437888848
+            },
+            4: {
+                62: 4.095016786713433,
+                64: 3.6867364579681587
+            },
+            5: {
+                48: 4.260740010786478,
+                50: 4.152970392617726
+            },
+            6: {
+                40: 4.298675707470258,
+                42: 3.9884678302777594
+            },
+            7: {
+                34: 4.218469498120002,
+                36: 4.09636224540939
+            },
+            8: {
+                30: 4.299777044591192,
+                32: 3.633717478015482
+            }
+        },
+        512: {
+            3: {
+                168: 4.016185108804742,
+                170: 4.028203232067135
+            },
+            4: {
+                126: 4.039199984086117,
+                128: 3.694796108995797
+            },
+            5: {
+                100: 4.012546598293882,
+                102: 3.8791966508371343
+            },
+            6: {
+                82: 4.071645334320387,
+                84: 4.31042853254462
+            },
+            7: {
+                70: 4.1408664186751505,
+                72: 4.060968141932326
+            },
+            8: {
+                62: 4.290524429312738,
+                64: 3.8260046870654842
+            }
+        }
+    }
+}
 
-    Returns the required Paper description [<format>,<orientation>], the FPDF containing the
-    produced cards, and the cryptocurrency accounts from the supplied slip39.Details.
-    """
-    if paper_format is None:
-        paper_format		= PAPER
-    if orientations is None:
-        orientations		= ('portrait', 'landscape')
-    # Deduce the card size
-    try:
-        (card_h,card_w),card_margin = CARD_SIZES[card_format.lower()]
-    except KeyError:
-        (card_h,card_w),card_margin = ast.literal_eval( card_format )
-    card_size			= Coordinate( y=card_h, x=card_w )
-
-    # Compute how many cards per page.  Flip page portrait/landscape to match the cards'.  Use the length
-    # of the first Group's first Mnemonic to determine the number of mnemonics on each card.
-    num_mnemonics		= len( groups[next(iter(groups.keys()))][1][0].split() )
-    card			= layout_card(  # converts to mm
-        card_size, card_margin, num_mnemonics=num_mnemonics )
-    card_dim			= card.mm()
-
-    # Find the best PDF and orientation, by max of returned cards_pp (cards per page).  Assumes
-    # layout_pdf returns a tuple that can be compared; cards_pp,orientation,... will always sort.
-    page_margin_mm		= PAGE_MARGIN * MM_IN
-    cards_pp,orientation,page_xy,pdf = max(
-        layout_pdf( card_dim, page_margin_mm, orientation=orientation, paper_format=paper_format )
-        for orientation in orientations
-    )
-    log.debug( f"Page: {paper_format} {orientation} {pdf.epw:.8}mm w x {pdf.eph:.8}mm h w/ {page_margin_mm}mm margins,"
-               f" Card: {card_format} {card_dim.x:.8}mm w x {card_dim.y:.8}mm h == {cards_pp} cards/page" )
 
-    card_elements		= list( card.elements() )
-    if log.isEnabledFor( logging.DEBUG ):
-        log.debug( f"Card elements: {json.dumps( card_elements, indent=4)}" )
-    tpl				= FlexTemplate( pdf, card_elements )
-
-    group_reqs			= list(
-        f"{g_nam}({g_of}/{len(g_mns)})" if g_of != len(g_mns) else f"{g_nam}({g_of})"
-        for g_nam,(g_of,g_mns) in groups.items() )
-    requires			= f"Recover w/ {group_threshold} of {len(group_reqs)} groups {', '.join(group_reqs[:4])}{'...' if len(group_reqs)>4 else ''}"
-
-    # Convert all of the first group's account(s) to an address QR code
-    assert accounts and accounts[0], \
-        "At least one cryptocurrency account must be supplied"
-    qr				= {}
-    for i,acct in enumerate( accounts[0] ):
-        qrc			= qrcode.QRCode(
-            version	= None,
-            error_correction = qrcode.constants.ERROR_CORRECT_M,
-            box_size	= 10,
-            border	= 1
-        )
-        qrc.add_data( acct.address )
-        qrc.make( fit=True )
+def shannon_entropy(
+    entropy: bytes,
+    stride: int			= 8,		# bits per symbol
+    overlap: bool		= True,
+    threshold: float		= None,         # Allow up to a certain % bits-per-symbol entropy deficit
+    show_details: bool		= True,		# include signal details (incl. expensive ifft)
+    snr_min: float		= 1/100,        # Minimum snr .01 == -40dB (eg. if all symbols unique)
+    N: Optional[int]		= None,		# If a max. number of unique symbols is known eg. dice
+) -> Optional[Signal]:
+    """Estimates the "Symbolised Shannon Entropy" for stride-bit chunks of the provided entropy; by
+    default, since we don't know the bit offset of any pattern, we'll scan at each possible bit
+    offset (overlap = True).
+
+    We'll compute the estimated predictability of the entropy, in the range [0,1], where 0 is
+    unpredictable (high entropy), and 1 is totally predictable (no entropy), but as a dB range,
+    where -'ve dB is below the threshold and acceptable, and +'ve is above the predictability
+    threshold, and is unacceptable.
+
+    Typically, for large entropy and/or small 'stride' values, the number of unique values N found
+    should tend toward 2^stride.  However, for small entropy (eg. insufficient data) or small known
+    N (eg. die rolls), we expect to see less unique values than would be implied by the stride.
+    Therefore, we reduce the N in those cases.
 
-        qr[i]			= qrc.make_image()
-        if log.isEnabledFor( logging.INFO ):
-            f			= io.StringIO()
-            qrc.print_ascii( out=f )
-            f.seek( 0 )
-            for line in f:
-                log.info( line.strip() )
-
-    if cover_text:
-        # Cover page is always laid out in landscape, and rotated if necessary
-        cvw			= max( pdf.epw, pdf.eph )
-        cvh			= min( pdf.epw, pdf.eph )
-        cover			= Region(
-            'cover', 0, 0, cvw / MM_IN, cvh / MM_IN
-        ).add_region_relative(
-            Box( 'cover-interior', x1=+1/2, y1=+1/2, x2=-1/2, y2=-1/2 )
-        )
-        cover.add_region_proportional(
-            Image( 'cover-image', x1=1/4, x2=3/4, y1=1/4, y2=3/4, priority=-3 )
-        ).square().add_region(
-            Image( 'cover-fade', priority=-2 )
-        )
-        cover.add_region_proportional(
-            Text( 'cover-text', y2=1/45, font='mono', multiline=True )  # 1st line
-        )
-        cover.add_region_proportional(
-            Region( 'cover-rhs', x1=3/5, y1=1/5 )  # On right, below full-width header
-        ).add_region_proportional(
-            Text( 'cover-sent', y2=1/25, font='mono', multiline=True )  # 1st line
-        )
+    The "strongest" (least entropy, most predictable, most indicative that the entropy is
+    unacceptable) signal will be returned.
 
-        cover_elements		= list( cover.elements() )
-        if log.isEnabledFor( logging.DEBUG ):
-            log.debug( f"Cover elements: {json.dumps( cover_elements, indent=4)}" )
-        tpl_cover		= FlexTemplate( pdf, cover_elements )
-        images			= os.path.dirname( __file__ )
-        tpl_cover['cover-image'] = os.path.join( images, 'SLIP-39.png' )
-        tpl_cover['cover-fade'] = os.path.join( images, '1x1-ffffffbf.png' )
-
-        slip39_mnems		= []
-        slip39_group		= []
-        g_nam_max		= max( map( len, groups.keys() ))
-        for g_nam,(g_of,g_mns) in groups.items():
-            slip39_mnems.extend( g_mns )
-            slip39_group.append( f"{g_nam:{g_nam_max}}: {g_of} of {len(g_mns)} to recover" )
-            slip39_group.extend( f"  {i+1:2}: ____________________" for i in range( len( g_mns )))
-        if using_bip39:
-            # Add the BIP-39 Mnemonics to the cover_text, by recovering the master_secret from the
-            # SLIP-39 Mnemonics.
-            master_secret	= recover( slip39_mnems )
-            bip39_enum		= enumerate_mnemonic( produce_bip39( entropy=master_secret ) )
-            rows		= ( len( bip39_enum ) + 4 ) // 5
-            cols		= ( len( bip39_enum ) + rows - 1 ) // rows
-            cover_text	       += "\n--------------8<-------------[ cut here ]------------------"
-            cover_text	       += "\n\n            Your BIP-39 Mnemonic Phrase is:\n"
-            for r in range( rows ):
-                cover_text     += "\n    "
-                for c in range( cols ):
-                    word	= bip39_enum.get( c * rows + r )
-                    cover_text += f"{word or '':12}"
-            cover_text	       += "\n"
-
-        tpl_cover['cover-text']	= cover_text
-        cover_sent		= "SLIP-39 Mnemonic Card Recipients:\n\n"
-        cover_sent	       += "\n".join( slip39_group )
-        tpl_cover['cover-sent']	= cover_sent
-
-        pdf.add_page()
-        if orientation.lower().startswith( 'p' ):
-            tpl_cover.render( offsetx=pdf.epw, rotate=-90.0 )
-        else:
-            tpl_cover.render()
-
-    card_n			= 0
-    page_n			= None
-    for g_n,(g_name,(g_of,g_mnems)) in enumerate( groups.items() ):
-        for mn_n,mnem in enumerate( g_mnems ):
-            p,(offsetx,offsety)	= page_xy( card_n )
-            if p != page_n:
-                pdf.add_page()
-                page_n		= p
-            card_n	       += 1
-
-            tpl['card-title']	= f"SLIP39 {g_name}({mn_n+1}/{len(g_mnems)}) for: {name}"
-            tpl['card-requires'] = requires
-            tpl['card-crypto1']	= f"{accounts[0][0].crypto} {accounts[0][0].path}: {accounts[0][0].address}"
-            tpl['card-qr1']	= qr[0].get_image()
-            if len( accounts[0] ) > 1:
-                tpl['card-crypto2'] = f"{accounts[0][1].crypto} {accounts[0][1].path}: {accounts[0][1].address}"
-                tpl['card-qr2']	= qr[1].get_image()
-            tpl[f'card-g{g_n}']	= f"{g_name:6.6}..{mn_n+1}" if len(g_name) > 7 else f"{g_name} {mn_n+1}"
-            tpl['card-link']	= 'slip39.com'
-            for n,m in enumerate_mnemonic( mnem ).items():
-                tpl[f"mnem-{n}"] = m
-
-            tpl.render( offsetx=offsetx, offsety=offsety )
-
-    return (paper_format,orientation),pdf,accounts
-
-
-def write_pdfs(
-    names		= None,		# sequence of [ <name>, ... ], or { "<name>": <details> }
-    master_secret	= None,		# Derive SLIP-39 details from this seed (if not supplied in names)
-    passphrase		= None,		# UTF-8 encoded passphrase; default is '' (empty)
-    using_bip39		= False,        # Generate Seed from Entropy via BIP-39 generation algorithm
-    group		= None,		# Group specifications, [ "Frens(3/6)", ... ]
-    group_threshold	= None,		# int, or 1/2 of groups by default
-    cryptocurrency	= None,		# sequence of [ 'ETH:<path>', ... ] to produce accounts for
-    edit		= None,		# Adjust crypto paths according to the provided path edit
-    card_format		= None,		# Eg. "credit"; False outputs no SLIP-39 Mnemonic cards to PDF
-    paper_format	= None,		# Eg. "Letter", "Legal", (x,y)
-    filename		= None,		# A file name format w/ {path}, etc. formatters
-    filepath		= True,		# A file path, if PDF output to file is desired; ''/True implies current dir.
-    printer		= None,		# A printer name (or True for default), if output to printer is desired
-    json_pwd		= None,		# If JSON wallet output desired, supply password
-    text		= None,		# Truthy outputs SLIP-39 recover phrases to stdout
-    wallet_pwd		= None,		# If paper wallet images desired, supply password
-    wallet_pwd_hint	= None,		# an optional password hint
-    wallet_format	= None,		# and a paper wallet format (eg. 'quarter')
-    wallet_paper	= None,		# default Wallets to output on Letter format paper,
-    cover_page		= True,         # Produce a cover page (including BIP-39 Mnemonic, if using_bip39)
-):
-    """Writes a PDF containing a unique SLIP-39 encoded Seed Entropy for each of the names specified.
-
-    If a sequence of multiple 'names' are supplied, then no master_secret is allowed (we must
-    generate for each name), or a dict of { 'name': <details>, ... } for each name must be provided
-    (neither master_secret nor using_bip39 allowed).
-
-    If we are generating master_secrets, and accounts, a number of Cryptocurrency wallet public
-    addresses and QR codes are generated; optionally, 'using_bip39' to force BIP-39 standard Seed
-    generation (instead of SLIP-39 standard, which uses the Seed Entropy directly).
-
-    If 'using_bip39' and 'cover_page', the BIP-39 Mnemonic phrase card is also produced.  It is
-    recommended to destroy this BIP-39 Mnemonic (ideally), or store it very, very securely (not
-    recommended).  Use the SLIP-39 "Recover" Controls, instead, to recover the BIP-39 Mnemonic
-    phrase when needed to restore a hardware wallet.
+    See: https://www.sciencedirect.com/topics/engineering/shannon-entropy
 
-    Returns a { "<filename>": <details>, ... } dictionary of all PDF files written, and each of
-    their account details.
+    We provide some known defaults for evaluating data of various sizes, which are tested to produce
+    only about a 1% rejection rate for good entropy.
 
     """
-    # Convert sequence of group specifications into standard { "<group>": (<needs>, <size>) ... }
-    if isinstance( group, dict ):
-        groups			= group
-    else:
-        groups			= dict(
-            group_parser( g )
-            for g in group or GROUPS
+    entropy_hex			= codecs.encode( entropy, 'hex_codec' ).decode( 'ascii' )
+    entropy_bin			= ''.join( f"{int(h,16):0>4b}" for h in entropy_hex )
+    length			= len( entropy_bin )
+
+    # Find all the unique n-bit symbols in the entropy at the desired offset(s)
+    strongest			= None
+    for offset in range( stride ) if overlap else (0,):
+        # Calculate the frequency of each unique symbol
+        frequency		= defaultdict( int )
+        # How many full n-bit symbols fit in the entropy at the current symbol-start offset?
+        symbols			= ( length - offset ) // stride
+        for s in range( symbols ):
+            i			= offset + s * stride
+            symbol		= entropy_bin[i:i+stride]
+            frequency[symbol]  += 1
+        assert sum( frequency.values() ) == symbols, \
+            f"Expected {symbols=} sum of probabilities events, found {frequency!r}"
+        assert all( len( s ) == stride for s in frequency ), \
+            f"Expected all {stride}-bit symbols, found {frequency!r}"
+
+        bitspersymbol			= -sum(  # sum may range: (~-0.0,...)
+            probability/symbols * math.log( probability/symbols, 2 )
+            for probability in frequency.values()
         )
-    assert groups and all( isinstance( k, str ) and len( v ) == 2 for k,v in groups.items() ), \
-        f"Each group member specification must be a '<group>': (<needs>, <size>), not {type(next(groups.items()))}"
-
-    group_threshold		= int( group_threshold ) if group_threshold else math.ceil( len( groups ) * GROUP_THRESHOLD_RATIO )
-
-    cryptopaths			= cryptopaths_parser( cryptocurrency, edit=edit )
-
-    # If account details not provided in names, generate them.  If using_bip39 is specified, this is
-    # where we use BIP-39 Seed generation to produce the wallet Seed, instead of SLIP-39 which uses
-    # the entropy directly (optionally, with a passphrase, which is not typically done, and isn't
-    # Trezor compatible).
-    if not isinstance( names, dict ):
-        assert not master_secret or not names or len( names ) == 1, \
-            "Creating multiple account details from the same secret entropy doesn't make sense"
-        names			= {
-            name: create(
-                name		= name,
-                group_threshold	= group_threshold,
-                groups		= groups,
-                master_secret	= master_secret,
-                passphrase	= passphrase.encode( 'utf-8' ) if passphrase else b'',
-                using_bip39	= using_bip39,  # Derive wallet Seed using BIP-39 Mnemonic + passphrase generation
-                cryptopaths	= cryptopaths,
+        # For small numbers of symbols, we cannot achieve a full N unique samples.  Therefore, the
+        # number of "bits of entropy" per symbol will be low -- even if all of the samples obtained
+        # are unique.  Therefore, we return a value in the range (0=bad,1=good) scaled by the bits
+        # required to encode the maximum number of unique symbols possible (due to the symbol or
+        # entropy size), not in the range [0,2^stride].
+        shannon			= 0.0
+        N_min			= min( N or symbols, symbols, 2**stride )
+        assert len( frequency ) <= N_min, \
+            f"Observed {len(frequency)} unique symbols; more than expected by min({N=}, {symbols=} or {2**stride=})"
+        if N_min > 1:
+            shannon		= bitspersymbol / math.log( N_min, 2 )
+
+        # So now, shannon is 1.0 for a "good" perfectly unpredictable entropy (all symbols
+        # different, full bits-per-symbol required to encode), and 0 for "bad" perfectly predictable
+        # entropy (all symbols identical, zero bits-per-symbol to encode).  This is the inverse of
+        # what we want: the more predictable something is, the stronger the "signal" is vs. the
+        # noise (entropy).  A 10% threshold means "I want at most 10% predictability; I want 90%
+        # noise".  This
+        predictability		= 1 - shannon			# 0 ==> good entropy, 1 ==> no entropy
+
+        # We want a -'ve dB if below (low predictability, good entropy, acceptable), +'ve if
+        # at/above threshold (high predictability, too much signal, reject).  1.0x == 0.0dB.
+        # However, we'll typically often see good, high-entropy data which turns out to have a
+        # shannon == 1.0, implying a predictability == 0, yielding an snr ratio of 0, which is
+        # invalid (tends to -oo).  We want to avoid this.  We know that the range is predictability
+        # range is (0,1), and we'll typically allow a threshold of 10%, so 0 is not -oo!  We really
+        # want to map (0...threshold,...1) onto a ratio range like .01 (-40dB) to 100 (+40dB), with
+        # 1.0 == 0dB right at threshold.  Map the range (0,threshold] to (.01,1] (mapped to -'ve
+        # dB), and let the +'ve dB (threshold,1) range fall where it may.  For example, if threshold
+        # is .1 and predictability is also .1, we want to map that to exactly 1.0:
+        #
+        #             predictability
+        #             v
+        #     1/100 + 0    / ( .1 / ( 1 - 1/100 )) == 0.0100 == -10.0   dB  # -'ve below threshold
+        #     1/100 + .043 / ( .1 / ( 1 - 1/100 )) == 0.4357 ==  -7.216 dB  #
+        #     1/100 + .1   / ( .1 / ( 1 - 1/100 )) == 1.0000 ==   0.0   dB  # exactly at threshold
+        #     1/100 + 1    / ( .1 / ( 1 - 1/100 )) == 9.9100 ==  19.20  dB  # +'ve above threshold
+        #
+        thresh			= shannon_entropy.shannon_limits.get(
+            overlap, {} ).get(
+                length, {} ).get(
+                    stride ) if threshold is None else threshold
+        assert thresh and 0 < thresh <= 2, \
+            f"A small +'ve ratio threshold of Shannon entropy deficit ~ (0, 1] is required for {length}-bit entropy w/ {symbols} x {stride}-bit symbols eg. 10%, not {thresh!r}"
+
+        snr			= snr_min + predictability / ( thresh / ( 1 - snr_min ))
+        snr_dB			= into_dB( snr )
+        weaker			= strongest and snr_dB < strongest.dB
+        ( log.debug if snr_dB < 0 else log.info )(
+            f"Found {len(frequency):3} unique (of {N_min:3} possible) in {symbols:3}"
+            f"x {stride:2}-bit symbols at offset {offset:2} in {length:4}-bit entropy:"
+            f" Shannon Entropy {bitspersymbol:7.3f} b/s, P({shannon:7.3f}) unpredictable; {predictability=:7.3f}"
+            f" vs. threshold={thresh:7.3f} == {snr=:7.3f} {snr_dB:7.3f}dB: {entropy_hex}"
+        )
+        if weaker:
+            continue
+        longest			= max(len(s) for s in frequency)
+        details			= ''
+        if snr_dB >= 0 and show_details:
+            details	       += f"{len(frequency):2} unique"
+            interesting		= sorted(
+                frequency.items(), reverse=True, key=lambda kv: kv[1]
             )
-            for name in names or [ "SLIP39" ]
-        }
-
-    if text and using_bip39:
-        # Output the BIP-39 Mnemonic phrase we're using to generate the Seed as text.  We'll label
-        # it as BIP-39, but it will just be ignored by standard SLIP-39 recovery attempts.
-        print( f"Using BIP-39 Mnemonic: {produce_bip39( entropy=master_secret )}" )
-
-    cover_text			= None
-    if cover_page:
-        cover_text		= open(os.path.join(os.path.dirname(__file__), 'COVER.txt')).read()
-        if using_bip39:
-            cover_text	       += open(os.path.join(os.path.dirname(__file__), 'COVER-BIP-39.txt')).read()
-        else:
-            cover_text	       += open(os.path.join(os.path.dirname(__file__), 'COVER-SLIP-39.txt')).read()
-
-    # Generate each desired SLIP-39 Mnemonic cards PDF.  Supports --card (the default).  Remember
-    # any deduced orientation and paper_format for below.
-    results			= {}
-    (pdf_paper,pdf_orient),pdf	= (None,None),None
-    for name, details in names.items():
-        # Get the first group of the accountgroups in details.accounts.
-        accounts		= details.accounts
-        assert accounts and accounts[0], \
-            "At least one --cryptocurrency must be specified"
-        for account in accounts[0]:
-            log.warning( f"{account.crypto:6} {account.path:20}: {account.address}" )
-
-        if text:
-            # Output the SLIP-39 mnemonics as text, to stdout:
-            #    name: <mnemonic>
-            # or, if no name, just:
-            #    <mnemonic>
-            g_nam_max		= max( map( len, details.groups.keys() ))
-            for g_name,(g_of,g_mnems) in details.groups.items():
-                for i,mnem in enumerate( g_mnems ):
-                    print( f"{name} {g_name:{g_nam_max}} {i+1}: {mnem}" )
-
-        # Unless no card_format (False) or paper wallet password specified, produce a PDF containing
-        # the SLIP-39 mnemonic recovery cards; remember the deduced (<pdf_paper>,<pdf_orient>).  If
-        # we're producing paper wallets, always force portrait orientation for the cards, to match.
-        if card_format is not False or wallet_pwd:
-            (pdf_paper,pdf_orient),pdf,_ = produce_pdf(
-                *details,
-                card_format	= card_format or CARD,
-                paper_format	= paper_format or PAPER,
-                orientations	= ('portrait', ) if wallet_pwd else None,
-                cover_text	= cover_text,
+            if stride < 7:
+                details	       += f" (base-{2**stride})"
+            details	       += ": " + commas(
+                f"{v:>{longest}} = {int_decode( int( v, 2 ), stride=stride ).strip()}: {c:2}"
+                for v,c in ( interesting[:4] if len( interesting ) > 5 else interesting )
             )
-
-        now			= datetime.now()
-
-        pdf_name		= ( filename or FILENAME_FORMAT ).format(
-            name	= name,
-            date	= datetime.strftime( now, '%Y-%m-%d' ),
-            time	= datetime.strftime( now, '%H.%M.%S'),
-            crypto	= accounts[0][0].crypto,
-            path	= accounts[0][0].path,
-            address	= accounts[0][0].address,
-        )
-        if not pdf_name.lower().endswith( '.pdf' ):
-            pdf_name	       += '.pdf'
-
-        if wallet_pwd:
-            # Deduce the paper wallet size and create a template.  All layouts are in specified in
-            # inches; template dimensions are in mm.
-            try:
-                (wall_h,wall_w),wall_margin = WALLET_SIZES[wallet_format.lower() if wallet_format else WALLET]
-            except KeyError:
-                (wall_h,wall_w),wall_margin = ast.literal_eval( wallet_format )
-
-            wall		= layout_wallet( Coordinate( y=wall_h, x=wall_w ), wall_margin )  # converts to mm
-            wall_dim		= wall.mm()
-
-            # Lay out wallets, always in Portrait orientation, defaulting to the Card paper_format
-            # if it is a standard size (a str, not an (x,y) tuple), otherwise to "Letter" paper.  Printers may
-            # have problems with a PDF mixing Landscape and Portrait, but do it if desired...
-            if wallet_paper is None:
-                wallet_paper	= paper_format if type(paper_format) is str else PAPER
-
-            pdf.add_page( orientation='P', format=wallet_paper )
-            page_margin_mm	= PAGE_MARGIN * MM_IN
-
-            walls_pp,page_xy	= layout_components( pdf, comp_dim=wall_dim, page_margin_mm=page_margin_mm )
-            wall_elements	= list( wall.elements() )
-            if log.isEnabledFor( logging.DEBUG ):
-                log.debug( f"Wallet elements: {json.dumps( wall_elements, indent=4)}" )
-            wall_tpl		= FlexTemplate( pdf, wall_elements )
-
-            # Place each Paper Wallet adding pages as necessary (we already have the first fresh page).
-            wall_n		= 0
-            page_n		= 0
-            for account_group in accounts:
-                for c_n,account in enumerate( account_group ):
-                    p,(offsetx,offsety) = page_xy( wall_n )
-                    if p != page_n:
-                        pdf.add_page( orientation='P', format=wallet_paper )
-                        page_n	= p
-                    try:
-                        private_enc		= account.encrypted( wallet_pwd )
-                    except NotImplementedError as exc:
-                        log.exception( f"{account.crypto} doesn't support BIP-38 or JSON wallet encryption: {exc}" )
-                        continue
-
-                    wall_n     += 1
-
-                    images			= os.path.dirname( __file__ )
-                    wall_tpl['wallet-bg']	= os.path.join( images, 'paper-wallet-background.png' )
-                    wall_tpl[f"crypto-f{c_n}"]	= account.crypto
-                    wall_tpl[f"crypto-b{c_n}"]	= account.crypto
-
-                    wall_tpl['center']		= os.path.join( images, account.crypto + '.png' )
-
-                    wall_tpl['name-label']	= "Wallet:"
-                    wall_tpl['name-bg']		= os.path.join( images, '1x1-ffffff54.png' )
-                    wall_tpl['name']		= name
-
-                    # wall_tpl['center-bg']	= os.path.join( images, 'guilloche-center.png' )
-
-                    public_qr	= qrcode.QRCode(
-                        version		= None,
-                        error_correction = qrcode.constants.ERROR_CORRECT_M,
-                        box_size	= 10,
-                        border		= 1,
-                    )
-                    public_qr.add_data( account.address )
-                    wall_tpl['address-l-bg']	= os.path.join( images, '1x1-ffffff54.png' )
-                    wall_tpl['address-l']	= account.address
-                    wall_tpl['address-r-bg']	= os.path.join( images, '1x1-ffffff54.png' )
-                    wall_tpl['address-r']	= account.address
-
-                    wall_tpl['address-qr-t']	= 'PUBLIC ADDRESS'
-                    wall_tpl['address-qr-bg']	= os.path.join( images, '1x1-ffffff54.png' )
-                    wall_tpl['address-qr']	= public_qr.make_image( back_color="transparent" ).get_image()
-                    wall_tpl['address-qr-b']	= 'DEPOSIT/VERIFY'
-                    wall_tpl['address-qr-r']	= account.path
-
-                    private_qr	= qrcode.QRCode(
-                        version		= None,
-                        error_correction = qrcode.constants.ERROR_CORRECT_M,
-                        box_size	= 10,
-                        border		= 1,
-                    )
-                    private_qr.add_data( private_enc )
-
-                    wall_tpl['private-bg']	= os.path.join( images, '1x1-ffffff54.png' )
-
-                    # If not enough lines, will throw Exception, as it should!  We don't want to
-                    # emit a Paper Wallet without the entire encrypted private key present.  This is
-                    # primarily an issue for Ethereum encrypted JSON wallets, which are very large.
-                    # As the vertical aspect ratio of the Paper Wallet increases (eg. for half- or
-                    # third-page vs. quarter-page Paper Wallets), the line length increases, but the
-                    # number of lines available decreases.  Estimate the number of characters on
-                    # each line.
-                    line_elm			= next( e for e in wall_elements if e['name'] == 'private-0' )
-                    line_points			= ( line_elm['x2'] - line_elm['x1'] ) / MM_IN * PT_IN
-                    line_fontsize		= line_elm['size']
-                    line_chars			= int( line_points / line_fontsize / ( 5 / 8 ))  # Chars ~ 5/8 width vs. height
-                    log.debug( f"Private key line length: {line_chars} chars" )
-                    for ln,line in enumerate( chunker( private_enc, line_chars )):
-                        wall_tpl[f"private-{ln}"] = line
-                    wall_tpl['private-hint-t']	= 'PASSWORD HINT:'
-                    wall_tpl['private-hint-bg']	= os.path.join( images, '1x1-ffffff54.png' )
-                    wall_tpl['private-hint']	= wallet_pwd_hint
-                    wall_tpl['private-qr-t']	= 'PRIVATE KEY'
-                    wall_tpl['private-qr-bg']	= os.path.join( images, '1x1-ffffff54.png' )
-                    wall_tpl['private-qr']	= private_qr.make_image( back_color="transparent" ).get_image()
-                    wall_tpl['private-qr-b']	= 'SPEND'
-
-                    wall_tpl.render( offsetx=offsetx, offsety=offsety )
-
-        if json_pwd:
-            # If -j|--json supplied, also emit the encrypted JSON wallet.  This may be a *different*
-            # password than the SLIP-39 master secret encryption passphrase.  It will be required to
-            # decrypt and use the saved JSON wallet file, eg. to load a software Ethereum wallet.
-            assert eth_account, \
-                "The optional eth-account package is required to support output of encrypted JSON wallets\n" \
-                "    python3 -m pip install eth-account"
-            assert any( 'ETH' == crypto for crypto,paths in cryptopaths ), \
-                "--json is only valid if '--crypto ETH' wallets are specified"
-
-            for eth in (
-                account
-                for group in accounts
-                for account in group
-                if account.crypto == 'ETH'
-            ):
-                json_str	= json.dumps( eth_account.Account.encrypt( eth.key, json_pwd ), indent=4 )
-                json_name	= ( filename or FILENAME_FORMAT ).format(
-                    name	= name or "SLIP39",
-                    date	= datetime.strftime( now, '%Y-%m-%d' ),
-                    time	= datetime.strftime( now, '%H.%M.%S'),
-                    crypto	= eth.crypto,
-                    path	= eth.path,
-                    address	= eth.address,
+            if len( interesting ) > 5:
+                details	       += f", ...x{len( interesting ) - 6}, " + commas(
+                    f"{v:>{longest}} = {int_decode( int( v, 2 ), stride=stride ).strip()}: {c:2}"
+                    for v,c in interesting[-2:]
                 )
-                if json_name.lower().endswith( '.pdf' ):
-                    json_name	= json_name[:-4]
-                json_name      += '.json'
-                while os.path.exists( json_name ):
-                    log.error( "ERROR: Will NOT overwrite {json_name}; adding '.new'!" )
-                    json_name  += '.new'
-                with open( json_name, 'w' ) as json_f:
-                    json_f.write( json_str )
-                log.warning( f"Wrote JSON {name or 'SLIP39'}'s encrypted ETH wallet {eth.address} derived at {eth.path} to: {json_name}" )
-
-                if pdf:
-                    # Add the encrypted JSON account recovery to the PDF also, if generated.
-                    pdf.add_page()
-                    margin_mm	= PAGE_MARGIN * MM_IN
-                    pdf.set_margin( 1.0 * MM_IN )
-
-                    col_width	= pdf.epw - 2 * margin_mm
-                    pdf.set_font( FONTS['sans'], size=10 )
-                    line_height	= pdf.font_size * 1.2
-                    pdf.cell( col_width, line_height, json_name )
-                    pdf.ln( line_height )
-
-                    pdf.set_font( FONTS['sans'], size=9 )
-                    line_height	= pdf.font_size * 1.1
-
-                    for line in json_str.split( '\n' ):
-                        pdf.cell( col_width, line_height, line )
-                        pdf.ln( line_height )
-                    pdf.image( qrcode.make( json_str ).get_image(), h=min(pdf.eph, pdf.epw)/2, w=min(pdf.eph, pdf.epw)/2 )
-
-        if pdf:
-            if filepath is not None:  # ''/True path implies current dir.
-                if filepath is True:
-                    filepath	= ''
-                pdf_path		= os.path.join( filepath, pdf_name ) if filepath else pdf_name
-                log.warning( f"Writing SLIP39-encoded wallet for {name!r} to: {pdf_path}" )
-                pdf.output( pdf_path )
-            if printer is not None:  # if True, uses "default" printer
-                printer		= None if printer is True else printer
-                log.warning( f"Printing SLIP39-encoded wallet for {name!r} to: {printer or '(default)'}: " )
-                printer_output(
-                    pdf.output(),
-                    printer		= printer,
-                    orientation		= pdf_orient,
-                    paper_format	= pdf_paper,
-                )
-
-        results[pdf_name]	= details
-
-    return results
-
+            details	       += "\n"
+            # Show the frequency of the symbols
+            offpref		= ''
+            if offset > 8:
+                details	       += f"...x{offset:<3}>{entropy_bin[offset:]}\n"
+                offpref		= ' ' * 8
+            else:
+                details	       += f"{entropy_bin}\n"
+                offpref		= ' ' * offset
+
+            most		= interesting[0][1]
+            least		= min( interesting[-1][1], most - 1 )
+            scale		= 255 // ( most - least )
+            wav			= ''
+            for s in range( symbols ):
+                i		= offset + s * stride
+                symbol		= entropy_bin[i:i+stride]
+                signal		= ( frequency[symbol] - least ) * scale - 128
+                wav	       += stride * signal_draw( signal )
+            details	       += f"{offpref}{wav}\n"
+
+        strongest		= Signal(
+            dB		= snr_dB,
+            stride	= stride,
+            symbols	= symbols,
+            offset	= offset,
+            details	= details,
+        )
+    return strongest
 
-def printers_available():
-    """
-    On macOS, find any available printers that appear to be available:
+shannon_entropy.shannon_limits	= {  # noqa: E305
+    False: {
+        128: {
+            3: 0.13774543485038598,
+            4: 0.21352083735742364,
+            5: 0.25857335693364575,
+            6: 0.18024155906953593,
+            7: 0.13393449488438314,
+            8: 0.10565473026867159
+        },
+        160: {
+            3: 0.10849932592752157,
+            4: 0.1732988370721074,
+            5: 0.2539763216172974,
+            6: 0.17643151270139718,
+            7: 0.13155406158983765,
+            8: 0.09785468929753503
+        },
+        192: {
+            3: 0.09151054889558748,
+            4: 0.14093100938467484,
+            5: 0.2264278561929118,
+            6: 0.1760839014542283,
+            7: 0.1271444744051939,
+            8: 0.08862800898521093
+        },
+        224: {
+            3: 0.07916495360459236,
+            4: 0.12252481621910122,
+            5: 0.20074807382273818,
+            6: 0.18204659485920255,
+            7: 0.12255892501570535,
+            8: 0.08642238826221553
+        },
+        256: {
+            3: 0.06465367140204993,
+            4: 0.11144594962520256,
+            5: 0.178731925009808,
+            6: 0.1819179694876547,
+            7: 0.12157462190503683,
+            8: 0.0860841002032892
+        },
+        512: {
+            3: 0.03404772973774162,
+            4: 0.05292514037032153,
+            5: 0.09170667883453174,
+            6: 0.15075753744881315,
+            7: 0.1264033310600746,
+            8: 0.08353573387816829
+        }
+    },
+    True: {
+        128: {
+            3: 0.15298580418729513,
+            4: 0.2451904173880027,
+            5: 0.2830395399608447,
+            6: 0.2028328095184408,
+            7: 0.16471175054429602,
+            8: 0.13936432438214608
+        },
+        160: {
+            3: 0.12038637754457157,
+            4: 0.19979446717148586,
+            5: 0.28247744681759446,
+            6: 0.19821636321414943,
+            7: 0.15105344745335572,
+            8: 0.1174014993567044
+        },
+        192: {
+            3: 0.09947716314352242,
+            4: 0.16262594321420024,
+            5: 0.24061446698597114,
+            6: 0.1988991682768491,
+            7: 0.14865256303627913,
+            8: 0.11409493984939509
+        },
+        224: {
+            3: 0.09107077508129978,
+            4: 0.13949972486012852,
+            5: 0.21449493978928671,
+            6: 0.18980489337861572,
+            7: 0.14016478187097317,
+            8: 0.10760893832461406
+        },
+        256: {
+            3: 0.07641224240206347,
+            4: 0.11638307614673703,
+            5: 0.19375895117831868,
+            6: 0.19231952709666766,
+            7: 0.13550085464769412,
+            8: 0.09588448833768029
+        },
+        512: {
+            3: 0.038422756462380414,
+            4: 0.057658537793532146,
+            5: 0.09918546794102677,
+            6: 0.16114705850045197,
+            7: 0.1402080308731611,
+            8: 0.09257360822755922
+        }
+    }
+}
 
-        printer Canon_G6000_series is idle.  enabled since Thu  3 Mar 09:24:56 2022
-                ...
-                Description: Canon G6000
-                Alerts: none
-                ...
-        printer Marg_s_Brother_HL_L2360D is idle.  enabled since Wed 15 Sep 12:19:48 2021
-                ...
-                Description: Marg's Brother HL-L2360D
-                Alerts: offline-report
-                ...
+def scan_entropy(
+    entropy: bytes,
+    strides: Optional[Union[int,Tuple[int,int]]] = None,  # If only a specific stride/s makes sense, eg. for ASCII symbols
+    overlap: bool		= True,
+    ignore_dc: bool		= False,
+    show_details: bool		= True,
+    N: Optional[int]		= None,			# shannon_entropy may specify limited unique symbols
+    signal_threshold: Optional[float]	= None,
+    shannon_threshold: Optional[float]	= None,
+) -> Tuple[List[Signal],List[Signal]]:
+    """Defaults to as many symbols as we can manage, given 'overlap' (which ensures we scan scan at
+    least a full stride of bit offsets).
+
+    There is usually little benefit to performing both with/without overlap; we still analyze the
+    0-offset symbols, but perhaps with a couple fewer total symbols, and with a slightly higher
+    threshold.
 
-    Yields a sequence of their names: (<system>,<long>), ...
     """
-    if sys.platform == 'darwin':
-        command		= [ '/usr/bin/lpstat', '-lt' ]
-        command_input	= None
+    if strides is None:
+        strides			= (3, 9)
     else:
-        raise NotImplementedError( f"Printing not supported on platform {sys.platform}" )
-
-    subproc			= subprocess.run(
-        command,
-        input		= command_input,
-        capture_output	= True,
-        encoding	= 'UTF-8'
-    )
-    assert subproc.returncode == 0 and subproc.stdout, \
-        f"{' '.join( command )!r} command failed, or no output returned"
-
-    if sys.platform == 'darwin':
-        system,human,ok		= None,None,None
-        for li in subproc.stdout.split( '\n' ):
-            printer		= re.match( r"^printer\s+([^\s]+)", li )
-            if printer:
-                system,human,ok	= printer.group(1).strip(),None,None
-                continue
-            descr		= re.match( r"^\s+Description:(.*)", li )
-            if descr:
-                human		= descr.group(1).strip()
-                continue
-            alerts		= re.match( r"^\s+Alerts:(.*)", li )
-            if alerts:
-                ok		= 'offline' not in alerts.group(1)
-                log.info( f"Printer: {human}: {alerts.group(1)}" )
-            if ok:
-                yield system,human
-                system,human,ok	= None,None,None
-
-
-def printer_output(
-    binary,			# Raw data for printer
-    printer		= None,
-    orientation		= None,
-    paper_format	= None,
-):
-    """Output raw binary data directly to the printer, eg.
-
-        ... | lpr -P "Canon_G6000_series" -o media=Letter -o sides=one-sided -o job-sheets=secret
+        try:
+            _,_			= strides
+        except TypeError:
+            strides		= (int(strides), int(strides)+1)
+
+    signals			= sorted(
+        (
+            s
+            for s in (
+                signal_entropy( entropy, stride=stride, overlap=overlap, ignore_dc=ignore_dc,
+                                show_details=show_details, threshold=signal_threshold )
+                for stride in range( *strides )
+            )
+            if s.dB >= 0
+        ), reverse=True )
+    shannons			= sorted(
+        (
+            s
+            for s in (
+                shannon_entropy( entropy, stride=stride, overlap=overlap, N=N,
+                                 show_details=show_details, threshold=shannon_threshold )
+                for stride in range( *strides )
+            )
+            if s.dB >= 0
+        ), reverse=True )
+    return signals, shannons
+
+
+def display_entropy( signals, shannons, what=None ):
+    result			= None
+    if signals or shannons:
+        report			= ''
+        dBs			= sorted( list( s.dB for s in signals ) + list( s.dB for s in shannons) )
+        dBr			= dBs[:1] + dBs[max( 1, len(dBs)-1):]
+        report		       += f"Entropy analysis {('of ' + what) if what else ''}: {len(signals)+len(shannons)}x"
+        report		       += f" {'-'.join( f'{dB:.1f}' for dB in dBr )}dB non-random patterns in"
+        report		       += f" {commas( sorted( set( s.stride for s in signals )), final_and=True)}-bit symbols\n\n"
+        for s,summary in sorted(
+                [
+                    (s, f"{s.dB:5.1f}dB Signal harmonic feature at offset {s.offset} in {s.symbols}x {s.stride}-bit symbols")
+                    for s in signals
+                ] + [
+                    (s, f"{s.dB:5.1f}dB Shannon entropy reduced at offset {s.offset} in {s.symbols}x {s.stride}-bit symbols")
+                    for s in shannons
+                ], reverse=True ):
+            report	       += f"-{summary}{': ' if s.details else ''}\n"
+            if s.details:
+                report	       += f"{s.details}\n"
+        result			= report
+    return result
+
+
+def analyze_entropy(
+    entropy: bytes,
+    strides: Optional[Union[int,Tuple[int,int]]] = None,  # If only a specific stride/s makes sense, eg. for ASCII symbols
+    overlap: bool		= True,
+    ignore_dc: bool		= False,
+    what: Optional[str]		= None,
+    show_details: bool		= True,
+    N: Optional[int]		= None,			# shannon_entropy may specify limited unique symbols
+    signal_threshold: Optional[float]	= None,
+    shannon_threshold: Optional[float]	= None,
+) -> Optional[str]:
+    """Analyzes the provided entropy.  If patterns are found, reports the findings; the peak Signal
+    and the aggregate report: (Signal, "...").
+
+    Seek strong Signals or weak Shannon Entropy, across a number of different interpretations (bit
+    strides and overlaps) of the entropy data.  We do not know where poor entropy may hide...
+
+    Since the probability of a signal being found is:
+
+        P( A or B or ... or Z ) = P(A) + P(B) + ... + P(Z) - P(A and B and ... Z )
+      = P( A or B or ... or Z ) = P(A) + P(B) + ... + P(Z) - ( P(A) * P(B) * ... P(Z) )
+
+    since we set the {signal,shannon}_entropy threshold values at ~ <1%, we know the P(A and B...)
+    term is very small; the probability we'll find an entropy failure it basically is the sum of the
+    individual probabilities of each test failing.
+
+    So, if we try 6 of each analysis, that's 12 * 1% =~= 12%.  If we want a total failure of about
+    1%, so we must target a ~0.1% failure on good entropy for each test.
+
+    However, it seems likely that if a signal appears in one bit-stride, it may appear in others, so
+    perhaps the analysis on different strides may be related.  So, it might be practical to target
+    0.25% failure on each individual test.
 
     """
-    if sys.platform == 'darwin':
-        command			= [ '/usr/bin/lpr', '-o', 'sides=one-sided' ]
-        command_input		= binary
-
-        # Find the desired printer's system name; otherwise use default printer
-        printer_system		= None
-        if printer:
-            printer_list	= list( printers_available() )
-            for system,human in printer_list:
-                if human.lower() == printer.lower() or system.lower() == printer.lower():
-                    printer_system = system
-            assert printer_system, \
-                f"Couldn't locate printer matching {printer!r}, in {', '.join( h for s,h in printer_list )}"
-        if printer_system:
-            command	       += [ '-P', printer_system ]
-        if paper_format:
-            command    	       += [ '-o', f"media={paper_format.capitalize()}" ]
-        if orientation:
-            # -o orientation-requested=N   Specify portrait (3) or landscape (4) orientation
-            N		= { 'p': 3, 'l': 4 }[orientation.lower()[0]]
-            command	       += [ '-o', f"orientation-requested={N}" ]
-
-    log.info( f"Printing via: {' '.join( command )}" )
-    subproc			= subprocess.run(
-        command,
-        input		= command_input,
-        capture_output	= True,
+    return display_entropy(
+        *scan_entropy(
+            entropy, strides, overlap, ignore_dc=ignore_dc, show_details=show_details, N=N,
+            signal_threshold=signal_threshold, shannon_threshold=shannon_threshold ),
+        what=what
     )
-    assert subproc.returncode == 0, \
-        f"{' '.join( command )!r} command failed"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slip39-9.0.4/slip39/layout/paper-wallet-background.png` & `slip39-9.1.2/slip39/layout/paper-wallet-background.png`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/main.py` & `slip39-9.1.2/slip39/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+
+#
+# Python-slip39 -- Ethereum SLIP-39 Account Generation and Recovery
+#
+# Copyright (c) 2022, Dominion Research & Development Corp.
+#
+# Python-slip39 is free software: you can redistribute it and/or modify it under
+# the terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.  It is also available under alternative (eg. Commercial) licenses, at
+# your option.  See the LICENSE file at the top of the source tree.
+#
+# Python-slip39 is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+
 import argparse
 import codecs
 import logging
 
 from .			import Account
 from .api		import random_secret
 from .util		import log_cfg, log_level, input_secure
@@ -84,14 +101,17 @@
                      default=True,
                      help="Produce PDF SLIP-39 cover page" )
     ap.add_argument( '--no-cover', dest="cover_page", action='store_false',
                      help="Disable PDF SLIP-39 cover page" )
     ap.add_argument( '--text', action='store_true',
                      default=None,
                      help="Enable textual SLIP-39 mnemonic output to stdout" )
+    ap.add_argument( '--watermark',
+                     default=None,
+                     help="Include a watermark on the output SLIP-39 mnemonic cards" )
     ap.add_argument( 'names', nargs="*",
                      help="Account names to produce; if --secret Entropy is supplied, only one is allowed.")
     args			= ap.parse_args( argv )
 
     # Set up logging; also, handle the degenerate case where logging has *already* been set up (and
     # basicConfig is a NO-OP), by (also) setting the logging level
     log_cfg['level']		= log_level( args.verbose - args.quiet )
@@ -178,12 +198,13 @@
             filename		= args.output,  # outputs to the current working dir, by default
             json_pwd		= json_pwd,
             text		= args.text,
             wallet_pwd		= wallet_pwd,
             wallet_pwd_hint	= wallet_pwd_hint,
             wallet_format	= wallet_format,
             cover_page		= args.cover_page,
+            watermark		= args.watermark,
         )
     except Exception as exc:
         log.exception( f"Failed to write PDFs: {exc}" )
         return 1
     return 0
```

### Comparing `slip39-9.0.4/slip39/output_test.py` & `slip39-9.1.2/slip39/output_test.py`

 * *Files identical despite different names*

### Comparing `slip39-9.0.4/slip39/recovery/__init__.py` & `slip39-9.1.2/slip39/recovery/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,38 @@
+
+#
+# Python-slip39 -- Ethereum SLIP-39 Account Generation and Recovery
+#
+# Copyright (c) 2022, Dominion Research & Development Corp.
+#
+# Python-slip39 is free software: you can redistribute it and/or modify it under
+# the terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.  It is also available under alternative (eg. Commercial) licenses, at
+# your option.  See the LICENSE file at the top of the source tree.
+#
+# Python-slip39 is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+
 import itertools
 import logging
 
 from typing		import List, Optional
 
 from shamir_mnemonic	import combine_mnemonics
 from mnemonic		import Mnemonic
 
 from ..util		import ordinal
+
+from .entropy		import (  # noqa F401
+    shannon_entropy, signal_entropy, analyze_entropy, scan_entropy, display_entropy
+)
+
 log				= logging.getLogger( __package__ )
 
 
 def recover(
     mnemonics: List[str],
     passphrase: bytes		= b"",
     using_bip39: bool		= False,
@@ -60,17 +82,17 @@
         if not secret:
             # No recovery; raise the Exception produced by original attempt w/ all mnemonics
             raise exc
     log.info(
         f"Recovered {len(secret)*8}-bit SLIP-39 Seed Entropy with {len(combo)}"
         f" ({'all' if len(combo) == len(mnemonics) else ', '.join( ordinal(i+1) for i in combo)})"
         f" of {len(mnemonics)} supplied mnemonics" + (
-            "; Seed generated using BIP-39 Mnemonic representation w/ passphrase"
+            f"; Seed decoded from SLIP-39 (w/ no passphrase) and generated using BIP-39 Mnemonic representation w/ {'a' if passphrase else 'no'} passphrase"
             if using_bip39 else
-            "; Seed decoded from SLIP-39 Mnemonics w/ passphrase"
+            f"; Seed decoded from SLIP-39 Mnemonics w/ {'a' if passphrase else 'no'} passphrase"
         )
     )
     if using_bip39:
         secret			= recover_bip39(
             mnemonic	= produce_bip39( entropy=secret ),
             passphrase	= passphrase,
         )
```

### Comparing `slip39-9.0.4/slip39/recovery/main.py` & `slip39-9.1.2/slip39/recovery/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+
+#
+# Python-slip39 -- Ethereum SLIP-39 Account Generation and Recovery
+#
+# Copyright (c) 2022, Dominion Research & Development Corp.
+#
+# Python-slip39 is free software: you can redistribute it and/or modify it under
+# the terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.  It is also available under alternative (eg. Commercial) licenses, at
+# your option.  See the LICENSE file at the top of the source tree.
+#
+# Python-slip39 is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+#
+
 import argparse
 import codecs
 import logging
 
 from ..util		import log_cfg, log_level, input_secure, ordinal
 from .			import recover, recover_bip39
 
@@ -53,14 +70,17 @@
                      help="Return the BIP-39 Mnemonic Seed Entropy instead of the generated Seed (default: False)" )
     ap.add_argument( '-b', '--bip39', action='store_true',
                      default=False,
                      help="Recover Entropy and generate 512-bit secret Seed from BIP-39 Mnemonic + passphrase" )
     ap.add_argument( '-u', '--using-bip39', action='store_true',
                      default=False,
                      help="Recover Entropy from SLIP-39, generate 512-bit secret Seed using BIP-39 Mnemonic + passphrase" )
+    ap.add_argument( '--binary', action='store_true',
+                     default=False,
+                     help="Output seed in binary instead of hex" )
     ap.add_argument( '-p', '--passphrase',
                      default=None,
                      help="Decrypt the SLIP-39 or BIP-39 master secret w/ this passphrase, '-' reads it from stdin (default: None/'')" )
     args			= ap.parse_args( argv )
 
     log_cfg['level']		= log_level( args.verbose - args.quiet )
 
@@ -73,15 +93,15 @@
         assert not args.passphrase, "--entropy and --passphrase cannot be used together"
     # Optional passphrase (utf-8 encoded bytes)
     passphrase			= args.passphrase or ""
     if passphrase == '-':
         passphrase		= input_secure( 'Master seed passphrase: ', secret=True )
     elif passphrase:
         log.warning( "It is recommended to not use '-p|--passphrase <password>'; specify '-' to read from input" )
-    passphrase			= passphrase.encode( 'utf-8' )
+    passphrase			= passphrase.encode( 'UTF-8' )
 
     # If BIP-39 recovery designated, only a single mnemonic is allowed:
     secret			= None
     algo			= "BIP-39" if args.bip39 else "SLIP-39"
     mnemonics			= args.mnemonic or []
     if args.bip39:
         # Recover actual BIP-39 Mnemonic.  By default, outputs the generated 512-bit wallet Seed.
@@ -116,9 +136,11 @@
                     return 0
                 if ':' in phrase:  # Discard any "<name>: <mnemonic>" name prefix.
                     _,phrase	= phrase.split( ':', 1 )
                 mnemonics.append( phrase )
     if secret:
         secret			= codecs.encode( secret, 'hex_codec' ).decode( 'ascii' )
         log.info( f"Recovered {algo} secret; To re-generate SLIP-39 wallet, send it to: python3 -m slip39 --secret -" )
+        if args.binary:
+            secret		= ''.join( f"{int(h,16):0>4b}" for h in secret )
         print( secret )
     return 0 if secret else 1
```

### Comparing `slip39-9.0.4/slip39.egg-info/PKG-INFO` & `slip39-9.1.2/slip39.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slip39
-Version: 9.0.4
+Version: 9.1.2
 Summary: Standards-compliant SLIP-39 cryptocurrency seed generation and recovery, compatible with Trezor hardware wallets
 Home-page: https://github.com/pjkundert/python-slip39
 Author: Perry Kundert
 Author-email: perry@dominionrnd.com
 License: Dual License; GPLv3 and Proprietary
 Project-URL: Bug Tracker, https://github.com/pjkundert/python-slip39/issues
 Keywords: Ethereum Bitcoin Dogecoin Litecoin cryptocurrency SLIP-39 BIP-39 seed recovery PDF BIP-38 paper wallet
```

