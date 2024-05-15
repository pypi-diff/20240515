# Comparing `tmp/ufit-1.8.2.tar.gz` & `tmp/ufit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufit-1.8.2.tar", last modified: Thu Feb 29 09:31:34 2024, max compression
+gzip compressed data, was "ufit-1.9.0.tar", last modified: Wed May 15 12:58:38 2024, max compression
```

## Comparing `ufit-1.8.2.tar` & `ufit-1.9.0.tar`

### file list

```diff
@@ -1,189 +1,112 @@
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.812291 ufit-1.8.2/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      126 2020-05-26 05:10:10.000000 ufit-1.8.2/.gitignore
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      144 2024-02-21 14:10:50.000000 ufit-1.8.2/.isort.cfg
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1324 2024-02-21 14:10:50.000000 ufit-1.8.2/LICENSE
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1346 2024-02-21 14:10:50.000000 ufit-1.8.2/License.txt
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       29 2020-05-26 05:10:10.000000 ufit-1.8.2/MANIFEST.in
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      286 2024-02-21 14:10:50.000000 ufit-1.8.2/Makefile
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      343 2024-02-29 09:31:34.811291 ufit-1.8.2/PKG-INFO
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2185 2020-11-25 08:08:06.000000 ufit-1.8.2/README
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      373 2020-06-04 08:06:51.000000 ufit-1.8.2/TODO
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7604 2022-10-14 06:58:33.000000 ufit-1.8.2/Ufit.pyproj
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1103 2020-05-26 05:10:10.000000 ufit-1.8.2/Ufit.sln
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      609 2024-02-21 14:10:50.000000 ufit-1.8.2/covergui.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.555291 ufit-1.8.2/docs/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6298 2020-06-04 08:06:52.000000 ufit-1.8.2/docs/Makefile
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.555291 ufit-1.8.2/docs/_templates/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      160 2020-06-04 08:06:52.000000 ufit-1.8.2/docs/_templates/layout.html
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      624 2024-02-21 14:10:50.000000 ufit-1.8.2/docs/conf.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       38 2020-06-04 08:06:52.000000 ufit-1.8.2/docs/gui.rst
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1766 2020-11-25 08:08:06.000000 ufit-1.8.2/docs/index.rst
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4668 2020-06-04 08:06:52.000000 ufit-1.8.2/docs/intro.rst
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      757 2020-06-04 08:06:52.000000 ufit-1.8.2/docs/models.rst
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.555291 ufit-1.8.2/docs/pics/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    91948 2020-06-04 08:06:52.000000 ufit-1.8.2/docs/pics/main1.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4627 2020-06-04 08:06:51.000000 ufit-1.8.2/docs/script.rst
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.557291 ufit-1.8.2/installer/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1490 2024-02-21 14:10:50.000000 ufit-1.8.2/installer/ufit-osx.spec
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1361 2020-11-25 08:08:06.000000 ufit-1.8.2/installer/ufit_singlefile.spec
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4331 2020-05-26 05:10:10.000000 ufit-1.8.2/installer/ufit_singlefolder.nsi
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1515 2020-11-25 08:08:06.000000 ufit-1.8.2/installer/ufit_singlefolder.spec
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6535 2024-02-21 14:10:50.000000 ufit-1.8.2/pylintrc
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.557291 ufit-1.8.2/qcoverage/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1178 2024-02-21 14:10:50.000000 ufit-1.8.2/qcoverage/bz.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      485 2024-02-21 14:10:50.000000 ufit-1.8.2/qcoverage/hhl-test.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1408 2024-02-21 14:10:50.000000 ufit-1.8.2/qcoverage/hk0-and-h0l.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      256 2020-05-26 05:10:09.000000 ufit-1.8.2/qcoverage/readme.txt
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       63 2024-02-21 14:10:50.000000 ufit-1.8.2/requirements-installer.txt
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.570291 ufit-1.8.2/resource/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7229 2024-02-21 14:10:50.000000 ufit-1.8.2/resource/appicon-16.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    25021 2024-02-21 14:10:50.000000 ufit-1.8.2/resource/appicon-48.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    12299 2024-02-21 14:10:50.000000 ufit-1.8.2/resource/appicon.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      589 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/arrow-180.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      836 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/arrow-circle-double.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      678 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/arrow-join.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      740 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/arrow-move.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      877 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/arrow-switch.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      590 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/arrow.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      746 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/chart--arrow.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      588 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/cross-button.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      544 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/cross.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      434 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/disk-black.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      520 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/disks-black.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      661 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/document-export.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      665 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/document-pdf.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      485 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/document.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      682 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/drawer--minus.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      724 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/drawer--plus.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3308 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/drawer-double-open.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      662 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/drawer-open.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      647 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/drawer.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      647 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/folder-open.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      736 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/gear.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1332 2024-02-21 14:10:50.000000 ufit-1.8.2/resource/gui.qrc
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      752 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/home.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      514 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/image-sunset.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      307 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/log-x.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      331 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/log-y.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      292 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/log-z.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      756 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/magnifier-zoom-fit.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1550 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/map.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      690 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/notebook--plus.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      596 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/notebook.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      715 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/printer.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      761 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/question-white.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      676 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/script-php.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      556 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/selection-resize.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)   253784 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/splash.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)   559615 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/splash.xcf
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      600 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/table-select-row.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      616 2020-05-26 05:10:10.000000 ufit-1.8.2/resource/terminal--arrow.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       98 2021-05-21 07:04:12.000000 ufit-1.8.2/resource/ufit.desktop
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)  1270499 2023-03-07 08:48:25.000000 ufit-1.8.2/resource/ufit.icns
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)   247458 2021-05-21 07:04:12.000000 ufit-1.8.2/resource/ufit.png
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       38 2024-02-29 09:31:34.812291 ufit-1.8.2/setup.cfg
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1785 2024-02-21 14:10:50.000000 ufit-1.8.2/setup.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.640291 ufit-1.8.2/ufit/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)        6 2024-02-29 09:31:34.000000 ufit-1.8.2/ufit/RELEASE-VERSION
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      779 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/__init__.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.647291 ufit-1.8.2/ufit/backends/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1313 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/backends/__init__.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2086 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/backends/lmfit.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2036 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/backends/minuit.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1989 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/backends/scipy.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    11225 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/backends/unifit.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7153 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/bzplot.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     5223 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/cluster.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.687291 ufit-1.8.2/ufit/data/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6619 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/__init__.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2371 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/cascade.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    13149 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/dataset.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3010 2023-03-07 08:52:26.000000 ufit-1.8.2/ufit/data/desy.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3950 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/dynacool.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9950 2024-02-29 09:16:15.000000 ufit-1.8.2/ufit/data/ill.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3792 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/llb.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     8752 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/loader.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1895 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/mapping.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4334 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/merge.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     5540 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/nicos.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4801 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/nicos_old.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3399 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/nist.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3403 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/simple.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      681 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/simple_csv.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2995 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/taipan.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3736 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/trisp.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3337 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/data/zebra.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.724291 ufit-1.8.2/ufit/gui/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3643 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/__init__.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2027 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/annotations.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6607 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/browse.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    11549 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/common.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2775 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/console.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6746 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/coverage.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10310 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/dataloader.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10572 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/dataops.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      484 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/datasetitem.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1685 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/datawidgets.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4744 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/dialogs.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    13155 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/fitter.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7909 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/imageitem.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3009 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/inspector.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6736 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/itemlist.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6330 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/loggers.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    26603 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/main.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9479 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/mappingitem.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6798 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/modelbuilder.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    11412 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/ploteditor.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    13207 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/scanitem.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9178 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/session.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.798291 ufit-1.8.2/ufit/gui/ui/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)        0 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/__init__.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2329 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/gui/ui/about.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1281 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/annotations.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3516 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/box.ui
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6427 2021-05-21 14:19:54.000000 ufit-1.8.2/ufit/gui/ui/browse.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2731 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/change.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3925 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/custommodel.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    14430 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/dataloader.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    13050 2022-05-07 11:38:59.000000 ufit-1.8.2/ufit/gui/ui/dataops.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1730 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/fitter.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3695 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/imageops.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2104 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/inspector.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    15265 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/main.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6896 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/mapping.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     8562 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/modelbuilder.ui
--rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    11375 2020-11-25 08:08:06.000000 ufit-1.8.2/ufit/gui/ui/multiops.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4650 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/paramselect.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2754 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/paramset.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2097 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/printpreview.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     5863 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/qexplorer.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2018 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/rebin.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2233 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/reorder.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2603 2020-05-26 05:10:09.000000 ufit-1.8.2/ufit/gui/ui/subtract.ui
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)  1351821 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/guires_qt5.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)   967693 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/guires_qt6.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      494 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/lab.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.808291 ufit-1.8.2/ufit/models/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1120 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/models/__init__.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    20252 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/models/base.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1760 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/models/conv.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2830 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/models/corr.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7188 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/models/other.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9449 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/models/peaks.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7071 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/models/sqwtas.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7722 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/param.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10610 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/plotting.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1951 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/qreader.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1114 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/qt.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    54601 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/rescalc.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7487 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/result.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2560 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/utils.py
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2212 2024-02-21 14:10:50.000000 ufit-1.8.2/ufit/version.py
-drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-02-29 09:31:34.641291 ufit-1.8.2/ufit.egg-info/
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      343 2024-02-29 09:31:34.000000 ufit-1.8.2/ufit.egg-info/PKG-INFO
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3634 2024-02-29 09:31:34.000000 ufit-1.8.2/ufit.egg-info/SOURCES.txt
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)        1 2024-02-29 09:31:34.000000 ufit-1.8.2/ufit.egg-info/dependency_links.txt
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       38 2024-02-29 09:31:34.000000 ufit-1.8.2/ufit.egg-info/entry_points.txt
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       96 2024-02-29 09:31:34.000000 ufit-1.8.2/ufit.egg-info/requires.txt
--rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)        5 2024-02-29 09:31:34.000000 ufit-1.8.2/ufit.egg-info/top_level.txt
--rwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)      453 2024-02-21 14:10:50.000000 ufit-1.8.2/ufitgui
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-05-15 12:58:38.596338 ufit-1.9.0/
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1324 2024-04-12 06:29:06.000000 ufit-1.9.0/LICENSE
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)       29 2017-03-13 09:11:35.000000 ufit-1.9.0/MANIFEST.in
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      343 2024-05-15 12:58:38.596338 ufit-1.9.0/PKG-INFO
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2185 2020-11-23 13:41:42.000000 ufit-1.9.0/README
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)       38 2024-05-15 12:58:38.596338 ufit-1.9.0/setup.cfg
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1785 2024-04-12 06:28:25.000000 ufit-1.9.0/setup.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-05-15 12:58:38.578338 ufit-1.9.0/ufit/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        6 2024-05-15 12:58:37.000000 ufit-1.9.0/ufit/RELEASE-VERSION
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      779 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/__init__.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-05-15 12:58:38.580339 ufit-1.9.0/ufit/backends/
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1313 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/backends/__init__.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2097 2024-04-17 06:48:32.000000 ufit-1.9.0/ufit/backends/lmfit.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2036 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/backends/minuit.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1989 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/backends/scipy.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    11225 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/backends/unifit.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7153 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/bzplot.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     5223 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/cluster.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-05-15 12:58:38.584339 ufit-1.9.0/ufit/data/
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6619 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/__init__.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2371 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/cascade.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    13150 2024-04-17 06:48:55.000000 ufit-1.9.0/ufit/data/dataset.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3010 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/desy.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3950 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/dynacool.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9950 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/ill.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3792 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/llb.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     8752 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/loader.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1895 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/mapping.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4337 2024-05-15 12:58:25.000000 ufit-1.9.0/ufit/data/merge.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     5540 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/nicos.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4801 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/nicos_old.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3399 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/nist.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3442 2024-05-15 12:58:25.000000 ufit-1.9.0/ufit/data/simple.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      681 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/simple_csv.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2995 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/taipan.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3736 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/trisp.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3337 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/data/zebra.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-05-15 12:58:38.589338 ufit-1.9.0/ufit/gui/
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3643 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/__init__.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2027 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/annotations.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6607 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/browse.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    12846 2024-04-17 07:09:14.000000 ufit-1.9.0/ufit/gui/common.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2775 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/console.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6746 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/coverage.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10520 2024-05-15 12:58:25.000000 ufit-1.9.0/ufit/gui/dataloader.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10572 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/dataops.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      484 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/datasetitem.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1685 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/datawidgets.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     4744 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/dialogs.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    13169 2024-04-12 06:44:11.000000 ufit-1.9.0/ufit/gui/fitter.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7909 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/imageitem.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     3009 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/inspector.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6736 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/itemlist.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6330 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/loggers.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    29686 2024-05-15 12:58:25.000000 ufit-1.9.0/ufit/gui/main.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9479 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/mappingitem.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     6798 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/modelbuilder.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    11412 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/ploteditor.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    15060 2024-04-17 14:13:40.000000 ufit-1.9.0/ufit/gui/scanitem.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9178 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/session.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-05-15 12:58:38.594338 ufit-1.9.0/ufit/gui/ui/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        0 2024-04-12 06:28:25.000000 ufit-1.9.0/ufit/gui/ui/__init__.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2329 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/gui/ui/about.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1281 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/annotations.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3516 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/box.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6427 2021-05-21 16:02:21.000000 ufit-1.9.0/ufit/gui/ui/browse.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2731 2017-03-13 09:11:35.000000 ufit-1.9.0/ufit/gui/ui/change.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3925 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/custommodel.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    17022 2024-04-17 13:09:42.000000 ufit-1.9.0/ufit/gui/ui/dataloader.ui
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    15588 2024-04-17 07:58:09.000000 ufit-1.9.0/ufit/gui/ui/dataops.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     1904 2024-04-17 07:10:30.000000 ufit-1.9.0/ufit/gui/ui/fitter.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     3695 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/imageops.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2104 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/inspector.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    16191 2024-04-17 07:42:48.000000 ufit-1.9.0/ufit/gui/ui/main.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     6896 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/mapping.ui
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2744 2024-04-17 14:13:27.000000 ufit-1.9.0/ufit/gui/ui/massrename.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     9734 2024-04-17 11:59:24.000000 ufit-1.9.0/ufit/gui/ui/modelbuilder.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)    14175 2024-04-17 13:17:36.000000 ufit-1.9.0/ufit/gui/ui/multiops.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     4650 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/paramselect.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2754 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/paramset.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2097 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/printpreview.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     5863 2017-03-30 09:53:10.000000 ufit-1.9.0/ufit/gui/ui/qexplorer.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2018 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/rebin.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2233 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/reorder.ui
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1043 2024-04-17 06:39:33.000000 ufit-1.9.0/ufit/gui/ui/results.ui
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2603 2017-03-13 08:56:46.000000 ufit-1.9.0/ufit/gui/ui/subtract.ui
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)  1351821 2024-04-12 06:28:25.000000 ufit-1.9.0/ufit/guires_qt5.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)   967693 2024-04-12 06:28:25.000000 ufit-1.9.0/ufit/guires_qt6.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)      494 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/lab.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-05-15 12:58:38.596338 ufit-1.9.0/ufit/models/
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1120 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/models/__init__.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    20252 2024-04-12 06:32:31.000000 ufit-1.9.0/ufit/models/base.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1760 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/models/conv.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2830 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/models/corr.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7188 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/models/other.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     9449 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/models/peaks.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7071 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/models/sqwtas.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7722 2024-04-17 06:48:55.000000 ufit-1.9.0/ufit/param.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    10610 2024-04-17 07:46:29.000000 ufit-1.9.0/ufit/plotting.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1951 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/qreader.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     1114 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/qt.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)    54601 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/rescalc.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     7487 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/result.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2560 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/utils.py
+-rw-r--r--   0 gbrandl   (1000) gbrandl   (1000)     2212 2024-04-12 06:29:06.000000 ufit-1.9.0/ufit/version.py
+drwxr-xr-x   0 gbrandl   (1000) gbrandl   (1000)        0 2024-05-15 12:58:38.579338 ufit-1.9.0/ufit.egg-info/
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)      343 2024-05-15 12:58:38.000000 ufit-1.9.0/ufit.egg-info/PKG-INFO
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)     2138 2024-05-15 12:58:38.000000 ufit-1.9.0/ufit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        1 2024-05-15 12:58:38.000000 ufit-1.9.0/ufit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)       38 2024-05-15 12:58:38.000000 ufit-1.9.0/ufit.egg-info/entry_points.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)       96 2024-05-15 12:58:38.000000 ufit-1.9.0/ufit.egg-info/requires.txt
+-rw-rw-r--   0 gbrandl   (1000) gbrandl   (1000)        5 2024-05-15 12:58:38.000000 ufit-1.9.0/ufit.egg-info/top_level.txt
```

### Comparing `ufit-1.8.2/LICENSE` & `ufit-1.9.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2013-2023, Georg Brandl and contributors.
+Copyright (c) 2013-2024, Georg Brandl and contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `ufit-1.8.2/README` & `ufit-1.9.0/README`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/setup.py` & `ufit-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/__init__.py` & `ufit-1.9.0/ufit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 # pylint: disable=wrong-import-position, wrong-import-order
 
 from ufit.version import get_version
