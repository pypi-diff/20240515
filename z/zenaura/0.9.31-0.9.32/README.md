# Comparing `tmp/zenaura-0.9.31.tar.gz` & `tmp/zenaura-0.9.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.31.tar", last modified: Mon May 13 15:56:20 2024, max compression
+gzip compressed data, was "zenaura-0.9.32.tar", last modified: Wed May 15 14:26:19 2024, max compression
```

## Comparing `zenaura-0.9.31.tar` & `zenaura-0.9.32.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:56:20.881262 zenaura-0.9.31/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.31/LICENSE
--rw-rw-rw-   0        0        0     1557 2024-05-13 15:56:20.880262 zenaura-0.9.31/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2024-05-13 15:49:51.000000 zenaura-0.9.31/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 15:56:20.881262 zenaura-0.9.31/setup.cfg
--rw-rw-rw-   0        0        0      707 2024-05-13 15:55:30.000000 zenaura-0.9.31/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:56:20.873762 zenaura-0.9.31/tests/
--rw-rw-rw-   0        0        0     6329 2024-05-13 15:49:51.000000 zenaura-0.9.31/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4109 2024-05-11 18:58:32.000000 zenaura-0.9.31/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1131 2024-05-11 17:44:57.000000 zenaura-0.9.31/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.31/tests/test_observer.py
--rw-rw-rw-   0        0        0    15531 2024-05-13 15:49:51.000000 zenaura-0.9.31/tests/test_tags.py
--rw-rw-rw-   0        0        0    13311 2024-05-13 15:49:51.000000 zenaura-0.9.31/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:56:20.874262 zenaura-0.9.31/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-11 11:31:00.000000 zenaura-0.9.31/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:56:20.879762 zenaura-0.9.31/zenaura.egg-info/
--rw-rw-rw-   0        0        0     1557 2024-05-13 15:56:20.000000 zenaura-0.9.31/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-13 15:56:20.000000 zenaura-0.9.31/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:56:20.000000 zenaura-0.9.31/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 15:56:20.000000 zenaura-0.9.31/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 14:26:19.418076 zenaura-0.9.32/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.32/LICENSE
+-rw-rw-rw-   0        0        0     1557 2024-05-15 14:26:19.417577 zenaura-0.9.32/PKG-INFO
+-rw-rw-rw-   0        0        0     1152 2024-05-13 18:21:23.000000 zenaura-0.9.32/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:26:19.418076 zenaura-0.9.32/setup.cfg
+-rw-rw-rw-   0        0        0      707 2024-05-15 14:25:52.000000 zenaura-0.9.32/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:26:19.409942 zenaura-0.9.32/tests/
+-rw-rw-rw-   0        0        0     5956 2024-05-14 06:59:05.000000 zenaura-0.9.32/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4109 2024-05-13 16:55:02.000000 zenaura-0.9.32/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1131 2024-05-11 17:44:57.000000 zenaura-0.9.32/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.32/tests/test_observer.py
+-rw-rw-rw-   0        0        0    15530 2024-05-14 16:04:33.000000 zenaura-0.9.32/tests/test_tags.py
+-rw-rw-rw-   0        0        0    13029 2024-05-15 11:56:22.000000 zenaura-0.9.32/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:26:19.410442 zenaura-0.9.32/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-11 11:31:00.000000 zenaura-0.9.32/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:26:19.417079 zenaura-0.9.32/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     1557 2024-05-15 14:26:19.000000 zenaura-0.9.32/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-15 14:26:19.000000 zenaura-0.9.32/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:26:19.000000 zenaura-0.9.32/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 14:26:19.000000 zenaura-0.9.32/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.31/LICENSE` & `zenaura-0.9.32/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.31/PKG-INFO` & `zenaura-0.9.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.31
+Version: 0.9.32
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zenaura
```

### Comparing `zenaura-0.9.31/README.md` & `zenaura-0.9.32/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.31/setup.py` & `zenaura-0.9.32/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.31',
+    version='0.9.32',
     description="Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura'],
     install_requires=[
         # Add any dependencies here
     ],
```

### Comparing `zenaura-0.9.31/tests/test_compiler.py` & `zenaura-0.9.32/tests/test_compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,20 +49,14 @@
         self.assertEqual(result, "<div><span>Hello</span></div>")
     
     def test_sanitize_html(self):
         input_html = '<script>alert("XSS attack")</script>'
         result = compiler.sanitize(input_html)
         self.assertEqual(result, '&lt;script&gt;alert(&quot;XSS attack&quot;)&lt;/script&gt;')
 
