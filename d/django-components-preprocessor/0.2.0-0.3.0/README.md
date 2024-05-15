# Comparing `tmp/django_components_preprocessor-0.2.0.tar.gz` & `tmp/django_components_preprocessor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_components_preprocessor-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_components_preprocessor-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_components_preprocessor-0.2.0.tar` & `django_components_preprocessor-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0       40 2024-02-11 21:09:45.619261 django_components_preprocessor-0.2.0/.gitignore
--rw-r--r--   0        0        0     1078 2024-02-10 14:23:32.448117 django_components_preprocessor-0.2.0/LICENSE
--rw-r--r--   0        0        0     2540 2024-02-11 21:26:22.148717 django_components_preprocessor-0.2.0/README.md
--rw-r--r--   0        0        0      269 2024-05-08 09:06:54.345273 django_components_preprocessor-0.2.0/django_components_preprocessor/__init__.py
--rw-r--r--   0        0        0     2139 2024-05-08 09:06:41.005371 django_components_preprocessor-0.2.0/django_components_preprocessor/loader.py
--rw-r--r--   0        0        0      234 2024-02-11 09:11:14.890960 django_components_preprocessor-0.2.0/example/components/calendar/calendar.html
--rw-r--r--   0        0        0      739 2024-02-10 17:52:35.364550 django_components_preprocessor-0.2.0/example/components/calendar/calendar.py
--rw-r--r--   0        0        0      220 2024-02-10 20:33:10.955395 django_components_preprocessor-0.2.0/example/components/calendar/script.js
--rw-r--r--   0        0        0      103 2024-02-10 16:19:08.060871 django_components_preprocessor-0.2.0/example/components/calendar/style.css
--rw-r--r--   0        0        0        0 2024-02-10 14:07:33.826613 django_components_preprocessor-0.2.0/example/core/__init__.py
--rw-r--r--   0        0        0       63 2024-02-10 14:07:33.826613 django_components_preprocessor-0.2.0/example/core/admin.py
--rw-r--r--   0        0        0      140 2024-02-10 14:07:33.946612 django_components_preprocessor-0.2.0/example/core/apps.py
--rw-r--r--   0        0        0        0 2024-02-10 14:07:33.830613 django_components_preprocessor-0.2.0/example/core/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-02-10 14:07:33.826613 django_components_preprocessor-0.2.0/example/core/models.py
--rw-r--r--   0        0        0      454 2024-02-11 21:10:07.219098 django_components_preprocessor-0.2.0/example/core/templates/core/index.html
--rw-r--r--   0        0        0       60 2024-02-10 14:07:33.826613 django_components_preprocessor-0.2.0/example/core/tests.py
--rw-r--r--   0        0        0      102 2024-02-10 14:37:40.763307 django_components_preprocessor-0.2.0/example/core/views.py
--rw-r--r--   0        0        0        0 2024-02-10 14:07:12.758895 django_components_preprocessor-0.2.0/example/example/__init__.py
--rw-r--r--   0        0        0      391 2024-02-10 14:07:12.890894 django_components_preprocessor-0.2.0/example/example/asgi.py
--rw-r--r--   0        0        0     3764 2024-02-11 21:20:58.938695 django_components_preprocessor-0.2.0/example/example/settings.py
--rw-r--r--   0        0        0      168 2024-02-10 14:38:21.451500 django_components_preprocessor-0.2.0/example/example/urls.py
--rw-r--r--   0        0        0      391 2024-02-10 14:07:12.890894 django_components_preprocessor-0.2.0/example/example/wsgi.py
--rwxr-xr-x   0        0        0      663 2024-02-10 14:07:12.894894 django_components_preprocessor-0.2.0/example/manage.py
--rw-r--r--   0        0        0      538 2024-05-08 09:06:21.917511 django_components_preprocessor-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 django_components_preprocessor-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-02-11 21:09:45.619261 django_components_preprocessor-0.3.0/.gitignore
+-rw-r--r--   0        0        0        8 2024-05-15 14:55:09.222419 django_components_preprocessor-0.3.0/.python-version
+-rw-r--r--   0        0        0     1078 2024-02-10 14:23:32.448117 django_components_preprocessor-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2758 2024-05-15 14:53:41.307091 django_components_preprocessor-0.3.0/README.md
+-rw-r--r--   0        0        0      269 2024-05-15 14:53:52.663004 django_components_preprocessor-0.3.0/django_components_preprocessor/__init__.py
+-rw-r--r--   0        0        0     2356 2024-05-15 14:51:28.532084 django_components_preprocessor-0.3.0/django_components_preprocessor/loader.py
+-rw-r--r--   0        0        0      234 2024-02-11 09:11:14.890960 django_components_preprocessor-0.3.0/example/components/calendar/calendar.html
+-rw-r--r--   0        0        0      739 2024-02-10 17:52:35.364550 django_components_preprocessor-0.3.0/example/components/calendar/calendar.py
+-rw-r--r--   0        0        0      220 2024-02-10 20:33:10.955395 django_components_preprocessor-0.3.0/example/components/calendar/script.js
+-rw-r--r--   0        0        0      103 2024-02-10 16:19:08.060871 django_components_preprocessor-0.3.0/example/components/calendar/style.css
+-rw-r--r--   0        0        0        0 2024-02-10 14:07:33.826613 django_components_preprocessor-0.3.0/example/core/__init__.py
+-rw-r--r--   0        0        0       63 2024-02-10 14:07:33.826613 django_components_preprocessor-0.3.0/example/core/admin.py
+-rw-r--r--   0        0        0      140 2024-02-10 14:07:33.946612 django_components_preprocessor-0.3.0/example/core/apps.py
+-rw-r--r--   0        0        0        0 2024-02-10 14:07:33.830613 django_components_preprocessor-0.3.0/example/core/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-02-10 14:07:33.826613 django_components_preprocessor-0.3.0/example/core/models.py
+-rw-r--r--   0        0        0      454 2024-02-11 21:10:07.219098 django_components_preprocessor-0.3.0/example/core/templates/core/index.html
+-rw-r--r--   0        0        0       60 2024-02-10 14:07:33.826613 django_components_preprocessor-0.3.0/example/core/tests.py
+-rw-r--r--   0        0        0      102 2024-02-10 14:37:40.763307 django_components_preprocessor-0.3.0/example/core/views.py
+-rw-r--r--   0        0        0        0 2024-02-10 14:07:12.758895 django_components_preprocessor-0.3.0/example/example/__init__.py
+-rw-r--r--   0        0        0      391 2024-02-10 14:07:12.890894 django_components_preprocessor-0.3.0/example/example/asgi.py
+-rw-r--r--   0        0        0     3764 2024-02-11 21:20:58.938695 django_components_preprocessor-0.3.0/example/example/settings.py
+-rw-r--r--   0        0        0      168 2024-02-10 14:38:21.451500 django_components_preprocessor-0.3.0/example/example/urls.py
+-rw-r--r--   0        0        0      391 2024-02-10 14:07:12.890894 django_components_preprocessor-0.3.0/example/example/wsgi.py
+-rwxr-xr-x   0        0        0      663 2024-02-10 14:07:12.894894 django_components_preprocessor-0.3.0/example/manage.py
+-rw-r--r--   0        0        0      538 2024-05-08 09:06:21.917511 django_components_preprocessor-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 django_components_preprocessor-0.3.0/PKG-INFO
```

### Comparing `django_components_preprocessor-0.2.0/LICENSE` & `django_components_preprocessor-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.2.0/README.md` & `django_components_preprocessor-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 This project allows you to use regular HTML tags for your django-component components.
 
 ### Before
 
 ```
 {% component_block "calendar" attr="value" %}
-  {% component_block "header" %}
+  {% fill "header" %}
     Custom header
-  {% endcomponent_block %}
+  {% endfill %}
 {% encomponent_block %}
 ```
 
 ### After
 
 ```
 <calendar attr="value">
-  <header>
+  <calendar.header>
     Custom header
-  </header>
+  </calendar.header>
 </calendar>
 ```
 
 ## Installation
 
 - Install the package using pip:
 