```

### Comparing `ufit-1.8.2/ufit/backends/__init__.py` & `ufit-1.9.0/ufit/backends/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Backend modules for different fitting packages/algorithms."""
 
 from ufit import UFitError
```

### Comparing `ufit-1.8.2/ufit/backends/lmfit.py` & `ufit-1.9.0/ufit/backends/lmfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Backend using lmfit."""
 
 from lmfit import Parameters, minimize, report_fit
 
@@ -48,16 +48,16 @@
         report_fit(out.params)
 
     pd = dict((pn, out.params[pn].value) for pn in varynames)
     update_params(dependent, meta, pd)
     for p in params:
         p.value = pd[p.name]
         if p.name in lmfparams:
-            p.error = out.params[p.name].stderr
-            p.correl = out.params[p.name].correl
+            p.error = out.params[p.name].stderr or 0
+            p.correl = out.params[p.name].correl or {}
         else:
             p.error = 0
             p.correl = {}
 
     # sadly, out.message is a bit buggy
     message = ''
     if not out.success:
```

### Comparing `ufit-1.8.2/ufit/backends/minuit.py` & `ufit-1.9.0/ufit/backends/minuit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Backend using iminuit."""
 
 from iminuit import Minuit
```

### Comparing `ufit-1.8.2/ufit/backends/scipy.py` & `ufit-1.9.0/ufit/backends/scipy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Backend using plain scipy leastsq."""
 
 from numpy import inf, sqrt
 from scipy.optimize import leastsq
```

### Comparing `ufit-1.8.2/ufit/backends/unifit.py` & `ufit-1.9.0/ufit/backends/unifit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Backend using "unifit" leastsq algorithm."""
 
 from copy import copy
 from time import time
```

### Comparing `ufit-1.8.2/ufit/bzplot.py` & `ufit-1.9.0/ufit/bzplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 from enum import Enum
 
 import numpy as np
```

### Comparing `ufit-1.8.2/ufit/cluster.py` & `ufit-1.9.0/ufit/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """
 Utilities for clustering execution of a piece of code to multiple hosts using
 SSH transport.
 """
```

### Comparing `ufit-1.8.2/ufit/data/__init__.py` & `ufit-1.9.0/ufit/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Data loading and treatment for ufit."""
 
 from ufit import UFitError
 from ufit.data import cascade, desy, dynacool, ill, llb, nicos, nicos_old, \
```

### Comparing `ufit-1.8.2/ufit/data/cascade.py` & `ufit-1.9.0/ufit/data/cascade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Loader for cascade image data."""
 
 import io
```

### Comparing `ufit-1.8.2/ufit/data/dataset.py` & `ufit-1.9.0/ufit/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Base dataset class."""
 
 import copy
 import operator
@@ -275,14 +275,15 @@
     def export_ascii(self, fp):
         savetxt(fp, array([self.x, self.y, self.dy]).T)
 
     def export_python(self, fp, objname='data'):
         fp.write('%s = as_data(%r, %r, %r, %r)\n' %
                  (objname, self.x, self.y, self.dy, self.name))
 
+
 # compatibility name
 Dataset = ScanData
 
 
 class ImageData(DataBase):
     def __init__(self, meta, arr, darr, norm=None, nscale=1,
                  name='', sources=None):
```

### Comparing `ufit-1.8.2/ufit/data/desy.py` & `ufit-1.9.0/ufit/data/desy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for DESY scattering data."""
 
 import io
 import time
```

### Comparing `ufit-1.8.2/ufit/data/dynacool.py` & `ufit-1.9.0/ufit/data/dynacool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for DynaCool PPMS data files."""
 
 import io
 from os import path
```

### Comparing `ufit-1.8.2/ufit/data/ill.py` & `ufit-1.9.0/ufit/data/ill.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for ILL TAS data."""
 
 import io
 import re
```

### Comparing `ufit-1.8.2/ufit/data/llb.py` & `ufit-1.9.0/ufit/data/llb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for LLB TAS data (binary format)."""
 
 import struct
 from time import mktime
```

### Comparing `ufit-1.8.2/ufit/data/loader.py` & `ufit-1.9.0/ufit/data/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Data loader object."""
 
 import io
```

### Comparing `ufit-1.8.2/ufit/data/mapping.py` & `ufit-1.9.0/ufit/data/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Routine for creating data mappings."""
 
 import numpy as np
 from matplotlib.cbook import flatten
```

### Comparing `ufit-1.8.2/ufit/data/merge.py` & `ufit-1.9.0/ufit/data/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Data merging routines."""
 
 from numpy import append, arange, array, ones, reshape, sqrt, zeros
 
@@ -117,15 +117,15 @@
 
     lastvals = []
     tomerge = []
     newlist = []
 
     for vals in data:
         # pylint: disable=use-implicit-booleaness-not-comparison
-        if lastvals != []:  # no "if lastvals", could be an array
+        if len(lastvals) > 0:  # no "if lastvals", could be an array
             if vals[0] > lastvals[0] + binsize:
                 # merge points in list:
                 newlist.append(mergeList(tomerge))
                 tomerge = []
         tomerge.append(vals)
         lastvals = vals
     newlist.append(mergeList(tomerge))
```

### Comparing `ufit-1.8.2/ufit/data/nicos.py` & `ufit-1.9.0/ufit/data/nicos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for NICOS2 data."""
 
 import io
 import time
```

### Comparing `ufit-1.8.2/ufit/data/nicos_old.py` & `ufit-1.9.0/ufit/data/nicos_old.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for OLD NICOS data."""
 
 import io
 import time
```

### Comparing `ufit-1.8.2/ufit/data/nist.py` & `ufit-1.9.0/ufit/data/nist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for NIST data files."""
 
 import io
 import re
```

### Comparing `ufit-1.8.2/ufit/data/simple.py` & `ufit-1.9.0/ufit/data/simple.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for simple whitespace-separated column data files."""
 
 import io
 from os import path
 
 from numpy import insert, loadtxt
 
 
 def guess_cols(colnames, coldata, meta):
-    if len(colnames) > 2:
+    if len(colnames) > 2 and not any(c < 0 for c in coldata[2]):
         dycol = colnames[2]
     else:
         dycol = None
     return colnames[0], colnames[1], dycol, None
 
 
 def check_data_simple(fp, sep=None):
```

### Comparing `ufit-1.8.2/ufit/data/simple_csv.py` & `ufit-1.9.0/ufit/data/simple_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for simple comma-separated column data files."""
 
 # pylint: disable=unused-import
 from ufit.data.simple import check_data_simple, guess_cols, read_data_simple
```

### Comparing `ufit-1.8.2/ufit/data/taipan.py` & `ufit-1.9.0/ufit/data/taipan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for TAIPAN data files."""
 
 import io
```

### Comparing `ufit-1.8.2/ufit/data/trisp.py` & `ufit-1.9.0/ufit/data/trisp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for TRISP spin-echo data."""
 
 import io
```

### Comparing `ufit-1.8.2/ufit/data/zebra.py` & `ufit-1.9.0/ufit/data/zebra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Load routine for PSI ZEBRA data files."""
 
 import io
```

### Comparing `ufit-1.8.2/ufit/gui/__init__.py` & `ufit-1.9.0/ufit/gui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Fitting/plotting GUI for ufit."""
 
 import argparse
 import sys
```

### Comparing `ufit-1.8.2/ufit/gui/annotations.py` & `ufit-1.9.0/ufit/gui/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Session annotation window."""
 
 from ufit.qt import QByteArray, QMainWindow, pyqtSignal
```

### Comparing `ufit-1.8.2/ufit/gui/browse.py` & `ufit-1.9.0/ufit/gui/browse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Data browsing window for the standalone GUI."""
 
 import os
 from os import path
```

### Comparing `ufit-1.8.2/ufit/gui/common.py` & `ufit-1.9.0/ufit/gui/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Common GUI elements."""
 
 import sys
 from io import BytesIO
@@ -17,16 +17,16 @@
 from matplotlib._pylab_helpers import Gcf
 from matplotlib.backend_bases import key_press_handler
 from matplotlib.backends.backend_qt5agg import \
     FigureCanvasQTAgg as FigureCanvas, FigureManagerQT, NavigationToolbar2QT
 from matplotlib.colors import LogNorm
 from matplotlib.figure import Figure
 
-from ufit.qt import QByteArray, QDialog, QFileDialog, QIcon, QLineEdit, \
-    QMessageBox, QPageLayout, QPainter, QPrintDialog, QPrinter, \
+from ufit.qt import QByteArray, QDialog, QFileDialog, QIcon, QLabel, \
+    QLineEdit, QMessageBox, QPageLayout, QPainter, QPrintDialog, QPrinter, \
     QPrintPreviewWidget, QRectF, QSettings, QSize, QSizePolicy, QSvgRenderer, \
     Qt, pyqtSignal, uic
 
 pyplot.rc('font', family='sans-serif')
 pyplot.rc('font', **{'sans-serif': 'Sans Serif, Arial, Helvetica, '
                      'Lucida Grande, DejaVu Sans'})
 
@@ -313,7 +313,50 @@
     def __enter__(self):
         self.settings.beginGroup(self.name)
         return self.settings
 
     def __exit__(self, *args):
         self.settings.endGroup()
         self.settings.sync()
+
+
+class SqueezedLabel(QLabel):
+    """A label that elides text to fit its width."""
+
+    def __init__(self, parent, designMode=False, **kwds):
+        self._fulltext = ''
+        QLabel.__init__(self, parent, **kwds)
+        self._squeeze()
+
+    def resizeEvent(self, event):
+        self._squeeze()
+        QLabel.resizeEvent(self, event)
+
+    def setText(self, text):
+        self._fulltext = text
+        self._squeeze(text)
+
+    def minimumSizeHint(self):
+        sh = QLabel.minimumSizeHint(self)
+        sh.setWidth(-1)
+        return sh
+
+    def _squeeze(self, text=None):
+        if text is None:
+            text = self._fulltext or self.text()
+        fm = self.fontMetrics()
+        labelwidth = self.size().width()
+        squeezed = False
+        new_lines = []
+        for line in text.split('\n'):
+            if fm.horizontalAdvance(line) > labelwidth:
+                squeezed = True
+                new_lines.append(fm.elidedText(
+                    line, Qt.TextElideMode.ElideRight, labelwidth))
+            else:
+                new_lines.append(line)
+        if squeezed:
+            QLabel.setText(self, '\n'.join(new_lines))
+            self.setToolTip(self._fulltext)
+        else:
+            QLabel.setText(self, self._fulltext)
+            self.setToolTip('')
```

### Comparing `ufit-1.8.2/ufit/gui/console.py` & `ufit-1.9.0/ufit/gui/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Embedded IPython qt console."""
 
 # pylint: disable=wrong-import-order
 from qtconsole.inprocess import QtInProcessKernelManager
```

### Comparing `ufit-1.8.2/ufit/gui/coverage.py` & `ufit-1.9.0/ufit/gui/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 import sys
 from os import path
 
 import numpy as np
```

### Comparing `ufit-1.8.2/ufit/gui/dataloader.py` & `ufit-1.9.0/ufit/gui/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Data loader panel."""
 
 from os import path
 
@@ -42,15 +42,20 @@
         session.itemsUpdated.connect(self.on_session_itemsUpdated)
         session.groupAdded.connect(self.on_session_itemsUpdated)
 
         with self.sgroup as settings:
             data_template_path = settings.value('last_data_template', '')
             if data_template_path:
                 self.templateEdit.setText(data_template_path)
-                self.set_template(data_template_path, 0, silent=True)
+                try:
+                    self.set_template(data_template_path, 0, silent=True)
+                except Exception:
+                    self.logger.exception(
+                        'while setting data template path: %r',
+                        data_template_path)
 
     def createUI(self, standalone):
         loadUi(self, 'dataloader.ui')
         self.dataformatBox.addItem('auto')
         for fmt in sorted(data_formats):
             self.dataformatBox.addItem(fmt)
```

### Comparing `ufit-1.8.2/ufit/gui/dataops.py` & `ufit-1.9.0/ufit/gui/dataops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Data operations panel."""
 
 from numpy import arange, linspace, ones
 from scipy.fftpack import fft
