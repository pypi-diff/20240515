# Comparing `tmp/django_meili-0.0.2.tar.gz` & `tmp/django_meili-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_meili-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_meili-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_meili-0.0.2.tar` & `django_meili-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,37 @@
--rw-r--r--   0        0        0      968 2024-01-18 14:42:40.664521 django_meili-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3077 2024-01-16 16:48:20.440054 django_meili-0.0.2/.gitignore
--rw-r--r--   0        0        0       44 2024-01-16 16:48:20.440054 django_meili-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0     1086 2024-01-18 14:55:11.811119 django_meili-0.0.2/LICENSE
--rw-r--r--   0        0        0     3547 2024-01-18 14:57:37.237036 django_meili-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-01-16 17:09:11.049816 django_meili-0.0.2/demo/__init__.py
--rw-r--r--   0        0        0      385 2024-01-16 17:09:11.049816 django_meili-0.0.2/demo/asgi.py
--rw-r--r--   0        0        0     3267 2024-01-17 20:45:23.669361 django_meili-0.0.2/demo/settings.py
--rw-r--r--   0        0        0      760 2024-01-16 17:09:11.049816 django_meili-0.0.2/demo/urls.py
--rw-r--r--   0        0        0      385 2024-01-16 17:09:11.049816 django_meili-0.0.2/demo/wsgi.py
--rw-r--r--   0        0        0       74 2024-01-18 14:36:05.481743 django_meili-0.0.2/django_meili/__init__.py
--rw-r--r--   0        0        0     1867 2024-01-17 20:46:17.316148 django_meili-0.0.2/django_meili/_settings.py
--rw-r--r--   0        0        0     2050 2024-01-18 14:29:38.309945 django_meili-0.0.2/django_meili/apps.py
--rw-r--r--   0        0        0        0 2024-01-16 16:48:20.440054 django_meili-0.0.2/django_meili/migrations/__init__.py
--rw-r--r--   0        0        0     9004 2024-01-18 14:49:28.316635 django_meili-0.0.2/django_meili/models.py
--rw-r--r--   0        0        0     1150 2024-01-18 14:32:17.710063 django_meili-0.0.2/django_meili/tests.py
--rw-r--r--   0        0        0    96233 2024-01-16 16:48:20.440054 django_meili-0.0.2/docs/Meilisearch_-_Django.jpg
--rwxr-xr-x   0        0        0      660 2024-01-16 17:09:11.049816 django_meili-0.0.2/manage.py
--rw-r--r--   0        0        0        0 2024-01-16 17:09:58.669807 django_meili-0.0.2/posts/__init__.py
--rw-r--r--   0        0        0      185 2024-01-17 20:44:31.376082 django_meili-0.0.2/posts/admin.py
--rw-r--r--   0        0        0      142 2024-01-16 17:09:58.669807 django_meili-0.0.2/posts/apps.py
--rw-r--r--   0        0        0      659 2024-01-17 20:46:41.576683 django_meili-0.0.2/posts/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-01-16 17:09:58.669807 django_meili-0.0.2/posts/migrations/__init__.py
--rw-r--r--   0        0        0      560 2024-01-17 21:06:10.706792 django_meili-0.0.2/posts/models.py
--rw-r--r--   0        0        0       60 2024-01-16 17:09:58.669807 django_meili-0.0.2/posts/tests.py
--rw-r--r--   0        0        0       63 2024-01-16 17:09:58.669807 django_meili-0.0.2/posts/views.py
--rw-r--r--   0        0        0      608 2024-01-16 16:57:36.409948 django_meili-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      261 2024-01-16 16:48:20.440054 django_meili-0.0.2/requirements.txt
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 django_meili-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      997 2024-05-14 22:09:47.297676 django_meili-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3077 2024-05-14 22:09:47.297676 django_meili-0.0.3/.gitignore
+-rw-r--r--   0        0        0       44 2024-05-14 22:09:47.297676 django_meili-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1086 2024-05-14 22:09:47.297676 django_meili-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3944 2024-05-14 22:09:47.297676 django_meili-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 22:09:47.297676 django_meili-0.0.3/demo/__init__.py
+-rw-r--r--   0        0        0      385 2024-05-14 22:09:47.297676 django_meili-0.0.3/demo/asgi.py
+-rw-r--r--   0        0        0     3267 2024-05-14 22:09:47.297676 django_meili-0.0.3/demo/settings.py
+-rw-r--r--   0        0        0      760 2024-05-14 22:09:47.297676 django_meili-0.0.3/demo/urls.py
+-rw-r--r--   0        0        0      385 2024-05-14 22:09:47.297676 django_meili-0.0.3/demo/wsgi.py
+-rw-r--r--   0        0        0       74 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/__init__.py
+-rw-r--r--   0        0        0     3698 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/_client.py
+-rw-r--r--   0        0        0     1867 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/_settings.py
+-rw-r--r--   0        0        0     3325 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/apps.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/management/commands/__init__.py
+-rw-r--r--   0        0        0      696 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/management/commands/clearindex.py
+-rw-r--r--   0        0        0     2089 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/management/commands/syncindex.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/migrations/__init__.py
+-rw-r--r--   0        0        0     5210 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/models.py
+-rw-r--r--   0        0        0     9834 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/querysets.py
+-rw-r--r--   0        0        0     2458 2024-05-14 22:09:47.297676 django_meili-0.0.3/django_meili/tests.py
+-rw-r--r--   0        0        0    96233 2024-05-14 22:09:47.297676 django_meili-0.0.3/docs/Meilisearch_-_Django.jpg
+-rwxr-xr-x   0        0        0      660 2024-05-14 22:09:47.297676 django_meili-0.0.3/manage.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/admin.py
+-rw-r--r--   0        0        0      142 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/apps.py
+-rw-r--r--   0        0        0      659 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/migrations/0001_initial.py
+-rw-r--r--   0        0        0      582 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/migrations/0002_post_lat_post_lng.py
+-rw-r--r--   0        0        0      689 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/migrations/0003_postnogeo.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/migrations/__init__.py
+-rw-r--r--   0        0        0     1310 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/models.py
+-rw-r--r--   0        0        0       60 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/tests.py
+-rw-r--r--   0        0        0       63 2024-05-14 22:09:47.297676 django_meili-0.0.3/posts/views.py
+-rw-r--r--   0        0        0      608 2024-05-14 22:09:47.297676 django_meili-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      261 2024-05-14 22:09:47.297676 django_meili-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     4509 1970-01-01 00:00:00.000000 django_meili-0.0.3/PKG-INFO
```

### Comparing `django_meili-0.0.2/.github/workflows/python-publish.yml` & `django_meili-0.0.3/.github/workflows/python-publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -27,8 +27,11 @@
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install flit
     - name: Publish package