@@ -67,14 +67,16 @@
 ```
 
 ## How it works
 
 Your templates will be preprocessed before being passed to the regular django template engine.
 The preprocessor will replace custom tags (i.e. `<calendar />`) with the regular django-component tags
 (i.e. `{% component "calendar" }`).
+Additionally, custom tags with dots (i.e. `<calendar.header />`) will be replaced with the regular django-component tags
+(i.e. `{% fill "header" %}`), where the slot name is the last part of the tag name split at the dot.
 The tags are matched by name and are case-sensitive.
 
 Currently, custom tags are found using regular expressions, which is obviously a bit whacky.
 It does however work for most cases, and is a lot more readable than the regular django-component tags.
 A more robust solution would be to use a proper HTML parser, but that's a bit overkill at this point in time.
 
 If, due to the limitations of the regular expressions, you find that the preprocessor doesn't work for your use case,
```

### Comparing `django_components_preprocessor-0.2.0/django_components_preprocessor/loader.py` & `django_components_preprocessor-0.3.0/django_components_preprocessor/loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,35 +11,44 @@
         self.loader = engine.find_template_loader(loader)
 
         # Monkey-patch the loader to replace component tags with template tags
         self.loader_get_contents = self.loader.get_contents
         self.loader.get_contents = self.get_contents
 
         # Prepare regular expressions for replacing tags