```

### Comparing `ufit-1.8.2/ufit/gui/datawidgets.py` & `ufit-1.9.0/ufit/gui/datawidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Various data display widgets for the GUI."""
 
 from ufit.qt import QListWidget, QListWidgetItem, Qt
```

### Comparing `ufit-1.8.2/ufit/gui/dialogs.py` & `ufit-1.9.0/ufit/gui/dialogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Various dialogs."""
 
 from numpy import array, nan, savetxt
```

### Comparing `ufit-1.8.2/ufit/gui/fitter.py` & `ufit-1.9.0/ufit/gui/fitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Data fitter panel."""
 
 from ufit.qt import QApplication, QCheckBox, QComboBox, QDialogButtonBox, \
     QFrame, QGridLayout, QIcon, QKeySequence, QLabel, QMainWindow, \
@@ -101,15 +101,15 @@
         self.original_params = {}
         combo_items = [''] + [par.name for par in self.model.params] + \
             ['data.' + m for m in sorted(self.data.meta)
              if isinstance(self.data.meta[m], (int, float))]
         for p in self.model.params:
             e0 = QLabel(p.name, self)
             e1 = SmallLineEdit('%.5g' % p.value, self)
-            e2 = QLabel('± %.5g' % p.error, self)
+            e2 = QLabel('± %.5g' % (p.error or 0), self)
             e2.setTextInteractionFlags(
                 Qt.TextInteractionFlag.TextSelectableByMouse |
                 Qt.TextInteractionFlag.TextSelectableByKeyboard)
             e3 = QCheckBox(self)
             e4 = QComboBox(self)
             e4.setEditable(True)
             e4.addItems(combo_items)
@@ -294,15 +294,15 @@
 
         self.statusLabel.setText(
             (res.success and 'Converged. ' or 'Failed. ') + res.message +
             ' Reduced chi^2 = %.3g.' % res.chisqr)
 
         for p in res.params:
             self.param_controls[p][1].setText('%.5g' % p.value)
-            self.param_controls[p][2].setText('± %.5g' % p.error)
+            self.param_controls[p][2].setText('± %.5g' % (p.error or 0))
 
         self.last_result = res
 
 
 class FitterMain(QMainWindow):
     def __init__(self, model, data, fit=True, fit_kws=None):
         QMainWindow.__init__(self)
```

### Comparing `ufit-1.8.2/ufit/gui/imageitem.py` & `ufit-1.9.0/ufit/gui/imageitem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Session item for datasets and corresponding GUI."""
 
 # pylint: disable=wrong-import-order
```

### Comparing `ufit-1.8.2/ufit/gui/inspector.py` & `ufit-1.9.0/ufit/gui/inspector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Metadata view window."""
 
 from ufit.qt import QByteArray, QMainWindow, QMessageBox, Qt, \
     QTableWidgetItem, pyqtSignal
```

### Comparing `ufit-1.8.2/ufit/gui/itemlist.py` & `ufit-1.9.0/ufit/gui/itemlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """A list view and model for different session items in the GUI."""
 
 # parts borrowed from M. Janoschek' nfit2 GUI
```

### Comparing `ufit-1.8.2/ufit/gui/loggers.py` & `ufit-1.9.0/ufit/gui/loggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Logging utilities for ufit.
 
 Mostly borrowed from nicos.utils.loggers.
 """
```

### Comparing `ufit-1.8.2/ufit/gui/main.py` & `ufit-1.9.0/ufit/gui/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Main window for the standalone GUI."""
 
 from os import path
+from pathlib import Path
+
+import matplotlib.style
 
 from ufit.qt import QAction, QActionGroup, QByteArray, QCursor, QDialog, \
     QFileDialog, QIcon, QInputDialog, QLabel, QMainWindow, QMenu, \
     QMessageBox, QModelIndex, QSplitter, Qt, QVBoxLayout, pyqtSlot
 
 from ufit import __version__, backends
 from ufit.data.dataset import ImageData, ScanData
@@ -90,45 +93,66 @@
         self.stacker.addWidget(self.dloader)
         self.current_panel = self.dloader
 
         # create item model
         self.itemlistmodel = ItemListModel()
         self.itemTree.setModel(self.itemlistmodel)
         self.itemlistmodel.reset()
-        self.itemTree.addAction(self.actionMergeData)
-        self.itemTree.addAction(self.actionRemoveData)
-        self.itemTree.addAction(self.menuMoveToGroup.menuAction())
-        self.itemTree.addAction(self.menuCopyToGroup.menuAction())
         self.itemTree.newSelection.connect(self.on_itemTree_newSelection)
 
         # backend selector
         self.backend_group = QActionGroup(self)
         for backend in backends.available:
             action = QAction(backend.backend_name, self)
             action.setCheckable(True)
             if backends.backend.backend_name == backend.backend_name:
                 action.setChecked(True)
             self.backend_group.addAction(action)
             self.menuBackend.addAction(action)
             action.triggered.connect(self.on_backend_action_triggered)
 
+        # style selector
+        self.style_group = QActionGroup(self)
+        for (i, style) in enumerate(['default'] + matplotlib.style.available):
+            action = QAction(style, self)
+            action.setCheckable(True)
+            if style == 'default':
+                action.setChecked(True)
+            self.style_group.addAction(action)
+            self.menuStyle.addAction(action)
+            action.triggered.connect(self.on_style_action_triggered)
+        self.menuStyle.addSeparator()
+        self.menuStyle.addAction(self.actionCustomStyle)
+
         # manage button
         menu = QMenu(self)
         menu.addAction(self.actionMergeData)
         menu.addAction(self.actionRemoveData)
         menu.addMenu(self.menuMoveToGroup)
         menu.addMenu(self.menuCopyToGroup)
         menu.addAction(self.actionReorder)
         menu.addSeparator()
         menu.addAction(self.actionNewGroup)
         menu.addMenu(self.menuRenameGroup)
         menu.addMenu(self.menuRemoveGroup)
         self.manageBtn.setMenu(menu)
 
-        # right-mouse-button menu for canvas
+        # right-mouse-button menu for items in tree
+        menu = self.itemMenu = QMenu(self)
+        menu.addAction(self.actionMergeData)
+        menu.addAction(self.actionRemoveData)
+        menu.addAction(self.menuMoveToGroup.menuAction())
+        menu.addAction(self.menuCopyToGroup.menuAction())
+
+        # right-mouse-button menu for groups in tree
+        menu = self.groupMenu = QMenu(self)
+        menu.addAction(self.actionRenameOneGroup)
+        menu.addAction(self.actionRemoveOneGroup)
+
+        # right-mouse-button menu for items on canvas
         menu = self.canvasMenu = QMenu(self)
         menu.addAction(self.actionUnzoom)
         menu.addAction(self.actionHideFit)
         menu.addSeparator()
         menu.addAction(self.actionDrawSymbols)
         menu.addAction(self.actionConnectData)
         menu.addAction(self.actionSmoothImages)
@@ -214,18 +238,26 @@
 
     @pyqtSlot()
     def on_actionClearRecent_triggered(self):
         """Clear recent files list"""
         self.recent_files = []
 
     def select_new_panel(self, panel):
+        active_tab = None
+        if isinstance(self.current_panel, ScanDataPanel):
+            active_tab = self.current_panel.currentIndex()
+
         if panel is not self.current_panel:
             if hasattr(self.current_panel, 'save_limits'):
                 self.current_panel.save_limits()
             self.current_panel = panel
+
+        if active_tab is not None and isinstance(panel, ScanDataPanel):
+            panel.setCurrentIndex(active_tab)
+
         self.stacker.setCurrentWidget(self.current_panel)  # doesn't hurt
 
     def on_canvas_pick(self, event):
         if isinstance(self.current_panel, ScanDataPanel):
             self.current_panel.on_canvas_pick(event)
 
     def on_canvas_click(self, event):
@@ -296,14 +328,29 @@
                 if not name:
                     return
                 session.rename_group(group, name)
             action.triggered.connect(rename)
             self.menuRenameGroup.addAction(action)
 
     @pyqtSlot()
+    def on_actionRemoveOneGroup_triggered(self):
+        group = self.selected_items(ItemGroup)[0]
+        session.remove_group(group)
+        self.re_expand_tree()
+
+    @pyqtSlot()
+    def on_actionRenameOneGroup_triggered(self):
+        group = self.selected_items(ItemGroup)[0]
+        name = QInputDialog.getText(self, 'ufit', 'Please enter a new name '
+                                    'for the group:', text=group.name)[0]
+        if not name:
+            return
+        session.rename_group(group, name)
+
+    @pyqtSlot()
     def on_actionRemoveData_triggered(self):
         items = self.selected_items()
         if not items:
             return
         q = QMessageBox.question(self, 'ufit',
                                  'OK to remove %d item(s)?' % len(items),
                                  QMessageBox.StandardButton.Yes |
@@ -346,14 +393,17 @@
         return [item for item in items if isinstance(item, itemcls)]
 
     def on_itemTree_newSelection(self):
         items = self.selected_items(None)
         if len(items) == 1 and isinstance(items[0], ItemGroup):
             # a group is selected -- act as if we selected all items
             items = items[0].items
+            # empty group?
+            if not items:
+                return
         if len(items) == 0:
             self.on_loadBtn_clicked()
         elif len(items) == 1:
             item = items[0]
             if item not in self.itempanels:
                 panel = self.itempanels[item] = \
                     item.create_panel(self, self.canvas)
@@ -391,14 +441,22 @@
         # expand / collapse all groups according to last saved state
         for group in session.groups:
             if group.expanded:
                 self.itemTree.expand(self.itemlistmodel.index_for_group(group))
             else:
                 self.itemTree.collapse(self.itemlistmodel.index_for_group(group))
 
+    def on_itemTree_customContextMenuRequested(self, point):
+        index = self.itemTree.indexAt(point)
+        if index.isValid():
+            if index.parent().isValid():  # an item
+                self.itemMenu.popup(QCursor.pos())
+            else:  # a group
+                self.groupMenu.popup(QCursor.pos())
+
     @pyqtSlot()
     def on_actionInspector_triggered(self):
         if self.inspector_window:
             self.inspector_window.activateWindow()
             return
         self.inspector_window = InspectorWindow(self)
 
@@ -602,14 +660,24 @@
             QMessageBox.warning(self, 'Error', 'Loading failed: %s' % err)
         else:
             self.re_expand_tree()
             self.setWindowModified(False)
             # if there are annotations, show the window automatically
             if session.props.get('annotations'):
                 self.on_actionAnnotations_triggered()
+            # apply style (but ignore failures)
+            if session.props.get('mpl_style'):
+                try:
+                    matplotlib.style.use(session.props.mpl_style)
+                except OSError:
+                    pass
+                for action in self.style_group.actions():
+                    if action.text() == session.props.mpl_style:
+                        action.setChecked(True)
+                        break
 
     def insert_session(self, filename):
         temp_session.load(filename)
         basename = path.basename(filename)
         if basename.endswith('.ufit'):
             basename = basename[:-5]
         # XXX slight HACK
@@ -695,8 +763,25 @@
                            Qt.WindowType.FramelessWindowHint)
         loadUi(dlg, 'about.ui')
         dlg.lbl.setText(dlg.lbl.text().replace('VERSION', __version__))
         dlg.exec()
 
     @pyqtSlot()
     def on_backend_action_triggered(self):
-        backends.set_backend(str(self.sender().text()))
+        backends.set_backend(self.sender().text())
+
+    @pyqtSlot()
+    def on_style_action_triggered(self):
+        style = self.sender().text()
+        matplotlib.style.use(style)
+        session.props.mpl_style = style
+        self.current_panel.plot(True)
+
+    @pyqtSlot()
+    def on_actionCustomStyle_triggered(self):
+        filename, _ = QFileDialog.getOpenFileName(
+            self, 'Select style file', str(Path.home()),
+            'Matplotlib styles (*.mplstyle)')
+        if filename:
+            session.props.mpl_style = filename
+            matplotlib.style.use(filename)
+            self.current_panel.plot(True)
```

### Comparing `ufit-1.8.2/ufit/gui/mappingitem.py` & `ufit-1.9.0/ufit/gui/mappingitem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Panel for mappings."""
 
 from matplotlib.cbook import flatten
 from numpy import array, mgrid, ptp, savetxt
```

### Comparing `ufit-1.8.2/ufit/gui/modelbuilder.py` & `ufit-1.9.0/ufit/gui/modelbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Model builder panel."""
 
 import re
```

### Comparing `ufit-1.8.2/ufit/gui/ploteditor.py` & `ufit-1.9.0/ufit/gui/ploteditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 # Originally matplotlib.backends.qt_editor.figureoptions
 # Copyright © 2009 Pierre Raybaut
 # Licensed under the terms of the MIT License
 # see the mpl licenses directory for a copy of the license
```

### Comparing `ufit-1.8.2/ufit/gui/scanitem.py` & `ufit-1.9.0/ufit/gui/scanitem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Session item for datasets and corresponding GUI."""
 
+import re
 from os import path
 
 from numpy import array, linspace, mean, savetxt, sqrt
 
-from ufit.qt import QDialog, QMessageBox, QTabWidget, QWidget, pyqtSignal, \
-    pyqtSlot
+from ufit.qt import QApplication, QDialog, QMessageBox, QTabWidget, QWidget, \
+    pyqtSignal, pyqtSlot
 
 from ufit.data.merge import rebin
 from ufit.gui import logger
 from ufit.gui.common import loadUi
 from ufit.gui.dataops import DataOps
 from ufit.gui.dialogs import ParamSetDialog
 from ufit.gui.fitter import Fitter
@@ -72,34 +73,33 @@
         return ScanDataPanel(mainwindow, canvas, self)
 
     def create_multi_panel(self, mainwindow, canvas):
         return MultiDataOps(mainwindow, canvas)
 
     def update_htmldesc(self):
         title = self.data.title
-        # XXX self.dataops.titleEdit.setText(title)
         self.title = title
         htmldesc = '<big><b>%s</b></big>' % self.index + \
             (title and ' - %s' % title or '') + \
             (self.data.environment and
              '<br>%s' % ', '.join(self.data.environment) or '') + \
             ('<br><small>%s</small>' % '<br>'.join(self.data.sources[:5]))
         if len(self.data.sources) > 5:
             htmldesc += '<br><small>...</small>'
         self.htmldesc = htmldesc
         session.itemsUpdated.emit()
 
     def export_python(self, filename):
