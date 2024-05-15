# Comparing `tmp/PythonVuetifyMarkdown-0.1.4.tar.gz` & `tmp/pythonvuetifymarkdown-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PythonVuetifyMarkdown-0.1.4.tar", last modified: Mon Aug 24 13:20:44 2020, max compression
+gzip compressed data, was "pythonvuetifymarkdown-0.2.0.tar", last modified: Tue May 14 17:20:08 2024, max compression
```

## Comparing `PythonVuetifyMarkdown-0.1.4.tar` & `pythonvuetifymarkdown-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2020-08-24 13:20:44.083838 PythonVuetifyMarkdown-0.1.4/
--rw-rw-rw-   0        0        0     2804 2020-08-24 13:20:44.082838 PythonVuetifyMarkdown-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-08-24 13:20:44.081838 PythonVuetifyMarkdown-0.1.4/PythonVuetifyMarkdown.egg-info/
--rw-rw-rw-   0        0        0     2804 2020-08-24 13:20:43.000000 PythonVuetifyMarkdown-0.1.4/PythonVuetifyMarkdown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2020-08-24 13:20:44.000000 PythonVuetifyMarkdown-0.1.4/PythonVuetifyMarkdown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-08-24 13:20:43.000000 PythonVuetifyMarkdown-0.1.4/PythonVuetifyMarkdown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2020-08-24 13:20:43.000000 PythonVuetifyMarkdown-0.1.4/PythonVuetifyMarkdown.egg-info/requires.txt
--rw-rw-rw-   0        0        0       46 2020-08-24 13:20:43.000000 PythonVuetifyMarkdown-0.1.4/PythonVuetifyMarkdown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1966 2020-08-24 13:16:41.000000 PythonVuetifyMarkdown-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2020-08-24 13:20:44.082838 PythonVuetifyMarkdown-0.1.4/python_vuetify_markdown/
--rw-rw-rw-   0        0        0      943 2020-08-24 13:12:25.000000 PythonVuetifyMarkdown-0.1.4/python_vuetify_markdown/__init__.py
--rw-rw-rw-   0        0        0       42 2020-08-24 13:20:44.083838 PythonVuetifyMarkdown-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      799 2020-08-24 13:17:51.000000 PythonVuetifyMarkdown-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:20:08.540020 pythonvuetifymarkdown-0.2.0/
+-rw-rw-rw-   0        0        0     1090 2020-03-24 01:50:19.000000 pythonvuetifymarkdown-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3389 2024-05-14 17:20:08.539014 pythonvuetifymarkdown-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 17:20:08.539014 pythonvuetifymarkdown-0.2.0/PythonVuetifyMarkdown.egg-info/
+-rw-rw-rw-   0        0        0     3389 2024-05-14 17:20:08.000000 pythonvuetifymarkdown-0.2.0/PythonVuetifyMarkdown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-14 17:20:08.000000 pythonvuetifymarkdown-0.2.0/PythonVuetifyMarkdown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:20:08.000000 pythonvuetifymarkdown-0.2.0/PythonVuetifyMarkdown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 17:20:08.000000 pythonvuetifymarkdown-0.2.0/PythonVuetifyMarkdown.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       46 2024-05-14 17:20:08.000000 pythonvuetifymarkdown-0.2.0/PythonVuetifyMarkdown.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2846 2024-05-14 17:17:19.000000 pythonvuetifymarkdown-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 17:20:08.537510 pythonvuetifymarkdown-0.2.0/python_vuetify_markdown/
+-rw-rw-rw-   0        0        0     3733 2024-05-14 17:02:41.000000 pythonvuetifymarkdown-0.2.0/python_vuetify_markdown/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:20:08.540020 pythonvuetifymarkdown-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      799 2024-05-14 16:13:16.000000 pythonvuetifymarkdown-0.2.0/setup.py
```

### Comparing `PythonVuetifyMarkdown-0.1.4/PKG-INFO` & `pythonvuetifymarkdown-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 Metadata-Version: 2.1
 Name: PythonVuetifyMarkdown
-Version: 0.1.4
+Version: 0.2.0
 Summary: Adds Vuetify typography classes to various tags
 Home-page: https://gitlab.com/robertjauss/python-vuetify-markdown
 Author: Robert Jauss
 Author-email: robertjauss@gmail.com
