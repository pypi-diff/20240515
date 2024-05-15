# Comparing `tmp/acslib-0.1.8.tar.gz` & `tmp/acslib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acslib-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acslib-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acslib-0.1.8.tar` & `acslib-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0      163 2024-05-01 13:37:48.327647 acslib-0.1.8/.coveragerc
--rw-r--r--   0        0        0      104 2024-05-01 13:37:48.327647 acslib-0.1.8/.dockerignore
--rw-r--r--   0        0        0      292 2024-05-01 13:37:48.327647 acslib-0.1.8/.editorconfig
--rw-r--r--   0        0        0      296 2024-05-01 13:37:48.327647 acslib-0.1.8/.github/pr_template.md
--rw-r--r--   0        0        0     9382 2024-05-01 13:37:48.327647 acslib-0.1.8/.github/workflows/test_publish_release..yml
--rw-r--r--   0        0        0     1388 2024-05-01 13:37:48.327647 acslib-0.1.8/.gitignore
--rw-r--r--   0        0        0       81 2024-05-01 13:37:48.327647 acslib-0.1.8/.isort.cfg
--rw-r--r--   0        0        0      875 2024-05-01 13:37:48.327647 acslib-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      118 2024-05-01 13:37:48.327647 acslib-0.1.8/AUTHORS.md
--rw-r--r--   0        0        0      212 2024-05-01 13:37:48.327647 acslib-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0      473 2024-05-01 13:37:48.327647 acslib-0.1.8/Dockerfile
--rw-r--r--   0        0        0       59 2024-05-01 13:37:48.327647 acslib-0.1.8/HISTORY.md
--rw-r--r--   0        0        0     1089 2024-05-01 13:37:48.327647 acslib-0.1.8/LICENSE
--rw-r--r--   0        0        0      589 2024-05-01 13:37:48.327647 acslib-0.1.8/Makefile
--rw-r--r--   0        0        0     5171 2024-05-01 13:37:48.327647 acslib-0.1.8/README.md
--rw-r--r--   0        0        0      188 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/__init__.py
--rw-r--r--   0        0        0      218 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/__init__.py
--rw-r--r--   0        0        0      259 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/acs.py
--rw-r--r--   0        0        0      172 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/config.py
--rw-r--r--   0        0        0     6294 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/connection.py
--rw-r--r--   0        0        0      272 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/search.py
--rw-r--r--   0        0        0     6113 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/status.py
--rw-r--r--   0        0        0      322 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/__init__.py
--rw-r--r--   0        0        0      595 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/base.py
--rw-r--r--   0        0        0     2923 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/config.py
--rw-r--r--   0        0        0     7460 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/connection.py
--rw-r--r--   0        0        0    20500 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/crud.py
--rw-r--r--   0        0        0     1070 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/data_models.py
--rw-r--r--   0        0        0     1141 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/endpoints.py
--rw-r--r--   0        0        0     7674 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/filters.py
--rw-r--r--   0        0        0       36 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/__init__.py
--rw-r--r--   0        0        0     1839 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/conftest.py
--rw-r--r--   0        0        0     2037 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/test_base.py
--rw-r--r--   0        0        0     2801 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/test_config.py
--rw-r--r--   0        0        0     2111 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/test_connection.py
--rw-r--r--   0        0        0     2588 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/test_search.py
--rw-r--r--   0        0        0      837 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/types.py
--rw-r--r--   0        0        0       11 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/api.md
--rw-r--r--   0        0        0       41 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/authors.md
--rw-r--r--   0        0        0       46 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/contributing.md
--rw-r--r--   0        0        0       41 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/history.md
--rw-r--r--   0        0        0       42 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/index.md
--rw-r--r--   0        0        0     1188 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/installation.md
--rw-r--r--   0        0        0       87 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/usage.md
--rw-r--r--   0        0        0       20 2024-05-01 13:37:48.327647 acslib-0.1.8/envrc_sample
--rw-r--r--   0        0        0     1949 2024-05-01 13:37:48.327647 acslib-0.1.8/mkdocs.yml
--rw-r--r--   0        0        0     1918 2024-05-01 13:37:48.327647 acslib-0.1.8/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
--rw-r--r--   0        0        0     2314 2024-05-01 13:37:48.327647 acslib-0.1.8/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
--rw-r--r--   0        0        0    12624 2024-05-01 13:37:48.327647 acslib-0.1.8/notebooks/encode_investigation.ipynb
--rw-r--r--   0        0        0     2699 2024-05-01 13:37:48.327647 acslib-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      219 2024-05-01 13:37:48.331647 acslib-0.1.8/pytest.ini
--rw-r--r--   0        0        0      926 2024-05-01 13:37:48.331647 acslib-0.1.8/requirements/base/base.txt
--rw-r--r--   0        0        0     4618 2024-05-01 13:37:48.331647 acslib-0.1.8/requirements/dev/dev.txt
--rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 acslib-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      163 2024-05-15 13:38:27.985336 acslib-0.1.9/.coveragerc
+-rw-r--r--   0        0        0      104 2024-05-15 13:38:27.985336 acslib-0.1.9/.dockerignore
+-rw-r--r--   0        0        0      292 2024-05-15 13:38:27.985336 acslib-0.1.9/.editorconfig
+-rw-r--r--   0        0        0      296 2024-05-15 13:38:27.985336 acslib-0.1.9/.github/pr_template.md
+-rw-r--r--   0        0        0     9383 2024-05-15 13:38:27.985336 acslib-0.1.9/.github/workflows/test_publish_release..yml
+-rw-r--r--   0        0        0     1388 2024-05-15 13:38:27.985336 acslib-0.1.9/.gitignore
+-rw-r--r--   0        0        0       81 2024-05-15 13:38:27.985336 acslib-0.1.9/.isort.cfg
+-rw-r--r--   0        0        0      875 2024-05-15 13:38:27.985336 acslib-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      118 2024-05-15 13:38:27.985336 acslib-0.1.9/AUTHORS.md
+-rw-r--r--   0        0        0      212 2024-05-15 13:38:27.985336 acslib-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      473 2024-05-15 13:38:27.985336 acslib-0.1.9/Dockerfile
+-rw-r--r--   0        0        0       59 2024-05-15 13:38:27.985336 acslib-0.1.9/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-05-15 13:38:27.985336 acslib-0.1.9/LICENSE
+-rw-r--r--   0        0        0      589 2024-05-15 13:38:27.985336 acslib-0.1.9/Makefile
+-rw-r--r--   0        0        0     5921 2024-05-15 13:38:27.985336 acslib-0.1.9/README.md
+-rw-r--r--   0        0        0      183 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/__init__.py
+-rw-r--r--   0        0        0      218 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/base/__init__.py
+-rw-r--r--   0        0        0      259 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/base/acs.py
+-rw-r--r--   0        0        0      172 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/base/config.py
+-rw-r--r--   0        0        0     6597 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/base/connection.py
+-rw-r--r--   0        0        0      272 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/base/search.py
+-rw-r--r--   0        0        0     6113 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/base/status.py
+-rw-r--r--   0        0        0      881 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/__init__.py
+-rw-r--r--   0        0        0     5339 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/actions.py
+-rw-r--r--   0        0        0     6993 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/base.py
+-rw-r--r--   0        0        0     2923 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/config.py
+-rw-r--r--   0        0        0     7460 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/connection.py
+-rw-r--r--   0        0        0    10951 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/crud.py
+-rw-r--r--   0        0        0     1070 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/data_models.py
+-rw-r--r--   0        0        0      652 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/endpoints.py
+-rw-r--r--   0        0        0     6913 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/filters.py
+-rw-r--r--   0        0        0       36 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/tests/__init__.py
+-rw-r--r--   0        0        0     1839 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/tests/conftest.py
+-rw-r--r--   0        0        0     1809 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/tests/test_base.py
+-rw-r--r--   0        0        0     2801 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/tests/test_config.py
+-rw-r--r--   0        0        0     2111 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/tests/test_connection.py
+-rw-r--r--   0        0        0     2588 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/tests/test_search.py
+-rw-r--r--   0        0        0     1470 2024-05-15 13:38:27.985336 acslib-0.1.9/acslib/ccure/types.py
+-rw-r--r--   0        0        0       11 2024-05-15 13:38:27.985336 acslib-0.1.9/docs/api.md
+-rw-r--r--   0        0        0       41 2024-05-15 13:38:27.985336 acslib-0.1.9/docs/authors.md
+-rw-r--r--   0        0        0       46 2024-05-15 13:38:27.985336 acslib-0.1.9/docs/contributing.md
+-rw-r--r--   0        0        0       41 2024-05-15 13:38:27.985336 acslib-0.1.9/docs/history.md
+-rw-r--r--   0        0        0       42 2024-05-15 13:38:27.985336 acslib-0.1.9/docs/index.md
+-rw-r--r--   0        0        0     1188 2024-05-15 13:38:27.985336 acslib-0.1.9/docs/installation.md
+-rw-r--r--   0        0        0       87 2024-05-15 13:38:27.985336 acslib-0.1.9/docs/usage.md
+-rw-r--r--   0        0        0       20 2024-05-15 13:38:27.985336 acslib-0.1.9/envrc_sample
+-rw-r--r--   0        0        0     1949 2024-05-15 13:38:27.985336 acslib-0.1.9/mkdocs.yml
+-rw-r--r--   0        0        0     1918 2024-05-15 13:38:27.985336 acslib-0.1.9/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
+-rw-r--r--   0        0        0     2314 2024-05-15 13:38:27.985336 acslib-0.1.9/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
+-rw-r--r--   0        0        0    12610 2024-05-15 13:38:27.985336 acslib-0.1.9/notebooks/encode_investigation.ipynb
+-rw-r--r--   0        0        0     2699 2024-05-15 13:38:27.985336 acslib-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-05-15 13:38:27.985336 acslib-0.1.9/pytest.ini
+-rw-r--r--   0        0        0      926 2024-05-15 13:38:27.985336 acslib-0.1.9/requirements/base/base.txt
+-rw-r--r--   0        0        0     4618 2024-05-15 13:38:27.985336 acslib-0.1.9/requirements/dev/dev.txt
+-rw-r--r--   0        0        0     7506 1970-01-01 00:00:00.000000 acslib-0.1.9/PKG-INFO
```

### Comparing `acslib-0.1.8/.github/workflows/test_publish_release..yml` & `acslib-0.1.9/.github/workflows/test_publish_release..yml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       - main
   pull_request:
   workflow_dispatch:
 
 env:
     REPO_NAME: acslib
     RELEASE_REPO: https://github.com/ncstate-sat/acslib