-        self.component_names = "|".join(registry.all().keys())
-        self.self_closing_tag_re = re.compile(f"<({self.component_names})([^>]*)/>")
-        self.opening_tag_re = re.compile(f"<({self.component_names})([^>]*)>")
-        self.closing_tag_re = re.compile(f"</({self.component_names})\s*>")
+        self.tags = "|".join(registry.all().keys())
+        self.self_closing_tag_re = re.compile(f"<({self.tags})([^>]*)/>")
+        self.opening_tag_re = re.compile(rf"<({self.tags})(\.(\w+))?([^>]*)>")
+        self.closing_tag_re = re.compile(rf"</({self.tags})(\.(\w+))?\s*>")
 
         super().__init__(engine)
 
     @staticmethod
     def replace_self_closing_tag(match):
         tag = match.group(1)
         args = match.group(2).replace("\n", " ")
         return f'{{% component "{tag}"{args} %}}{{% endcomponent %}}'
 
     @staticmethod
     def replace_opening_tag(match):
         tag = match.group(1)
-        args = match.group(2).replace("\n", " ")
+        slot = match.group(3)
+        args = match.group(4).replace("\n", " ")
+
+        if slot:
+            assert not args, "Slots cannot have attributes"
+            return f'{{% fill "{slot}" %}}' 
+
         return f'{{% component "{tag}"{args} %}}'
 
     @staticmethod
     def replace_closing_tag(match):
+        slot = match.group(3)
+        if slot:
+            return f"{{% endfill %}}"
         return "{% endcomponent %}"
 
     def get_contents(self, origin):
         contents = self.loader_get_contents(origin)
 
         contents = self.self_closing_tag_re.sub(self.replace_self_closing_tag, contents)
         contents = self.opening_tag_re.sub(self.replace_opening_tag, contents)
```

### Comparing `django_components_preprocessor-0.2.0/example/components/calendar/calendar.py` & `django_components_preprocessor-0.3.0/example/components/calendar/calendar.py`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.2.0/example/example/settings.py` & `django_components_preprocessor-0.3.0/example/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.2.0/example/manage.py` & `django_components_preprocessor-0.3.0/example/manage.py`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.2.0/pyproject.toml` & `django_components_preprocessor-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.2.0/PKG-INFO` & `django_components_preprocessor-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-components-preprocessor
-Version: 0.2.0
+Version: 0.3.0
 Summary: A preprocessor for Django templates that replaces custom HTML tags with component tags.
 Author-email: Fabian Binz <fabian.binz@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django-components >= 0.5
 Project-URL: Home, https://github.com/fbinz/django-components-preprocessor
 
@@ -16,27 +16,27 @@
 
 This project allows you to use regular HTML tags for your django-component components.
 
 ### Before
 
 ```
 {% component_block "calendar" attr="value" %}
-  {% component_block "header" %}
+  {% fill "header" %}
     Custom header
-  {% endcomponent_block %}
+  {% endfill %}
 {% encomponent_block %}
 ```
 
 ### After
 
 ```
 <calendar attr="value">
-  <header>
+  <calendar.header>
     Custom header
-  </header>
+  </calendar.header>
 </calendar>
 ```
 
 ## Installation
 
 - Install the package using pip:
 
@@ -77,14 +77,16 @@
 ```
 
 ## How it works
 
 Your templates will be preprocessed before being passed to the regular django template engine.
 The preprocessor will replace custom tags (i.e. `<calendar />`) with the regular django-component tags
 (i.e. `{% component "calendar" }`).
+Additionally, custom tags with dots (i.e. `<calendar.header />`) will be replaced with the regular django-component tags
+(i.e. `{% fill "header" %}`), where the slot name is the last part of the tag name split at the dot.
 The tags are matched by name and are case-sensitive.
 
 Currently, custom tags are found using regular expressions, which is obviously a bit whacky.
 It does however work for most cases, and is a lot more readable than the regular django-component tags.
 A more robust solution would be to use a proper HTML parser, but that's a bit overkill at this point in time.
 
 If, due to the limitations of the regular expressions, you find that the preprocessor doesn't work for your use case,
```