-    def test_compile_with_component_name(self):
-        elm = Node("button")
-        elm.attributes.append(Attribute("onclick", "counter.handleClick"))
-        result = compiler.compile(elm, componentName="myButton", zenaura_dom_mode=False)
-        expected_output = '<button onclick="counter.handleClick"></button>'
-        self.assertEqual(result, expected_output)
 
     def test_process_attributes_with_keywords(self):
         attrs = [Attribute("styles", "my-button"), Attribute("id", "btn-1")]
         result = compiler.process_attributes(attrs)
         self.assertEqual(result, ' class="my-button" id="btn-1"')
 
     def test_compile_with_nested_elements(self):
```

#### html2text {}

```diff
@@ -20,19 +20,15 @@
 id="my-node" class="important"') def test_compile_with_children(self): div =
 Node("div") span = Node("span") span.children = [ "Hello" ] div.children.append
 (span) result = compiler.compile(div, zenaura_dom_mode=False) self.assertEqual
 (result, "
 Hello
 ") def test_sanitize_html(self): input_html = '
 ' result = compiler.sanitize(input_html) self.assertEqual(result,
-'<script>alert("XSS attack")</script>') def test_compile_with_component_name
-(self): elm = Node("button") elm.attributes.append(Attribute("onclick",
-"counter.handleClick")) result = compiler.compile(elm,
-componentName="myButton", zenaura_dom_mode=False) expected_output = ''
-self.assertEqual(result, expected_output) def
+'<script>alert("XSS attack")</script>') def
 test_process_attributes_with_keywords(self): attrs = [Attribute("styles", "my-
 button"), Attribute("id", "btn-1")] result = compiler.process_attributes(attrs)
 self.assertEqual(result, ' class="my-button" id="btn-1"') def
 test_compile_with_nested_elements(self): div = Node("div") span = Node("span")
 span.children = ["Hello"] div.children.append(span) result = compiler.compile
 (div, zenaura_dom_mode=False) self.assertEqual(result, "
 Hello
```

### Comparing `zenaura-0.9.31/tests/test_component_e2e.py` & `zenaura-0.9.32/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.31/tests/test_component_unit.py` & `zenaura-0.9.32/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.31/tests/test_observer.py` & `zenaura-0.9.32/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.31/tests/test_tags.py` & `zenaura-0.9.32/tests/test_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from zenaura.client.tags import Node, Attribute, HTMLTags
+from zenaura.client.tags import Node, Attribute, Builder
 import unittest
 
 class DataclassTests(unittest.TestCase):
 
 
     def test_attribute_creation(self):
         attribute = Attribute(key="test", value="test")
@@ -24,59 +24,59 @@
         child = Node(name="test")
         parent = Node(name="div")
         parent.children.append(child)
         self.assertTrue(child.nodeId)
         self.assertTrue(parent.nodeId)
 
     def test_node_builder(self):
-        node = HTMLTags().div \
+        node = Builder('div') \
             .with_attribute("test", "test") \
             .with_child(
                 Node(name="test")
             ).build()
         
         self.assertEqual(len(node.children), 1)
         self.assertEqual(len(node.attributes), 1)
         self.assertTrue(isinstance(node.children[0], Node ))
         self.assertTrue(isinstance(node.attributes[0], Attribute))
 
     def test_init(self):
-        tb = HTMLTags().div.build()
+        tb = Builder('div').build()
         self.assertEqual(tb.name, "div")
         self.assertEqual(tb.attributes, [])  
         self.assertEqual(tb.children, []) 
 
     def test_with_attribute(self):
-        tb = HTMLTags().p
+        tb = Builder('p')
         tb.with_attribute("id", "main-paragraph").build()
         self.assertEqual(tb.node.attributes[0].key, "id")
         self.assertEqual(tb.node.attributes[0].value, "main-paragraph")
 
 
     def test_with_styles(self):
-        tb = HTMLTags().p
+        tb = Builder('p')
         tb.with_styles({"color": "blue", "font-size": "16px"}).build()
         self.assertEqual(tb.node.attributes[0].key, "style")
         self.assertEqual(tb.node.attributes[0].value, "color:blue;font-size:16px")
 
     def test_with_class(self):
-        tb = HTMLTags().p
+        tb = Builder('p')
         tb.with_class("my-class").build() 
         self.assertEqual(tb.node.attributes[0].key, "class")
         self.assertEqual(tb.node.attributes[0].value, "my-class")
 
     def test_with_classes(self):
-        tb = HTMLTags().span
+        tb = Builder('span')
         tb.with_classes("highlighted", "bold").build()
         self.assertEqual(tb.node.attributes[0].key, "class")
         self.assertEqual(tb.node.attributes[0].value, "highlighted bold")
 
 
     def test_with_class_avoid_duplicates(self):
-        tb = HTMLTags().div
+        tb = Builder('div')
         tb.with_class("container").with_class("container").build()
         self.assertEqual(tb.node.attributes[0].key, "class")
         self.assertEqual(tb.node.attributes[0].value, "container")
 
     def test_node_to_html_with_nested_nodes(self):
         # Create a nested node structure
         node1 = Node("div")
```

### Comparing `zenaura-0.9.31/tests/test_zenaura_dom.py` & `zenaura-0.9.32/tests/test_zenaura_dom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import unittest
 from unittest.mock import patch, MagicMock
 from tests.mocks.browser_mocks import MockDocument, MockWindow
 from zenaura.client.tags import Node
 from zenaura.client.component import Component
+from zenaura.client.compiler import compiler
 
 sys.modules["pyscript"] = MagicMock()
 
 class TestDom(unittest.TestCase):
 
     @patch('pyscript.document')
     @patch('pyscript.window')
@@ -38,28 +39,31 @@
 	
     def test_search(self):
         prevTree = self.counter.node()
         # simulate search table mount manually for testing
         self.zenaura_dom.zen_dom_table[self.counter.componentId] = prevTree
         self.counter.set_state("test")
         newTree = self.counter.node()
-        diff = self.zenaura_dom.search(prevTree, newTree)
+        diff = self.zenaura_dom.search(prevTree, newTree, self.counter.componentId)
         # hader location on tree, effected by change
-        changedNodeId = prevTree.nodeId
-        self.assertEqual(changedNodeId, diff[0][0])
+        # do not be confused with this, please see docs on method
+        # here the changed node is in level 3, index 0 of the component
+        # see docs keyed UID algorithm.
+        changedNodeId = compiler.getKeyedUID(self.counter.componentId, 3, 0)
 
 
     def test_render(self):
         self.zenaura_dom.mount(self.counter)
         self.counter.set_state(self.counterState(count=1))
         self.zenaura_dom.render(self.counter)
         re_rendered = self.zenaura_dom.zen_dom_table[self.counter.componentId]
         # print end of line 
         print("\n")
-        self.assertEqual(re_rendered.children[0].children[0].children[0].children[0], f'Counter: {self.counterState(count=1)}')
+        # new data structure Data for data binding
+        self.assertEqual(re_rendered.children[0].children[0].children[0].children[0].content, f'Counter: {self.counterState(count=1)}')
 
     def test_update(self):
         prevTree = self.counter.node()
         newChildren = Node(name="div", children=["test"])
         updated = self.zenaura_dom.update(prevTree, prevTree.nodeId, newChildren)
         self.assertEqual(prevTree.children, newChildren.children)
 
@@ -94,72 +98,55 @@
         updated_tree = self.zenaura_dom.update(prev_tree, prev_tree.nodeId, new_children)
 
         
         self.assertEqual(updated_tree.children[0], new_children.children[0])
 
     def test_search_identical_trees(self):
         
-        prev_tree = Node(name="div", children=["test"])
-        new_tree = Node(name="div", children=["test"])
+        prev_tree = Node(name="div")
+        new_tree = Node(name="div")
         
         
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
+        diff = self.zenaura_dom.search(prev_tree, new_tree, "test")
 
         self.assertEqual(diff, [])
 
 
     def test_search_different_trees_with_nested_structure(self):
         prev_tree = Node(name="div", children=[Node(name="span", children=["test"])])
         new_tree = Node(name="div", children=[Node(name="span", children=["new test"])])
         
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
+        diff = self.zenaura_dom.search(prev_tree, new_tree, self.counter.componentId)
 
         self.assertNotEqual(diff, [])
 
     def test_search_identical_trees_with_empty_structure(self):
         prev_tree = Node(name="div", children=[])
         new_tree = Node(name="div", children=[])
         
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
+        diff = self.zenaura_dom.search(prev_tree, new_tree, self.counter.componentId)
 
         self.assertEqual(diff, [])
 
-    def test_search_different_trees_with_empty_structure(self):
-        prev_tree = Node(name="div", children=[])
-        new_tree = Node(name="div", children=[Node(name="span", children=["test"])])
-        
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
-
-        self.assertNotEqual(diff, [])
-
-
     def test_search_different_trees_with_nested_structure(self):
         prev_tree = Node(name="div", children=[Node(name="span", children=["test"])])
         new_tree = Node(name="div", children=[Node(name="span", children=["new test"])])
         
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
+        diff = self.zenaura_dom.search(prev_tree, new_tree, self.counter.componentId)
 
         self.assertNotEqual(diff, [])
 
     def test_search_identical_trees_with_empty_structure(self):
         prev_tree = Node(name="div", children=[])
         new_tree = Node(name="div", children=[])
         
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
+        diff = self.zenaura_dom.search(prev_tree, new_tree, self.counter.componentId)
 
         self.assertEqual(diff, [])
 
-    def test_search_different_trees_with_empty_structure(self):
-        prev_tree = Node(name="div", children=[])
-        new_tree = Node(name="div", children=[Node(name="span", children=["test"])])
-        
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
-
-        self.assertNotEqual(diff, [])
-
 
     def test_update_with_empty_prev_tree(self):
         prev_tree = Node(name="div", children=[])
         new_children = Node(name="div", children=["test"])
 
         updated_tree = self.zenaura_dom.update(prev_tree, prev_tree.nodeId, new_children)
 
@@ -183,15 +170,15 @@
 
 
 
     def test_search_and_update_different_trees_with_nested_structure(self):
         prev_tree = Node(name="div", children=[Node(name="span", children=["test"])])
         new_tree = Node(name="div", children=[Node(name="span", children=["new test"])])
         
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
+        diff = self.zenaura_dom.search(prev_tree, new_tree, self.counter.componentId)
         self.assertNotEqual(diff, [])
 
         updated_tree = self.zenaura_dom.update(prev_tree, prev_tree.nodeId, new_tree)
         # confusing i know this, but this is how it works
         # it should update the changed node with the new node
         # not the entire tree
         self.assertEqual(updated_tree.nodeId, prev_tree.nodeId)
@@ -199,25 +186,25 @@
         self.assertEqual(updated_tree.children[0].nodeId, prev_tree.children[0].nodeId)
         self.assertEqual(updated_tree.children[0].children[0], new_tree.children[0].children[0])
 
     def test_search_and_update_with_empty_trees(self):
         prev_tree = Node(name="div", children=[])
         new_tree = Node(name="div", children=[])
         
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
+        diff = self.zenaura_dom.search(prev_tree, new_tree, self.counter.componentId)
         self.assertEqual(diff, [])
 
         updated_tree = self.zenaura_dom.update(prev_tree, prev_tree.nodeId, new_tree)
         self.assertEqual(updated_tree.nodeId, prev_tree.nodeId)
 
 
     def test_search_method_returns_diff_nodes(self):
         prev_tree = Node("div")
         new_tree = Node("div")
-        diff = self.zenaura_dom.search(prev_tree, new_tree)
+        diff = self.zenaura_dom.search(prev_tree, new_tree, self.counter.componentId)
         # Assert that the search method returns the expected diff nodes
         assert diff == []
 
     # Graceful degradation: testing componentDidCatchError lifecycle method 
         
     def test_componentDidCatchError_with_custom_error_component(self):
         # Arrange
@@ -226,15 +213,15 @@
                 super().__init__()
                 self.error_message = error_message
             def node(self):
                 return Node("div", children=[Node("p", children=[str(self.error_message)])])
 
         class TestComponent(Component):
             def componentDidCatchError(self, error):
-                return CustomErrorComponent(error_message=error).node()
+                return CustomErrorComponent(error_message=error)
 
         test_component = TestComponent()
 
         self.zenaura_dom.componentDidCatchError(test_component, "Custom error message")
 
         self.assertEqual(self.zenaura_dom.zen_dom_table[test_component.componentId].children[0].children[0], "Custom error message")
 
@@ -298,16 +285,14 @@
             def node(self):
                 return Node("p")
             
         component = TestComponent()
 
         self.assertEqual(component.x, 0)
         self.zenaura_dom.mount(component)
-
-        self.assertEqual(component.componentId, self.zenaura_dom.mounted_component_id)
       
         self.assertEqual(component.x, 10)
 
 
     def test_component_did_update_without_componentDidUpdate_method(self):
         class TestComponent(Component):
             def node(self):
```

### Comparing `zenaura-0.9.31/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.32/zenaura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.31
+Version: 0.9.32
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zenaura
```

