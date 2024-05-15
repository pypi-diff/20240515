# Comparing `tmp/iSwitch-1.0.6.tar.gz` & `tmp/iSwitch-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iSwitch-1.0.6.tar", last modified: Tue May 14 09:15:05 2024, max compression
+gzip compressed data, was "iSwitch-1.0.7.tar", last modified: Wed May 15 15:18:40 2024, max compression
```

## Comparing `iSwitch-1.0.6.tar` & `iSwitch-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-14 09:15:05.339137 iSwitch-1.0.6/
--rw-r--r--   0 mac        (501) staff       (20)     1057 2024-05-11 18:46:44.000000 iSwitch-1.0.6/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     6900 2024-05-14 09:15:05.338435 iSwitch-1.0.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     6549 2024-05-14 09:13:26.000000 iSwitch-1.0.6/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-14 09:15:05.337062 iSwitch-1.0.6/iSwitch.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     6900 2024-05-14 09:15:05.000000 iSwitch-1.0.6/iSwitch.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      276 2024-05-14 09:15:05.000000 iSwitch-1.0.6/iSwitch.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-14 09:15:05.000000 iSwitch-1.0.6/iSwitch.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       26 2024-05-14 09:15:05.000000 iSwitch-1.0.6/iSwitch.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-14 09:15:05.000000 iSwitch-1.0.6/iSwitch.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-14 09:15:05.336140 iSwitch-1.0.6/iswitch/
--rw-r--r--   0 mac        (501) staff       (20)      328 2024-05-12 10:01:33.000000 iSwitch-1.0.6/iswitch/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7777 2024-05-14 07:57:00.000000 iSwitch-1.0.6/iswitch/_client.py
--rw-r--r--   0 mac        (501) staff       (20)     7672 2024-05-13 21:46:29.000000 iSwitch-1.0.6/iswitch/_services.py
--rw-r--r--   0 mac        (501) staff       (20)     8086 2024-05-14 07:48:05.000000 iSwitch-1.0.6/iswitch/_types.py
--rw-r--r--   0 mac        (501) staff       (20)     3247 2024-05-12 10:42:22.000000 iSwitch-1.0.6/iswitch/_utils.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-14 09:15:05.339296 iSwitch-1.0.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      617 2024-05-14 09:14:42.000000 iSwitch-1.0.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-15 15:18:40.115620 iSwitch-1.0.7/
+-rw-r--r--   0 mac        (501) staff       (20)     1057 2024-05-11 18:46:44.000000 iSwitch-1.0.7/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)     6893 2024-05-15 15:18:40.114636 iSwitch-1.0.7/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     6542 2024-05-15 14:02:05.000000 iSwitch-1.0.7/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-15 15:18:40.113582 iSwitch-1.0.7/iSwitch.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     6893 2024-05-15 15:18:40.000000 iSwitch-1.0.7/iSwitch.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      276 2024-05-15 15:18:40.000000 iSwitch-1.0.7/iSwitch.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-15 15:18:40.000000 iSwitch-1.0.7/iSwitch.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       26 2024-05-15 15:18:40.000000 iSwitch-1.0.7/iSwitch.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-15 15:18:40.000000 iSwitch-1.0.7/iSwitch.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-15 15:18:40.112248 iSwitch-1.0.7/iswitch/
+-rw-r--r--   0 mac        (501) staff       (20)      328 2024-05-12 10:01:33.000000 iSwitch-1.0.7/iswitch/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     7744 2024-05-15 15:15:50.000000 iSwitch-1.0.7/iswitch/_client.py
+-rw-r--r--   0 mac        (501) staff       (20)     7672 2024-05-13 21:46:29.000000 iSwitch-1.0.7/iswitch/_services.py
+-rw-r--r--   0 mac        (501) staff       (20)     8086 2024-05-14 07:48:05.000000 iSwitch-1.0.7/iswitch/_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     3247 2024-05-12 10:42:22.000000 iSwitch-1.0.7/iswitch/_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-15 15:18:40.115938 iSwitch-1.0.7/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      617 2024-05-15 15:18:20.000000 iSwitch-1.0.7/setup.py
```

### Comparing `iSwitch-1.0.6/LICENSE` & `iSwitch-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.6/PKG-INFO` & `iSwitch-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSwitch
-Version: 1.0.6
+Version: 1.0.7
 Summary: SwitchPay Python SDK for AllDotPy internal use. 
 Home-page: https://github.com/AllDotPy/iSwitch.git
 Author: #Einswilli
 Author-email: einswilligoeh@email.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
