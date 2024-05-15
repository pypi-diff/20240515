# Comparing `tmp/open-cravat-2.6.0.tar.gz` & `tmp/open-cravat-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-cravat-2.6.0.tar", last modified: Wed Apr 24 13:29:53 2024, max compression
+gzip compressed data, was "open-cravat-2.6.1.tar", last modified: Thu May  9 18:20:15 2024, max compression
```

## Comparing `open-cravat-2.6.0.tar` & `open-cravat-2.6.1.tar`

### file list

```diff
@@ -1,338 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.338945 open-cravat-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 13:29:51.000000 open-cravat-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-24 13:29:53.338945 open-cravat-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 13:29:51.000000 open-cravat-2.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.290944 open-cravat-2.6.0/cravat/
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60556 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/admin_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    19600 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.290944 open-cravat-2.6.0/cravat/annotator_template/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_template/annotator_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_template/annotator_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_template/annotator_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.290944 open-cravat-2.6.0/cravat/annotator_template/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_template/data/annotator_template.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_commonmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17199 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_postaggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20758 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12114 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat-system.template.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat.yml
--rw-r--r--   0 runner    (1001) docker     (127)    32368 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    85512 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    31514 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    42490 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)    51476 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    56209 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/example_input
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19608 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/inout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.294944 open-cravat-2.6.0/cravat/liftover/
--rw-r--r--   0 runner    (1001) docker     (127)   931825 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/liftover/hg18ToHg38.over.chain
--rw-r--r--   0 runner    (1001) docker     (127)   606773 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/liftover/hg19ToHg38.over.chain
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/mp_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/oc.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/runcravat.py
--rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/store_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    18622 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/vcfanno.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.294944 open-cravat-2.6.0/cravat/webresult/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.294944 open-cravat-2.6.0/cravat/webresult/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/css/pqselect.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/email.png
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.298944 open-cravat-2.6.0/cravat/webresult/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-bold-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19508 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-bold-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-light-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18980 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-light-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-medium-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19416 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-medium-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    33072 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25740 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.306944 open-cravat-2.6.0/cravat/webresult/images/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-90deg-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-down-right-circle-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-down-right-circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-down-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-spinner-static.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-spinner.gif
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrows-move.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/back_arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)   264317 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/bigSpinner.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/camera.png
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/camera.svg
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/caret-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/close-button.png
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/close.png
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/close_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download-material-black.png
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download-material-blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download.png
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download.svg
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download12.png
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/grip-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/help_16x16.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/help_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    32137 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/loading-gif-animation.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/mail.png
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/menu.png
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/openNewTab.png
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/package.png
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/pencil.png
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/pin-2.png
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/pin.png
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/pin.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/plus-circle-dotted.svg
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/plus-circle-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/question.png
--rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/resize.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/save.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/save_new.png
--rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/search.png
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/sorry.png
--rw-r--r--   0 runner    (1001) docker     (127)    55605 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/spinCircle.gif
--rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/spinner.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/triangle-down.png
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/triangle-right.png
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/upload-material-black.png
--rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/upload-material-blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/x-lg.svg
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/x.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.310944 open-cravat-2.6.0/cravat/webresult/js/
--rw-r--r--   0 runner    (1001) docker     (127)   398184 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/Chart.js
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/dom-to-image.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/download.js
--rw-r--r--   0 runner    (1001) docker     (127)   954164 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/graphics.js
--rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-3.2.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.310944 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.282944 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.310944 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
--rw-r--r--   0 runner    (1001) docker     (127)   293430 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.314944 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)    32588 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    35997 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (127)   520714 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   253668 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18705 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery.tools.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery.url.js
--rw-r--r--   0 runner    (1001) docker     (127)    84772 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/packery.pkgd.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.318945 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (127)   103213 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.318945 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/horiz-bg.png
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/square-red-rb.gif
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/square-red-tr.gif
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/square_dirty.gif
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/vert-bg.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.318945 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76985 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.318945 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    16186 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css
--rw-r--r--   0 runner    (1001) docker     (127)   481365 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   242939 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.286944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/brown/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/gray/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/office/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/purple/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/red/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/tan/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/violet/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/pqselect.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    92225 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/raphael-min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/jsonreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/nocache/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.326944 open-cravat-2.6.0/cravat/webresult/nocache/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/css/singlevariantpage.css
--rw-r--r--   0 runner    (1001) docker     (127)    21047 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/css/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/css/widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.326944 open-cravat-2.6.0/cravat/webresult/nocache/js/
--rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/filter.js
--rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/infomgr.js
--rw-r--r--   0 runner    (1001) docker     (127)    44130 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)   102552 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/setup.js
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/showvariant.js
--rw-r--r--   0 runner    (1001) docker     (127)    35998 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/singlevariantpage.js
--rw-r--r--   0 runner    (1001) docker     (127)    31708 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/variables.js
--rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/widgethelper.js
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/variant.html
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/question.png
--rw-r--r--   0 runner    (1001) docker     (127)    30198 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/webresult.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/webviewer.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.326944 open-cravat-2.6.0/cravat/webstore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/cravat_store.css
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.330944 open-cravat-2.6.0/cravat/webstore/images/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/chat-dots-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/chat-dots.svg
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/chat-left-text-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/chat-left-text.svg
--rw-r--r--   0 runner    (1001) docker     (127)    22268 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/done.png
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/email.png
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/empty.png
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    38197 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/genericmodulelogo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/hamburger.png
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/left_arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)    67804 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/new.png
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/question.png
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/right_arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/x-lg.svg
--rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/jquery-3.3.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.330944 open-cravat-2.6.0/cravat/webstore/js/
--rw-r--r--   0 runner    (1001) docker     (127)    75673 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/js/showdown-1.9.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    91924 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/js/showdown.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.330944 open-cravat-2.6.0/cravat/webstore/nocache/
--rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/nocache/webstore.css
--rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/nocache/webstore.js
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/sse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/store_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/webstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/ws.html
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/ws.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.334945 open-cravat-2.6.0/cravat/websubmit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)   210024 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/Chart.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/down.png
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/email.png
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/googleAnalytics.js
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/help.png
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/house-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.334945 open-cravat-2.6.0/cravat/websubmit/input-examples/
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/input-examples/cravat.hg38.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/input-examples/vcf.hg38.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/jquery-3.3.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    53784 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    56098 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/logo_transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/menu.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.334945 open-cravat-2.6.0/cravat/websubmit/nocache/
--rw-r--r--   0 runner    (1001) docker     (127)    13800 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/broken_wheel.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/core.js
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/header.js
--rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/moduleinfo.js
--rw-r--r--   0 runner    (1001) docker     (127)    17348 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/websubmit.css
--rw-r--r--   0 runner    (1001) docker     (127)    79780 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/websubmit.js
--rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nointernet.png
--rw-r--r--   0 runner    (1001) docker     (127)    27869 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/pqselect.dev.customforsubmit.js
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/question.png
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/refresh.png
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/setting.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/threedots.png
--rw-r--r--   0 runner    (1001) docker     (127)    49732 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/websubmit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/wincravat.pyw
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.338945 open-cravat-2.6.0/open_cravat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:29:53.338945 open-cravat-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-24 13:29:51.000000 open-cravat-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.040770 open-cravat-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 18:20:13.000000 open-cravat-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 18:20:15.040770 open-cravat-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 18:20:13.000000 open-cravat-2.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:14.996770 open-cravat-2.6.1/cravat/
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60556 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/admin_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19600 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/annotator_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:14.996770 open-cravat-2.6.1/cravat/annotator_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/annotator_template/annotator_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/annotator_template/annotator_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/annotator_template/annotator_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:14.996770 open-cravat-2.6.1/cravat/annotator_template/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/annotator_template/data/annotator_template.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/base_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/base_commonmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17199 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/base_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/base_postaggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20758 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/base_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat-system.template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    32279 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85512 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31514 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42490 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51476 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56209 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/cravat_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/example_input
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19608 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/inout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:14.996770 open-cravat-2.6.1/cravat/liftover/
+-rw-r--r--   0 runner    (1001) docker     (127)   931825 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/liftover/hg18ToHg38.over.chain
+-rw-r--r--   0 runner    (1001) docker     (127)   606773 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/liftover/hg19ToHg38.over.chain
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/mp_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/oc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/runcravat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/store_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/vcfanno.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.000770 open-cravat-2.6.1/cravat/webresult/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.000770 open-cravat-2.6.1/cravat/webresult/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/css/pqselect.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/email.png
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.000770 open-cravat-2.6.1/cravat/webresult/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/fonts/roboto-bold-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19508 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/fonts/roboto-bold-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/fonts/roboto-light-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18980 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/fonts/roboto-light-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/fonts/roboto-medium-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19416 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/fonts/roboto-medium-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    33072 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25740 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.008770 open-cravat-2.6.1/cravat/webresult/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-90deg-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-down-right-circle-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-down-right-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-down-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-spinner-static.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-spinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/arrows-move.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/back_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)   264317 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/bigSpinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/camera.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/close-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/close.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/close_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/download-material-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/download-material-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/download.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/download.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/download12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/grip-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/help_16x16.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/help_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32137 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/loading-gif-animation.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/mail.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/openNewTab.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/package.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/pin-2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/pin.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/pin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/plus-circle-dotted.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/plus-circle-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/question.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/resize.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/save.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/save_new.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/search.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/sorry.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55605 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/spinCircle.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/spinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/triangle-down.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/triangle-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/upload-material-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/upload-material-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/x-lg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/images/x.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.012770 open-cravat-2.6.1/cravat/webresult/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   398184 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/Chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/dom-to-image.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/download.js
+-rw-r--r--   0 runner    (1001) docker     (127)   954164 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/graphics.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-3.2.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.016770 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:14.988769 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.016770 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
+-rw-r--r--   0 runner    (1001) docker     (127)   293430 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.020770 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32588 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    35997 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)   520714 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   253668 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18705 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery.tools.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/jquery.url.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84772 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/packery.pkgd.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.020770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   103213 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/EULA.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.024770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/horiz-bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/sprite.png
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/square-red-rb.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/square-red-tr.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/square_dirty.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/vert-bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.024770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76985 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.024770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.024770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16186 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)   481365 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   242939 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:14.988769 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.024770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.024770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/brown/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.024770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.024770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/gray/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/office/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/purple/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/red/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/tan/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/violet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/pqselect.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    92225 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/js/raphael-min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/jsonreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/nocache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.028770 open-cravat-2.6.1/cravat/webresult/nocache/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/css/singlevariantpage.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21047 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/css/widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.032770 open-cravat-2.6.1/cravat/webresult/nocache/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/filter.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/infomgr.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44130 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)   102552 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/showvariant.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35998 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/singlevariantpage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31708 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/variables.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/js/widgethelper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/nocache/variant.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/question.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30198 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/webresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webresult/webviewer.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.032770 open-cravat-2.6.1/cravat/webstore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/cravat_store.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.036770 open-cravat-2.6.1/cravat/webstore/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/chat-dots-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/chat-dots.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/chat-left-text-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/chat-left-text.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    22268 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/done.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/email.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38197 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/genericmodulelogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/hamburger.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/left_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67804 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/new.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/question.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/right_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/images/x-lg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/jquery-3.3.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.036770 open-cravat-2.6.1/cravat/webstore/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    75673 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/js/showdown-1.9.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91924 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/js/showdown.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.036770 open-cravat-2.6.1/cravat/webstore/nocache/
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/nocache/webstore.css
+-rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/nocache/webstore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/store_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16403 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/webstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/ws.html
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/webstore/ws.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.040770 open-cravat-2.6.1/cravat/websubmit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)   210024 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/Chart.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/down.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/email.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/googleAnalytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/help.png
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/house-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.040770 open-cravat-2.6.1/cravat/websubmit/input-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/input-examples/cravat.hg38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/input-examples/hgvs.hg38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/input-examples/vcf.hg38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/jquery-3.3.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    53784 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56098 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/logo_transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/menu.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.040770 open-cravat-2.6.1/cravat/websubmit/nocache/
+-rw-r--r--   0 runner    (1001) docker     (127)    13800 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nocache/broken_wheel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nocache/core.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nocache/header.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18094 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nocache/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nocache/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nocache/moduleinfo.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nocache/websubmit.css
+-rw-r--r--   0 runner    (1001) docker     (127)    79836 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nocache/websubmit.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/nointernet.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27869 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/pqselect.dev.customforsubmit.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/question.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/refresh.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/setting.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/threedots.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49732 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/websubmit/websubmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-09 18:20:13.000000 open-cravat-2.6.1/cravat/wincravat.pyw
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:20:15.040770 open-cravat-2.6.1/open_cravat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 18:20:14.000000 open-cravat-2.6.1/open_cravat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-05-09 18:20:14.000000 open-cravat-2.6.1/open_cravat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:20:14.000000 open-cravat-2.6.1/open_cravat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 18:20:14.000000 open-cravat-2.6.1/open_cravat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 18:20:14.000000 open-cravat-2.6.1/open_cravat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 18:20:14.000000 open-cravat-2.6.1/open_cravat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:20:15.044770 open-cravat-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-09 18:20:13.000000 open-cravat-2.6.1/setup.py
```

### Comparing `open-cravat-2.6.0/LICENSE` & `open-cravat-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/PKG-INFO` & `open-cravat-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-cravat
-Version: 2.6.0
+Version: 2.6.1
 Summary: OpenCRAVAT - variant analysis toolkit
 Home-page: https://www.opencravat.org
 Author: Kyle Moad, Kyle Anderson, Madison Larsen, Jeltje van Baren, and Rachel Karchin
 Author-email: support@opencravat.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `open-cravat-2.6.0/README.rst` & `open-cravat-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/__init__.py` & `open-cravat-2.6.1/cravat/__init__.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/admin_util.py` & `open-cravat-2.6.1/cravat/admin_util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/aggregator.py` & `open-cravat-2.6.1/cravat/aggregator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/annotator_options.py` & `open-cravat-2.6.1/cravat/annotator_options.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/annotator_template/annotator_template.py` & `open-cravat-2.6.1/cravat/annotator_template/annotator_template.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/annotator_template/annotator_template.yml` & `open-cravat-2.6.1/cravat/annotator_template/annotator_template.yml`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/base_annotator.py` & `open-cravat-2.6.1/cravat/base_annotator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/base_commonmodule.py` & `open-cravat-2.6.1/cravat/base_commonmodule.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/base_converter.py` & `open-cravat-2.6.1/cravat/base_converter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/base_mapper.py` & `open-cravat-2.6.1/cravat/base_mapper.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/base_postaggregator.py` & `open-cravat-2.6.1/cravat/base_postaggregator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/base_summarizer.py` & `open-cravat-2.6.1/cravat/base_summarizer.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/config_loader.py` & `open-cravat-2.6.1/cravat/config_loader.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/constants.py` & `open-cravat-2.6.1/cravat/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,47 @@
     default_log_dir = os.path.join(oc_root_dir, log_dir_name)
     if os.path.exists(default_log_dir) == False:
         os.mkdir(default_log_dir)
     conf[log_dir_key] = default_log_dir
 # Live conf
 live_conf_fname = "live.yml"
 
