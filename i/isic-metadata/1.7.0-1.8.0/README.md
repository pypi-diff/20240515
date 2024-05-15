# Comparing `tmp/isic_metadata-1.7.0.tar.gz` & `tmp/isic_metadata-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic_metadata-1.7.0.tar", last modified: Mon May 13 20:43:41 2024, max compression
+gzip compressed data, was "isic_metadata-1.8.0.tar", last modified: Wed May 15 20:34:43 2024, max compression
```

## Comparing `isic_metadata-1.7.0.tar` & `isic_metadata-1.8.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.593458 isic_metadata-1.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.597458 isic_metadata-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.597458 isic_metadata-1.7.0/isic_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/isic_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/isic_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 20:43:41.000000 isic_metadata-1.7.0/isic_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:41.601458 isic_metadata-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/test_dependent_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-13 20:43:26.000000 isic_metadata-1.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.857272 isic_metadata-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.849272 isic_metadata-1.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.853272 isic_metadata-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 20:34:43.857272 isic_metadata-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.853272 isic_metadata-1.8.0/isic_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/isic_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.857272 isic_metadata-1.8.0/isic_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 20:34:43.000000 isic_metadata-1.8.0/isic_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:34:43.857272 isic_metadata-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:43.853272 isic_metadata-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/test_dependent_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-15 20:34:31.000000 isic_metadata-1.8.0/tox.ini
```

### Comparing `isic_metadata-1.7.0/.github/workflows/ci.yml` & `isic_metadata-1.8.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/.github/workflows/release.yml` & `isic_metadata-1.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/.gitignore` & `isic_metadata-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/LICENSE` & `isic_metadata-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/PKG-INFO` & `isic_metadata-1.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.7.0
+Version: 1.8.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic_metadata-1.7.0/isic_metadata/__init__.py` & `isic_metadata-1.8.0/isic_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/isic_metadata/fields.py` & `isic_metadata-1.8.0/isic_metadata/fields.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/isic_metadata/metadata.py` & `isic_metadata-1.8.0/isic_metadata/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,23 @@
     MelMitoticIndexEnum,
     MelThickMm,
     MelTypeEnum,
     NevusTypeEnum,
     TBPTileTypeEnum,
 )
 
+"""
+IGNORE_RCM_MODEL_CHECKS is a special attribute that allows disabling RCM model checks. It's
+provided to allow batch checks to be performed on a set of metadata rows, some of which may
+not be valid on a row level. e.g. if a batch of metadata rows contains RCM case ids that are
+inconsistent with lesion ids, that ought to be validated even if the row with an RCM case id
+has a missing image_type for instance.
+"""
+IGNORE_RCM_MODEL_CHECKS = "_ignore_rcm_model_checks"
+
 CUSTOM_MESSAGES = {
     "enum": "Unsupported value for {loc}: '{value}'.",
     "int_parsing": "Unable to parse value as an integer.",
     "bool_parsing": "Unable to parse value as a boolean.",
     "float_parsing": "Unable to parse value as a number.",
     "greater_than_equal": "Number must be greater than or equal to {ge}.",
 }
@@ -151,14 +160,34 @@
                 "rcm_multiple_macroscopics",
                 "One or more RCM cases have multiple macroscopic images.",
                 {"examples": bad_rcm_cases[:5]},
             )
 
         return self
 
+    @model_validator(mode="after")
+    def check_rcm_case_at_most_one_lesion(self) -> MetadataBatch:
+        rcm_case_to_lesions: dict[str, set[str]] = defaultdict(set)
+
+        for item in self.items:
+            if item.rcm_case_id and item.lesion_id:
+                rcm_case_to_lesions[item.rcm_case_id].add(item.lesion_id)
+
+        bad_rcm_cases = [
+            rcm_case for rcm_case in rcm_case_to_lesions if len(rcm_case_to_lesions[rcm_case]) > 1
+        ]
+        if bad_rcm_cases:
+            raise PydanticCustomError(
+                "one_rcm_case_multiple_lesions",
+                "One or more RCM cases belong to multiple lesions.",
+                {"examples": bad_rcm_cases[:5]},
+            )
+
+        return self
+
 
 class MetadataRow(BaseModel):
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         # This is useful for patient/lesion id fields, which could be numeric
         coerce_numbers_to_str=True,
         # extra values should be gathered by build_extra, so there's no need to allow them here
@@ -206,14 +235,26 @@
 
     # Unused and undocumented
     marker_pen: bool | None = None
     hairy: bool | None = None
     blurry: bool | None = None
     color_tint: ColorTintEnum | None = None
 