-    SLACK_UPDATES: true
+    SLACK_UPDATES: false
     # sends notifications to the clearance slack channel
     SLACK_CHANNEL_ID: ${{ secrets.ACSLIB_CHANNEL_ID }}
     FLIT_USERNAME: __token__
     FLIT_PASSWORD: ${{ secrets.PYPI_TOKEN }}
 
 jobs:
   run_tests:
```

### Comparing `acslib-0.1.8/.gitignore` & `acslib-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/.pre-commit-config.yaml` & `acslib-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/LICENSE` & `acslib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/Makefile` & `acslib-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/README.md` & `acslib-0.1.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -20,197 +20,234 @@
 
 * Free software: MIT
 * Documentation: <https://github.com/ncstate-sat/acslib>
 
 
 ## Features
 
-* Currently supports Search for `Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k
+* Currently supports CRUD operations for `Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k, and all other Ccure object types.
 * Supports search by custom fields.
 
 ## Usage
 
 ### Personnel
 
 #### Find a person by name
 
 ```python
 from acslib import CcureAPI
 
-ccure_api = CcureAPI()
-response = ccure_api.personnel.search("Roddy Piper".split())
+ccure = CcureAPI()
+response = ccure.personnel.search("Roddy Piper".split())
 ```
 
 #### Find a person by custom field
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.filters import PersonnelFilter, FUZZ
 
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 search_filter = PersonnelFilter(lookups={"Text1": FUZZ})
-response = ccure_api.personnel.search(["PER0892347"], search_filter=search_filter)
+response = ccure.personnel.search(["PER0892347"], search_filter=search_filter)
 ```
 
 #### Update a personnel record
 
 ```python
 from acslib import CcureAPI
 
 # change MiddleName and Text14 for the person with CCure ID 5001
-ccure_api = CcureAPI()
-ccure_api.personnel.update(5001, {"Text14": "new text here", "MiddleName": "Shaquille"})
+ccure = CcureAPI()
+ccure.personnel.update(5001, {"Text14": "new text here", "MiddleName": "Shaquille"})
 ```
 
 #### Add new personnel record
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.types import PersonnelCreateData as pcd
 
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 new_person_data = pcd(FirstName="Kenny", LastName="Smith", Text1="001132808")
-ccure_api.personnel.create(new_person_data)
+ccure.personnel.create(new_person_data)
 ```
 
 #### Delete a personnel record
 
 ```python
 from acslib import CcureAPI
 
 # delete the personnel record with the CCure ID 6008
-ccure_api = CcureAPI()
-ccure_api.personnel.delete(6008)
+ccure = CcureAPI()
+ccure.personnel.delete(6008)
 ```
 
 ### Clearance
 
 #### Find a Clearance by name
 
 ```python
 from acslib import CcureAPI
 
-ccure_api = CcureAPI()
-response = ccure_api.clearance.search(["suite", "door"])
+ccure = CcureAPI()
+response = ccure.clearance.search(["suite", "door"])
 ```
 
 #### Find a Clearance by other field
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.filters import ClearanceFilter, NFUZZ
 
 # search by ObjectID
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 search_filter = ClearanceFilter(lookups={"ObjectID": NFUZZ})
-response = ccure_api.clearance.search([8897], search_filter=search_filter)
+response = ccure.clearance.search([8897], search_filter=search_filter)
 ```
 
 ### Credential
 
 #### Find all credentials
 
 ```python
 from acslib import CcureAPI
 
-ccure_api = CcureAPI()
-response = ccure_api.credential.search()
+ccure = CcureAPI()
+response = ccure.credential.search()
 ```
 
 #### Find a credential by name
 
 ```python
 from acslib import CcureAPI
 
 # fuzzy search by name