-      run: FLIT_USERNAME=__token__ FLIT_PASSWORD=${{ secrets.PYPI_API_SECRET }} python -m flit publish
+      run: python -m flit publish
+      env:
+        FLIT_USERNAME: __token__
+        FLIT_PASSWORD: ${{ secrets.PYPI_API_SECRET }}
```

### Comparing `django_meili-0.0.2/.gitignore` & `django_meili-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `django_meili-0.0.2/LICENSE` & `django_meili-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_meili-0.0.2/README.md` & `django_meili-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,109 @@
 # Django-Meili
 
 ![](./docs/Meilisearch_-_Django.jpg)
 
-A package to integrate Meilisearch with Django in a seamless way.
+A package to integrate Meilisearch with Django in a seamless way. This pacakge is tested on Meilisearch `v1.60`.
 
 ## Usage
-
-Set the following variables in `settings.py`.
-
-```python
-MEILISEARCH = {
-   "HOST": "localhost",
-   "PORT": 7700,
-   "HTTPS": False,
-   "MASTER_KEY": "...",
-   "SYNC": False, # Should Meilisearch action resolve before continuing
-}
-```
-
-Register the app in `INSTALLED_APPS`
-
+### Settings
+Update your `settings.py` file to include the following:
 ```python
 INSTALLED_APPS = [
-    ...,
+    # ...,  <--- Any 3rd Party code
     "django_meili",
-    ...,
+    # ...,  <--- All your modules
 ]
-```
 
-Just subclass `django_meili.models.IndexMixin`
+# ....
 
-```python
+MEILISEARCH = {}
+```
+You must define the `django_meili` application before any of your code that
+uses the application.
 
+### Example in Models
+Update a model to include the following:
+```python
 from django_meili.models import IndexMixin
+from django.db import models
 
 class Post(IndexMixin, models.Model):
