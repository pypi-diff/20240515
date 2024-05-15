# Comparing `tmp/jupyterlab_translate-1.3.6.tar.gz` & `tmp/jupyterlab_translate-1.3.7.tar.gz`

## Comparing `jupyterlab_translate-1.3.6.tar` & `jupyterlab_translate-1.3.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/RELEASE.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/package.json
--rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/yarn.lock
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/.github/workflows/release_publish.yml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/__init__.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/api.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/cli.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/constants.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/contributors.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/converters.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/finder.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/gettext_extract.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/hooks.py
--rwxr-xr-x   0        0        0  3617291 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/index.js
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/plugin.py
--rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/pybabel_config.cfg
--rw-r--r--   0        0        0    22145 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/jupyterlab_translate/utils.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/dummy_pkg.patch
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/example.json
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/test_hatch_hook.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/test_utils.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/dummy_pkg/locale/dummy_pkg.pot
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/tests/dummy_pkg/src/documentwidget.ts
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/LICENSE.txt
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/README.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/RELEASE.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/package.json
+-rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/yarn.lock
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/.github/workflows/release_publish.yml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/__init__.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/api.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/cli.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/constants.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/contributors.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/converters.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/finder.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/gettext_extract.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/hooks.py
+-rwxr-xr-x   0        0        0  3617291 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/index.js
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/plugin.py
+-rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/pybabel_config.cfg
+-rw-r--r--   0        0        0    22275 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/jupyterlab_translate/utils.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/tests/dummy_pkg.patch
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/tests/example.json
+-rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/tests/test_hatch_hook.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/tests/test_utils.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/tests/dummy_pkg/locale/dummy_pkg.pot
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/tests/dummy_pkg/src/documentwidget.ts
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/README.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 jupyterlab_translate-1.3.7/PKG-INFO
```

### Comparing `jupyterlab_translate-1.3.6/CONTRIBUTING.md` & `jupyterlab_translate-1.3.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/package.json` & `jupyterlab_translate-1.3.7/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/yarn.lock` & `jupyterlab_translate-1.3.7/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/.github/workflows/release_publish.yml` & `jupyterlab_translate-1.3.7/.github/workflows/release_publish.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/.github/workflows/tests.yml` & `jupyterlab_translate-1.3.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/jupyterlab_translate/api.py` & `jupyterlab_translate-1.3.7/jupyterlab_translate/api.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/jupyterlab_translate/cli.py` & `jupyterlab_translate-1.3.7/jupyterlab_translate/cli.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/jupyterlab_translate/constants.py` & `jupyterlab_translate-1.3.7/jupyterlab_translate/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/jupyterlab_translate/contributors.py` & `jupyterlab_translate-1.3.7/jupyterlab_translate/contributors.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/jupyterlab_translate/converters.py` & `jupyterlab_translate-1.3.7/jupyterlab_translate/converters.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/jupyterlab_translate/finder.py` & `jupyterlab_translate-1.3.7/jupyterlab_translate/finder.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/jupyterlab_translate/index.js` & `jupyterlab_translate-1.3.7/jupyterlab_translate/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/jupyterlab_translate/utils.py` & `jupyterlab_translate-1.3.7/jupyterlab_translate/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,31 +104,35 @@
         locale: Locale
         template_url: Language pack template
         template_ref: Template git reference
     """
     if not check_locale(locale):
         raise Exception("Invalid locale!")
 
-    loc = babel.Locale.parse("nb_NO" if locale == "no_NO" else locale)
+    try:
+        loc = babel.Locale.parse("nb_NO" if locale == "no_NO" else locale)
+        language_name = loc.english_name
+    except babel.UnknownLocaleError:
+        language_name = "unknown"
 
     locale_dash = locale.replace("_", "-")
     pkg_dir = Path(output_dir) / f"jupyterlab-language-pack-{locale_dash}"
     pkg_dir.mkdir(parents=True, exist_ok=True)
     copier.run_auto(
         template_url,
         pkg_dir,
-        data={"locale": locale_dash, "language": loc.english_name, "version": version},
+        data={"locale": locale_dash, "language": language_name, "version": version},
         vcs_ref=template_ref,
     )
 
 
 def check_locale(locale: str) -> bool:
     """Check if a locale is a valid value."""
-    # Add exception for no_NO
-    if locale == "no_NO":
+    # Add exceptions
+    if locale in {"ach_UG", "no_NO"}:
         return True
 
     value = False
     try:
         babel.Locale.parse(locale)
         value = True
     except Exception as e:
@@ -303,19 +307,19 @@
     "title": _default_schema_context,
     "description": _default_schema_context,
     "properties/.*/title": _default_settings_context,
     "properties/.*/description": _default_settings_context,
     "definitions/.*/properties/.*/title": _default_settings_context,
     "definitions/.*/properties/.*/description": _default_settings_context,
     # JupyterLab-specific
-    "jupyter\.lab\.setting-icon-label": _default_settings_context,
-    "jupyter\.lab\.menus/.*/label": "menu",
-    "jupyter\.lab\.metadataforms/.*/label": "metadataforms",
-    "jupyter\.lab\.toolbars/.*/label": "toolbar",
-    "jupyter\.lab\.toolbars/.*/caption": "toolbar",
+    r"jupyter\.lab\.setting-icon-label": _default_settings_context,
+    r"jupyter\.lab\.menus/.*/label": "menu",
+    r"jupyter\.lab\.metadataforms/.*/label": "metadataforms",
+    r"jupyter\.lab\.toolbars/.*/label": "toolbar",
+    r"jupyter\.lab\.toolbars/.*/caption": "toolbar",
 }
 
 
 def _prepare_schema_patterns(schema: dict) -> Dict[Pattern, str]:
     selectors = {
         **DEFAULT_SCHEMA_SELECTORS,
         **{
```

### Comparing `jupyterlab_translate-1.3.6/tests/dummy_pkg.patch` & `jupyterlab_translate-1.3.7/tests/dummy_pkg.patch`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/tests/example.json` & `jupyterlab_translate-1.3.7/tests/example.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/tests/test_hatch_hook.py` & `jupyterlab_translate-1.3.7/tests/test_hatch_hook.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/tests/test_utils.py` & `jupyterlab_translate-1.3.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/tests/dummy_pkg/src/documentwidget.ts` & `jupyterlab_translate-1.3.7/tests/dummy_pkg/src/documentwidget.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/.gitignore` & `jupyterlab_translate-1.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/LICENSE.txt` & `jupyterlab_translate-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/README.md` & `jupyterlab_translate-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/pyproject.toml` & `jupyterlab_translate-1.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_translate-1.3.6/PKG-INFO` & `jupyterlab_translate-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-translate
-Version: 1.3.6
+Version: 1.3.7
 Summary: JupyterLab Language Pack Translations Helper
 Project-URL: homepage, https://github.com/jupyterlab/jupyterlab-translate
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2020 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

