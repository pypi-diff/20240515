# Comparing `tmp/pyams_content-1.99.3.tar.gz` & `tmp/pyams_content-1.99.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_content-1.99.3.tar", last modified: Sun May  5 21:03:27 2024, max compression
+gzip compressed data, was "dist/pyams_content-1.99.4.tar", last modified: Wed May 15 16:47:45 2024, max compression
```

## Comparing `pyams_content-1.99.3.tar` & `pyams_content-1.99.4.tar`

### file list

```diff
@@ -1,659 +1,659 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-05 21:02:51.000000 pyams_content-1.99.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-05 21:02:51.000000 pyams_content-1.99.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2753 2024-05-05 21:03:27.000000 pyams_content-1.99.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/docs/
--rwxrwxrwx   0 root         (0) root         (0)      920 2024-05-05 21:02:51.000000 pyams_content-1.99.3/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-05 21:02:51.000000 pyams_content-1.99.3/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 21:03:27.000000 pyams_content-1.99.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3377 2024-05-05 21:02:51.000000 pyams_content-1.99.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/association/
--rw-rw-rw-   0 root         (0) root         (0)     3402 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4072 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3230 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2091 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2162 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/templates/association-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1960 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/templates/association-viewlet.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5882 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9011 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2039 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/calendar/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/cards/
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     1773 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/cards.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/cards/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2094 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/contact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/
--rw-rw-rw-   0 root         (0) root         (0)     7387 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     9775 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2467 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3254 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     2798 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3504 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5218 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/mail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/templates/form-submit.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/templates/paragraph-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/file/
--rw-rw-rw-   0 root         (0) root         (0)     1583 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/frame/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/frame/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/frame/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/
--rw-rw-rw-   0 root         (0) root         (0)     6052 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     1661 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4654 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2175 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt
--rw-rw-rw-   0 root         (0) root         (0)     2954 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4053 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt
--rw-rw-rw-   0 root         (0) root         (0)     2891 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-random.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8399 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11985 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1995 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/
--rw-rw-rw-   0 root         (0) root         (0)     7780 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4725 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2005 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6710 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1390 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     2530 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/templates/illustration-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6234 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/illustration.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/illustration-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/illustration-side.pt
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5108 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/paragraph.py
--rw-rw-rw-   0 root         (0) root         (0)     1989 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/keynumber/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/keynumber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/links/
--rw-rw-rw-   0 root         (0) root         (0)    10891 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4819 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/html.py
--rw-rw-rw-   0 root         (0) root         (0)     5037 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/links/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8653 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/map/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/map/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/milestone/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/milestone/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/
--rw-rw-rw-   0 root         (0) root         (0)     6756 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5966 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     5173 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4693 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     7591 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4105 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/templates/navigation-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7323 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/html.pt
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/raw-code.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/raw.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    17744 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17950 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     4263 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/templates/title-toolbar.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/pictogram/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/pictogram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/
--rw-rw-rw-   0 root         (0) root         (0)     7603 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2699 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/templates/tags.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12144 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     6509 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/verbatim/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/verbatim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/
--rw-rw-rw-   0 root         (0) root         (0)     2307 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3286 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/dailymotion.py
--rw-rw-rw-   0 root         (0) root         (0)     9322 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/vimeo.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/
--rw-rw-rw-   0 root         (0) root         (0)     2159 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/dailymotion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/custom-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/dailymotion-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      542 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/youtube-render.pt
--rw-rw-rw-   0 root         (0) root         (0)     1503 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/vimeo.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/templates/video-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12014 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/
--rw-rw-rw-   0 root         (0) root         (0)     3608 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2142 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/alerts.pt
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/context-alerts.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2205 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/audit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6737 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1803 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/sitemap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary-sitemap.pt
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary.pt
--rw-rw-rw-   0 root         (0) root         (0)     1731 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-associations.pt
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-body.pt
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-footer.pt
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     3568 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/term.py
--rw-rw-rw-   0 root         (0) root         (0)     3180 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/history/
--rw-rw-rw-   0 root         (0) root         (0)     3000 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/templates/history.pt
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/html/
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/html/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/
--rw-rw-rw-   0 root         (0) root         (0)     6800 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     3392 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3551 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2154 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1339 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3353 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7344 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2670 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/qrcode/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/qrcode/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/redirect/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/redirect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/renderer/
--rw-rw-rw-   0 root         (0) root         (0)     5451 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/renderer/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/review/
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3253 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/chat.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4664 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    11045 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/comment.pt
--rw-rw-rw-   0 root         (0) root         (0)     2784 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/comments.pt
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/mail-notification.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/
--rw-rw-rw-   0 root         (0) root         (0)     3169 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7419 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3804 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4861 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2527 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)    11035 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6230 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt
--rw-rw-rw-   0 root         (0) root         (0)     5146 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     5176 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt
--rw-rw-rw-   0 root         (0) root         (0)     4985 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1187 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt
--rw-rw-rw-   0 root         (0) root         (0)     5184 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt
--rw-rw-rw-   0 root         (0) root         (0)     4002 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/zmi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1258 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7625 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3101 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     3955 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/share/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/share/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/
--rw-rw-rw-   0 root         (0) root         (0)     4558 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/
--rw-rw-rw-   0 root         (0) root         (0)      299 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/humans.pt
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/robots.pt
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/root-sitemap.pt
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/toolbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/toolbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/generations/
--rw-rw-rw-   0 root         (0) root         (0)    10545 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9656 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     4659 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)   125110 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo
--rw-rw-rw-   0 root         (0) root         (0)   225312 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po
--rw-rw-rw-   0 root         (0) root         (0)   162899 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/locales/pyams_content.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/
--rw-rw-rw-   0 root         (0) root         (0)     4561 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/
--rw-rw-rw-   0 root         (0) root         (0)     1996 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2917 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     6747 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3851 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/templates/pictogram-header.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)     2896 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/templates/selection-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     3174 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4440 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/root/
--rw-rw-rw-   0 root         (0) root         (0)     4904 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6721 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4841 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3885 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25806 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    13639 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5338 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/sites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5270 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2824 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3268 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     9134 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/blog/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/blog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/calendar/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)    11763 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    15461 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5998 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/header.py
--rw-rw-rw-   0 root         (0) root         (0)     5197 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1762 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2618 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/specificities-default.pt
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/title-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/title.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/specificities.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/title.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/specificities-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/title-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1369 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/title.py
--rw-rw-rw-   0 root         (0) root         (0)     9807 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)     3877 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2333 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/oid.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/templates/breadcrumbs.pt
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/templates/card-datatype.pt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/templates/publication-date.pt
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/title.py
--rw-rw-rw-   0 root         (0) root         (0)     2556 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/types.py
--rw-rw-rw-   0 root         (0) root         (0)     4801 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/url.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    12425 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    23132 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14934 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/content.py
--rw-rw-rw-   0 root         (0) root         (0)    36824 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3872 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4679 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    18561 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/owner.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/portal.py
--rw-rw-rw-   0 root         (0) root         (0)     2899 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/reference.py
--rw-rw-rw-   0 root         (0) root         (0)    18640 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)    17565 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     8992 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      537 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/content-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/content-workflow.pt
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/owner-change.pt
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/quick-search.pt
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/sequence-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/
--rw-rw-rw-   0 root         (0) root         (0)     7226 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5005 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/container.py
--rw-rw-rw-   0 root         (0) root         (0)     2605 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/content.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     3179 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29957 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/file/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/form/
--rw-rw-rw-   0 root         (0) root         (0)     2560 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/form/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2046 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/form/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/hub/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/hub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/logo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/logo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/logo/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1149 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/logo/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/news/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/news/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/resource/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/container.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     8784 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7205 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/link.py
--rw-rw-rw-   0 root         (0) root         (0)     5429 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8526 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/folder.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    15922 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/link.py
--rw-rw-rw-   0 root         (0) root         (0)     8144 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5391 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/rename.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/topic.py
--rw-rw-rw-   0 root         (0) root         (0)    21405 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     1899 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/
--rw-rw-rw-   0 root         (0) root         (0)     8677 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     7663 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/query.py
--rw-rw-rw-   0 root         (0) root         (0)     5853 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6223 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4700 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5886 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6787 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
--rw-rw-rw-   0 root         (0) root         (0)     2449 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     2666 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/zmi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     6586 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/query.py
--rw-rw-rw-   0 root         (0) root         (0)     6661 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/skin/templates/preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     7845 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4191 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/zmi/references.py
--rw-rw-rw-   0 root         (0) root         (0)     6188 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/skin/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/workflow/
--rw-rw-rw-   0 root         (0) root         (0)    48067 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21211 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/basic.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4984 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/notify.py
--rw-rw-rw-   0 root         (0) root         (0)     6360 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/publication.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/templates/publication-header.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7680 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     2383 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/html.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/properties.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    19424 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/content.js
--rw-rw-rw-   0 root         (0) root         (0)    10283 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/content.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/langs/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/langs/fr.js
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/viewlet/toplinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/seo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1260 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/templates/seo-textline-input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2753 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24617 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:03:18.000000 pyams_content-1.99.3/src/pyams_content.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-15 16:47:01.000000 pyams_content-1.99.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-15 16:47:01.000000 pyams_content-1.99.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-05-15 16:47:45.000000 pyams_content-1.99.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      998 2024-05-15 16:47:01.000000 pyams_content-1.99.4/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-15 16:47:01.000000 pyams_content-1.99.4/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 16:47:45.000000 pyams_content-1.99.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3377 2024-05-15 16:47:01.000000 pyams_content-1.99.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/association/
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/association/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/association/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/skin/templates/association-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/skin/templates/association-viewlet.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/association/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5882 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9011 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2039 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/association/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/cards/
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/cards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/cards/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/cards/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/cards/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/cards/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/cards/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/cards/skin/templates/cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/cards/skin/templates/cards.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/cards/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/cards/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/contact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/
+-rw-rw-rw-   0 root         (0) root         (0)     7387 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     9775 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3254 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/fields/
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/fields/handler/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3504 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/handler/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5218 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/handler/mail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/fields/handler/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/handler/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/handler/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/fields/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/fields/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/skin/templates/form-submit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/skin/templates/paragraph-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/fields/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/fields/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/file/
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/frame/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/frame/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/frame/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1661 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4053 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/skin/templates/gallery-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/skin/templates/gallery-random.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8399 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/
+-rw-rw-rw-   0 root         (0) root         (0)     7780 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6710 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/zmi/templates/illustration-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/illustration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/templates/illustration-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/templates/illustration-side.pt
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/zmi/paragraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/illustration/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/keynumber/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/keynumber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/links/
+-rw-rw-rw-   0 root         (0) root         (0)    10891 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4819 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/links/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/links/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/links/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8653 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/links/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/links/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/links/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/map/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/map/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/milestone/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/milestone/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/
+-rw-rw-rw-   0 root         (0) root         (0)     6756 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5966 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     5173 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/interfaces/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     7591 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/zmi/templates/navigation-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7323 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/interfaces/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/templates/html.pt
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/templates/raw-code.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/templates/raw.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    17744 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17950 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4263 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/templates/title-toolbar.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/pictogram/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/pictogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/
+-rw-rw-rw-   0 root         (0) root         (0)     7603 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/skin/templates/tags.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12216 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     6509 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/thesaurus/zmi/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/verbatim/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/verbatim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/video/
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/video/provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3286 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/provider/dailymotion.py
+-rw-rw-rw-   0 root         (0) root         (0)     9322 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/provider/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/provider/vimeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/provider/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/dailymotion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/templates/custom-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/templates/dailymotion-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/templates/youtube-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/vimeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/skin/templates/video-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/component/video/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12014 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/component/video/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2142 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/skin/templates/alerts.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/skin/templates/context-alerts.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/alert/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/audit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6737 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/sitemap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/glossary-sitemap.pt
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/glossary.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/term-associations.pt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/term-body.pt
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/term-footer.pt
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/term-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/term-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3568 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/glossary/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/history/
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/history/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/history/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/history/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/history/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/history/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/history/zmi/templates/history.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/history/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/html/
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/html/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/
+-rw-rw-rw-   0 root         (0) root         (0)     6800 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     3392 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3551 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7344 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/navigation/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/preview/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/preview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/preview/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/preview/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/preview/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/preview/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/qrcode/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/qrcode/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/redirect/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/redirect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     5451 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/renderer/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/review/
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/review/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/review/chat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/review/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/review/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/review/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    11045 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/review/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/review/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/review/zmi/templates/comment.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/review/zmi/templates/comments.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/review/zmi/templates/mail-notification.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/search/
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7419 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)    11035 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6230 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5176 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4002 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/zmi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/search/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7625 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/zmi/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/search/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/share/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/share/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/sitemap/
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/sitemap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/sitemap/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/sitemap/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/sitemap/templates/humans.pt
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/sitemap/templates/robots.pt
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/sitemap/templates/root-sitemap.pt
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/feature/toolbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/feature/toolbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/generations/
+-rw-rw-rw-   0 root         (0) root         (0)    10545 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9656 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)   125110 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo
+-rw-rw-rw-   0 root         (0) root         (0)   225312 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po
+-rw-rw-rw-   0 root         (0) root         (0)   162899 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/locales/pyams_content.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2917 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/templates/pictogram-header.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/templates/selection-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4440 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/reference/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/reference/zmi/viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/root/
+-rw-rw-rw-   0 root         (0) root         (0)     4904 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6721 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/root/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4841 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/root/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25806 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/root/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13639 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/root/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     5338 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/root/zmi/sites.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5270 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9134 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/alert/zmi/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/blog/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/blog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)    11763 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    15461 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5998 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/interfaces/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/templates/specificities-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/templates/title-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/specificities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/title.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1435 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/templates/specificities-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/templates/title-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     9807 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3877 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/oid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/templates/breadcrumbs.pt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/templates/card-datatype.pt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/templates/publication-date.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     4801 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/skin/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    12425 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    23132 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14934 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/content.py
+-rw-rw-rw-   0 root         (0) root         (0)    36824 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3872 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    18561 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/owner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/portal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2899 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    18640 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17565 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     8992 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      537 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/content-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/content-workflow.pt
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/owner-change.pt
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/quick-search.pt
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/sequence-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/
+-rw-rw-rw-   0 root         (0) root         (0)     7226 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5005 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/content.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29957 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/common/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/file/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/form/
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/form/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/form/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/form/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/form/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/form/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/form/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/form/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/hub/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/hub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/logo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/logo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/logo/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/logo/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/news/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/news/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/resource/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8784 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7205 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     5429 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8526 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    15922 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     8144 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5391 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/rename.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)    21405 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/topic/
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/topic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/topic/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/topic/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/topic/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/topic/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/
+-rw-rw-rw-   0 root         (0) root         (0)     8677 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     7663 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/interfaces/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5853 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/interfaces/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6223 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4700 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6787 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/zmi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6586 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/skin/templates/preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     7845 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/shared/view/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4191 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/zmi/references.py
+-rw-rw-rw-   0 root         (0) root         (0)     6323 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/shared/view/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/workflow/
+-rw-rw-rw-   0 root         (0) root         (0)    48067 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21211 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4984 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/notify.py
+-rw-rw-rw-   0 root         (0) root         (0)     6360 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/workflow/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/zmi/publication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/workflow/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/workflow/zmi/templates/publication-header.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7680 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2383 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/properties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    19424 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/content.js
+-rw-rw-rw-   0 root         (0) root         (0)    10283 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/content.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/headers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/headers/langs/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/headers/langs/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/internal-link/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/viewlet/toplinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/widget/seo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-05-15 16:47:01.000000 pyams_content-1.99.4/src/pyams_content/zmi/widget/templates/seo-textline-input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24617 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:47:35.000000 pyams_content-1.99.4/src/pyams_content.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-15 16:47:45.000000 pyams_content-1.99.4/src/pyams_content.egg-info/top_level.txt
```

### Comparing `pyams_content-1.99.3/LICENSE` & `pyams_content-1.99.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/PKG-INFO` & `pyams_content-1.99.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_content
-Version: 1.99.3
+Version: 1.99.4
 Summary: PyAMS content management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS CMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,14 +48,18 @@
 Please note that PyAMS_content only provide a basic Bootstrap based skin, so you will have to
 include other extension packages (like PyAMS_content_themes) to get more advanced graphical themes.
 
 
 Changelog
 =========
 