-License: UNKNOWN
-Description: # Python Vuetify Markdown
-        
-        This is an extension for [Python-Markdown](https://github.com/Python-Markdown/markdown/) created for those who combine Python, Markdown, Vue, and Vuetify. I've been using this combination in several projects, and finally came across a need to process Markdown code, and keep it styled with Vuetify. Rather than McGuyver some solution in, I settled on a simple extension to do the heavy lifting.
-        
-        The code is dead simple, and can be modified or extended to fit your needs. 
-        
-        # Installation
-        <code>pip install PythonVuetifyMarkdown</code>
-        
-        # Usage
-        Here's a quick example of usage within a Django project. We have a Page model for custom pages, and a function to return the content parsed through Markdown.
-        
-        ```python
-        from django.db import models
-        from django.utils.html import mark_safe
-        import markdown
-        from python_vuetify_markdown import PythonVuetifyMarkdown
-        
-        
-        class Page(models.Model):
-            title = models.CharField(max_length=200)
-            body = models.TextField()
-        
-            def get_body_as_markdown(self):
-                return mark_safe(markdown.markdown(self.body, extensions=[PythonVuetifyMarkdown()]))
-        ```
-        
-        With this, you can create a Page object, and when displaying the body, you can use `Page.get_body_as_markdown()` to pass in the Markdown-formatted code.
-        
-        # Features
-        Currently, this extension modifies H1 to H6 tags and P tags. The styles can be found on the [Vuetify Typography page](https://vuetifyjs.com/en/styles/typography).
-        * **&lt;h1&gt;** &rarr; &lt;h1 class="text-h1"&gt;
-        * **&lt;h2&gt;** &rarr; &lt;h2 class="text-h2"&gt;
-        * **&lt;h3&gt;** &rarr; &lt;h3 class="text-h3"&gt;
-        * **&lt;h4&gt;** &rarr; &lt;h4 class="text-h4"&gt;
-        * **&lt;h5&gt;** &rarr; &lt;h5 class="text-h5"&gt;
-        * **&lt;h6&gt;** &rarr; &lt;h6 class="text-h6"&gt;
-        * **&lt;p&gt;** &rarr; &lt;p class="text-body-1"&gt;
-        
-        # Support
-        There is none. This is a small side project, like 30 minutes of research and work went into it. Good luck.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: markdown>=3.6
+
+# Python Vuetify Markdown
+
+This is an extension for [Python-Markdown](https://github.com/Python-Markdown/markdown/) created for those who combine Python, Markdown, Vue, and Vuetify. I've been using this combination in several projects, and finally came across a need to process Markdown code, and keep it styled with Vuetify. Rather than McGuyver some solution in, I settled on a simple extension to do the heavy lifting.
+
+The code is dead simple, and can be modified or extended to fit your needs. 
+
+# Installation
+<code>pip install PythonVuetifyMarkdown</code>
+
+# Usage
+Here's a quick example of usage within a Django project. We have a Page model for custom pages, and a function to return the content parsed through Markdown.
+
+```python
+from django.db import models
+from django.utils.html import mark_safe
+import markdown
+from python_vuetify_markdown import PythonVuetifyMarkdown
+
+
+class Page(models.Model):
+    title = models.CharField(max_length=200)
+    body = models.TextField()
+
+    def get_body_as_markdown(self):
+        return mark_safe(markdown.markdown(self.body, extensions=[PythonVuetifyMarkdown()]))
+```
+
+With this, you can create a Page object, and when displaying the body, you can use `Page.get_body_as_markdown()` to pass in the Markdown-formatted code.
+
+# Features
+Currently, this extension modifies several tags, and adds spoiler text functionality. The styles can be found on the [Vuetify Typography page](https://vuetifyjs.com/en/styles/typography).
+* **&lt;h1&gt;** &rarr; &lt;h1 class="text-h1"&gt;
+* **&lt;h2&gt;** &rarr; &lt;h2 class="text-h2"&gt;
+* **&lt;h3&gt;** &rarr; &lt;h3 class="text-h3"&gt;
+* **&lt;h4&gt;** &rarr; &lt;h4 class="text-h4"&gt;
+* **&lt;h5&gt;** &rarr; &lt;h5 class="text-h5"&gt;
+* **&lt;h6&gt;** &rarr; &lt;h6 class="text-h6"&gt;
+* **&lt;p&gt;** &rarr; &lt;p class="text-body-1"&gt;
+* **&lt;a&gt;** &rarr; &lt;a class="text-no-decoration"&gt;
+* **&ast;text&ast;** &rarr; &lt;span class="font-weight-medium"&gt;text&lt;/span&gt;
+* **&ast;&ast;text&ast;&ast;** &rarr; &lt;span class="font-weight-bold"&gt;text&lt;/span&gt;
+* **&ast;&ast;&ast;text&ast;&ast;&ast;** &rarr; &lt;span class="font-weight-black"&gt;text&lt;/span&gt;
+* **!text!** &rarr; &lt;span class="font-weight-light"&gt;text&lt;/span&gt;
+* **!!text!!** &rarr; &lt;span class="font-weight-thin"&gt;text&lt;/span&gt;
+* **&lowbar;text&lowbar;** &rarr; &lt;span class="font-italic"&gt;text&lt;/span&gt;
+* **&lowbar;&lowbar;text&lowbar;&lowbar;** &rarr; &lt;span class="font-decoration-underline"&gt;text&lt;/span&gt;
+* **--text--** &rarr; &lt;span class="font-decoration-line-through"&gt;text&lt;/span&gt;
+* **||text||** &rarr; "â–’â–’â–’â–’" normally, "text" on hover
+
+# Support
+There is none. This is a small side project, like 30 minutes of research and work went into it. Good luck.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PythonVuetifyMarkdown-0.1.4/PythonVuetifyMarkdown.egg-info/PKG-INFO` & `pythonvuetifymarkdown-0.2.0/PythonVuetifyMarkdown.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 Metadata-Version: 2.1
 Name: PythonVuetifyMarkdown
-Version: 0.1.4
+Version: 0.2.0
 Summary: Adds Vuetify typography classes to various tags
 Home-page: https://gitlab.com/robertjauss/python-vuetify-markdown
 Author: Robert Jauss
 Author-email: robertjauss@gmail.com
-License: UNKNOWN
-Description: # Python Vuetify Markdown
-        
-        This is an extension for [Python-Markdown](https://github.com/Python-Markdown/markdown/) created for those who combine Python, Markdown, Vue, and Vuetify. I've been using this combination in several projects, and finally came across a need to process Markdown code, and keep it styled with Vuetify. Rather than McGuyver some solution in, I settled on a simple extension to do the heavy lifting.
-        
-        The code is dead simple, and can be modified or extended to fit your needs. 
-        
-        # Installation
-        <code>pip install PythonVuetifyMarkdown</code>
-        
-        # Usage
-        Here's a quick example of usage within a Django project. We have a Page model for custom pages, and a function to return the content parsed through Markdown.
-        
-        ```python
-        from django.db import models
-        from django.utils.html import mark_safe
-        import markdown
-        from python_vuetify_markdown import PythonVuetifyMarkdown
-        
-        
-        class Page(models.Model):
-            title = models.CharField(max_length=200)
-            body = models.TextField()
-        
-            def get_body_as_markdown(self):
-                return mark_safe(markdown.markdown(self.body, extensions=[PythonVuetifyMarkdown()]))
-        ```
-        
-        With this, you can create a Page object, and when displaying the body, you can use `Page.get_body_as_markdown()` to pass in the Markdown-formatted code.
-        
-        # Features
-        Currently, this extension modifies H1 to H6 tags and P tags. The styles can be found on the [Vuetify Typography page](https://vuetifyjs.com/en/styles/typography).
-        * **&lt;h1&gt;** &rarr; &lt;h1 class="text-h1"&gt;
-        * **&lt;h2&gt;** &rarr; &lt;h2 class="text-h2"&gt;
-        * **&lt;h3&gt;** &rarr; &lt;h3 class="text-h3"&gt;
-        * **&lt;h4&gt;** &rarr; &lt;h4 class="text-h4"&gt;
-        * **&lt;h5&gt;** &rarr; &lt;h5 class="text-h5"&gt;
-        * **&lt;h6&gt;** &rarr; &lt;h6 class="text-h6"&gt;
-        * **&lt;p&gt;** &rarr; &lt;p class="text-body-1"&gt;
-        
-        # Support
-        There is none. This is a small side project, like 30 minutes of research and work went into it. Good luck.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: markdown>=3.6
+
+# Python Vuetify Markdown
+
+This is an extension for [Python-Markdown](https://github.com/Python-Markdown/markdown/) created for those who combine Python, Markdown, Vue, and Vuetify. I've been using this combination in several projects, and finally came across a need to process Markdown code, and keep it styled with Vuetify. Rather than McGuyver some solution in, I settled on a simple extension to do the heavy lifting.
+
+The code is dead simple, and can be modified or extended to fit your needs. 
+
+# Installation
+<code>pip install PythonVuetifyMarkdown</code>
+
+# Usage
+Here's a quick example of usage within a Django project. We have a Page model for custom pages, and a function to return the content parsed through Markdown.
+
+```python
+from django.db import models
+from django.utils.html import mark_safe
+import markdown
+from python_vuetify_markdown import PythonVuetifyMarkdown
+
+
+class Page(models.Model):
+    title = models.CharField(max_length=200)
+    body = models.TextField()
+
+    def get_body_as_markdown(self):
+        return mark_safe(markdown.markdown(self.body, extensions=[PythonVuetifyMarkdown()]))
+```
+
+With this, you can create a Page object, and when displaying the body, you can use `Page.get_body_as_markdown()` to pass in the Markdown-formatted code.
+
+# Features
+Currently, this extension modifies several tags, and adds spoiler text functionality. The styles can be found on the [Vuetify Typography page](https://vuetifyjs.com/en/styles/typography).
+* **&lt;h1&gt;** &rarr; &lt;h1 class="text-h1"&gt;
+* **&lt;h2&gt;** &rarr; &lt;h2 class="text-h2"&gt;
+* **&lt;h3&gt;** &rarr; &lt;h3 class="text-h3"&gt;
+* **&lt;h4&gt;** &rarr; &lt;h4 class="text-h4"&gt;
+* **&lt;h5&gt;** &rarr; &lt;h5 class="text-h5"&gt;
+* **&lt;h6&gt;** &rarr; &lt;h6 class="text-h6"&gt;
+* **&lt;p&gt;** &rarr; &lt;p class="text-body-1"&gt;
+* **&lt;a&gt;** &rarr; &lt;a class="text-no-decoration"&gt;
+* **&ast;text&ast;** &rarr; &lt;span class="font-weight-medium"&gt;text&lt;/span&gt;
+* **&ast;&ast;text&ast;&ast;** &rarr; &lt;span class="font-weight-bold"&gt;text&lt;/span&gt;
+* **&ast;&ast;&ast;text&ast;&ast;&ast;** &rarr; &lt;span class="font-weight-black"&gt;text&lt;/span&gt;
+* **!text!** &rarr; &lt;span class="font-weight-light"&gt;text&lt;/span&gt;
+* **!!text!!** &rarr; &lt;span class="font-weight-thin"&gt;text&lt;/span&gt;
+* **&lowbar;text&lowbar;** &rarr; &lt;span class="font-italic"&gt;text&lt;/span&gt;
+* **&lowbar;&lowbar;text&lowbar;&lowbar;** &rarr; &lt;span class="font-decoration-underline"&gt;text&lt;/span&gt;
+* **--text--** &rarr; &lt;span class="font-decoration-line-through"&gt;text&lt;/span&gt;
+* **||text||** &rarr; "â–’â–’â–’â–’" normally, "text" on hover
+
+# Support
+There is none. This is a small side project, like 30 minutes of research and work went into it. Good luck.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PythonVuetifyMarkdown-0.1.4/README.md` & `pythonvuetifymarkdown-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -24,18 +24,28 @@
     def get_body_as_markdown(self):
         return mark_safe(markdown.markdown(self.body, extensions=[PythonVuetifyMarkdown()]))
 ```
 
 With this, you can create a Page object, and when displaying the body, you can use `Page.get_body_as_markdown()` to pass in the Markdown-formatted code.
 
 # Features
-Currently, this extension modifies H1 to H6 tags and P tags. The styles can be found on the [Vuetify Typography page](https://vuetifyjs.com/en/styles/typography).
+Currently, this extension modifies several tags, and adds spoiler text functionality. The styles can be found on the [Vuetify Typography page](https://vuetifyjs.com/en/styles/typography).
 * **&lt;h1&gt;** &rarr; &lt;h1 class="text-h1"&gt;
 * **&lt;h2&gt;** &rarr; &lt;h2 class="text-h2"&gt;
 * **&lt;h3&gt;** &rarr; &lt;h3 class="text-h3"&gt;
 * **&lt;h4&gt;** &rarr; &lt;h4 class="text-h4"&gt;
 * **&lt;h5&gt;** &rarr; &lt;h5 class="text-h5"&gt;
 * **&lt;h6&gt;** &rarr; &lt;h6 class="text-h6"&gt;
 * **&lt;p&gt;** &rarr; &lt;p class="text-body-1"&gt;
+* **&lt;a&gt;** &rarr; &lt;a class="text-no-decoration"&gt;
+* **&ast;text&ast;** &rarr; &lt;span class="font-weight-medium"&gt;text&lt;/span&gt;
+* **&ast;&ast;text&ast;&ast;** &rarr; &lt;span class="font-weight-bold"&gt;text&lt;/span&gt;
+* **&ast;&ast;&ast;text&ast;&ast;&ast;** &rarr; &lt;span class="font-weight-black"&gt;text&lt;/span&gt;
+* **!text!** &rarr; &lt;span class="font-weight-light"&gt;text&lt;/span&gt;
+* **!!text!!** &rarr; &lt;span class="font-weight-thin"&gt;text&lt;/span&gt;
+* **&lowbar;text&lowbar;** &rarr; &lt;span class="font-italic"&gt;text&lt;/span&gt;
+* **&lowbar;&lowbar;text&lowbar;&lowbar;** &rarr; &lt;span class="font-decoration-underline"&gt;text&lt;/span&gt;
+* **--text--** &rarr; &lt;span class="font-decoration-line-through"&gt;text&lt;/span&gt;
+* **||text||** &rarr; "▒▒▒▒" normally, "text" on hover
 
 # Support
 There is none. This is a small side project, like 30 minutes of research and work went into it. Good luck.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