-ccure_api = CcureAPI()
-response = ccure_api.credential.search(["charles", "barkley"])
+ccure = CcureAPI()
+response = ccure.credential.search(["charles", "barkley"])
 ```
 
 #### Find a credential by other field
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.filters import CredentialFilter, NFUZZ
 
 # search by ObjectID
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 search_filter = CredentialFilter(lookups={"ObjectID": NFUZZ})
-response = ccure_api.credential.search([5001], search_filter=search_filter)
+response = ccure.credential.search([5001], search_filter=search_filter)
 ```
 
 #### Update a credential
 
 ```python
 from acslib import CcureAPI
 
 # update CardInt1 for the credential with ObjectID 5001
-ccure_api = CcureAPI()
-response = ccure_api.credential.update(5001, {"CardInt1": 12345})
+ccure = CcureAPI()
+response = ccure.credential.update(5001, {"CardInt1": 12345})
 ```
 
 ### ClearanceItem
 
 Clearance items include "door" and "elevator."
 
 #### Find ClearanceItem by name
 
 ```python
 from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemType as cit
+from acslib.ccure.types import ObjectType
 
 # fuzzy search for doors by name
-ccure_api = CcureAPI()
-response = ccure_api.clearance_item.search(cit.DOOR, ["hall", "interior"])
+ccure = CcureAPI()
+response = ccure.clearance_item.search(ObjectType.DOOR.complete, ["hall", "interior"])
 ```
 
 #### Find ClearanceItem by other field
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.filters import ClearanceItemFilter, NFUZZ
-from acslib.ccure.types import ClearanceItemType as cit
+from acslib.ccure.types import ObjectType
 
 # search elevators by ObjectID
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 search_filter = ClearanceItemFilter(lookups={"ObjectID": NFUZZ})
-response = ccure_api.clearance_item.search(cit.ELEVATOR, [5000], search_filter=search_filter)
+response = ccure.clearance_item.search(ObjectType.ELEVATOR.complete, [5000], search_filter=search_filter)
 ```
 
 #### Update ClearanceItem
 
 ```python
 from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemType as cit
+from acslib.ccure.types import ObjectType
 # change a door's name
-ccure_api = CcureAPI()
-response = ccure_api.clearance_item.update(cit.DOOR, 5000, update_data={"Name": "new door name 123"})
+ccure = CcureAPI()
+response = ccure.clearance_item.update(ObjectType.DOOR.complete, 5000, update_data={"Name": "new door name 123"})
 ```
 
 #### Create ClearanceItem
 
 ```python
 from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemCreateData, ClearanceItemType as cit
+from acslib.ccure.types import ClearanceItemCreateData, ObjectType
 
 # create a new elevator
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 new_elevator_data = ClearanceItemCreateData(
     Name="New elevator 1",
     Description="newest elevator in town",
     ParentID=5000,
     ParentType="SoftwareHouse.NextGen.Common.SecurityObjects.iStarController",
     ControllerID=5000,
     ControllerClassType="SoftwareHouse.NextGen.Common.SecurityObjects.iStarController"
 )
-response = ccure_api.clearance_item.create(cit.ELEVATOR, create_data=new_elevator_data)
+response = ccure.clearance_item.create(ObjectType.ELEVATOR.complete, create_data=new_elevator_data)
 ```
 
 #### Delete ClearanceItem
 
 ```python
 from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemType as cit
+from acslib.ccure.types import ObjectType
+
 # delete a door
-ccure_api = CcureAPI()
-response = ccure_api.clearance_item.delete(cit.DOOR, 5000)
+ccure = CcureAPI()
+response = ccure.clearance_item.delete(ObjectType.DOOR.complete, 5000)
+```
+
+### Other item types
+
+#### Search for CCure item
+
+```python
+from acslib import CcureAPI
+from acslib.ccure.filters import CcureFilter, NFUZZ
+
+# search for schedule objects by ObjectID
+ccure = CcureAPI()
+schedule_type_full = "SoftwareHouse.CrossFire.Common.Objects.TimeSpec"
+search_filter = CcureFilter()
+response = ccure.ccure_object.search(
+    object_type=schedule_type_full,
+    search_filter=search_filter,
+    terms=[5001]
+)
+```
+
+### Other common actions
+
+Use `ccure.action` to perform some common tasks like assigning or revoking clearances or getting personnel images.
+
+#### Assign a clearance
+
+```python
+from acslib import CcureAPI
+
+# assign clearances 5002 and 5003 to person 5005
+ccure = CcureAPI()
+response = ccure.action.personnel.assign_clearances(
+    personnel_id=5005,
+    clearance_ids=[5002, 5003],
+)
 ```
```

#### html2text {}

