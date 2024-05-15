# Comparing `tmp/pyams_app_msc-1.99.3.tar.gz` & `tmp/pyams_app_msc-1.99.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_app_msc-1.99.3.tar", last modified: Sun May  5 21:12:40 2024, max compression
+gzip compressed data, was "dist/pyams_app_msc-1.99.4.tar", last modified: Wed May 15 16:59:16 2024, max compression
```

## Comparing `pyams_app_msc-1.99.3.tar` & `pyams_app_msc-1.99.4.tar`

### file list

```diff
@@ -1,393 +1,395 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3973 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/docs/
--rwxrwxrwx   0 root         (0) root         (0)     2436 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/booking.puml
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/classes.puml
--rw-rw-rw-   0 root         (0) root         (0)    16507 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/docs/es-mapping.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/assets/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/clock.png
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/email.png
--rw-rw-rw-   0 root         (0) root         (0)   207972 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-brands-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)   117372 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-brands-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)    68004 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-regular-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)    25452 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-regular-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)   419720 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-solid-900.ttf
--rw-rw-rw-   0 root         (0) root         (0)   156496 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-solid-900.woff2
--rw-rw-rw-   0 root         (0) root         (0)    10832 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-v4compatibility.ttf
--rw-rw-rw-   0 root         (0) root         (0)     4792 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/fa-v4compatibility.woff2
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/form.png
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/layers-2x.png
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/layers.png
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/marker-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/phone.png
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/select2-spinner.gif
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/select2.png
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/select2x2.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/assets/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/css/dev/
--rw-rw-rw-   0 root         (0) root         (0)   263831 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/dev/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/css/dist/
--rw-rw-rw-   0 root         (0) root         (0)   337917 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/dist/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/css/img/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/clock.png
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/download.svg
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/email.png
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/form.png
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/link.svg
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/phone.png
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/print.svg
--rw-rw-rw-   0 root         (0) root         (0)     4315 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/search.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/css/img/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/js/dev/
--rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/mscapp.js.map
--rw-rw-rw-   0 root         (0) root         (0)     4652 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    10624 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)     6409 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    19333 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
--rw-rw-rw-   0 root         (0) root         (0)    29675 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   209738 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
--rw-rw-rw-   0 root         (0) root         (0)   236865 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   182041 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
--rw-rw-rw-   0 root         (0) root         (0)   230602 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
--rw-rw-rw-   0 root         (0) root         (0)   181575 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
--rw-rw-rw-   0 root         (0) root         (0)   230045 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
--rw-rw-rw-   0 root         (0) root         (0)   174144 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
--rw-rw-rw-   0 root         (0) root         (0)   220941 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
--rw-rw-rw-   0 root         (0) root         (0)    21983 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)    18395 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    18911 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
--rw-rw-rw-   0 root         (0) root         (0)    20127 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   450498 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
--rw-rw-rw-   0 root         (0) root         (0)   569896 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    46418 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
--rw-rw-rw-   0 root         (0) root         (0)    53162 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)   153997 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
--rw-rw-rw-   0 root         (0) root         (0)   189149 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   114212 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
--rw-rw-rw-   0 root         (0) root         (0)   139871 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/pkg/js/dist/
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/116.js
--rw-rw-rw-   0 root         (0) root         (0)     8340 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/137.js
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/178.js
--rw-rw-rw-   0 root         (0) root         (0)    67548 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/23.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/23.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/243.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/243.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16009 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/274.js
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/284.js
--rw-rw-rw-   0 root         (0) root         (0)    69465 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/458.js
--rw-rw-rw-   0 root         (0) root         (0)     3219 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/47.js
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/481.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/481.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/528.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/528.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70026 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/612.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/612.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16008 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/623.js
--rw-rw-rw-   0 root         (0) root         (0)    61493 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/624.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/624.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   105878 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/660.js
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/660.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/671.js
--rw-rw-rw-   0 root         (0) root         (0)    69464 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/686.js
--rw-rw-rw-   0 root         (0) root         (0)    61491 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/698.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/698.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/814.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/814.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/830.js
--rw-rw-rw-   0 root         (0) root         (0)     1859 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/854.js
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/860.js
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/882.js
--rw-rw-rw-   0 root         (0) root         (0)   937336 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/pkg/js/dist/mscapp.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3899 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5092 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1500 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt
--rw-rw-rw-   0 root         (0) root         (0)      968 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/
--rw-rw-rw-   0 root         (0) root         (0)    12350 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/container.py
--rw-rw-rw-   0 root         (0) root         (0)     9708 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4366 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/reminder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6130 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     3861 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    36247 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15562 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/home.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/reminder.py
--rw-rw-rw-   0 root         (0) root         (0)     8133 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3155 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
--rw-rw-rw-   0 root         (0) root         (0)    38087 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/
--rw-rw-rw-   0 root         (0) root         (0)     1816 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/
--rw-rw-rw-   0 root         (0) root         (0)     2173 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3464 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/
--rw-rw-rw-   0 root         (0) root         (0)     3511 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5672 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    12100 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8538 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16194 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2395 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/
--rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7142 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/password.py
--rw-rw-rw-   0 root         (0) root         (0)    11384 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     6337 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12105 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/
--rw-rw-rw-   0 root         (0) root         (0)    20787 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   167336 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)   167000 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
--rw-rw-rw-   0 root         (0) root         (0)   168644 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/
--rw-rw-rw-   0 root         (0) root         (0)    17688 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4826 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/generations/
--rw-rw-rw-   0 root         (0) root         (0)     3771 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8674 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/include.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    63416 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
--rw-rw-rw-   0 root         (0) root         (0)   109342 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
--rw-rw-rw-   0 root         (0) root         (0)    77437 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/locales/pyams_app_msc.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5752 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3216 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2257 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/root/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/api/
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1862 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2381 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4485 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3434 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     2050 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3704 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     6790 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8974 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6079 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/
--rw-rw-rw-   0 root         (0) root         (0)     8410 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4330 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/audience.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    12262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/audience.py
--rw-rw-rw-   0 root         (0) root         (0)     4080 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/price.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/room.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/page.py
--rw-rw-rw-   0 root         (0) root         (0)     4262 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/price.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/room.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/session.py
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12486 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9666 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/audience.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5472 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/planning.py
--rw-rw-rw-   0 root         (0) root         (0)     3108 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/presentation.py
--rw-rw-rw-   0 root         (0) root         (0)     9318 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)     9175 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/room.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4526 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/types.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/form.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     5255 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/
--rw-rw-rw-   0 root         (0) root         (0)    11860 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_form.js
--rw-rw-rw-   0 root         (0) root         (0)     5731 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_gis.js
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_i18n.js
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_search.js
--rw-rw-rw-   0 root         (0) root         (0)     9714 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4237 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/mscapp.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_content.scss
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_list.scss
--rw-rw-rw-   0 root         (0) root         (0)     4416 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_search.scss
--rw-rw-rw-   0 root         (0) root         (0)     4329 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/msc.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/skin/templates/select-admin-theater.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/img/
--rw-rw-rw-   0 root         (0) root         (0)     4680 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/img/pass-culture.webp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    24830 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/msc.js
--rw-rw-rw-   0 root         (0) root         (0)    10063 2024-05-05 21:11:57.000000 pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/msc.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3973 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13539 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:12:29.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      698 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-05 21:12:40.000000 pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4406 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     2869 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/docs/booking.puml
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/docs/classes.puml
+-rw-rw-rw-   0 root         (0) root         (0)    16507 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/docs/es-mapping.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/email.png
+-rw-rw-rw-   0 root         (0) root         (0)   207972 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/fa-brands-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   117372 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/fa-brands-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    68004 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/fa-regular-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    25452 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/fa-regular-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   419720 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/fa-solid-900.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   156496 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/fa-solid-900.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    10832 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/fa-v4compatibility.ttf
+-rw-rw-rw-   0 root         (0) root         (0)     4792 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/fa-v4compatibility.woff2
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/form.png
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/layers-2x.png
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/layers.png
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/marker-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/select2-spinner.gif
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/select2.png
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/select2x2.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/assets/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/css/dev/
+-rw-rw-rw-   0 root         (0) root         (0)   263831 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/dev/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/css/dist/
+-rw-rw-rw-   0 root         (0) root         (0)   337917 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/dist/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/css/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/download.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/email.png
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/form.png
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/link.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/print.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/search.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/css/img/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/js/dev/
+-rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/mscapp.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     4652 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    10624 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    19333 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    29675 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   209738 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   236865 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   182041 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
+-rw-rw-rw-   0 root         (0) root         (0)   230602 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   181575 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
+-rw-rw-rw-   0 root         (0) root         (0)   230045 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   174144 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
+-rw-rw-rw-   0 root         (0) root         (0)   220941 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    21983 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    18395 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    18911 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   450498 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   569896 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    46418 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    53162 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   153997 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   189149 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   114212 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   139871 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/pkg/js/dist/
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/116.js
+-rw-rw-rw-   0 root         (0) root         (0)     8340 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/137.js
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/178.js
+-rw-rw-rw-   0 root         (0) root         (0)    67548 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/23.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/23.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/243.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/243.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16009 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/274.js
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/284.js
+-rw-rw-rw-   0 root         (0) root         (0)    69465 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/458.js
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/47.js
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/481.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/481.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/528.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/528.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70026 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/612.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/612.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16008 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/623.js
+-rw-rw-rw-   0 root         (0) root         (0)    61493 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/624.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/624.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   105878 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/660.js
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/660.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/671.js
+-rw-rw-rw-   0 root         (0) root         (0)    69464 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/686.js
+-rw-rw-rw-   0 root         (0) root         (0)    61491 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/698.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/698.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/814.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/814.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/830.js
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/854.js
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/860.js
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/882.js
+-rw-rw-rw-   0 root         (0) root         (0)   937336 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/pkg/js/dist/mscapp.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3908 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/address/
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/address/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/address/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/address/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/address/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/admininfo/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/admininfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/admininfo/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/admininfo/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/admininfo/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/banking/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/banking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/banking/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/banking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/banking/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/contact/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/contact/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/contact/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/contact/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt
+-rw-rw-rw-   0 root         (0) root         (0)      968 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/paragraph/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/paragraph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/paragraph/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/paragraph/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/component/paragraph/zmi/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/
+-rw-rw-rw-   0 root         (0) root         (0)    10607 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/container.py
+-rw-rw-rw-   0 root         (0) root         (0)    11980 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     4366 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/reminder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    39632 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15590 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/home.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/reminder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8133 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3155 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
+-rw-rw-rw-   0 root         (0) root         (0)    34793 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/messaging/
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/messaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/messaging/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/messaging/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/messaging/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/oauth/
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/oauth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/oauth/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3464 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/oauth/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/
+-rw-rw-rw-   0 root         (0) root         (0)     3511 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    12108 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8168 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16194 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/zmi/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7142 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/password.py
+-rw-rw-rw-   0 root         (0) root         (0)    11384 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6337 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12271 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/
+-rw-rw-rw-   0 root         (0) root         (0)    21215 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   167336 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   167000 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   168644 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/
+-rw-rw-rw-   0 root         (0) root         (0)    17688 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4826 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8674 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    64836 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
+-rw-rw-rw-   0 root         (0) root         (0)   111551 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
+-rw-rw-rw-   0 root         (0) root         (0)    78802 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/locales/pyams_app_msc.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/reference/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/root/
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/root/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     6790 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8974 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6079 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/common/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/site/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/site/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/
+-rw-rw-rw-   0 root         (0) root         (0)     8410 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4330 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/audience.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    13256 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)     4080 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/room.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     5620 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12558 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9666 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5472 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/planning.py
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/presentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9318 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9175 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5255 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)    11860 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_form.js
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_gis.js
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_i18n.js
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_search.js
+-rw-rw-rw-   0 root         (0) root         (0)     9714 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/mscapp.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_content.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_list.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_search.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/msc.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/skin/templates/select-admin-theater.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/img/
+-rw-rw-rw-   0 root         (0) root         (0)     4680 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/img/pass-culture.webp
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    25533 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/js/msc.js
+-rw-rw-rw-   0 root         (0) root         (0)    10403 2024-05-15 16:58:24.000000 pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/js/msc.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4406 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13638 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:59:05.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      705 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-15 16:59:16.000000 pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/top_level.txt
```

### Comparing `pyams_app_msc-1.99.3/LICENSE` & `pyams_app_msc-1.99.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/PKG-INFO` & `pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_app_msc
-Version: 1.99.3
+Name: pyams-app-msc
+Version: 1.99.4
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -44,14 +44,24 @@
 PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.4
+------
+ - issue #27: added theater setting to set first week day displayed in calendars
+ - issue #30: updated actions used to update content illustrations from medias gallery
+ - issue #31: added free accompanists count in booking data
+ - issue #32: allow direct booking validation from creation form
+ - updated event title getter
+ - updated user profile edit form
+ - added column priority getter for use in responsive tables
+
 1.99.3
 ------
  - issue #21: added display of principal phone number
  - issue #22: updated shared content header viewlet to add button to go back to dashboard
  - issue #25: updated prompt of activity selection widget
  - issue #26: added support for vertical synchronization of calendars
  - issue #27: removed theater week view from calendar
```

### Comparing `pyams_app_msc-1.99.3/docs/HISTORY.rst` & `pyams_app_msc-1.99.4/docs/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+1.99.4
+------
+ - issue #27: added theater setting to set first week day displayed in calendars
+ - issue #30: updated actions used to update content illustrations from medias gallery
+ - issue #31: added free accompanists count in booking data
+ - issue #32: allow direct booking validation from creation form
+ - updated event title getter
+ - updated user profile edit form
+ - added column priority getter for use in responsive tables
+
 1.99.3
 ------
  - issue #21: added display of principal phone number
  - issue #22: updated shared content header viewlet to add button to go back to dashboard
  - issue #25: updated prompt of activity selection widget
  - issue #26: added support for vertical synchronization of calendars
  - issue #27: removed theater week view from calendar
