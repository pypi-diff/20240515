# Comparing `tmp/dtogen-0.0.7.tar.gz` & `tmp/dtogen-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtogen-0.0.7.tar", last modified: Sun Jul 23 06:10:24 2023, max compression
+gzip compressed data, was "dtogen-0.0.8.tar", last modified: Wed May 15 19:38:59 2024, max compression
```

## Comparing `dtogen-0.0.7.tar` & `dtogen-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-23 06:10:24.351123 dtogen-0.0.7/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3099 2023-07-23 06:10:24.350935 dtogen-0.0.7/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2777 2023-07-20 21:30:14.000000 dtogen-0.0.7/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-23 06:10:24.347393 dtogen-0.0.7/dtogen/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      934 2023-07-22 22:13:03.000000 dtogen-0.0.7/dtogen/__main__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1620 2023-07-22 22:11:21.000000 dtogen-0.0.7/dtogen/dtogenerator.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-23 06:10:24.349333 dtogen-0.0.7/dtogen/filewriters/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      183 2023-07-22 22:10:45.000000 dtogen-0.0.7/dtogen/filewriters/__init__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2024 2023-07-22 22:12:24.000000 dtogen-0.0.7/dtogen/filewriters/filewriter.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-22 22:11:52.000000 dtogen-0.0.7/dtogen/filewriters/filewriter_java.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      588 2023-07-22 22:12:03.000000 dtogen-0.0.7/dtogen/filewriters/filewriter_python.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      558 2023-07-22 22:12:15.000000 dtogen-0.0.7/dtogen/filewriters/filewriter_typescript.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-20 21:12:11.000000 dtogen-0.0.7/dtogen/interfaces.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-23 06:10:24.350338 dtogen-0.0.7/dtogen/transformers/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      191 2023-07-22 22:10:22.000000 dtogen-0.0.7/dtogen/transformers/__init__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     4518 2023-07-22 22:12:57.000000 dtogen-0.0.7/dtogen/transformers/transformer.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      913 2023-07-22 22:11:38.000000 dtogen-0.0.7/dtogen/transformers/transformer_java.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      805 2023-07-22 22:12:41.000000 dtogen-0.0.7/dtogen/transformers/transformer_python.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      836 2023-07-22 22:12:49.000000 dtogen-0.0.7/dtogen/transformers/transformer_typescript.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-23 06:10:24.348388 dtogen-0.0.7/dtogen.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3099 2023-07-23 06:10:24.000000 dtogen-0.0.7/dtogen.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      660 2023-07-23 06:10:24.000000 dtogen-0.0.7/dtogen.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-23 06:10:24.000000 dtogen-0.0.7/dtogen.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       15 2023-07-23 06:10:24.000000 dtogen-0.0.7/dtogen.egg-info/requires.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        7 2023-07-23 06:10:24.000000 dtogen-0.0.7/dtogen.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-23 06:10:24.351174 dtogen-0.0.7/setup.cfg
--rw-r--r--   0 mujdecisy   (501) staff       (20)      734 2023-07-23 06:10:05.000000 dtogen-0.0.7/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-23 06:10:24.350666 dtogen-0.0.7/test/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1195 2023-07-22 06:17:14.000000 dtogen-0.0.7/test/test_dtogenerator.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1285 2023-07-22 06:17:14.000000 dtogen-0.0.7/test/test_transform.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.631774 dtogen-0.0.8/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3151 2024-05-15 19:38:59.631315 dtogen-0.0.8/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2777 2023-07-20 21:30:14.000000 dtogen-0.0.8/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.625664 dtogen-0.0.8/dtogen/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1148 2024-05-15 19:30:55.000000 dtogen-0.0.8/dtogen/__main__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1620 2023-07-22 22:11:21.000000 dtogen-0.0.8/dtogen/dtogenerator.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.628142 dtogen-0.0.8/dtogen/filewriters/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      183 2023-07-22 22:10:45.000000 dtogen-0.0.8/dtogen/filewriters/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2024 2023-07-22 22:12:24.000000 dtogen-0.0.8/dtogen/filewriters/filewriter.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-22 22:11:52.000000 dtogen-0.0.8/dtogen/filewriters/filewriter_java.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      588 2023-07-22 22:12:03.000000 dtogen-0.0.8/dtogen/filewriters/filewriter_python.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      558 2023-07-22 22:12:15.000000 dtogen-0.0.8/dtogen/filewriters/filewriter_typescript.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-20 21:12:11.000000 dtogen-0.0.8/dtogen/interfaces.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.629958 dtogen-0.0.8/dtogen/transformers/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      191 2023-07-22 22:10:22.000000 dtogen-0.0.8/dtogen/transformers/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     4518 2023-07-22 22:12:57.000000 dtogen-0.0.8/dtogen/transformers/transformer.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      913 2023-07-22 22:11:38.000000 dtogen-0.0.8/dtogen/transformers/transformer_java.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      805 2023-07-22 22:12:41.000000 dtogen-0.0.8/dtogen/transformers/transformer_python.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      836 2023-07-22 22:12:49.000000 dtogen-0.0.8/dtogen/transformers/transformer_typescript.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.631011 dtogen-0.0.8/dtogen.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3151 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      660 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       22 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/requires.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        7 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2024-05-15 19:38:59.631922 dtogen-0.0.8/setup.cfg
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      741 2024-05-15 19:31:25.000000 dtogen-0.0.8/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.630601 dtogen-0.0.8/test/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1195 2023-07-22 06:17:14.000000 dtogen-0.0.8/test/test_dtogenerator.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1285 2023-07-22 06:17:14.000000 dtogen-0.0.8/test/test_transform.py
```

### Comparing `dtogen-0.0.7/PKG-INFO` & `dtogen-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: dtogen
-Version: 0.0.7
-Summary: DTO generator for Java, TypeScript, Python
-Home-page: https://github.com/mujdecisy/dtogen
-Author: mujdecisy
-Author-email: mujdecisy@gmail.com
-Keywords: python,DTO,generator
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-
 # DTOgen - Data Transfer Object Generator
 
 DTOgen is a powerful library that allows users to **effortlessly generate Data Transfer Object (DTO) classes** in multiple programming languages from YAML definitions. DTOgen aims to **simplify the process of mapping** JSON or XML data to objects, making it an excellent tool for microservices development.
 
 With DTOgen, syncing Data Transfer Objects (DTOs) across services becomes a seamless process. Since DTOgen allows you to define DTOs in a centralized YAML file and **generates the corresponding classes in multiple programming languages**, you can ensure consistency across your microservices easily. 
 
 DTOgen is designed to handle not only simple data types but also **complex data structures** like lists and maps. With the ability to represent lists and maps in the YAML definitions, DTOgen can generate DTO classes that accurately reflect these data structures in multiple programming languages.