-base_modules_key = "base_modules"
 main_conf_fname = "cravat.yml"
 main_conf_path = os.path.join(default_conf_dir, main_conf_fname)
 if os.path.exists(main_conf_path) == False:
     shutil.copyfile(os.path.join(packagedir, main_conf_fname), main_conf_path)
 
+# Base modules
+base_modules = [
+    'cravat-converter',
+    'vcf-converter',
+    'oldcravat-converter',
+    'hgvs-converter',
+    'textreporter',
+    'excelreporter',
+    'tagsampler',
+    'vcfinfo',
+    'hg38',
+    'casecontrol',
+    'wgbase',
+    'wghg19',
+    'wgncrna',
+    'wglollipop',
+    'wgndex',
+    'wgcircossummary',
+    'wgcodingvsnoncodingsummary',
+    'wggosummary',
+    'wgsosamplesummary',
+    'wgsosummary',
+    'wgnote',
+    'wgvcfinfo',
+    'hg38wgs',
+    'varmeta',
+    'wgrankscore',
+]
 
 # metrics
 save_metrics_key = 'save_metrics'
 default_save_metrics = True
 metrics_url_key = 'metrics_url'
 default_metrics_url = 'https://metrics.opencravat.org'
```

### Comparing `open-cravat-2.6.0/cravat/cravat_admin.py` & `open-cravat-2.6.1/cravat/cravat_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,17 +404,15 @@
         if 'publish_password' in sys_conf:
             args.password = sys_conf['publish_password']
         else:
             args.password = getpass()
     au.publish_module(args.module, args.user, args.password, overwrite=args.overwrite, include_data=args.data)
 
 def install_base (args):
