# Comparing `tmp/eodc_faas_sen2like-2024.5.0.tar.gz` & `tmp/eodc_faas_sen2like-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_sen2like-2024.5.0.tar", max compression
+gzip compressed data, was "eodc_faas_sen2like-2024.5.1.tar", max compression
```

## Comparing `eodc_faas_sen2like-2024.5.0.tar` & `eodc_faas_sen2like-2024.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2024.5.0/README.md
--rw-r--r--   0        0        0      637 2024-05-06 07:12:34.168000 eodc_faas_sen2like-2024.5.0/pyproject.toml
--rw-r--r--   0        0        0      105 2024-05-06 07:12:34.168000 eodc_faas_sen2like-2024.5.0/sen2like_processor_bindings/__init__.py
--rw-r--r--   0        0        0     3011 2024-02-23 14:12:59.060000 eodc_faas_sen2like-2024.5.0/sen2like_processor_bindings/model.py
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2024.5.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2024.5.1/README.md
+-rw-r--r--   0        0        0      637 2024-05-15 05:55:53.508000 eodc_faas_sen2like-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0      105 2024-05-15 05:55:53.508000 eodc_faas_sen2like-2024.5.1/sen2like_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     3054 2024-05-15 05:53:27.460000 eodc_faas_sen2like-2024.5.1/sen2like_processor_bindings/model.py
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2024.5.1/PKG-INFO
```

### Comparing `eodc_faas_sen2like-2024.5.0/pyproject.toml` & `eodc_faas_sen2like-2024.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-sen2like"
-version = "2024.5.0"
+version = "2024.5.1"
 description = "Bindings for the sen2like processor exposed at EODC"
 authors = ["Valentina Hutter <valentina.hutter@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "sen2like_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_sen2like-2024.5.0/sen2like_processor_bindings/model.py` & `eodc_faas_sen2like-2024.5.1/sen2like_processor_bindings/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         for item in tile.iterdir():
             if (
                 item.suffix == ".SAFE"
                 and target_product.upper() in item.name
                 and (item.name.startswith("S2") or item.name.startswith("LS"))
             ):  # result either L2F or L2H
                 item_path = item / (item.stem + ".json")
-                stac_item_paths.append(item_path)
+                if item_path.exists():
+                    stac_item_paths.append(item_path)
 
     logger.info(
         f"Found {len(stac_item_paths)} STAC items in {sen2like_parameters.output_path}"
     )
 
     return stac_item_paths
```

### Comparing `eodc_faas_sen2like-2024.5.0/PKG-INFO` & `eodc_faas_sen2like-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-sen2like
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Bindings for the sen2like processor exposed at EODC
 Author: Valentina Hutter
 Author-email: valentina.hutter@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