@@ -86,8 +75,8 @@
 ```typescript
 export class Person {
     name: string | undefined;
     age: number | undefined;
 }
 ```
 
-DTOgen simplifies the process of creating Data Transfer Objects, enabling developers to focus more on building efficient microservices without worrying about complex data mapping.
+DTOgen simplifies the process of creating Data Transfer Objects, enabling developers to focus more on building efficient microservices without worrying about complex data mapping.
```

### Comparing `dtogen-0.0.7/README.md` & `dtogen-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: dtogen
+Version: 0.0.8
+Summary: DTO generator for Java, TypeScript, Python
+Home-page: https://github.com/mujdecisy/dtogen
+Author: mujdecisy
+Author-email: mujdecisy@gmail.com
+Keywords: python,DTO,generator
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+Requires-Dist: mapperr==0.2.4
+Requires-Dist: pyyaml
+
 # DTOgen - Data Transfer Object Generator
 
 DTOgen is a powerful library that allows users to **effortlessly generate Data Transfer Object (DTO) classes** in multiple programming languages from YAML definitions. DTOgen aims to **simplify the process of mapping** JSON or XML data to objects, making it an excellent tool for microservices development.
 
 With DTOgen, syncing Data Transfer Objects (DTOs) across services becomes a seamless process. Since DTOgen allows you to define DTOs in a centralized YAML file and **generates the corresponding classes in multiple programming languages**, you can ensure consistency across your microservices easily. 
 
 DTOgen is designed to handle not only simple data types but also **complex data structures** like lists and maps. With the ability to represent lists and maps in the YAML definitions, DTOgen can generate DTO classes that accurately reflect these data structures in multiple programming languages.
