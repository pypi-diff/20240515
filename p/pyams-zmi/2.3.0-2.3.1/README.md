# Comparing `tmp/pyams_zmi-2.3.0.tar.gz` & `tmp/pyams_zmi-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_zmi-2.3.0.tar", last modified: Sun May  5 20:47:11 2024, max compression
+gzip compressed data, was "dist/pyams_zmi-2.3.1.tar", last modified: Wed May 15 16:25:39 2024, max compression
```

## Comparing `pyams_zmi-2.3.0.tar` & `pyams_zmi-2.3.1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8335 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)     6697 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3129 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/doctests/rest.rst
--rw-rw-rw-   0 root         (0) root         (0)     1364 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/factory.py
--rw-rw-rw-   0 root         (0) root         (0)    11775 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/form.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/generations/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/generations/zodbupdate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/helper/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/helper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5819 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/helper/container.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/helper/event.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     1922 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9446 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5167 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/form.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     3318 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/admin-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-checker.pt
--rw-rw-rw-   0 root         (0) root         (0)     2663 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1834 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-group.pt
--rw-rw-rw-   0 root         (0) root         (0)     1606 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-switcher.pt
--rw-rw-rw-   0 root         (0) root         (0)     1393 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-tabform.pt
--rw-rw-rw-   0 root         (0) root         (0)     3399 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form.pt
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/inner-table-empty.pt
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/inner-table.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/search-view.pt
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/table-empty.pt
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/table-multiple.pt
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/table-switcher.pt
--rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/table.pt
--rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/interfaces/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13199 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.mo
--rw-rw-rw-   0 root         (0) root         (0)    20789 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.po
--rw-rw-rw-   0 root         (0) root         (0)    14818 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/locales/pyams_zmi.pot
--rw-rw-rw-   0 root         (0) root         (0)     4085 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/skin.py
--rw-rw-rw-   0 root         (0) root         (0)    23077 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/tests/
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1821 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1860 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     7476 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4413 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/controlpanel.py
--rw-rw-rw-   0 root         (0) root         (0)     7478 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3310 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/metas.py
--rw-rw-rw-   0 root         (0) root         (0)     3822 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     6604 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/css/
--rw-rw-rw-   0 root         (0) root         (0)   193993 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/css/swagger-ui.css
--rw-rw-rw-   0 root         (0) root         (0)   145117 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/css/swagger-ui.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)     1162 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/js/swagger-initializer.js
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/js/swagger-initializer.min.js
--rw-rw-rw-   0 root         (0) root         (0)  1061591 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/js/swagger-ui-bundle.min.js
--rw-rw-rw-   0 root         (0) root         (0)   312217 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/js/swagger-ui-standalone-preset.min.js
--rw-rw-rw-   0 root         (0) root         (0)     3528 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     5116 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/skin.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/swagger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/templates/admin-index.pt
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/templates/breadcrumbs.pt
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/templates/swagger.pt
--rw-rw-rw-   0 root         (0) root         (0)     1768 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/timezone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/aside.py
--rw-rw-rw-   0 root         (0) root         (0)     2052 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     3953 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/logo.py
--rw-rw-rw-   0 root         (0) root         (0)     4020 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/menu.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/nav.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/ribbon.py
--rw-rw-rw-   0 root         (0) root         (0)     1522 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/ajax-gear.pt
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/header.pt
--rw-rw-rw-   0 root         (0) root         (0)      332 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/hide-nav.pt
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/logo.pt
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/modal-header.pt
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/nav-divider.pt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/nav-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/nav-item.pt
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/nav-menu.pt
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/page-aside.pt
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/page-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/page-nav.pt
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/page-ribbon.pt
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/site-search.pt
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/toolbar.pt
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/top-links.pt
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/top-menu-item.pt
--rw-rw-rw-   0 root         (0) root         (0)      519 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/top-menu.pt
--rw-rw-rw-   0 root         (0) root         (0)      785 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/top-menus-group.pt
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/top-tab.pt
--rw-rw-rw-   0 root         (0) root         (0)      397 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/top-tabs.pt
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/user-links.pt
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/user-menu.pt
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/version.pt
--rw-rw-rw-   0 root         (0) root         (0)     3098 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/toolbar.py
--rw-rw-rw-   0 root         (0) root         (0)     3848 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/toplinks.py
--rw-rw-rw-   0 root         (0) root         (0)     3552 2024-05-05 20:46:38.000000 pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/userlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8335 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4542 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:47:05.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-05 20:47:11.000000 pyams_zmi-2.3.0/src/pyams_zmi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8429 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     6771 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3129 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/doctests/rest.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    11775 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/generations/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/generations/zodbupdate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/helper/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/helper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5819 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/helper/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/helper/event.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9446 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5167 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3318 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/admin-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-checker.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2663 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-group.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-switcher.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-tabform.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3399 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form.pt
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/inner-table-empty.pt
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/inner-table.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/search-view.pt
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/table-empty.pt
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/table-multiple.pt
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/table-switcher.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/table.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/interfaces/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    13199 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.mo
+-rw-rw-rw-   0 root         (0) root         (0)    20789 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.po
+-rw-rw-rw-   0 root         (0) root         (0)    14818 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/locales/pyams_zmi.pot
+-rw-rw-rw-   0 root         (0) root         (0)     4085 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1435 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/skin.py
+-rw-rw-rw-   0 root         (0) root         (0)    23381 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1860 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7476 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/controlpanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     7478 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3310 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/metas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3822 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6604 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/css/
+-rw-rw-rw-   0 root         (0) root         (0)   193993 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/css/swagger-ui.css
+-rw-rw-rw-   0 root         (0) root         (0)   145117 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/css/swagger-ui.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/js/swagger-initializer.js
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/js/swagger-initializer.min.js
+-rw-rw-rw-   0 root         (0) root         (0)  1061591 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/js/swagger-ui-bundle.min.js
+-rw-rw-rw-   0 root         (0) root         (0)   312217 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/js/swagger-ui-standalone-preset.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     5116 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/skin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/swagger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/templates/admin-index.pt
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/templates/breadcrumbs.pt
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/templates/swagger.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1768 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/timezone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/aside.py
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3953 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/logo.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/menu.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/nav.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/ribbon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/ajax-gear.pt
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      332 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/hide-nav.pt
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/logo.pt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/modal-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/nav-divider.pt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/nav-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/nav-item.pt
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/nav-menu.pt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/page-aside.pt
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/page-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/page-nav.pt
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/page-ribbon.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/site-search.pt
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/toolbar.pt
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/top-links.pt
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/top-menu-item.pt
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/top-menu.pt
+-rw-rw-rw-   0 root         (0) root         (0)      785 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/top-menus-group.pt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/top-tab.pt
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/top-tabs.pt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/user-links.pt
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/user-menu.pt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/version.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/toolbar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3848 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/toplinks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2024-05-15 16:25:10.000000 pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/userlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8429 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4542 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-15 16:25:39.000000 pyams_zmi-2.3.1/src/pyams_zmi.egg-info/top_level.txt
```

### Comparing `pyams_zmi-2.3.0/LICENSE` & `pyams_zmi-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/PKG-INFO` & `pyams_zmi-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyams_zmi
-Version: 2.3.0
+Version: 2.3.1
 Summary: PyAMS management interface package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: test
