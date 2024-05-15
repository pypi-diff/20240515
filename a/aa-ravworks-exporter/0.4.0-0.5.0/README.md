# Comparing `tmp/aa_ravworks_exporter-0.4.0.tar.gz` & `tmp/aa_ravworks_exporter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_ravworks_exporter-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_ravworks_exporter-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_ravworks_exporter-0.4.0.tar` & `aa_ravworks_exporter-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    35149 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/LICENSE
--rw-r--r--   0        0        0     1472 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/README.md
--rwxr-xr-x   0        0        0     1567 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      136 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/__init__.py
--rw-r--r--   0        0        0      531 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/__init__.py
--rw-r--r--   0        0        0      726 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/corptools.py
--rw-r--r--   0        0        0      753 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/memberaudit.py
--rw-r--r--   0        0        0      344 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/skill_settings.py
--rw-r--r--   0        0        0        0 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/__init__.py
--rw-r--r--   0        0        0     1850 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/structures.py
--rw-r--r--   0        0        0    10791 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/structures_settings.py
--rw-r--r--   0        0        0     2378 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/forms.py
--rw-r--r--   0        0        0        0 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/migrations/__init__.py
--rw-r--r--   0        0        0       29 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/models.py
--rw-r--r--   0        0        0      620 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/templates/ravworks_exporter/index.html
--rw-r--r--   0        0        0      142 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/urls.py
--rw-r--r--   0        0        0     2593 2024-05-12 10:06:42.947410 aa_ravworks_exporter-0.4.0/ravworks_exporter/views.py
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 aa_ravworks_exporter-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1472 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/README.md
+-rwxr-xr-x   0        0        0     1567 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      136 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/skills/__init__.py
+-rw-r--r--   0        0        0      726 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/skills/corptools.py
+-rw-r--r--   0        0        0      753 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/skills/memberaudit.py
+-rw-r--r--   0        0        0      344 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/skills/skill_settings.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/structures/__init__.py
+-rw-r--r--   0        0        0     1231 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/structures/corptools.py
+-rw-r--r--   0        0        0     1850 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/structures/structures.py
+-rw-r--r--   0        0        0    10791 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/structures/structures_settings.py
+-rw-r--r--   0        0        0     2540 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/forms.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/migrations/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/models.py
+-rw-r--r--   0        0        0      620 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/templates/ravworks_exporter/index.html
+-rw-r--r--   0        0        0      142 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/urls.py
+-rw-r--r--   0        0        0     2941 2024-05-15 15:52:29.251657 aa_ravworks_exporter-0.5.0/ravworks_exporter/views.py
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 aa_ravworks_exporter-0.5.0/PKG-INFO
```

### Comparing `aa_ravworks_exporter-0.4.0/LICENSE` & `aa_ravworks_exporter-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/README.md` & `aa_ravworks_exporter-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/pyproject.toml` & `aa_ravworks_exporter-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/ravworks_exporter/auth_hooks.py` & `aa_ravworks_exporter-0.5.0/ravworks_exporter/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/corptools.py` & `aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/skills/corptools.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/skills/memberaudit.py` & `aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/skills/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/structures.py` & `aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/structures/structures.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/ravworks_exporter/exporters/structures/structures_settings.py` & `aa_ravworks_exporter-0.5.0/ravworks_exporter/exporters/structures/structures_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/ravworks_exporter/forms.py` & `aa_ravworks_exporter-0.5.0/ravworks_exporter/forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 
 class ExportForm(forms.Form):
     config = forms.FileField(required=True, label='Config file')
     skills = forms.ChoiceField(required=False, label='Skills', choices=[
         (None, 'Do not export'),
     ])
-    structures = forms.BooleanField(initial=True, required=False, label='Structures')
+    structures = forms.ChoiceField(required=False, label='Structures', choices=[
+        (None, 'Do not export'),
+    ])
 
     def __init__(self, user, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        if 'structures' not in settings.INSTALLED_APPS:
-            self.fields['structures'].disabled = True
-            self.fields['structures'].initial = False
-            self.fields['structures'].label = 'Structures (not available)'
+        if 'structures' in settings.INSTALLED_APPS:
+            self.fields['structures'].choices = [*self.fields['structures'].choices, ('structures', 'Structures')]
 
         if 'memberaudit' in settings.INSTALLED_APPS and user.has_perm('memberaudit.basic_access'):
             from memberaudit.models import Character
 
             ownerships = (
                 user.character_ownerships
                 .filter(
@@ -58,8 +58,11 @@
             choices = [
                 (f"corptools-{ownership.character.character_id}", f"CorpTools - {ownership.character.character_name}")
                 for ownership in ownerships
             ]
 
             self.fields['skills'].choices = [*self.fields['skills'].choices, *choices]
 
+            self.fields['structures'].choices = [*self.fields['structures'].choices, ('corptools', 'CorpTools')]
+
         self.fields['skills'].initial = self.fields['skills'].choices[-1][0]
+        self.fields['structures'].initial = self.fields['structures'].choices[-1][0]
```

### Comparing `aa_ravworks_exporter-0.4.0/ravworks_exporter/templates/ravworks_exporter/index.html` & `aa_ravworks_exporter-0.5.0/ravworks_exporter/templates/ravworks_exporter/index.html`

 * *Files identical despite different names*

### Comparing `aa_ravworks_exporter-0.4.0/ravworks_exporter/views.py` & `aa_ravworks_exporter-0.5.0/ravworks_exporter/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,15 +44,21 @@
                     if not is_character_added(character):
                         messages.error(request, f"Character {character.character_name} is not added to CorpTools")
                         error = True
                     else:
                         config.update(import_skills(character))
 
             if form.cleaned_data['structures']:
-                from .exporters.structures.structures import export_structures
+                if 'structures' == form.cleaned_data['structures']:
+                    from .exporters.structures.structures import export_structures
+                elif 'corptools' == form.cleaned_data['structures']:
+                    from .exporters.structures.corptools import export_structures
+                else:
+                    messages.error(request, "Invalid structures app")
+                    error = True
 
                 config['hidden_my_structures'] = export_structures(request.user)
                 config['hidden_allocation_dict'] = {}
 
             if not error:
                 updated_config = ContentFile(json.dumps(config, indent=4).encode())
                 return FileResponse(updated_config, as_attachment=True, filename='config.json')
```

### Comparing `aa_ravworks_exporter-0.4.0/PKG-INFO` & `aa_ravworks_exporter-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-ravworks-exporter
-Version: 0.4.0
+Version: 0.5.0
 Summary: Ravworks config exporter for AllianceAuth
 Keywords: allianceauth,ravworks,allianceauth_ravworks,ravworks_exporter,ravworks_config,eveonline
 Author-email: Matteo Ghia <matteo.ghia@yahoo.it>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