-    sys_conf = au.get_system_conf()
-    base_modules = sys_conf.get(constants.base_modules_key,[])
-    args = SimpleNamespace(modules=base_modules,
+    args = SimpleNamespace(modules=constants.base_modules,
         force_data=args.force_data,
         version=None,
         yes=True,
         private=False,
         skip_dependencies=False,
         force=args.force,
         skip_data=False,
```

### Comparing `open-cravat-2.6.0/cravat/cravat_class.py` & `open-cravat-2.6.1/cravat/cravat_class.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/cravat_convert.py` & `open-cravat-2.6.1/cravat/cravat_convert.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/cravat_filter.py` & `open-cravat-2.6.1/cravat/cravat_filter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/cravat_metrics.py` & `open-cravat-2.6.1/cravat/cravat_metrics.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/cravat_pack.py` & `open-cravat-2.6.1/cravat/cravat_pack.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/cravat_report.py` & `open-cravat-2.6.1/cravat/cravat_report.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/cravat_test.py` & `open-cravat-2.6.1/cravat/cravat_test.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/cravat_util.py` & `open-cravat-2.6.1/cravat/cravat_util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/cravat_web.py` & `open-cravat-2.6.1/cravat/cravat_web.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/example_input` & `open-cravat-2.6.1/cravat/example_input`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/exceptions.py` & `open-cravat-2.6.1/cravat/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/inout.py` & `open-cravat-2.6.1/cravat/inout.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/liftover/hg18ToHg38.over.chain` & `open-cravat-2.6.1/cravat/liftover/hg18ToHg38.over.chain`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/liftover/hg19ToHg38.over.chain` & `open-cravat-2.6.1/cravat/liftover/hg19ToHg38.over.chain`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/mp_runners.py` & `open-cravat-2.6.1/cravat/mp_runners.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/oc.py` & `open-cravat-2.6.1/cravat/oc.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/store_utils.py` & `open-cravat-2.6.1/cravat/store_utils.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/util.py` & `open-cravat-2.6.1/cravat/util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/vcfanno.py` & `open-cravat-2.6.1/cravat/vcfanno.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 import subprocess
 import pathlib
 from io import StringIO
 from collections import OrderedDict
 import cravat
 import vcf
 import json
-from Bio import bgzf
 from cravat.inout import AllMappingsParser
+try:
+    from Bio import bgzf
+except ModuleNotFoundError:
+    bgzf = None
+    pass
 
 # from vcf_line_processor import VCFLineProcessor
 
 class VCFLineProcessor(object):
 
     perc_encode = [
         [r'%', r'%25'],
@@ -392,14 +396,18 @@
         with gzip.open(self.input_path, mode='rt') as gzip_file:
             header_count = self.process_header(gzip_file)
             self.multi_process_data(gzip_file)
 
         self.merge_output()
 
 def vcfanno(args):
+    try:
+        from Bio import bgzf
+    except ModuleNotFoundError:
+        raise ModuleNotFoundError('vcfanno requires biopython. Try running "pip install biopython".')
     input_path = pathlib.Path(args.input_path)
     if args.output_path is not None:
         output_path = args.output_path
     else:
         output_path = pathlib.Path(str(input_path)+'.oc.vcf.gz')
     handler = logging.StreamHandler(sys.stdout)
     handler.setLevel(logging.DEBUG)
```

### Comparing `open-cravat-2.6.0/cravat/webresult/css/pqselect.min.css` & `open-cravat-2.6.1/cravat/webresult/css/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/email.png` & `open-cravat-2.6.1/cravat/webresult/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/favicon.ico` & `open-cravat-2.6.1/cravat/webresult/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/favicon.png` & `open-cravat-2.6.1/cravat/webresult/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/fonts/roboto-bold-webfont.woff` & `open-cravat-2.6.1/cravat/webresult/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/fonts/roboto-bold-webfont.woff2` & `open-cravat-2.6.1/cravat/webresult/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/fonts/roboto-light-webfont.woff` & `open-cravat-2.6.1/cravat/webresult/fonts/roboto-light-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/fonts/roboto-light-webfont.woff2` & `open-cravat-2.6.1/cravat/webresult/fonts/roboto-light-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/fonts/roboto-medium-webfont.woff` & `open-cravat-2.6.1/cravat/webresult/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/fonts/roboto-medium-webfont.woff2` & `open-cravat-2.6.1/cravat/webresult/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff` & `open-cravat-2.6.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2` & `open-cravat-2.6.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/arrow-spinner-static.gif` & `open-cravat-2.6.1/cravat/webresult/images/arrow-spinner-static.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/arrow-spinner.gif` & `open-cravat-2.6.1/cravat/webresult/images/arrow-spinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/arrows-move.svg` & `open-cravat-2.6.1/cravat/webresult/images/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/back_arrow.png` & `open-cravat-2.6.1/cravat/webresult/images/back_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/bigSpinner.gif` & `open-cravat-2.6.1/cravat/webresult/images/bigSpinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/camera.png` & `open-cravat-2.6.1/cravat/webresult/images/camera.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/camera.svg` & `open-cravat-2.6.1/cravat/webresult/images/camera.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/close-button.png` & `open-cravat-2.6.1/cravat/webresult/images/close-button.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/close.png` & `open-cravat-2.6.1/cravat/webresult/images/close.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/close.svg` & `open-cravat-2.6.1/cravat/webresult/images/close.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/close_icon.png` & `open-cravat-2.6.1/cravat/webresult/images/close_icon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/download-material-black.png` & `open-cravat-2.6.1/cravat/webresult/images/download-material-black.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/download-material-blue.png` & `open-cravat-2.6.1/cravat/webresult/images/download-material-blue.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/download.svg` & `open-cravat-2.6.1/cravat/webresult/images/download.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/help_16x16.gif` & `open-cravat-2.6.1/cravat/webresult/images/help_16x16.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/help_icon.png` & `open-cravat-2.6.1/cravat/webresult/images/help_icon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/loading-gif-animation.gif` & `open-cravat-2.6.1/cravat/webresult/images/loading-gif-animation.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/mail.png` & `open-cravat-2.6.1/cravat/webresult/images/mail.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/menu.png` & `open-cravat-2.6.1/cravat/webresult/images/menu.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/openNewTab.png` & `open-cravat-2.6.1/cravat/webresult/images/openNewTab.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/package.png` & `open-cravat-2.6.1/cravat/webresult/images/package.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/pencil.png` & `open-cravat-2.6.1/cravat/webresult/images/pencil.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/pin-2.png` & `open-cravat-2.6.1/cravat/webresult/images/pin-2.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/pin.png` & `open-cravat-2.6.1/cravat/webresult/images/pin.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/pin.svg` & `open-cravat-2.6.1/cravat/webresult/images/pin.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/plus-circle-dotted.svg` & `open-cravat-2.6.1/cravat/webresult/images/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/question.png` & `open-cravat-2.6.1/cravat/webresult/images/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/resize.jpg` & `open-cravat-2.6.1/cravat/webresult/images/resize.jpg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/save.png` & `open-cravat-2.6.1/cravat/webresult/images/save.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/save_new.png` & `open-cravat-2.6.1/cravat/webresult/images/save_new.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/search.png` & `open-cravat-2.6.1/cravat/webresult/images/search.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/sorry.png` & `open-cravat-2.6.1/cravat/webresult/images/sorry.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/spinCircle.gif` & `open-cravat-2.6.1/cravat/webresult/images/spinCircle.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/spinner.gif` & `open-cravat-2.6.1/cravat/webresult/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/triangle-down.png` & `open-cravat-2.6.1/cravat/webresult/images/triangle-down.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/triangle-right.png` & `open-cravat-2.6.1/cravat/webresult/images/triangle-right.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/upload-material-black.png` & `open-cravat-2.6.1/cravat/webresult/images/upload-material-black.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/images/upload-material-blue.png` & `open-cravat-2.6.1/cravat/webresult/images/upload-material-blue.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/index.html` & `open-cravat-2.6.1/cravat/webresult/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/Chart.js` & `open-cravat-2.6.1/cravat/webresult/js/Chart.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/dom-to-image.min.js` & `open-cravat-2.6.1/cravat/webresult/js/dom-to-image.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/download.js` & `open-cravat-2.6.1/cravat/webresult/js/download.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/graphics.js` & `open-cravat-2.6.1/cravat/webresult/js/graphics.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-3.2.1.min.js` & `open-cravat-2.6.1/cravat/webresult/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json` & `open-cravat-2.6.1/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery.tools.min.js` & `open-cravat-2.6.1/cravat/webresult/js/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/jquery.url.js` & `open-cravat-2.6.1/cravat/webresult/js/jquery.url.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/packery.pkgd.js` & `open-cravat-2.6.1/cravat/webresult/js/packery.pkgd.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/EULA.pdf`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/loading.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/images/sprite.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/readme.txt` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/readme.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js` & `open-cravat-2.6.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/pqselect.min.js` & `open-cravat-2.6.1/cravat/webresult/js/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/js/raphael-min.js` & `open-cravat-2.6.1/cravat/webresult/js/raphael-min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/jsonreporter.py` & `open-cravat-2.6.1/cravat/webresult/jsonreporter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/css/singlevariantpage.css` & `open-cravat-2.6.1/cravat/webresult/nocache/css/singlevariantpage.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/css/style.css` & `open-cravat-2.6.1/cravat/webresult/nocache/css/style.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/css/widget.css` & `open-cravat-2.6.1/cravat/webresult/nocache/css/widget.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/filter.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/filter.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/infomgr.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/infomgr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/main.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/main.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/setup.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/setup.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/showvariant.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/showvariant.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/singlevariantpage.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/singlevariantpage.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/util.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/util.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/variables.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/variables.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/js/widgethelper.js` & `open-cravat-2.6.1/cravat/webresult/nocache/js/widgethelper.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/nocache/variant.html` & `open-cravat-2.6.1/cravat/webresult/nocache/variant.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/question.png` & `open-cravat-2.6.1/cravat/webresult/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webresult/webresult.py` & `open-cravat-2.6.1/cravat/webresult/webresult.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/cravat_store.css` & `open-cravat-2.6.1/cravat/webstore/cravat_store.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/favicon.ico` & `open-cravat-2.6.1/cravat/webstore/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/chat-dots.svg` & `open-cravat-2.6.1/cravat/webstore/images/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/chat-left-text.svg` & `open-cravat-2.6.1/cravat/webstore/images/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/done.png` & `open-cravat-2.6.1/cravat/webstore/images/done.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/email.png` & `open-cravat-2.6.1/cravat/webstore/images/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/empty.png` & `open-cravat-2.6.1/cravat/webstore/images/empty.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/favicon.png` & `open-cravat-2.6.1/cravat/webstore/images/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/folder.png` & `open-cravat-2.6.1/cravat/webstore/images/folder.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/genericmodulelogo.png` & `open-cravat-2.6.1/cravat/webstore/images/genericmodulelogo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/hamburger.png` & `open-cravat-2.6.1/cravat/webstore/images/hamburger.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/left_arrow.png` & `open-cravat-2.6.1/cravat/webstore/images/left_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/logo.png` & `open-cravat-2.6.1/cravat/webstore/images/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/new.png` & `open-cravat-2.6.1/cravat/webstore/images/new.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/question.png` & `open-cravat-2.6.1/cravat/webstore/images/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/images/right_arrow.png` & `open-cravat-2.6.1/cravat/webstore/images/right_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/jquery-3.3.1.min.js` & `open-cravat-2.6.1/cravat/webstore/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/js/showdown-1.9.1.min.js` & `open-cravat-2.6.1/cravat/webstore/js/showdown-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/js/showdown.min.js.map` & `open-cravat-2.6.1/cravat/webstore/js/showdown.min.js.map`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/nocache/webstore.css` & `open-cravat-2.6.1/cravat/webstore/nocache/webstore.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/nocache/webstore.js` & `open-cravat-2.6.1/cravat/webstore/nocache/webstore.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/sse.py` & `open-cravat-2.6.1/cravat/webstore/sse.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/store_handlers.py` & `open-cravat-2.6.1/cravat/webstore/store_handlers.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/webstore/webstore.py` & `open-cravat-2.6.1/cravat/webstore/webstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,27 +246,24 @@
     install_queue.put(data)
     deps = au.get_install_deps(module_name, module_version)
     for dep_name, dep_version in deps.items():
         install_queue.put({'module':dep_name,'version':dep_version})
     return web.Response(text = 'queued ' + queries['module'])
 
 async def get_base_modules (request):
-    global system_conf
-    base_modules = system_conf['base_modules']
-    return web.json_response(base_modules)
+    return web.json_response(constants.base_modules)
 
 async def install_base_modules (request):
     global servermode
     if servermode and server_ready:
         r = await cravat_multiuser.is_admin_loggedin(request)
         if r == False:
             response = 'failed'
             return web.json_response(response)
-    base_modules = system_conf.get(constants.base_modules_key,[])
-    for module in base_modules:
+    for module in constants.base_modules:
         install_queue.put({'module': module, 'version': None})
     response = 'queued'
     return web.json_response(response)
 
 async def get_md (request):
     modules_dir = au.get_modules_dir()
     return web.Response(text=modules_dir)
```

### Comparing `open-cravat-2.6.0/cravat/webstore/ws.js` & `open-cravat-2.6.1/cravat/webstore/ws.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/Chart.bundle.min.js` & `open-cravat-2.6.1/cravat/websubmit/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/arrow.png` & `open-cravat-2.6.1/cravat/websubmit/arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/down.png` & `open-cravat-2.6.1/cravat/websubmit/down.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/email.png` & `open-cravat-2.6.1/cravat/websubmit/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/favicon.ico` & `open-cravat-2.6.1/cravat/websubmit/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/favicon.png` & `open-cravat-2.6.1/cravat/websubmit/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/help.png` & `open-cravat-2.6.1/cravat/websubmit/help.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/house-solid.svg` & `open-cravat-2.6.1/cravat/websubmit/house-solid.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/input-examples/cravat.hg38.txt` & `open-cravat-2.6.1/cravat/websubmit/input-examples/cravat.hg38.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/input-examples/vcf.hg38.txt` & `open-cravat-2.6.1/cravat/websubmit/input-examples/vcf.hg38.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/jquery-3.3.1.min.js` & `open-cravat-2.6.1/cravat/websubmit/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/logo.png` & `open-cravat-2.6.1/cravat/websubmit/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/logo_transparent.png` & `open-cravat-2.6.1/cravat/websubmit/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/nocache/broken_wheel.gif` & `open-cravat-2.6.1/cravat/websubmit/nocache/broken_wheel.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/nocache/core.js` & `open-cravat-2.6.1/cravat/websubmit/nocache/core.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/nocache/header.js` & `open-cravat-2.6.1/cravat/websubmit/nocache/header.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/nocache/index.html` & `open-cravat-2.6.1/cravat/websubmit/nocache/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -68,65 +68,56 @@
 </div>
 
 <div id='submitdiv' class='appdiv'>
     <table><tr><td valign='top' style=''>
     <div id='submitcontentdiv'>
         <div id="submit-form">
             <div id='submit-variant-div' class='container'>
+                <div class='divbanner'></div>
                 <span class='divtitle'>Variants</span>
-                <table>
-                    <tr>
-                        <td>
+                <div class="flexcol">
+                    <label for="assembly-select" class="input-label">Genome:</label>
                             <div id='assembly-select-div'>
-                                Genome:
                                 <select id="assembly-select">
                                     <option value="hg38">hg38/GRCh38</option>
                                     <option value="hg19" selected=true>hg19/GRCh37</option>
                                     <option value="hg18">hg18/GRCh36</option>
                                 </select>
                             </div>
-                        </td>
-                    </tr>
-                    <tr>
-                        <td valign='top' class='variant-input-border-bottom' title="Upload file(s). Select multiple files using ctrl and shift keys">
-                                <br />
-                            <input type="file" name="input-file" id="input-file" multiple/>
-                            <label for="input-file">Add input files</label>
-                            <button id='clear_inputfilelist_button' class='butn' style='display: none;'>Clear file(s)</button>
+                        <span class='variant-input-border-bottom' title="Upload file(s). Select multiple files using ctrl and shift keys">
+                            <div class="flexrow">
+                                <input type="file" name="input-file" id="input-file" multiple/>
+                                <label for="input-file">Add input files</label>
+                                <button id='clear_inputfilelist_button' class='butn' style='display: none;'>Clear file(s)</button>
+                            </div>
                             <div id="mult-inputs-message" style="display: none; margin-top: 4px;">
                                 <div id="mult-inputs-list"></div>
                             </div>
-                        </td>
-                    </tr>
-                    <tr>
-                        <td valign='top' class='variant-input-border-bottom' style='text-align: left;'>
-                            <br />
-                            <div style='text-align: left;'>
-                                <textarea rows="3" id="input-text" style='' placeholder="Enter variants in a supported input format such as VCF or TSV, or type a list of the paths to input files in the server."></textarea>
+                        </span>
+                            <div class='or input-label'>OR</div>
+                            <div>
+                                <textarea rows="3" id="input-text" placeholder="Enter variants in a supported input format such as VCF or TSV, or type a list of the paths to input files in the server."></textarea>
                             </div>
                             <select id='submit-input-format-select' disabled style='display: none;'>
                                 <option value=''>Detect</option>
                             </select>
-                            <span style='font-size: 13px;'>Example:</span>
-                            <button value="vcf" class='butn input-example-button'>VCF</button>
-                            <button value="cravat" class='butn input-example-button'>TSV</button>
-                            <div class='or'>OR</div>
-                        </td>
-                    </tr>
-                    <tr>
-                        <td>
-                            <div style='margin-top: 14px;'>
-                                <span style='vertical-align: top;'>Note: </span>
+                            <div class="flexrow">
+                                <span class="input-label">Example:</span>
+                            </div>
+                            <div class="flexrow">
+                                <button value="vcf" class='butn input-example-button'>VCF</button>
+                                <button value="cravat" class='butn input-example-button'>TSV</button>
+                                <button value="hgvs" class='butn input-example-button'>HGVS</button>
+                            </div>
+                            <div class="flexcol">
+                                <span class="input-label">Note: </span>
                                 <textarea id='jobnoteinput' rows='1' placeholder='Enter a note for the analysis (optional)'></textarea>
                             </div>
-                        </td>
-                    </tr>
-                </table>
-                <div class='divbanner'></div>
-                <div class='chevrondiv'><div class='chevron chevron1to2'></div></div>
+                </div>
+                <div class='chevrondiv flexrow'>&nbsp;<div class='chevron chevron1to2'></div></div>
             </div>
   
             <div id='modchoose' class='container'>
                 <div id="modchoose-header">
                     <div id='show-annotator' class='divtitle'>Annotations</div>
                     <div id='show-package' class='divtitle' style="display:none;">Packages</div>
                 </div>
@@ -143,18 +134,18 @@
                     <div id="divbanner-pkg" class="divbanner-split" style="background-color:#3175b0"></div>
                 </div>
             </div>
             <div id='addtl-analysis-div' class='container' style='display:none'>
                 <span class='divtitle'>Additional Analysis</span>
                 <div id='addtl-analysis-content'></div>
                 <div class='divbanner'></div>
+                <div class='chevrondiv'><div class='chevron chevron2to3'></div></div>
             </div>
+            <div class="annotate-container"><button id="submit-job-button" class='butn submit-annotate-button'>ANNOTATE</button></div>
         </div>
-        <div class='chevrondiv'><div class='chevron chevron2to3'></div></div>
-        <div style='text-align: center;'><button id="submit-job-button" class='butn submit-annotate-button'>ANNOTATE</button></div>
     </div>
 
     </td><td valign='top' style='padding-left: 5px; width: 100%;'>
     <div id="jobdiv">
         <div id="jobdivspinnerdiv" class="spinnerdiv"><img src="/submit/nocache/broken_wheel.gif"></img></div>
         <div style='width: 100%; text-align: right;'>
             <button id='refresh-jobs-table-btn' class='butn'>&#x21ba;</button>
```

#### html2text {}

```diff
@@ -5,27 +5,27 @@
 System update available Update
 Version:
 [Open Cravat Logo]
 _[_/_s_u_b_m_i_t_/_h_o_u_s_e_-_s_o_l_i_d_._s_v_g_]_[_/_r_e_s_u_l_t_/_i_m_a_g_e_s_/_q_u_e_s_t_i_o_n_._p_n_g_]_[_/_r_e_s_u_l_t_/_i_m_a_g_e_s_/_m_a_i_l_._p_n_g_]
 [/submit/setting.png]
 [/submit/nointernet.png]
 Variants          [/submit/nocache/broken_wheel.gif]
-Genome:[One of:   ↺
-hg38/GRCh38/hg19/ JJoobb IInnppuutt VVaarriiaannttss AAnnnnoottaattoorrss GGeennoommee NNoottee SSttaattuuss DDoowwnnllooaadd DDeelleettee
-GRCh37/hg18/      IIDD  FFiillee
-GRCh36]           < >
-
+Genome:           ↺
+[One of: hg38/    JJoobb IInnppuutt VVaarriiaannttss AAnnnnoottaattoorrss GGeennoommee NNoottee SSttaattuuss DDoowwnnllooaadd DDeelleettee
+GRCh38/hg19/      IIDD  FFiillee
+GRCh37/hg18/      < >
+GRCh36]
 [File]Add input
 files Clear file
 (s)
-
-[One of:
-Detect]Example:
-VCF TSV
 OR
+[One of: Detect]
+Example:
+VCF TSV HGVS
+ 
 Annotations
 Packages
 [/submit/nocache/
 broken_wheel.gif]
 Additional
 Analysis
 ANNOTATE
```

### Comparing `open-cravat-2.6.0/cravat/websubmit/nocache/moduleinfo.js` & `open-cravat-2.6.1/cravat/websubmit/nocache/moduleinfo.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/nocache/websubmit.css` & `open-cravat-2.6.1/cravat/websubmit/nocache/websubmit.css`

 * *Files 2% similar despite different names*

```diff
@@ -105,29 +105,28 @@
     margin-right: 10px;
 }
 
 .container * {
     font-size: 13px;
 }
 
+.annotate-container {
+    margin-right: 10px;
+}
+
 .divtitle {
     font-family: sourcesanspro-bold;
     font-size: 22px;
     color: #ffffff;
     top: -15px;
     position: relative;
     z-index: 1;
 }
 
 .or {
-    position: absolute;
-    top: -17px;
-    left: 30px;
-    padding-top: 5px;
-    padding-bottom: 5px;
     width: 26px;
     color: #4b4b4b;
 }
 
 .divbanner {
     position: absolute;
     background-color: #385487;
@@ -238,27 +237,45 @@
     padding: 14px;
     font-size: 13px;
 }
 
 .variant-input-border-bottom {
     position: relative;
     border-bottom: 1px dotted #cbcbcb;
-    padding-bottom: 20px;
+    padding-top: 1em;
+}
+
+.flexcol {
+    display: flex;
+    flex-direction: column;
+}
+
+.flexrow {
+    display: flex;
+    flex-direction: row;
 }
 
 #submitcontentdiv {
     width: 390px;
 }
 
 #jobnoteinput {
