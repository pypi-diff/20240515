# Comparing `tmp/glances-4.0.3.tar.gz` & `tmp/glances-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glances-4.0.3.tar", last modified: Wed May 15 07:44:11 2024, max compression
+gzip compressed data, was "glances-4.0.4.tar", last modified: Wed May 15 09:25:11 2024, max compression
```

## Comparing `glances-4.0.3.tar` & `glances-4.0.4.tar`

### file list

```diff
@@ -1,406 +1,406 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.409433 glances-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-15 07:44:05.000000 glances-4.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-15 07:44:05.000000 glances-4.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-05-15 07:44:05.000000 glances-4.0.3/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.405433 glances-4.0.3/Glances.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-15 07:44:11.000000 glances-4.0.3/Glances.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-15 07:44:11.000000 glances-4.0.3/Glances.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:44:11.000000 glances-4.0.3/Glances.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 07:44:11.000000 glances-4.0.3/Glances.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-15 07:44:11.000000 glances-4.0.3/Glances.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 07:44:11.000000 glances-4.0.3/Glances.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 07:44:05.000000 glances-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    72478 2024-05-15 07:44:05.000000 glances-4.0.3/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-15 07:44:11.409433 glances-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-15 07:44:05.000000 glances-4.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.341434 glances-4.0.3/conf/
--rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-05-15 07:44:05.000000 glances-4.0.3/conf/glances.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.345434 glances-4.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-15 07:44:05.000000 glances-4.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 07:44:05.000000 glances-4.0.3/docs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.365433 glances-4.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/Glances Logo dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/Glances Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/Glances Text Logo dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/Glances Text Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29273 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/amp-dropbox.png
--rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/amp-python-warning.png
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/amp-python.png
--rw-r--r--   0 runner    (1001) docker     (127)    80498 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/amps.png
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/aws.png
--rw-r--r--   0 runner    (1001) docker     (127)    44160 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/browser.png
--rw-r--r--   0 runner    (1001) docker     (127)    21111 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/cloud.png
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/connected.png
--rw-r--r--   0 runner    (1001) docker     (127)    29245 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/connections.png
--rw-r--r--   0 runner    (1001) docker     (127)    34093 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/containers.png
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/cpu-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/cpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/disconnected.png
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/diskio.png
--rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/events.png
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/folders.png
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/fs.png
--rw-r--r--   0 runner    (1001) docker     (127)    56273 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-architecture.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)   123499 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)    92793 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-cgraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)   114983 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-flame.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-influxdb.png
--rw-r--r--   0 runner    (1001) docker     (127)    33567 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-memory-profiling-with-history.png
--rw-r--r--   0 runner    (1001) docker     (127)    31797 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-memory-profiling-without-history.png
--rw-r--r--   0 runner    (1001) docker     (127)    29500 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-pyinstrument.html
--rw-r--r--   0 runner    (1001) docker     (127)   295283 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-responsive-webdesign.png
--rw-r--r--   0 runner    (1001) docker     (127)   435038 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/glances-summary.png
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/gpu.png
--rw-r--r--   0 runner    (1001) docker     (127)   141657 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/grafana.png
--rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/graph-load.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14415 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/hddtemp.png
--rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/header.png
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/ip.png
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/irq.png
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/load.png
--rw-r--r--   0 runner    (1001) docker     (127)    20009 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/loadpercent.png
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/mem-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/mem.png
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/monitored.png
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/network.png
--rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/per-cpu.png
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/pergpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/ports.png
--rw-r--r--   0 runner    (1001) docker     (127)    63154 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/processlist-extended.png
--rw-r--r--   0 runner    (1001) docker     (127)   160408 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/processlist-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)    53684 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/processlist-top.png
--rw-r--r--   0 runner    (1001) docker     (127)   227401 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/processlist-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)   151590 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/processlist.png
--rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/prometheus_exporter.png
--rw-r--r--   0 runner    (1001) docker     (127)    91914 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/prometheus_server.png
--rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/quicklook-percpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/quicklook.png
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/raid.png
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/reddit.png
--rw-r--r--   0 runner    (1001) docker     (127)  1089975 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/screencast.gif
--rw-r--r--   0 runner    (1001) docker     (127)   265567 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/screenshot-web.png
--rw-r--r--   0 runner    (1001) docker     (127)    36097 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/screenshot-web2.png
--rw-r--r--   0 runner    (1001) docker     (127)  1098062 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/screenshot-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)   508044 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/sensors.png
--rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/smart.png
--rw-r--r--   0 runner    (1001) docker     (127)    41952 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/sparkline.png
--rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/trend.png
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/twitter-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_static/wifi.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.365433 glances-4.0.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-15 07:44:05.000000 glances-4.0.3/docs/_templates/links.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.369433 glances-4.0.3/docs/aoa/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/actions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/amps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/cloud.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/connections.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/containers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/cpu.rst
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/diskio.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/folders.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/fs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/gpu.rst
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/hddtemp.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/header.rst
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/irq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/load.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/memory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/network.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/ports.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/ps.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/quicklook.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/raid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/sensors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/smart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 07:44:05.000000 glances-4.0.3/docs/aoa/wifi.rst
--rw-r--r--   0 runner    (1001) docker     (127)    50249 2024-05-15 07:44:05.000000 glances-4.0.3/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-05-15 07:44:05.000000 glances-4.0.3/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-15 07:44:05.000000 glances-4.0.3/docs/cmds.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-05-15 07:44:05.000000 glances-4.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-15 07:44:05.000000 glances-4.0.3/docs/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.369433 glances-4.0.3/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-15 07:44:05.000000 glances-4.0.3/docs/dev/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   328258 2024-05-15 07:44:05.000000 glances-4.0.3/docs/dev/glances-cprofile.png
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-15 07:44:05.000000 glances-4.0.3/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 07:44:05.000000 glances-4.0.3/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 07:44:05.000000 glances-4.0.3/docs/glances.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.373433 glances-4.0.3/docs/gw/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/cassandra.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/couchdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/csv.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/elastic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/graph.rst
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/graphite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/influxdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/json.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/mongodb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/mqtt.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/opentsdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/rabbitmq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/restful.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/riemann.rst
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/statsd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 07:44:05.000000 glances-4.0.3/docs/gw/zeromq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 07:44:05.000000 glances-4.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 07:44:05.000000 glances-4.0.3/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-15 07:44:05.000000 glances-4.0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.373433 glances-4.0.3/docs/man/
--rwxr-xr-x   0 runner    (1001) docker     (127)    19253 2024-05-15 07:44:05.000000 glances-4.0.3/docs/man/glances.1
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-15 07:44:05.000000 glances-4.0.3/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-15 07:44:05.000000 glances-4.0.3/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 07:44:05.000000 glances-4.0.3/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.377433 glances-4.0.3/glances/
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-15 07:44:05.000000 glances-4.0.3/glances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 07:44:05.000000 glances-4.0.3/glances/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-15 07:44:05.000000 glances-4.0.3/glances/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.377433 glances-4.0.3/glances/amps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/amps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-15 07:44:05.000000 glances-4.0.3/glances/amps/amp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/amps/default/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-15 07:44:05.000000 glances-4.0.3/glances/amps/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/amps/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-15 07:44:05.000000 glances-4.0.3/glances/amps/nginx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/amps/systemd/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-15 07:44:05.000000 glances-4.0.3/glances/amps/systemd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/amps/systemv/
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-15 07:44:05.000000 glances-4.0.3/glances/amps/systemv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-15 07:44:05.000000 glances-4.0.3/glances/amps_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-15 07:44:05.000000 glances-4.0.3/glances/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-05-15 07:44:05.000000 glances-4.0.3/glances/autodiscover.py
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-15 07:44:05.000000 glances-4.0.3/glances/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10101 2024-05-15 07:44:05.000000 glances-4.0.3/glances/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-15 07:44:05.000000 glances-4.0.3/glances/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-15 07:44:05.000000 glances-4.0.3/glances/cpu_percent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-15 07:44:05.000000 glances-4.0.3/glances/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-15 07:44:05.000000 glances-4.0.3/glances/events_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_cassandra/
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_cassandra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_couchdb/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_couchdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_csv/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_csv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_elasticsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_graph/
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_graphite/
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_graphite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_influxdb/
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_influxdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_influxdb2/
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_influxdb2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_json/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_mqtt/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5011 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_opentsdb/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_opentsdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_prometheus/
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_prometheus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_restful/
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_restful/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_riemann/
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_riemann/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_statsd/
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_statsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.381433 glances-4.0.3/glances/exports/glances_zeromq/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-15 07:44:05.000000 glances-4.0.3/glances/exports/glances_zeromq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-15 07:44:05.000000 glances-4.0.3/glances/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-15 07:44:05.000000 glances-4.0.3/glances/folder_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-05-15 07:44:05.000000 glances-4.0.3/glances/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-15 07:44:05.000000 glances-4.0.3/glances/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-15 07:44:05.000000 glances-4.0.3/glances/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    30810 2024-05-15 07:44:05.000000 glances-4.0.3/glances/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outdated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.385433 glances-4.0.3/glances/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)    48721 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_curses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_curses_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    29836 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_restful_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_sparklines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_stdout_apidoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_stdout_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_stdout_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_stdout_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/glances_unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.385433 glances-4.0.3/glances/outputs/static/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.385433 glances-4.0.3/glances/outputs/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/css/bootstrap.less
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/css/style.scss
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/css/variables.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.389433 glances-4.0.3/glances/outputs/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/images/glances.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.389433 glances-4.0.3/glances/outputs/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/App.vue
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.393433 glances-4.0.3/glances/outputs/static/js/components/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/help.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-alert.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-amps.vue
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-cloud.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-connections.vue
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-containers.vue
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-cpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-diskio.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-folders.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-fs.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-gpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-ip.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-irq.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-load.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-mem-more.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-mem.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-memswap.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-network.vue
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-now.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-percpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-ports.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-process.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-processcount.vue
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-processlist.vue
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-quicklook.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-raid.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-sensors.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-smart.vue
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-system.vue
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-uptime.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/components/plugin-wifi.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/filters.js
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/services.js
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/store.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/js/uiconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   452411 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.393433 glances-4.0.3/glances/outputs/static/public/
--rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   448748 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/public/glances.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.393433 glances-4.0.3/glances/outputs/static/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-15 07:44:05.000000 glances-4.0.3/glances/outputs/static/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-15 07:44:05.000000 glances-4.0.3/glances/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-15 07:44:05.000000 glances-4.0.3/glances/password_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.393433 glances-4.0.3/glances/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/__pycache__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/alert/
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/amps/
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/amps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/containers/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/containers/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/containers/engines/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/containers/engines/podman.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/containers/stats_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/cpu/
--rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/cpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/diskio/
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/diskio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/folders/
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/folders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/fs/
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/fs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/gpu/
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/gpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/gpu/cards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/gpu/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/gpu/cards/amd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/gpu/cards/nvidia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/help/
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/help/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/ip/
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/irq/
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/irq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.397433 glances-4.0.3/glances/plugins/load/
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/mem/
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/mem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/memswap/
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/memswap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/network/
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/now/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/now/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/percpu/
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/percpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47262 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/plugin/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/ports/
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/ports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/processcount/
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/processcount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/processlist/
--rw-r--r--   0 runner    (1001) docker     (127)    36694 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/processlist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/psutilversion/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/psutilversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/quicklook/
--rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/quicklook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/raid/
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/raid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/sensors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/sensors/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/sensors/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/sensors/sensor/glances_batpercent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/sensors/sensor/glances_hddtemp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/smart/
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/smart/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/uptime/
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/uptime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/version/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:44:11.401433 glances-4.0.3/glances/plugins/wifi/
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-15 07:44:05.000000 glances-4.0.3/glances/plugins/wifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-15 07:44:05.000000 glances-4.0.3/glances/ports_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    26474 2024-05-15 07:44:05.000000 glances-4.0.3/glances/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-15 07:44:05.000000 glances-4.0.3/glances/programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-15 07:44:05.000000 glances-4.0.3/glances/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-15 07:44:05.000000 glances-4.0.3/glances/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-15 07:44:05.000000 glances-4.0.3/glances/snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-05-15 07:44:05.000000 glances-4.0.3/glances/standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-15 07:44:05.000000 glances-4.0.3/glances/static_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-15 07:44:05.000000 glances-4.0.3/glances/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-15 07:44:05.000000 glances-4.0.3/glances/stats_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-15 07:44:05.000000 glances-4.0.3/glances/stats_client_snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 07:44:05.000000 glances-4.0.3/glances/stats_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-15 07:44:05.000000 glances-4.0.3/glances/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-15 07:44:05.000000 glances-4.0.3/glances/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-15 07:44:05.000000 glances-4.0.3/glances/web_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-15 07:44:05.000000 glances-4.0.3/glances/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-15 07:44:05.000000 glances-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:44:11.409433 glances-4.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4418 2024-05-15 07:44:05.000000 glances-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.852857 glances-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-15 09:25:06.000000 glances-4.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-15 09:25:06.000000 glances-4.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-05-15 09:25:06.000000 glances-4.0.4/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.848857 glances-4.0.4/Glances.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 09:25:11.000000 glances-4.0.4/Glances.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 09:25:06.000000 glances-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    72575 2024-05-15 09:25:06.000000 glances-4.0.4/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-15 09:25:11.852857 glances-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-15 09:25:06.000000 glances-4.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.788856 glances-4.0.4/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-05-15 09:25:06.000000 glances-4.0.4/conf/glances.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.788856 glances-4.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-15 09:25:06.000000 glances-4.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 09:25:06.000000 glances-4.0.4/docs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.808857 glances-4.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/Glances Logo dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/Glances Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/Glances Text Logo dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/Glances Text Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29273 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/amp-dropbox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/amp-python-warning.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/amp-python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80498 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/amps.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/aws.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44160 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21111 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/cloud.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/connected.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29245 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/connections.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34093 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/containers.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/cpu-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/cpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/disconnected.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/diskio.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/events.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/folders.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/fs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56273 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-architecture.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)   123499 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92793 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-cgraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   114983 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-flame.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-influxdb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33567 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-memory-profiling-with-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31797 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-memory-profiling-without-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29500 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-pyinstrument.html
+-rw-r--r--   0 runner    (1001) docker     (127)   295283 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-responsive-webdesign.png
+-rw-r--r--   0 runner    (1001) docker     (127)   435038 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/glances-summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/gpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141657 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/grafana.png
+-rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/graph-load.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14415 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/hddtemp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/ip.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/irq.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/load.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20009 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/loadpercent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/mem-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/mem.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/monitored.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/network.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/per-cpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/pergpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/ports.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63154 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist-extended.png
+-rw-r--r--   0 runner    (1001) docker     (127)   160408 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53684 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist-top.png
+-rw-r--r--   0 runner    (1001) docker     (127)   227401 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151590 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/processlist.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/prometheus_exporter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91914 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/prometheus_server.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/quicklook-percpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/quicklook.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/raid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/reddit.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1089975 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screencast.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   265567 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screenshot-web.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36097 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screenshot-web2.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1098062 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screenshot-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)   508044 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/sensors.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/smart.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41952 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/sparkline.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/trend.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/twitter-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_static/wifi.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.808857 glances-4.0.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-15 09:25:06.000000 glances-4.0.4/docs/_templates/links.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.812857 glances-4.0.4/docs/aoa/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/actions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/amps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/cloud.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/cpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/diskio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/folders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/fs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/gpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/hddtemp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/header.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/irq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/load.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/memory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/network.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/ports.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/ps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/quicklook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/raid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/smart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 09:25:06.000000 glances-4.0.4/docs/aoa/wifi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    50249 2024-05-15 09:25:06.000000 glances-4.0.4/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-05-15 09:25:06.000000 glances-4.0.4/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-15 09:25:06.000000 glances-4.0.4/docs/cmds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-05-15 09:25:06.000000 glances-4.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-15 09:25:06.000000 glances-4.0.4/docs/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.812857 glances-4.0.4/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-15 09:25:06.000000 glances-4.0.4/docs/dev/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   328258 2024-05-15 09:25:07.000000 glances-4.0.4/docs/dev/glances-cprofile.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-15 09:25:07.000000 glances-4.0.4/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 09:25:07.000000 glances-4.0.4/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 09:25:07.000000 glances-4.0.4/docs/glances.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.816857 glances-4.0.4/docs/gw/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/cassandra.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/couchdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/elastic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/graphite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/influxdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/json.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/kafka.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/mongodb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/mqtt.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/opentsdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/rabbitmq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/restful.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/riemann.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 09:25:07.000000 glances-4.0.4/docs/gw/zeromq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 09:25:07.000000 glances-4.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 09:25:07.000000 glances-4.0.4/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-15 09:25:07.000000 glances-4.0.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.816857 glances-4.0.4/docs/man/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19253 2024-05-15 09:25:07.000000 glances-4.0.4/docs/man/glances.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-15 09:25:07.000000 glances-4.0.4/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-15 09:25:07.000000 glances-4.0.4/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 09:25:07.000000 glances-4.0.4/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-15 09:25:07.000000 glances-4.0.4/glances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 09:25:07.000000 glances-4.0.4/glances/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-15 09:25:07.000000 glances-4.0.4/glances/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/amp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/nginx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/systemd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/systemd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/amps/systemv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps/systemv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-15 09:25:07.000000 glances-4.0.4/glances/amps_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-15 09:25:07.000000 glances-4.0.4/glances/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-05-15 09:25:07.000000 glances-4.0.4/glances/autodiscover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-15 09:25:07.000000 glances-4.0.4/glances/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10101 2024-05-15 09:25:07.000000 glances-4.0.4/glances/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-15 09:25:07.000000 glances-4.0.4/glances/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-15 09:25:07.000000 glances-4.0.4/glances/cpu_percent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-15 09:25:07.000000 glances-4.0.4/glances/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-15 09:25:07.000000 glances-4.0.4/glances/events_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.820857 glances-4.0.4/glances/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_cassandra/
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_cassandra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_couchdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_couchdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_csv/
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_csv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_elasticsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_graphite/
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_graphite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_influxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_influxdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_influxdb2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_influxdb2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_mqtt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5011 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_opentsdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_opentsdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_prometheus/
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_prometheus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_restful/
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_restful/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_riemann/
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_riemann/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_statsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_statsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.824857 glances-4.0.4/glances/exports/glances_zeromq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-15 09:25:07.000000 glances-4.0.4/glances/exports/glances_zeromq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-15 09:25:07.000000 glances-4.0.4/glances/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-15 09:25:07.000000 glances-4.0.4/glances/folder_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-05-15 09:25:07.000000 glances-4.0.4/glances/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-15 09:25:07.000000 glances-4.0.4/glances/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-15 09:25:07.000000 glances-4.0.4/glances/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30810 2024-05-15 09:25:07.000000 glances-4.0.4/glances/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outdated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.828857 glances-4.0.4/glances/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_bars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48721 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_curses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_curses_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29836 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_sparklines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout_apidoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_stdout_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/glances_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.828857 glances-4.0.4/glances/outputs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.828857 glances-4.0.4/glances/outputs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/css/bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/css/style.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/css/variables.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.828857 glances-4.0.4/glances/outputs/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/images/glances.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.832857 glances-4.0.4/glances/outputs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/App.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.836857 glances-4.0.4/glances/outputs/static/js/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/help.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-alert.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-amps.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-cloud.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-connections.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-containers.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-cpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-diskio.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-folders.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-fs.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-gpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-ip.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-irq.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-load.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-mem-more.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-mem.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-memswap.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-network.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-now.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-percpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-ports.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-process.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-processcount.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-processlist.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-quicklook.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-raid.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-sensors.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-smart.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-system.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-uptime.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/components/plugin-wifi.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/filters.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/services.js
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/store.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/js/uiconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   452411 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.836857 glances-4.0.4/glances/outputs/static/public/
+-rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   448748 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/public/glances.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/outputs/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-15 09:25:07.000000 glances-4.0.4/glances/outputs/static/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-15 09:25:07.000000 glances-4.0.4/glances/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-15 09:25:07.000000 glances-4.0.4/glances/password_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/__pycache__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/amps/
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/amps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/containers/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/engines/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/engines/podman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/containers/stats_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/cpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/diskio/
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/diskio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/folders/
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/folders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/fs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/gpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/gpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/gpu/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/gpu/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/gpu/cards/amd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/gpu/cards/nvidia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.840857 glances-4.0.4/glances/plugins/help/
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/help/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/irq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/irq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/load/
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/mem/
+-rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/mem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/memswap/
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/memswap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/network/
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/now/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/now/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/percpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/percpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47262 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/plugin/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/ports/
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/ports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/processcount/
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/processcount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/processlist/
+-rw-r--r--   0 runner    (1001) docker     (127)    36694 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/processlist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/psutilversion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/psutilversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/quicklook/
+-rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/quicklook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/raid/
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/raid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/sensors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/sensors/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/sensors/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/sensors/sensor/glances_batpercent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/sensors/sensor/glances_hddtemp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/smart/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/smart/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.844857 glances-4.0.4/glances/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.848857 glances-4.0.4/glances/plugins/uptime/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/uptime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.848857 glances-4.0.4/glances/plugins/version/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:25:11.848857 glances-4.0.4/glances/plugins/wifi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-15 09:25:07.000000 glances-4.0.4/glances/plugins/wifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-15 09:25:07.000000 glances-4.0.4/glances/ports_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26474 2024-05-15 09:25:07.000000 glances-4.0.4/glances/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-15 09:25:07.000000 glances-4.0.4/glances/programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-15 09:25:07.000000 glances-4.0.4/glances/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-15 09:25:07.000000 glances-4.0.4/glances/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-15 09:25:07.000000 glances-4.0.4/glances/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-05-15 09:25:07.000000 glances-4.0.4/glances/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-15 09:25:07.000000 glances-4.0.4/glances/static_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-15 09:25:07.000000 glances-4.0.4/glances/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-15 09:25:07.000000 glances-4.0.4/glances/stats_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-15 09:25:07.000000 glances-4.0.4/glances/stats_client_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 09:25:07.000000 glances-4.0.4/glances/stats_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-15 09:25:07.000000 glances-4.0.4/glances/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-15 09:25:07.000000 glances-4.0.4/glances/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-15 09:25:07.000000 glances-4.0.4/glances/web_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-15 09:25:07.000000 glances-4.0.4/glances/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-15 09:25:07.000000 glances-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 09:25:11.852857 glances-4.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4418 2024-05-15 09:25:07.000000 glances-4.0.4/setup.py
```

### Comparing `glances-4.0.3/AUTHORS` & `glances-4.0.4/AUTHORS`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/CONTRIBUTING.md` & `glances-4.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/COPYING` & `glances-4.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/Glances.egg-info/PKG-INFO` & `glances-4.0.4/Glances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 4.0.3
+Version: 4.0.4
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `glances-4.0.3/Glances.egg-info/SOURCES.txt` & `glances-4.0.4/Glances.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/Glances.egg-info/requires.txt` & `glances-4.0.4/Glances.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/NEWS.rst` & `glances-4.0.4/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 ==============================================================================
                                 Glances ChangeLog
 ==============================================================================
 
 ===============
