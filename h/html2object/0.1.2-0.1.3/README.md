# Comparing `tmp/html2object-0.1.2.tar.gz` & `tmp/html2object-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2object-0.1.2.tar", last modified: Tue May 14 20:20:22 2024, max compression
+gzip compressed data, was "html2object-0.1.3.tar", last modified: Wed May 15 13:23:12 2024, max compression
```

## Comparing `html2object-0.1.2.tar` & `html2object-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:22.862776 html2object-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 20:20:14.000000 html2object-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-14 20:20:22.862776 html2object-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-14 20:20:14.000000 html2object-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:22.858776 html2object-0.1.2/html2object/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 20:20:14.000000 html2object-0.1.2/html2object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-14 20:20:14.000000 html2object-0.1.2/html2object/html2object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-14 20:20:14.000000 html2object-0.1.2/html2object/html_element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:22.862776 html2object-0.1.2/html2object.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-14 20:20:22.000000 html2object-0.1.2/html2object.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 20:20:22.000000 html2object-0.1.2/html2object.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:20:22.000000 html2object-0.1.2/html2object.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 20:20:22.000000 html2object-0.1.2/html2object.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:20:22.862776 html2object-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-14 20:20:14.000000 html2object-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:22.858776 html2object-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:20:14.000000 html2object-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-14 20:20:14.000000 html2object-0.1.2/tests/test_html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:12.097100 html2object-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 13:23:02.000000 html2object-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-15 13:23:12.097100 html2object-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 13:23:02.000000 html2object-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:12.093100 html2object-0.1.3/html2object/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 13:23:02.000000 html2object-0.1.3/html2object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-15 13:23:02.000000 html2object-0.1.3/html2object/html2object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-15 13:23:02.000000 html2object-0.1.3/html2object/html_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:12.097100 html2object-0.1.3/html2object.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-15 13:23:12.000000 html2object-0.1.3/html2object.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 13:23:12.000000 html2object-0.1.3/html2object.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:23:12.000000 html2object-0.1.3/html2object.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 13:23:12.000000 html2object-0.1.3/html2object.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:23:12.097100 html2object-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-15 13:23:02.000000 html2object-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:12.093100 html2object-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:02.000000 html2object-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 13:23:02.000000 html2object-0.1.3/tests/test_html2object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-15 13:23:02.000000 html2object-0.1.3/tests/test_html_element.py
```

### Comparing `html2object-0.1.2/LICENSE` & `html2object-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `html2object-0.1.2/PKG-INFO` & `html2object-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2object
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools to handle the CRUD of .html files as objects.
 Home-page: https://github.com/boterop/html2object
 Author: boterop
 Author-email: boterop22@gmail.com
 Keywords: html,utils,html_utils,html_element,html_parser,html_writer,html_reader,html_crud,html_object,html_file,html_utils.py,html_element.py,html_parser.py,html_writer.py,html_reader.py,html_crud.py,html_object.py,html_file.py,html2object,html2object.py,html2object.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `html2object-0.1.2/README.md` & `html2object-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `html2object-0.1.2/html2object/html2object.py` & `html2object-0.1.3/html2object/html2object.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,34 +19,27 @@
     )
 
 
 def get_name(html: str) -> str:
     return re.search(r"<([a-zA-Z][a-zA-Z0-9]*)\b", html).group().replace("<", "")
 
 
-def get_id(html: str) -> str:
-    id = re.search(r'id=[\'"]([^\'"]+)[\'"]', html)
-    if not id:
-        return ""
-    return id.group()
-
-
 def get_attributes(html: str) -> dict:
-    attribs = re.search(r"<([a-zA-Z][a-zA-Z0-9]*)\b([^>]*)>", html).group(2).strip()
+    attribs = re.search(r"<([a-zA-Z][a-zA-Z0-9]*)\b([^>]*)>", html)[2].strip()
     attribs_list = attribs.split(" ")
     attribs_list = _fix_attrs(attribs_list)
     attributes = {}
     last_key = ""
     for attr in attribs_list:
-        if attr != "" and attr != "/":
+        if attr not in ["", "/"]:
             attr_div = attr.strip().split("=", 1)
             key = attr_div[0]
             if len(attr_div) == 1:
                 key = last_key
-                value = attributes[key] + " " + attr_div[0]
+                value = f"{attributes[key]} {attr_div[0]}"
             else:
                 value = attr_div[1]
             last_key = key
             attributes[key] = value
     return attributes
 
 
@@ -64,28 +57,28 @@
         else:
             element_end += 1
             count += 1
         if element_end < 1:
             break
     for _ in range(count):
         html = re.sub(rf"<\/{name}>", "<remove>", html, 1)
+    (_, start_index) = re.search(rf"<{name}\b[^>]*>", html).span()
     (end_index, _) = re.search(rf"<\/{name}>", html).span()
     html = re.sub("<remove>", f"</{name}>", html)
     end_index = end_index - ((5 - len(name)) * count)
-    child = html[:end_index].replace(element, "").strip()
-    return child
+    return html[start_index:end_index].strip()
 
 
 def _fix_attrs(attrs: list) -> list:
     no_splitable = [",", ":", ";"]
     new_list = []
     mix = None
     for attr in attrs:
         if attr.strip() != "":
             if mix:
-                attr = mix + " " + attr
+                attr = f"{mix} {attr}"
                 mix = None
             if attr.strip()[-1] in no_splitable:
                 mix = attr
             else:
                 new_list.append(attr)
     return new_list
```

