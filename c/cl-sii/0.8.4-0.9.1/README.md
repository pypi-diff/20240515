# Comparing `tmp/cl-sii-0.8.4.tar.gz` & `tmp/cl-sii-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cl-sii-0.8.4.tar", last modified: Thu Feb  6 22:28:10 2020, max compression
+gzip compressed data, was "dist/cl-sii-0.9.1.tar", last modified: Fri Mar 20 23:26:38 2020, max compression
```

## Comparing `cl-sii-0.8.4.tar` & `cl-sii-0.9.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/
--rw-r--r--   0 root         (0) root         (0)     5275 2020-02-06 22:27:52.000000 cl-sii-0.8.4/HISTORY.rst
--rw-r--r--   0 root         (0) root         (0)     1071 2020-02-06 22:27:52.000000 cl-sii-0.8.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      241 2020-02-06 22:27:52.000000 cl-sii-0.8.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9833 2020-02-06 22:28:10.000000 cl-sii-0.8.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1968 2020-02-06 22:27:52.000000 cl-sii-0.8.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/
--rw-r--r--   0 root         (0) root         (0)       69 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/base/
--rw-r--r--   0 root         (0) root         (0)        0 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      203 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/base/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/contribuyente/
--rw-r--r--   0 root         (0) root         (0)        0 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/contribuyente/__init__.py
--rw-r--r--   0 root         (0) root         (0)      504 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/contribuyente/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/cte/
--rw-r--r--   0 root         (0) root         (0)      969 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/cte/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/cte/f29/
--rw-r--r--   0 root         (0) root         (0)      163 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/cte/f29/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13753 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/cte/f29/data_models.py
--rw-r--r--   0 root         (0) root         (0)     4473 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/cte/f29/parse_datos_obj.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/data/cte/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/data/cte/schemas-json/
--rw-r--r--   0 root         (0) root         (0)     3447 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/cte/schemas-json/f29_datos_obj.schema.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/data/ref/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/
--rw-r--r--   0 root         (0) root         (0)     3962 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/AEC_v10.xsd
--rw-r--r--   0 root         (0) root         (0)     9034 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/Cesion_v10.xsd
--rw-r--r--   0 root         (0) root         (0)     2619 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/DTECedido_v10.xsd
--rw-r--r--   0 root         (0) root         (0)   232527 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/DTE_v10.xsd
--rw-r--r--   0 root         (0) root         (0)     4738 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/EnvioDTE_v10.xsd
--rw-r--r--   0 root         (0) root         (0)     6000 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/LceCal_v10.xsd
--rw-r--r--   0 root         (0) root         (0)     2518 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/LceCoCertif_v10.xsd
--rw-r--r--   0 root         (0) root         (0)     9604 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/LceSiiTypes_v10.xsd
--rw-r--r--   0 root         (0) root         (0)    72177 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/LibroCV_v10.xsd
--rw-r--r--   0 root         (0) root         (0)     4202 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/Recibos_v10.xsd
--rw-r--r--   0 root         (0) root         (0)    30967 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/SiiTypes_v10.xsd
--rw-r--r--   0 root         (0) root         (0)     7135 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/xmldsignature_v10.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/dte/
--rw-r--r--   0 root         (0) root         (0)        0 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/dte/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8169 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/dte/constants.py
--rw-r--r--   0 root         (0) root         (0)    14583 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/dte/data_models.py
--rw-r--r--   0 root         (0) root         (0)    21288 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/dte/parse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/extras/
--rw-r--r--   0 root         (0) root         (0)        0 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/extras/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6468 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/extras/dj_model_fields.py
--rw-r--r--   0 root         (0) root         (0)     2123 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/extras/drf_fields.py
--rw-r--r--   0 root         (0) root         (0)     7376 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/extras/mm_fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/libs/
--rw-r--r--   0 root         (0) root         (0)       87 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4643 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/crypto_utils.py
--rw-r--r--   0 root         (0) root         (0)     1834 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/csv_utils.py
--rw-r--r--   0 root         (0) root         (0)     3475 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/dataclass_utils.py
--rw-r--r--   0 root         (0) root         (0)     1775 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/encoding_utils.py
--rw-r--r--   0 root         (0) root         (0)     2234 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/io_utils.py
--rw-r--r--   0 root         (0) root         (0)     1342 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/json_utils.py
--rw-r--r--   0 root         (0) root         (0)     4767 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/mm_utils.py
--rw-r--r--   0 root         (0) root         (0)     6091 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/rows_processing.py
--rw-r--r--   0 root         (0) root         (0)     5297 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/tz_utils.py
--rw-r--r--   0 root         (0) root         (0)    17704 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/libs/xml_utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/rcv/
--rw-r--r--   0 root         (0) root         (0)      392 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/rcv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9341 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/rcv/constants.py
--rw-r--r--   0 root         (0) root         (0)    10753 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/rcv/data_models.py
--rw-r--r--   0 root         (0) root         (0)    42985 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/rcv/parse_csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii/rut/
--rw-r--r--   0 root         (0) root         (0)     5979 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/rut/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2020-02-06 22:27:52.000000 cl-sii-0.8.4/cl_sii/rut/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9833 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1978 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      233 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2020-02-06 22:28:10.000000 cl-sii-0.8.4/cl_sii.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1182 2020-02-06 22:28:10.000000 cl-sii-0.8.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     3243 2020-02-06 22:27:52.000000 cl-sii-0.8.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     5661 2020-03-20 23:25:54.000000 cl-sii-0.9.1/HISTORY.rst
+-rw-r--r--   0 root         (0) root         (0)     1071 2020-03-20 23:25:54.000000 cl-sii-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      241 2020-03-20 23:25:54.000000 cl-sii-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10315 2020-03-20 23:26:38.000000 cl-sii-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1968 2020-03-20 23:25:54.000000 cl-sii-0.9.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/
+-rw-r--r--   0 root         (0) root         (0)       69 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      203 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/base/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/contribuyente/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/contribuyente/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      504 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/contribuyente/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/cte/
+-rw-r--r--   0 root         (0) root         (0)      969 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/cte/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/cte/f29/
+-rw-r--r--   0 root         (0) root         (0)      163 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/cte/f29/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13864 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/cte/f29/data_models.py
+-rw-r--r--   0 root         (0) root         (0)     6106 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/cte/f29/parse_datos_obj.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/data/cte/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/data/cte/schemas-json/
+-rw-r--r--   0 root         (0) root         (0)     3457 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/cte/schemas-json/f29_datos_obj.schema.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/data/ref/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/
+-rw-r--r--   0 root         (0) root         (0)     3962 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/AEC_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)     9034 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/Cesion_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)     2619 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/DTECedido_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)   232527 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/DTE_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)     4738 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/EnvioDTE_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)     6000 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/LceCal_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)     2518 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/LceCoCertif_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)     9604 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/LceSiiTypes_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)    72177 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/LibroCV_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)     4202 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/Recibos_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)    30967 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/SiiTypes_v10.xsd
+-rw-r--r--   0 root         (0) root         (0)     7135 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/xmldsignature_v10.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/dte/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/dte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8169 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/dte/constants.py
+-rw-r--r--   0 root         (0) root         (0)    14583 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/dte/data_models.py
+-rw-r--r--   0 root         (0) root         (0)    21288 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/dte/parse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/extras/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/extras/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6468 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/extras/dj_model_fields.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/extras/drf_fields.py
+-rw-r--r--   0 root         (0) root         (0)     7376 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/extras/mm_fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/libs/
+-rw-r--r--   0 root         (0) root         (0)       87 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4643 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/crypto_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/csv_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3475 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/dataclass_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/encoding_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/io_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1342 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/json_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4767 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/mm_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6091 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/rows_processing.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/tz_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17704 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/libs/xml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/rcv/
+-rw-r--r--   0 root         (0) root         (0)      392 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/rcv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9341 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/rcv/constants.py
+-rw-r--r--   0 root         (0) root         (0)    10753 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/rcv/data_models.py
+-rw-r--r--   0 root         (0) root         (0)    42985 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/rcv/parse_csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii/rut/
+-rw-r--r--   0 root         (0) root         (0)     5979 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/rut/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2020-03-20 23:25:54.000000 cl-sii-0.9.1/cl_sii/rut/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-20 23:26:38.000000 cl-sii-0.9.1/cl_sii.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10315 2020-03-20 23:26:37.000000 cl-sii-0.9.1/cl_sii.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1978 2020-03-20 23:26:37.000000 cl-sii-0.9.1/cl_sii.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-03-20 23:26:37.000000 cl-sii-0.9.1/cl_sii.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-03-20 23:26:37.000000 cl-sii-0.9.1/cl_sii.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      233 2020-03-20 23:26:37.000000 cl-sii-0.9.1/cl_sii.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2020-03-20 23:26:37.000000 cl-sii-0.9.1/cl_sii.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1182 2020-03-20 23:26:38.000000 cl-sii-0.9.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     3243 2020-03-20 23:25:54.000000 cl-sii-0.9.1/setup.py
```

### Comparing `cl-sii-0.8.4/HISTORY.rst` & `cl-sii-0.9.1/HISTORY.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 .. :changelog:
 
 History
 -------
 