```diff
@@ -1,69 +1,79 @@
 # Access Control Systems Library
 _[_R_e_l_e_a_s_e_ _S_t_a_t_u_s_]A library for interacting with Access Control Systems like
 Genetec or Ccure9k. This is a work in progress and is not ready for production
 use. Currently development is heavily influenced by Ccure9k, but the goal is to
 abstract the differences between the two systems and provide a common interface
 for interacting with them.
 * Free software: MIT * Documentation:
-github.com/ncstate-sat/acslib> ## Features * Currently supports Search for
-`Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k *
-Supports search by custom fields. ## Usage ### Personnel #### Find a person by
-name ```python from acslib import CcureAPI ccure_api = CcureAPI() response =
-ccure_api.personnel.search("Roddy Piper".split()) ``` #### Find a person by
-custom field ```python from acslib import CcureAPI from acslib.ccure.filters
-import PersonnelFilter, FUZZ ccure_api = CcureAPI() search_filter =
-PersonnelFilter(lookups={"Text1": FUZZ}) response = ccure_api.personnel.search(
-["PER0892347"], search_filter=search_filter) ``` #### Update a personnel record
-```python from acslib import CcureAPI # change MiddleName and Text14 for the
-person with CCure ID 5001 ccure_api = CcureAPI() ccure_api.personnel.update
-(5001, {"Text14": "new text here", "MiddleName": "Shaquille"}) ``` #### Add new
-personnel record ```python from acslib import CcureAPI from acslib.ccure.types
-import PersonnelCreateData as pcd ccure_api = CcureAPI() new_person_data = pcd
-(FirstName="Kenny", LastName="Smith", Text1="001132808")
-ccure_api.personnel.create(new_person_data) ``` #### Delete a personnel record
-```python from acslib import CcureAPI # delete the personnel record with the
-CCure ID 6008 ccure_api = CcureAPI() ccure_api.personnel.delete(6008) ``` ###
-Clearance #### Find a Clearance by name ```python from acslib import CcureAPI
-ccure_api = CcureAPI() response = ccure_api.clearance.search(["suite", "door"])
-``` #### Find a Clearance by other field ```python from acslib import CcureAPI
-from acslib.ccure.filters import ClearanceFilter, NFUZZ # search by ObjectID
-ccure_api = CcureAPI() search_filter = ClearanceFilter(lookups={"ObjectID":
-NFUZZ}) response = ccure_api.clearance.search([8897],
+github.com/ncstate-sat/acslib> ## Features * Currently supports CRUD operations
+for `Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k,
+and all other Ccure object types. * Supports search by custom fields. ## Usage
+### Personnel #### Find a person by name ```python from acslib import CcureAPI
+ccure = CcureAPI() response = ccure.personnel.search("Roddy Piper".split()) ```
+#### Find a person by custom field ```python from acslib import CcureAPI from
+acslib.ccure.filters import PersonnelFilter, FUZZ ccure = CcureAPI()
+search_filter = PersonnelFilter(lookups={"Text1": FUZZ}) response =
+ccure.personnel.search(["PER0892347"], search_filter=search_filter) ``` ####
+Update a personnel record ```python from acslib import CcureAPI # change
+MiddleName and Text14 for the person with CCure ID 5001 ccure = CcureAPI()
+ccure.personnel.update(5001, {"Text14": "new text here", "MiddleName":
+"Shaquille"}) ``` #### Add new personnel record ```python from acslib import
+CcureAPI from acslib.ccure.types import PersonnelCreateData as pcd ccure =
+CcureAPI() new_person_data = pcd(FirstName="Kenny", LastName="Smith",
+Text1="001132808") ccure.personnel.create(new_person_data) ``` #### Delete a
+personnel record ```python from acslib import CcureAPI # delete the personnel
+record with the CCure ID 6008 ccure = CcureAPI() ccure.personnel.delete(6008)
+``` ### Clearance #### Find a Clearance by name ```python from acslib import
+CcureAPI ccure = CcureAPI() response = ccure.clearance.search(["suite",
+"door"]) ``` #### Find a Clearance by other field ```python from acslib import
+CcureAPI from acslib.ccure.filters import ClearanceFilter, NFUZZ # search by
+ObjectID ccure = CcureAPI() search_filter = ClearanceFilter(lookups=
+{"ObjectID": NFUZZ}) response = ccure.clearance.search([8897],
 search_filter=search_filter) ``` ### Credential #### Find all credentials
-```python from acslib import CcureAPI ccure_api = CcureAPI() response =
-ccure_api.credential.search() ``` #### Find a credential by name ```python from
-acslib import CcureAPI # fuzzy search by name ccure_api = CcureAPI() response =
-ccure_api.credential.search(["charles", "barkley"]) ``` #### Find a credential
-by other field ```python from acslib import CcureAPI from acslib.ccure.filters
-import CredentialFilter, NFUZZ # search by ObjectID ccure_api = CcureAPI()
+```python from acslib import CcureAPI ccure = CcureAPI() response =
+ccure.credential.search() ``` #### Find a credential by name ```python from
+acslib import CcureAPI # fuzzy search by name ccure = CcureAPI() response =
+ccure.credential.search(["charles", "barkley"]) ``` #### Find a credential by
+other field ```python from acslib import CcureAPI from acslib.ccure.filters
+import CredentialFilter, NFUZZ # search by ObjectID ccure = CcureAPI()
 search_filter = CredentialFilter(lookups={"ObjectID": NFUZZ}) response =
-ccure_api.credential.search([5001], search_filter=search_filter) ``` ####
-Update a credential ```python from acslib import CcureAPI # update CardInt1 for
-the credential with ObjectID 5001 ccure_api = CcureAPI() response =
-ccure_api.credential.update(5001, {"CardInt1": 12345}) ``` ### ClearanceItem
+ccure.credential.search([5001], search_filter=search_filter) ``` #### Update a
+credential ```python from acslib import CcureAPI # update CardInt1 for the
+credential with ObjectID 5001 ccure = CcureAPI() response =
+ccure.credential.update(5001, {"CardInt1": 12345}) ``` ### ClearanceItem
 Clearance items include "door" and "elevator." #### Find ClearanceItem by name
-```python from acslib import CcureAPI from acslib.ccure.types import
-ClearanceItemType as cit # fuzzy search for doors by name ccure_api = CcureAPI
-() response = ccure_api.clearance_item.search(cit.DOOR, ["hall", "interior"])
-``` #### Find ClearanceItem by other field ```python from acslib import
-CcureAPI from acslib.ccure.filters import ClearanceItemFilter, NFUZZ from
-acslib.ccure.types import ClearanceItemType as cit # search elevators by
-ObjectID ccure_api = CcureAPI() search_filter = ClearanceItemFilter(lookups=
-{"ObjectID": NFUZZ}) response = ccure_api.clearance_item.search(cit.ELEVATOR,
-[5000], search_filter=search_filter) ``` #### Update ClearanceItem ```python
-from acslib import CcureAPI from acslib.ccure.types import ClearanceItemType as
-cit # change a door's name ccure_api = CcureAPI() response =
-ccure_api.clearance_item.update(cit.DOOR, 5000, update_data={"Name": "new door
-name 123"}) ``` #### Create ClearanceItem ```python from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemCreateData, ClearanceItemType as
-cit # create a new elevator ccure_api = CcureAPI() new_elevator_data =
-ClearanceItemCreateData( Name="New elevator 1", Description="newest elevator in
-town", ParentID=5000,
+```python from acslib import CcureAPI from acslib.ccure.types import ObjectType
+# fuzzy search for doors by name ccure = CcureAPI() response =
+ccure.clearance_item.search(ObjectType.DOOR.complete, ["hall", "interior"]) ```
+#### Find ClearanceItem by other field ```python from acslib import CcureAPI
+from acslib.ccure.filters import ClearanceItemFilter, NFUZZ from
+acslib.ccure.types import ObjectType # search elevators by ObjectID ccure =
+CcureAPI() search_filter = ClearanceItemFilter(lookups={"ObjectID": NFUZZ})
+response = ccure.clearance_item.search(ObjectType.ELEVATOR.complete, [5000],
+search_filter=search_filter) ``` #### Update ClearanceItem ```python from
+acslib import CcureAPI from acslib.ccure.types import ObjectType # change a
+door's name ccure = CcureAPI() response = ccure.clearance_item.update
+(ObjectType.DOOR.complete, 5000, update_data={"Name": "new door name 123"}) ```
+#### Create ClearanceItem ```python from acslib import CcureAPI from
+acslib.ccure.types import ClearanceItemCreateData, ObjectType # create a new
+elevator ccure = CcureAPI() new_elevator_data = ClearanceItemCreateData
+( Name="New elevator 1", Description="newest elevator in town", ParentID=5000,
 ParentType="SoftwareHouse.NextGen.Common.SecurityObjects.iStarController",
 ControllerID=5000,
 ControllerClassType="SoftwareHouse.NextGen.Common.SecurityObjects.iStarController"
-) response = ccure_api.clearance_item.create(cit.ELEVATOR,
+) response = ccure.clearance_item.create(ObjectType.ELEVATOR.complete,
 create_data=new_elevator_data) ``` #### Delete ClearanceItem ```python from
-acslib import CcureAPI from acslib.ccure.types import ClearanceItemType as cit
-# delete a door ccure_api = CcureAPI() response =
-ccure_api.clearance_item.delete(cit.DOOR, 5000) ```
+acslib import CcureAPI from acslib.ccure.types import ObjectType # delete a
+door ccure = CcureAPI() response = ccure.clearance_item.delete
+(ObjectType.DOOR.complete, 5000) ``` ### Other item types #### Search for CCure
+item ```python from acslib import CcureAPI from acslib.ccure.filters import
+CcureFilter, NFUZZ # search for schedule objects by ObjectID ccure = CcureAPI()
+schedule_type_full = "SoftwareHouse.CrossFire.Common.Objects.TimeSpec"
+search_filter = CcureFilter() response = ccure.ccure_object.search
+( object_type=schedule_type_full, search_filter=search_filter, terms=[5001] )
+``` ### Other common actions Use `ccure.action` to perform some common tasks
+like assigning or revoking clearances or getting personnel images. #### Assign
+a clearance ```python from acslib import CcureAPI # assign clearances 5002 and
+5003 to person 5005 ccure = CcureAPI() response =
+ccure.action.personnel.assign_clearances( personnel_id=5005, clearance_ids=
+[5002, 5003], ) ```
```

### Comparing `acslib-0.1.8/acslib/base/connection.py` & `acslib-0.1.9/acslib/base/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,25 @@
     Exception raised on a failed request, including exceptions
     from the requests module and 400+ status codes
     """
 
     def __init__(self, status_code: int, log_message: str):
         self.status_code = status_code
         self.message = log_message
+        self.exception_name = "RequestException"
 
     def __str__(self):
-        return f"RequestException: {self.status_code} {self.message}"
+        return f"{self.exception_name}: {self.status_code} {self.message}"
+
+
+class ACSNotImplementedException(ACSRequestException):
+    def __init__(self, log_message: str):
+        self.status_code = status.HTTP_501_NOT_IMPLEMENTED
+        self.message = log_message
+        self.exception_name = "NotImplementedException"
 
 
 class ACSRequestMethod(Enum):
     GET = "get"
     POST = "post"
     PUT = "put"
     DELETE = "delete"
```

### Comparing `acslib-0.1.8/acslib/base/status.py` & `acslib-0.1.9/acslib/base/status.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/acslib/ccure/config.py` & `acslib-0.1.9/acslib/ccure/config.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/acslib/ccure/connection.py` & `acslib-0.1.9/acslib/ccure/connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/acslib/ccure/data_models.py` & `acslib-0.1.9/acslib/ccure/data_models.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/acslib/ccure/filters.py` & `acslib-0.1.9/acslib/ccure/filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,63 +24,61 @@
 RFUZZ = right_fuzz
 FUZZ = full_fuzz
 NFUZZ = no_fuzz
 
 PERSONNEL_LOOKUP_FIELDS = {"FirstName": FUZZ, "LastName": FUZZ}
 CLEARANCE_LOOKUP_FIELDS = {"Name": FUZZ}
 CREDENTIAL_LOOKUP_FIELDS = {"Name": FUZZ}
+CLEARANCE_ITEM_LOOKUP_FIELDS = {"Name": FUZZ}
 
 
-class SearchTypes(Enum):
-    PERSONNEL = "personnel"
-    CLEARANCE = "clearance"
-    CREDENTIAL = "credential"
-
-
-class BaseCcureFilter(ACSFilter):
+class CcureFilter(ACSFilter):
     """Base CCure Filter
     :param lookups: Dict containing searchable field names and their lookup functions
     :param outer_bool: Boolean operator to use between search terms
     :param inner_bool: Boolean operator to use between lookups
     :param term_operator: Term operator to use between field and a search term
     :attribute
     """
 
     def __init__(
         self,
-        lookups: dict[str, callable] = None,
+        lookups: dict[str, callable] = {"ObjectID": NFUZZ},
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
+        display_properties: list[str] = [],
     ):
         self.filter_fields = lookups
         self.outer_bool = outer_bool.value
         self.inner_bool = inner_bool.value
         self.term_operator = term_operator.value
         #: List of properties from CCURE to be included in the CCURE response
-        self.display_properties = []
+        self.display_properties = display_properties
 
     def _compile_term(self, term) -> str:
         """Get all parts of the query for one search term"""
         fields = [(field_name, lookup(term)) for field_name, lookup in self.filter_fields.items()]
         field_queries = [
             f"{field_name} {self.term_operator} '{lookup}'" for field_name, lookup in fields
         ]
         return f"({self.inner_bool.join(field_queries)})"
 
     def update_display_properties(self, properties: list[str]):
         if not isinstance(properties, list):
             raise TypeError("Properties must be a list of strings")
         self.display_properties += properties
 
-    def filter(self, search):
-        pass
+    def filter(self, search: list[str]) -> str:
+        if not isinstance(search, list):
+            raise TypeError("Search must be a list of strings")
+        return self.outer_bool.join(self._compile_term(term) for term in search)
 
 
-class PersonnelFilter(BaseCcureFilter):
+class PersonnelFilter(CcureFilter):
     """Basic CCure Personnel Filter
     :param lookups: Dict containing searchable field names and their lookup functions
     :param outer_bool: Boolean operator to use between search terms
     :param inner_bool: Boolean operator to use between lookups
     :param term_operator: Term operator to use between field and a search term
     :param display_properties: List of properties from CCure to be included in the CCure response
     :attribute
@@ -98,21 +96,16 @@
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
         self.display_properties = ["FirstName", "MiddleName", "LastName", "ObjectID"]
         if display_properties is not None:
             self.display_properties = display_properties
 
-    def filter(self, search: list[str]) -> str:
-        if not isinstance(search, list):
-            raise TypeError("Search must be a list of strings")
-        return self.outer_bool.join(self._compile_term(term) for term in search)
-
 
-class ClearanceFilter(BaseCcureFilter):
+class ClearanceFilter(CcureFilter):
     """Basic CCure Clearance Filter
     :param lookups: Dict containing searchable field names and their lookup functions
     :param outer_bool: Boolean operator to use between search terms
     :param inner_bool: Boolean operator to use between lookups
     :param term_operator: Term operator to use between field and a search term
     :param display_properties: List of properties from CCure to be included in the CCure response
     :attribute
@@ -130,21 +123,16 @@
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
         self.display_properties = ["Name"]
         if display_properties is not None:
             self.display_properties = display_properties
 
-    def filter(self, search: list[str]) -> str:
-        if not isinstance(search, list):
-            raise TypeError("Search must be a list of strings")
-        return self.outer_bool.join(self._compile_term(term) for term in search)
 
-
-class CredentialFilter(BaseCcureFilter):
+class CredentialFilter(CcureFilter):
     """Basic CCure Credential Filter
     :param lookups: Dict containing searchable field names and their lookup functions
     :param outer_bool: Boolean operator to use between search terms
     :param inner_bool: Boolean operator to use between lookups
     :param term_operator: Term operator to use between field and a search term
     :param display_properties: List of properties from CCure to be included in the CCure response
     :attribute
@@ -162,21 +150,16 @@
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
         self.display_properties = ["Name"]
         if display_properties is not None:
             self.display_properties = display_properties
 
-    def filter(self, search: list) -> str:
-        if not isinstance(search, list):
-            raise TypeError("`search` must be a list of search terms")
-        return self.outer_bool.join(self._compile_term(term) for term in search)
 
-
-class ClearanceItemFilter(BaseCcureFilter):
+class ClearanceItemFilter(CcureFilter):
     """Basic CCure ClearanceItem Filter
     :param lookups: Dict containing searchable field names and their lookup functions
     :param outer_bool: Boolean operator to use between search terms
     :param inner_bool: Boolean operator to use between lookups
     :param term_operator: Term operator to use between field and a search term
     :param display_properties: List of properties from CCure to be included in the CCure response
     :attribute
@@ -186,19 +169,14 @@
         self,
         lookups: Optional[dict[str, callable]] = None,
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
         display_properties: Optional[list[str]] = None,
     ):
-        self.filter_fields = lookups or CREDENTIAL_LOOKUP_FIELDS
+        self.filter_fields = lookups or CLEARANCE_ITEM_LOOKUP_FIELDS
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
         self.display_properties = ["Name"]
         if display_properties is not None:
             self.display_properties = display_properties
-
-    def filter(self, search: list) -> str:
-        if not isinstance(search, list):
-            raise TypeError("`search` must be a list of search terms")
-        return self.outer_bool.join(self._compile_term(term) for term in search)
```

### Comparing `acslib-0.1.8/acslib/ccure/tests/conftest.py` & `acslib-0.1.9/acslib/ccure/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/acslib/ccure/tests/test_base.py` & `acslib-0.1.9/acslib/ccure/tests/test_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from unittest.mock import patch
 
 import pytest
 
 from acslib.ccure.base import CcureACS, CcureConnection
-from acslib.ccure.filters import PersonnelFilter, SearchTypes
+from acslib.ccure import CcureAPI
+from acslib.ccure.filters import PersonnelFilter
 
 
 def test_default_ccure_acs(env_config, caplog):
     """Default picks up env vars."""
     ccure = CcureACS()
     assert ccure.config.base_url == "https://example.com/ccure"
     assert ccure.logger.name == "acslib.ccure.connection"
@@ -21,34 +22,27 @@
 
     cc_conn = CcureConnection(logger=logging.getLogger("test"))
     ccure = CcureACS(connection=cc_conn)
     assert ccure.logger.name == "test"
     assert "test:connection" in caplog.text
 
 
-@pytest.mark.skip(reason="ccure search no longer works this way")
-def test_default_ccure_search(env_config, personnel_response, caplog):
-    ccure = CcureACS()
-    with patch(
-        "acslib.ccure.base.CcureACS._search_people", return_value=personnel_response
-    ) as mock_search:
-        ccure.search(search_type=SearchTypes.PERSONNEL, terms=["test"])
-        mock_search.assert_called_with(["test"])
-    assert "Searching for personnel" in caplog.text
-
-
-@pytest.mark.skip(reason="ccure search no longer works this way")
-def test_ccure_search_with_filter(env_config, personnel_response, caplog):
-    ccure = CcureACS()
-    filter = PersonnelFilter()
-    with patch(
-        "acslib.ccure.base.CcureACS._search_people", return_value=personnel_response
-    ) as mock_search:
-        ccure.search(search_type=SearchTypes.PERSONNEL, terms=["test"], search_filter=filter)
-        mock_search.assert_called_with(["test"], filter)
+def test_ccure_personnel_search(env_config, personnel_response, ccure_connection, caplog):
+    ccure = CcureAPI(ccure_connection)
+    search_filter = PersonnelFilter(display_properties=["ObjectID", "FirstName"])
+    with patch("acslib.ccure.base.CcureACS.search", return_value=personnel_response) as mock_search:
+        ccure.personnel.search(terms=["test"], search_filter=search_filter)
+        mock_search.assert_called_with(
+            object_type="SoftwareHouse.NextGen.Common.SecurityObjects.Personnel",
+            search_filter=search_filter,
+            terms=["test"],
+            page_size=None,
+            page_number=1,
+            search_options=None,
+        )
     assert "Searching for personnel" in caplog.text
 
 
 @pytest.mark.skip(reason="ccure search no longer works this way")
 def test_invalid_search_type(env_config):
     class NewTypes(Enum):
         NEW = "new"
```

### Comparing `acslib-0.1.8/acslib/ccure/tests/test_config.py` & `acslib-0.1.9/acslib/ccure/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/acslib/ccure/tests/test_connection.py` & `acslib-0.1.9/acslib/ccure/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/acslib/ccure/tests/test_search.py` & `acslib-0.1.9/acslib/ccure/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/docs/installation.md` & `acslib-0.1.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/mkdocs.yml` & `acslib-0.1.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint` & `acslib-0.1.9/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb` & `acslib-0.1.9/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/notebooks/encode_investigation.ipynb` & `acslib-0.1.9/notebooks/encode_investigation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985416666666667%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'from acslib.ccure.types import CredentialCreateData, "*

 * *            "ObjectTypes\\n')], delete: [2]}}, 3: {'source': ['ObjectTypes.DOOR.complete']}}"}*

```diff
@@ -40,15 +40,15 @@
             "execution_count": 3,
             "id": "4521ec54-884b-4c19-adcf-e3169e3bfe4f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from acslib import CcureAPI\n",
                 "from acslib.ccure.search_filtering import ClearanceFilter, NFUZZ\n",
-                "from acslib.ccure.types import CredentialCreateData, ClearanceItemTypes\n",
+                "from acslib.ccure.types import CredentialCreateData, ObjectTypes\n",
                 "ccure_api = CcureAPI()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "af388e2c-fb70-4cf9-b95b-d9313fda648f",
@@ -62,15 +62,15 @@
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ClearanceItemTypes.DOOR.complete"
+                "ObjectTypes.DOOR.complete"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "9648a15f-2912-4604-8df0-04d95cea3053",
             "metadata": {},
```

### Comparing `acslib-0.1.8/pyproject.toml` & `acslib-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2, <4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "acslib"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     { name="Jeremy Gibson", email="jmgibso3@ncsu.edu" },
     { name="Luc Sanchez", email="lgsanche@ncsu.edu" },
     { name="Ryan Semmler", email="rsemmle@ncsu.edu" },
 ]
 description = "A library for interacting with Access Control Systems like Genetec or Ccure9k"
 readme = "README.md"
```

### Comparing `acslib-0.1.8/requirements/base/base.txt` & `acslib-0.1.9/requirements/base/base.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/requirements/dev/dev.txt` & `acslib-0.1.9/requirements/dev/dev.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.8/PKG-INFO` & `acslib-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acslib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for interacting with Access Control Systems like Genetec or Ccure9k
 Author-email: Jeremy Gibson <jmgibso3@ncsu.edu>, Luc Sanchez <lgsanche@ncsu.edu>, Ryan Semmler <rsemmle@ncsu.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0
 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev"
@@ -51,198 +51,235 @@
 
 * Free software: MIT
 * Documentation: <https://github.com/ncstate-sat/acslib>
 
 
 ## Features
 
-* Currently supports Search for `Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k
+* Currently supports CRUD operations for `Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k, and all other Ccure object types.
 * Supports search by custom fields.
 
 ## Usage
 
 ### Personnel
 
 #### Find a person by name
 
 ```python
 from acslib import CcureAPI
 
-ccure_api = CcureAPI()
-response = ccure_api.personnel.search("Roddy Piper".split())
+ccure = CcureAPI()
+response = ccure.personnel.search("Roddy Piper".split())
 ```
 
 #### Find a person by custom field
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.filters import PersonnelFilter, FUZZ
 
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 search_filter = PersonnelFilter(lookups={"Text1": FUZZ})
-response = ccure_api.personnel.search(["PER0892347"], search_filter=search_filter)
+response = ccure.personnel.search(["PER0892347"], search_filter=search_filter)
 ```
 
 #### Update a personnel record
 
 ```python
 from acslib import CcureAPI
 
 # change MiddleName and Text14 for the person with CCure ID 5001
-ccure_api = CcureAPI()
-ccure_api.personnel.update(5001, {"Text14": "new text here", "MiddleName": "Shaquille"})
+ccure = CcureAPI()
+ccure.personnel.update(5001, {"Text14": "new text here", "MiddleName": "Shaquille"})
 ```
 
 #### Add new personnel record
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.types import PersonnelCreateData as pcd
 
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 new_person_data = pcd(FirstName="Kenny", LastName="Smith", Text1="001132808")
-ccure_api.personnel.create(new_person_data)
+ccure.personnel.create(new_person_data)
 ```
 
 #### Delete a personnel record
 
 ```python
 from acslib import CcureAPI
 
 # delete the personnel record with the CCure ID 6008
-ccure_api = CcureAPI()
-ccure_api.personnel.delete(6008)
+ccure = CcureAPI()
+ccure.personnel.delete(6008)
 ```
 
 ### Clearance
 
 #### Find a Clearance by name
 
 ```python
 from acslib import CcureAPI
 
-ccure_api = CcureAPI()
-response = ccure_api.clearance.search(["suite", "door"])
+ccure = CcureAPI()
+response = ccure.clearance.search(["suite", "door"])
 ```
 
 #### Find a Clearance by other field
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.filters import ClearanceFilter, NFUZZ
 
 # search by ObjectID
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 search_filter = ClearanceFilter(lookups={"ObjectID": NFUZZ})
-response = ccure_api.clearance.search([8897], search_filter=search_filter)
+response = ccure.clearance.search([8897], search_filter=search_filter)
 ```
 
 ### Credential
 
 #### Find all credentials
 
 ```python
 from acslib import CcureAPI
 
-ccure_api = CcureAPI()
-response = ccure_api.credential.search()
+ccure = CcureAPI()
+response = ccure.credential.search()
 ```
 
 #### Find a credential by name
 
 ```python
 from acslib import CcureAPI
 
 # fuzzy search by name
-ccure_api = CcureAPI()
-response = ccure_api.credential.search(["charles", "barkley"])
+ccure = CcureAPI()
+response = ccure.credential.search(["charles", "barkley"])
 ```
 
 #### Find a credential by other field
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.filters import CredentialFilter, NFUZZ
 
 # search by ObjectID
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 search_filter = CredentialFilter(lookups={"ObjectID": NFUZZ})
-response = ccure_api.credential.search([5001], search_filter=search_filter)
+response = ccure.credential.search([5001], search_filter=search_filter)
 ```
 
 #### Update a credential
 
 ```python
 from acslib import CcureAPI
 
 # update CardInt1 for the credential with ObjectID 5001
-ccure_api = CcureAPI()
-response = ccure_api.credential.update(5001, {"CardInt1": 12345})
+ccure = CcureAPI()
+response = ccure.credential.update(5001, {"CardInt1": 12345})
 ```
 
 ### ClearanceItem
 
 Clearance items include "door" and "elevator."
 
 #### Find ClearanceItem by name
 
 ```python
 from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemType as cit
+from acslib.ccure.types import ObjectType
 
 # fuzzy search for doors by name
-ccure_api = CcureAPI()
-response = ccure_api.clearance_item.search(cit.DOOR, ["hall", "interior"])
+ccure = CcureAPI()
+response = ccure.clearance_item.search(ObjectType.DOOR.complete, ["hall", "interior"])
 ```
 
 #### Find ClearanceItem by other field
 
 ```python
 from acslib import CcureAPI
 from acslib.ccure.filters import ClearanceItemFilter, NFUZZ
-from acslib.ccure.types import ClearanceItemType as cit
+from acslib.ccure.types import ObjectType
 
 # search elevators by ObjectID
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 search_filter = ClearanceItemFilter(lookups={"ObjectID": NFUZZ})
-response = ccure_api.clearance_item.search(cit.ELEVATOR, [5000], search_filter=search_filter)
+response = ccure.clearance_item.search(ObjectType.ELEVATOR.complete, [5000], search_filter=search_filter)
 ```
 
 #### Update ClearanceItem
 
 ```python
 from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemType as cit
+from acslib.ccure.types import ObjectType
 # change a door's name
-ccure_api = CcureAPI()
-response = ccure_api.clearance_item.update(cit.DOOR, 5000, update_data={"Name": "new door name 123"})
+ccure = CcureAPI()
+response = ccure.clearance_item.update(ObjectType.DOOR.complete, 5000, update_data={"Name": "new door name 123"})
 ```
 
 #### Create ClearanceItem
 
 ```python
 from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemCreateData, ClearanceItemType as cit
+from acslib.ccure.types import ClearanceItemCreateData, ObjectType
 
 # create a new elevator
-ccure_api = CcureAPI()
+ccure = CcureAPI()
 new_elevator_data = ClearanceItemCreateData(
     Name="New elevator 1",
     Description="newest elevator in town",
     ParentID=5000,
     ParentType="SoftwareHouse.NextGen.Common.SecurityObjects.iStarController",
     ControllerID=5000,
     ControllerClassType="SoftwareHouse.NextGen.Common.SecurityObjects.iStarController"
 )
-response = ccure_api.clearance_item.create(cit.ELEVATOR, create_data=new_elevator_data)
+response = ccure.clearance_item.create(ObjectType.ELEVATOR.complete, create_data=new_elevator_data)
 ```
 
 #### Delete ClearanceItem
 
 ```python
 from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemType as cit
+from acslib.ccure.types import ObjectType
+
 # delete a door
-ccure_api = CcureAPI()
-response = ccure_api.clearance_item.delete(cit.DOOR, 5000)
+ccure = CcureAPI()
+response = ccure.clearance_item.delete(ObjectType.DOOR.complete, 5000)
+```
+
+### Other item types
+
+#### Search for CCure item
+
+```python
+from acslib import CcureAPI
+from acslib.ccure.filters import CcureFilter, NFUZZ
+
+# search for schedule objects by ObjectID
+ccure = CcureAPI()
+schedule_type_full = "SoftwareHouse.CrossFire.Common.Objects.TimeSpec"
+search_filter = CcureFilter()
+response = ccure.ccure_object.search(
+    object_type=schedule_type_full,
+    search_filter=search_filter,
+    terms=[5001]
+)
+```
+
+### Other common actions
+
+Use `ccure.action` to perform some common tasks like assigning or revoking clearances or getting personnel images.
+
+#### Assign a clearance
+
+```python
+from acslib import CcureAPI
+
+# assign clearances 5002 and 5003 to person 5005
+ccure = CcureAPI()
+response = ccure.action.personnel.assign_clearances(
+    personnel_id=5005,
+    clearance_ids=[5002, 5003],
+)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acslib Version: 0.1.8 Summary: A library for
+Metadata-Version: 2.1 Name: acslib Version: 0.1.9 Summary: A library for
 interacting with Access Control Systems like Genetec or Ccure9k Author-email:
 Jeremy Gibson
 ncsu.edu>, Luc Sanchez
 ncsu.edu>, Ryan Semmler
 ncsu.edu> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev" Requires-Dist: pytest-
@@ -23,69 +23,79 @@
 github.ncsu.edu/SAT/acslib Provides-Extra: dev # Access Control Systems Library
 _[_R_e_l_e_a_s_e_ _S_t_a_t_u_s_]A library for interacting with Access Control Systems like
 Genetec or Ccure9k. This is a work in progress and is not ready for production
 use. Currently development is heavily influenced by Ccure9k, but the goal is to
 abstract the differences between the two systems and provide a common interface
 for interacting with them.
 * Free software: MIT * Documentation:
-github.com/ncstate-sat/acslib> ## Features * Currently supports Search for
-`Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k *
-Supports search by custom fields. ## Usage ### Personnel #### Find a person by
-name ```python from acslib import CcureAPI ccure_api = CcureAPI() response =
-ccure_api.personnel.search("Roddy Piper".split()) ``` #### Find a person by
-custom field ```python from acslib import CcureAPI from acslib.ccure.filters
-import PersonnelFilter, FUZZ ccure_api = CcureAPI() search_filter =
-PersonnelFilter(lookups={"Text1": FUZZ}) response = ccure_api.personnel.search(
-["PER0892347"], search_filter=search_filter) ``` #### Update a personnel record
-```python from acslib import CcureAPI # change MiddleName and Text14 for the
-person with CCure ID 5001 ccure_api = CcureAPI() ccure_api.personnel.update
-(5001, {"Text14": "new text here", "MiddleName": "Shaquille"}) ``` #### Add new
-personnel record ```python from acslib import CcureAPI from acslib.ccure.types
-import PersonnelCreateData as pcd ccure_api = CcureAPI() new_person_data = pcd
-(FirstName="Kenny", LastName="Smith", Text1="001132808")
-ccure_api.personnel.create(new_person_data) ``` #### Delete a personnel record
-```python from acslib import CcureAPI # delete the personnel record with the
-CCure ID 6008 ccure_api = CcureAPI() ccure_api.personnel.delete(6008) ``` ###
-Clearance #### Find a Clearance by name ```python from acslib import CcureAPI
-ccure_api = CcureAPI() response = ccure_api.clearance.search(["suite", "door"])
-``` #### Find a Clearance by other field ```python from acslib import CcureAPI
-from acslib.ccure.filters import ClearanceFilter, NFUZZ # search by ObjectID
-ccure_api = CcureAPI() search_filter = ClearanceFilter(lookups={"ObjectID":
-NFUZZ}) response = ccure_api.clearance.search([8897],
+github.com/ncstate-sat/acslib> ## Features * Currently supports CRUD operations
+for `Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k,
+and all other Ccure object types. * Supports search by custom fields. ## Usage
+### Personnel #### Find a person by name ```python from acslib import CcureAPI
+ccure = CcureAPI() response = ccure.personnel.search("Roddy Piper".split()) ```
+#### Find a person by custom field ```python from acslib import CcureAPI from
+acslib.ccure.filters import PersonnelFilter, FUZZ ccure = CcureAPI()
+search_filter = PersonnelFilter(lookups={"Text1": FUZZ}) response =
+ccure.personnel.search(["PER0892347"], search_filter=search_filter) ``` ####
+Update a personnel record ```python from acslib import CcureAPI # change
+MiddleName and Text14 for the person with CCure ID 5001 ccure = CcureAPI()
+ccure.personnel.update(5001, {"Text14": "new text here", "MiddleName":
+"Shaquille"}) ``` #### Add new personnel record ```python from acslib import
+CcureAPI from acslib.ccure.types import PersonnelCreateData as pcd ccure =
+CcureAPI() new_person_data = pcd(FirstName="Kenny", LastName="Smith",
+Text1="001132808") ccure.personnel.create(new_person_data) ``` #### Delete a
+personnel record ```python from acslib import CcureAPI # delete the personnel
+record with the CCure ID 6008 ccure = CcureAPI() ccure.personnel.delete(6008)
+``` ### Clearance #### Find a Clearance by name ```python from acslib import
+CcureAPI ccure = CcureAPI() response = ccure.clearance.search(["suite",
+"door"]) ``` #### Find a Clearance by other field ```python from acslib import
+CcureAPI from acslib.ccure.filters import ClearanceFilter, NFUZZ # search by
+ObjectID ccure = CcureAPI() search_filter = ClearanceFilter(lookups=
+{"ObjectID": NFUZZ}) response = ccure.clearance.search([8897],
 search_filter=search_filter) ``` ### Credential #### Find all credentials
-```python from acslib import CcureAPI ccure_api = CcureAPI() response =
-ccure_api.credential.search() ``` #### Find a credential by name ```python from
-acslib import CcureAPI # fuzzy search by name ccure_api = CcureAPI() response =
-ccure_api.credential.search(["charles", "barkley"]) ``` #### Find a credential
-by other field ```python from acslib import CcureAPI from acslib.ccure.filters
-import CredentialFilter, NFUZZ # search by ObjectID ccure_api = CcureAPI()
+```python from acslib import CcureAPI ccure = CcureAPI() response =
+ccure.credential.search() ``` #### Find a credential by name ```python from
+acslib import CcureAPI # fuzzy search by name ccure = CcureAPI() response =
+ccure.credential.search(["charles", "barkley"]) ``` #### Find a credential by
+other field ```python from acslib import CcureAPI from acslib.ccure.filters
+import CredentialFilter, NFUZZ # search by ObjectID ccure = CcureAPI()
 search_filter = CredentialFilter(lookups={"ObjectID": NFUZZ}) response =
-ccure_api.credential.search([5001], search_filter=search_filter) ``` ####
-Update a credential ```python from acslib import CcureAPI # update CardInt1 for
-the credential with ObjectID 5001 ccure_api = CcureAPI() response =
-ccure_api.credential.update(5001, {"CardInt1": 12345}) ``` ### ClearanceItem
+ccure.credential.search([5001], search_filter=search_filter) ``` #### Update a
+credential ```python from acslib import CcureAPI # update CardInt1 for the
+credential with ObjectID 5001 ccure = CcureAPI() response =
+ccure.credential.update(5001, {"CardInt1": 12345}) ``` ### ClearanceItem
 Clearance items include "door" and "elevator." #### Find ClearanceItem by name
-```python from acslib import CcureAPI from acslib.ccure.types import
-ClearanceItemType as cit # fuzzy search for doors by name ccure_api = CcureAPI
-() response = ccure_api.clearance_item.search(cit.DOOR, ["hall", "interior"])
-``` #### Find ClearanceItem by other field ```python from acslib import
-CcureAPI from acslib.ccure.filters import ClearanceItemFilter, NFUZZ from
-acslib.ccure.types import ClearanceItemType as cit # search elevators by
-ObjectID ccure_api = CcureAPI() search_filter = ClearanceItemFilter(lookups=
-{"ObjectID": NFUZZ}) response = ccure_api.clearance_item.search(cit.ELEVATOR,
-[5000], search_filter=search_filter) ``` #### Update ClearanceItem ```python
-from acslib import CcureAPI from acslib.ccure.types import ClearanceItemType as
-cit # change a door's name ccure_api = CcureAPI() response =
-ccure_api.clearance_item.update(cit.DOOR, 5000, update_data={"Name": "new door
-name 123"}) ``` #### Create ClearanceItem ```python from acslib import CcureAPI
-from acslib.ccure.types import ClearanceItemCreateData, ClearanceItemType as
-cit # create a new elevator ccure_api = CcureAPI() new_elevator_data =
-ClearanceItemCreateData( Name="New elevator 1", Description="newest elevator in
-town", ParentID=5000,
+```python from acslib import CcureAPI from acslib.ccure.types import ObjectType
+# fuzzy search for doors by name ccure = CcureAPI() response =
+ccure.clearance_item.search(ObjectType.DOOR.complete, ["hall", "interior"]) ```
+#### Find ClearanceItem by other field ```python from acslib import CcureAPI
+from acslib.ccure.filters import ClearanceItemFilter, NFUZZ from
+acslib.ccure.types import ObjectType # search elevators by ObjectID ccure =
+CcureAPI() search_filter = ClearanceItemFilter(lookups={"ObjectID": NFUZZ})
+response = ccure.clearance_item.search(ObjectType.ELEVATOR.complete, [5000],
+search_filter=search_filter) ``` #### Update ClearanceItem ```python from
+acslib import CcureAPI from acslib.ccure.types import ObjectType # change a
+door's name ccure = CcureAPI() response = ccure.clearance_item.update
+(ObjectType.DOOR.complete, 5000, update_data={"Name": "new door name 123"}) ```
+#### Create ClearanceItem ```python from acslib import CcureAPI from
+acslib.ccure.types import ClearanceItemCreateData, ObjectType # create a new
+elevator ccure = CcureAPI() new_elevator_data = ClearanceItemCreateData
+( Name="New elevator 1", Description="newest elevator in town", ParentID=5000,
 ParentType="SoftwareHouse.NextGen.Common.SecurityObjects.iStarController",
 ControllerID=5000,
 ControllerClassType="SoftwareHouse.NextGen.Common.SecurityObjects.iStarController"
-) response = ccure_api.clearance_item.create(cit.ELEVATOR,
+) response = ccure.clearance_item.create(ObjectType.ELEVATOR.complete,
 create_data=new_elevator_data) ``` #### Delete ClearanceItem ```python from
-acslib import CcureAPI from acslib.ccure.types import ClearanceItemType as cit
-# delete a door ccure_api = CcureAPI() response =
-ccure_api.clearance_item.delete(cit.DOOR, 5000) ```
+acslib import CcureAPI from acslib.ccure.types import ObjectType # delete a
+door ccure = CcureAPI() response = ccure.clearance_item.delete
+(ObjectType.DOOR.complete, 5000) ``` ### Other item types #### Search for CCure
+item ```python from acslib import CcureAPI from acslib.ccure.filters import
+CcureFilter, NFUZZ # search for schedule objects by ObjectID ccure = CcureAPI()
+schedule_type_full = "SoftwareHouse.CrossFire.Common.Objects.TimeSpec"
+search_filter = CcureFilter() response = ccure.ccure_object.search
+( object_type=schedule_type_full, search_filter=search_filter, terms=[5001] )
+``` ### Other common actions Use `ccure.action` to perform some common tasks
+like assigning or revoking clearances or getting personnel images. #### Assign
+a clearance ```python from acslib import CcureAPI # assign clearances 5002 and
+5003 to person 5005 ccure = CcureAPI() response =
+ccure.action.personnel.assign_clearances( personnel_id=5005, clearance_ids=
+[5002, 5003], ) ```
```

