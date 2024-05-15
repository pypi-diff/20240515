# Comparing `tmp/netbox-qrcode-0.0.8.tar.gz` & `tmp/netbox-qrcode-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netbox-qrcode/netbox-qrcode/dist/tmptcg4ohwh/netbox-qrcode-0.0.8.tar", last modified: Tue Nov 15 13:11:32 2022, max compression
+gzip compressed data, was "/home/runner/work/netbox-qrcode/netbox-qrcode/dist/.tmp-e74chgjg/netbox-qrcode-0.0.9.tar", last modified: Wed Feb  8 05:06:37 2023, max compression
```

## Comparing `netbox-qrcode-0.0.8.tar` & `netbox-qrcode-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)    10173 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       92 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4277 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3808 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode/
--rw-r--r--   0 runner    (1001) docker     (116)     1199 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode/fonts/
--rw-r--r--   0 runner    (1001) docker     (116)   122556 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/fonts/ArialBlack.ttf
--rw-r--r--   0 runner    (1001) docker     (116)   710044 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/fonts/ArialMT.ttf
--rw-r--r--   0 runner    (1001) docker     (116)   120120 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/fonts/ComicSansMSBold.ttf
--rw-r--r--   0 runner    (1001) docker     (116)   691796 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/fonts/CourierNewBold.ttf
--rw-r--r--   0 runner    (1001) docker     (116)   681120 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/fonts/Tahoma.ttf
--rw-r--r--   0 runner    (1001) docker     (116)   626928 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/fonts/TahomaBold.ttf
--rw-r--r--   0 runner    (1001) docker     (116)     3320 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode/templates/netbox_qrcode/
--rw-r--r--   0 runner    (1001) docker     (116)      694 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/templates/netbox_qrcode/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (116)      682 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/templates/netbox_qrcode/qrcode3.html
--rw-r--r--   0 runner    (1001) docker     (116)     2885 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/utilities.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/netbox_qrcode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4277 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      647 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/netbox_qrcode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-15 13:11:32.000000 netbox-qrcode-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1352 2022-11-15 13:11:23.000000 netbox-qrcode-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    10173 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       92 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     4570 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4101 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode/
+-rw-r--r--   0 runner    (1001) docker     (116)     1199 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode/fonts/
+-rw-r--r--   0 runner    (1001) docker     (116)   122556 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/fonts/ArialBlack.ttf
+-rw-r--r--   0 runner    (1001) docker     (116)   710044 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/fonts/ArialMT.ttf
+-rw-r--r--   0 runner    (1001) docker     (116)   120120 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/fonts/ComicSansMSBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (116)   691796 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/fonts/CourierNewBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (116)   681120 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/fonts/Tahoma.ttf
+-rw-r--r--   0 runner    (1001) docker     (116)   626928 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/fonts/TahomaBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (116)     3703 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode/templates/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode/templates/netbox_qrcode/
+-rw-r--r--   0 runner    (1001) docker     (116)      694 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/templates/netbox_qrcode/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (116)      682 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/templates/netbox_qrcode/qrcode3.html
+-rw-r--r--   0 runner    (1001) docker     (116)     2885 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/netbox_qrcode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4570 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      647 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/netbox_qrcode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-08 05:06:37.000000 netbox-qrcode-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1352 2023-02-08 05:06:27.000000 netbox-qrcode-0.0.9/setup.py
```

### Comparing `netbox-qrcode-0.0.8/LICENSE` & `netbox-qrcode-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/PKG-INFO` & `netbox-qrcode-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-qrcode
-Version: 0.0.8
+Version: 0.0.9
 Summary: QR Code generation for netbox objects
 Home-page: https://github.com/k01ek/netbox-qrcode
 Author: Nikolay Yuzefovich
 Author-email: mgk.kolek@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
@@ -20,14 +20,20 @@
 
 ## Compatibility
 
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 2.8 and later.
 
 ## Installation
 
+If Netbox was installed according to the standard installation instructions. It may be necessary to activate the virtual environment.
+
+```
+source /opt/netbox/venv/bin/activate
+```
+
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-qrcode
 ```
 Enable the plugin in /opt/netbox/netbox/netbox/configuration.py:
 ```
@@ -36,14 +42,15 @@
 Restart NetBox and add `netbox-qrcode` to your local_requirements.txt
 
 ## Configuration
 
 The following options are available:
 
 * `with_text`: Boolean (default True). Text label will be added to QR code image if enabled.