### Comparing `html2object-0.1.2/html2object/html_element.py` & `html2object-0.1.3/html2object/html_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         self.uuid = str(uuid.uuid4())
         self.parent = parent
         if html:
             self._parse(html)
             return
         self.id = id
         self.name = name
-        if id:
-            self.attributes = {"id": id, **attributes}
-        else:
-            self.attributes = attributes
+        self.attributes = {"id": id, **attributes} if id else attributes
         self.children = children
 
     def add_child(self, child: str | object) -> object:
         if not self.children:
             self.children = []
         if type(child) == HtmlElement:
             child.set_parent(self)
@@ -51,34 +48,29 @@
             pile = []
         if self.id == id:
             return self
         if self.uuid in pile:
             return None
         pile.append(self.uuid)
 
-        result = None
-        if self.parent:
-            result = self.parent.find_element_by_id(id, pile)
+        result = self.parent.find_element_by_id(id, pile) if self.parent else None
         if self.children and not result:
             for child in self.children:
                 result = (
                     None if type(child) == str else child.find_element_by_id(id, pile)
                 )
                 if result:
                     break
         return result
 
     def __str__(self) -> str:
         children_html = ""
-        children = self.children if self.children else []
+        children = self.children or []
         for child in children:
-            if type(child) is str:
-                children_html += child
-            else:
-                children_html += str(child)
+            children_html += child if type(child) is str else str(child)
             children_html += "\n"
         children_html = children_html.strip()
         attributes = (
             json.dumps(self.attributes, separators=(" ", "="))
             .replace("{", " ")
             .replace("}", "")
             .replace("'", "<single_quote>")
@@ -97,22 +89,21 @@
         element = html_u.get_element(html)
         self.name = html_u.get_name(element)
         self.attributes = html_u.get_attributes(element)
         self.id = self.attributes.get("id")
         if self.id:
             self.id = self.id.replace('"', "")
         children_html = html_u.get_child(html, name=self.name)
-        if children_html == None:
-            self.children = None
-        else:
+        self.children = None
+        if children_html is not None:
             self.children = []
             self._add_children(children_html)
 
     def _add_children(self, html: str):
-        if html == "":
+        if not html:
             return
         try:
             element = html_u.get_element(html)
             name = html_u.get_name(element)
             self.children.append(HtmlElement(html=html, parent=self))
             self._add_children(html_u.remove_element(html, name))
         except AttributeError as e:
```

### Comparing `html2object-0.1.2/html2object.egg-info/PKG-INFO` & `html2object-0.1.3/html2object.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2object
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools to handle the CRUD of .html files as objects.
 Home-page: https://github.com/boterop/html2object
 Author: boterop
 Author-email: boterop22@gmail.com
 Keywords: html,utils,html_utils,html_element,html_parser,html_writer,html_reader,html_crud,html_object,html_file,html_utils.py,html_element.py,html_parser.py,html_writer.py,html_reader.py,html_crud.py,html_object.py,html_file.py,html2object,html2object.py,html2object.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `html2object-0.1.2/setup.py` & `html2object-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="html2object",
-    version="0.1.2",
+    version="0.1.3",
     author="boterop",
     author_email="boterop22@gmail.com",
     description="Tools to handle the CRUD of .html files as objects.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/boterop/html2object",
     packages=find_packages(),
```

### Comparing `html2object-0.1.2/tests/test_html_element.py` & `html2object-0.1.3/tests/test_html_element.py`

 * *Files identical despite different names*

