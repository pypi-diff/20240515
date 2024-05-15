# Comparing `tmp/multiform_validator-0.0.8.tar.gz` & `tmp/multiform_validator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiform_validator-0.0.8.tar", last modified: Mon May  6 21:17:38 2024, max compression
+gzip compressed data, was "multiform_validator-0.0.9.tar", last modified: Thu May  9 21:13:30 2024, max compression
```

## Comparing `multiform_validator-0.0.8.tar` & `multiform_validator-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:38.260419 multiform_validator-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/src/multiform_validator/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/cnpjValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/cpfValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/getOnlyEmail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/identifyFlagCard.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/isCreditCardValid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/isEmail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/passwordStrengthTester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/validateBRPhoneNumber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/src/multiform_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-06 21:17:38.000000 multiform_validator-0.0.8/src/multiform_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-06 21:17:38.000000 multiform_validator-0.0.8/src/multiform_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:17:38.000000 multiform_validator-0.0.8/src/multiform_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 21:17:38.000000 multiform_validator-0.0.8/src/multiform_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:13:30.540358 multiform_validator-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-09 21:13:30.540358 multiform_validator-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:13:30.540358 multiform_validator-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:13:30.536358 multiform_validator-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:13:30.540358 multiform_validator-0.0.9/src/multiform_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/cnpjValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/cpfValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/getOnlyEmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/identifyFlagCard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/isCreditCardValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/isEmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/passwordStrengthTester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-09 21:13:19.000000 multiform_validator-0.0.9/src/multiform_validator/validateBRPhoneNumber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:13:30.540358 multiform_validator-0.0.9/src/multiform_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-09 21:13:30.000000 multiform_validator-0.0.9/src/multiform_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 21:13:30.000000 multiform_validator-0.0.9/src/multiform_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:13:30.000000 multiform_validator-0.0.9/src/multiform_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-09 21:13:30.000000 multiform_validator-0.0.9/src/multiform_validator.egg-info/top_level.txt
```

### Comparing `multiform_validator-0.0.8/LICENSE` & `multiform_validator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/PKG-INFO` & `multiform_validator-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: multiform-validator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more.
 Author: Gabriel Logan
-Project-URL: Homepage, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
+Project-URL: Homepage, https://gabriel-logan.github.io/multiform-validator/documentation
 Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,15 +16,15 @@
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
 This package provides Python functions to validate various forms fields.
 
-Documentation: https://github.com/gabriel-logan/multiform-validator
+Documentation: https://gabriel-logan.github.io/multiform-validator/documentation/py
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
 
 <p align="center">
 	<a href="https://www.buymeacoffee.com/gabriellogan" target="_blank">
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: multiform-validator Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: multiform-validator Version: 0.0.9 Summary:
 Multilingual library made for validation, various form fields, such as: email,
 cpf, cnpj, credit card, and much more. Author: Gabriel Logan Project-URL:
-Homepage, https://github.com/gabriel-logan/multiform-validator/tree/main/
-packages/python Project-URL: Bug Tracker, https://github.com/gabriel-logan/
-multiform-validator/tree/main/packages/python Classifier: Programming Language
-:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
-Type: text/markdown License-File: LICENSE # Multiform-validator [![PyPI
-version](https://badge.fury.io/py/multiform-validator.svg)](https://
-badge.fury.io/py/multiform-validator) [![License: MIT](https://img.shields.io/
-badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI
-downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-
-square)](https://pypistats.org/packages/multiform-validator) This package
-provides Python functions to validate various forms fields. Documentation:
-https://github.com/gabriel-logan/multiform-validator Feel free to find bugs and
+Homepage, https://gabriel-logan.github.io/multiform-validator/documentation
+Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/
+tree/main/packages/python Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE # Multiform-validator [![PyPI version](https://
+badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-
+validator) [![License: MIT](https://img.shields.io/badge/License-MIT-
+yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI downloads](https://
+img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://
+pypistats.org/packages/multiform-validator) This package provides Python
+functions to validate various forms fields. Documentation: https://gabriel-
+logan.github.io/multiform-validator/documentation/py Feel free to find bugs and
 report them to me. Your feedback is highly appreciated. Hugs from Gabriel
 Logan! If you want to help me, you can buy me a coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ### Installation ```bash pip install multiform-validator ``` # Data Validator
 This package contains various modules for validating different types of data.
 Below are the available validation modules: # Avaliable for while -
 **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
```

### Comparing `multiform_validator-0.0.8/README.md` & `multiform_validator-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
 This package provides Python functions to validate various forms fields.
 
-Documentation: https://github.com/gabriel-logan/multiform-validator
+Documentation: https://gabriel-logan.github.io/multiform-validator/documentation/py
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
 
 <p align="center">
 	<a href="https://www.buymeacoffee.com/gabriellogan" target="_blank">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 # Multiform-validator [![PyPI version](https://badge.fury.io/py/multiform-
 validator.svg)](https://badge.fury.io/py/multiform-validator) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
 licenses/MIT) [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-
 validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-
 validator) This package provides Python functions to validate various forms