+1.99.4
+------
+ - removed arguments override in thesaurus handlers components
+
 1.99.3
 ------
  - updated shared content header viewlet to add button to go back to dashboard
  - added status to scheduler tasks execution result
  - added support for direct content retiring or archiving for managers
  - added support for custom modal content class
```

### Comparing `pyams_content-1.99.3/docs/HISTORY.rst` & `pyams_content-1.99.4/docs/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.99.4
+------
+ - removed arguments override in thesaurus handlers components
+
 1.99.3
 ------
  - updated shared content header viewlet to add button to go back to dashboard
  - added status to scheduler tasks execution result
  - added support for direct content retiring or archiving for managers
  - added support for custom modal content class
```

### Comparing `pyams_content-1.99.3/docs/README.rst` & `pyams_content-1.99.4/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/setup.py` & `pyams_content-1.99.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.3'
+version = '1.99.4'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_security_views',
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
```

### Comparing `pyams_content-1.99.3/src/pyams_content/__init__.py` & `pyams_content-1.99.4/src/pyams_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/association/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/container.py` & `pyams_content-1.99.4/src/pyams_content/component/association/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/association/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/association/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/association/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/skin/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/association/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/skin/templates/association-viewlet.pt` & `pyams_content-1.99.4/src/pyams_content/component/association/skin/templates/association-viewlet.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/association/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/zmi/container.py` & `pyams_content-1.99.4/src/pyams_content/component/association/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/association/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/association/zmi/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/association/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/calendar/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/cards/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/cards/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/cards/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/cards/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/cards/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/cards/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/cards/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/cards-masonry.pt` & `pyams_content-1.99.4/src/pyams_content/component/cards/skin/templates/cards-masonry.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/cards.pt` & `pyams_content-1.99.4/src/pyams_content/component/cards/skin/templates/cards.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/cards/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/cards/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/extfile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/extfile/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/manager.py` & `pyams_content-1.99.4/src/pyams_content/component/extfile/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/manager.py` & `pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt` & `pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt` & `pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/widget.py` & `pyams_content-1.99.4/src/pyams_content/component/extfile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/handler/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/handler/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/handler/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/handler/mail.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/handler/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/handler/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/mail.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/handler/zmi/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/skin/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/fields/zmi/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/fields/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/file/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/frame/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/frame/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/file.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/file.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-default.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/skin/templates/gallery-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-random.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/skin/templates/gallery-random.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/file.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/file.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/helpers.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/helpers.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt` & `pyams_content-1.99.4/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt` & `pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt` & `pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/illustration.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/skin/illustration.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/illustration-default.pt` & `pyams_content-1.99.4/src/pyams_content/component/illustration/skin/templates/illustration-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/illustration-side.pt` & `pyams_content-1.99.4/src/pyams_content/component/illustration/skin/templates/illustration-side.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt` & `pyams_content-1.99.4/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/thesaurus.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/thesaurus.py` & `pyams_content-1.99.4/src/pyams_content/component/illustration/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/keynumber/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/keynumber/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/links/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/links/html.py` & `pyams_content-1.99.4/src/pyams_content/component/links/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/links/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/links/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/links/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/links/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/links/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/links/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/links/zmi/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/links/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/map/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/map/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/milestone/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/milestone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/container.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/html.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/html.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/settings.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/html.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/html.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/html.pt` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/skin/templates/html.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/container.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/helper.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/helper.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/html.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/paragraph/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/thesaurus/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/thesaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/thesaurus/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/thesaurus/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/thesaurus/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/thesaurus/zmi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
                 context=ITagsTarget, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=350,
                 permission=VIEW_SYSTEM_PERMISSION)
 class TagsMenu(NavigationMenuItem):
     """Tags menu"""
 
     def __new__(cls, context, request, view, manager):  # pylint: disable=unused-argument
-        manager = ITagsManager(request.root, None)
-        if (manager is None) or not manager.thesaurus_name:
+        tags_manager = ITagsManager(request.root, None)
+        if (tags_manager is None) or not tags_manager.thesaurus_name:
             return None
         return NavigationMenuItem.__new__(cls)
 
     label = _("Tags")
     href = '#tags.html'
 
 
@@ -174,16 +174,16 @@
                 context=IThemesTarget, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=360,
                 permission=VIEW_SYSTEM_PERMISSION)
 class ThemesMenu(NavigationMenuItem):
     """Themes menu"""
 
     def __new__(cls, context, request, view, manager):  # pylint: disable=unused-argument
-        manager = IThemesManager(request.root, None)
-        if (manager is None) or not manager.thesaurus_name:
+        themes_manager = IThemesManager(request.root, None)
+        if (themes_manager is None) or not themes_manager.thesaurus_name:
             return None
         return NavigationMenuItem.__new__(cls)
 
     label = _("Themes")
     href = '#themes.html'
 
 
@@ -302,16 +302,16 @@
                 context=ICollectionsTarget, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=370,
                 permission=VIEW_SYSTEM_PERMISSION)
 class CollectionsMenu(NavigationMenuItem):
     """Collections menu"""
 
     def __new__(cls, context, request, view, manager):  # pylint: disable=unused-argument
-        manager = ICollectionsManager(request.root, None)
-        if (manager is None) or not manager.thesaurus_name:
+        collections_manager = ICollectionsManager(request.root, None)
+        if (collections_manager is None) or not collections_manager.thesaurus_name:
             return None
         return NavigationMenuItem.__new__(cls)
 
     label = _("Collections")
     href = '#collections.html'
```