+* `text_template`: Jinja2 template with {{ obj }}  as context, using it ignores `text_fields` and `custom_text`
 * `text_fields`: List of String (default ['name']). Text fields of an object that will be added as text label to QR image. It's possible to use custom field values.
 * `font`: String (default TahomaBold) Font name for text label ( Some font include in package, see fonts dir).
 * `text_location`: Where to render the text, relative to the QR code.  Valid values are `"right"` (default), `"left"`", `"up"`, and `"down"`.
 * `custom_text`: String or None (default None) additional text label to QR code image (will be added after text_fields).
 * `qr_version`: Integer (default 1) parameter is an integer from 1 to 40 that controls the size of
 the QR Code (the smallest, version 1, is a 21x21 matrix).
 * `qr_error_correction`: Integer (default 0),  controls the error correction used for the
```

### Comparing `netbox-qrcode-0.0.8/README.md` & `netbox-qrcode-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 ## Compatibility
 
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 2.8 and later.
 
 ## Installation
 
+If Netbox was installed according to the standard installation instructions. It may be necessary to activate the virtual environment.
+
+```
+source /opt/netbox/venv/bin/activate
+```
+
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-qrcode
 ```
 Enable the plugin in /opt/netbox/netbox/netbox/configuration.py:
 ```
@@ -22,14 +28,15 @@
 Restart NetBox and add `netbox-qrcode` to your local_requirements.txt
 
 ## Configuration
 
 The following options are available:
 
 * `with_text`: Boolean (default True). Text label will be added to QR code image if enabled.
+* `text_template`: Jinja2 template with {{ obj }}  as context, using it ignores `text_fields` and `custom_text`
 * `text_fields`: List of String (default ['name']). Text fields of an object that will be added as text label to QR image. It's possible to use custom field values.
 * `font`: String (default TahomaBold) Font name for text label ( Some font include in package, see fonts dir).
 * `text_location`: Where to render the text, relative to the QR code.  Valid values are `"right"` (default), `"left"`", `"up"`, and `"down"`.
 * `custom_text`: String or None (default None) additional text label to QR code image (will be added after text_fields).
 * `qr_version`: Integer (default 1) parameter is an integer from 1 to 40 that controls the size of
 the QR Code (the smallest, version 1, is a 21x21 matrix).
 * `qr_error_correction`: Integer (default 0),  controls the error correction used for the