+Version 4.0.4
+===============
+
+Hostfix release for support sensors on python3.8
+
+===============
 Version 4.0.3
 ===============
 
 Additional fixes for Sensor plugin.
 
 ===============
 Version 4.0.2
```

### Comparing `glances-4.0.3/PKG-INFO` & `glances-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 4.0.3
+Version: 4.0.4
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `glances-4.0.3/README.rst` & `glances-4.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/conf/glances.conf` & `glances-4.0.4/conf/glances.conf`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/Makefile` & `glances-4.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/Glances Logo dark.svg` & `glances-4.0.4/docs/_static/Glances Logo dark.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/Glances Logo.svg` & `glances-4.0.4/docs/_static/Glances Logo.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/Glances Text Logo dark.svg` & `glances-4.0.4/docs/_static/Glances Text Logo dark.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/Glances Text Logo.svg` & `glances-4.0.4/docs/_static/Glances Text Logo.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/amp-dropbox.png` & `glances-4.0.4/docs/_static/amp-dropbox.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/amp-python-warning.png` & `glances-4.0.4/docs/_static/amp-python-warning.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/amp-python.png` & `glances-4.0.4/docs/_static/amp-python.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/amps.png` & `glances-4.0.4/docs/_static/amps.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/aws.png` & `glances-4.0.4/docs/_static/aws.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/browser.png` & `glances-4.0.4/docs/_static/browser.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/cloud.png` & `glances-4.0.4/docs/_static/cloud.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/connected.png` & `glances-4.0.4/docs/_static/connected.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/connections.png` & `glances-4.0.4/docs/_static/connections.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/containers.png` & `glances-4.0.4/docs/_static/containers.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/cpu-wide.png` & `glances-4.0.4/docs/_static/cpu-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/cpu.png` & `glances-4.0.4/docs/_static/cpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/disconnected.png` & `glances-4.0.4/docs/_static/disconnected.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/diskio.png` & `glances-4.0.4/docs/_static/diskio.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/events.png` & `glances-4.0.4/docs/_static/events.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/folders.png` & `glances-4.0.4/docs/_static/folders.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/fs.png` & `glances-4.0.4/docs/_static/fs.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-architecture.excalidraw` & `glances-4.0.4/docs/_static/glances-architecture.excalidraw`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-architecture.png` & `glances-4.0.4/docs/_static/glances-architecture.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-cgraph.svg` & `glances-4.0.4/docs/_static/glances-cgraph.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-flame.svg` & `glances-4.0.4/docs/_static/glances-flame.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-influxdb.png` & `glances-4.0.4/docs/_static/glances-influxdb.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-memory-profiling-with-history.png` & `glances-4.0.4/docs/_static/glances-memory-profiling-with-history.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-memory-profiling-without-history.png` & `glances-4.0.4/docs/_static/glances-memory-profiling-without-history.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-pyinstrument.html` & `glances-4.0.4/docs/_static/glances-pyinstrument.html`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-responsive-webdesign.png` & `glances-4.0.4/docs/_static/glances-responsive-webdesign.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/glances-summary.png` & `glances-4.0.4/docs/_static/glances-summary.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/gpu.png` & `glances-4.0.4/docs/_static/gpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/grafana.png` & `glances-4.0.4/docs/_static/grafana.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/graph-load.svg` & `glances-4.0.4/docs/_static/graph-load.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/hddtemp.png` & `glances-4.0.4/docs/_static/hddtemp.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/header.png` & `glances-4.0.4/docs/_static/header.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/ip.png` & `glances-4.0.4/docs/_static/ip.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/irq.png` & `glances-4.0.4/docs/_static/irq.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/load.png` & `glances-4.0.4/docs/_static/load.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/loadpercent.png` & `glances-4.0.4/docs/_static/loadpercent.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/mem-wide.png` & `glances-4.0.4/docs/_static/mem-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/mem.png` & `glances-4.0.4/docs/_static/mem.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/monitored.png` & `glances-4.0.4/docs/_static/monitored.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/network.png` & `glances-4.0.4/docs/_static/network.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/per-cpu.png` & `glances-4.0.4/docs/_static/per-cpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/pergpu.png` & `glances-4.0.4/docs/_static/pergpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/ports.png` & `glances-4.0.4/docs/_static/ports.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/processlist-extended.png` & `glances-4.0.4/docs/_static/processlist-extended.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/processlist-filter.png` & `glances-4.0.4/docs/_static/processlist-filter.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/processlist-top.png` & `glances-4.0.4/docs/_static/processlist-top.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/processlist-wide.png` & `glances-4.0.4/docs/_static/processlist-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/processlist.png` & `glances-4.0.4/docs/_static/processlist.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/prometheus_exporter.png` & `glances-4.0.4/docs/_static/prometheus_exporter.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/prometheus_server.png` & `glances-4.0.4/docs/_static/prometheus_server.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/quicklook-percpu.png` & `glances-4.0.4/docs/_static/quicklook-percpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/quicklook.png` & `glances-4.0.4/docs/_static/quicklook.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/raid.png` & `glances-4.0.4/docs/_static/raid.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/reddit.png` & `glances-4.0.4/docs/_static/reddit.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/screencast.gif` & `glances-4.0.4/docs/_static/screencast.gif`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/screenshot-web.png` & `glances-4.0.4/docs/_static/screenshot-web.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/screenshot-web2.png` & `glances-4.0.4/docs/_static/screenshot-web2.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/screenshot-wide.png` & `glances-4.0.4/docs/_static/screenshot-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/screenshot.png` & `glances-4.0.4/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/sensors.png` & `glances-4.0.4/docs/_static/sensors.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/smart.png` & `glances-4.0.4/docs/_static/smart.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/sparkline.png` & `glances-4.0.4/docs/_static/sparkline.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/trend.png` & `glances-4.0.4/docs/_static/trend.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/twitter-icon.png` & `glances-4.0.4/docs/_static/twitter-icon.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/_static/wifi.png` & `glances-4.0.4/docs/_static/wifi.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/actions.rst` & `glances-4.0.4/docs/aoa/actions.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/amps.rst` & `glances-4.0.4/docs/aoa/amps.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/connections.rst` & `glances-4.0.4/docs/aoa/connections.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/containers.rst` & `glances-4.0.4/docs/aoa/containers.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/cpu.rst` & `glances-4.0.4/docs/aoa/cpu.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/diskio.rst` & `glances-4.0.4/docs/aoa/diskio.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/events.rst` & `glances-4.0.4/docs/aoa/events.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/folders.rst` & `glances-4.0.4/docs/aoa/folders.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/fs.rst` & `glances-4.0.4/docs/aoa/fs.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/gpu.rst` & `glances-4.0.4/docs/aoa/gpu.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/hddtemp.rst` & `glances-4.0.4/docs/aoa/hddtemp.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/header.rst` & `glances-4.0.4/docs/aoa/header.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/index.rst` & `glances-4.0.4/docs/aoa/index.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/irq.rst` & `glances-4.0.4/docs/aoa/irq.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/load.rst` & `glances-4.0.4/docs/aoa/load.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/memory.rst` & `glances-4.0.4/docs/aoa/memory.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/network.rst` & `glances-4.0.4/docs/aoa/network.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/ports.rst` & `glances-4.0.4/docs/aoa/ports.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/ps.rst` & `glances-4.0.4/docs/aoa/ps.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/quicklook.rst` & `glances-4.0.4/docs/aoa/quicklook.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/sensors.rst` & `glances-4.0.4/docs/aoa/sensors.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/smart.rst` & `glances-4.0.4/docs/aoa/smart.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/aoa/wifi.rst` & `glances-4.0.4/docs/aoa/wifi.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/api.rst` & `glances-4.0.4/docs/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1076,15 +1076,15 @@
 
 GET version
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/version
-    "4.0.3"
+    "4.0.4"
 
 GET wifi
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/wifi
```