@@ -48,14 +49,18 @@
 This package is using many content providers and viewlet managers (including in forms), so it can
 be extended easily by extensions packages without having to modify existing code.
 
 
 Changelog
 =========
 
+2.3.1
+-----
+ - added column priority getter for use in responsive tables
+
 2.3.0
 -----
  - added support for custom modal content class
 
 2.2.5
 -----
  - added formatting strings constants
@@ -308,7 +313,9 @@
  - added support for IObjectData interface in tables
  - updated forms templates
  - added missing IDs in inner tabs sub-forms
 
 1.0.0
 -----
  - initial release
+
+
```

### Comparing `pyams_zmi-2.3.0/docs/HISTORY.rst` & `pyams_zmi-2.3.1/docs/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.3.1
+-----
+ - added column priority getter for use in responsive tables
+
 2.3.0
 -----
  - added support for custom modal content class
 
 2.2.5
 -----
  - added formatting strings constants
```

### Comparing `pyams_zmi-2.3.0/docs/README.rst` & `pyams_zmi-2.3.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/setup.py` & `pyams_zmi-2.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.3.0'
+version = '2.3.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_file',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/__init__.py` & `pyams_zmi-2.3.1/src/pyams_zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/configuration.py` & `pyams_zmi-2.3.1/src/pyams_zmi/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/doctests/README.rst` & `pyams_zmi-2.3.1/src/pyams_zmi/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/doctests/rest.rst` & `pyams_zmi-2.3.1/src/pyams_zmi/doctests/rest.rst`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/factory.py` & `pyams_zmi-2.3.1/src/pyams_zmi/factory.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/form.py` & `pyams_zmi-2.3.1/src/pyams_zmi/form.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/generations/__init__.py` & `pyams_zmi-2.3.1/src/pyams_zmi/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/generations/zodbupdate.py` & `pyams_zmi-2.3.1/src/pyams_zmi/generations/zodbupdate.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/helper/__init__.py` & `pyams_zmi-2.3.1/src/pyams_zmi/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/helper/container.py` & `pyams_zmi-2.3.1/src/pyams_zmi/helper/container.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/helper/event.py` & `pyams_zmi-2.3.1/src/pyams_zmi/helper/event.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/include.py` & `pyams_zmi-2.3.1/src/pyams_zmi/include.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/__init__.py` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/configuration.py` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/form.py` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/form.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/profile.py` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/table.py` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/table.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/admin-layout.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/admin-layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-checker.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-checker.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-display.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-group.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-group.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-switcher.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-switcher.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form-tabform.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form-tabform.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/form.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/form.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/inner-table-empty.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/inner-table-empty.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/inner-table.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/inner-table.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/table-empty.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/table-empty.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/table-multiple.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/table-multiple.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/table-switcher.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/table-switcher.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/templates/table.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/templates/table.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/interfaces/viewlet.py` & `pyams_zmi-2.3.1/src/pyams_zmi/interfaces/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.mo` & `pyams_zmi-2.3.1/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.mo`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.po` & `pyams_zmi-2.3.1/src/pyams_zmi/locales/fr/LC_MESSAGES/pyams_zmi.po`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/locales/pyams_zmi.pot` & `pyams_zmi-2.3.1/src/pyams_zmi/locales/pyams_zmi.pot`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/profile.py` & `pyams_zmi-2.3.1/src/pyams_zmi/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/rest.py` & `pyams_zmi-2.3.1/src/pyams_zmi/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/search.py` & `pyams_zmi-2.3.1/src/pyams_zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/skin.py` & `pyams_zmi-2.3.1/src/pyams_zmi/skin.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/table.py` & `pyams_zmi-2.3.1/src/pyams_zmi/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,19 @@
 
 
 def get_column_type(column, ignored=None):  # pylint: disable=unused-argument
     """Get column sort type attribute"""
     return getattr(column, 'sort_type', None)
 
 
+def get_column_priority(column, ignored=None):  # pylint: disable=unused-argument
+    """Get column responsive priority attribute"""
+    return getattr(column, 'responsive_priority', None)
+
+
 def get_row_id(table, element, context=None):
     """Row ID getter"""
     return f'{table.id}::{ICacheKeyValue(element)}'
 
 
 def get_row_name(table, element, view=None):
     """Element name getter"""
@@ -181,15 +186,16 @@
                     lambda row, col: 'modal' if getattr(get_row_editor(self, row),
                                                         'modal_target', None)
                     else None
             },
             'th': {
                 'data-ams-column-name': lambda row, col: self.get_row_name(row),
                 'data-ams-sortable': get_column_sort,
-                'data-ams-type': get_column_type
+                'data-ams-type': get_column_type,
+                'data-priority': get_column_priority
             }
         }
         for name, adapter in self.request.registry.getAdapters((self.context, self.request, self),
                                                                ITableAttributes):
             adapter.update_attributes(result)
         return result
 
@@ -432,14 +438,15 @@
 
 
 class NameColumn(I18nColumnMixin, GetAttrColumn):
     """Common name column"""
 
     i18n_header = _("Name")
     weight = 10
+    responsive_priority = 10
 
     def get_value(self, obj):
         return get_object_label(obj, self.request, self.table)
 
 
 class IconColumn(Column):
     """Base icon column"""
@@ -694,14 +701,15 @@
     """Table actions column"""
 
     i18n_header = _("Actions")
     css_classes = {
         'th': 'action'
     }
     weight = 900
+    responsive_priority = 900
 
     def render_cell(self, item):
         """Cell renderer"""
         registry = self.request.registry
         viewlet = registry.queryMultiAdapter((item, self.request, self.table),
                                              IViewletManager,
                                              name='pyams.table_actions')
```

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/tests/__init__.py` & `pyams_zmi-2.3.1/src/pyams_zmi/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/tests/test_utilsdocs.py` & `pyams_zmi-2.3.1/src/pyams_zmi/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/tests/test_utilsdocstrings.py` & `pyams_zmi-2.3.1/src/pyams_zmi/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/utils.py` & `pyams_zmi-2.3.1/src/pyams_zmi/utils.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/view.py` & `pyams_zmi-2.3.1/src/pyams_zmi/view.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/__init__.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/breadcrumb.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/configuration.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/controlpanel.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/controlpanel.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/environment.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/environment.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/interfaces.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/metas.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/metas.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/profile.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/registry.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/registry.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/css/swagger-ui.css` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/css/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/css/swagger-ui.min.css` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/css/swagger-ui.min.css`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/js/swagger-initializer.js` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/js/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/js/swagger-ui-bundle.min.js` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/js/swagger-ui-bundle.min.js`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources/js/swagger-ui-standalone-preset.min.js` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources/js/swagger-ui-standalone-preset.min.js`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/resources.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/resources.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/skin.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/skin.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/swagger.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/swagger.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/timezone.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/timezone.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/__init__.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/aside.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/aside.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/breadcrumb.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/header.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/header.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/logo.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/logo.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/menu.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/menu.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/nav.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/nav.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/ribbon.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/ribbon.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/search.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/search.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/nav-item.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/nav-item.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/page-nav.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/page-nav.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/site-search.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/site-search.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/top-menu.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/top-menu.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/templates/top-menus-group.pt` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/templates/top-menus-group.pt`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/toolbar.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/toplinks.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/toplinks.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi/zmi/viewlet/userlinks.py` & `pyams_zmi-2.3.1/src/pyams_zmi/zmi/viewlet/userlinks.py`

 * *Files identical despite different names*

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi.egg-info/PKG-INFO` & `pyams_zmi-2.3.1/src/pyams_zmi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyams-zmi
-Version: 2.3.0
+Version: 2.3.1
 Summary: PyAMS management interface package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: test
@@ -48,14 +49,18 @@
 This package is using many content providers and viewlet managers (including in forms), so it can
 be extended easily by extensions packages without having to modify existing code.
 
 
 Changelog
 =========
 
+2.3.1
+-----
+ - added column priority getter for use in responsive tables
+
 2.3.0
 -----
  - added support for custom modal content class
 
 2.2.5
 -----
  - added formatting strings constants
@@ -308,7 +313,9 @@
  - added support for IObjectData interface in tables
  - updated forms templates
  - added missing IDs in inner tabs sub-forms
 
 1.0.0
 -----
  - initial release
+
+
```

### Comparing `pyams_zmi-2.3.0/src/pyams_zmi.egg-info/SOURCES.txt` & `pyams_zmi-2.3.1/src/pyams_zmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