-fields. Documentation: https://github.com/gabriel-logan/multiform-validator
-Feel free to find bugs and report them to me. Your feedback is highly
-appreciated. Hugs from Gabriel Logan! If you want to help me, you can buy me a
-coffee (:
+fields. Documentation: https://gabriel-logan.github.io/multiform-validator/
+documentation/py Feel free to find bugs and report them to me. Your feedback is
+highly appreciated. Hugs from Gabriel Logan! If you want to help me, you can
+buy me a coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ### Installation ```bash pip install multiform-validator ``` # Data Validator
 This package contains various modules for validating different types of data.
 Below are the available validation modules: # Avaliable for while -
 **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
 **getOnlyEmail**: Extracts only the email or emails address from a string. -
 **identifyFlagCard**: Identifies the flag of a credit card. -
```

### Comparing `multiform_validator-0.0.8/pyproject.toml` & `multiform_validator-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 requires = [
     "setuptools>=61"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "multiform-validator"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Gabriel Logan" },
 ]
 description = "Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python"
+"Homepage" = "https://gabriel-logan.github.io/multiform-validator/documentation"
 "Bug Tracker" = "https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python"
```

### Comparing `multiform_validator-0.0.8/src/multiform_validator/cnpjValidator.py` & `multiform_validator-0.0.9/src/multiform_validator/cnpjValidator.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/src/multiform_validator/cpfValidator.py` & `multiform_validator-0.0.9/src/multiform_validator/cpfValidator.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/src/multiform_validator/getOnlyEmail.py` & `multiform_validator-0.0.9/src/multiform_validator/getOnlyEmail.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/src/multiform_validator/identifyFlagCard.py` & `multiform_validator-0.0.9/src/multiform_validator/identifyFlagCard.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/src/multiform_validator/isCreditCardValid.py` & `multiform_validator-0.0.9/src/multiform_validator/isCreditCardValid.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/src/multiform_validator/isEmail.py` & `multiform_validator-0.0.9/src/multiform_validator/isEmail.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/src/multiform_validator/passwordStrengthTester.py` & `multiform_validator-0.0.9/src/multiform_validator/passwordStrengthTester.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/src/multiform_validator/validateBRPhoneNumber.py` & `multiform_validator-0.0.9/src/multiform_validator/validateBRPhoneNumber.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.8/src/multiform_validator.egg-info/PKG-INFO` & `multiform_validator-0.0.9/src/multiform_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: multiform-validator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more.
 Author: Gabriel Logan
-Project-URL: Homepage, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
+Project-URL: Homepage, https://gabriel-logan.github.io/multiform-validator/documentation
 Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,15 +16,15 @@
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
 This package provides Python functions to validate various forms fields.
 
-Documentation: https://github.com/gabriel-logan/multiform-validator
+Documentation: https://gabriel-logan.github.io/multiform-validator/documentation/py
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
 
 <p align="center">
 	<a href="https://www.buymeacoffee.com/gabriellogan" target="_blank">
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: multiform-validator Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: multiform-validator Version: 0.0.9 Summary:
 Multilingual library made for validation, various form fields, such as: email,
 cpf, cnpj, credit card, and much more. Author: Gabriel Logan Project-URL:
-Homepage, https://github.com/gabriel-logan/multiform-validator/tree/main/
-packages/python Project-URL: Bug Tracker, https://github.com/gabriel-logan/
-multiform-validator/tree/main/packages/python Classifier: Programming Language
-:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
-Type: text/markdown License-File: LICENSE # Multiform-validator [![PyPI
-version](https://badge.fury.io/py/multiform-validator.svg)](https://
-badge.fury.io/py/multiform-validator) [![License: MIT](https://img.shields.io/
-badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI
-downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-
-square)](https://pypistats.org/packages/multiform-validator) This package
-provides Python functions to validate various forms fields. Documentation:
-https://github.com/gabriel-logan/multiform-validator Feel free to find bugs and
+Homepage, https://gabriel-logan.github.io/multiform-validator/documentation
+Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/
+tree/main/packages/python Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE # Multiform-validator [![PyPI version](https://
+badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-
+validator) [![License: MIT](https://img.shields.io/badge/License-MIT-
+yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI downloads](https://
+img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://
+pypistats.org/packages/multiform-validator) This package provides Python
+functions to validate various forms fields. Documentation: https://gabriel-
+logan.github.io/multiform-validator/documentation/py Feel free to find bugs and
 report them to me. Your feedback is highly appreciated. Hugs from Gabriel
 Logan! If you want to help me, you can buy me a coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ### Installation ```bash pip install multiform-validator ``` # Data Validator
 This package contains various modules for validating different types of data.
 Below are the available validation modules: # Avaliable for while -
 **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
```

### Comparing `multiform_validator-0.0.8/src/multiform_validator.egg-info/SOURCES.txt` & `multiform_validator-0.0.9/src/multiform_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

