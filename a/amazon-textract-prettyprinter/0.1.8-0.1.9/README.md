# Comparing `tmp/amazon-textract-prettyprinter-0.1.8.tar.gz` & `tmp/amazon-textract-prettyprinter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-prettyprinter-0.1.8.tar", last modified: Thu Nov 16 20:38:21 2023, max compression
+gzip compressed data, was "amazon-textract-prettyprinter-0.1.9.tar", last modified: Thu Feb  8 12:11:58 2024, max compression
```

## Comparing `amazon-textract-prettyprinter-0.1.8.tar` & `amazon-textract-prettyprinter-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-11-16 20:38:21.294826 amazon-textract-prettyprinter-0.1.8/
--rw-r--r--   0 schadem    (504) staff       (20)    10142 2022-09-08 17:40:40.000000 amazon-textract-prettyprinter-0.1.8/LICENSE
--rw-r--r--   0 schadem    (504) staff       (20)      161 2022-09-08 17:40:40.000000 amazon-textract-prettyprinter-0.1.8/MANIFEST.in
--rw-r--r--   0 schadem    (504) staff       (20)     7243 2023-11-16 20:38:21.294928 amazon-textract-prettyprinter-0.1.8/PKG-INFO
--rw-r--r--   0 schadem    (504) staff       (20)     5385 2023-11-16 20:37:50.000000 amazon-textract-prettyprinter-0.1.8/README.md
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-11-16 20:38:21.293612 amazon-textract-prettyprinter-0.1.8/amazon_textract_prettyprinter.egg-info/
--rw-r--r--   0 schadem    (504) staff       (20)     7243 2023-11-16 20:38:21.000000 amazon-textract-prettyprinter-0.1.8/amazon_textract_prettyprinter.egg-info/PKG-INFO
--rw-r--r--   0 schadem    (504) staff       (20)      515 2023-11-16 20:38:21.000000 amazon-textract-prettyprinter-0.1.8/amazon_textract_prettyprinter.egg-info/SOURCES.txt
--rw-r--r--   0 schadem    (504) staff       (20)        1 2023-11-16 20:38:21.000000 amazon-textract-prettyprinter-0.1.8/amazon_textract_prettyprinter.egg-info/dependency_links.txt
--rw-r--r--   0 schadem    (504) staff       (20)       83 2023-11-16 20:38:21.000000 amazon-textract-prettyprinter-0.1.8/amazon_textract_prettyprinter.egg-info/requires.txt
--rw-r--r--   0 schadem    (504) staff       (20)       22 2023-11-16 20:38:21.000000 amazon-textract-prettyprinter-0.1.8/amazon_textract_prettyprinter.egg-info/top_level.txt
--rw-r--r--   0 schadem    (504) staff       (20)      406 2023-11-16 20:38:21.295224 amazon-textract-prettyprinter-0.1.8/setup.cfg
--rw-r--r--   0 schadem    (504) staff       (20)     2106 2023-11-16 20:38:11.000000 amazon-textract-prettyprinter-0.1.8/setup.py
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-11-16 20:38:21.294667 amazon-textract-prettyprinter-0.1.8/textractprettyprinter/
--rw-r--r--   0 schadem    (504) staff       (20)      308 2023-11-16 20:37:50.000000 amazon-textract-prettyprinter-0.1.8/textractprettyprinter/__init__.py
--rw-r--r--   0 schadem    (504) staff       (20)       22 2023-11-16 20:38:11.000000 amazon-textract-prettyprinter-0.1.8/textractprettyprinter/_version.py
--rw-r--r--   0 schadem    (504) staff       (20)    28294 2023-11-16 20:32:08.000000 amazon-textract-prettyprinter-0.1.8/textractprettyprinter/t_pretty_print.py
--rw-r--r--   0 schadem    (504) staff       (20)    10901 2022-12-20 03:08:04.000000 amazon-textract-prettyprinter-0.1.8/textractprettyprinter/t_pretty_print_expense.py
--rw-r--r--   0 schadem    (504) staff       (20)    16647 2023-11-16 20:37:50.000000 amazon-textract-prettyprinter-0.1.8/textractprettyprinter/t_pretty_print_layout.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2024-02-08 12:11:58.133708 amazon-textract-prettyprinter-0.1.9/
+-rw-r--r--   0 schadem    (504) staff       (20)    10142 2022-09-08 17:40:40.000000 amazon-textract-prettyprinter-0.1.9/LICENSE
+-rw-r--r--   0 schadem    (504) staff       (20)      161 2022-09-08 17:40:40.000000 amazon-textract-prettyprinter-0.1.9/MANIFEST.in
+-rw-r--r--   0 schadem    (504) staff       (20)    10308 2024-02-08 12:11:58.133832 amazon-textract-prettyprinter-0.1.9/PKG-INFO
+-rw-r--r--   0 schadem    (504) staff       (20)     8258 2024-01-16 14:34:07.000000 amazon-textract-prettyprinter-0.1.9/README.md
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2024-02-08 12:11:58.131870 amazon-textract-prettyprinter-0.1.9/amazon_textract_prettyprinter.egg-info/
+-rw-r--r--   0 schadem    (504) staff       (20)    10308 2024-02-08 12:11:58.000000 amazon-textract-prettyprinter-0.1.9/amazon_textract_prettyprinter.egg-info/PKG-INFO
+-rw-r--r--   0 schadem    (504) staff       (20)      515 2024-02-08 12:11:58.000000 amazon-textract-prettyprinter-0.1.9/amazon_textract_prettyprinter.egg-info/SOURCES.txt
+-rw-r--r--   0 schadem    (504) staff       (20)        1 2024-02-08 12:11:58.000000 amazon-textract-prettyprinter-0.1.9/amazon_textract_prettyprinter.egg-info/dependency_links.txt
+-rw-r--r--   0 schadem    (504) staff       (20)       83 2024-02-08 12:11:58.000000 amazon-textract-prettyprinter-0.1.9/amazon_textract_prettyprinter.egg-info/requires.txt
+-rw-r--r--   0 schadem    (504) staff       (20)       22 2024-02-08 12:11:58.000000 amazon-textract-prettyprinter-0.1.9/amazon_textract_prettyprinter.egg-info/top_level.txt
+-rw-r--r--   0 schadem    (504) staff       (20)      406 2024-02-08 12:11:58.134179 amazon-textract-prettyprinter-0.1.9/setup.cfg
+-rw-r--r--   0 schadem    (504) staff       (20)     2106 2024-02-08 12:11:45.000000 amazon-textract-prettyprinter-0.1.9/setup.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2024-02-08 12:11:58.133523 amazon-textract-prettyprinter-0.1.9/textractprettyprinter/
+-rw-r--r--   0 schadem    (504) staff       (20)      308 2023-11-16 20:37:50.000000 amazon-textract-prettyprinter-0.1.9/textractprettyprinter/__init__.py
+-rw-r--r--   0 schadem    (504) staff       (20)       22 2024-02-08 12:11:45.000000 amazon-textract-prettyprinter-0.1.9/textractprettyprinter/_version.py
+-rw-r--r--   0 schadem    (504) staff       (20)    28294 2023-11-16 20:32:08.000000 amazon-textract-prettyprinter-0.1.9/textractprettyprinter/t_pretty_print.py
+-rw-r--r--   0 schadem    (504) staff       (20)    10901 2022-12-20 03:08:04.000000 amazon-textract-prettyprinter-0.1.9/textractprettyprinter/t_pretty_print_expense.py
+-rw-r--r--   0 schadem    (504) staff       (20)    16946 2024-02-08 12:11:28.000000 amazon-textract-prettyprinter-0.1.9/textractprettyprinter/t_pretty_print_layout.py
```

### Comparing `amazon-textract-prettyprinter-0.1.8/LICENSE` & `amazon-textract-prettyprinter-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-prettyprinter-0.1.8/amazon_textract_prettyprinter.egg-info/SOURCES.txt` & `amazon-textract-prettyprinter-0.1.9/amazon_textract_prettyprinter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-textract-prettyprinter-0.1.8/setup.py` & `amazon-textract-prettyprinter-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     os.system('python setup.py sdist bdist_wheel')
     os.system('twine check dist/*')
     os.system('twine upload --repository pypi dist/*')
     sys.exit()
 
 setup(name='amazon-textract-prettyprinter',
       packages=['textractprettyprinter'],
-      version='0.1.8',
+      version='0.1.9',
       description='Amazon Textract Helper tools for pretty printing',
       install_requires=requirements,
       long_description_content_type='text/markdown',
       long_description=read('README.md'),
       author='Amazon Rekognition Textract Demoes',
       author_email='rekognition-textract-demos@amazon.com',
       url='https://github.com/aws-samples/amazon-textract-textractor/tree/master/prettyprinter',
```

### Comparing `amazon-textract-prettyprinter-0.1.8/textractprettyprinter/t_pretty_print.py` & `amazon-textract-prettyprinter-0.1.9/textractprettyprinter/t_pretty_print.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-prettyprinter-0.1.8/textractprettyprinter/t_pretty_print_expense.py` & `amazon-textract-prettyprinter-0.1.9/textractprettyprinter/t_pretty_print_expense.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-prettyprinter-0.1.8/textractprettyprinter/t_pretty_print_layout.py` & `amazon-textract-prettyprinter-0.1.9/textractprettyprinter/t_pretty_print_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 continue
             
             # Handle LAYOUT_TABLE type
             if not self.skip_table and block["BlockType"] == "LAYOUT_TABLE":
                 table_data = []
                 # Find the matching TABLE block for the LAYOUT_TABLE
                 table_block = None
-                for potential_table in [b for b in self.j['Blocks'] if b['BlockType'] == 'TABLE']:
+                for potential_table in [b for b in self.j['Blocks'] if b['BlockType'] == 'TABLE' and b.get('Page',1) == block.get('Page', 1)]:
                     if self._geometry_match(block['Geometry']['BoundingBox'], potential_table['Geometry']['BoundingBox']):
                         table_block = potential_table
                         break
 
                 if table_block and "Relationships" in table_block:
                     table_content = {}
                     headers = {}
@@ -234,25 +234,28 @@
             occurrences[string] += 1
         else:
             occurrences[string] = 1
         return occurrences[string]
 
     return counter
 
-
-
 def get_layout_csv_from_trp2(trp2_doc: TDocument) -> List[List[List[str]]]:
-    """customers want to generate the layout.csv from the Amazon Textract Web Console download
+    """
+    Generate the layout.csv from the Amazon Textract Web Console download
     This does generate for each page a list of the entries:
-    'Page number,'Layout,'Text,'Reading Order,'Confidence score 
-    Page number: starting at 1, incrementing for eac page
-    Layout: the BlockType + a number indicating the sequence for this BlockType starting at 1 and for LAYOUT_LIST elements the string:  "- part of LAYOUT_LIST (index)" is added
-    Text: except for LAYOUT_LIST and LAYOUT_FIGURE the underlying text
-    Reading Order: increasing int for each LAYOUT element starting with 0
-    Confidence score: confidence in this being a LAYOUT element
+
+    'Page number','Layout','Text','Reading Order','Confidence score'
+
+    Page number     : Starting at 1, incrementing for each page
+    Layout          : The BlockType + a number indicating the sequence for 
+                      this BlockType starting at 1 and for LAYOUT_LIST elements 
+                      the string:  "- part of LAYOUT_LIST (index)" is added
+    Text            : The underlying text (except LAYOUT_LIST and LAYOUT_FIGURE )
+    Reading Order   : Increasing int for each LAYOUT element starting with 0
+    Confidence score: Confidence in this being a LAYOUT element
     """
     result_value:List[List[List[str]]] = list()
 
     counter_instance = string_counter()
     for page_number, page in enumerate(trp2_doc.pages):
         page_result:List[List[str]] = list()
         processed_ids = []
@@ -298,14 +301,20 @@
 
                         page_result.append([str(page_number + 1), child_block_relation_text, layout_text, str(idx + child_idx + 1), list_child_block.block_type, str(list_child_block.confidence)])
                         # print(page_number + 1, child_block_relation_text, layout_text, idx + child_idx + 1,
                         #         list_child_block.block_type)
                         processed_ids.append(list_child_block.id)
             elif layout_block.id not in processed_ids:
                 layout_block_rel = layout_block.get_relationships_for_type()
+
+                # Bug fix - #284
+                if layout_block_rel is None:
+                    logger.info (f'Block {layout_block} has no relationships')
+                    continue
+
                 layout_blocks = [
                     trp2_doc.get_block_by_id(id) for id in layout_block_rel.ids if layout_block_rel.ids
                 ]
                 # get the text, but not for figures
                 layout_text = trp2_doc.get_text_for_tblocks(
                     layout_blocks) if layout_block.block_type != "LAYOUT_FIGURE" else ""
                 block_type_count = counter_instance(layout_block.block_type)
```