+0.9.1 (2020-03-20)
++++++++++++++++++++++++
+
+* Fix incorrect version used in the previous release's changelog.
+
+0.9.0 (2020-03-20)
++++++++++++++++++++++++
+
+* (PR #104, 2020-02-27) cte.f29.parser: Rename custom validator and deserializer parameters
+* (PR #97, 2020-02-25) cte: Allow four digit Form 29 codes
+* (PR #103, 2020-02-24) cte: Add custom validators and deserializers to parser
+
 0.8.4 (2020-02-06)
 +++++++++++++++++++++++
 
 * (PR #100, 2020-02-06) Update everything for Fyntex, the new owner
 
 0.8.3 (2020-02-06)
 +++++++++++++++++++++++
```

### Comparing `cl-sii-0.8.4/LICENSE` & `cl-sii-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/PKG-INFO` & `cl-sii-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cl-sii
-Version: 0.8.4
+Version: 0.9.1
 Summary: Python library for Servicio de Impuestos Internos (SII) of Chile.
 Home-page: https://github.com/fyntex/lib-cl-sii-python
 Author: Fyntex TI SpA
 Author-email: no-reply@fyntex.ai
 License: MIT
 Description: =================
         cl-sii Python lib
@@ -88,14 +88,26 @@
         
         
         
         
         History
         -------
         
+        0.9.1 (2020-03-20)
+        +++++++++++++++++++++++
+        
+        * Fix incorrect version used in the previous release's changelog.
+        
+        0.9.0 (2020-03-20)
+        +++++++++++++++++++++++
+        
+        * (PR #104, 2020-02-27) cte.f29.parser: Rename custom validator and deserializer parameters
+        * (PR #97, 2020-02-25) cte: Allow four digit Form 29 codes
+        * (PR #103, 2020-02-24) cte: Add custom validators and deserializers to parser
+        
         0.8.4 (2020-02-06)
         +++++++++++++++++++++++
         
         * (PR #100, 2020-02-06) Update everything for Fyntex, the new owner
         
         0.8.3 (2020-02-06)
         +++++++++++++++++++++++
```

### Comparing `cl-sii-0.8.4/README.rst` & `cl-sii-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/cte/__init__.py` & `cl-sii-0.9.1/cl_sii/cte/__init__.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/cte/f29/data_models.py` & `cl-sii-0.9.1/cl_sii/cte/f29/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
         563: None,  # "BASE IMPONIBLE"
         564: None,  # "CANT. DOC. SIN DER. A CRED. FISCAL"
         584: None,  # "CANT.INT.EX.NO GRAV.SIN DER. CRED.FISCAL"
         585: None,  # Exportaciones | Cantidad
         586: None,  # "CANT. VTAS. Y/O SERV. PREST. INT. EXENT."
         587: None,  # Facturas de Compra recibidas c/ret. total y Fact. de Inicio emitida | Monto
         595: None,  # "SUB TOTAL IMP. DETERMINADO ANVERSO"
+        596: None,  # "RETENCION CAMBIO DE SUJETO"
         601: None,  # Fax
         610: 'numero_direccion',  # Nº Dirección
         708: None,  # "CANT. NOTAS CRED. EMIT. VALES MAQ. IVA"
         709: None,  # "MONTO NOTAS CRED. EMIT. VALES MAQ. IVA."
         755: None,  # IVA Postergado
         756: None,  # Casillero (checkbox) "Postergación pago de IVA"
         761: None,  # "CANT. FACT. SUPERMERCADOS Y SIMILARES"
@@ -163,14 +164,15 @@
         763: None,  # "CANT. FACT. POR VENTA BIENES INMUEBLES"
         764: None,  # "DÉB. FACT. POR VENTA BIENES INMUEBLES"
         765: None,  # "CANT. FACT. ADQ. O CONSTR. B. INMUEBLES"
         766: None,  # "DÉB. FACT. ADQ. O CONSTR. B. INMUEBLES"
         795: None,  # "MONTO DE CONDONACION SII"
         915: 'fecha_condonacion',  # "Fecha de Vigencia de Condonacion"
         922: 'num_res_condonacion',  # "NUMERO RESOLUCION SII AUTO. CONDONACION"
+        9906: None,  # "FECHA PRESENTACION DECL. PRIMITIVA"
     }
 
     def __post_init__(self) -> None:
         # -----Set Fields from Extra-----
 
         new_extra: MutableMapping[int, object] = {}
```

### Comparing `cl-sii-0.8.4/cl_sii/cte/f29/parse_datos_obj.py` & `cl-sii-0.9.1/cl_sii/cte/f29/parse_datos_obj.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from datetime import datetime
 from decimal import Decimal
 from pathlib import Path
-from typing import Mapping, MutableMapping
+from typing import Callable, Mapping, MutableMapping, Optional
 
 import jsonschema
 
 from cl_sii.libs.json_utils import JsonSchemaValidationError, read_json_schema
 from cl_sii.rut import Rut
 from cl_sii.rcv.data_models import PeriodoTributario
 
@@ -18,49 +18,72 @@
 _CTE_F29_DATOS_OBJ_SCHEMA_PATH = (
     Path(__file__).parent.parent.parent
     / 'data' / 'cte' / 'schemas-json' / 'f29_datos_obj.schema.json'
 )
 CTE_F29_DATOS_OBJ_SCHEMA = read_json_schema(_CTE_F29_DATOS_OBJ_SCHEMA_PATH)
 
 
-def parse_sii_cte_f29_datos_obj(datos_obj: SiiCteF29DatosObjType) -> CteForm29:
+def parse_sii_cte_f29_datos_obj(
+    datos_obj: SiiCteF29DatosObjType,
+    schema_validator: Optional[Callable[[SiiCteF29DatosObjType], None]] = None,
+    campo_deserializer: Optional[Callable[[object, str], object]] = None,
+) -> CteForm29:
     """
     Parse the ``datos`` JavaScript object embedded in the IFrames of the
     HTML version of the CTE's 'Declaraciones de IVA (F29)'.
 
+    :param schema_validator: Schema validator. For the signature of the callable, see the docstring
+        of ``cte_f29_datos_schema_default_validator``.
+    :param campo_deserializer: 'Campo' deserializer. For the signature of the callable, see the
+        docstring of ``cte_f29_datos_obj_campo_default_deserializer``.
     :raises JsonSchemaValidationError: If schema validation fails.
     """
-    obj_params = _parse_sii_cte_f29_datos_obj_to_dict(datos_obj=datos_obj)
+    if schema_validator is None:
+        schema_validator = cte_f29_datos_schema_default_validator
+    if campo_deserializer is None:
+        campo_deserializer = cte_f29_datos_obj_campo_default_deserializer
+
+    obj_params = _parse_sii_cte_f29_datos_obj_to_dict(
+        datos_obj=datos_obj,
+        schema_validator=schema_validator,
+        campo_deserializer=campo_deserializer,
+    )
     obj = CteForm29(**obj_params)
     return obj
 
 
-def _parse_sii_cte_f29_datos_obj_to_dict(datos_obj: SiiCteF29DatosObjType) -> Mapping[str, object]:
+def _parse_sii_cte_f29_datos_obj_to_dict(
+    datos_obj: SiiCteF29DatosObjType,
+    schema_validator: Callable[[SiiCteF29DatosObjType], None],
+    campo_deserializer: Callable[[object, str], object],
+) -> Mapping[str, object]:
     """
     Parse the ``datos`` JavaScript object embedded in the IFrames of the
     HTML version of the CTE's 'Declaraciones de IVA (F29)' and return a
     dictionary.
 
+    :param schema_validator:
+    :param campo_deserializer:
     :raises JsonSchemaValidationError: If schema validation fails.
     """
-    _validate_cte_f29_datos_schema(datos_obj=datos_obj)
+    schema_validator(datos_obj)
 
     datos_obj_campos: Mapping[int, str] = {
         int(code): str(value) for code, value in datos_obj['campos'].items()
     }
     datos_obj_extras: Mapping[str, object] = datos_obj['extras']
     datos_obj_glosa: Mapping[int, str] = {  # noqa: F841
         int(code): str(value) for code, value in datos_obj['glosa'].items()
     }
     datos_obj_tipos: Mapping[int, str] = {
         int(code): str(value) for code, value in datos_obj['tipos'].items()
     }
 
     deserialized_datos_obj_campos = {
-        code: _deserialize_cte_f29_datos_obj_campo(campo_value=value, tipo=datos_obj_tipos[code])
+        code: campo_deserializer(value, datos_obj_tipos[code])
         for code, value in datos_obj_campos.items()
     }
 
     obj_extra: MutableMapping[int, object] = {}
     for code, value in deserialized_datos_obj_campos.items():
         obj_extra[code] = value
 
@@ -78,21 +101,22 @@
         medio_pago=datos_obj_extras.get('MEDIO_PAGO'),
 
         extra=obj_extra,
     )
     return obj_dict
 
 
-def _deserialize_cte_f29_datos_obj_campo(campo_value: object, tipo: str) -> object:
+def cte_f29_datos_obj_campo_default_deserializer(campo_value: object, tipo: str) -> object:
     """
     Convert raw values from the ``datos`` object to the corresponding Python
     data type.
 
     :param campo_value: Raw value from 'campos'.
     :param tipo: Data type code from 'tipos'.
+    :raises ValueError: If value conversion fails.
     """
     if not isinstance(campo_value, str):
         return campo_value
 
     deserialized_value: object
 
     if tipo == 'R':
@@ -107,15 +131,34 @@
         deserialized_value = Decimal(campo_value)
     else:
         raise ValueError(f"Invalid or unknown tipo of campo: '{tipo}'")
 
     return deserialized_value
 
 
-def _validate_cte_f29_datos_schema(datos_obj: SiiCteF29DatosObjType) -> None:
+def cte_f29_datos_obj_campo_best_effort_deserializer(campo_value: object, tipo: str) -> object:
+    """
+    Convert raw values from the ``datos`` object to the corresponding Python
+    data type. Values that cannot be converted will be returned without modification.
+
+    :param campo_value: Raw value from 'campos'.
+    :param tipo: Data type code from 'tipos'.
+    """
+    try:
+        deserialized_value = cte_f29_datos_obj_campo_default_deserializer(
+            campo_value=campo_value,
+            tipo=tipo,
+        )
+    except Exception:
+        deserialized_value = campo_value
+
+    return deserialized_value
+
+
+def cte_f29_datos_schema_default_validator(datos_obj: SiiCteF29DatosObjType) -> None:
     """
     Validate the ``datos`` object against the schema.
 
     :raises JsonSchemaValidationError: If schema validation fails.
     :returns: ``None`` if schema validation passed.
     """
     try:
```

### Comparing `cl-sii-0.8.4/cl_sii/data/cte/schemas-json/f29_datos_obj.schema.json` & `cl-sii-0.9.1/cl_sii/data/cte/schemas-json/f29_datos_obj.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950396825396824%*

 * *Differences: {"'properties'": "{'campos': {'patternProperties': {replace: OrderedDict([('^\\\\d{3,4}$', "*

 * *                 "OrderedDict([('type', 'string')]))])}}, 'glosa': {'patternProperties': {replace: "*

 * *                 "OrderedDict([('^\\\\d{3,4}$', OrderedDict([('type', 'string')]))])}}, 'justif': "*

 * *                 "{'patternProperties': {replace: OrderedDict([('^\\\\d{3,4}$', "*

 * *                 "OrderedDict([('type', 'string'), ('enum', ['I', 'D', '-'])]))])}}, 'linea': "*

 * *                 "{'patternProperties':  […]*

```diff
@@ -1,15 +1,15 @@
 {
     "additionalProperties": true,
     "description": "Schema of (a subset of) the 'datos' JavaScript object embedded in the IFrames of the HTML version of the CTE's 'Declaraciones de IVA (F29)'.",
     "properties": {
         "campos": {
             "additionalProperties": false,
             "patternProperties": {
-                "^\\d{3}$": {
+                "^\\d{3,4}$": {
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "extras": {
             "additionalProperties": false,
@@ -103,48 +103,48 @@
         },
         "folioF": {
             "type": "object"
         },
         "glosa": {
             "additionalProperties": false,
             "patternProperties": {
-                "^\\d{3}$": {
+                "^\\d{3,4}$": {
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "justif": {
             "additionalProperties": false,
             "patternProperties": {
-                "^\\d{3}$": {
+                "^\\d{3,4}$": {
                     "enum": [
                         "I",
                         "D",
                         "-"
                     ],
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "linea": {
             "additionalProperties": false,
             "patternProperties": {
-                "^\\d{3}$": {
+                "^\\d{3,4}$": {
                     "pattern": "^\\d+$",
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "tipos": {
             "additionalProperties": false,
             "patternProperties": {
-                "^\\d{3}$": {
+                "^\\d{3,4}$": {
                     "enum": [
                         "C",
                         "D",
                         "F",
                         "M",
                         "N",
                         "R"
```

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/AEC_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/AEC_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/Cesion_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/Cesion_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/DTECedido_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/DTECedido_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/DTE_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/DTE_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/EnvioDTE_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/EnvioDTE_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/LceCal_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/LceCal_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/LceCoCertif_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/LceCoCertif_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/LceSiiTypes_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/LceSiiTypes_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/LibroCV_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/LibroCV_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/Recibos_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/Recibos_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/SiiTypes_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/SiiTypes_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/data/ref/factura_electronica/schemas-xml/xmldsignature_v10.xsd` & `cl-sii-0.9.1/cl_sii/data/ref/factura_electronica/schemas-xml/xmldsignature_v10.xsd`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/dte/constants.py` & `cl-sii-0.9.1/cl_sii/dte/constants.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/dte/data_models.py` & `cl-sii-0.9.1/cl_sii/dte/data_models.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/dte/parse.py` & `cl-sii-0.9.1/cl_sii/dte/parse.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/extras/dj_model_fields.py` & `cl-sii-0.9.1/cl_sii/extras/dj_model_fields.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/extras/drf_fields.py` & `cl-sii-0.9.1/cl_sii/extras/drf_fields.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/extras/mm_fields.py` & `cl-sii-0.9.1/cl_sii/extras/mm_fields.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/crypto_utils.py` & `cl-sii-0.9.1/cl_sii/libs/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/csv_utils.py` & `cl-sii-0.9.1/cl_sii/libs/csv_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/dataclass_utils.py` & `cl-sii-0.9.1/cl_sii/libs/dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/encoding_utils.py` & `cl-sii-0.9.1/cl_sii/libs/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/io_utils.py` & `cl-sii-0.9.1/cl_sii/libs/io_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/json_utils.py` & `cl-sii-0.9.1/cl_sii/libs/json_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/mm_utils.py` & `cl-sii-0.9.1/cl_sii/libs/mm_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/rows_processing.py` & `cl-sii-0.9.1/cl_sii/libs/rows_processing.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/tz_utils.py` & `cl-sii-0.9.1/cl_sii/libs/tz_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/libs/xml_utils.py` & `cl-sii-0.9.1/cl_sii/libs/xml_utils.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/rcv/constants.py` & `cl-sii-0.9.1/cl_sii/rcv/constants.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/rcv/data_models.py` & `cl-sii-0.9.1/cl_sii/rcv/data_models.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/rcv/parse_csv.py` & `cl-sii-0.9.1/cl_sii/rcv/parse_csv.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/rut/__init__.py` & `cl-sii-0.9.1/cl_sii/rut/__init__.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii/rut/constants.py` & `cl-sii-0.9.1/cl_sii/rut/constants.py`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/cl_sii.egg-info/PKG-INFO` & `cl-sii-0.9.1/cl_sii.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cl-sii
-Version: 0.8.4
+Version: 0.9.1
 Summary: Python library for Servicio de Impuestos Internos (SII) of Chile.
 Home-page: https://github.com/fyntex/lib-cl-sii-python
 Author: Fyntex TI SpA
 Author-email: no-reply@fyntex.ai
 License: MIT
 Description: =================
         cl-sii Python lib
@@ -88,14 +88,26 @@
         
         
         
         
         History
         -------
         
+        0.9.1 (2020-03-20)
+        +++++++++++++++++++++++
+        
+        * Fix incorrect version used in the previous release's changelog.
+        
+        0.9.0 (2020-03-20)
+        +++++++++++++++++++++++
+        
+        * (PR #104, 2020-02-27) cte.f29.parser: Rename custom validator and deserializer parameters
+        * (PR #97, 2020-02-25) cte: Allow four digit Form 29 codes
+        * (PR #103, 2020-02-24) cte: Add custom validators and deserializers to parser
+        
         0.8.4 (2020-02-06)
         +++++++++++++++++++++++
         
         * (PR #100, 2020-02-06) Update everything for Fyntex, the new owner
         
         0.8.3 (2020-02-06)
         +++++++++++++++++++++++
```

### Comparing `cl-sii-0.8.4/cl_sii.egg-info/SOURCES.txt` & `cl-sii-0.9.1/cl_sii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/setup.cfg` & `cl-sii-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cl-sii-0.8.4/setup.py` & `cl-sii-0.9.1/setup.py`

 * *Files identical despite different names*