```

### Comparing `pyams_app_msc-1.99.3/docs/README.rst` & `pyams_app_msc-1.99.4/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/docs/classes.puml` & `pyams_app_msc-1.99.4/docs/classes.puml`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/docs/es-mapping.json` & `pyams_app_msc-1.99.4/docs/es-mapping.json`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/clock.png` & `pyams_app_msc-1.99.4/pkg/assets/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/email.png` & `pyams_app_msc-1.99.4/pkg/assets/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/fa-brands-400.ttf` & `pyams_app_msc-1.99.4/pkg/assets/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/fa-brands-400.woff2` & `pyams_app_msc-1.99.4/pkg/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/fa-regular-400.ttf` & `pyams_app_msc-1.99.4/pkg/assets/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/fa-regular-400.woff2` & `pyams_app_msc-1.99.4/pkg/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/fa-solid-900.ttf` & `pyams_app_msc-1.99.4/pkg/assets/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/fa-solid-900.woff2` & `pyams_app_msc-1.99.4/pkg/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/fa-v4compatibility.ttf` & `pyams_app_msc-1.99.4/pkg/assets/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/fa-v4compatibility.woff2` & `pyams_app_msc-1.99.4/pkg/assets/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/form.png` & `pyams_app_msc-1.99.4/pkg/assets/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/layers-2x.png` & `pyams_app_msc-1.99.4/pkg/assets/layers-2x.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/layers.png` & `pyams_app_msc-1.99.4/pkg/assets/layers.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/list-item.png` & `pyams_app_msc-1.99.4/pkg/assets/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/map.png` & `pyams_app_msc-1.99.4/pkg/assets/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/marker-icon.png` & `pyams_app_msc-1.99.4/pkg/assets/marker-icon.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/mobile-menu.png` & `pyams_app_msc-1.99.4/pkg/assets/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/phone.png` & `pyams_app_msc-1.99.4/pkg/assets/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/select2-spinner.gif` & `pyams_app_msc-1.99.4/pkg/assets/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/select2.png` & `pyams_app_msc-1.99.4/pkg/assets/select2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/select2x2.png` & `pyams_app_msc-1.99.4/pkg/assets/select2x2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/assets/social-icons.png` & `pyams_app_msc-1.99.4/pkg/assets/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/dev/msc.css` & `pyams_app_msc-1.99.4/pkg/css/dev/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/dist/msc.css` & `pyams_app_msc-1.99.4/pkg/css/dist/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/clock.png` & `pyams_app_msc-1.99.4/pkg/css/img/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/download.svg` & `pyams_app_msc-1.99.4/pkg/css/img/download.svg`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/email.png` & `pyams_app_msc-1.99.4/pkg/css/img/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/form.png` & `pyams_app_msc-1.99.4/pkg/css/img/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/list-item.png` & `pyams_app_msc-1.99.4/pkg/css/img/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/map.png` & `pyams_app_msc-1.99.4/pkg/css/img/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/mobile-menu.png` & `pyams_app_msc-1.99.4/pkg/css/img/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/phone.png` & `pyams_app_msc-1.99.4/pkg/css/img/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/search.png` & `pyams_app_msc-1.99.4/pkg/css/img/search.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/css/img/social-icons.png` & `pyams_app_msc-1.99.4/pkg/css/img/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/mscapp.js` & `pyams_app_msc-1.99.4/pkg/js/dev/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/mscapp.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/mscapp.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js` & `pyams_app_msc-1.99.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js` & `pyams_app_msc-1.99.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js` & `pyams_app_msc-1.99.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map` & `pyams_app_msc-1.99.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/116.js` & `pyams_app_msc-1.99.4/pkg/js/dist/116.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/137.js` & `pyams_app_msc-1.99.4/pkg/js/dist/137.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/23.js` & `pyams_app_msc-1.99.4/pkg/js/dist/23.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/23.js.LICENSE.txt` & `pyams_app_msc-1.99.4/pkg/js/dist/23.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/243.js` & `pyams_app_msc-1.99.4/pkg/js/dist/243.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/274.js` & `pyams_app_msc-1.99.4/pkg/js/dist/274.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/284.js` & `pyams_app_msc-1.99.4/pkg/js/dist/284.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/458.js` & `pyams_app_msc-1.99.4/pkg/js/dist/458.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/47.js` & `pyams_app_msc-1.99.4/pkg/js/dist/47.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/481.js` & `pyams_app_msc-1.99.4/pkg/js/dist/481.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/528.js` & `pyams_app_msc-1.99.4/pkg/js/dist/528.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/528.js.LICENSE.txt` & `pyams_app_msc-1.99.4/pkg/js/dist/528.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/612.js` & `pyams_app_msc-1.99.4/pkg/js/dist/612.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/612.js.LICENSE.txt` & `pyams_app_msc-1.99.4/pkg/js/dist/612.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/623.js` & `pyams_app_msc-1.99.4/pkg/js/dist/623.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/624.js` & `pyams_app_msc-1.99.4/pkg/js/dist/624.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/660.js` & `pyams_app_msc-1.99.4/pkg/js/dist/660.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/686.js` & `pyams_app_msc-1.99.4/pkg/js/dist/686.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/698.js` & `pyams_app_msc-1.99.4/pkg/js/dist/698.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/814.js` & `pyams_app_msc-1.99.4/pkg/js/dist/814.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/814.js.LICENSE.txt` & `pyams_app_msc-1.99.4/pkg/js/dist/814.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/830.js` & `pyams_app_msc-1.99.4/pkg/js/dist/830.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/854.js` & `pyams_app_msc-1.99.4/pkg/js/dist/854.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/860.js` & `pyams_app_msc-1.99.4/pkg/js/dist/860.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/882.js` & `pyams_app_msc-1.99.4/pkg/js/dist/882.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/mscapp.js` & `pyams_app_msc-1.99.4/pkg/js/dist/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/pkg/js/dist/mscapp.js.LICENSE.txt` & `pyams_app_msc-1.99.4/pkg/js/dist/mscapp.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/setup.py` & `pyams_app_msc-1.99.4/setup.py`

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
 
 data_dir = 'pkg'
 data_files = [(d, [os.path.join(d, f) for f in files])
               for d, folders, files in os.walk(data_dir)]
 
 tests_require = [
@@ -97,15 +97,15 @@
           'pyams_sequence',
           'pyams_site',
           'pyams_skin',
           'pyams_table',
           'pyams_utils >= 2.3.1',
           'pyams_viewlet',
           'pyams_workflow',
-          'pyams_zmi',
+          'pyams_zmi >= 2.3.1',
           'pyams_zmq',
           'pyramid',
           'pyramid_mailer',
           'reportlab',
           'requests',
           'transaction',
           'ZODB',
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/address/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/address/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/address/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/address/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/admininfo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/admininfo/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/admininfo/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/admininfo/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/banking/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/banking/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/banking/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/banking/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/contact/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/contact/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/contact/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/schema.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/duration/zmi/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/duration/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,71 +15,98 @@
 """
 
 from pyramid.httpexceptions import HTTPForbidden, HTTPInternalServerError
 from pyramid.view import view_config
 from zope.copy import copy
 from zope.interface import Interface
 
+from pyams_app_msc.component.gallery.zmi.interfaces import IGalleryIllustrationActionsMenu
 from pyams_app_msc.zmi import msc
 from pyams_content.component.gallery import IGalleryContainer, IGalleryFile
 from pyams_content.component.gallery.zmi import GalleryMediasViewlet, GalleryView
-from pyams_content.component.illustration import IIllustration
+from pyams_content.component.illustration import IIllustration, ILinkIllustration
 from pyams_content.interfaces import MANAGE_CONTENT_PERMISSION
 from pyams_content.shared.common import IWfSharedContent
 from pyams_i18n.interfaces import INegotiator
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.permission import get_edit_permission
 from pyams_skin.interfaces.viewlet import IContextActionsViewletManager
-from pyams_skin.viewlet.actions import ContextAction
+from pyams_skin.viewlet.actions import ContextAction, ContextActionsMenu
+from pyams_skin.viewlet.menu import MenuItem
 from pyams_template.template import override_template
 from pyams_utils.registry import get_utility
 from pyams_utils.traversing import get_parent
+from pyams_viewlet.manager import viewletmanager_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.interfaces import IAdminLayer
 
 __docformat__ = 'restructuredtext'
 
 from pyams_app_msc import _
 
 
-@viewlet_config(name='set-content-illustration.action',
-                context=IGalleryFile, layer=IAdminLayer, view=Interface,
-                manager=IContextActionsViewletManager, weight=30,
-                permission=MANAGE_CONTENT_PERMISSION)
-class GalleryFileIllustrationGetter(ContextAction):
-    """Gallery file illustration getter"""
+@viewletmanager_config(name='set-content-illustration.menu',
+                       context=IGalleryFile, layer=IAdminLayer, view=Interface,
+                       manager=IContextActionsViewletManager, weight=100,
+                       provides=IGalleryIllustrationActionsMenu,
+                       permission=MANAGE_CONTENT_PERMISSION)
+class GalleryFileIllustrationsGetter(ContextActionsMenu):
+    """Gallery file illustrations getter"""
 
     def __new__(cls, context, request, view, manager):
         gallery = get_parent(context, IGalleryContainer)
         if gallery is not None:
             edit_permission = get_edit_permission(request, context=gallery, view=view)
             if not request.has_permission(edit_permission, context=context):
                 return None
-        return ContextAction.__new__(cls)
+        return ContextActionsMenu.__new__(cls)
 
-    hint = _("Set as content illustration")
+    # hint = _("Set content illustration")
     css_class = 'btn-sm px-1'
     icon_class = 'fas fa-file-image'
 
+    def update(self):
+        super().update()
+        msc.need()
+
+
+@viewlet_config(name='content-illustration.action',
+                context=IGalleryFile, layer=IAdminLayer, view=Interface,
+                manager=IGalleryIllustrationActionsMenu, weight=10,
+                permission=MANAGE_CONTENT_PERMISSION)
+class ContentIllustrationSetter(MenuItem):
+    """Content illustration setter"""
+
+    label = _("Set content illustration")
+
     def get_href(self):
         """Icon URL getter"""
         return None
 
-    click_handler = 'MyAMS.msc.catalog.setIllustrationFromGallery'
+    click_handler = 'MyAMS.msc.catalog.setContentIllustrationFromGallery'
 
-    def update(self):
-        super().update()
-        msc.need()
 
+@viewlet_config(name='link-illustration.action',
+                context=IGalleryFile, layer=IAdminLayer, view=Interface,
+                manager=IGalleryIllustrationActionsMenu, weight=10,
+                permission=MANAGE_CONTENT_PERMISSION)
+class LinkIllustrationSetter(MenuItem):
+    """Link illustration setter"""
 
-@view_config(name='set-content-illustration.json',
-             context=IGalleryContainer, request_type=IPyAMSLayer,
-             renderer='json', xhr=True)
-def set_content_illustration(request):
-    """Set content illustration from medias gallery file"""
+    label = _("Set navigation illustration")
+
+    def get_href(self):
+        """Icon URL getter"""
+        return None
+
+    click_handler = 'MyAMS.msc.catalog.setLinkIllustrationFromGallery'
+
+
+def set_illustration(request, illustration_interface):
+    """Set content illustration"""
     translate = request.localizer.translate
     name = request.params.get('object_name')
     if not name:
         return {
             'status': 'message',
             'messagebox': {
                 'status': 'error',
@@ -105,15 +132,15 @@
             }
         }
     permission = get_edit_permission(request, content)
     if permission is None:
         raise HTTPInternalServerError("Missing permission definition!")
     if not request.has_permission(permission, context=content):
         raise HTTPForbidden()
-    illustration = IIllustration(content, None)
+    illustration = illustration_interface(content, None)
     if illustration is None:
         return {
             'status': 'message',
             'messagebox': {
                 'status': 'error',
                 'message': translate(_("No illustration on content!"))
             }
@@ -125,18 +152,34 @@
     illustration.description = media.description
     illustration.author = media.author
     illustration.data = {
         negotiator.server_language: copy(media.data)
     }
     return {
         'status': 'success',
-        'message': translate(_("Content illustration has been updated successfully."))
+        'message': translate(_("Illustration has been updated successfully."))
     }
 
 
+@view_config(name='set-content-illustration.json',
+             context=IGalleryContainer, request_type=IPyAMSLayer,
+             renderer='json', xhr=True)
+def set_content_illustration(request):
+    """Set content illustration from medias gallery file"""
+    return set_illustration(request, IIllustration)
+
+
+@view_config(name='set-link-illustration.json',
+             context=IGalleryContainer, request_type=IPyAMSLayer,
+             renderer='json', xhr=True)
+def set_link_illustration(request):
+    """Set link illustration from medias gallery file"""
+    return set_illustration(request, ILinkIllustration)
+
+
 override_template(GalleryMediasViewlet,
                   template='templates/gallery-medias.pt',
                   layer=IAdminLayer)
 
 override_template(GalleryView,
                   template='templates/gallery-view.pt',
                   layer=IAdminLayer)
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/paragraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/paragraph/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/component/paragraph/zmi/container.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/component/paragraph/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/doctests/README.rst` & `pyams_app_msc-1.99.4/src/pyams_app_msc/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,103 +15,63 @@
 """
 
 from datetime import datetime, timedelta
 
 from persistent import Persistent
 from pyramid.events import subscriber
 from zope.container.contained import Contained
-from zope.dublincore.interfaces import IZopeDublinCore
 from zope.interface import implementer
 from zope.lifecycleevent import ObjectModifiedEvent
 from zope.lifecycleevent.interfaces import IObjectModifiedEvent
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_app_msc.feature.booking.interfaces import BOOKING_STATUS, IBookingContainer, IBookingInfo, IBookingTarget
 from pyams_app_msc.feature.booking.reminder import BookingReminderTask
 from pyams_app_msc.feature.messaging.interfaces import IMessagingSettings
 from pyams_app_msc.feature.planning.interfaces import IPlanning, ISession
 from pyams_app_msc.feature.profile.interfaces import IUserProfile
 from pyams_app_msc.feature.quotation import Quotation
 from pyams_app_msc.interfaces import MANAGE_BOOKING_PERMISSION
-from pyams_app_msc.shared.catalog.interfaces import ICatalogEntry
 from pyams_app_msc.shared.theater.interfaces import IMovieTheater, IMovieTheaterSettings
 from pyams_app_msc.shared.theater.interfaces.price import ICinemaPriceContainer
 from pyams_catalog.utils import index_object
 from pyams_content.feature.history.interfaces import IHistoryTarget
 from pyams_content.interfaces import IObjectType
-from pyams_file.interfaces.thumbnail import IThumbnails
 from pyams_file.property import FileProperty
-from pyams_i18n.interfaces import II18n
 from pyams_mail.interfaces import IPrincipalMailInfo
 from pyams_mail.message import HTMLMessage
 from pyams_scheduler.interfaces import IScheduler
 from pyams_scheduler.interfaces.task import IDateTaskScheduling, SCHEDULER_TASK_DATE_MODE
 from pyams_security.interfaces import ISecurityManager, IViewContextPermissionChecker
 from pyams_security.interfaces.base import FORBIDDEN_PERMISSION
 from pyams_security.security import ProtectedObjectMixin
 from pyams_security.utility import get_principal
 from pyams_site.interfaces import ISiteRoot
 from pyams_utils.adapter import ContextAdapter, adapter_config
-from pyams_utils.date import format_date, format_datetime
 from pyams_utils.factory import factory_config, get_interface_base_name
 from pyams_utils.interfaces import ICacheKeyValue
 from pyams_utils.registry import get_pyramid_registry, get_utility, query_utility
 from pyams_utils.timezone import tztime
 from pyams_utils.traversing import get_parent
-from pyams_utils.url import absolute_url
 from pyams_utils.zodb import load_object, volatile_property
-from pyams_workflow.interfaces import IWorkflowVersions
-from pyams_zmi.utils import get_object_label
 
 __docformat__ = 'restructuredtext'
 
 
-def get_booking_message_values(context, request, view):
-    """Get booking message values"""
-    theater = get_parent(context, IMovieTheater)
-    # generate templates values
-    session = ISession(context)
-    entry = get_parent(session, ICatalogEntry)
-    if entry is not None:
-        versions = IWorkflowVersions(entry, None)
-        if versions is not None:
-            entry = versions.get_version(-1)
-    values = {
-        'theater_name': II18n(theater).query_attribute('title', request=request),
-        'theater_email': theater.contact_email or '',
-        'theater_phone': theater.phone_number or '',
-        'theater_logo': '',
-        'sender_name': request.principal.title,
-        'sender_email': '',
-        'booking_date': format_date(IZopeDublinCore(session).created),
-        'session': get_object_label(session, request, view, name='short-text'),
-        'session_title': get_object_label(entry, request, view),
-        'session_date': format_datetime(session.start_date)
-    }
-    logo = theater.logo
-    if logo:
-        thumbnail = IThumbnails(logo).get_thumbnail('h160')
-        values['theater_logo'] = (f'<img src="{absolute_url(thumbnail, request)}"'
-                                  f' alt="Logo" />')
-    mail_info = IPrincipalMailInfo(request.principal, None)
-    if mail_info is not None:
-        values['sender_email'] = next(mail_info.get_addresses())
-    return values
-
-
 @factory_config(IBookingInfo)
 @implementer(IHistoryTarget)
 class BookingInfo(ProtectedObjectMixin, Persistent, Contained):
     """Booking information"""
 
     creator = FieldProperty(IBookingInfo['creator'])
     recipient = FieldProperty(IBookingInfo['recipient'])
     status = FieldProperty(IBookingInfo['status'])
     nb_participants = FieldProperty(IBookingInfo['nb_participants'])
     nb_accompanists = FieldProperty(IBookingInfo['nb_accompanists'])
+    nb_free_accompanists = FieldProperty(IBookingInfo['nb_free_accompanists'])
     nb_groups = FieldProperty(IBookingInfo['nb_groups'])
     price = FieldProperty(IBookingInfo['price'])
     accompanying_ratio = FieldProperty(IBookingInfo['accompanying_ratio'])
     cultural_pass = FieldProperty(IBookingInfo['cultural_pass'])
     comments = FieldProperty(IBookingInfo['comments'])
     notepad = FieldProperty(IBookingInfo['notepad'])
     archived = FieldProperty(IBookingInfo['archived'])
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/container.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/container.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from collections import OrderedDict
 from enum import Enum
 
 from zope.annotation.interfaces import IAttributeAnnotatable
 from zope.container.constraints import contains
 from zope.container.interfaces import IContainer
-from zope.interface import Attribute
+from zope.interface import Attribute, Invalid, invariant
 from zope.schema import Bool, Choice, Datetime, Int, Text, TextLine
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_app_msc.shared.theater.interfaces.price import PRICES_VOCABULARY
 from pyams_file.schema import FileField
 from pyams_scheduler.interfaces import ITask
 from pyams_security.schema import PrincipalField
@@ -124,18 +124,29 @@
 
     nb_participants = Int(title=_("Participants"),
                           description=_("Number of participants seats reserved for this session"),
                           required=True,
                           min=0)
 
     nb_accompanists = Int(title=_("Accompanists"),
-                          description=_("Number of accompanists seats reserved for this session"),
+                          description=_("Total number of accompanists seats reserved for this session"),
                           required=True,
                           min=0)
-
+    
+    nb_free_accompanists = Int(title=_("Free accompanists"),
+                               description=_("Number of free accompanists seats reserved for this session"),
+                               required=True,
+                               min=0,
+                               default=0)
+    
+    @invariant
+    def check_nb_accompanists(self):
+        if self.nb_free_accompanists > self.nb_accompanists:
+            raise Invalid(_("Number of free accompanists can't be higher than total number of accompanists!"))
+        
     nb_groups = Int(title=_("Groups count"),
                     description=_("Number of groups or classrooms attending this session"),
                     required=True,
                     min=1,
                     default=1)
 
     price = Choice(title=_("Price"),
@@ -231,14 +242,60 @@
                              description=_("Date and time at which reminder message was sent"),
                              required=False)
 
     def send_reminder_message(self):
         """Send reminder message"""
 
 
+class IBookingAcceptInfo(IBookingInfo):
+    """Booking accept info interface"""
+
+    accepted = Bool(title=_("Accept booking"),
+                    required=True,
+                    default=False)
+
+
+class IBaseBookingWorkflowInfo(IBookingInfo):
+    """Base booking workflow info interface"""
+
+    created = Datetime(title=_("Creation date"),
+                       description=_("Date at which the booking was created"),
+                       required=False)
+
+    notify_recipient = Bool(title=_("Notify recipient?"),
+                            description=_("If 'yes', a notification message will be sent to the recipient"),
+                            required=False,
+                            default=True)
+
+    notify_subject = TextLine(title=_("Notification subject"),
+                              description=_("Subject of notification message sent to the recipient"),
+                              required=False)
+
+    notify_message = HTMLField(title=_("Notification message"),
+                               description=_("Notification message sent to the recipient"),
+                               required=False)
+
+
+class IAcceptedBookingWorkflowInfo(IBaseBookingWorkflowInfo):
+    """Accepted booking workflow interface"""
+
+    include_quotation = Bool(title=_("Include quotation"),
+                             description=_("Include quotation document into notification message"),
+                             required=False,
+                             default=True)
+
+    quotation_message = Text(title=_("Quotation message"),
+                             description=_("This message will be added to quotation"),
+                             required=False)
+
+
+#
+# Booking container
+#
+
 BOOKING_CONTAINER_KEY = 'msc.booking'
 
 
 class IBookingContainer(IContainer):
     """Booking manager interface
 
     This interface is an :py:class:`IBookingInfo` container.
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/reminder.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/task.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 
 from pyramid.decorator import reify
 from pyramid.events import subscriber
 from pyramid.response import Response
 from pyramid.view import view_config
 from pyramid_mailer.message import Attachment
 from zope.interface import Interface, Invalid, alsoProvides, implementer
+from zope.lifecycleevent import ObjectModifiedEvent
 from zope.principalannotation.interfaces import IPrincipalAnnotationUtility
 
-from pyams_app_msc.feature.booking import get_booking_message_values
-from pyams_app_msc.feature.booking.interfaces import BOOKING_STATUS, BOOKING_STATUS_VOCABULARY, IBookingContainer, \
-    IBookingInfo, IBookingTarget
+from pyams_app_msc.feature.booking.interfaces import BOOKING_STATUS, BOOKING_STATUS_VOCABULARY, \
+    IAcceptedBookingWorkflowInfo, IBookingAcceptInfo, IBookingContainer, IBookingInfo, IBookingTarget
+from pyams_app_msc.feature.booking.message import get_booking_message, get_booking_message_values
 from pyams_app_msc.feature.booking.zmi.interfaces import IBookingContainerTable, IBookingContainerView, IBookingForm
 from pyams_app_msc.feature.messaging import IMessagingSettings
 from pyams_app_msc.feature.planning.interfaces import ISession
 from pyams_app_msc.feature.profile import IOperatorProfile, IUserProfile, USER_PROFILE_KEY
 from pyams_app_msc.feature.profile.interfaces import SEATS_DISPLAY_MODE
 from pyams_app_msc.feature.profile.zmi.widget import PrincipalSelectFieldWidget
 from pyams_app_msc.interfaces import MANAGE_BOOKING_PERMISSION, VIEW_BOOKING_PERMISSION
@@ -40,14 +41,15 @@
 from pyams_app_msc.zmi import msc
 from pyams_content.feature.history import IHistoryContainer
 from pyams_content.feature.history.zmi.viewlet import HistoryCommentsContentProvider
 from pyams_content.zmi import content_js
 from pyams_form.ajax import ajax_form_config
 from pyams_form.button import Buttons, handler
 from pyams_form.field import Fields
+from pyams_form.form import apply_changes
 from pyams_form.group import Group
 from pyams_form.interfaces import DISPLAY_MODE
 from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent, IGroup
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_mail.interfaces import IPrincipalMailInfo
 from pyams_mail.message import HTMLMessage
 from pyams_pagelet.pagelet import pagelet_config
@@ -60,24 +62,25 @@
 from pyams_table.column import GetAttrColumn
 from pyams_table.interfaces import IColumn, IValues
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
 from pyams_utils.factory import factory_config
 from pyams_utils.fanstatic import get_resource_path
 from pyams_utils.interfaces import MISSING_INFO
 from pyams_utils.interfaces.data import IObjectData
+from pyams_utils.interfaces.form import NO_VALUE, NO_VALUE_STRING
 from pyams_utils.registry import get_utility
 from pyams_utils.timezone import tztime
 from pyams_utils.traversing import get_parent
 from pyams_utils.url import absolute_url
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminModalAddForm, AdminModalDisplayForm, AdminModalEditForm, \
     FormGroupChecker, SimpleAddFormRenderer, SimpleEditFormRenderer
 from pyams_zmi.helper.container import delete_container_element
 from pyams_zmi.interfaces import IAdminLayer, IObjectLabel, TITLE_SPAN_BREAK
-from pyams_zmi.interfaces.form import IFormTitle, IModalAddFormButtons, IModalDisplayFormButtons, check_submit_button
+from pyams_zmi.interfaces.form import IFormTitle, IModalDisplayFormButtons, check_submit_button
 from pyams_zmi.interfaces.table import ITableElementEditor, ITableWithActions
 from pyams_zmi.interfaces.viewlet import IToolbarViewletManager
 from pyams_zmi.table import I18nColumnMixin, IconColumn, InnerTableAdminView, NameColumn, Table, TableElementEditor, \
     TrashColumn
 from pyams_zmi.utils import get_object_hint, get_object_label
 
 __docformat__ = 'restructuredtext'
@@ -349,37 +352,39 @@
             return None
         return ContextAddAction.__new__(cls)
 
     def get_href(self):
         return absolute_url(self.context, self.request, f'++booking++/{self.href}')
 
 
-class IBookingAddFormButtons(IModalAddFormButtons):
-    """Booking add form buttons"""
-
-    validate = SubmitButton(name='validate',
-                            title=_("Add and accept"),
-                            condition=check_submit_button)
+# class IBookingAddFormButtons(IModalAddFormButtons):
+#     """Booking add form buttons"""
+#
+#     validate = SubmitButton(name='validate',
+#                             title=_("Add and accept"),
+#                             condition=check_submit_button)
 
 
 @ajax_form_config(name='add-booking.html',
                   context=IBookingContainer, layer=IPyAMSLayer,
                   permission=MANAGE_BOOKING_PERMISSION)
 class BookingAddForm(AdminModalAddForm):
     """Booking add form"""
 
+    modal_class = 'modal-xl'
+
     subtitle = _("New booking")
     legend = _("New booking properties")
 
     fields = Fields(IBookingInfo).select('recipient', 'status',
-                                         'nb_participants', 'nb_accompanists',
+                                         'nb_participants', 'nb_accompanists', 'nb_free_accompanists',
                                          'nb_groups', 'price', 'accompanying_ratio',
                                          'cultural_pass', 'comments', 'notepad')
     fields['recipient'].widget_factory = PrincipalSelectFieldWidget
-    buttons = Buttons(IBookingAddFormButtons).select('add', 'validate', 'close')
+    # buttons = Buttons(IBookingAddFormButtons).select('add', 'validate', 'close')
 
     content_factory = IBookingInfo
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         status = self.widgets.get('status')
         if status is not None:
@@ -402,50 +407,130 @@
                 'ams-select2-helper-argument': 'price_id',
                 'ams-select2-helper-callback': 'MyAMS.msc.booking.priceChanged'
             }
             alsoProvides(price, IObjectData)
 
     def update_actions(self):
         super().update_actions()
-        validate  =self.actions.get('validate')
+        validate = self.actions.get('validate')
         if validate is not None:
             validate.add_class('btn-info')
 
     def update_content(self, obj, data):
+        request = self.request
         form_data = data.get(self, data)
-        if form_data.get('notepad'):
+        notepad = form_data.get('notepad')
+        message = form_data.get('notify_message') if form_data.get('notify_recipient') else None
+        if notepad or message:
             history = IHistoryContainer(obj, None)
             if history is not None:
                 history.add_history(obj,
-                                    comment=form_data.get('notepad'),
-                                    request=self.request)
-        changes = super().update_content(obj, data)
-        obj.creator = self.request.principal.id
+                                    comment=notepad,
+                                    message=message,
+                                    request=request)
+        changes = apply_changes(self, obj, form_data)
+        obj.creator = request.principal.id
+        accepted = form_data.get('accepted', False)
+        if accepted:
+            obj.status = BOOKING_STATUS.ACCEPTED.value
+            if 'quotation_message' in form_data:
+                obj.quotation_message = form_data['quotation_message']
+            request.registry.notify(ObjectModifiedEvent(obj))
+            if message:
+                settings = IMessagingSettings(request.root, None)
+                if settings is None:
+                    return changes
+                mailer = settings.get_mailer()
+                if mailer is None:
+                    return changes
+                html_message = get_booking_message(_("Booking accepted"), form_data,
+                                                   obj, request, settings)
+                if html_message is not None:
+                    mailer.send(html_message)
         return changes
 
     def add(self, obj):
         IBookingContainer(self.context).append(obj)
 
-    @handler(IBookingAddFormButtons['add'])
-    def handle_add(self, action):
-        return super().handle_add(self, action)
-
-    @handler(IBookingAddFormButtons['validate'])
-    def handle_validate(self, action):
-        return self.handle_add(self, action)
-
 
 @adapter_config(required=(IBookingContainer, IAdminLayer, BookingAddForm),
                 provides=IFormTitle)
 def booking_add_form_title(context, request, form):
     """Booking add form title"""
     session = get_parent(context, ISession)
     return booking_target_edit_form_title(session, request, form)
 
 
+@adapter_config(name='validate.group',
+                required=(IBookingContainer, IAdminLayer, BookingAddForm),
+                provides=IGroup)
+class BookingAddFormValidateGroup(FormGroupChecker):
+    """Booking add form validate group"""
+
+    fields = Fields(IBookingAcceptInfo).select('accepted')
+    weight = 20
+
+
+@subscriber(IDataExtractedEvent, form_selector=BookingAddFormValidateGroup)
+def handle_validate_group_data(event):
+    """Handle validate group data"""
+    data = event.data
+    if data.get('accepted'):
+        parent_form = event.form.parent_form
+        if NO_VALUE_STRING in parent_form.widgets['price'].value:
+            event.form.widgets.errors += (Invalid(_("You must set a price to accept a booking!")),)
+
+
+@adapter_config(name='notify.group',
+                required=(IBookingContainer, IAdminLayer, BookingAddFormValidateGroup),
+                provides=IGroup)
+class BookingAddFormNotifyGroup(FormGroupChecker):
+    """Booking add form notify group"""
+
+    fields = Fields(IAcceptedBookingWorkflowInfo).select('notify_recipient', 'notify_subject',
+                                                         'notify_message')
+    weight = 20
+
+    def update_widgets(self, prefix=None, use_form_mode=True):
+        super().update_widgets(prefix, use_form_mode)
+        notify = self.widgets.get('notify_recipient')
+        if notify is not None:
+            notify.value = ()
+        # generate formatted messages
+        theater = get_parent(self.context, IMovieTheater)
+        templates = IMailTemplates(theater)
+        values = get_booking_message_values(self.context, self.request, self)
+        subject = self.widgets.get('notify_subject')
+        if subject is not None:
+            template = getattr(templates, 'accept_subject')
+            if template:
+                subject.value = template.format(**values)
+        message = self.widgets.get('notify_message')
+        if message is not None:
+            template = getattr(templates, f'accept_template')
+            if template:
+                message.value = template.format(**values)
+
+
+@adapter_config(name='quotation.group',
+                required=(IBookingContainer, IAdminLayer, BookingAddFormNotifyGroup),
+                provides=IGroup)
+class BookingAddFormQuotationGroup(FormGroupChecker):
+    """Booking add form quotation group"""
+
+    fields = Fields(IAcceptedBookingWorkflowInfo).select('include_quotation', 'quotation_message')
+    weight = 10
+
+    def update_widgets(self, prefix=None, use_form_mode=True):
+        super().update_widgets(prefix, use_form_mode)
+        include_quotation = self.widgets.get('include_quotation')
+        if include_quotation is not None:
+            include_quotation.value = ()
+
+
 @adapter_config(required=(IBookingContainer, IAdminLayer, BookingAddForm),
                 provides=IAJAXFormRenderer)
 class BookingAddFormRenderer(SimpleAddFormRenderer):
     """Booking add form renderer"""
 
     table_factory = IBookingContainerTable
 
@@ -457,28 +542,14 @@
                 'options': {
                     'room_id': ISession(self.context).room
                 }
             })
         return result
 
 
-@adapter_config(name='validate',
-                required=(IBookingContainer, IAdminLayer, BookingAddForm),
-                provides=IAJAXFormRenderer)
-class BookingAddFormValidateRenderer(BookingAddFormRenderer):
-    """Booking add form validate button renderer"""
-
-    def render(self, changes):
-        result = super().render(changes)
-        if changes:
-            result['status'] = 'modal'
-            result['location'] = absolute_url(changes, self.request, 'booking-accept.html')
-        return result
-
-
 @adapter_config(required=(IBookingInfo, IAdminLayer, IBookingContainerTable),
                 provides=ITableElementEditor)
 class BookingInfoEditor(TableElementEditor):
     """Booking info editor"""
 
 
 @adapter_config(required=(IBookingInfo, IAdminLayer, IBookingForm),
@@ -525,15 +596,15 @@
         return translate(_("Booking: {}")).format(
             get_object_label(self.context, self.request, self))
 
     modal_class = 'modal-xl'
     legend = _("Booking properties")
 
     fields = Fields(IBookingInfo).select('creator', 'recipient', 'status',
-                                         'nb_participants', 'nb_accompanists',
+                                         'nb_participants', 'nb_accompanists', 'nb_free_accompanists',
                                          'nb_groups', 'price', 'accompanying_ratio',
                                          'cultural_pass', 'comments', 'notepad')
     fields['recipient'].widget_factory = PrincipalSelectFieldWidget
 
     @reify
     def buttons(self):
         if self.mode == DISPLAY_MODE:
@@ -898,14 +969,15 @@
     """Preview new PDF from booking quotation"""
     booking = IBookingInfo(request.context)
     params = request.params
     quotation = booking.get_quotation(force_refresh=True,
                                       store=False,
                                       nb_participants=params.get('nb_participants'),
                                       nb_accompanists=params.get('nb_accompanists'),
+                                      nb_free_accompanists=params.get('nb_free_accompanists'),
                                       price=params.get('price'),
                                       ratio=params.get('ratio'))
     if isinstance(quotation, tuple):
         filename, quotation = quotation
     else:
         filename = 'quotation.pdf'
     return Response(content_type='application/pdf',
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/dashboard.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,15 @@
     """Booking status session column"""
 
     i18n_header = _("Session")
     css_classes = {
         'td': 'text-nowrap'
     }
     weight = 10
+    responsive_priority = 1
 
     def get_value(self, obj):
         if obj.entry is None:
             label = obj.session.label
             if label:
                 label = f'({label})'
             else:
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/home.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/home.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/reminder.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/search.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/task.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/booking/zmi/workflow.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/booking/zmi/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,30 @@
 
 from datetime import datetime, timedelta
 
 from pyramid.events import subscriber
 from pyramid.httpexceptions import HTTPBadRequest, HTTPNotFound
 from pyramid.response import Response
 from pyramid.view import view_config
-from pyramid_mailer.message import Attachment
 from zope.dublincore.interfaces import IZopeDublinCore
 from zope.interface import Interface, Invalid, alsoProvides, implementer
 from zope.lifecycleevent import ObjectModifiedEvent
 from zope.lifecycleevent.interfaces import IObjectModifiedEvent
-from zope.schema import Bool, Choice, Datetime, Text, TextLine
+from zope.schema import Choice
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary, getVocabularyRegistry
 
-from pyams_app_msc.feature.booking import get_booking_message_values
 from pyams_app_msc.feature.booking.interfaces import BOOKING_ACCEPTABLE_STATUS, BOOKING_CANCELLABLE_STATUS, \
     BOOKING_OPTIONABLE_STATUS, BOOKING_REFUSABLE_STATUS, BOOKING_SESSIONS_VOCABULARY, BOOKING_STATUS, \
-    IBookingContainer, IBookingInfo
+    IAcceptedBookingWorkflowInfo, IBaseBookingWorkflowInfo, IBookingContainer, IBookingInfo
+from pyams_app_msc.feature.booking.message import get_booking_message, get_booking_message_values
 from pyams_app_msc.feature.booking.zmi.dashboard import IBookingElement, get_booking_element
 from pyams_app_msc.feature.booking.zmi.interfaces import IBookingAcceptedStatusTable, IBookingContainerTable, \
     IBookingForm, IBookingStatusTable, IBookingWaitingStatusTable
 from pyams_app_msc.feature.messaging.interfaces import IMessagingSettings
-from pyams_app_msc.feature.planning.interfaces import IPlanning
-from pyams_app_msc.feature.planning.interfaces import ISession
+from pyams_app_msc.feature.planning.interfaces import IPlanning, ISession
 from pyams_app_msc.interfaces import MANAGE_BOOKING_PERMISSION
 from pyams_app_msc.shared.theater.api.interfaces import MSC_PRICE_API_PATH, MSC_PRICE_API_ROUTE
 from pyams_app_msc.shared.theater.interfaces import IMovieTheater, IMovieTheaterSettings
 from pyams_app_msc.shared.theater.interfaces.mail import IMailTemplates
 from pyams_app_msc.shared.theater.interfaces.room import ROOMS_VOCABULARY
 from pyams_app_msc.zmi import msc
 from pyams_content.feature.history.interfaces import IHistoryContainer
@@ -49,31 +47,26 @@
 from pyams_form.ajax import AJAXFormRenderer, ajax_form_config
 from pyams_form.button import Buttons, handler
 from pyams_form.field import Fields
 from pyams_form.group import Group
 from pyams_form.interfaces import DISPLAY_MODE
 from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent, IFormContent, IGroup
 from pyams_layer.interfaces import IPyAMSLayer
-from pyams_mail.interfaces import IPrincipalMailInfo
-from pyams_mail.message import HTMLMessage
-from pyams_security.interfaces import ISecurityManager
 from pyams_skin.interfaces.viewlet import IFormHeaderViewletManager, IHelpViewletManager
 from pyams_skin.schema.button import ActionButton, CloseButton, SubmitButton
 from pyams_skin.viewlet.help import AlertMessage
 from pyams_skin.viewlet.menu import MenuDivider, MenuItem
 from pyams_utils.adapter import adapter_config
 from pyams_utils.date import SH_TIME_FORMAT, format_date, format_datetime, format_time
 from pyams_utils.factory import create_object
 from pyams_utils.fanstatic import get_resource_path
 from pyams_utils.interfaces import ICacheKeyValue
 from pyams_utils.interfaces.data import IObjectData
 from pyams_utils.interfaces.form import NO_VALUE_STRING
-from pyams_utils.registry import get_utility
 from pyams_utils.request import query_request
-from pyams_utils.schema import HTMLField
 from pyams_utils.timezone import tztime
 from pyams_utils.traversing import get_parent
 from pyams_utils.url import absolute_url
 from pyams_utils.vocabulary import vocabulary_config
 from pyams_utils.zodb import load_object
 from pyams_viewlet.viewlet import RawContentProvider, viewlet_config
 from pyams_zmi.form import AdminModalAddForm, FormGroupChecker
@@ -89,35 +82,14 @@
 from pyams_app_msc import _
 
 
 #
 # Booking actions
 #
 
-class IBaseBookingWorkflowInfo(IBookingInfo):
-    """Base booking workflow info interface"""
-
-    created = Datetime(title=_("Creation date"),
-                       description=_("Date at which the booking was created"),
-                       required=False)
-
-    notify_recipient = Bool(title=_("Notify recipient?"),
-                            description=_("If 'yes', a notification message will be sent to the recipient"),
-                            required=False,
-                            default=True)
-
-    notify_subject = TextLine(title=_("Notification subject"),
-                              description=_("Subject of notification message sent to the recipient"),
-                              required=False)
-
-    notify_message = HTMLField(title=_("Notification message"),
-                               description=_("Notification message sent to the recipient"),
-                               required=False)
-
-
 class BaseBookingMenuItem(MenuItem):
     """Base booking menu item"""
 
     def __new__(cls, context, request, view, manager):
         booking = IBookingInfo(context)
         if booking.archived:
             return None
@@ -410,48 +382,19 @@
         if message:
             settings = IMessagingSettings(request.root, None)
             if settings is None:
                 return
             mailer = settings.get_mailer()
             if mailer is None:
                 return
-            html_message = self.get_message(data, context, request, settings)
+            html_message = get_booking_message(self.email_subject, data,
+                                               context, request, settings)
             if html_message is not None:
                 mailer.send(html_message)
 
-    def get_message(self, data, context, request, settings):
-        sm = get_utility(ISecurityManager)
-        principal = sm.get_raw_principal(context.recipient)
-        mail_info = IPrincipalMailInfo(principal, None)
-        if mail_info is None:
-            return
-        mail_addresses = [
-            f'{name} <{address}>'
-            for name, address in mail_info.get_addresses()
-        ]
-        translate = request.localizer.translate
-        subject = data.get('notify_subject') or translate(self.email_subject)
-        cc = None
-        theater = get_parent(self.context, IMovieTheater)
-        templates = IMailTemplates(theater)
-        if templates.send_copy_to_sender:
-            principal = request.principal
-            if principal is not None:
-                mail_info = IPrincipalMailInfo(principal, None)
-                if mail_info is not None:
-                    cc = [
-                        f'{name} <{address}>'
-                        for name, address in mail_info.get_addresses()
-                    ]
-        return HTMLMessage(f'{settings.subject_prefix} {subject}',
-                           from_addr=f'{settings.source_name} <{settings.source_address}>',
-                           to_addr=mail_addresses,
-                           cc=cc,
-                           html=data.get('notify_message'))
-
 
 @subscriber(IObjectModifiedEvent, context_selector=IBookingInfo)
 def update_booking_quotation(event):
     """Update booking quotation"""
     booking = event.object
     if booking.status == BOOKING_STATUS.ACCEPTED.value:
         booking.get_quotation(force_refresh=True)
@@ -483,15 +426,16 @@
 @adapter_config(name='booking.group',
                 required=(IBookingInfo, IAdminLayer, BaseBookingAdminForm),
                 provides=IGroup)
 class BookingWorkflowInfoGroup(Group):
     """Booking info group"""
 
     legend = _("Booking properties")
-    fields = Fields(IBaseBookingWorkflowInfo).select('created', 'nb_participants', 'nb_accompanists',
+    fields = Fields(IBaseBookingWorkflowInfo).select('created', 'nb_participants',
+                                                     'nb_accompanists', 'nb_free_accompanists',
                                                      'nb_groups', 'price', 'accompanying_ratio',
                                                      'comments', 'notepad')
     weight = 10
 
     def update_widgets(self, prefix=None, use_form_mode=True):
         super().update_widgets(prefix, use_form_mode)
         created = self.widgets.get('created')
@@ -502,14 +446,18 @@
         if participants is not None:
             participants.mode = DISPLAY_MODE
             participants.value = self.context.nb_participants
         accompanists = self.widgets.get('nb_accompanists')
         if accompanists is not None:
             accompanists.mode = DISPLAY_MODE
             accompanists.value = self.context.nb_accompanists
+        free_accompanists = self.widgets.get('nb_free_accompanists')
+        if free_accompanists is not None:
+            free_accompanists.mode = DISPLAY_MODE
+            free_accompanists.value = self.context.nb_free_accompanists
         groups = self.widgets.get('nb_groups')
         if groups is not None:
             groups.mode = DISPLAY_MODE
             groups.value = self.context.nb_groups
         price = self.widgets.get('price')
         if price is not None:
             price.value = self.context.price or ()
@@ -733,26 +681,14 @@
         super().handle_add(self, action)
 
 
 #
 # Accepted booking
 #
 
-class IAcceptedBookingWorkflowInfo(IBaseBookingWorkflowInfo):
-    """Accepted booking workflow interface"""
-
-    include_quotation = Bool(title=_("Include quotation"),
-                             description=_("Include quotation document into notification message"),
-                             required=False,
-                             default=True)
-
-    quotation_message = Text(title=_("Quotation message"),
-                             description=_("This message will be added to quotation"),
-                             required=False)
-
 
 @viewlet_config(name='booking-accept.menu',
                 context=IBookingInfo, layer=IAdminLayer, view=IBookingContainerTable,
                 manager=ITableActionsColumnMenu, weight=40,
                 permission=MANAGE_BOOKING_PERMISSION)
 @viewlet_config(name='booking-accept.menu',
                 context=IBookingElement, layer=IAdminLayer, view=IBookingStatusTable,
@@ -792,24 +728,14 @@
                 'ams-click-handler': 'MyAMS.msc.booking.previewQuotation',
                 'ams-click-handler-options': {
                     'target': absolute_url(self.context, self.request, 'preview-quotation.pdf')
                 }
             }
             alsoProvides(preview_quotation, IObjectData)
 
-    def get_message(self, data, context, request, settings):
-        html_message = super().get_message(data, context, request, settings)
-        if (html_message is not None) and data.get('include_quotation'):
-            quotation = context.get_quotation()
-            if quotation is not None:
-                html_message.attach(Attachment(content_type='application/pdf',
-                                               data=str(quotation),
-                                               filename=f'{context.quotation_number}.pdf'))
-        return html_message
-
     @handler(IAcceptedBookingButtons['add'])
     def handle_add(self, action):
         super().handle_add(self, action)
 
 
 @adapter_config(name='booking.group',
                 required=(IBookingInfo, IAdminLayer, BookingAcceptForm),
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/messaging/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/messaging/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/messaging/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/oauth/skin/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/oauth/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/session.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
                 provides=IJSONExporter)
 class JSONSessionExporter(JSONBaseExporter):
     """JSON session exporter"""
 
     def _add_seats(self, value):
         """Add capacity and confirmed seats to label"""
         if not self.context.bookable:
-            return value
+            return f'{value} \n'
         profile = IOperatorProfile(self.request)
         if profile.session_seats_display_mode == SEATS_DISPLAY_MODE.NONE.value:
             return f'{value} \n'
         else:
             container = IBookingContainer(self.context)
             return f'{value} \n({container.get_seats(profile.session_seats_display_mode)})'
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/zmi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,48 +100,39 @@
     def can_edit_planning(self):
         """Calendar editor checker"""
         return bool(self.request.has_permission(MANAGE_PLANNING_PERMISSION, context=self.context))
 
     def get_calendar_options(self, room):
         """Calendar options getter"""
         context = self.get_context()
+        request = self.request
         settings = IMovieTheaterSettings(self.theater)
-        can_edit = self.request.has_permission(MANAGE_PLANNING_PERMISSION, context=context)
+        can_edit = request.has_permission(MANAGE_PLANNING_PERMISSION, context=context)
         now = tztime(datetime.utcnow())
         week_day = now.weekday()
         next_wednesday = now + timedelta(days=abs(week_day - 2))
-        translate = self.request.localizer.translate
+        translate = request.localizer.translate
         options = {
             'editable': can_edit,
             'droppable': can_edit,
             'eventSources': [{
-                'url': absolute_url(context, self.request, 'get-planning-events.json'),
+                'url': absolute_url(context, request, 'get-planning-events.json'),
                 'extraParams': {
                     'room': room.__name__
                 }
             }],
             'height': '100%',
             'initialDate': next_wednesday.date().isoformat(),
-            # 'views': {
-            #     'cinemaGridWeek': {
-            #         'type': 'timeGrid',
-            #         'duration': {
-            #             'days': 7
-            #         },
-            #         'firstDay': 3,
-            #         'buttonText': translate(_('Theater week'))
-            #     }
-            # },
+            'firstDay': settings.calendar_first_day,
             'dateClick': 'MyAMS.msc.calendar.addEvent',
             'initialView': 'timeGridWeek',
             'headerToolbar': {
                 'center': 'today',
                 'right': 'prev,next dayGridMonth,timeGridWeek,timeGridDay,listMonth'
-                # 'right': 'prev,next dayGridMonth,timeGridWeek,cinemaGridWeek,timeGridDay,listMonth'
-        },
+            },
             'allDaySlot': False,
             'slotDuration': f'00:{settings.calendar_slot_duration:#02}:00',
             'slotMinTime': room.start_time.isoformat(),
             'slotMaxTime': room.end_time.isoformat(),
             'buttonText': {
                 'today': translate(_("Today")),
                 'month': translate(_("Month")),
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/session.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/zmi/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/password.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/password.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/register.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/register.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/task.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/zmi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,29 +169,32 @@
     def buttons(self):
         if self.mode == DISPLAY_MODE:
             return Buttons(IModalDisplayFormButtons)
         return Buttons(IUserProfileEditFormButtons).select('disable', 'enable', 'apply', 'close')
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
-        principal_id = self.widgets.get('principal_id')
-        if principal_id is not None:
-            principal_id.mode = HIDDEN_MODE
+        request = self.request
+        principal_id = (request.params.get('principal_id') or
+                        request.params.get(f'{self.prefix}widgets.principal_id'))
+        principal_widget = self.widgets.get('principal_id')
+        if principal_widget is not None:
+            principal_widget.mode = HIDDEN_MODE
+            principal_widget.value = principal_id
         phone_number = self.widgets.get('phone_number')
         if phone_number is not None:
             phone_number.object_data = {
                 'input-mask': '[+9{3}] [9]9 99 99 99 99'
             }
             alsoProvides(phone_number, IObjectData)
         email = self.widgets.get('email')
         if email is not None:
             email.readonly = 'readonly'
             if not email.value:
                 sm = get_utility(ISecurityManager)
-                principal_id = self.request.params.get('principal_id')
                 principal_info = sm.get_principal(principal_id, info=False)
                 if principal_info is not None:
                     mail_info = IPrincipalMailInfo(principal_info, None)
                     if mail_info is not None:
                         _title, principal_email = next(mail_info.get_addresses())
                         email.value = principal_email
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/profile/zmi/widget.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/profile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,20 @@
 from pyams_app_msc.shared.theater import IMovieTheater, IMovieTheaterSettings
 from pyams_app_msc.shared.theater.interfaces.price import ICinemaPriceContainer
 from pyams_i18n.interfaces import II18n
 from pyams_security.utility import get_principal
 from pyams_utils.date import SH_DATE_FORMAT, format_date, format_datetime
 from pyams_utils.interfaces import MISSING_INFO
 from pyams_utils.request import query_request
+from pyams_utils.text import get_text_parts
 
 __docformat__ = 'restructuredtext'
 
 from pyams_app_msc import _
-from pyams_utils.text import get_text_parts
+
 
 dirname = os.path.dirname(__file__)
 registerFont(TTFont('Roboto-Light', f"{dirname}/fonts/Roboto-Light.ttf"))
 registerFont(TTFont('Roboto-Medium', f"{dirname}/fonts/Roboto-Medium.ttf"))
 registerFont(TTFont('Roboto-Bold', f"{dirname}/fonts/Roboto-Bold.ttf"))
 
 
@@ -262,31 +263,37 @@
                 else:
                     nb_participants = int(nb_participants or 0)
                 nb_accompanists = preview_args.get('nb_accompanists')
                 if nb_accompanists is None:
                     nb_accompanists = booking.nb_accompanists
                 else:
                     nb_accompanists = int(nb_accompanists or 0)
+                nb_free_accompanists = preview_args.get('nb_free_accompanists')
+                if nb_free_accompanists is None:
+                    nb_free_accompanists = booking.nb_free_accompanists
+                else:
+                    nb_free_accompanists = int(nb_free_accompanists or 0)
+                nb_paid_accompanists = nb_accompanists - nb_free_accompanists
                 if price is not None:
                     if price.accompanying_price == 0.:
                         free_accompanists = nb_accompanists
                         paid_accompanists = 0
                     else:
                         ratio = preview_args.get('ratio')
                         if ratio is None:
                             ratio = booking.accompanying_ratio
                         else:
                             ratio = float(ratio or 0)
                         if ratio:
                             max_accompanists = math.ceil(nb_participants / ratio)
-                            free_accompanists = min(max_accompanists, nb_accompanists)
+                            free_accompanists = min(max_accompanists, nb_paid_accompanists) + nb_free_accompanists
                             paid_accompanists = nb_accompanists - free_accompanists
                         else:
-                            free_accompanists = 0
-                            paid_accompanists = nb_accompanists
+                            free_accompanists = nb_free_accompanists
+                            paid_accompanists = nb_paid_accompanists
                     participants_amount = price.participant_price * nb_participants
                     accompanying_amount = price.accompanying_price * paid_accompanists
                 else:
                     free_accompanists = nb_accompanists
                     paid_accompanists = 0
                     participants_amount = 0.
                     accompanying_amount = 0.
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/api/schema.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/feature/tmdb/zmi/lookup.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/feature/tmdb/zmi/lookup.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/generations/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/include.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/include.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo` & `pyams_app_msc-1.99.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -331,14 +331,17 @@
 
 msgid "Bookings archiver task"
 msgstr "Archivage des réservations"
 
 msgid "Bookings search form"
 msgstr "Recherche de réservations"
 
+msgid "Calendar first week day"
+msgstr "Premier jour de la semaine"
+
 msgid "Calendar slot duration"
 msgstr "Durée des créneaux horaires"
 
 msgid "Calendar time slots frequency in week or day views"
 msgstr ""
 "Indiquée en minutes, cette valeur indique la durée des créneaux horaires "
 "affichés dans les vues par semaine ou par jour de l'agenda ; vous pouvez "
@@ -511,17 +514,14 @@
 
 msgid "Contact phone number"
 msgstr "Téléphone"
 
 msgid "Contacts"
 msgstr "Contacts"
 
-msgid "Content illustration has been updated successfully."
-msgstr "L'illustration du contenu a été modifiée avec succès."
-
 msgid "Contributors"
 msgstr "Contributeurs"
 
 msgid ""
 "Contributors can add activities to theater catalog, but can't publish them"
 msgstr ""
 "Les contributeurs peuvent ajouter des activités au catalogue, mais ne "
@@ -717,20 +717,31 @@
 
 msgid "First name"
 msgstr "Prénom"
 
 msgid "First time available for sessions planning"
 msgstr "Heure à partir de laquelle des événements peuvent être programmés"
 
+msgid "First week day used in calendars"
+msgstr ""
+"Le premier jour de la semaine est utilisé pour l'affichage des semaines dans "
+"les agendas, que ce soit en mode \"mois\" ou en mode \"semaine\""
+
 msgid "Forbidden cancellation"
 msgstr "Annulation impossible"
 
+msgid "Free accompanists"
+msgstr "... dont accompagnateurs non payants"
+
 msgid "Free seats"
 msgstr "Places disponibles"
 
+msgid "Friday"
+msgstr "Vendredi"
+
 msgid "Full name"
 msgstr "Nom complet"
 
 msgid "Full theater address"
 msgstr "Adresse complète du cinéma"
 
 msgid "Gallery medias"
@@ -839,14 +850,17 @@
 "Si 'oui', cet événement est encore temporaire, en attente de confirmation..."
 
 msgid "If no label is set, activity label will be used"
 msgstr ""
 "Ce libellé sera affiché s'il n'y a pas d'activité associée à cet événement, "
 "ou à la place du libellé de l'activité si vous en avez sélectionné une"
 
+msgid "Illustration has been updated successfully."
+msgstr "L'illustration a été modifiée avec succès."
+
 msgid "Images URL"
 msgstr "URL des images"
 
 msgid "Inactive users can't login anymore to website"
 msgstr ""
 "Un profil désactivé ne peut plus être utilisé pour se connecter au site"
 
@@ -1053,14 +1067,17 @@
 
 msgid "Minimum notice period before session"
 msgstr "Imposer un préavis minimum avant le début de la séance"
 
 msgid "Modification date"
 msgstr "Date de modification"
 
+msgid "Monday"
+msgstr "Lundi"
+
 msgid "Month"
 msgstr "Mois"
 
 msgid "Movie ID in TMDB database"
 msgstr "Identifiant du film dans la base TMDB"
 
 msgid "Movie credits path"
@@ -1201,20 +1218,30 @@
 
 msgid "Notify recipient?"
 msgstr "Notifier le bénéficiaire"
 
 msgid "Number and street"
 msgstr "Numéro et rue"
 
-msgid "Number of accompanists seats reserved for this session"
-msgstr "Nombre de places réservées pour les accompagnants à cet événement"
-
 msgid "Number of actors "
 msgstr "Nombre maximal d'acteurs récupérés via l'API"
 
+msgid ""
+"Number of free accompanists can't be higher than total number of "
+"accompanists!"
+msgstr ""
+"Le nombre d'accompagnateurs non payants ne peut pas être supérieur au nombre "
+"total d'accompagnateurs !"
+
+msgid "Number of free accompanists seats reserved for this session"
+msgstr ""
+"Nombre d'accompagnateurs non payants pris en charge à cet événement ; seuls "
+"les accompagnateurs au-delà de ce nombre sont pris en compte dans le calcul "
+"du ratio indiqué ci-dessous"
+
 msgid "Number of free seats for this session"
 msgstr ""
 "Nombre de places encore disponibles pour cet événement ; seules les "
 "réservations validées sont prises en compte, y compris cette réservation le "
 "cas échéant"
 
 msgid "Number of groups or classrooms attending this session"
@@ -1530,14 +1557,17 @@
 
 msgid "SIRET code"
 msgstr "Code SIRET"
 
 msgid "SIRET: {}"
 msgstr "SIRET : {}"
 
+msgid "Saturday"
+msgstr "Samedi"
+
 msgid "Search results"
 msgstr "Résultats de la recherche"
 
 msgid "Seats"
 msgstr "Places"
 
 msgid "Select structure type matching this establishment"
@@ -1622,16 +1652,19 @@
 
 msgid "Sessions planning"
 msgstr "Agenda des événements programmés"
 
 msgid "Sessions weeks"
 msgstr "Nombre de semaines"
 
-msgid "Set as content illustration"
-msgstr "Utiliser comme illustration du contenu"
+msgid "Set content illustration"
+msgstr "Utiliser comme illustration principale"
+
+msgid "Set navigation illustration"
+msgstr "Utiliser comme illustration de navigation"
 
 msgid "Settings"
 msgstr "Paramètres"
 
 msgid "Site's header is generally displayed in page header"
 msgstr "Le chapô est généralement affiché dans les en-têtes de pages"
 
@@ -1676,14 +1709,17 @@
 
 msgid "Subject of update message sent to the recipient"
 msgstr "Sujet du message de modification adressé au bénéficiaire"
 
 msgid "Subject prefix"
 msgstr "Préfixe des sujets"
 
+msgid "Sunday"
+msgstr "Dimanche"
+
 msgid "Synchronize calendars scrolling"
 msgstr "Synchroniser le défilement des agendas"
 
 msgid "Synchronize calendars views"
 msgstr "Synchroniser les vues des agendas"
 
 msgid "Synopsis"
@@ -2004,14 +2040,17 @@
 
 msgid ""
 "This template is used when a session booking is updated after being accepted"
 msgstr ""
 "Ce modèle est utilisé en cas de modification d'une demande de réservation "
 "déjà acceptée"
 
+msgid "Thursday"
+msgstr "Jeudi"
+
 msgid "Title"
 msgstr "Titre"
 
 msgid "Today"
 msgstr "Aujourd'hui"
 
 msgid "Today program"
@@ -2019,20 +2058,27 @@
 
 msgid "Total"
 msgstr "Total"
 
 msgid "Total amount"
 msgstr "Total TTC"
 
+msgid "Total number of accompanists seats reserved for this session"
+msgstr ""
+"Nombre total de places réservées pour les accompagnateurs à cet événement"
+
 msgid "Translated version"
 msgstr "Version traduite"
 
 msgid "Transpose calendars"
 msgstr "Transposer les agendas"
 
+msgid "Tuesday"
+msgstr "Mardi"
+
 msgid "URL of theater web site"
 msgstr "URL du site web du cinéma"
 
 msgid "Unit price"
 msgstr "Tarif"
 
 msgid "Units"
@@ -2116,14 +2162,17 @@
 "Vous devriez recevoir très prochainement un nouveau message électronique "
 "contenant un lien vous permettant de confirmer votre changement de mot de "
 "passe."
 
 msgid "Website address"
 msgstr "Addresse web"
 
+msgid "Wednesday"
+msgstr "Mercredi"
+
 msgid "Week"
 msgstr "Semaine"
 
 msgid "Workflow name"
 msgstr "Nom du workflow"
 
 msgid "Writer:"
@@ -2167,17 +2216,20 @@
 "\"hors catalogue\" ne vous empêche pas cependant d'y associer des "
 "réservations"
 
 msgid ""
 "You can set an integer number which will define the count of participants "
 "for which one accompanying person will have free access"
 msgstr ""
-"Vous pouvez indiquer ici le nombre de participants par accompagnateur qui "
-"bénéficient d'une entrée non payante, ou 0 pour que tous les accompagnateurs "
-"aient à régler leur entrée"
+"Ce ratio s'applique pour déterminer le nombre d'accompagnateurs payants, qui "
+"est calculé en divisant le nombre d'entrées par le nombre d'accompagnateurs "
+"au-delà du nombre d'accompagnateurs non payants indiqué ci-dessus (arrondi "
+"au nombre supérieur) ; vous pouvez donc indiquer ici le nombre de "
+"participants par accompagnateur qui bénéficient d'une entrée non payante, ou "
+"0 pour que tous les accompagnateurs aient à régler leur entrée"
 
 msgid ""
 "You can set an integer number which will define the count of participants "
 "for which one accompanying person will have free access; this ratio will "
 "still be updatable on all bookings using this price"
 msgstr ""
 "Vous pouvez indiquer ici le nombre de participants par accompagnateur qui "
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po` & `pyams_app_msc-1.99.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # PyAMS application for cinema reservation management
 #
 # This file is distributed under the same license as the PACKAGE package.
 # Thierry Florac <tflorac@ulthar.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: PyAMS MSC application 1.0.0\n"
-"POT-Creation-Date: 2024-05-05 20:34+0200\n"
+"POT-Creation-Date: 2024-05-14 22:26+0200\n"
 "Last-Translator: Thierry Florac <tflorac@ulthar.net>\n"
 "Language-Team: FRENCH <FR@li.org>\n"
 "Language: French\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
@@ -461,23 +461,23 @@
 msgid "Enable profile"
 msgstr "Activer le profil"
 
 #: src/pyams_app_msc/feature/profile/zmi/__init__.py:163
 msgid "User edit form"
 msgstr "Modification d'un compte utilisateur"
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:204
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:207
 msgid ""
 "Disabled profiles can't be used for website login anymore but can still be "
 "assigned new bookings"
 msgstr ""
 "Un profil utilisateur désactivé ne peut plus être utilisé pour se connecter "
 "sur le site, mais peut toujours être bénéficiaire de nouvelles réservations"
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:292
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:295
 msgid "Operator profile"
 msgstr "Mon profil opérateur"
 
 #: src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt:53
 msgid "Edit user profile"
 msgstr "Modifier le profil utilisateur"
 
@@ -715,15 +715,15 @@
 
 #: src/pyams_app_msc/feature/messaging/zmi/__init__.py:54
 msgid "Messaging properties"
 msgstr "Propriétés de la messagerie"
 
 #: src/pyams_app_msc/feature/planning/session.py:155
 #: src/pyams_app_msc/feature/planning/zmi/session.py:236
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:198
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:199
 #: src/pyams_app_msc/shared/theater/zmi/session.py:76
 msgid "Out of catalog activity"
 msgstr "(activité hors-catalogue)"
 
 #: src/pyams_app_msc/feature/planning/session.py:160
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:180
 #, python-format
@@ -870,29 +870,29 @@
 #: src/pyams_app_msc/feature/planning/interfaces.py:129
 msgid "These comments will be displayed to the users on booking form"
 msgstr ""
 "Ce commentaire sera visible sur le formulaire de réservation associé à cet "
 "événement"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:132
-#: src/pyams_app_msc/feature/booking/interfaces.py:165
+#: src/pyams_app_msc/feature/booking/interfaces.py:176
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:59
 #: src/pyams_app_msc/shared/theater/interfaces/audience.py:58
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:103
 #: src/pyams_app_msc/shared/theater/interfaces/price.py:62
 msgid "Notepad"
 msgstr "Bloc-notes"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:133
-#: src/pyams_app_msc/feature/booking/interfaces.py:166
+#: src/pyams_app_msc/feature/booking/interfaces.py:177
 msgid "These comments are for internal use only"
 msgstr "Ce commentaire est à usage interne uniquement"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:140
-#: src/pyams_app_msc/feature/quotation/__init__.py:297
+#: src/pyams_app_msc/feature/quotation/__init__.py:304
 msgid "Activity"
 msgstr "Activité"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:141
 msgid ""
 "You can select an existing activity from your catalog, or keep this input "
 "empty if you just want to mark a period as not being available for booking"
@@ -969,47 +969,47 @@
 msgid "Planning"
 msgstr "Agenda"
 
 #: src/pyams_app_msc/feature/planning/zmi/__init__.py:76
 msgid "Sessions planning"
 msgstr "Agenda des événements programmés"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:146
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:137
 msgid "Today"
 msgstr "Aujourd'hui"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:147
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:138
 msgid "Month"
 msgstr "Mois"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:148
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:139
 msgid "Week"
 msgstr "Semaine"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:149
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:140
 msgid "Day"
 msgstr "Jour"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:150
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:141
 msgid "List"
 msgstr "Liste"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:151
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:142
 msgid "All-day"
 msgstr "(jour)"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:197
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:188
 msgid "Transpose calendars"
 msgstr "Transposer les agendas"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:210
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:201
 msgid "Synchronize calendars views"
 msgstr "Synchroniser les vues des agendas"
 
-#: src/pyams_app_msc/feature/planning/zmi/__init__.py:223
+#: src/pyams_app_msc/feature/planning/zmi/__init__.py:214
 msgid "Synchronize calendars scrolling"
 msgstr "Synchroniser le défilement des agendas"
 
 #: src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:13
 #: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:13
 #: src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt:17
 msgid "Back to previous page"
@@ -1019,128 +1019,128 @@
 msgid "Manage event booking..."
 msgstr "Gérer les réservations"
 
 #: src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:50
 msgid "Clone event..."
 msgstr "Dupliquer l'événement"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:166
+#: src/pyams_app_msc/feature/quotation/__init__.py:167
 msgid "QUOTATION"
 msgstr "DEVIS"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:194
+#: src/pyams_app_msc/feature/quotation/__init__.py:195
 msgid "#Quotation:"
 msgstr "N° de devis :"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:196
+#: src/pyams_app_msc/feature/quotation/__init__.py:197
 msgid "Date:"
 msgstr "Date :"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:198
+#: src/pyams_app_msc/feature/quotation/__init__.py:199
 msgid "Object:"
 msgstr "Objet :"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:298
+#: src/pyams_app_msc/feature/quotation/__init__.py:305
 msgid "Units"
 msgstr "Unités"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:299
+#: src/pyams_app_msc/feature/quotation/__init__.py:306
 msgid "Unit price"
 msgstr "Tarif"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:300
+#: src/pyams_app_msc/feature/quotation/__init__.py:307
 msgid "Total"
 msgstr "Total"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:305
+#: src/pyams_app_msc/feature/quotation/__init__.py:312
 #, python-format
 msgid "   - Entries ({})"
 msgstr "   - Entrées ({})"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:306
+#: src/pyams_app_msc/feature/quotation/__init__.py:313
 #: src/pyams_app_msc/feature/booking/zmi/home.py:93
 msgid "1 group"
 msgstr "1 groupe"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:307
+#: src/pyams_app_msc/feature/quotation/__init__.py:314
 #: src/pyams_app_msc/feature/booking/zmi/home.py:92
 #, python-format
 msgid "{} groups"
 msgstr "{} groupes"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:314
+#: src/pyams_app_msc/feature/quotation/__init__.py:321
 msgid "   - Free accompanists"
 msgstr "   - Accompagnateurs non payants"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:321
+#: src/pyams_app_msc/feature/quotation/__init__.py:328
 msgid "   - Paying accompanists"
 msgstr "   - Accompagnateurs payants"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:332
+#: src/pyams_app_msc/feature/quotation/__init__.py:339
 msgid "Base amount"
 msgstr "Total HT"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:336
+#: src/pyams_app_msc/feature/quotation/__init__.py:343
 msgid "VAT"
 msgstr "TVA"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:340
+#: src/pyams_app_msc/feature/quotation/__init__.py:347
 msgid "Total amount"
 msgstr "Total TTC"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:375
+#: src/pyams_app_msc/feature/quotation/__init__.py:382
 #, python-format
 msgid "Bank location: {}"
 msgstr "Établissement bancaire : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:376
+#: src/pyams_app_msc/feature/quotation/__init__.py:383
 #: src/pyams_app_msc/component/banking/interfaces.py:31
 msgid "Bank code"
 msgstr "Code banque"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:377
+#: src/pyams_app_msc/feature/quotation/__init__.py:384
 #: src/pyams_app_msc/component/banking/interfaces.py:36
 msgid "Counter code"
 msgstr "Code guichet"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:378
+#: src/pyams_app_msc/feature/quotation/__init__.py:385
 #: src/pyams_app_msc/component/banking/interfaces.py:41
 msgid "Account number"
 msgstr "N° de compte"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:379
+#: src/pyams_app_msc/feature/quotation/__init__.py:386
 msgid "Key"
 msgstr "Clé"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:384
+#: src/pyams_app_msc/feature/quotation/__init__.py:391
 #, python-format
 msgid "IBAN: {}"
 msgstr "IBAN : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:387
+#: src/pyams_app_msc/feature/quotation/__init__.py:394
 #, python-format
 msgid "BIC: {}"
 msgstr "BIC : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:418
+#: src/pyams_app_msc/feature/quotation/__init__.py:425
 #, python-format
 msgid "APE: {}"
 msgstr "APE : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:419
+#: src/pyams_app_msc/feature/quotation/__init__.py:426
 #, python-format
 msgid "SIRET: {}"
 msgstr "SIRET : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:421
+#: src/pyams_app_msc/feature/quotation/__init__.py:428
 #, python-format
 msgid "VAT: {}"
 msgstr "Code TVA : {}"
 
-#: src/pyams_app_msc/feature/quotation/__init__.py:447
+#: src/pyams_app_msc/feature/quotation/__init__.py:454
 #, python-format
 msgid "Quotation: {}"
 msgstr "Devis : {}"
 
 #: src/pyams_app_msc/feature/booking/reminder.py:50
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:821
 #: src/pyams_app_msc/shared/theater/zmi/mail.py:142
@@ -1164,36 +1164,36 @@
 msgstr "En attente de confirmation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:79
 msgid "Accepted"
 msgstr "Acceptée"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:109
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:242
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:243
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:126
 msgid "Creator"
 msgstr "Créateur"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:110
 msgid "Name of the principal who created the booking"
 msgstr "Nom du mandataire ayant effectué la demande de réservation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:113
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:258
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:259
 #: src/pyams_app_msc/feature/booking/zmi/search.py:71
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:140
 msgid "Recipient"
 msgstr "Bénéficiaire"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:114
 msgid "Name of the principal for which the booking is done"
 msgstr "Nom du mandataire bénéficiaire de la réservation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:120
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:302
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:303
 #: src/pyams_app_msc/feature/booking/zmi/search.py:74
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:183
 msgid "Status"
 msgstr "Statut"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:125
 msgid "Participants"
@@ -1204,192 +1204,215 @@
 msgstr "Nombre de places réservées pour les participants à cet événement"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:130
 msgid "Accompanists"
 msgstr "Accompagnateurs"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:131
-msgid "Number of accompanists seats reserved for this session"
-msgstr "Nombre de places réservées pour les accompagnants à cet événement"
+msgid "Total number of accompanists seats reserved for this session"
+msgstr ""
+"Nombre total de places réservées pour les accompagnateurs à cet événement"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:135
+msgid "Free accompanists"
+msgstr "... dont accompagnateurs non payants"
+
+#: src/pyams_app_msc/feature/booking/interfaces.py:136
+msgid "Number of free accompanists seats reserved for this session"
+msgstr ""
+"Nombre d'accompagnateurs non payants pris en charge à cet événement ; seuls "
+"les accompagnateurs au-delà de ce nombre sont pris en compte dans le calcul "
+"du ratio indiqué ci-dessous"
+
+#: src/pyams_app_msc/feature/booking/interfaces.py:144
+msgid ""
+"Number of free accompanists can't be higher than total number of "
+"accompanists!"
+msgstr ""
+"Le nombre d'accompagnateurs non payants ne peut pas être supérieur au nombre "
+"total d'accompagnateurs !"
+
+#: src/pyams_app_msc/feature/booking/interfaces.py:146
 msgid "Groups count"
 msgstr "Nombre de groupes"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:136
+#: src/pyams_app_msc/feature/booking/interfaces.py:147
 msgid "Number of groups or classrooms attending this session"
 msgstr "Nombre de groupes ou de classes participant à cet événement"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:141
+#: src/pyams_app_msc/feature/booking/interfaces.py:152
 msgid "Price"
 msgstr "Tarif"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:142
+#: src/pyams_app_msc/feature/booking/interfaces.py:153
 msgid "Price applied to this booking"
 msgstr "Tarif appliqué à cette réservation"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:149
+#: src/pyams_app_msc/feature/booking/interfaces.py:160
 #: src/pyams_app_msc/shared/theater/interfaces/price.py:46
 msgid "Accompanying ratio"
 msgstr "Ratio d'accompagnateurs"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:150
+#: src/pyams_app_msc/feature/booking/interfaces.py:161
 msgid ""
 "You can set an integer number which will define the count of participants "
 "for which one accompanying person will have free access"
 msgstr ""
-"Vous pouvez indiquer ici le nombre de participants par accompagnateur qui "
-"bénéficient d'une entrée non payante, ou 0 pour que tous les accompagnateurs "
-"aient à régler leur entrée"
+"Ce ratio s'applique pour déterminer le nombre d'accompagnateurs payants, qui "
+"est calculé en divisant le nombre d'entrées par le nombre d'accompagnateurs "
+"au-delà du nombre d'accompagnateurs non payants indiqué ci-dessus (arrondi "
+"au nombre supérieur) ; vous pouvez donc indiquer ici le nombre de "
+"participants par accompagnateur qui bénéficient d'une entrée non payante, ou "
+"0 pour que tous les accompagnateurs aient à régler leur entrée"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:156
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:272
+#: src/pyams_app_msc/feature/booking/interfaces.py:167
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:273
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:169
 #: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:47
 msgid "Cultural pass"
 msgstr "Pass Culture"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:157
+#: src/pyams_app_msc/feature/booking/interfaces.py:168
 msgid "Check this option if payment is done using cultural pass"
 msgstr ""
 "Sélectionnez cette option lorsque le paiement est fait via un Pass Culture"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:161
+#: src/pyams_app_msc/feature/booking/interfaces.py:172
 #: src/pyams_app_msc/feature/booking/skin/__init__.py:53
 #: src/pyams_app_msc/component/address/interfaces.py:41
 #: src/pyams_app_msc/shared/theater/interfaces/audience.py:50
 #: src/pyams_app_msc/shared/theater/interfaces/price.py:58
 msgid "Comments"
 msgstr "Commentaire"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:162
+#: src/pyams_app_msc/feature/booking/interfaces.py:173
 msgid "These comments where added by booking recipient"
 msgstr "Ce commentaire précise la demande du bénéficiaire"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:169
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:363
+#: src/pyams_app_msc/feature/booking/interfaces.py:180
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:364
 msgid "Archived"
 msgstr "Archivée"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:170
+#: src/pyams_app_msc/feature/booking/interfaces.py:181
 msgid ""
 "A booking is archived automatically after session end and can't be modified "
 "anymore"
 msgstr ""
 "Une réservation est archivée automatiquement après la fin de l'événement "
 "correspondant et ne peut plus être modifiée"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:187
+#: src/pyams_app_msc/feature/booking/interfaces.py:198
 msgid "Quotation number"
 msgstr "Numéro de devis"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:188
+#: src/pyams_app_msc/feature/booking/interfaces.py:199
 msgid "This is the reference number of the quotation"
 msgstr "Ceci est la référence du devis"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:191
+#: src/pyams_app_msc/feature/booking/interfaces.py:202
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:748
 msgid "Quotation message"
 msgstr "Message associé au devis"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:192
+#: src/pyams_app_msc/feature/booking/interfaces.py:203
 msgid "This message is added to quotation as an information message"
 msgstr "Ce message d'information est associé au devis envoyé au client"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:195
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:320
+#: src/pyams_app_msc/feature/booking/interfaces.py:206
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:321
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:214
 msgid "Quotation"
 msgstr "Devis"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:196
+#: src/pyams_app_msc/feature/booking/interfaces.py:207
 msgid "This quotation was attached to booking confirmation"
 msgstr "Ceci est le document au format PDF contenant le devis"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:199
+#: src/pyams_app_msc/feature/booking/interfaces.py:210
 msgid "Send update message?"
 msgstr "Envoyer un nouveau message de modification"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:200
+#: src/pyams_app_msc/feature/booking/interfaces.py:211
 msgid "If 'yes', a message will be sent to the recipient "
 msgstr ""
 "Si cette option est activée, un message de notification sera adressé au "
 "bénéficiaire de la demande de réservation en cas de modification de cette "
 "demande de réservation qui a déjà été validée"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:204
+#: src/pyams_app_msc/feature/booking/interfaces.py:215
 msgid "Update subject"
 msgstr "Sujet des messages"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:205
+#: src/pyams_app_msc/feature/booking/interfaces.py:216
 msgid "Subject of update message sent to the recipient"
 msgstr "Sujet du message de modification adressé au bénéficiaire"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:208
+#: src/pyams_app_msc/feature/booking/interfaces.py:219
 msgid "Update message"
 msgstr "Contenu du message"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:209
+#: src/pyams_app_msc/feature/booking/interfaces.py:220
 msgid ""
 "Update message will be sent to the recipient if booking properties are "
 "changed..."
 msgstr ""
 "Ce message sera adressé au bénéficiaire en cas de modification des éléments "
 "de la réservation"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:213
+#: src/pyams_app_msc/feature/booking/interfaces.py:224
 msgid "Send reminder?"
 msgstr "Envoyer un message de rappel"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:214
+#: src/pyams_app_msc/feature/booking/interfaces.py:225
 msgid ""
 "If 'yes', a reminder message will be sent to the recipient a few days before "
 "the session take place; delay before session is defined into theater settings"
 msgstr ""
 "Si cette option est activée, un message de rappel sera envoyé au "
 "bénéficiaire de la réservations quelques heures ou jours avant le début de "
 "l'événement ; ce délai est spécifié dans les paramètres du cinéma"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:220
+#: src/pyams_app_msc/feature/booking/interfaces.py:231
 #: src/pyams_app_msc/shared/theater/interfaces/mail.py:81
 msgid "Reminder subject"
 msgstr "Sujet des messages"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:221
+#: src/pyams_app_msc/feature/booking/interfaces.py:232
 msgid "Subject of reminder message sent to the recipient"
 msgstr "Sujet du message de rappel adressé au bénéficiaire"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:224
+#: src/pyams_app_msc/feature/booking/interfaces.py:235
 msgid "Reminder message"
 msgstr "Contenu du message"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:225
+#: src/pyams_app_msc/feature/booking/interfaces.py:236
 msgid ""
 "Reminder message will be sent to the recipient a few days before the session "
 "take place; delay before session is defined into theater settings"
 msgstr ""
 "Le message de rappel est envoyé au bénéficiaire quelques heures ou jours "
 "avant le début de l'événement, en fonction du paramétrage appliqué au niveau "
 "du cinéma"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:230
+#: src/pyams_app_msc/feature/booking/interfaces.py:241
 msgid "Reminder date"
 msgstr "Date du rappel"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:231
+#: src/pyams_app_msc/feature/booking/interfaces.py:242
 msgid "Date and time at which reminder message was sent"
 msgstr ""
 "Date et heure auxquelles le message de rappel a été envoyé ; une valeur vide "
 "indique que ce message n'a pas encore été envoyé..."
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:263
+#: src/pyams_app_msc/feature/booking/interfaces.py:274
 msgid "Free seats"
 msgstr "Places disponibles"
 
-#: src/pyams_app_msc/feature/booking/interfaces.py:264
+#: src/pyams_app_msc/feature/booking/interfaces.py:275
 msgid "Number of free seats for this session"
 msgstr ""
 "Nombre de places encore disponibles pour cet événement ; seules les "
 "réservations validées sont prises en compte, y compris cette réservation le "
 "cas échéant"
 
 #: src/pyams_app_msc/feature/booking/task.py:51
@@ -1602,53 +1625,53 @@
 msgid "Booking dashboard"
 msgstr "Gestion des réservations"
 
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:186
 msgid "Session"
 msgstr "Séance"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:209
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:210
 msgid "Room"
 msgstr "Salle"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:226
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:227
 msgid "Date"
 msgstr "Date"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:286
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:287
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:199
 msgid "Seats"
 msgstr "Places"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:341
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:342
 msgid "Last update"
 msgstr "Dernière modification"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:407
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:408
 msgid "MANAGER - No booking waiting for your action"
 msgstr "RESPONSABLE - Aucune réservation en attente"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:408
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:409
 msgid "MANAGER - 1 booking waiting for your action"
 msgstr "RESPONSABLE - 1 réservation en attente"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:409
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:410
 #, python-format
 msgid "MANAGER - {} bookings waiting for your action"
 msgstr "RESPONSABLE - {} réservations en attente"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:449
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:450
 msgid "MANAGER - No booking accepted"
 msgstr "RESPONSABLE - Aucune réservation acceptée"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:450
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:451
 msgid "MANAGER - 1 booking accepted"
 msgstr "RESPONSABLE - 1 réservation acceptée"
 
-#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:451
+#: src/pyams_app_msc/feature/booking/zmi/dashboard.py:452
 #, python-format
 msgid "MANAGER - {} bookings accepted"
 msgstr "RESPONSABLE - {} réservations acceptées"
 
 #: src/pyams_app_msc/feature/booking/zmi/search.py:64
 #: src/pyams_app_msc/feature/booking/zmi/search.py:115
 msgid "Advanced search"
@@ -1895,37 +1918,41 @@
 
 #: src/pyams_app_msc/component/address/interfaces.py:42
 msgid "Optional observations which can be added to describe the location"
 msgstr ""
 "Observations complémentaires qui peuvent être ajoutées pour décrire "
 "l'emplacement"
 
-#: src/pyams_app_msc/component/gallery/zmi/__init__.py:59
-msgid "Set as content illustration"
-msgstr "Utiliser comme illustration du contenu"
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:79
+msgid "Set content illustration"
+msgstr "Utiliser comme illustration principale"
 
-#: src/pyams_app_msc/component/gallery/zmi/__init__.py:86
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:95
+msgid "Set navigation illustration"
+msgstr "Utiliser comme illustration de navigation"
+
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:113
 msgid "No provided object_name argument!"
 msgstr "L'argument manquant !"
 
-#: src/pyams_app_msc/component/gallery/zmi/__init__.py:95
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:122
 msgid "Given element name doesn't exist!"
 msgstr "Le nom indiqué n'existe pas !"
 
-#: src/pyams_app_msc/component/gallery/zmi/__init__.py:104
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:131
 msgid "Can't find illustration target!"
 msgstr "Impossible de trouver la cible de l'illustration !"
 
-#: src/pyams_app_msc/component/gallery/zmi/__init__.py:118
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:145
 msgid "No illustration on content!"
 msgstr "Ce contenu ne comporte pas d'illustration !"
 
-#: src/pyams_app_msc/component/gallery/zmi/__init__.py:132
-msgid "Content illustration has been updated successfully."
-msgstr "L'illustration du contenu a été modifiée avec succès."
+#: src/pyams_app_msc/component/gallery/zmi/__init__.py:159
+msgid "Illustration has been updated successfully."
+msgstr "L'illustration a été modifiée avec succès."
 
 #: src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt:15
 msgid "Gallery medias"
 msgstr "Galerie de médias"
 
 #: src/pyams_app_msc/component/contact/interfaces.py:30
 msgid "Full name"
@@ -2212,35 +2239,35 @@
 msgid "Movie theater settings"
 msgstr "Paramètres du cinéma"
 
 #: src/pyams_app_msc/shared/theater/zmi/__init__.py:243
 msgid "Main theater settings"
 msgstr "Paramètres principaux"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:263
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:264
 msgid "Booking settings"
 msgstr "Gestion des réservations"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:276
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:277
 msgid "Booking cancel mode"
 msgstr "Gestion des annulations"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:290
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:291
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 "Le délai maximum après la réservation doit être indiqué pour utiliser ce "
 "mode d'annulation !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:293
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:294
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
 "Le préavis minimum avant l'événement doit être indiqué pour utiliser ce mode "
 "d'annulation !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:302
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:303
 msgid "Quotations settings"
 msgstr "Gestion des devis"
 
 #: src/pyams_app_msc/shared/theater/zmi/price.py:60
 #: src/pyams_app_msc/shared/theater/zmi/price.py:159
 msgid "Cinema prices"
 msgstr "Gestion des tarifs"
@@ -2590,135 +2617,173 @@
 msgid ""
 "Readers are guest users which can only view theater properties and "
 "activities catalog"
 msgstr ""
 "Les invités peuvent uniquement consulter les propriétés du cinéma ainsi que "
 "le catalogue des activités"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:155
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:159
+msgid "Sunday"
+msgstr "Dimanche"
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:160
+msgid "Monday"
+msgstr "Lundi"
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:161
+msgid "Tuesday"
+msgstr "Mardi"
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:162
+msgid "Wednesday"
+msgstr "Mercredi"
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:163
+msgid "Thursday"
+msgstr "Jeudi"
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:164
+msgid "Friday"
+msgstr "Vendredi"
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:165
+msgid "Saturday"
+msgstr "Samedi"
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:183
 msgid "Forbidden cancellation"
 msgstr "Annulation impossible"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:156
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:184
 msgid "Max delay after booking"
 msgstr "Imposer un délai maximum après le dépôt de la demande"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:157
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:185
 msgid "Minimum notice period before session"
 msgstr "Imposer un préavis minimum avant le début de la séance"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:170
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:198
+msgid "Calendar first week day"
+msgstr "Premier jour de la semaine"
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:199
+msgid "First week day used in calendars"
+msgstr ""
+"Le premier jour de la semaine est utilisé pour l'affichage des semaines "
+"dans les agendas, que ce soit en mode \"mois\" ou en mode \"semaine\""
+
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:204
 msgid "Calendar slot duration"
 msgstr "Durée des créneaux horaires"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:171
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:205
 msgid "Calendar time slots frequency in week or day views"
 msgstr ""
 "Indiquée en minutes, cette valeur indique la durée des créneaux horaires "
 "affichés dans les vues par semaine ou par jour de l'agenda ; vous pouvez "
 "toujours ajuster la durée des événements plus finement, si besoin, dans le "
 "formulaire de mise à jour des propriétés d'un événement"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:177
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:211
 msgid "Default session duration"
 msgstr "Durée de base des événements"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:178
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:212
 msgid ""
 "This is a default duration, in minutes, of sessions for which activity has "
 "no duration"
 msgstr ""
 "Cette durée, exprimée en minutes, est appliquée par défaut aux événements "
 "dont l'activité n'a pas de durée indiquée"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:183
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:217
 msgid "Session duration delta"
 msgstr "Temps minimum entre les événements"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:184
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:218
 msgid ""
 "This is a number of minutes which will be added automatically to activities "
 "duration when adding new sessions"
 msgstr ""
 "Cette durée, exprimée en minutes, indique la durée qui sera ajoutée "
 "automatiquement à la durée des activités pour définir la durée des séances "
 "proposée aux gestionnaires"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:189
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:223
 msgid "Reminder delay"
 msgstr "Délai de rappel"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:190
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:224
 msgid ""
 "This is a delay, given in days before a session beginning, at which a "
 "reminder message can be sent to booking recipients; leave value empty or set "
 "it to 0 to disable reminders messages"
 msgstr ""
 "Ce délai, exprimé en jours, indique combien de temps avant le début d'une "
 "activité est attendu avant l'envoi d'un message de rappel aux bénéficiaires "
 "d'une réservation ; vous pouvez laisser cette valeur vide ou indiquer la "
 "valeur 0 si vous ne souhaitez pas envoyer de messages de rappel. ATTENTION : "
 "les réservations confirmées au-delà de ce délai ne feront pas l'objet de "
 "messages de rappel !"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:195
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:229
 msgid "User booking cancel mode"
 msgstr "Annulation des réservations"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:196
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:230
 msgid ""
 "This mode determines how and when a principal can cancel a booking by it's "
 "own way"
 msgstr ""
 "Ce paramètre indique de quelle manière un utilisateur ayant déposé une "
 "demande de réservation est à même de l'annuler par lui-même"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:202
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:236
 msgid "Cancel max delay"
 msgstr "Délai maximum après la réservation"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:203
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:237
 msgid ""
 "This is the maximum period length after user booking, given in hours, during "
 "which a principal can cancel a booking by it's own way"
 msgstr ""
 "Ce délai maximum, indiqué en heures, correspond à la durée pendant laquelle, "
 "après avoir déposé sa demande de réservation, un bénéficiaire peut encore "
 "annuler cette demande par lui-même, sans contacter le cinéma"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:209
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:243
 msgid "Cancel notice period"
 msgstr "Préavis minimum avant l'événement"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:210
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:244
 msgid ""
 "This is the minimum amount of time before session, given in hours, during "
 "which a principal can cancel a booking by it's own way"
 msgstr ""
 "Ce préavis, indiqué en heures, correspond à la durée minimale avant le début "
 "de l'événement jusqu'à laquelle un bénéficiaire peut encore annuler cette "
 "demande par lui-même, sans contacter le cinéma"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:216
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:250
 msgid "Booking retention duration"
 msgstr "Durée de rétention des réservations"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:217
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:251
 msgid ""
 "This is the minimum amount of time, given in hours, during which a a booking "
 "is kept 'active' before being archived"
 msgstr ""
 "Ceci est la durée minimale, indiquée en heures, avant qu'une réservation "
 "associée à un événement terminé ne soit archivée automatiquement"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:223
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:257
 msgid "Quotation number format"
 msgstr "Format des numéros de devis"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:224
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:258
 #, python-format
 msgid ""
 "This number will be used as formatting string to create quotations numbers; "
 "you can use date elements like {yyyy} for current year in long format, {yy} "
 "for current year in short format, {mm} for current month, {dd} for current "
 "date, {yinc} for year increment, {minc} for month increment and {operator} "
 "for operator initials"
@@ -2726,48 +2791,48 @@
 "Vous pouvez indiquer une \"chaîne de formattage\" utilisée pour générer les "
 "numéros de devis ; vous pouvez utiliser des éléments dynamiques comme {yyyy} "
 "pour indiquer l'année en cours sur quatre chiffres, {yy} pour l'année en "
 "cours sur deux chiffres, {mm} pour le mois en cours, {dd} pour le jour du "
 "mois, {yinc} pour un numéro d'incrément annuel, {minc} pour un incrément "
 "mensuel et {operator} pour les initiales de l'opérateur"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:233
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:267
 msgid "Quotation logo"
 msgstr "Logo d'en-tête"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:234
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:268
 msgid "This image will be displayed in quotations headers"
 msgstr "Cette image sera affichée dans l'en-tête des devis"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:240
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:274
 msgid "Base color"
 msgstr "Couleur de base"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:241
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:275
 msgid ""
 "This color will be used as base color for graphic elements displayed in "
 "quotations"
 msgstr ""
 "Cette couleur sera utilisée comme couleur de base pour les éléments "
 "graphiques affichés dans les devis ; si aucune couleur n'est indiquée, une "
 "couleur sera générée automatiquement à partir des couleurs du logo"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:245
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:279
 msgid "Currency"
 msgstr "Devise"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:246
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:280
 msgid "This is the currency used for all transactions"
 msgstr "Ceci est la devise utilisée pour toutes les informations monétaires"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:249
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:283
 msgid "VAT rate"
 msgstr "Taux de TVA"
 
-#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:250
+#: src/pyams_app_msc/shared/theater/interfaces/__init__.py:284
 msgid "This is the VAT rate which will be used in quotations"
 msgstr "Ceci est le taux de TVA appliqué lors de l'édition' des devis"
 
 #: src/pyams_app_msc/shared/theater/interfaces/price.py:33
 msgid "Active price?"
 msgstr "Tarif actif ?"
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/locales/pyams_app_msc.pot` & `pyams_app_msc-1.99.4/src/pyams_app_msc/locales/pyams_app_msc.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-05-05 20:34+0200\n"
+"POT-Creation-Date: 2024-05-14 22:26+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -425,21 +425,21 @@
 msgid "Enable profile"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:163
 msgid "User edit form"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:204
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:207
 msgid ""
 "Disabled profiles can't be used for website login anymore but can still be "
 "assigned new bookings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:292
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:295
 msgid "Operator profile"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt:53
 msgid "Edit user profile"
 msgstr ""
 
@@ -652,15 +652,15 @@
 
 #: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:54
 msgid "Messaging properties"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/session.py:155
 #: ./src/pyams_app_msc/feature/planning/zmi/session.py:236
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:198
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:199
 #: ./src/pyams_app_msc/shared/theater/zmi/session.py:76
 msgid "Out of catalog activity"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/session.py:160
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:180
 #, python-format
@@ -798,29 +798,29 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:129
 msgid "These comments will be displayed to the users on booking form"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:132
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:165
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:176
 #: ./src/pyams_app_msc/shared/theater/interfaces/room.py:59
 #: ./src/pyams_app_msc/shared/theater/interfaces/audience.py:58
 #: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:103
 #: ./src/pyams_app_msc/shared/theater/interfaces/price.py:62
 msgid "Notepad"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:133
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:166
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:177
 msgid "These comments are for internal use only"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:140
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:297
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:304
 msgid "Activity"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:141
 msgid ""
 "You can select an existing activity from your catalog, or keep this input "
 "empty if you just want to mark a period as not being available for booking"
@@ -885,47 +885,47 @@
 msgid "Planning"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:76
 msgid "Sessions planning"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:146
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:137
 msgid "Today"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:147
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:138
 msgid "Month"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:148
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:139
 msgid "Week"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:149
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:140
 msgid "Day"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:150
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:141
 msgid "List"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:151
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:142
 msgid "All-day"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:197
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:188
 msgid "Transpose calendars"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:210
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:201
 msgid "Synchronize calendars views"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:223
+#: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:214
 msgid "Synchronize calendars scrolling"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:13
 #: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:13
 #: ./src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt:17
 msgid "Back to previous page"
@@ -935,128 +935,128 @@
 msgid "Manage event booking..."
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:50
 msgid "Clone event..."
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:166
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:167
 msgid "QUOTATION"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:194
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:195
 msgid "#Quotation:"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:196
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:197
 msgid "Date:"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:198
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:199
 msgid "Object:"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:298
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:305
 msgid "Units"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:299
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:306
 msgid "Unit price"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:300
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:307
 msgid "Total"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:305
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:312
 #, python-format
 msgid "   - Entries ({})"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:306
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:313
 #: ./src/pyams_app_msc/feature/booking/zmi/home.py:93
 msgid "1 group"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:307
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:314
 #: ./src/pyams_app_msc/feature/booking/zmi/home.py:92
 #, python-format
 msgid "{} groups"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:314
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:321
 msgid "   - Free accompanists"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:321
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:328
 msgid "   - Paying accompanists"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:332
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:339
 msgid "Base amount"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:336
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:343
 msgid "VAT"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:340
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:347
 msgid "Total amount"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:375
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:382
 #, python-format
 msgid "Bank location: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:376
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:383
 #: ./src/pyams_app_msc/component/banking/interfaces.py:31
 msgid "Bank code"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:377
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:384
 #: ./src/pyams_app_msc/component/banking/interfaces.py:36
 msgid "Counter code"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:378
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:385
 #: ./src/pyams_app_msc/component/banking/interfaces.py:41
 msgid "Account number"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:379
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:386
 msgid "Key"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:384
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:391
 #, python-format
 msgid "IBAN: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:387
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:394
 #, python-format
 msgid "BIC: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:418
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:425
 #, python-format
 msgid "APE: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:419
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:426
 #, python-format
 msgid "SIRET: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:421
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:428
 #, python-format
 msgid "VAT: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/quotation/__init__.py:447
+#: ./src/pyams_app_msc/feature/quotation/__init__.py:454
 #, python-format
 msgid "Quotation: {}"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/reminder.py:50
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:821
 #: ./src/pyams_app_msc/shared/theater/zmi/mail.py:142
@@ -1080,36 +1080,36 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:79
 msgid "Accepted"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:109
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:242
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:243
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:126
 msgid "Creator"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:110
 msgid "Name of the principal who created the booking"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:113
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:258
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:259
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:71
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:140
 msgid "Recipient"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:114
 msgid "Name of the principal for which the booking is done"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:120
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:302
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:303
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:74
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:183
 msgid "Status"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:125
 msgid "Participants"
@@ -1120,173 +1120,187 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:130
 msgid "Accompanists"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:131
-msgid "Number of accompanists seats reserved for this session"
+msgid "Total number of accompanists seats reserved for this session"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:135
-msgid "Groups count"
+msgid "Free accompanists"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:136
+msgid "Number of free accompanists seats reserved for this session"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:144
+msgid ""
+"Number of free accompanists can't be higher than total number of "
+"accompanists!"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:146
+msgid "Groups count"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:147
 msgid "Number of groups or classrooms attending this session"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:141
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:152
 msgid "Price"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:142
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:153
 msgid "Price applied to this booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:149
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:160
 #: ./src/pyams_app_msc/shared/theater/interfaces/price.py:46
 msgid "Accompanying ratio"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:150
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:161
 msgid ""
 "You can set an integer number which will define the count of participants for"
 " which one accompanying person will have free access"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:156
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:272
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:167
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:273
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:169
 #: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:47
 msgid "Cultural pass"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:157
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:168
 msgid "Check this option if payment is done using cultural pass"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:161
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:172
 #: ./src/pyams_app_msc/feature/booking/skin/__init__.py:53
 #: ./src/pyams_app_msc/component/address/interfaces.py:41
 #: ./src/pyams_app_msc/shared/theater/interfaces/audience.py:50
 #: ./src/pyams_app_msc/shared/theater/interfaces/price.py:58
 msgid "Comments"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:162
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:173
 msgid "These comments where added by booking recipient"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:169
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:363
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:180
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:364
 msgid "Archived"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:170
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:181
 msgid ""
 "A booking is archived automatically after session end and can't be modified "
 "anymore"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:187
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:198
 msgid "Quotation number"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:188
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:199
 msgid "This is the reference number of the quotation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:191
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:202
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:748
 msgid "Quotation message"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:192
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:203
 msgid "This message is added to quotation as an information message"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:195
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:320
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:206
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:321
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:214
 msgid "Quotation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:196
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:207
 msgid "This quotation was attached to booking confirmation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:199
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:210
 msgid "Send update message?"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:200
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:211
 msgid "If 'yes', a message will be sent to the recipient "
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:204
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:215
 msgid "Update subject"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:205
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:216
 msgid "Subject of update message sent to the recipient"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:208
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:219
 msgid "Update message"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:209
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:220
 msgid ""
 "Update message will be sent to the recipient if booking properties are "
 "changed..."
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:213
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:224
 msgid "Send reminder?"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:214
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:225
 msgid ""
 "If 'yes', a reminder message will be sent to the recipient a few days before "
 "the session take place; delay before session is defined into theater settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:220
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:231
 #: ./src/pyams_app_msc/shared/theater/interfaces/mail.py:81
 msgid "Reminder subject"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:221
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:232
 msgid "Subject of reminder message sent to the recipient"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:224
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:235
 msgid "Reminder message"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:225
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:236
 msgid ""
 "Reminder message will be sent to the recipient a few days before the session "
 "take place; delay before session is defined into theater settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:230
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:241
 msgid "Reminder date"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:231
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:242
 msgid "Date and time at which reminder message was sent"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:263
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:274
 msgid "Free seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/interfaces.py:264
+#: ./src/pyams_app_msc/feature/booking/interfaces.py:275
 msgid "Number of free seats for this session"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/task.py:51
 msgid "Bookings archiver task"
 msgstr ""
 
@@ -1486,53 +1500,53 @@
 msgid "Booking dashboard"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:186
 msgid "Session"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:209
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:210
 msgid "Room"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:226
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:227
 msgid "Date"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:286
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:287
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:199
 msgid "Seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:341
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:342
 msgid "Last update"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:407
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:408
 msgid "MANAGER - No booking waiting for your action"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:408
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:409
 msgid "MANAGER - 1 booking waiting for your action"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:409
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:410
 #, python-format
 msgid "MANAGER - {} bookings waiting for your action"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:449
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:450
 msgid "MANAGER - No booking accepted"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:450
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:451
 msgid "MANAGER - 1 booking accepted"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:451
+#: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:452
 #, python-format
 msgid "MANAGER - {} bookings accepted"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:64
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:115
 msgid "Advanced search"
@@ -1762,36 +1776,40 @@
 msgid "City"
 msgstr ""
 
 #: ./src/pyams_app_msc/component/address/interfaces.py:42
 msgid "Optional observations which can be added to describe the location"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:59
-msgid "Set as content illustration"
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:79
+msgid "Set content illustration"
+msgstr ""
+
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:95
+msgid "Set navigation illustration"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:86
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:113
 msgid "No provided object_name argument!"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:95
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:122
 msgid "Given element name doesn't exist!"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:104
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:131
 msgid "Can't find illustration target!"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:118
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:145
 msgid "No illustration on content!"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:132
-msgid "Content illustration has been updated successfully."
+#: ./src/pyams_app_msc/component/gallery/zmi/__init__.py:159
+msgid "Illustration has been updated successfully."
 msgstr ""
 
 #: ./src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt:15
 msgid "Gallery medias"
 msgstr ""
 
 #: ./src/pyams_app_msc/component/contact/interfaces.py:30
@@ -2066,31 +2084,31 @@
 msgid "Movie theater settings"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:243
 msgid "Main theater settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:263
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:264
 msgid "Booking settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:276
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:277
 msgid "Booking cancel mode"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:290
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:291
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:293
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:294
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:302
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:303
 msgid "Quotations settings"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/price.py:60
 #: ./src/pyams_app_msc/shared/theater/zmi/price.py:159
 msgid "Cinema prices"
 msgstr ""
@@ -2408,150 +2426,186 @@
 
 #: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:138
 msgid ""
 "Readers are guest users which can only view theater properties and activities"
 " catalog"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:155
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:159
+msgid "Sunday"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:160
+msgid "Monday"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:161
+msgid "Tuesday"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:162
+msgid "Wednesday"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:163
+msgid "Thursday"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:164
+msgid "Friday"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:165
+msgid "Saturday"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:183
 msgid "Forbidden cancellation"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:156
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:184
 msgid "Max delay after booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:157
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:185
 msgid "Minimum notice period before session"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:170
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:198
+msgid "Calendar first week day"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:199
+msgid "First week day used in calendars"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:204
 msgid "Calendar slot duration"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:171
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:205
 msgid "Calendar time slots frequency in week or day views"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:177
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:211
 msgid "Default session duration"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:178
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:212
 msgid ""
 "This is a default duration, in minutes, of sessions for which activity has no"
 " duration"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:183
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:217
 msgid "Session duration delta"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:184
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:218
 msgid ""
 "This is a number of minutes which will be added automatically to activities "
 "duration when adding new sessions"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:189
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:223
 msgid "Reminder delay"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:190
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:224
 msgid ""
 "This is a delay, given in days before a session beginning, at which a "
 "reminder message can be sent to booking recipients; leave value empty or set "
 "it to 0 to disable reminders messages"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:195
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:229
 msgid "User booking cancel mode"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:196
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:230
 msgid ""
 "This mode determines how and when a principal can cancel a booking by it's "
 "own way"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:202
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:236
 msgid "Cancel max delay"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:203
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:237
 msgid ""
 "This is the maximum period length after user booking, given in hours, during "
 "which a principal can cancel a booking by it's own way"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:209
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:243
 msgid "Cancel notice period"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:210
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:244
 msgid ""
 "This is the minimum amount of time before session, given in hours, during "
 "which a principal can cancel a booking by it's own way"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:216
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:250
 msgid "Booking retention duration"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:217
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:251
 msgid ""
 "This is the minimum amount of time, given in hours, during which a a booking "
 "is kept 'active' before being archived"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:223
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:257
 msgid "Quotation number format"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:224
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:258
 #, python-format
 msgid ""
 "This number will be used as formatting string to create quotations numbers; "
 "you can use date elements like {yyyy} for current year in long format, {yy} "
 "for current year in short format, {mm} for current month, {dd} for current "
 "date, {yinc} for year increment, {minc} for month increment and {operator} "
 "for operator initials"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:233
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:267
 msgid "Quotation logo"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:234
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:268
 msgid "This image will be displayed in quotations headers"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:240
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:274
 msgid "Base color"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:241
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:275
 msgid ""
 "This color will be used as base color for graphic elements displayed in "
 "quotations"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:245
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:279
 msgid "Currency"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:246
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:280
 msgid "This is the currency used for all transactions"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:249
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:283
 msgid "VAT rate"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:250
+#: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:284
 msgid "This is the VAT rate which will be used in quotations"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/interfaces/price.py:33
 msgid "Active price?"
 msgstr ""
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/structure/zmi/table.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/reference/structure/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/reference/zmi/viewlet.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/reference/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/root/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/root/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/root/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/root/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/api/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/index.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/index.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/manager.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/page.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/search.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/security.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/security.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/dashboard.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/catalog/zmi/workflow.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/catalog/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/common/zmi/viewlet.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/common/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/site/zmi/viewlet.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/site/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/price.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/api/schema.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/audience.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,14 +140,42 @@
                                      role_id=MSC_READER_ROLE,
                                      required=False)
 
 
 MOVIE_THEATER_SETTINGS_KEY = 'msc.theater.settings'
 
 
+class CALENDAR_DAYS(Enum):
+    """Calendar days enumeration"""
+    SUNDAY = 0
+    MONDAY = 1
+    TUESDAY = 2
+    WEDNESDAY = 3
+    THURSDAY = 4
+    FRIDAY = 5
+    SATURDAY = 6
+
+
+CALENDAR_FIRST_DAY = OrderedDict((
+    (CALENDAR_DAYS.SUNDAY, _("Sunday")),
+    (CALENDAR_DAYS.MONDAY, _("Monday")),
+    (CALENDAR_DAYS.TUESDAY, _("Tuesday")),
+    (CALENDAR_DAYS.WEDNESDAY, _("Wednesday")),
+    (CALENDAR_DAYS.THURSDAY, _("Thursday")),
+    (CALENDAR_DAYS.FRIDAY, _("Friday")),
+    (CALENDAR_DAYS.SATURDAY, _("Saturday"))
+))
+
+
+CALENDAR_FIRST_DAY_VOCABULARY = SimpleVocabulary([
+    SimpleTerm(v.value, title=t)
+    for v, t in CALENDAR_FIRST_DAY.items()
+])
+
+
 class BOOKING_CANCEL_MODE(Enum):
     """Booking cancel modes"""
     FORBIDDEN = 'forbidden'
     MAX_DELAY = 'max-delay'
     NOTICE_PERIOD = 'notice-period'
 
 
@@ -163,14 +191,20 @@
     for v, t in BOOKING_CANCEL_MODE_LABEL.items()
 ])
 
 
 class IMovieTheaterSettings(Interface):
     """Movie theater settings"""
 
+    calendar_first_day = Choice(title=_("Calendar first week day"),
+                                description=_("First week day used in calendars"),
+                                vocabulary=CALENDAR_FIRST_DAY_VOCABULARY,
+                                required=False,
+                                default=CALENDAR_DAYS.SUNDAY.value)
+
     calendar_slot_duration = Int(title=_("Calendar slot duration"),
                                  description=_("Calendar time slots frequency in week or day views"),
                                  required=False,
                                  min=5,
                                  max=60,
                                  default=30)
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/audience.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/mail.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/price.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/interfaces/room.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/interfaces/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/mail.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/page.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/price.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/room.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/session.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/settings.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from pyams_utils.request import query_request
 
 
 @factory_config(IMovieTheaterSettings)
 class MovieTheaterSettings(Persistent, Contained):
     """Movie theater settings persistent class"""
 
+    calendar_first_day = FieldProperty(IMovieTheaterSettings['calendar_first_day'])
     calendar_slot_duration = FieldProperty(IMovieTheaterSettings['calendar_slot_duration'])
     default_session_duration = FieldProperty(IMovieTheaterSettings['default_session_duration'])
     session_duration_delta = FieldProperty(IMovieTheaterSettings['session_duration_delta'])
 
     reminder_delay = FieldProperty(IMovieTheaterSettings['reminder_delay'])
     booking_cancel_mode = FieldProperty(IMovieTheaterSettings['booking_cancel_mode'])
     booking_cancel_max_delay = FieldProperty(IMovieTheaterSettings['booking_cancel_max_delay'])
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,16 @@
                   permission=VIEW_SYSTEM_PERMISSION)
 class MovieTheaterSettingsEditForm(AdminEditForm):
     """Movie theater settings edit form"""
 
     title = _("Movie theater settings")
     legend = _("Main theater settings")
 
-    fields = Fields(IMovieTheaterSettings).select('calendar_slot_duration',
+    fields = Fields(IMovieTheaterSettings).select('calendar_first_day',
+                                                  'calendar_slot_duration',
                                                   'default_session_duration',
                                                   'session_duration_delta')
 
 
 @adapter_config(required=(IMovieTheater, IPyAMSLayer, MovieTheaterSettingsEditForm),
                 provides=IFormContent)
 def movie_theater_settings_edit_form_content(context, request, form):
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/audience.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/interfaces.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/mail.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/planning.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/planning.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/presentation.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/presentation.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/price.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/restrictions.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/room.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/search.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/session.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/types.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/types.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/shared/theater/zmi/viewlet.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/shared/theater/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/form.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/form.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/layer.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/layer.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/login.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/login.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_form.js` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_form.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_gis.js` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_gis.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_search.js` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_search.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/_utils.js` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/_utils.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/js/app.js` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/js/app.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_content.scss` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_content.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_footer.scss` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_footer.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_forms.scss` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_forms.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_layout.scss` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_layout.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_misc.scss` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_misc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/_variables.scss` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/_variables.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/resources/src/sass/msc.scss` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/resources/src/sass/msc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/skin/templates/select-admin-theater.pt` & `pyams_app_msc-1.99.4/src/pyams_app_msc/skin/templates/select-admin-theater.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/tests/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/tests/test_utilsdocs.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/tests/test_utilsdocstrings.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/__init__.py` & `pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/img/pass-culture.webp` & `pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/img/pass-culture.webp`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/msc.js` & `pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/js/msc.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -41,15 +41,15 @@
                 select = source.siblings('select'),
                 principalId = select.val();
             MyAMS.require('modal').then(() => {
                 MyAMS.modal.open(`edit-user-profile.html?principal_id=${principalId}`);
             })
         },
 
-        setIllustrationFromGallery: (evt, options) => {
+        setIllustration: (evt, options, target) => {
             const
                 source = $(evt.currentTarget),
                 sourceHtml = source.html(),
                 media = source.parents('.media-thumbnail'),
                 gallery = media.parents('.gallery'),
                 location = gallery.data('ams-location');
             MyAMS.require('ajax', 'alert', 'i18n').then(() => {
@@ -61,15 +61,15 @@
                     successLabel: MyAMS.i18n.CONFIRM,
                     cancelLabel: MyAMS.i18n.BTN_CANCEL
                 }).then((status) => {
                     if (status !== 'success') {
                         return
                     }
                     source.html('<i class="fas fa-fw fa-spinner fa-spin"></i>');
-                    MyAMS.ajax.post(`${location}/set-content-illustration.json`, {
+                    MyAMS.ajax.post(`${location}/set-${target}-illustration.json`, {
                         object_name: media.data('ams-element-name')
                     }).then((result) => {
                         MyAMS.require('alert').then(() => {
                             MyAMS.alert.smallBox({
                                 status: result.status,
                                 message: result.message,
                                 icon: 'fa-info-circle',
@@ -78,14 +78,22 @@
                             source.html(sourceHtml);
                         });
                     }).catch(() => {
                         source.html(sourceHtml);
                     });
                 });
             });
+        },
+
+        setContentIllustrationFromGallery: (evt, options) => {
+            msc.catalog.setIllustration(evt, options, 'content');
+        },
+
+        setLinkIllustrationFromGallery: (evt, options) => {
+            msc.catalog.setIllustration(evt, options, 'link');
         }
     },
 
     /**
      * Session management
      */
     session: {
@@ -126,26 +134,43 @@
         synchronized: localStorage.getItem('msc.synchronized') === 'true',
         scrolling: localStorage.getItem('msc.scrolling') === 'true',
 
         /**
          * Initialize calendar events handlers
          */
         init: (event, element, settings, veto) => {
+            settings['viewDidMount'] = MyAMS.msc.calendar.onMountedView;
             settings['eventContent'] = MyAMS.msc.calendar.setEventContent;
             settings['eventClassNames'] = MyAMS.msc.calendar.setEventClassNames;
             settings['eventDidMount'] = MyAMS.msc.calendar.renderedEvent;
             settings['dateClick'] = MyAMS.msc.calendar.addEvent;
             settings['eventClick'] = MyAMS.msc.calendar.showEvent;
             settings['eventDrop'] = MyAMS.msc.calendar.dropEvent;
             settings['eventResize'] = MyAMS.msc.calendar.resizeEvent;
             settings['eventReceive'] = MyAMS.msc.calendar.receiveEvent;
             settings['datesSet'] = MyAMS.msc.calendar.setDates;
         },
 
         /**
+         * Initialize scroll on mounted view
+         */
+        onMountedView: (evt) => {
+            if (MyAMS.msc.calendar.scrolling) {
+                const
+                    calendar = $(evt.el),
+                    scroller = $('.fc-scroller', calendar);
+                scroller.off('scroll')
+                    .on('scroll', (evt) => {
+                        const top = $(evt.currentTarget).scrollTop();
+                        $('.fc-scroller', $('.calendar tbody td')).scrollTop(top);
+                    });
+            }
+        },
+
+        /**
          * Refresh current view of calendar matching given room
          */
         refresh: (roomId, options) => {
             if (typeof(options) === 'object') {
                 roomId = options.room_id;
             }
             const calendar = $(`.calendar[data-msc-room="${roomId}"]`).data('msc-calendar');
@@ -194,22 +219,14 @@
                 if (button.exists()) {
                     button.button('toggle')
                         .toggleClass('btn-light')
                         .toggleClass('btn-link')
                         .toggleClass('btn-secondary')
                         .toggleClass('border-secondary');
                 }
-                setTimeout(() => {
-                    const scrollers = $('.fc-scroller', $('.calendar tbody td'));
-                    scrollers.off('scroll')
-                        .on('scroll', (evt) => {
-                            const top = $(evt.currentTarget).scrollTop();
-                            scrollers.scrollTop(top);
-                        });
-                }, 50);
             }
         },
 
         setEventContent: (info) => {
             const title = info.event.title.split('\n');
             return {
                 html: `<strong>${title[0]}</strong><br />${title[1] || ''}`
@@ -624,14 +641,15 @@
          */
         previewQuotation: (evt, options) => {
             MyAMS.require('ajax', 'alert').then(() => {
                 const
                     form = $(evt.currentTarget).parents('form'),
                     nb_participants = $(`input[name="form.widgets.nb_participants"]`, form).val(),
                     nb_accompanists = $(`input[name="form.widgets.nb_accompanists"]`, form).val(),
+                    nb_free_accompanists = $(`input[name="form.widgets.nb_free_accompanists"]`, form).val(),
                     price = $(`select[name="form.widgets.price"]`, form).val(),
                     ratio = $(`input[name="form.widgets.accompanying_ratio"]`, form).val();
                 if (!nb_participants ||
                     !nb_accompanists ||
                     (!price || (price === '--NOVALUE--'))) {
                     MyAMS.alert.messageBox({
                         status: 'error',
@@ -639,14 +657,15 @@
                         message: "Vous devez définir le nombre de participants et " +
                             "sélectionner un tarif pour pouvoir prévisualiser le devis..."
                     });
                 } else {
                     window.open(`${options.target}?` +
                         `nb_participants=${nb_participants}&` +
                         `nb_accompanists=${nb_accompanists}&` +
+                        `nb_free_accompanists=${nb_free_accompanists}&` +
                         `price=${price}&` +
                         `ratio=${ratio || 0}`, '_blank');
                 }
             });
         },
 
         /**
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc/zmi/resources/js/msc.min.js` & `pyams_app_msc-1.99.4/src/pyams_app_msc/zmi/resources/js/msc.min.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -19,45 +19,51 @@
             const t = $(e.currentTarget),
                 a = t.siblings("select"),
                 n = a.val();
             MyAMS.require("modal").then(() => {
                 MyAMS.modal.open("edit-user-profile.html?principal_id=" + n)
             })
         },
-        setIllustrationFromGallery: (e, t) => {
-            const a = $(e.currentTarget),
-                n = a.html(),
-                r = a.parents(".media-thumbnail"),
-                s = r.parents(".gallery"),
-                o = s.data("ams-location");
+        setIllustration: (e, t, a) => {
+            const n = $(e.currentTarget),
+                r = n.html(),
+                s = n.parents(".media-thumbnail"),
+                o = s.parents(".gallery"),
+                l = o.data("ams-location");
             MyAMS.require("ajax", "alert", "i18n").then(() => {
                 MyAMS.alert.bigBox({
                     status: "warning",
                     icon: "fas fa-bell",
                     title: MyAMS.i18n.WARNING,
                     message: "Confirmez-vous le remplacement de l'illustration ?",
                     successLabel: MyAMS.i18n.CONFIRM,
                     cancelLabel: MyAMS.i18n.BTN_CANCEL
                 }).then(e => {
-                    "success" === e && (a.html('<i class="fas fa-fw fa-spinner fa-spin"></i>'), MyAMS.ajax.post(o + "/set-content-illustration.json", {
-                        object_name: r.data("ams-element-name")
+                    "success" === e && (n.html('<i class="fas fa-fw fa-spinner fa-spin"></i>'), MyAMS.ajax.post(l + `/set-${a}-illustration.json`, {
+                        object_name: s.data("ams-element-name")
                     }).then(e => {
                         MyAMS.require("alert").then(() => {
                             MyAMS.alert.smallBox({
                                 status: e.status,
                                 message: e.message,
                                 icon: "fa-info-circle",
                                 timeout: 3e3
-                            }), a.html(n)
+                            }), n.html(r)
                         })
                     }).catch(() => {
-                        a.html(n)
+                        n.html(r)
                     }))
                 })
             })
+        },
+        setContentIllustrationFromGallery: (e, t) => {
+            msc.catalog.setIllustration(e, t, "content")
+        },
+        setLinkIllustrationFromGallery: (e, t) => {
+            msc.catalog.setIllustration(e, t, "link")
         }
     },
     session: {
         changeActivity: e => {
             $("html").attr("lang");
             const n = $(e.currentTarget).parents("form"),
                 t = $('select[name$=".widgets.activity"]', n),
@@ -71,34 +77,34 @@
         }
     },
     calendar: {
         transposed: "true" === localStorage.getItem("msc.transposed"),
         synchronized: "true" === localStorage.getItem("msc.synchronized"),
         scrolling: "true" === localStorage.getItem("msc.scrolling"),
         init: (e, t, a, n) => {
-            a.eventContent = MyAMS.msc.calendar.setEventContent, a.eventClassNames = MyAMS.msc.calendar.setEventClassNames, a.eventDidMount = MyAMS.msc.calendar.renderedEvent, a.dateClick = MyAMS.msc.calendar.addEvent, a.eventClick = MyAMS.msc.calendar.showEvent, a.eventDrop = MyAMS.msc.calendar.dropEvent, a.eventResize = MyAMS.msc.calendar.resizeEvent, a.eventReceive = MyAMS.msc.calendar.receiveEvent, a.datesSet = MyAMS.msc.calendar.setDates
+            a.viewDidMount = MyAMS.msc.calendar.onMountedView, a.eventContent = MyAMS.msc.calendar.setEventContent, a.eventClassNames = MyAMS.msc.calendar.setEventClassNames, a.eventDidMount = MyAMS.msc.calendar.renderedEvent, a.dateClick = MyAMS.msc.calendar.addEvent, a.eventClick = MyAMS.msc.calendar.showEvent, a.eventDrop = MyAMS.msc.calendar.dropEvent, a.eventResize = MyAMS.msc.calendar.resizeEvent, a.eventReceive = MyAMS.msc.calendar.receiveEvent, a.datesSet = MyAMS.msc.calendar.setDates
+        },
+        onMountedView: e => {
+            MyAMS.msc.calendar.scrolling && (e = $(e.el), $(".fc-scroller", e).off("scroll").on("scroll", e => {
+                e = $(e.currentTarget).scrollTop();
+                $(".fc-scroller", $(".calendar tbody td")).scrollTop(e)
+            }))
         },
         refresh: (e, t) => {
             "object" == typeof t && (e = t.room_id);
             t = $(`.calendar[data-msc-room="${e}"]`).data("msc-calendar");
             t && t.refetchEvents()
         },
         refreshAll: () => {
             $(".calendar").each((e, t) => {
                 $(t).data("msc-calendar").refetchEvents()
             })
         },
         afterInit: (e, t, a) => {
-            t.data("msc-calendar", a), msc.calendar.transposed && ($(".calendar-wrapper").addClass("transposed"), (t = $('a[href="MyAMS.msc.calendar.transpose"]')).exists()) && t.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), msc.calendar.synchronized && (a = $('a[href="MyAMS.msc.calendar.synchronize"]')).exists() && a.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), msc.calendar.scrolling && ((t = $('a[href="MyAMS.msc.calendar.scroll"]')).exists() && t.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), setTimeout(() => {
-                const t = $(".fc-scroller", $(".calendar tbody td"));
-                t.off("scroll").on("scroll", e => {
-                    e = $(e.currentTarget).scrollTop();
-                    t.scrollTop(e)
-                })
-            }, 50))
+            t.data("msc-calendar", a), msc.calendar.transposed && ($(".calendar-wrapper").addClass("transposed"), (t = $('a[href="MyAMS.msc.calendar.transpose"]')).exists()) && t.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), msc.calendar.synchronized && (a = $('a[href="MyAMS.msc.calendar.synchronize"]')).exists() && a.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), msc.calendar.scrolling && (t = $('a[href="MyAMS.msc.calendar.scroll"]')).exists() && t.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary")
         },
         setEventContent: e => {
             e = e.event.title.split("\n");
             return {
                 html: `<strong>${e[0]}</strong><br />` + (e[1] || "")
             }
         },
@@ -286,22 +292,23 @@
                 })) : n.val(null)
             })
         },
         changeSession: (e, t) => {
             var a;
             t.old_session !== t.new_session && (t = t.row_id, (a = (t = $(`tr[id="${t}"]`)).parents("table")).hasClass("datatable") ? a.DataTable().row(t).remove().draw() : t.remove()), MyAMS.msc.calendar.refreshAll()
         },
-        previewQuotation: (r, s) => {
+        previewQuotation: (s, o) => {
             MyAMS.require("ajax", "alert").then(() => {
-                var e = $(r.currentTarget).parents("form"),
+                var e = $(s.currentTarget).parents("form"),
                     t = $('input[name="form.widgets.nb_participants"]', e).val(),
                     a = $('input[name="form.widgets.nb_accompanists"]', e).val(),
-                    n = $('select[name="form.widgets.price"]', e).val(),
+                    n = $('input[name="form.widgets.nb_free_accompanists"]', e).val(),
+                    r = $('select[name="form.widgets.price"]', e).val(),
                     e = $('input[name="form.widgets.accompanying_ratio"]', e).val();
-                t && a && n && "--NOVALUE--" !== n ? window.open(s.target + "?" + `nb_participants=${t}&` + `nb_accompanists=${a}&` + `price=${n}&` + "ratio=" + (e || 0), "_blank") : MyAMS.alert.messageBox({
+                t && a && r && "--NOVALUE--" !== r ? window.open(o.target + "?" + `nb_participants=${t}&` + `nb_accompanists=${a}&` + `nb_free_accompanists=${n}&` + `price=${r}&` + "ratio=" + (e || 0), "_blank") : MyAMS.alert.messageBox({
                     status: "error",
                     title: "Prévisualisation impossible !",
                     message: "Vous devez définir le nombre de participants et sélectionner un tarif pour pouvoir prévisualiser le devis..."
                 })
             })
         },
         resetQuotation: (e, t) => {
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/PKG-INFO` & `pyams_app_msc-1.99.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-app-msc
-Version: 1.99.3
+Name: pyams_app_msc
+Version: 1.99.4
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -44,14 +44,24 @@
 PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.4
+------
+ - issue #27: added theater setting to set first week day displayed in calendars
+ - issue #30: updated actions used to update content illustrations from medias gallery
+ - issue #31: added free accompanists count in booking data
+ - issue #32: allow direct booking validation from creation form
+ - updated event title getter
+ - updated user profile edit form
+ - added column priority getter for use in responsive tables
+
 1.99.3
 ------
  - issue #21: added display of principal phone number
  - issue #22: updated shared content header viewlet to add button to go back to dashboard
  - issue #25: updated prompt of activity selection widget
  - issue #26: added support for vertical synchronization of calendars
  - issue #27: removed theater week view from calendar
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/SOURCES.txt` & `pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -133,24 +133,26 @@
 src/pyams_app_msc/component/duration/__init__.py
 src/pyams_app_msc/component/duration/interfaces.py
 src/pyams_app_msc/component/duration/schema.py
 src/pyams_app_msc/component/duration/zmi/__init__.py
 src/pyams_app_msc/component/duration/zmi/interfaces.py
 src/pyams_app_msc/component/gallery/__init__.py
 src/pyams_app_msc/component/gallery/zmi/__init__.py
+src/pyams_app_msc/component/gallery/zmi/interfaces.py
 src/pyams_app_msc/component/gallery/zmi/templates/gallery-medias.pt
 src/pyams_app_msc/component/gallery/zmi/templates/gallery-view.pt
 src/pyams_app_msc/component/paragraph/__init__.py
 src/pyams_app_msc/component/paragraph/zmi/__init__.py
 src/pyams_app_msc/component/paragraph/zmi/container.py
 src/pyams_app_msc/doctests/README.rst
 src/pyams_app_msc/feature/__init__.py
 src/pyams_app_msc/feature/booking/__init__.py
 src/pyams_app_msc/feature/booking/container.py
 src/pyams_app_msc/feature/booking/interfaces.py
+src/pyams_app_msc/feature/booking/message.py
 src/pyams_app_msc/feature/booking/reminder.py
 src/pyams_app_msc/feature/booking/task.py
 src/pyams_app_msc/feature/booking/skin/__init__.py
 src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
 src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
 src/pyams_app_msc/feature/booking/zmi/__init__.py
 src/pyams_app_msc/feature/booking/zmi/dashboard.py
```

### Comparing `pyams_app_msc-1.99.3/src/pyams_app_msc.egg-info/requires.txt` & `pyams_app_msc-1.99.4/src/pyams_app_msc.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 pyams_sequence
 pyams_site
 pyams_skin
 pyams_table
 pyams_utils>=2.3.1
 pyams_viewlet
 pyams_workflow
-pyams_zmi
+pyams_zmi>=2.3.1
 pyams_zmq
 pyramid
 pyramid_mailer
 reportlab
 requests
 transaction
 ZODB
```