### Comparing `pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/thesaurus/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/manager.py` & `pyams_content-1.99.4/src/pyams_content/component/thesaurus/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/video/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/video/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/video/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/provider/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/video/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/provider/dailymotion.py` & `pyams_content-1.99.4/src/pyams_content/component/video/provider/dailymotion.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/provider/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/video/provider/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/provider/vimeo.py` & `pyams_content-1.99.4/src/pyams_content/component/video/provider/vimeo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/provider/youtube.py` & `pyams_content-1.99.4/src/pyams_content/component/video/provider/youtube.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/video/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/component/video/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/dailymotion.py` & `pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/dailymotion.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt` & `pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/vimeo.py` & `pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/vimeo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/youtube.py` & `pyams_content-1.99.4/src/pyams_content/component/video/skin/provider/youtube.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/skin/templates/video-default.pt` & `pyams_content-1.99.4/src/pyams_content/component/video/skin/templates/video-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/component/video/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/component/video/zmi/paragraph.py` & `pyams_content-1.99.4/src/pyams_content/component/video/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/doctests/README.rst` & `pyams_content-1.99.4/src/pyams_content/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/alert/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/alert/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/alert/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/alert/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/alert/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/alerts.pt` & `pyams_content-1.99.4/src/pyams_content/feature/alert/skin/templates/alerts.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/context-alerts.pt` & `pyams_content-1.99.4/src/pyams_content/feature/alert/skin/templates/context-alerts.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/alert/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/alert/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/sitemap.py` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/sitemap.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary.pt` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/glossary.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-associations.pt` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/term-associations.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/term.py` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/skin/term.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/task.py` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/glossary/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/glossary/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/history/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/history/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/history/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/history/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/history/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/history/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/history/zmi/viewlet.py` & `pyams_content-1.99.4/src/pyams_content/feature/history/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/html/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/container.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/navigation/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/preview/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/preview/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/preview/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/preview/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt` & `pyams_content-1.99.4/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/renderer/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/renderer/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/renderer/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/review/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/review/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/review/chat.py` & `pyams_content-1.99.4/src/pyams_content/feature/review/chat.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/review/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/review/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/review/manager.py` & `pyams_content-1.99.4/src/pyams_content/feature/review/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/review/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/review/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/comment.pt` & `pyams_content-1.99.4/src/pyams_content/feature/review/zmi/templates/comment.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/comments.pt` & `pyams_content-1.99.4/src/pyams_content/feature/review/zmi/templates/comments.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/mail-notification.pt` & `pyams_content-1.99.4/src/pyams_content/feature/review/zmi/templates/mail-notification.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/manager.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/zmi.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/skin/zmi.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt` & `pyams_content-1.99.4/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/thesaurus.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/zmi/manager.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/zmi/reference.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/search/zmi/thesaurus.py` & `pyams_content-1.99.4/src/pyams_content/feature/search/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/sitemap/__init__.py` & `pyams_content-1.99.4/src/pyams_content/feature/sitemap/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/feature/sitemap/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/feature/sitemap/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/generations/__init__.py` & `pyams_content-1.99.4/src/pyams_content/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/include.py` & `pyams_content-1.99.4/src/pyams_content/include.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/interfaces/__init__.py` & `pyams_content-1.99.4/src/pyams_content/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo` & `pyams_content-1.99.4/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po` & `pyams_content-1.99.4/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po`

 * *Files 0% similar despite different names*