-    width: calc(100% - 44px);
+    width: calc(100% - 8px);
+    resize: vertical;
 }
 
 #input-text {
-    width: calc(100% + 40px);
+    width: calc(100% - 8px);
+    height: 4em;
+    transition: all ease .2s;
+    resize: vertical;
+}
+
+#input-text.input-text-selected {
+    height: 15em;
 }
 
 #refresh-jobs-table-btn {
     width: 14px; 
     height: 17px;
     position: absolute; 
     top: 8px; 
@@ -513,27 +530,32 @@
 
 .butn:hover {
   background: #5cb5e5;
   text-decoration: none;
 }
 
 .input-example-button {
-    width: 35px;
-    height: 23px;
+    min-width: 35px;
     font-size: 11px;
     background-color: #6e593a;
+    padding: 3px 6px;
+}
+
+.input-label {
+    font-size: 13px;
+    margin-top: 0.3em;
 }
 
 .submit-annotate-button {
     font-size: 24px; 
-    width: 391px;
+    width: 100%;
     padding: 9px;
     background-color: #de6342;
-    position: absolute;
-    left: 1px;
+    margin-left: 0;
+    margin-top: 1em;
 }
 
 .launch-button {
     background-color: #c5af8d;
 }
 
 .launch-button:hover {
@@ -762,17 +784,14 @@
 }
 
 .chevron1to2:after {
   background-color: #5fa3c6;
 }
 
 .chevron2to3 {
-  position: relative;
-  top: -30px;
-  left: 329px;
 }
 
 .chevron2to3:before {
   background-color: #94d1eb;
 }
 
 .chevron2to3:after {
@@ -904,16 +923,19 @@
     transform: translateX(-50%) translateY(-50%);
     width: 200px;
     height: 30px;
     color: white;
 }
 
 #assembly-select-div {