### Comparing `glances-4.0.3/docs/cmds.rst` & `glances-4.0.4/docs/cmds.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/conf.py` & `glances-4.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/config.rst` & `glances-4.0.4/docs/config.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/dev/glances-cprofile.png` & `glances-4.0.4/docs/dev/glances-cprofile.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/docker.rst` & `glances-4.0.4/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/glances.rst` & `glances-4.0.4/docs/glances.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/cassandra.rst` & `glances-4.0.4/docs/gw/cassandra.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/couchdb.rst` & `glances-4.0.4/docs/gw/couchdb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/csv.rst` & `glances-4.0.4/docs/gw/csv.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/graph.rst` & `glances-4.0.4/docs/gw/graph.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/graphite.rst` & `glances-4.0.4/docs/gw/graphite.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/influxdb.rst` & `glances-4.0.4/docs/gw/influxdb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/kafka.rst` & `glances-4.0.4/docs/gw/kafka.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/mongodb.rst` & `glances-4.0.4/docs/gw/mongodb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/mqtt.rst` & `glances-4.0.4/docs/gw/mqtt.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/prometheus.rst` & `glances-4.0.4/docs/gw/prometheus.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/restful.rst` & `glances-4.0.4/docs/gw/restful.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/statsd.rst` & `glances-4.0.4/docs/gw/statsd.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/gw/zeromq.rst` & `glances-4.0.4/docs/gw/zeromq.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/index.rst` & `glances-4.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/install.rst` & `glances-4.0.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/make.bat` & `glances-4.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/man/glances.1` & `glances-4.0.4/docs/man/glances.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "GLANCES" "1" "May 15, 2024" "4.0.3" "Glances"
+.TH "GLANCES" "1" "May 15, 2024" "4.0.4" "Glances"
 .SH NAME
 glances \- An eye on your system
 .SH SYNOPSIS
 .sp
 \fBglances\fP [OPTIONS]
 .SH DESCRIPTION
 .sp