```

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/__init__.py` & `netbox-qrcode-0.0.9/netbox_qrcode/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/fonts/ArialBlack.ttf` & `netbox-qrcode-0.0.9/netbox_qrcode/fonts/ArialBlack.ttf`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/fonts/ArialMT.ttf` & `netbox-qrcode-0.0.9/netbox_qrcode/fonts/ArialMT.ttf`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/fonts/ComicSansMSBold.ttf` & `netbox-qrcode-0.0.9/netbox_qrcode/fonts/ComicSansMSBold.ttf`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/fonts/CourierNewBold.ttf` & `netbox-qrcode-0.0.9/netbox_qrcode/fonts/CourierNewBold.ttf`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/fonts/Tahoma.ttf` & `netbox-qrcode-0.0.9/netbox_qrcode/fonts/Tahoma.ttf`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/fonts/TahomaBold.ttf` & `netbox-qrcode-0.0.9/netbox_qrcode/fonts/TahomaBold.ttf`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/template_content.py` & `netbox-qrcode-0.0.9/netbox_qrcode/template_content.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from packaging import version
 
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
+from django.template import engines
 
 from extras.plugins import PluginTemplateExtension
 
 from .utilities import get_img_b64, get_qr, get_qr_text, get_concat
 
 
 class QRCode(PluginTemplateExtension):
@@ -25,39 +26,44 @@
         qr_args = {}
         for k, v in config.items():
             if k.startswith('qr_'):
                 qr_args[k.replace('qr_', '')] = v
 
         qr_img = get_qr(url, **qr_args)
         if config.get('with_text'):
-            text = []
-            for text_field in config.get('text_fields', []):
-                cfn = None
-                if '.' in text_field:
-                    try:
-                        text_field, cfn = text_field.split('.')
-                    except ValueError:
-                        cfn = None
-                if getattr(obj, text_field, None):
-                    if cfn:
+            if config.get('text_template'):
+                django_engine = engines["django"]
+                template = django_engine.from_string(config.get('text_template'))
+                text = template.render({'obj': obj})
+            else:
+                text = []
+                for text_field in config.get('text_fields', []):
+                    cfn = None
+                    if '.' in text_field:
                         try:
-                            if getattr(obj, text_field).get(cfn):
-                                text.append('{}'.format(getattr(obj, text_field).get(cfn)))
-                        except AttributeError:
-                            # fix for nb3.3: trying to get cable termination and device in same way as custom field
-                            if type(getattr(obj, text_field)) is list:
-                                first_element = next(iter(getattr(obj, text_field)), None)
-                                if first_element and getattr(first_element, cfn, None):
-                                    text.append('{}'.format(getattr(first_element, cfn)))
-                    else:
-                        text.append('{}'.format(getattr(obj, text_field)))
-            custom_text = config.get('custom_text')
-            if custom_text:
-                text.append(custom_text)
-            text = '\n'.join(text)
+                            text_field, cfn = text_field.split('.')
+                        except ValueError:
+                            cfn = None
+                    if getattr(obj, text_field, None):
+                        if cfn:
+                            try:
+                                if getattr(obj, text_field).get(cfn):
+                                    text.append('{}'.format(getattr(obj, text_field).get(cfn)))
+                            except AttributeError:
+                                # fix for nb3.3: trying to get cable termination and device in same way as custom field
+                                if type(getattr(obj, text_field)) is list:
+                                    first_element = next(iter(getattr(obj, text_field)), None)
+                                    if first_element and getattr(first_element, cfn, None):
+                                        text.append('{}'.format(getattr(first_element, cfn)))
+                        else:
+                            text.append('{}'.format(getattr(obj, text_field)))
+                custom_text = config.get('custom_text')
+                if custom_text:
+                    text.append(custom_text)
+                text = '\n'.join(text)
             text_img = get_qr_text(qr_img.size, text, config.get('font'))
             qr_with_text = get_concat(qr_img, text_img, config.get('text_location', 'right'))
 
             img = get_img_b64(qr_with_text)
         else:
             img = get_img_b64(qr_img)
         try:
```

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/templates/netbox_qrcode/qrcode.html` & `netbox-qrcode-0.0.9/netbox_qrcode/templates/netbox_qrcode/qrcode.html`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/templates/netbox_qrcode/qrcode3.html` & `netbox-qrcode-0.0.9/netbox_qrcode/templates/netbox_qrcode/qrcode3.html`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode/utilities.py` & `netbox-qrcode-0.0.9/netbox_qrcode/utilities.py`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode.egg-info/PKG-INFO` & `netbox-qrcode-0.0.9/netbox_qrcode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-qrcode
-Version: 0.0.8
+Version: 0.0.9
 Summary: QR Code generation for netbox objects
 Home-page: https://github.com/k01ek/netbox-qrcode
 Author: Nikolay Yuzefovich
 Author-email: mgk.kolek@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
@@ -20,14 +20,20 @@
 
 ## Compatibility
 
 This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 2.8 and later.
 
 ## Installation
 
+If Netbox was installed according to the standard installation instructions. It may be necessary to activate the virtual environment.
+
+```
+source /opt/netbox/venv/bin/activate
+```
+
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-qrcode
 ```
 Enable the plugin in /opt/netbox/netbox/netbox/configuration.py:
 ```
@@ -36,14 +42,15 @@
 Restart NetBox and add `netbox-qrcode` to your local_requirements.txt
 
 ## Configuration
 
 The following options are available:
 
 * `with_text`: Boolean (default True). Text label will be added to QR code image if enabled.
+* `text_template`: Jinja2 template with {{ obj }}  as context, using it ignores `text_fields` and `custom_text`
 * `text_fields`: List of String (default ['name']). Text fields of an object that will be added as text label to QR image. It's possible to use custom field values.
 * `font`: String (default TahomaBold) Font name for text label ( Some font include in package, see fonts dir).
 * `text_location`: Where to render the text, relative to the QR code.  Valid values are `"right"` (default), `"left"`", `"up"`, and `"down"`.
 * `custom_text`: String or None (default None) additional text label to QR code image (will be added after text_fields).
 * `qr_version`: Integer (default 1) parameter is an integer from 1 to 40 that controls the size of
 the QR Code (the smallest, version 1, is a 21x21 matrix).
 * `qr_error_correction`: Integer (default 0),  controls the error correction used for the
```

### Comparing `netbox-qrcode-0.0.8/netbox_qrcode.egg-info/SOURCES.txt` & `netbox-qrcode-0.0.9/netbox_qrcode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-qrcode-0.0.8/setup.py` & `netbox-qrcode-0.0.9/setup.py`

 * *Files identical despite different names*