```diff
@@ -971,16 +971,16 @@
 msgstr "Bonjour,"
 
 #: src/pyams_content/feature/review/zmi/templates/mail-notification.pt:31
 msgid ""
 "You have been requested by ${sender}, contributor of « ${service_name} » "
 "website, to make a review of a content."
 msgstr ""
-"Vous êtes sollicité par ${sender}, contributor du site internet "
-"« ${service_name} », qui souhaite recueillir votre commentaire à propos d'un "
+"Vous êtes sollicité par ${sender}, contributor du site internet « "
+"${service_name} », qui souhaite recueillir votre commentaire à propos d'un "
 "contenu."
 
 #: src/pyams_content/feature/review/zmi/templates/mail-notification.pt:36
 msgid "${sender} added the following message to his request:"
 msgstr "${sender} a accompagné sa demande de relecture du message suivant :"
 
 #: src/pyams_content/feature/review/zmi/templates/mail-notification.pt:41
```

### Comparing `pyams_content-1.99.3/src/pyams_content/locales/pyams_content.pot` & `pyams_content-1.99.4/src/pyams_content/locales/pyams_content.pot`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/__init__.py` & `pyams_content-1.99.4/src/pyams_content/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/reference/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/__init__.py` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/manager.py` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/manager.py` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/table.py` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/__init__.py` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/manager.py` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt` & `pyams_content-1.99.4/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/zmi/table.py` & `pyams_content-1.99.4/src/pyams_content/reference/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/reference/zmi/viewlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/reference/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/root/__init__.py` & `pyams_content-1.99.4/src/pyams_content/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/root/configuration.py` & `pyams_content-1.99.4/src/pyams_content/root/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/root/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/root/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/root/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/root/zmi/dashboard.py` & `pyams_content-1.99.4/src/pyams_content/root/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/root/zmi/search.py` & `pyams_content-1.99.4/src/pyams_content/root/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/root/zmi/sites.py` & `pyams_content-1.99.4/src/pyams_content/root/zmi/sites.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/alert/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/alert/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/alert/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/alert/manager.py` & `pyams_content-1.99.4/src/pyams_content/shared/alert/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/alert/types.py` & `pyams_content-1.99.4/src/pyams_content/shared/alert/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/alert/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/alert/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/types.py` & `pyams_content-1.99.4/src/pyams_content/shared/alert/zmi/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/blog/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/blog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/calendar/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/types.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/interfaces/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/manager.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portal.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portal.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/header.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/header.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/specificities.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/title.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/skin/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/specificities.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/title.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/header.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/specificities.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/title.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/portlet/zmi/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/restrictions.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/security.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/security.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/skin/breadcrumb.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/skin/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/skin/oid.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/skin/oid.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/skin/specificities.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/skin/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/skin/title.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/skin/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/skin/types.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/skin/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/skin/url.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/skin/url.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/skin/workflow.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/skin/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/types.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/content.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/content.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/dashboard.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/header.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/manager.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/owner.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/owner.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/portal.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/portal.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/reference.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/restrictions.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/search.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/summary.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/summary.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/content-header.pt` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/content-header.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/quick-search.pt` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/quick-search.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/container.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/content.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/content.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/types/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/viewlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/workflow.py` & `pyams_content-1.99.4/src/pyams_content/shared/common/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/file/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/form/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/form/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/form/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/form/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/form/manager.py` & `pyams_content-1.99.4/src/pyams_content/shared/form/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/form/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/form/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/form/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/form/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/hub/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/logo/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/logo/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/container.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/folder.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/link.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/link.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/manager.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/topic.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/topic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/folder.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/link.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/link.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/manager.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/rename.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/rename.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/search.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/topic.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/topic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/tree.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/tree.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/viewlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/folder.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt` & `pyams_content-1.99.4/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/topic/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/topic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/topic/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/topic/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/topic/manager.py` & `pyams_content-1.99.4/src/pyams_content/shared/topic/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/topic/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/topic/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/query.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/interfaces/query.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/settings.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/manager.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/merge.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/merge.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/zmi.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/skin/zmi.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt` & `pyams_content-1.99.4/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/query.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/query.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/reference.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/thesaurus.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/zmi/references.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/zmi/references.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/shared/view/zmi/thesaurus.py` & `pyams_content-1.99.4/src/pyams_content/shared/view/zmi/thesaurus.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,16 +44,16 @@
                 context=IWfView, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=350,
                 permission=VIEW_SYSTEM_PERMISSION)
 class ViewTagsMenu(NavigationMenuItem):
     """View tags menu"""
 
     def __new__(cls, context, request, view, manager):