```

### Comparing `glances-4.0.3/docs/objects.inv` & `glances-4.0.4/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/docs/quickstart.rst` & `glances-4.0.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/__init__.py` & `glances-4.0.4/glances/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import platform
 import signal
 import sys
 
 # Global name
 # Version should start and end with a numerical char
 # See https://packaging.python.org/specifications/core-metadata/#version
-__version__ = '4.0.3'
+__version__ = '4.0.4'
 __apiversion__ = '4'
 __author__ = 'Nicolas Hennion <nicolas@nicolargo.com>'
 __license__ = 'LGPLv3'
 
 # Import psutil
 try:
     from psutil import __version__ as psutil_version
```

### Comparing `glances-4.0.3/glances/actions.py` & `glances-4.0.4/glances/actions.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/amps/amp.py` & `glances-4.0.4/glances/amps/amp.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/amps/default/__init__.py` & `glances-4.0.4/glances/amps/default/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/amps/nginx/__init__.py` & `glances-4.0.4/glances/amps/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/amps/systemd/__init__.py` & `glances-4.0.4/glances/amps/systemd/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/amps/systemv/__init__.py` & `glances-4.0.4/glances/amps/systemv/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/amps_list.py` & `glances-4.0.4/glances/amps_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/attribute.py` & `glances-4.0.4/glances/attribute.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/autodiscover.py` & `glances-4.0.4/glances/autodiscover.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/client.py` & `glances-4.0.4/glances/client.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/client_browser.py` & `glances-4.0.4/glances/client_browser.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/config.py` & `glances-4.0.4/glances/config.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/cpu_percent.py` & `glances-4.0.4/glances/cpu_percent.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/event.py` & `glances-4.0.4/glances/event.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/events_list.py` & `glances-4.0.4/glances/events_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/export.py` & `glances-4.0.4/glances/exports/export.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_cassandra/__init__.py` & `glances-4.0.4/glances/exports/glances_cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_couchdb/__init__.py` & `glances-4.0.4/glances/exports/glances_couchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_csv/__init__.py` & `glances-4.0.4/glances/exports/glances_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_elasticsearch/__init__.py` & `glances-4.0.4/glances/exports/glances_elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_graph/__init__.py` & `glances-4.0.4/glances/exports/glances_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_graphite/__init__.py` & `glances-4.0.4/glances/exports/glances_graphite/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_influxdb/__init__.py` & `glances-4.0.4/glances/exports/glances_influxdb/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_influxdb2/__init__.py` & `glances-4.0.4/glances/exports/glances_influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_json/__init__.py` & `glances-4.0.4/glances/exports/glances_json/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_kafka/__init__.py` & `glances-4.0.4/glances/exports/glances_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_mongodb/__init__.py` & `glances-4.0.4/glances/exports/glances_mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_mqtt/__init__.py` & `glances-4.0.4/glances/exports/glances_mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_opentsdb/__init__.py` & `glances-4.0.4/glances/exports/glances_opentsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_prometheus/__init__.py` & `glances-4.0.4/glances/exports/glances_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_rabbitmq/__init__.py` & `glances-4.0.4/glances/exports/glances_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_restful/__init__.py` & `glances-4.0.4/glances/exports/glances_restful/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_riemann/__init__.py` & `glances-4.0.4/glances/exports/glances_riemann/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_statsd/__init__.py` & `glances-4.0.4/glances/exports/glances_statsd/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/exports/glances_zeromq/__init__.py` & `glances-4.0.4/glances/exports/glances_zeromq/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/filter.py` & `glances-4.0.4/glances/filter.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/folder_list.py` & `glances-4.0.4/glances/folder_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/globals.py` & `glances-4.0.4/glances/globals.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/history.py` & `glances-4.0.4/glances/history.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/logger.py` & `glances-4.0.4/glances/logger.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/main.py` & `glances-4.0.4/glances/main.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outdated.py` & `glances-4.0.4/glances/outdated.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_bars.py` & `glances-4.0.4/glances/outputs/glances_bars.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_curses.py` & `glances-4.0.4/glances/outputs/glances_curses.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_curses_browser.py` & `glances-4.0.4/glances/outputs/glances_curses_browser.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_restful_api.py` & `glances-4.0.4/glances/outputs/glances_restful_api.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_sparklines.py` & `glances-4.0.4/glances/outputs/glances_sparklines.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_stdout.py` & `glances-4.0.4/glances/outputs/glances_stdout.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_stdout_apidoc.py` & `glances-4.0.4/glances/outputs/glances_stdout_apidoc.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_stdout_csv.py` & `glances-4.0.4/glances/outputs/glances_stdout_csv.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_stdout_issue.py` & `glances-4.0.4/glances/outputs/glances_stdout_issue.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_stdout_json.py` & `glances-4.0.4/glances/outputs/glances_stdout_json.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/glances_unicode.py` & `glances-4.0.4/glances/outputs/glances_unicode.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/README.md` & `glances-4.0.4/glances/outputs/static/README.md`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/css/bootstrap.less` & `glances-4.0.4/glances/outputs/static/css/bootstrap.less`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/css/style.scss` & `glances-4.0.4/glances/outputs/static/css/style.scss`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/images/favicon.ico` & `glances-4.0.4/glances/outputs/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/images/glances.png` & `glances-4.0.4/glances/outputs/static/images/glances.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/App.vue` & `glances-4.0.4/glances/outputs/static/js/App.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/help.vue` & `glances-4.0.4/glances/outputs/static/js/components/help.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-alert.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-alert.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-amps.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-amps.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-cloud.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-cloud.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-connections.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-connections.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-containers.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-containers.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-cpu.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-cpu.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-diskio.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-diskio.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-folders.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-folders.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-fs.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-fs.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-gpu.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-gpu.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-ip.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-ip.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-irq.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-irq.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-load.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-load.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-mem-more.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-mem-more.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-mem.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-mem.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-memswap.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-memswap.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-network.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-network.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-now.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-now.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-percpu.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-percpu.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-ports.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-ports.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-process.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-process.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-processcount.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-processcount.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-processlist.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-processlist.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-quicklook.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-quicklook.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-raid.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-raid.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-sensors.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-sensors.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-smart.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-smart.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-system.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-system.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/components/plugin-wifi.vue` & `glances-4.0.4/glances/outputs/static/js/components/plugin-wifi.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/filters.js` & `glances-4.0.4/glances/outputs/static/js/filters.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/js/services.js` & `glances-4.0.4/glances/outputs/static/js/services.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/package-lock.json` & `glances-4.0.4/glances/outputs/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/package.json` & `glances-4.0.4/glances/outputs/static/package.json`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png` & `glances-4.0.4/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/public/favicon.ico` & `glances-4.0.4/glances/outputs/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/public/glances.js` & `glances-4.0.4/glances/outputs/static/public/glances.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/outputs/static/webpack.config.js` & `glances-4.0.4/glances/outputs/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/password.py` & `glances-4.0.4/glances/password.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/password_list.py` & `glances-4.0.4/glances/password_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/alert/__init__.py` & `glances-4.0.4/glances/plugins/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/amps/__init__.py` & `glances-4.0.4/glances/plugins/amps/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/cloud/__init__.py` & `glances-4.0.4/glances/plugins/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/connections/__init__.py` & `glances-4.0.4/glances/plugins/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/containers/__init__.py` & `glances-4.0.4/glances/plugins/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/containers/engines/docker.py` & `glances-4.0.4/glances/plugins/containers/engines/docker.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/containers/engines/podman.py` & `glances-4.0.4/glances/plugins/containers/engines/podman.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/containers/stats_streamer.py` & `glances-4.0.4/glances/plugins/containers/stats_streamer.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/core/__init__.py` & `glances-4.0.4/glances/plugins/core/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/cpu/__init__.py` & `glances-4.0.4/glances/plugins/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/diskio/__init__.py` & `glances-4.0.4/glances/plugins/diskio/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/folders/__init__.py` & `glances-4.0.4/glances/plugins/folders/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/fs/__init__.py` & `glances-4.0.4/glances/plugins/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/gpu/__init__.py` & `glances-4.0.4/glances/plugins/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/gpu/cards/amd.py` & `glances-4.0.4/glances/plugins/gpu/cards/amd.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/gpu/cards/nvidia.py` & `glances-4.0.4/glances/plugins/gpu/cards/nvidia.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/help/__init__.py` & `glances-4.0.4/glances/plugins/help/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/ip/__init__.py` & `glances-4.0.4/glances/plugins/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/irq/__init__.py` & `glances-4.0.4/glances/plugins/irq/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/load/__init__.py` & `glances-4.0.4/glances/plugins/load/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/mem/__init__.py` & `glances-4.0.4/glances/plugins/mem/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/memswap/__init__.py` & `glances-4.0.4/glances/plugins/memswap/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/network/__init__.py` & `glances-4.0.4/glances/plugins/network/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/now/__init__.py` & `glances-4.0.4/glances/plugins/now/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/percpu/__init__.py` & `glances-4.0.4/glances/plugins/percpu/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/plugin/model.py` & `glances-4.0.4/glances/plugins/plugin/model.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/ports/__init__.py` & `glances-4.0.4/glances/plugins/ports/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/processcount/__init__.py` & `glances-4.0.4/glances/plugins/processcount/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/processlist/__init__.py` & `glances-4.0.4/glances/plugins/processlist/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/psutilversion/__init__.py` & `glances-4.0.4/glances/plugins/psutilversion/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/quicklook/__init__.py` & `glances-4.0.4/glances/plugins/quicklook/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/raid/__init__.py` & `glances-4.0.4/glances/plugins/raid/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/sensors/__init__.py` & `glances-4.0.4/glances/plugins/sensors/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
 
         if self.sensor_type == SensorType.FAN_SPEED:
             # psutil>=5.2.0, Linux-only
             return psutil.sensors_fans()
 
         raise ValueError(f"Unsupported sensor_type: {self.sensor_type}")
 