+    __slots__ = (IGNORE_RCM_MODEL_CHECKS,)
+
+    # see https://github.com/pydantic/pydantic/issues/655#issuecomment-570312649 for details on
+    # implementing a private property to be used internally.
+    def __init__(self, **kwargs) -> None:
+        object.__setattr__(self, IGNORE_RCM_MODEL_CHECKS, False)
+
+        if IGNORE_RCM_MODEL_CHECKS in kwargs:
+            object.__setattr__(self, IGNORE_RCM_MODEL_CHECKS, kwargs.pop(IGNORE_RCM_MODEL_CHECKS))
+
+        super().__init__(**kwargs)
+
     # See https://github.com/samuelcolvin/pydantic/issues/2285 for more detail
     @model_validator(mode="before")
     @classmethod
     def build_extra(cls, values: dict[str, Any]) -> dict[str, Any]:
         structured_field_names = {field for field in cls.model_fields if field != "unstructured"}
 
         unstructured: dict[str, Any] = {}
@@ -310,14 +351,17 @@
                     field, "diagnosis", field2_value=self.diagnosis.value
                 )
 
         return self
 
     @model_validator(mode="after")
     def validate_rcm_fields(self) -> MetadataRow:
+        if getattr(self, IGNORE_RCM_MODEL_CHECKS):
+            return self
+
         if not self.rcm_case_id:
             return self
 
         if not self.image_type:
             raise error_missing_field("rcm_case_id", "image_type")
 
         if self.image_type != ImageTypeEnum.rcm_macroscopic:
```

### Comparing `isic_metadata-1.7.0/isic_metadata.egg-info/PKG-INFO` & `isic_metadata-1.8.0/isic_metadata.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.7.0
+Version: 1.8.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic_metadata-1.7.0/isic_metadata.egg-info/SOURCES.txt` & `isic_metadata-1.8.0/isic_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/pyproject.toml` & `isic_metadata-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/setup.py` & `isic_metadata-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/tests/test_batch.py` & `isic_metadata-1.8.0/tests/test_batch.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,7 +47,32 @@
 
     MetadataBatch(
         items=[
             MetadataRow(image_type="RCM: macroscopic", rcm_case_id="foo"),
             MetadataRow(image_type="RCM: macroscopic", rcm_case_id="bar"),
         ]
     )
+
+
+def test_rcm_cases_belong_to_same_lesion():
+    with pytest.raises(ValidationError) as excinfo:
+        MetadataBatch(
+            items=[
+                MetadataRow(
+                    rcm_case_id="foo", lesion_id="foolesion", _ignore_rcm_model_checks=True
+                ),
+                MetadataRow(
+                    rcm_case_id="foo", lesion_id="barlesion", _ignore_rcm_model_checks=True
+                ),
+            ]
+        )
+    assert len(excinfo.value.errors()) == 1
+    assert "belong to multiple lesions" in excinfo.value.errors()[0]["msg"]
+
+
+def test_blank_rcm_cases_dont_belong_to_same_lesion():
+    MetadataBatch(
+        items=[
+            MetadataRow(rcm_case_id="", lesion_id="foolesion"),
+            MetadataRow(rcm_case_id="", lesion_id="barlesion"),
+        ]
+    )
```

### Comparing `isic_metadata-1.7.0/tests/test_dependent_fields.py` & `isic_metadata-1.8.0/tests/test_dependent_fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,23 @@
         MetadataRow.model_validate({"rcm_case_id": "12345"})
     assert len(excinfo.value.errors()) == 1
     assert "rcm_case_id requires setting image_type" in excinfo.value.errors()[0]["msg"]
 
     MetadataRow.model_validate({"rcm_case_id": "12345", "image_type": "RCM: macroscopic"})
 
 
+def test_rcm_model_checks_disabling():
+    with pytest.raises(ValidationError) as excinfo:
+        MetadataRow(rcm_case_id="12345")
+    assert len(excinfo.value.errors()) == 1
+    assert "rcm_case_id requires setting image_type" in excinfo.value.errors()[0]["msg"]
+
+    MetadataRow(rcm_case_id="12345", _ignore_rcm_model_checks=True)
+
+
 def test_tbp_tile_type_requires_image_type_tbp_tile():
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow.model_validate({"tbp_tile_type": "2D"})
     assert len(excinfo.value.errors()) == 1
     assert "tbp_tile_type requires setting image_type" in excinfo.value.errors()[0]["msg"]
 
     MetadataRow.model_validate({"tbp_tile_type": "2D", "image_type": "TBP tile: close-up"})
```

### Comparing `isic_metadata-1.7.0/tests/test_fields.py` & `isic_metadata-1.8.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.7.0/tox.ini` & `isic_metadata-1.8.0/tox.ini`

 * *Files identical despite different names*