-        manager = ITagsManager(request.root, None)
-        if not manager.thesaurus_name:
+        tags_manager = ITagsManager(request.root, None)
+        if (tags_manager is None) or not tags_manager.thesaurus_name:
             return None
         return NavigationMenuItem.__new__(cls)
 
     label = _("Tags")
     href = '#tags.html'
 
 
@@ -92,16 +92,16 @@
                 context=IWfView, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=360,
                 permission=VIEW_SYSTEM_PERMISSION)
 class ViewThemesMenu(NavigationMenuItem):
     """View themes menu"""
 
     def __new__(cls, context, request, view, manager):
-        manager = IThemesManager(request.root, None)
-        if not manager.thesaurus_name:
+        themes_manager = IThemesManager(request.root, None)
+        if (themes_manager is None) or not themes_manager.thesaurus_name:
             return None
         return NavigationMenuItem.__new__(cls)
 
     label = _("Themes")
     href = '#themes.html'
 
 
@@ -140,16 +140,16 @@
                 context=IWfView, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=370,
                 permission=VIEW_SYSTEM_PERMISSION)
 class ViewCollectionsMenu(NavigationMenuItem):
     """View collections menu"""
 
     def __new__(cls, context, request, view, manager):
-        manager = ICollectionsManager(request.root, None)
-        if not manager.thesaurus_name:
+        collections_manager = ICollectionsManager(request.root, None)
+        if (collections_manager is None) or not collections_manager.thesaurus_name:
             return None
         return NavigationMenuItem.__new__(cls)
 
     label = _("Collections")
     href = '#collections.html'