-    def update(self) -> list[dict]:
+    def update(self) -> List[dict]:
         """Update the stats."""
         if not self.init:
             return []
 
         # Temperatures sensors
         ret = []
         data = self.__fetch_psutil()
```

### Comparing `glances-4.0.3/glances/plugins/sensors/sensor/glances_batpercent.py` & `glances-4.0.4/glances/plugins/sensors/sensor/glances_batpercent.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/sensors/sensor/glances_hddtemp.py` & `glances-4.0.4/glances/plugins/sensors/sensor/glances_hddtemp.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/smart/__init__.py` & `glances-4.0.4/glances/plugins/smart/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/system/__init__.py` & `glances-4.0.4/glances/plugins/system/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/uptime/__init__.py` & `glances-4.0.4/glances/plugins/uptime/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/version/__init__.py` & `glances-4.0.4/glances/plugins/version/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/plugins/wifi/__init__.py` & `glances-4.0.4/glances/plugins/wifi/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/ports_list.py` & `glances-4.0.4/glances/ports_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/processes.py` & `glances-4.0.4/glances/processes.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/programs.py` & `glances-4.0.4/glances/programs.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/secure.py` & `glances-4.0.4/glances/secure.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/server.py` & `glances-4.0.4/glances/server.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/snmp.py` & `glances-4.0.4/glances/snmp.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/standalone.py` & `glances-4.0.4/glances/standalone.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/static_list.py` & `glances-4.0.4/glances/static_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/stats.py` & `glances-4.0.4/glances/stats.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/stats_client.py` & `glances-4.0.4/glances/stats_client.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/stats_client_snmp.py` & `glances-4.0.4/glances/stats_client_snmp.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/stats_server.py` & `glances-4.0.4/glances/stats_server.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/thresholds.py` & `glances-4.0.4/glances/thresholds.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/timer.py` & `glances-4.0.4/glances/timer.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/web_list.py` & `glances-4.0.4/glances/web_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/glances/webserver.py` & `glances-4.0.4/glances/webserver.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/pyproject.toml` & `glances-4.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `glances-4.0.3/setup.py` & `glances-4.0.4/setup.py`

 * *Files identical despite different names*