@@ -20,21 +20,19 @@
 - <img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9eIXxPvwTKAgJYxFO7mR6ZGIrTaK16qFI0UsGnIQg&s' height = 60 ></img>
 - <img src = 'https://www.fedapay.com/wp-content/themes/fedapay_theme/pictures/feda-logo-blue-new.svg' height = 60 ></img> 
 
 ## Next
 We will add progressively support for following Providers:
 - <img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT3sWIPK8p28IQhWbqKpewYYtCHZaAk6O98T4dUiEhp&s' height = 60 ></img> 
 <span style = 'margin-left:10'></span>
-<img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQstE0NII74XhnGdDhMDWpA-7uL55uaooz3fn-yjrvl6g&s' height = 60 ></img>
-<span style = 'margin-left:10'></span>
-<img src = 'https://asset.brandfetch.io/idBsplB3mt/idyp_5HZE4.png' height = 60 >
+<img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQstE0NII74XhnGdDhMDWpA-7uL55uaooz3fn-yjrvl6g&s' height = 60 ></img><span style = 'margin-left:10'></span><img src = 'https://asset.brandfetch.io/idBsplB3mt/idyp_5HZE4.png' height = 55 >
 </img>
+
 - <img src = 'https://bankassurafrik.com/wp-content/uploads/2022/07/telechargement-2.png' height = 60 ></img>
-<span style = 'margin-left:10'></span>
-<img src = 'https://payplus.africa/img/logo.png' height = 60 ></img>
+<span style = 'margin-left:10'></span><img src = 'https://payplus.africa/img/logo.png' height = 60 ></img>
 <span style = 'margin-left:10'></span>
 <img src = 'https://paydunya.com/refont/images/logo/blue_logo.png' height = 60 ></img>
 
 
 
 ## Prerequisites
 
@@ -103,20 +101,19 @@
 
 ## Transactions 
 
 ### Create Order
 ```python
 # Creating order for SEMOA Transaction.
 semoa_order = {
-    'merchant_reference': 'USD-marchant',
-    'transaction_id': '123456',
+    'merchant_reference': '13fx5er5v7',
     'client': {
         'last_name': 'Doe',
         'first_name': 'John',
-        'phone': '123456789',
+        'phone': '+123456789',
     }
 }
 
 # Creating order for CINETPAY Transaction.
 cinetpay_order = {
     'transaction_id': '123456',
     'currency': 'XOF',
@@ -162,21 +159,21 @@
 ```python
 response = client.list_transactions()
 ```
 
 ### Retrieve Transaction
 To get a specific transaction you can use the `get_transaction` function.
 ```python
-response = client.get_transaction()
+response = client.get_transaction(transaction_id)
 ```
 
 ### Get a Specific Transaction payment url
 You can also get a payment URL for a specific Transaction using `get_bill_url` function.
 ```python
-response = client.get_bill_url()
+response = client.get_bill_url(transaction_id)
 ```
 
 ## Responses
 - ### Response class
 The default Request response class, is returned when `detail` is set to `True` in the request.
 ```python
 response = client.create_transaction(my_transaction)