```

### Comparing `pyams_content-1.99.3/src/pyams_content/skin/__init__.py` & `pyams_content-1.99.4/src/pyams_content/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/skin/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/tests/__init__.py` & `pyams_content-1.99.4/src/pyams_content/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/tests/test_utilsdocs.py` & `pyams_content-1.99.4/src/pyams_content/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/tests/test_utilsdocstrings.py` & `pyams_content-1.99.4/src/pyams_content/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/utils/__init__.py` & `pyams_content-1.99.4/src/pyams_content/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/workflow/__init__.py` & `pyams_content-1.99.4/src/pyams_content/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/workflow/basic.py` & `pyams_content-1.99.4/src/pyams_content/workflow/basic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/workflow/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/workflow/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/workflow/notify.py` & `pyams_content-1.99.4/src/pyams_content/workflow/notify.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/workflow/task.py` & `pyams_content-1.99.4/src/pyams_content/workflow/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/workflow/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/workflow/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/workflow/zmi/publication.py` & `pyams_content-1.99.4/src/pyams_content/workflow/zmi/publication.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/workflow/zmi/task.py` & `pyams_content-1.99.4/src/pyams_content/workflow/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/__init__.py` & `pyams_content-1.99.4/src/pyams_content/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/dashboard.py` & `pyams_content-1.99.4/src/pyams_content/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/html.py` & `pyams_content-1.99.4/src/pyams_content/zmi/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/properties.py` & `pyams_content-1.99.4/src/pyams_content/zmi/properties.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/content.js` & `pyams_content-1.99.4/src/pyams_content/zmi/resources/js/content.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/content.min.js` & `pyams_content-1.99.4/src/pyams_content/zmi/resources/js/content.min.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js` & `pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js` & `pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js` & `pyams_content-1.99.4/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/viewlet/__init__.py` & `pyams_content-1.99.4/src/pyams_content/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/viewlet/toplinks.py` & `pyams_content-1.99.4/src/pyams_content/zmi/viewlet/toplinks.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/widget/__init__.py` & `pyams_content-1.99.4/src/pyams_content/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/widget/interfaces.py` & `pyams_content-1.99.4/src/pyams_content/zmi/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/widget/seo.py` & `pyams_content-1.99.4/src/pyams_content/zmi/widget/seo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content/zmi/widget/templates/seo-textline-input.pt` & `pyams_content-1.99.4/src/pyams_content/zmi/widget/templates/seo-textline-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content.egg-info/PKG-INFO` & `pyams_content-1.99.4/src/pyams_content.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-content
-Version: 1.99.3
+Version: 1.99.4
 Summary: PyAMS content management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS CMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,14 +48,18 @@
 Please note that PyAMS_content only provide a basic Bootstrap based skin, so you will have to
 include other extension packages (like PyAMS_content_themes) to get more advanced graphical themes.
 
 
 Changelog
 =========
 
+1.99.4
+------
+ - removed arguments override in thesaurus handlers components
+
 1.99.3
 ------
  - updated shared content header viewlet to add button to go back to dashboard
  - added status to scheduler tasks execution result
  - added support for direct content retiring or archiving for managers
  - added support for custom modal content class
```

### Comparing `pyams_content-1.99.3/src/pyams_content.egg-info/SOURCES.txt` & `pyams_content-1.99.4/src/pyams_content.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.3/src/pyams_content.egg-info/requires.txt` & `pyams_content-1.99.4/src/pyams_content.egg-info/requires.txt`

 * *Files identical despite different names*