-    id = models.UUIDField()
+    """Model definition for Post."""
+
     title = models.CharField(max_length=255)
     body = models.TextField()
 
-    # Attributes to handle in Meilisearch
-    displayed_fields = ("title", "body")
-    searchable_fields = ("title", "body")
+    class Meta:
+        """Meta definition for Post."""
+
+        verbose_name = "Post"
+        verbose_name_plural = "Posts"
+
+    class MeiliMeta:
+        filterable_fields = ("title",)
+        searchable_fields = ("id", "title", "body")
+        displayed_fields = ("id", "title", "body")
 
     def __str__(self):
         return self.title
 ```
 
-Then when you are ready to search this model, just use the built-in "queryset".
+### Searching
+Now you can search from meilisearch using `Model.meilisearch`:
 ```python
-Post.objects.create(title="Hello", body="World")
-posts = Post.meilisearch.search("hello") # Returns a Django Queryset of results
-print(posts.first()) # Hello
+Post.meilisearch.search("Hello World") # => <Queryset for Post>
 ```
 
 ## API
-
-### `django_meili.models.IndexQuerySet`
-
-This is a custom queryset built to mimic Django's queryset. Currently does not support `Q` objects, but that is a plan for the future.
-
-Methods:
-| Name | Description | Example |
-|------|-------------|---------|
-| **__getitem__** | Use slices to set limit and offset. The default is 20 and 0 respectively. | ```Post.meilisearch[:10]```
-| **count** | Return the total number of documents within the index. *Does not reflect the count for the search query* | ```Post.meilisearch.count()```
-| **order_by** | Takes a Django `order_by` parameter and sets a sort value based on that. Can take multiple sorts | ```Post.meilisearch.order_by("-likes")```
-| **filter** | Takes a Django filter query. Supports: `lte`, `gte`, `lt`, `gt`, `exact`, `in`, `range`, `isnull`, `exists` | `Post.meilisearch.filter(title__exact="Hello World")`
-| **matching_strategy** | Set the default strategy. Defaults to `last` | ```Post.meilisearch.matching_strategy('all')```
-| **attributes_to_search_on** | Choose what fields to search on, defaults to all. | `Post.meilisearch.attributes_to_search_on("title", "body")`
-| **search** | Executes the actual search. Takes an optional query and returns a Django Queryset of results | `Post.meilisearch.search()`
+### `MEILISEARCH` in `settings.py`
+These are the settings available to the package. The values
+show are the defaults.
+```python
+MEILISEARCH = {
+    'HTTPS': False, # Whether HTTPS is enabled for the meilisearch server
+    'HOST': 'localhost', # The host for the meilisearch server
+    'MASTER_KEY': None, # The master key for meilisearch. See https://www.meilisearch.com/docs/learn/security/basic_security for more detail
+    'PORT': 7700, # The port for the meilisearch server
+    'TIMEOUT': None, # The timeout to wait for when using sync meilisearch server
+    'CLIENT_AGENTS': None, # The client agents for the meilisearch server
+    'DEBUG': DEBUG, # Whether to throw exceptions on failed creation of documents
+    'SYNC': False, # Whether to execute operations to meilisearch in a synchronous manner (waiting for each rather than letting the task queue operate)
+}
+```
 
 ### `django_meili.models.IndexMixin`
 
-Subclass Parameters:
-
-| Name            | Type            | Description                                                          |
-| --------------- | --------------- | -------------------------------------------------------------------- |
-| **index_name**  | `Optional[str]` | The name of the index to generate. Defaults to `__name__` attribute. |
-| **primary_key** | `Optional[str]` | The primary key of the index. Defaults to `pk`.                      |
+The `IndexMixin` is how an index is defined on a model.
+To configure the `IndexMixin` define a class on the model called `MeiliMeta`.
+The `IndexMixin` defines two new properties on the model:
+1. `meilisearch` - The queryset used to search.
+2. `_meilisearch` - the `MeiliMeta` values available on the model.
+
+In addition, the `IndexMixin` defines three methods:
+1. `meili_filter()` - Should this row be synced in meilisearch
+2. `meili_serialize()` - How the model is serialized into a dictionary
+3. `meili_geo()` - What does the `_geo` column look like (optional)
 
-Attributes:
+#### `MeiliMeta`
+The listed values here are default values. The displayed, searchable, filterable, and sortable should all be iterables containing field names, see the example above.
 
-| Name                  | Type         | Description                                 |
-| --------------------- | ------------ | ------------------------------------------- |
-| **displayed_fields**  | `tuple[str]` | The fields to display. By default uses all. |
-| **searchable_fields** | `tuple[str]` | The fields to search. By default uses all.  |
-| **filterable_fields** | `tuple[str]` | The fields to filter. By default uses none. |
-| **meilisearch** | `django_meili.models.IndexQuerySet` | The queryset used for filtering and searching |
-
----
+```python
+class MeiliMeta:
+    displayed_fields = None # the fields displayed when querying meilisearch
+    searchable_fields = None # the searchable fields when querying meilisearch
+    filterable_fields = None # the fields available to filter by using meilisearch
+    sortable_fields = None # the fields that can be sorted by using meilisearch
+    supports_geo = False # Does the model support geolocation
+    index_name = "<model.__name__>" # the name of the meilisearch index
+    primary_key = "pk" # the primary key field for the index
+```
 
-Copyright 2024 Ian Kollipara <<ian.kollipara@cune.edu>>
+### `django_meili.querysets.IndexQuerySet`
+The queryset defines the searchable operations on the index.
+It attempts to mimic the django queryset API, but differs in 2 notable ways:
+1. To do geo-filtering, you pass a positional argument
+2. Not all queryset operations are implemented.
+
+## Contact
+If there are any issues, please feel free to make an issue.
+If you have suggested improvements, please make an issue where we can discuss.
```