-        with open(filename, 'wb') as fp:
-            fp.write(b'from ufit.lab import *\n')
-            fp.write(b'\n')
+        with open(filename, 'w') as fp:
+            fp.write('from ufit.lab import *\n')
+            fp.write('\n')
             self.data.export_python(fp, 'data')
             fp.write('\n')
             self.model.export_python(fp, 'model')
-            fp.write(b'''\
+            fp.write('''\
 ## just plot current values
 data.plot()
 model.plot_components(data)
 model.plot(data)
 
 ## to fit again use this...
 #result = model.fit(data)
@@ -206,23 +206,25 @@
 
 
 class MultiDataOps(QWidget):
     replotRequest = pyqtSignal(object)
 
     def __init__(self, parent, canvas):
         QWidget.__init__(self, parent)
+        self.mainwindow = parent
         self.canvas = canvas
         self.replotRequest.connect(self.plot)
 
         loadUi(self, 'multiops.ui')
 
     def initialize(self, items):
         self.items = [i for i in items if isinstance(i, ScanDataItem)]
         self.datas = [i.data for i in self.items]
-        self.monscaleEdit.setText(str(int(mean([d.nscale for d in self.datas]))))
+        self.monscaleEdit.setText(
+            str(int(mean([d.nscale for d in self.datas]))))
         self.onemodelBox.clear()
         self.onemodelBox.addItems(['%d' % i.index for i in self.items])
 
     def plot(self, limits=True, canvas=None):
         canvas = canvas or self.canvas
         xlabels = set()
         ylabels = set()
@@ -331,35 +333,55 @@
     @pyqtSlot()
     def on_floatMergeBtn_clicked(self):
         try:
             precision = float(self.mergeEdit.text())
         except ValueError:
             QMessageBox.warning(self, 'Error', 'Enter a valid precision.')
             return
-        new_data = self.datas[0].merge(precision, floatmerge=True, *self.datas[1:])
+        new_data = self.datas[0].merge(precision, floatmerge=True,
+                                       *self.datas[1:])
         session.add_item(ScanDataItem(new_data), self.items[-1].group)
 
     @pyqtSlot()
     def on_onemodelBtn_clicked(self):
         which = self.onemodelBox.currentIndex()
         if which < 0:
             return
-        model = self.items[which].model
+        src_item = self.items[which]
         with_params = self.onemodelWithParamsBox.isChecked()
+        # ensure params are updated from the last entered values in controls
+        if with_params:
+            src_panel = self.mainwindow.itempanels.get(src_item)
+            if src_panel:
+                src_panel.fitter.update_from_controls()
         for i, item in enumerate(self.items):
             if i == which:
                 continue
-            item.change_model(model.copy(), keep_param_values=not with_params)
+            item.change_model(src_item.model.copy(),
+                              keep_param_values=not with_params)
         self.replotRequest.emit(None)
 
     @pyqtSlot()
     def on_fitallBtn_clicked(self):
-        for item in self.items:
+        results = []
+        n = len(self.items)
+        for (i, item) in enumerate(self.items):
+            self.fitallLbl.setText(f'Working on dataset {i+1}/{n}...')
+            QApplication.processEvents()
             res = item.model.fit(item.data)
+            results.append(
+                f'{item.data.title} {item.data.name}: ' +
+                (res.success and 'Converged. ' or 'Failed. ') + res.message +
+                ' Reduced chi^2 = %.3g.' % res.chisqr)
             session.modelFitted.emit(item, res)
+        self.fitallLbl.setText('')
+        resdlg = QDialog(self)
+        loadUi(resdlg, 'results.ui')
+        resdlg.textBox.setText('\n'.join(results))
+        resdlg.show()
         self.replotRequest.emit(None)
 
     @pyqtSlot()
     def on_paramsetBtn_clicked(self):
         dlg = ParamSetDialog(self, self.items)
         if dlg.exec() != QDialog.DialogCode.Accepted:
             return
@@ -384,7 +406,34 @@
         for i, item in enumerate(self.items):
             item.export_fits(base + '.%d' % i + ext)
 
     def export_python(self, filename):
         base, ext = path.splitext(filename)
         for i, item in enumerate(self.items):
             item.export_python(base + '.%d' % i + ext)
+
+    @pyqtSlot()
+    def on_massrenameBtn_clicked(self):
+        dlg = QDialog(self)
+        loadUi(dlg, 'massrename.ui')
+        dlg.availEdit.setText('name, ' + ', '.join(self.items[0].data.meta))
+        if dlg.exec() != QDialog.DialogCode.Accepted:
+            return
+
+        title_tpl = dlg.titleEdit.text()
+        name_tpl = dlg.nameEdit.text()
+        for item in self.items:
+            def repl(m):
+                key = m.group(1)
+                if key == 'name':
+                    return item.data.name
+                return str(item.data.meta.get(key, '?'))
+
+            item.data.meta.title = re.sub(r'\{(.*?)\}', repl, title_tpl)
+            item.data.name = re.sub(r'\{(.*?)\}', repl, name_tpl)
+            item.update_htmldesc()
+
+            panel = self.mainwindow.itempanels.get(item)
+            if panel:
+                panel.dataops.initialize(item)
+        session.set_dirty()
+        self.replotRequest.emit(None)
```

### Comparing `ufit-1.8.2/ufit/gui/session.py` & `ufit-1.9.0/ufit/gui/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Session and session item abstraction."""
 
 import pickle
 from os import path
```

### Comparing `ufit-1.8.2/ufit/gui/ui/about.ui` & `ufit-1.9.0/ufit/gui/ui/about.ui`

 * *Files 1% similar despite different names*

#### Comparing `ufit-1.8.2/ufit/gui/ui/about.ui` & `ufit-1.9.0/ufit/gui/ui/about.ui`

```diff
@@ -60,15 +60,15 @@
           <x>350</x>
           <y>210</y>
           <width>251</width>
           <height>121</height>
         </rect>
       </property>
       <property name="text">
-        <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-weight:600;&quot;&gt;ufit, a neutron data fitting suite&lt;/span&gt;&lt;/p&gt;&lt;p&gt;Version VERSION&lt;/p&gt;&lt;p&gt;Written by Georg Brandl, 2013-2023&lt;br/&gt;Contributions by Petr Cermak&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+        <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-weight:600;&quot;&gt;ufit, a neutron data fitting suite&lt;/span&gt;&lt;/p&gt;&lt;p&gt;Version VERSION&lt;/p&gt;&lt;p&gt;Written by Georg Brandl, 2013-2024&lt;br/&gt;Contributions by Petr Cermak&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
       </property>
       <property name="alignment">
         <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
       </property>
     </widget>
   </widget>
   <resources>
```

### Comparing `ufit-1.8.2/ufit/gui/ui/annotations.ui` & `ufit-1.9.0/ufit/gui/ui/annotations.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/box.ui` & `ufit-1.9.0/ufit/gui/ui/box.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/browse.ui` & `ufit-1.9.0/ufit/gui/ui/browse.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/change.ui` & `ufit-1.9.0/ufit/gui/ui/change.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/custommodel.ui` & `ufit-1.9.0/ufit/gui/ui/custommodel.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/dataloader.ui` & `ufit-1.9.0/ufit/gui/ui/dataloader.ui`

 * *Files 8% similar despite different names*

#### Comparing `ufit-1.8.2/ufit/gui/ui/dataloader.ui` & `ufit-1.9.0/ufit/gui/ui/dataloader.ui`

```diff
@@ -11,474 +11,506 @@
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QHBoxLayout" name="horizontalLayout">
       <item>
-        <layout class="QGridLayout" name="gridLayout">
-          <item row="4" column="1" colspan="2">
-            <layout class="QHBoxLayout" name="horizontalLayout_2">
-              <item>
-                <widget class="QLabel" name="label_5">
-                  <property name="sizePolicy">
-                    <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                      <horstretch>0</horstretch>
-                      <verstretch>0</verstretch>
-                    </sizepolicy>
-                  </property>
-                  <property name="minimumSize">
-                    <size>
-                      <width>30</width>
-                      <height>0</height>
-                    </size>
-                  </property>
-                  <property name="text">
-                    <string>Y</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QComboBox" name="ycolBox">
-                  <property name="editable">
-                    <bool>true</bool>
-                  </property>
-                  <item>
-                    <property name="text">
-                      <string>auto</string>
-                    </property>
+        <widget class="QScrollArea" name="scrollArea">
+          <property name="frameShape">
+            <enum>QFrame::NoFrame</enum>
+          </property>
+          <property name="widgetResizable">
+            <bool>true</bool>
+          </property>
+          <widget class="QWidget" name="scrollAreaWidgetContents_2">
+            <property name="geometry">
+              <rect>
+                <x>0</x>
+                <y>0</y>
+                <width>579</width>
+                <height>528</height>
+              </rect>
+            </property>
+            <layout class="QGridLayout" name="gridLayout_2">
+              <property name="leftMargin">
+                <number>0</number>
+              </property>
+              <property name="topMargin">
+                <number>0</number>
+              </property>
+              <property name="bottomMargin">
+                <number>0</number>
+              </property>
+              <item row="0" column="0">
+                <layout class="QGridLayout" name="gridLayout">
+                  <item row="4" column="1" colspan="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout_2">
+                      <item>
+                        <widget class="QLabel" name="label_5">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="minimumSize">
+                            <size>
+                              <width>30</width>
+                              <height>0</height>
+                            </size>
+                          </property>
+                          <property name="text">
+                            <string>Y</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QComboBox" name="ycolBox">
+                          <property name="editable">
+                            <bool>true</bool>
+                          </property>
+                          <item>
+                            <property name="text">
+                              <string>auto</string>
+                            </property>
+                          </item>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer_2">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
+                          </property>
+                          <property name="sizeType">
+                            <enum>QSizePolicy::Fixed</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>25</width>
+                              <height>20</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
                   </item>
-                </widget>
-              </item>
-              <item>
-                <spacer name="horizontalSpacer_2">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeType">
-                    <enum>QSizePolicy::Fixed</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>25</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </item>
-          <item row="11" column="1">
-            <spacer name="verticalSpacer">
-              <property name="orientation">
-                <enum>Qt::Vertical</enum>
-              </property>
-              <property name="sizeHint" stdset="0">
-                <size>
-                  <width>20</width>
-                  <height>40</height>
-                </size>
-              </property>
-            </spacer>
-          </item>
-          <item row="12" column="0" colspan="5">
-            <widget class="QDialogButtonBox" name="buttonBox">
-              <property name="standardButtons">
-                <set>QDialogButtonBox::NoButton</set>
-              </property>
-            </widget>
-          </item>
-          <item row="9" column="0">
-            <widget class="QLabel" name="label_13">
-              <property name="text">
-                <string>Merging type:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="9" column="1">
-            <widget class="QRadioButton" name="rbRebin">
-              <property name="text">
-                <string>Rebin</string>
-              </property>
-              <property name="checked">
-                <bool>false</bool>
-              </property>
-            </widget>
-          </item>
-          <item row="9" column="2">
-            <widget class="QRadioButton" name="rbFloatMerge">
-              <property name="text">
-                <string>Floating merge</string>
-              </property>
-              <property name="checkable">
-                <bool>true</bool>
-              </property>
-              <property name="checked">
-                <bool>true</bool>
-              </property>
-            </widget>
-          </item>
-          <item row="0" column="0" colspan="2">
-            <widget class="QLabel" name="label_10">
-              <property name="font">
-                <font>
-                  <weight>75</weight>
-                  <bold>true</bold>
-                </font>
-              </property>
-              <property name="text">
-                <string>Data loading</string>
-              </property>
-            </widget>
-          </item>
-          <item row="7" column="0">
-            <widget class="QLabel" name="label_6">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Numors:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="7" column="1" colspan="3">
-            <widget class="QLineEdit" name="numorsEdit"/>
-          </item>
-          <item row="7" column="4">
-            <widget class="QPushButton" name="numorHelpBtn">
-              <property name="text">
-                <string>?</string>
-              </property>
-            </widget>
-          </item>
-          <item row="8" column="0">
-            <widget class="QLabel" name="label_7">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Merge precision:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="8" column="1">
-            <widget class="QLineEdit" name="precisionEdit">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Ignored" vsizetype="Fixed">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>0</string>
-              </property>
-            </widget>
-          </item>
-          <item row="8" column="2">
-            <widget class="QLabel" name="label_12">
-              <property name="text">
-                <string>(0 means no merging)</string>
-              </property>
-            </widget>
-          </item>
-          <item row="7" column="4">
-            <widget class="QPushButton" name="browseBtn">
-              <property name="text">
-                <string>Browse...</string>
-              </property>
-            </widget>
-          </item>
-          <item row="3" column="1" colspan="2">
-            <layout class="QHBoxLayout" name="horizontalLayout_4">
-              <item>
-                <widget class="QLabel" name="label_4">
-                  <property name="sizePolicy">
-                    <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                      <horstretch>0</horstretch>
-                      <verstretch>0</verstretch>
-                    </sizepolicy>
-                  </property>
-                  <property name="minimumSize">
-                    <size>
-                      <width>30</width>
-                      <height>0</height>
-                    </size>
-                  </property>
-                  <property name="text">
-                    <string>X</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QComboBox" name="xcolBox">
-                  <property name="editable">
-                    <bool>true</bool>
-                  </property>
-                  <item>
-                    <property name="text">
-                      <string>auto</string>
-                    </property>
+                  <item row="11" column="1">
+                    <spacer name="verticalSpacer">
+                      <property name="orientation">
+                        <enum>Qt::Vertical</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>20</width>
+                          <height>40</height>
+                        </size>
+                      </property>
+                    </spacer>
                   </item>
-                </widget>
-              </item>
-              <item>
-                <spacer name="horizontalSpacer">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeType">
-                    <enum>QSizePolicy::Fixed</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>25</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </item>
-          <item row="5" column="3" colspan="2">
-            <layout class="QHBoxLayout" name="horizontalLayout_6">
-              <item>
-                <widget class="QLabel" name="label_9">
-                  <property name="sizePolicy">
-                    <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                      <horstretch>0</horstretch>
-                      <verstretch>0</verstretch>
-                    </sizepolicy>
-                  </property>
-                  <property name="text">
-                    <string>Monitor scale</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QLineEdit" name="monscaleEdit">
-                  <property name="text">
-                    <string>10000</string>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </item>
-          <item row="1" column="0">
-            <widget class="QLabel" name="label_2">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Data template:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="1" column="1" colspan="3">
-            <widget class="QLineEdit" name="templateEdit">
-              <property name="readOnly">
-                <bool>true</bool>
-              </property>
-            </widget>
-          </item>
-          <item row="1" column="4">
-            <widget class="QPushButton" name="settemplateBtn">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Choose</string>
-              </property>
-              <property name="icon">
-                <iconset theme="document-open">
-                  <normaloff/>
-                </iconset>
-              </property>
-            </widget>
-          </item>
-          <item row="2" column="0">
-            <widget class="QLabel" name="label">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Data format:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="2" column="1" colspan="4">
-            <widget class="QComboBox" name="dataformatBox"/>
-          </item>
-          <item row="3" column="0">
-            <widget class="QLabel" name="label_3">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Columns:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="4" column="3" colspan="2">
-            <layout class="QHBoxLayout" name="horizontalLayout_3">
-              <item>
-                <widget class="QLabel" name="label_11">
-                  <property name="sizePolicy">
-                    <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                      <horstretch>0</horstretch>
-                      <verstretch>0</verstretch>
-                    </sizepolicy>
-                  </property>
-                  <property name="minimumSize">
-                    <size>
-                      <width>30</width>
-                      <height>0</height>
-                    </size>
-                  </property>
-                  <property name="text">
-                    <string>DY</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QComboBox" name="dycolBox">
-                  <property name="editable">
-                    <bool>true</bool>
-                  </property>
-                  <item>
-                    <property name="text">
-                      <string>auto</string>
-                    </property>
+                  <item row="12" column="0" colspan="5">
+                    <widget class="QDialogButtonBox" name="buttonBox">
+                      <property name="standardButtons">
+                        <set>QDialogButtonBox::NoButton</set>
+                      </property>
+                    </widget>
                   </item>
-                </widget>
-              </item>
-            </layout>
-          </item>
-          <item row="5" column="1" colspan="2">
-            <layout class="QHBoxLayout" name="horizontalLayout_5">
-              <item>
-                <widget class="QLabel" name="label_8">
-                  <property name="sizePolicy">
-                    <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                      <horstretch>0</horstretch>
-                      <verstretch>0</verstretch>
-                    </sizepolicy>
-                  </property>
-                  <property name="text">
-                    <string>Monitor</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QComboBox" name="moncolBox">
-                  <property name="editable">
-                    <bool>true</bool>
-                  </property>
-                  <item>
-                    <property name="text">
-                      <string>auto</string>
-                    </property>
+                  <item row="9" column="0">
+                    <widget class="QLabel" name="label_13">
+                      <property name="text">
+                        <string>Merging type:</string>
+                      </property>
+                    </widget>
                   </item>
-                </widget>
-              </item>
-              <item>
-                <spacer name="horizontalSpacer_3">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeType">
-                    <enum>QSizePolicy::Fixed</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>25</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
+                  <item row="9" column="1">
+                    <widget class="QRadioButton" name="rbRebin">
+                      <property name="text">
+                        <string>Rebin</string>
+                      </property>
+                      <property name="checked">
+                        <bool>false</bool>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="9" column="2">
+                    <widget class="QRadioButton" name="rbFloatMerge">
+                      <property name="text">
+                        <string>Floating merge</string>
+                      </property>
+                      <property name="checkable">
+                        <bool>true</bool>
+                      </property>
+                      <property name="checked">
+                        <bool>true</bool>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="0" column="0" colspan="2">
+                    <widget class="QLabel" name="label_10">
+                      <property name="font">
+                        <font>
+                          <weight>75</weight>
+                          <bold>true</bold>
+                        </font>
+                      </property>
+                      <property name="text">
+                        <string>Data loading</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="7" column="0">
+                    <widget class="QLabel" name="label_6">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Numors:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="7" column="1" colspan="3">
+                    <widget class="QLineEdit" name="numorsEdit"/>
+                  </item>
+                  <item row="7" column="4">
+                    <widget class="QPushButton" name="numorHelpBtn">
+                      <property name="text">
+                        <string>?</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="8" column="0">
+                    <widget class="QLabel" name="label_7">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Merge precision:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="8" column="1">
+                    <widget class="QLineEdit" name="precisionEdit">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Ignored" vsizetype="Fixed">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>0</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="8" column="2">
+                    <widget class="QLabel" name="label_12">
+                      <property name="text">
+                        <string>(0 means no merging)</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="7" column="4">
+                    <widget class="QPushButton" name="browseBtn">
+                      <property name="text">
+                        <string>Browse...</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="3" column="1" colspan="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout_4">
+                      <item>
+                        <widget class="QLabel" name="label_4">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="minimumSize">
+                            <size>
+                              <width>30</width>
+                              <height>0</height>
+                            </size>
+                          </property>
+                          <property name="text">
+                            <string>X</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QComboBox" name="xcolBox">
+                          <property name="editable">
+                            <bool>true</bool>
+                          </property>
+                          <item>
+                            <property name="text">
+                              <string>auto</string>
+                            </property>
+                          </item>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
+                          </property>
+                          <property name="sizeType">
+                            <enum>QSizePolicy::Fixed</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>25</width>
+                              <height>20</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </item>
+                  <item row="5" column="3" colspan="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout_6">
+                      <item>
+                        <widget class="QLabel" name="label_9">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="text">
+                            <string>Monitor scale</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLineEdit" name="monscaleEdit">
+                          <property name="text">
+                            <string>10000</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </item>
+                  <item row="1" column="0">
+                    <widget class="QLabel" name="label_2">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Data template:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="1" colspan="3">
+                    <widget class="QLineEdit" name="templateEdit">
+                      <property name="readOnly">
+                        <bool>true</bool>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="4">
+                    <widget class="QPushButton" name="settemplateBtn">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Choose</string>
+                      </property>
+                      <property name="icon">
+                        <iconset theme="document-open">
+                          <normaloff>.</normaloff>
+                          .
+                        </iconset>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="2" column="0">
+                    <widget class="QLabel" name="label">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Data format:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="2" column="1" colspan="4">
+                    <widget class="QComboBox" name="dataformatBox"/>
+                  </item>
+                  <item row="3" column="0">
+                    <widget class="QLabel" name="label_3">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Columns:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="4" column="3" colspan="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout_3">
+                      <item>
+                        <widget class="QLabel" name="label_11">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="minimumSize">
+                            <size>
+                              <width>30</width>
+                              <height>0</height>
+                            </size>
+                          </property>
+                          <property name="text">
+                            <string>DY</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QComboBox" name="dycolBox">
+                          <property name="editable">
+                            <bool>true</bool>
+                          </property>
+                          <item>
+                            <property name="text">
+                              <string>auto</string>
+                            </property>
+                          </item>
+                        </widget>
+                      </item>
+                    </layout>
+                  </item>
+                  <item row="5" column="1" colspan="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout_5">
+                      <item>
+                        <widget class="QLabel" name="label_8">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="text">
+                            <string>Monitor</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QComboBox" name="moncolBox">
+                          <property name="editable">
+                            <bool>true</bool>
+                          </property>
+                          <item>
+                            <property name="text">
+                              <string>auto</string>
+                            </property>
+                          </item>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer_3">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
+                          </property>
+                          <property name="sizeType">
+                            <enum>QSizePolicy::Fixed</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>25</width>
+                              <height>20</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </item>
+                  <item row="6" column="0">
+                    <widget class="QLabel" name="filterLbl">
+                      <property name="text">
+                        <string>Filter:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="6" column="1" colspan="2">
+                    <widget class="QComboBox" name="filtercolBox">
+                      <property name="editable">
+                        <bool>true</bool>
+                      </property>
+                      <item>
+                        <property name="text">
+                          <string>none</string>
+                        </property>
+                      </item>
+                    </widget>
+                  </item>
+                  <item row="6" column="3" colspan="2">
+                    <widget class="QLineEdit" name="filtervalEdit">
+                      <property name="text">
+                        <string/>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="10" column="0">
+                    <widget class="QLabel" name="groupBoxLbl">
+                      <property name="text">
+                        <string>Put into group:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="10" column="1" colspan="2">
+                    <widget class="QComboBox" name="groupBox">
+                      <property name="editable">
+                        <bool>true</bool>
+                      </property>
+                      <item>
+                        <property name="text">
+                          <string>Default</string>
+                        </property>
+                      </item>
+                    </widget>
+                  </item>
+                  <item row="10" column="3" colspan="2">
+                    <widget class="QLabel" name="groupBoxDesc">
+                      <property name="text">
+                        <string>(enter name to create new group)</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="3" column="3" colspan="2">
+                    <widget class="QLabel" name="label_12">
+                      <property name="text">
+                        <string>(to refresh column list, use &quot;Choose&quot; above)</string>
+                      </property>
+                    </widget>
+                  </item>
+                </layout>
               </item>
             </layout>
-          </item>
-          <item row="6" column="0">
-            <widget class="QLabel" name="filterLbl">
-              <property name="text">
-                <string>Filter:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="6" column="1" colspan="2">
-            <widget class="QComboBox" name="filtercolBox">
-              <property name="editable">
-                <bool>true</bool>
-              </property>
-              <item>
-                <property name="text">
-                  <string>none</string>
-                </property>
-              </item>
-            </widget>
-          </item>
-          <item row="6" column="3" colspan="2">
-            <widget class="QLineEdit" name="filtervalEdit">
-              <property name="text">
-                <string/>
-              </property>
-            </widget>
-          </item>
-          <item row="10" column="0">
-            <widget class="QLabel" name="groupBoxLbl">
-              <property name="text">
-                <string>Put into group:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="10" column="1" colspan="2">
-            <widget class="QComboBox" name="groupBox">
-              <property name="editable">
-                <bool>true</bool>
-              </property>
-              <item>
-                <property name="text">
-                  <string>Default</string>
-                </property>
-              </item>
-            </widget>
-          </item>
-          <item row="10" column="3" colspan="2">
-            <widget class="QLabel" name="groupBoxDesc">
-              <property name="text">
-                <string>(enter name to create new group)</string>
-              </property>
-            </widget>
-          </item>
-          <item row="3" column="3" colspan="2">
-            <widget class="QLabel" name="label_12">
-              <property name="text">
-                <string>(to refresh column list, use &quot;Choose&quot; above)</string>
-              </property>
-            </widget>
-          </item>
-        </layout>
+          </widget>
+        </widget>
       </item>
     </layout>
   </widget>
   <tabstops>
     <tabstop>templateEdit</tabstop>
     <tabstop>settemplateBtn</tabstop>
     <tabstop>dataformatBox</tabstop>
```

### Comparing `ufit-1.8.2/ufit/gui/ui/dataops.ui` & `ufit-1.9.0/ufit/gui/ui/dataops.ui`

 * *Files 8% similar despite different names*

#### Comparing `ufit-1.8.2/ufit/gui/ui/dataops.ui` & `ufit-1.9.0/ufit/gui/ui/dataops.ui`

```diff
@@ -3,436 +3,467 @@
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>805</width>
-        <height>696</height>
+        <height>750</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
-        <layout class="QGridLayout" name="gridLayout">
-          <item row="8" column="1" colspan="2">
-            <widget class="QLineEdit" name="scaleXConstEdit">
-              <property name="text">
-                <string>1</string>
-              </property>
-            </widget>
-          </item>
-          <item row="7" column="3">
-            <widget class="QPushButton" name="shiftBtn">
-              <property name="text">
-                <string>Shift</string>
-              </property>
-            </widget>
-          </item>
-          <item row="2" column="0">
-            <widget class="QLabel" name="label_12">
-              <property name="text">
-                <string>Set short name:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="13" column="2">
-            <layout class="QHBoxLayout" name="horizontalLayout_2">
-              <item>
-                <widget class="QPushButton" name="badResetBtn">
-                  <property name="sizePolicy">
-                    <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
-                      <horstretch>0</horstretch>
-                      <verstretch>0</verstretch>
-                    </sizepolicy>
-                  </property>
-                  <property name="text">
-                    <string>Reset</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <spacer name="horizontalSpacer">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>40</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </item>
-          <item row="15" column="0">
-            <widget class="QLabel" name="label_4">
-              <property name="text">
-                <string>Fit limits:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="3" column="3">
-            <widget class="QPushButton" name="arbBtn">
-              <property name="text">
-                <string>Do it</string>
-              </property>
-            </widget>
-          </item>
-          <item row="7" column="1" colspan="2">
-            <widget class="QLineEdit" name="shiftConstEdit">
-              <property name="text">
-                <string>0</string>
-              </property>
-            </widget>
-          </item>
-          <item row="5" column="3">
-            <widget class="QPushButton" name="addBtn">
-              <property name="text">
-                <string>Add</string>
-              </property>
-            </widget>
-          </item>
-          <item row="10" column="0">
-            <widget class="QLabel" name="label_13">
-              <property name="text">
-                <string>Subtract dataset:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="8" column="3">
-            <widget class="QPushButton" name="scaleXBtn">
-              <property name="text">
-                <string>Scale</string>
-              </property>
-            </widget>
-          </item>
-          <item row="11" column="1" colspan="2">
-            <layout class="QHBoxLayout" name="horizontalLayout_4">
-              <item>
-                <widget class="QLabel" name="label_17">
-                  <property name="text">
-                    <string>Number of interpolated points:</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QLineEdit" name="fftNpointsEdit">
-                  <property name="text">
-                    <string>100</string>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </item>
-          <item row="7" column="0">
-            <widget class="QLabel" name="label_3">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Shift X values:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="2" column="3">
-            <widget class="QPushButton" name="nameBtn">
-              <property name="text">
-                <string>Set</string>
-              </property>
-            </widget>
-          </item>
-          <item row="3" column="2">
-            <widget class="QLabel" name="label_15">
-              <property name="text">
-                <string>Change x/y values by formula:</string>
-              </property>
-              <property name="alignment">
-                <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-              </property>
-            </widget>
-          </item>
-          <item row="6" column="1" colspan="2">
-            <widget class="QLineEdit" name="scaleConstEdit">
-              <property name="text">
-                <string>1</string>
-              </property>
-            </widget>
-          </item>
-          <item row="13" column="1">
-            <widget class="QPushButton" name="badPointsBtn">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Start</string>
-              </property>
-            </widget>
-          </item>
-          <item row="5" column="1" colspan="2">
-            <widget class="QLineEdit" name="addConstEdit">
-              <property name="text">
-                <string>0</string>
-              </property>
-            </widget>
-          </item>
-          <item row="1" column="0">
-            <widget class="QLabel" name="label_11">
-              <property name="text">
-                <string>Set title:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="3" column="1">
-            <widget class="QPushButton" name="cloneBtn">
-              <property name="text">
-                <string>Clone</string>
-              </property>
-            </widget>
-          </item>
-          <item row="2" column="1" colspan="2">
-            <widget class="QLineEdit" name="nameEdit"/>
-          </item>
-          <item row="4" column="1" colspan="2">
-            <layout class="QHBoxLayout" name="horizontalLayout_3">
-              <item>
-                <widget class="QLineEdit" name="precisionEdit">
-                  <property name="text">
-                    <string>0.001</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QPushButton" name="floatmergeBtn">
-                  <property name="text">
-                    <string>Float merge</string>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </item>
-          <item row="13" column="0">
-            <widget class="QLabel" name="label_8">
-              <property name="text">
-                <string>Mask out points:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="1" column="1" colspan="2">
-            <widget class="QLineEdit" name="titleEdit"/>
-          </item>
-          <item row="11" column="0">
-            <widget class="QLabel" name="label_16">
-              <property name="text">
-                <string>FFT (creates new set):</string>
-              </property>
-            </widget>
-          </item>
-          <item row="5" column="0">
-            <widget class="QLabel" name="label">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Add a constant:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="13" column="3">
-            <widget class="QLabel" name="pickedLbl">
-              <property name="text">
-                <string>0 picked</string>
-              </property>
-            </widget>
-          </item>
-          <item row="12" column="0" colspan="4">
-            <widget class="Line" name="line">
-              <property name="orientation">
-                <enum>Qt::Horizontal</enum>
-              </property>
-            </widget>
-          </item>
-          <item row="8" column="0">
-            <widget class="QLabel" name="label_14">
-              <property name="text">
-                <string>Scale X with constant:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="0" column="0" colspan="3">
-            <widget class="QLabel" name="label_10">
-              <property name="font">
-                <font>
-                  <weight>75</weight>
-                  <bold>true</bold>
-                </font>
-              </property>
-              <property name="text">
-                <string>Data operations</string>
-              </property>
-            </widget>
-          </item>
-          <item row="6" column="3">
-            <widget class="QPushButton" name="mulBtn">
-              <property name="text">
-                <string>Scale</string>
-              </property>
-            </widget>
-          </item>
-          <item row="15" column="1" colspan="2">
-            <layout class="QHBoxLayout" name="horizontalLayout">
-              <item>
-                <widget class="QLineEdit" name="limitminEdit"/>
-              </item>
-              <item>
-                <widget class="QLabel" name="label_5">
-                  <property name="text">
-                    <string>to</string>
-                  </property>
-                </widget>
-              </item>
-              <item>
-                <widget class="QLineEdit" name="limitmaxEdit"/>
-              </item>
-            </layout>
-          </item>
-          <item row="4" column="3">
-            <widget class="QPushButton" name="rebinBtn">
-              <property name="text">
-                <string>Rebin</string>
-              </property>
-            </widget>
-          </item>
-          <item row="9" column="3">
-            <widget class="QPushButton" name="monscaleBtn">
-              <property name="text">
-                <string>Change</string>
-              </property>
-            </widget>
-          </item>
-          <item row="4" column="0">
-            <widget class="QLabel" name="label_2">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Merge/Rebin (destructive):</string>
-              </property>
-            </widget>
-          </item>
-          <item row="9" column="1" colspan="2">
-            <widget class="QLineEdit" name="monscaleEdit">
-              <property name="text">
-                <string>10000</string>
-              </property>
-            </widget>
-          </item>
-          <item row="1" column="3">
-            <widget class="QPushButton" name="titleBtn">
-              <property name="text">
-                <string>Set</string>
-              </property>
-            </widget>
-          </item>
-          <item row="9" column="0">
-            <widget class="QLabel" name="label_6">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>New monitor scale:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="11" column="3">
-            <widget class="QPushButton" name="fftBtn">
-              <property name="text">
-                <string>FFT</string>
-              </property>
-            </widget>
-          </item>
-          <item row="3" column="0">
-            <widget class="QLabel" name="label_9">
-              <property name="text">
-                <string>Clone to new:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="6" column="0">
-            <widget class="QLabel" name="label_7">
-              <property name="sizePolicy">
-                <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                  <horstretch>0</horstretch>
-                  <verstretch>0</verstretch>
-                </sizepolicy>
-              </property>
-              <property name="text">
-                <string>Scale Y with constant:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="15" column="3">
-            <widget class="QPushButton" name="limitsBtn">
-              <property name="text">
-                <string>Set</string>
-              </property>
-            </widget>
-          </item>
-          <item row="10" column="1">
-            <widget class="QPushButton" name="subtractBtn">
-              <property name="text">
-                <string>Subtract...</string>
-              </property>
-            </widget>
-          </item>
-          <item row="10" column="3">
-            <widget class="QPushButton" name="mappingBtn">
-              <property name="text">
-                <string>Mapping</string>
-              </property>
-              <property name="icon">
-                <iconset resource="../../../resource/gui.qrc">
-                  <normaloff>:/map.png</normaloff>
-                  :/map.png
-                </iconset>
-              </property>
-            </widget>
-          </item>
-        </layout>
-      </item>
-      <item>
-        <spacer name="verticalSpacer">
-          <property name="orientation">
-            <enum>Qt::Vertical</enum>
+        <widget class="QScrollArea" name="scrollArea">
+          <property name="frameShape">
+            <enum>QFrame::NoFrame</enum>
           </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>20</width>
-              <height>40</height>
-            </size>
+          <property name="widgetResizable">
+            <bool>true</bool>
           </property>
-        </spacer>
+          <widget class="QWidget" name="scrollAreaWidgetContents">
+            <property name="geometry">
+              <rect>
+                <x>0</x>
+                <y>0</y>
+                <width>793</width>
+                <height>738</height>
+              </rect>
+            </property>
+            <layout class="QGridLayout" name="gridLayout_2">
+              <property name="leftMargin">
+                <number>0</number>
+              </property>
+              <property name="topMargin">
+                <number>0</number>
+              </property>
+              <property name="bottomMargin">
+                <number>0</number>
+              </property>
+              <item row="0" column="0">
+                <layout class="QGridLayout" name="gridLayout">
+                  <item row="8" column="0">
+                    <widget class="QLabel" name="label_14">
+                      <property name="text">
+                        <string>Scale X with constant:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="4" column="3">
+                    <widget class="QPushButton" name="rebinBtn">
+                      <property name="text">
+                        <string>Rebin</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="11" column="0">
+                    <widget class="QLabel" name="label_16">
+                      <property name="text">
+                        <string>FFT (creates new set):</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="10" column="3">
+                    <widget class="QPushButton" name="mappingBtn">
+                      <property name="text">
+                        <string>Mapping</string>
+                      </property>
+                      <property name="icon">
+                        <iconset resource="../../../resource/gui.qrc">
+                          <normaloff>:/map.png</normaloff>
+                          :/map.png
+                        </iconset>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="2" column="0">
+                    <widget class="QLabel" name="label_12">
+                      <property name="text">
+                        <string>Set short name:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="3" column="1">
+                    <widget class="QPushButton" name="cloneBtn">
+                      <property name="text">
+                        <string>Clone</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="11" column="3">
+                    <widget class="QPushButton" name="fftBtn">
+                      <property name="text">
+                        <string>FFT</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="4" column="0">
+                    <widget class="QLabel" name="label_2">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Merge/Rebin (destructive):</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="13" column="3">
+                    <widget class="QLabel" name="pickedLbl">
+                      <property name="text">
+                        <string>0 picked</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="15" column="3">
+                    <widget class="QPushButton" name="limitsBtn">
+                      <property name="text">
+                        <string>Set</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="0" column="0" colspan="3">
+                    <widget class="QLabel" name="label_10">
+                      <property name="font">
+                        <font>
+                          <weight>75</weight>
+                          <bold>true</bold>
+                        </font>
+                      </property>
+                      <property name="text">
+                        <string>Data operations</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="3">
+                    <widget class="QPushButton" name="titleBtn">
+                      <property name="text">
+                        <string>Set</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="2" column="1" colspan="2">
+                    <widget class="QLineEdit" name="nameEdit"/>
+                  </item>
+                  <item row="3" column="3">
+                    <widget class="QPushButton" name="arbBtn">
+                      <property name="text">
+                        <string>Do it</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="11" column="1" colspan="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout_4">
+                      <item>
+                        <widget class="QLabel" name="label_17">
+                          <property name="text">
+                            <string>Number of interpolated points:</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLineEdit" name="fftNpointsEdit">
+                          <property name="text">
+                            <string>100</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </item>
+                  <item row="9" column="0">
+                    <widget class="QLabel" name="label_6">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>New monitor scale:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="5" column="1" colspan="2">
+                    <widget class="QLineEdit" name="addConstEdit">
+                      <property name="text">
+                        <string>0</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="13" column="0">
+                    <widget class="QLabel" name="label_8">
+                      <property name="text">
+                        <string>Mask out points:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="12" column="0" colspan="4">
+                    <widget class="Line" name="line">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="15" column="1" colspan="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout">
+                      <item>
+                        <widget class="QLineEdit" name="limitminEdit"/>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="label_5">
+                          <property name="text">
+                            <string>to</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLineEdit" name="limitmaxEdit"/>
+                      </item>
+                    </layout>
+                  </item>
+                  <item row="5" column="0">
+                    <widget class="QLabel" name="label">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Add a constant:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="3" column="0">
+                    <widget class="QLabel" name="label_9">
+                      <property name="text">
+                        <string>Clone to new:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="8" column="1" colspan="2">
+                    <widget class="QLineEdit" name="scaleXConstEdit">
+                      <property name="text">
+                        <string>1</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="1" colspan="2">
+                    <widget class="QLineEdit" name="titleEdit"/>
+                  </item>
+                  <item row="3" column="2">
+                    <widget class="QLabel" name="label_15">
+                      <property name="text">
+                        <string>Change x/y values by formula:</string>
+                      </property>
+                      <property name="alignment">
+                        <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="1" column="0">
+                    <widget class="QLabel" name="label_11">
+                      <property name="text">
+                        <string>Set title:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="15" column="0">
+                    <widget class="QLabel" name="label_4">
+                      <property name="text">
+                        <string>Fit limits:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="10" column="1">
+                    <widget class="QPushButton" name="subtractBtn">
+                      <property name="text">
+                        <string>Subtract...</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="4" column="1" colspan="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout_3">
+                      <item>
+                        <widget class="QLineEdit" name="precisionEdit">
+                          <property name="text">
+                            <string>0.001</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="floatmergeBtn">
+                          <property name="text">
+                            <string>Float merge</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </item>
+                  <item row="7" column="3">
+                    <widget class="QPushButton" name="shiftBtn">
+                      <property name="text">
+                        <string>Shift</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="5" column="3">
+                    <widget class="QPushButton" name="addBtn">
+                      <property name="text">
+                        <string>Add</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="6" column="0">
+                    <widget class="QLabel" name="label_7">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Scale Y with constant:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="8" column="3">
+                    <widget class="QPushButton" name="scaleXBtn">
+                      <property name="text">
+                        <string>Scale</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="10" column="0">
+                    <widget class="QLabel" name="label_13">
+                      <property name="text">
+                        <string>Subtract dataset:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="9" column="1" colspan="2">
+                    <widget class="QLineEdit" name="monscaleEdit">
+                      <property name="text">
+                        <string>10000</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="7" column="1" colspan="2">
+                    <widget class="QLineEdit" name="shiftConstEdit">
+                      <property name="text">
+                        <string>0</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="7" column="0">
+                    <widget class="QLabel" name="label_3">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Shift X values:</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="9" column="3">
+                    <widget class="QPushButton" name="monscaleBtn">
+                      <property name="text">
+                        <string>Change</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="13" column="2">
+                    <layout class="QHBoxLayout" name="horizontalLayout_2">
+                      <item>
+                        <widget class="QPushButton" name="badResetBtn">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="text">
+                            <string>Reset</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="horizontalSpacer">
+                          <property name="orientation">
+                            <enum>Qt::Horizontal</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>40</width>
+                              <height>20</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </item>
+                  <item row="13" column="1">
+                    <widget class="QPushButton" name="badPointsBtn">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="text">
+                        <string>Start</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="2" column="3">
+                    <widget class="QPushButton" name="nameBtn">
+                      <property name="text">
+                        <string>Set</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="6" column="1" colspan="2">
+                    <widget class="QLineEdit" name="scaleConstEdit">
+                      <property name="text">
+                        <string>1</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="6" column="3">
+                    <widget class="QPushButton" name="mulBtn">
+                      <property name="text">
+                        <string>Scale</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item row="16" column="0">
+                    <spacer name="verticalSpacer">
+                      <property name="orientation">
+                        <enum>Qt::Vertical</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>20</width>
+                          <height>40</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                </layout>
+              </item>
+            </layout>
+          </widget>
+        </widget>
       </item>
     </layout>
   </widget>
   <tabstops>
     <tabstop>titleEdit</tabstop>
     <tabstop>titleBtn</tabstop>
     <tabstop>nameEdit</tabstop>
```

### Comparing `ufit-1.8.2/ufit/gui/ui/fitter.ui` & `ufit-1.9.0/ufit/gui/ui/fitter.ui`

 * *Files 13% similar despite different names*

#### Comparing `ufit-1.8.2/ufit/gui/ui/fitter.ui` & `ufit-1.9.0/ufit/gui/ui/fitter.ui`

```diff
@@ -11,15 +11,15 @@
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
-        <widget class="QLabel" name="modelLabel">
+        <widget class="SqueezedLabel" name="modelLabel">
           <property name="font">
             <font>
               <weight>75</weight>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
@@ -40,15 +40,15 @@
           </property>
           <widget class="QWidget" name="scrollAreaWidgetContents">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
                 <width>499</width>
-                <height>378</height>
+                <height>372</height>
               </rect>
             </property>
           </widget>
         </widget>
       </item>
       <item>
         <widget class="QLabel" name="statusLabel">
@@ -64,10 +64,17 @@
         </widget>
       </item>
       <item>
         <widget class="QDialogButtonBox" name="buttonBox"/>
       </item>
     </layout>
   </widget>
+  <customwidgets>
+    <customwidget>
+      <class>SqueezedLabel</class>
+      <extends>QLabel</extends>
+      <header>ufit.gui.common</header>
+    </customwidget>
+  </customwidgets>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `ufit-1.8.2/ufit/gui/ui/imageops.ui` & `ufit-1.9.0/ufit/gui/ui/imageops.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/inspector.ui` & `ufit-1.9.0/ufit/gui/ui/inspector.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/main.ui` & `ufit-1.9.0/ufit/gui/ui/main.ui`

 * *Files 2% similar despite different names*

#### Comparing `ufit-1.8.2/ufit/gui/ui/main.ui` & `ufit-1.9.0/ufit/gui/ui/main.ui`

```diff
@@ -11,15 +11,24 @@
       </rect>
     </property>
     <property name="windowTitle">
       <string>ufit[*]</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <layout class="QHBoxLayout" name="horizontalLayout_2">
-        <property name="margin">
+        <property name="leftMargin">
+          <number>0</number>
+        </property>
+        <property name="topMargin">
+          <number>0</number>
+        </property>
+        <property name="rightMargin">
+          <number>0</number>
+        </property>
+        <property name="bottomMargin">
           <number>0</number>
         </property>
         <item>
           <widget class="QSplitter" name="splitter">
             <property name="orientation">
               <enum>Qt::Horizontal</enum>
             </property>
@@ -104,15 +113,15 @@
                       <string>Select one or more datasets:</string>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <widget class="ItemTreeView" name="itemTree">
                     <property name="contextMenuPolicy">
-                      <enum>Qt::ActionsContextMenu</enum>
+                      <enum>Qt::CustomContextMenu</enum>
                     </property>
                     <property name="indentation">
                       <number>14</number>
                     </property>
                   </widget>
                 </item>
               </layout>
@@ -123,15 +132,15 @@
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>386</width>
-          <height>20</height>
+          <height>31</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>&amp;File</string>
         </property>
         <widget class="QMenu" name="menuRecent">
@@ -194,18 +203,24 @@
         <addaction name="actionDrawSymbols"/>
         <addaction name="actionConnectData"/>
         <addaction name="actionDrawGrid"/>
         <addaction name="actionShowLegend"/>
         <addaction name="separator"/>
         <addaction name="actionSmoothImages"/>
       </widget>
+      <widget class="QMenu" name="menuStyle">
+        <property name="title">
+          <string>Style</string>
+        </property>
+      </widget>
       <addaction name="menuFile"/>
       <addaction name="menuView"/>
       <addaction name="menu_Plot"/>
       <addaction name="menuBackend"/>
+      <addaction name="menuStyle"/>
       <addaction name="menuHelp"/>
     </widget>
     <widget class="QToolBar" name="toolBar">
       <property name="windowTitle">
         <string>toolBar</string>
       </property>
       <attribute name="toolBarArea">
@@ -533,14 +548,35 @@
       </property>
     </action>
     <action name="actionQExplorer">
       <property name="text">
         <string>Open Q-Explorer</string>
       </property>
     </action>
+    <action name="actionRemoveOneGroup">
+      <property name="icon">
+        <iconset resource="../../../resource/gui.qrc">
+          <normaloff>:/drawer--minus.png</normaloff>
+          :/drawer--minus.png
+        </iconset>
+      </property>
+      <property name="text">
+        <string>Remove group</string>
+      </property>
+    </action>
+    <action name="actionRenameOneGroup">
+      <property name="text">
+        <string>Rename group</string>
+      </property>
+    </action>
+    <action name="actionCustomStyle">
+      <property name="text">
+        <string>Custom...</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>ItemTreeView</class>
       <extends>QTreeView</extends>
       <header>ufit.gui.itemlist</header>
     </customwidget>
```

### Comparing `ufit-1.8.2/ufit/gui/ui/mapping.ui` & `ufit-1.9.0/ufit/gui/ui/mapping.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/modelbuilder.ui` & `ufit-1.9.0/ufit/gui/ui/modelbuilder.ui`

 * *Files 10% similar despite different names*

#### Comparing `ufit-1.8.2/ufit/gui/ui/modelbuilder.ui` & `ufit-1.9.0/ufit/gui/ui/modelbuilder.ui`

```diff
@@ -3,15 +3,15 @@
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>509</width>
-        <height>434</height>
+        <height>257</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QHBoxLayout" name="horizontalLayout">
       <item>
@@ -49,44 +49,43 @@
           <item row="1" column="0" colspan="4">
             <widget class="QStackedWidget" name="modeldefStacker">
               <property name="currentIndex">
                 <number>0</number>
               </property>
               <widget class="QWidget" name="page">
                 <layout class="QHBoxLayout" name="horizontalLayout_2">
-                  <property name="margin">
+                  <property name="leftMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="topMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="rightMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="bottomMargin">
                     <number>0</number>
                   </property>
                   <item>
                     <layout class="QGridLayout" name="gridLayout_2">
                       <item row="0" column="0" colspan="4">
                         <widget class="QTextEdit" name="modeldefEdit">
+                          <property name="minimumSize">
+                            <size>
+                              <width>0</width>
+                              <height>30</height>
+                            </size>
+                          </property>
                           <property name="html">
                             <string>&lt;!DOCTYPE HTML PUBLIC &quot;-//W3C//DTD HTML 4.0//EN&quot; &quot;http://www.w3.org/TR/REC-html40/strict.dtd&quot;&gt;
 &lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
 p, li { white-space: pre-wrap; }
-&lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Liberation Sans'; font-size:9pt; font-weight:400; font-style:normal;&quot;&gt;
-&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;span style=&quot; font-family:'Lucida Grande';&quot;&gt;Background(bkgd=0)&lt;/span&gt;&lt;/p&gt;
-&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;span style=&quot; font-family:'Lucida Grande';&quot;&gt;+ Gauss('peak', pos=0, ampl=1, fwhm=1)&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                          </property>
-                        </widget>
-                      </item>
-                      <item row="2" column="0" rowspan="2" colspan="2">
-                        <widget class="QListWidget" name="premodelsList"/>
-                      </item>
-                      <item row="3" column="3">
-                        <widget class="QPushButton" name="addCustomBtn">
-                          <property name="sizePolicy">
-                            <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
-                              <horstretch>0</horstretch>
-                              <verstretch>0</verstretch>
-                            </sizepolicy>
-                          </property>
-                          <property name="text">
-                            <string>Add custom model...</string>
+&lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Segoe UI'; font-size:10pt; font-weight:400; font-style:normal;&quot;&gt;
+&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;span style=&quot; font-family:'Lucida Grande'; font-size:9pt;&quot;&gt;Background(bkgd=0)&lt;/span&gt;&lt;/p&gt;
+&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;span style=&quot; font-family:'Lucida Grande'; font-size:9pt;&quot;&gt;+ Gauss('peak', pos=0, ampl=1, fwhm=1)&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                           </property>
                         </widget>
                       </item>
                       <item row="4" column="0" colspan="4">
                         <widget class="QLabel" name="statusLbl">
                           <property name="font">
                             <font>
@@ -108,36 +107,77 @@
                             </sizepolicy>
                           </property>
                           <property name="text">
                             <string>Add predefined model:</string>
                           </property>
                         </widget>
                       </item>
+                      <item row="3" column="2">
+                        <widget class="QPushButton" name="addmodelBtn">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="text">
+                            <string>Add</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item row="3" column="3">
+                        <widget class="QPushButton" name="addCustomBtn">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="text">
+                            <string>Add custom model...</string>
+                          </property>
+                        </widget>
+                      </item>
                       <item row="2" column="2" colspan="2">
                         <widget class="QScrollArea" name="scrollArea">
+                          <property name="minimumSize">
+                            <size>
+                              <width>0</width>
+                              <height>30</height>
+                            </size>
+                          </property>
                           <property name="frameShape">
                             <enum>QFrame::NoFrame</enum>
                           </property>
                           <property name="frameShadow">
                             <enum>QFrame::Plain</enum>
                           </property>
                           <property name="widgetResizable">
                             <bool>true</bool>
                           </property>
                           <widget class="QWidget" name="scrollAreaWidgetContents">
                             <property name="geometry">
                               <rect>
                                 <x>0</x>
                                 <y>0</y>
-                                <width>214</width>
-                                <height>125</height>
+                                <width>224</width>
+                                <height>30</height>
                               </rect>
                             </property>
                             <layout class="QVBoxLayout" name="verticalLayout">
-                              <property name="margin">
+                              <property name="leftMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="topMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="rightMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="bottomMargin">
                                 <number>0</number>
                               </property>
                               <item>
                                 <widget class="QLabel" name="modelinfoLbl">
                                   <property name="text">
                                     <string>(Model info)</string>
                                   </property>
@@ -149,24 +189,21 @@
                                   </property>
                                 </widget>
                               </item>
                             </layout>
                           </widget>
                         </widget>
                       </item>
-                      <item row="3" column="2">
-                        <widget class="QPushButton" name="addmodelBtn">
-                          <property name="sizePolicy">
-                            <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
-                              <horstretch>0</horstretch>
-                              <verstretch>0</verstretch>
-                            </sizepolicy>
-                          </property>
-                          <property name="text">
-                            <string>Add</string>
+                      <item row="2" column="0" rowspan="2" colspan="2">
+                        <widget class="QListWidget" name="premodelsList">
+                          <property name="minimumSize">
+                            <size>
+                              <width>0</width>
+                              <height>30</height>
+                            </size>
                           </property>
                         </widget>
                       </item>
                     </layout>
                   </item>
                 </layout>
               </widget>
```

### Comparing `ufit-1.8.2/ufit/gui/ui/multiops.ui` & `ufit-1.9.0/ufit/gui/ui/multiops.ui`

 * *Files 8% similar despite different names*

#### Comparing `ufit-1.8.2/ufit/gui/ui/multiops.ui` & `ufit-1.9.0/ufit/gui/ui/multiops.ui`

```diff
@@ -3,391 +3,437 @@
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>624</width>
-        <height>403</height>
+        <height>480</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="0" column="0">
-        <widget class="QGroupBox" name="groupBox">
-          <property name="title">
-            <string>Data manipulation</string>
+      <item row="0" column="0" colspan="2">
+        <widget class="QScrollArea" name="scrollArea">
+          <property name="frameShape">
+            <enum>QFrame::NoFrame</enum>
           </property>
-          <layout class="QGridLayout" name="gridLayout_2">
-            <item row="0" column="2">
-              <widget class="QPushButton" name="rebinBtn">
-                <property name="text">
-                  <string>Rebin</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="2">
-              <widget class="QPushButton" name="mulBtn">
-                <property name="text">
-                  <string>Scale</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="1">
-              <widget class="QLineEdit" name="scaleConstEdit">
-                <property name="text">
-                  <string>1</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="1">
-              <widget class="QLineEdit" name="addConstEdit">
-                <property name="text">
-                  <string>0</string>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="1">
-              <widget class="QLineEdit" name="precisionEdit">
-                <property name="text">
-                  <string>0.001</string>
-                </property>
-              </widget>
-            </item>
-            <item row="5" column="0">
-              <widget class="QLabel" name="label_6">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="text">
-                  <string>Change monitor:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="5" column="1">
-              <widget class="QLineEdit" name="monscaleEdit">
-                <property name="text">
-                  <string>10000</string>
-                </property>
-              </widget>
-            </item>
-            <item row="4" column="0">
-              <widget class="QLabel" name="label_9">
-                <property name="text">
-                  <string>Scale X values:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="3" column="0">
-              <widget class="QLabel" name="label_3">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="text">
-                  <string>Shift X values:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="0">
-              <widget class="QLabel" name="label_2">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="text">
-                  <string>Rebin individual sets:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="3" column="1">
-              <widget class="QLineEdit" name="shiftConstEdit">
-                <property name="text">
-                  <string>0</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="2">
-              <widget class="QPushButton" name="addBtn">
-                <property name="text">
-                  <string>Add</string>
-                </property>
-              </widget>
-            </item>
-            <item row="5" column="2">
-              <widget class="QPushButton" name="monscaleBtn">
-                <property name="text">
-                  <string>Change</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="0">
-              <widget class="QLabel" name="label_7">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="text">
-                  <string>Scale Y values:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="0">
-              <widget class="QLabel" name="label">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="text">
-                  <string>Add a constant:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="3" column="2">
-              <widget class="QPushButton" name="shiftBtn">
-                <property name="text">
-                  <string>Shift</string>
-                </property>
-              </widget>
-            </item>
-            <item row="4" column="1">
-              <widget class="QLineEdit" name="scaleXConstEdit">
-                <property name="text">
-                  <string>1</string>
-                </property>
-              </widget>
-            </item>
-            <item row="4" column="2">
-              <widget class="QPushButton" name="scaleXBtn">
-                <property name="text">
-                  <string>Scale</string>
-                </property>
-              </widget>
-            </item>
-          </layout>
-          <zorder>precisionEdit</zorder>
-          <zorder>label</zorder>
-          <zorder>label_3</zorder>
-          <zorder>label_6</zorder>
-          <zorder>mulBtn</zorder>
-          <zorder>label_2</zorder>
-          <zorder>label_7</zorder>
-          <zorder>rebinBtn</zorder>
-          <zorder>monscaleBtn</zorder>
-          <zorder>shiftConstEdit</zorder>
-          <zorder>monscaleEdit</zorder>
-          <zorder>addConstEdit</zorder>
-          <zorder>scaleConstEdit</zorder>
-          <zorder>shiftBtn</zorder>
-          <zorder>addBtn</zorder>
-          <zorder>label_9</zorder>
-          <zorder>scaleXConstEdit</zorder>
-          <zorder>scaleXBtn</zorder>
-        </widget>
-      </item>
-      <item row="1" column="0" colspan="2">
-        <widget class="QGroupBox" name="groupBox_3">
-          <property name="title">
-            <string>Data extraction</string>
-          </property>
-          <layout class="QVBoxLayout" name="verticalLayout_2">
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_3">
-                <item>
-                  <widget class="QLabel" name="label_5">
-                    <property name="text">
-                      <string>Merge all with precision:</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QLineEdit" name="mergeEdit">
-                    <property name="text">
-                      <string>0.001</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="floatMergeBtn">
-                    <property name="text">
-                      <string>Float merge</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="mergeBtn">
-                    <property name="text">
-                      <string>Merge + Rebin</string>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_4">
-                <item>
-                  <widget class="QLabel" name="label_4">
-                    <property name="text">
-                      <string>Create dataset from parameter(s):</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="paramsetBtn">
-                    <property name="text">
-                      <string>Do it</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <spacer name="horizontalSpacer_3">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>0</width>
-                        <height>0</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="mappingBtn">
-                    <property name="text">
-                      <string>Make mapping</string>
-                    </property>
-                    <property name="icon">
-                      <iconset resource="../../../resource/gui.qrc">
-                        <normaloff>:/map.png</normaloff>
-                        :/map.png
-                      </iconset>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-            <item>
-              <spacer name="verticalSpacer">
-                <property name="orientation">
-                  <enum>Qt::Vertical</enum>
-                </property>
-                <property name="sizeHint" stdset="0">
-                  <size>
-                    <width>0</width>
-                    <height>0</height>
-                  </size>
-                </property>
-              </spacer>
-            </item>
-          </layout>
-        </widget>
-      </item>
-      <item row="0" column="1">
-        <widget class="QGroupBox" name="groupBox_2">
-          <property name="title">
-            <string>Modeling &amp;&amp; Fitting</string>
+          <property name="widgetResizable">
+            <bool>true</bool>
           </property>
-          <layout class="QVBoxLayout" name="verticalLayout">
-            <item>
-              <widget class="QLabel" name="label_8">
-                <property name="text">
-                  <string>Use the model from this dataset for all selected:</string>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <widget class="QComboBox" name="onemodelBox"/>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout">
-                <item>
-                  <widget class="QCheckBox" name="onemodelWithParamsBox">
-                    <property name="text">
-                      <string>With param values</string>
-                    </property>
-                    <property name="checked">
-                      <bool>true</bool>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <spacer name="horizontalSpacer">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>0</width>
-                        <height>0</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="onemodelBtn">
-                    <property name="text">
-                      <string>Copy model</string>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-            <item>
-              <widget class="Line" name="line">
-                <property name="orientation">
-                  <enum>Qt::Horizontal</enum>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_2">
-                <item>
-                  <widget class="QPushButton" name="fitallBtn">
-                    <property name="text">
-                      <string>Fit all datasets</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <spacer name="horizontalSpacer_2">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>0</width>
-                        <height>0</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="globalfitBtn">
-                    <property name="text">
-                      <string>Global fit</string>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-          </layout>
+          <widget class="QWidget" name="scrollAreaWidgetContents">
+            <property name="geometry">
+              <rect>
+                <x>0</x>
+                <y>0</y>
+                <width>612</width>
+                <height>468</height>
+              </rect>
+            </property>
+            <layout class="QGridLayout" name="gridLayout_3">
+              <property name="leftMargin">
+                <number>0</number>
+              </property>
+              <property name="topMargin">
+                <number>0</number>
+              </property>
+              <property name="bottomMargin">
+                <number>0</number>
+              </property>
+              <item row="0" column="0">
+                <widget class="QGroupBox" name="groupBox">
+                  <property name="title">
+                    <string>Data manipulation</string>
+                  </property>
+                  <layout class="QGridLayout" name="gridLayout_2">
+                    <item row="2" column="2">
+                      <widget class="QPushButton" name="mulBtn">
+                        <property name="text">
+                          <string>Scale</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="2">
+                      <widget class="QPushButton" name="rebinBtn">
+                        <property name="text">
+                          <string>Rebin</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="3" column="0">
+                      <widget class="QLabel" name="label_3">
+                        <property name="sizePolicy">
+                          <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                            <horstretch>0</horstretch>
+                            <verstretch>0</verstretch>
+                          </sizepolicy>
+                        </property>
+                        <property name="text">
+                          <string>Shift X values:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="2">
+                      <widget class="QPushButton" name="addBtn">
+                        <property name="text">
+                          <string>Add</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
+                      <widget class="QLabel" name="label">
+                        <property name="sizePolicy">
+                          <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                            <horstretch>0</horstretch>
+                            <verstretch>0</verstretch>
+                          </sizepolicy>
+                        </property>
+                        <property name="text">
+                          <string>Add a constant:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QLineEdit" name="precisionEdit">
+                        <property name="text">
+                          <string>0.001</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="3" column="2">
+                      <widget class="QPushButton" name="shiftBtn">
+                        <property name="text">
+                          <string>Shift</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="label_2">
+                        <property name="sizePolicy">
+                          <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                            <horstretch>0</horstretch>
+                            <verstretch>0</verstretch>
+                          </sizepolicy>
+                        </property>
+                        <property name="text">
+                          <string>Rebin individual sets:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="5" column="2">
+                      <widget class="QPushButton" name="monscaleBtn">
+                        <property name="text">
+                          <string>Change</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="5" column="1">
+                      <widget class="QLineEdit" name="monscaleEdit">
+                        <property name="text">
+                          <string>10000</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="3" column="1">
+                      <widget class="QLineEdit" name="shiftConstEdit">
+                        <property name="text">
+                          <string>0</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="1">
+                      <widget class="QLineEdit" name="scaleConstEdit">
+                        <property name="text">
+                          <string>1</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="4" column="2">
+                      <widget class="QPushButton" name="scaleXBtn">
+                        <property name="text">
+                          <string>Scale</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="4" column="1">
+                      <widget class="QLineEdit" name="scaleXConstEdit">
+                        <property name="text">
+                          <string>1</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="1">
+                      <widget class="QLineEdit" name="addConstEdit">
+                        <property name="text">
+                          <string>0</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="4" column="0">
+                      <widget class="QLabel" name="label_9">
+                        <property name="text">
+                          <string>Scale X values:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="5" column="0">
+                      <widget class="QLabel" name="label_6">
+                        <property name="sizePolicy">
+                          <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                            <horstretch>0</horstretch>
+                            <verstretch>0</verstretch>
+                          </sizepolicy>
+                        </property>
+                        <property name="text">
+                          <string>Change monitor:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="0">
+                      <widget class="QLabel" name="label_7">
+                        <property name="sizePolicy">
+                          <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
+                            <horstretch>0</horstretch>
+                            <verstretch>0</verstretch>
+                          </sizepolicy>
+                        </property>
+                        <property name="text">
+                          <string>Scale Y values:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="6" column="2">
+                      <widget class="QPushButton" name="massrenameBtn">
+                        <property name="text">
+                          <string>Rename...</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                  <zorder>precisionEdit</zorder>
+                  <zorder>label</zorder>
+                  <zorder>label_3</zorder>
+                  <zorder>label_6</zorder>
+                  <zorder>mulBtn</zorder>
+                  <zorder>label_2</zorder>
+                  <zorder>label_7</zorder>
+                  <zorder>rebinBtn</zorder>
+                  <zorder>monscaleBtn</zorder>
+                  <zorder>shiftConstEdit</zorder>
+                  <zorder>monscaleEdit</zorder>
+                  <zorder>addConstEdit</zorder>
+                  <zorder>scaleConstEdit</zorder>
+                  <zorder>shiftBtn</zorder>
+                  <zorder>addBtn</zorder>
+                  <zorder>label_9</zorder>
+                  <zorder>scaleXConstEdit</zorder>
+                  <zorder>scaleXBtn</zorder>
+                  <zorder>massrenameBtn</zorder>
+                </widget>
+              </item>
+              <item row="0" column="1">
+                <widget class="QGroupBox" name="groupBox_2">
+                  <property name="title">
+                    <string>Modeling &amp;&amp; Fitting</string>
+                  </property>
+                  <layout class="QVBoxLayout" name="verticalLayout">
+                    <item>
+                      <widget class="QLabel" name="label_8">
+                        <property name="text">
+                          <string>Use the model from this dataset for all selected:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QComboBox" name="onemodelBox"/>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout">
+                        <item>
+                          <widget class="QCheckBox" name="onemodelWithParamsBox">
+                            <property name="text">
+                              <string>With param values/limits</string>
+                            </property>
+                            <property name="checked">
+                              <bool>true</bool>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <spacer name="horizontalSpacer">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>0</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="onemodelBtn">
+                            <property name="text">
+                              <string>Copy model</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </item>
+                    <item>
+                      <widget class="Line" name="line">
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout_2">
+                        <item>
+                          <widget class="QPushButton" name="fitallBtn">
+                            <property name="text">
+                              <string>Fit all datasets</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <spacer name="horizontalSpacer_2">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>0</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="globalfitBtn">
+                            <property name="text">
+                              <string>Global fit</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </item>
+                    <item>
+                      <widget class="QLabel" name="fitallLbl">
+                        <property name="text">
+                          <string/>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </widget>
+              </item>
+              <item row="1" column="0" colspan="2">
+                <widget class="QGroupBox" name="groupBox_3">
+                  <property name="title">
+                    <string>Data extraction</string>
+                  </property>
+                  <layout class="QVBoxLayout" name="verticalLayout_2">
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout_3">
+                        <item>
+                          <widget class="QLabel" name="label_5">
+                            <property name="text">
+                              <string>Merge all with precision:</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLineEdit" name="mergeEdit">
+                            <property name="text">
+                              <string>0.001</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="floatMergeBtn">
+                            <property name="text">
+                              <string>Float merge</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="mergeBtn">
+                            <property name="text">
+                              <string>Merge + Rebin</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout_4">
+                        <item>
+                          <widget class="QLabel" name="label_4">
+                            <property name="text">
+                              <string>Create dataset from parameter(s):</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="paramsetBtn">
+                            <property name="text">
+                              <string>Do it</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <spacer name="horizontalSpacer_3">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>0</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="mappingBtn">
+                            <property name="text">
+                              <string>Make mapping</string>
+                            </property>
+                            <property name="icon">
+                              <iconset resource="../../../resource/gui.qrc">
+                                <normaloff>:/map.png</normaloff>
+                                :/map.png
+                              </iconset>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </item>
+                    <item>
+                      <spacer name="verticalSpacer">
+                        <property name="orientation">
+                          <enum>Qt::Vertical</enum>
+                        </property>
+                        <property name="sizeHint" stdset="0">
+                          <size>
+                            <width>0</width>
+                            <height>0</height>
+                          </size>
+                        </property>
+                      </spacer>
+                    </item>
+                  </layout>
+                </widget>
+              </item>
+            </layout>
+          </widget>
         </widget>
       </item>
     </layout>
   </widget>
   <resources>
     <include location="../../../resource/gui.qrc"/>
   </resources>
```

### Comparing `ufit-1.8.2/ufit/gui/ui/paramselect.ui` & `ufit-1.9.0/ufit/gui/ui/paramselect.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/paramset.ui` & `ufit-1.9.0/ufit/gui/ui/paramset.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/printpreview.ui` & `ufit-1.9.0/ufit/gui/ui/printpreview.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/qexplorer.ui` & `ufit-1.9.0/ufit/gui/ui/qexplorer.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/rebin.ui` & `ufit-1.9.0/ufit/gui/ui/rebin.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/reorder.ui` & `ufit-1.9.0/ufit/gui/ui/reorder.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/gui/ui/subtract.ui` & `ufit-1.9.0/ufit/gui/ui/subtract.ui`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/guires_qt5.py` & `ufit-1.9.0/ufit/guires_qt5.py`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/guires_qt6.py` & `ufit-1.9.0/ufit/guires_qt6.py`

 * *Files identical despite different names*

### Comparing `ufit-1.8.2/ufit/models/__init__.py` & `ufit-1.9.0/ufit/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Models package for ufit."""
 
 from ufit.models.base import *
 from ufit.models.conv import *
```

### Comparing `ufit-1.8.2/ufit/models/base.py` & `ufit-1.9.0/ufit/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """ufit base models."""
 
 import inspect
 import operator
```

### Comparing `ufit-1.8.2/ufit/models/conv.py` & `ufit-1.9.0/ufit/models/conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Convolution models."""
 
 import re
```

### Comparing `ufit-1.8.2/ufit/models/corr.py` & `ufit-1.9.0/ufit/models/corr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Models for several data corrections."""
 
 from numpy import arcsin, exp, pi, sqrt, tan
```

### Comparing `ufit-1.8.2/ufit/models/other.py` & `ufit-1.9.0/ufit/models/other.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Diverse other models."""
 
 from numpy import cos, exp, log, pi, piecewise, sign, sin, tanh
```

### Comparing `ufit-1.8.2/ufit/models/peaks.py` & `ufit-1.9.0/ufit/models/peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Models for different peak shapes."""
 
 from numpy import cos, exp, log, pi, sin, sqrt
 from scipy.special import wofz
```

### Comparing `ufit-1.8.2/ufit/models/sqwtas.py` & `ufit-1.9.0/ufit/models/sqwtas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Model of S(q,w) with resolution convolution for TAS."""
 
 import inspect
```

### Comparing `ufit-1.8.2/ufit/param.py` & `ufit-1.9.0/ufit/param.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Parameter definition class and helper functions for evaluating parameters."""
 
 import copy
 import re
```

### Comparing `ufit-1.8.2/ufit/plotting.py` & `ufit-1.9.0/ufit/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Plotting routines for ufit using matplotlib."""
 
 from itertools import cycle
 
@@ -108,15 +108,15 @@
             axes.errorbar(data.x_plot[~mask], data.y[~mask] + offset,
                           data.dy[~mask], ls='', marker=marker, ms=ms,
                           picker=5, mfc='white', mec=color, **kw)
         if not multi:
             if data.fitmin is not None:
                 axes.axvline(data.fitmin, ls='-', color='gray')
             if data.fitmax is not None:
-                axes.axvline(data.fitmax, ls='-', color='grey')
+                axes.axvline(data.fitmax, ls='-', color='gray')
             axes.set_title('%s\n%s' % (data.title, data.subtitle))
             self.plot_finish(data.xaxis, data.yaxis)
         return color
 
     def plot_finish(self, xlabel=None, ylabel=None, title=None):
         axes = self.axes
         if xlabel is not None:
```

### Comparing `ufit-1.8.2/ufit/qreader.py` & `ufit-1.9.0/ufit/qreader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 import numpy as np
 
 import ufit.lab as uf
```

### Comparing `ufit-1.8.2/ufit/qt.py` & `ufit-1.9.0/ufit/qt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Qt compatibility layer."""
 
 # pylint: disable=wildcard-import, unused-import, unused-wildcard-import
```

### Comparing `ufit-1.8.2/ufit/rescalc.py` & `ufit-1.9.0/ufit/rescalc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """
 Resolution calculation using the Popovici method.  Based on
 neutrons.instruments.tas.tasres from the neutrons Python package, compiled by
 Marc Janoschek.
```

### Comparing `ufit-1.8.2/ufit/result.py` & `ufit-1.9.0/ufit/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Fit result class."""
 
 import copy
```

### Comparing `ufit-1.8.2/ufit/utils.py` & `ufit-1.9.0/ufit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 """Utility functions and classes."""
 
 import re
 from os import path
```

### Comparing `ufit-1.8.2/ufit/version.py` & `ufit-1.9.0/ufit/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 # *****************************************************************************
 # ufit, a universal scattering fitting suite
 #
-# Copyright (c) 2013-2023, Georg Brandl and contributors.  All rights reserved.
+# Copyright (c) 2013-2024, Georg Brandl and contributors.  All rights reserved.
 # Licensed under a 2-clause BSD license, see LICENSE.
 # *****************************************************************************
 
 # Original author: Douglas Creager <dcreager@dcreager.net>
 # This file is placed into the public domain.
 
 import os.path
```