-    width: fit-content;
-    padding: 2px;
+    width: 100%;
+}
+
+#assembly-select {
+    width: 100%;
 }
 
 .fileaddbutn {
     font-size: 10px;
 }
 
 .btn_overlay {
```

### Comparing `open-cravat-2.6.0/cravat/websubmit/nocache/websubmit.js` & `open-cravat-2.6.1/cravat/websubmit/nocache/websubmit.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1822,20 +1822,20 @@
             OC.mediator.publish('getRemote');
         });
     });
 }
 
 function onClickInputTextArea() {
     let input = document.getElementById('input-text');
-    input.rows = 20;
+    input.classList.add('input-text-selected')
 }
 
 function onBlurInputTextArea() {
     let input = document.getElementById('input-text');
-    input.rows = 1;
+    input.classList.remove('input-text-selected')
 }
 
 function resizePage() {
     var div = document.getElementById('submit-form');
     var h = window.innerHeight - 148;
     div.style.height = h + 'px';
     var div = document.getElementById('jobdiv');
```

### Comparing `open-cravat-2.6.0/cravat/websubmit/nointernet.png` & `open-cravat-2.6.1/cravat/websubmit/nointernet.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/pqselect.dev.customforsubmit.js` & `open-cravat-2.6.1/cravat/websubmit/pqselect.dev.customforsubmit.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/question.png` & `open-cravat-2.6.1/cravat/websubmit/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/refresh.png` & `open-cravat-2.6.1/cravat/websubmit/refresh.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/setting.png` & `open-cravat-2.6.1/cravat/websubmit/setting.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/websubmit/websubmit.py` & `open-cravat-2.6.1/cravat/websubmit/websubmit.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/cravat/wincravat.pyw` & `open-cravat-2.6.1/cravat/wincravat.pyw`

 * *Files identical despite different names*

### Comparing `open-cravat-2.6.0/open_cravat.egg-info/PKG-INFO` & `open-cravat-2.6.1/open_cravat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-cravat
-Version: 2.6.0
+Version: 2.6.1
 Summary: OpenCRAVAT - variant analysis toolkit
 Home-page: https://www.opencravat.org
 Author: Kyle Moad, Kyle Anderson, Madison Larsen, Jeltje van Baren, and Rachel Karchin
 Author-email: support@opencravat.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `open-cravat-2.6.0/open_cravat.egg-info/SOURCES.txt` & `open-cravat-2.6.1/open_cravat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -268,14 +268,15 @@
 cravat/websubmit/pqselect.dev.customforsubmit.js
 cravat/websubmit/question.png
 cravat/websubmit/refresh.png
 cravat/websubmit/setting.png
 cravat/websubmit/threedots.png
 cravat/websubmit/websubmit.py
 cravat/websubmit/input-examples/cravat.hg38.txt
+cravat/websubmit/input-examples/hgvs.hg38.txt
 cravat/websubmit/input-examples/vcf.hg38.txt
 cravat/websubmit/nocache/broken_wheel.gif
 cravat/websubmit/nocache/core.js
 cravat/websubmit/nocache/header.js
 cravat/websubmit/nocache/index.html
 cravat/websubmit/nocache/main.js
 cravat/websubmit/nocache/moduleinfo.js
```

### Comparing `open-cravat-2.6.0/setup.py` & `open-cravat-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 for root, dirs, files in os.walk(os.path.join('cravat', 'websubmit')):
     root_files = [os.path.join('..', root, f) for f in files]
     data_files.extend(root_files)
 
 setup(
     name='open-cravat',
     packages=['cravat'],
-    version='2.6.0',
+    version='2.6.1',
     description='OpenCRAVAT - variant analysis toolkit',
     long_description=readme(),
     author='Kyle Moad, Kyle Anderson, Madison Larsen, Jeltje van Baren, and Rachel Karchin',
     author_email='support@opencravat.org',
     url='https://www.opencravat.org',
     license='',
     package_data={
```