### Comparing `django_meili-0.0.2/demo/settings.py` & `django_meili-0.0.3/demo/settings.py`

 * *Files identical despite different names*

### Comparing `django_meili-0.0.2/demo/urls.py` & `django_meili-0.0.3/demo/urls.py`

 * *Files identical despite different names*

### Comparing `django_meili-0.0.2/django_meili/_settings.py` & `django_meili-0.0.3/django_meili/_settings.py`

 * *Files identical despite different names*

### Comparing `django_meili-0.0.2/docs/Meilisearch_-_Django.jpg` & `django_meili-0.0.3/docs/Meilisearch_-_Django.jpg`

 * *Files identical despite different names*

### Comparing `django_meili-0.0.2/manage.py` & `django_meili-0.0.3/manage.py`

 * *Files identical despite different names*

### Comparing `django_meili-0.0.2/posts/migrations/0001_initial.py` & `django_meili-0.0.3/posts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_meili-0.0.2/posts/models.py` & `django_meili-0.0.3/posts/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,53 @@
 from django.db import models
-from django_meili.models import IndexMixin
+from django_meili.models import IndexMixin, MeiliGeo
 
 # Create your models here.
 
+class PostNoGeo(IndexMixin, models.Model):
+    """Model definition for Post."""
+
+    title = models.CharField(max_length=255)
+    body = models.TextField()
+
+    class Meta:
+        """Meta definition for Post."""
+
+        verbose_name = "Post"
+        verbose_name_plural = "Posts"
+
+    class MeiliMeta:
+        filterable_fields = ("title",)
+        searchable_fields = ("id", "title", "body")
+        displayed_fields = ("id", "title", "body")
+
+    def __str__(self):
+        return self.title
 
 class Post(IndexMixin, models.Model):
     """Model definition for Post."""
 
     title = models.CharField(max_length=255)
     body = models.TextField()
+    lat = models.FloatField()
+    lng = models.FloatField()
+
+    def meili_geo(self) -> MeiliGeo:
+        return {
+            "lat": self.lat,
+            "lng": self.lng,
+        }
 
     class Meta:
         """Meta definition for Post."""
 
         verbose_name = "Post"
         verbose_name_plural = "Posts"
 
-    filterable_fields = ("title",)
-    searchable_fields = ("id", "title", "body")
-    displayed_fields = ("id", "title", "body")
+    class MeiliMeta:
+        filterable_fields = ("title",)
+        searchable_fields = ("id", "title", "body")
+        displayed_fields = ("id", "title", "body")
+        supports_geo = True
 
     def __str__(self):
         return self.title
```

### Comparing `django_meili-0.0.2/pyproject.toml` & `django_meili-0.0.3/pyproject.toml`

 * *Files identical despite different names*