```

### Comparing `iSwitch-1.0.6/README.md` & `iSwitch-1.0.7/iSwitch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+Metadata-Version: 2.1
+Name: iSwitch
+Version: 1.0.7
+Summary: SwitchPay Python SDK for AllDotPy internal use. 
+Home-page: https://github.com/AllDotPy/iSwitch.git
+Author: #Einswilli
+Author-email: einswilligoeh@email.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: simplejson
+Requires-Dist: colorlog
+
 # iSwitch😎 Python Library
 
 [SwitchPay](https://github.com/AllDotPy/SwitchPay) Python SDK for AllDotPy internal use.
 
 ## Currently Supported Providers
 - <img src = 'https://cinetpay.com/brand/logo-cinetpay.webp' height = 60 ></img>
 - <img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9eIXxPvwTKAgJYxFO7mR6ZGIrTaK16qFI0UsGnIQg&s' height = 60 ></img>
 - <img src = 'https://www.fedapay.com/wp-content/themes/fedapay_theme/pictures/feda-logo-blue-new.svg' height = 60 ></img> 
 
 ## Next
 We will add progressively support for following Providers:
 - <img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT3sWIPK8p28IQhWbqKpewYYtCHZaAk6O98T4dUiEhp&s' height = 60 ></img> 
 <span style = 'margin-left:10'></span>
-<img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQstE0NII74XhnGdDhMDWpA-7uL55uaooz3fn-yjrvl6g&s' height = 60 ></img>
-<span style = 'margin-left:10'></span>
-<img src = 'https://asset.brandfetch.io/idBsplB3mt/idyp_5HZE4.png' height = 60 >
+<img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQstE0NII74XhnGdDhMDWpA-7uL55uaooz3fn-yjrvl6g&s' height = 60 ></img><span style = 'margin-left:10'></span><img src = 'https://asset.brandfetch.io/idBsplB3mt/idyp_5HZE4.png' height = 55 >
 </img>
+
 - <img src = 'https://bankassurafrik.com/wp-content/uploads/2022/07/telechargement-2.png' height = 60 ></img>
-<span style = 'margin-left:10'></span>
-<img src = 'https://payplus.africa/img/logo.png' height = 60 ></img>
+<span style = 'margin-left:10'></span><img src = 'https://payplus.africa/img/logo.png' height = 60 ></img>
 <span style = 'margin-left:10'></span>
 <img src = 'https://paydunya.com/refont/images/logo/blue_logo.png' height = 60 ></img>
 
 
 
 ## Prerequisites
 
@@ -90,20 +101,19 @@
 
 ## Transactions 
 
 ### Create Order
 ```python
 # Creating order for SEMOA Transaction.
 semoa_order = {
-    'merchant_reference': 'USD-marchant',
-    'transaction_id': '123456',
+    'merchant_reference': '13fx5er5v7',
     'client': {
         'last_name': 'Doe',
         'first_name': 'John',
-        'phone': '123456789',
+        'phone': '+123456789',
     }
 }
 
 # Creating order for CINETPAY Transaction.
 cinetpay_order = {
     'transaction_id': '123456',
     'currency': 'XOF',
@@ -149,21 +159,21 @@
 ```python
 response = client.list_transactions()
 ```
 
 ### Retrieve Transaction
 To get a specific transaction you can use the `get_transaction` function.
 ```python
-response = client.get_transaction()
+response = client.get_transaction(transaction_id)
 ```
 
 ### Get a Specific Transaction payment url
 You can also get a payment URL for a specific Transaction using `get_bill_url` function.
 ```python
-response = client.get_bill_url()
+response = client.get_bill_url(transaction_id)
 ```
 
 ## Responses
 - ### Response class
 The default Request response class, is returned when `detail` is set to `True` in the request.
 ```python
 response = client.create_transaction(my_transaction)
```

### Comparing `iSwitch-1.0.6/iSwitch.egg-info/PKG-INFO` & `iSwitch-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,25 @@
-Metadata-Version: 2.1
-Name: iSwitch
-Version: 1.0.6
-Summary: SwitchPay Python SDK for AllDotPy internal use. 
-Home-page: https://github.com/AllDotPy/iSwitch.git
-Author: #Einswilli
-Author-email: einswilligoeh@email.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx
-Requires-Dist: simplejson
-Requires-Dist: colorlog
-
 # iSwitch😎 Python Library
 
 [SwitchPay](https://github.com/AllDotPy/SwitchPay) Python SDK for AllDotPy internal use.
 
 ## Currently Supported Providers
 - <img src = 'https://cinetpay.com/brand/logo-cinetpay.webp' height = 60 ></img>
 - <img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9eIXxPvwTKAgJYxFO7mR6ZGIrTaK16qFI0UsGnIQg&s' height = 60 ></img>
 - <img src = 'https://www.fedapay.com/wp-content/themes/fedapay_theme/pictures/feda-logo-blue-new.svg' height = 60 ></img> 
 
 ## Next
 We will add progressively support for following Providers:
 - <img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT3sWIPK8p28IQhWbqKpewYYtCHZaAk6O98T4dUiEhp&s' height = 60 ></img> 
 <span style = 'margin-left:10'></span>
-<img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQstE0NII74XhnGdDhMDWpA-7uL55uaooz3fn-yjrvl6g&s' height = 60 ></img>
-<span style = 'margin-left:10'></span>
-<img src = 'https://asset.brandfetch.io/idBsplB3mt/idyp_5HZE4.png' height = 60 >
+<img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQstE0NII74XhnGdDhMDWpA-7uL55uaooz3fn-yjrvl6g&s' height = 60 ></img><span style = 'margin-left:10'></span><img src = 'https://asset.brandfetch.io/idBsplB3mt/idyp_5HZE4.png' height = 55 >
 </img>
+
 - <img src = 'https://bankassurafrik.com/wp-content/uploads/2022/07/telechargement-2.png' height = 60 ></img>
-<span style = 'margin-left:10'></span>
-<img src = 'https://payplus.africa/img/logo.png' height = 60 ></img>
+<span style = 'margin-left:10'></span><img src = 'https://payplus.africa/img/logo.png' height = 60 ></img>
 <span style = 'margin-left:10'></span>
 <img src = 'https://paydunya.com/refont/images/logo/blue_logo.png' height = 60 ></img>
 
 
 
 ## Prerequisites
 
@@ -103,20 +88,19 @@
 
 ## Transactions 
 
 ### Create Order
 ```python
 # Creating order for SEMOA Transaction.
 semoa_order = {
-    'merchant_reference': 'USD-marchant',
-    'transaction_id': '123456',
+    'merchant_reference': '13fx5er5v7',
     'client': {
         'last_name': 'Doe',
         'first_name': 'John',
-        'phone': '123456789',
+        'phone': '+123456789',
     }
 }
 
 # Creating order for CINETPAY Transaction.
 cinetpay_order = {
     'transaction_id': '123456',
     'currency': 'XOF',
@@ -162,21 +146,21 @@
 ```python
 response = client.list_transactions()
 ```
 
 ### Retrieve Transaction
 To get a specific transaction you can use the `get_transaction` function.
 ```python
-response = client.get_transaction()
+response = client.get_transaction(transaction_id)
 ```
 
 ### Get a Specific Transaction payment url
 You can also get a payment URL for a specific Transaction using `get_bill_url` function.
 ```python
-response = client.get_bill_url()
+response = client.get_bill_url(transaction_id)
 ```
 
 ## Responses
 - ### Response class
 The default Request response class, is returned when `detail` is set to `True` in the request.
 ```python
 response = client.create_transaction(my_transaction)
```

### Comparing `iSwitch-1.0.6/iswitch/_client.py` & `iSwitch-1.0.7/iswitch/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,14 @@
                     if p['name'] == self.config['service']:
                         return p
                 # THEN THIS PAGE DON'T CONTAINS THE SPECIFIED PROVIDER
                 if p.has_next:
                     search(p.next_page)
             
             return None       
-        print(search(providers))
         return search(providers)     
     
     def authenticate(self):
         ''' Authenticates App. '''
         
         # GET AUTH CREDENTIALS
         creds = self.config['credentials']
```

### Comparing `iSwitch-1.0.6/iswitch/_services.py` & `iSwitch-1.0.7/iswitch/_services.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.6/iswitch/_types.py` & `iSwitch-1.0.7/iswitch/_types.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.6/iswitch/_utils.py` & `iSwitch-1.0.7/iswitch/_utils.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.6/setup.py` & `iSwitch-1.0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # LOADING DOCUMENTATION
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = 'iSwitch',
-    version = '1.0.6',
+    version = '1.0.7',
     packages = find_packages(),
     install_requires = [
         'httpx',
         'simplejson',
         'colorlog'
     ],
     long_description=long_description,
```