@@ -75,8 +88,8 @@
 ```typescript
 export class Person {
     name: string | undefined;
     age: number | undefined;
 }
 ```
 
-DTOgen simplifies the process of creating Data Transfer Objects, enabling developers to focus more on building efficient microservices without worrying about complex data mapping.
+DTOgen simplifies the process of creating Data Transfer Objects, enabling developers to focus more on building efficient microservices without worrying about complex data mapping.
```

### Comparing `dtogen-0.0.7/dtogen/dtogenerator.py` & `dtogen-0.0.8/dtogen/dtogenerator.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/filewriters/filewriter.py` & `dtogen-0.0.8/dtogen/filewriters/filewriter.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/filewriters/filewriter_java.py` & `dtogen-0.0.8/dtogen/filewriters/filewriter_java.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/filewriters/filewriter_python.py` & `dtogen-0.0.8/dtogen/filewriters/filewriter_python.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/filewriters/filewriter_typescript.py` & `dtogen-0.0.8/dtogen/filewriters/filewriter_typescript.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/interfaces.py` & `dtogen-0.0.8/dtogen/interfaces.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/transformers/transformer.py` & `dtogen-0.0.8/dtogen/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/transformers/transformer_java.py` & `dtogen-0.0.8/dtogen/transformers/transformer_java.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/transformers/transformer_python.py` & `dtogen-0.0.8/dtogen/transformers/transformer_python.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen/transformers/transformer_typescript.py` & `dtogen-0.0.8/dtogen/transformers/transformer_typescript.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/dtogen.egg-info/PKG-INFO` & `dtogen-0.0.8/dtogen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: dtogen
-Version: 0.0.7
+Version: 0.0.8
 Summary: DTO generator for Java, TypeScript, Python
 Home-page: https://github.com/mujdecisy/dtogen
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,DTO,generator
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Requires-Dist: mapperr==0.2.4
+Requires-Dist: pyyaml
 
 # DTOgen - Data Transfer Object Generator
 
 DTOgen is a powerful library that allows users to **effortlessly generate Data Transfer Object (DTO) classes** in multiple programming languages from YAML definitions. DTOgen aims to **simplify the process of mapping** JSON or XML data to objects, making it an excellent tool for microservices development.
 
 With DTOgen, syncing Data Transfer Objects (DTOs) across services becomes a seamless process. Since DTOgen allows you to define DTOs in a centralized YAML file and **generates the corresponding classes in multiple programming languages**, you can ensure consistency across your microservices easily.
```

### Comparing `dtogen-0.0.7/dtogen.egg-info/SOURCES.txt` & `dtogen-0.0.8/dtogen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/setup.py` & `dtogen-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="dtogen",
-    version="0.0.7",
+    version="0.0.8",
     description="DTO generator for Java, TypeScript, Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/dtogen",
     keywords=["python", "DTO", "generator"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     packages=['dtogen','dtogen.transformers','dtogen.filewriters'],
     include_package_data=True,
-    install_requires=["mapperr", "pyyaml"],
+    install_requires=["mapperr==0.2.4", "pyyaml"],
 )
```

### Comparing `dtogen-0.0.7/test/test_dtogenerator.py` & `dtogen-0.0.8/test/test_dtogenerator.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.7/test/test_transform.py` & `dtogen-0.0.8/test/test_transform.py`

 * *Files identical despite different names*

