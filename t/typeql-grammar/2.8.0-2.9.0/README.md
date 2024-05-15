# Comparing `tmp/typeql-grammar-2.8.0.tar.gz` & `tmp/typeql-grammar-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeql-grammar-2.8.0.tar", last modified: Tue Mar 22 12:04:11 2022, max compression
+gzip compressed data, was "typeql-grammar-2.9.0.tar", last modified: Fri May 20 13:29:45 2022, max compression
```

## Comparing `typeql-grammar-2.8.0.tar` & `typeql-grammar-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:11.178806 typeql-grammar-2.8.0/
--rw-r--r--   0 grabl     (1000) grabl     (1000)    13540 2022-03-22 12:04:11.178806 typeql-grammar-2.8.0/PKG-INFO
--rw-rw-r--   0 grabl     (1000) grabl     (1000)    10643 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/README.md
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:11.174806 typeql-grammar-2.8.0/bazel-out/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/bazel-out/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:11.174806 typeql-grammar-2.8.0/bazel-out/k8-fastbuild/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/bazel-out/k8-fastbuild/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:11.174806 typeql-grammar-2.8.0/bazel-out/k8-fastbuild/bin/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/bazel-out/k8-fastbuild/bin/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:11.174806 typeql-grammar-2.8.0/bazel-out/k8-fastbuild/bin/grammar/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/bazel-out/k8-fastbuild/bin/grammar/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:11.174806 typeql-grammar-2.8.0/bazel-out/k8-fastbuild/bin/grammar/python/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/bazel-out/k8-fastbuild/bin/grammar/python/__init__.py
--rw-r--r--   0 grabl     (1000) grabl     (1000)       67 2022-03-22 12:04:11.178806 typeql-grammar-2.8.0/setup.cfg
--rw-r--r--   0 grabl     (1000) grabl     (1000)     1933 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/setup.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:04:11.178806 typeql-grammar-2.8.0/typeql_grammar.egg-info/
--rw-r--r--   0 grabl     (1000) grabl     (1000)    13540 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/typeql_grammar.egg-info/PKG-INFO
--rw-r--r--   0 grabl     (1000) grabl     (1000)      507 2022-03-22 12:04:11.000000 typeql-grammar-2.8.0/typeql_grammar.egg-info/SOURCES.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/typeql_grammar.egg-info/dependency_links.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/typeql_grammar.egg-info/not-zip-safe
--rw-r--r--   0 grabl     (1000) grabl     (1000)       30 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/typeql_grammar.egg-info/requires.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)       10 2022-03-22 12:04:10.000000 typeql-grammar-2.8.0/typeql_grammar.egg-info/top_level.txt
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)    11601 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/PKG-INFO
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)    10643 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/README.md
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/bazel-out/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/bazel-out/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/bazel-out/k8-fastbuild/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/bazel-out/k8-fastbuild/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/bazel-out/k8-fastbuild/bin/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/bazel-out/k8-fastbuild/bin/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/bazel-out/k8-fastbuild/bin/grammar/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/bazel-out/k8-fastbuild/bin/grammar/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/bazel-out/k8-fastbuild/bin/grammar/python/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/bazel-out/k8-fastbuild/bin/grammar/python/__init__.py
+-rw-r--r--   0 grabl     (1000) grabl     (1000)       67 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/setup.cfg
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     1933 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/setup.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 13:29:45.291410 typeql-grammar-2.9.0/typeql_grammar.egg-info/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)    11601 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/typeql_grammar.egg-info/PKG-INFO
+-rw-r--r--   0 grabl     (1000) grabl     (1000)      507 2022-05-20 13:29:45.000000 typeql-grammar-2.9.0/typeql_grammar.egg-info/SOURCES.txt
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/typeql_grammar.egg-info/dependency_links.txt
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-05-20 13:29:44.000000 typeql-grammar-2.9.0/typeql_grammar.egg-info/not-zip-safe
+-rw-r--r--   0 grabl     (1000) grabl     (1000)       30 2022-05-20 13:29:45.000000 typeql-grammar-2.9.0/typeql_grammar.egg-info/requires.txt
+-rw-r--r--   0 grabl     (1000) grabl     (1000)       10 2022-05-20 13:29:45.000000 typeql-grammar-2.9.0/typeql_grammar.egg-info/top_level.txt
```

### Comparing `typeql-grammar-2.8.0/PKG-INFO` & `typeql-grammar-2.9.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,257 +1,15 @@
 Metadata-Version: 2.1
 Name: typeql-grammar
-Version: 2.8.0
+Version: 2.9.0
 Summary: TypeQL Grammar for Python
 Home-page: https://github.com/vaticle/typeql
 Author: Vaticle
 Author-email: community@vaticle.com
 License: AGPLv3
-Description: [![Grabl](https://grabl.io/api/status/vaticle/typeql/badge.svg)](https://grabl.io/vaticle/typeql)
-        [![GitHub release](https://img.shields.io/github/release/vaticle/typeql.svg)](https://github.com/vaticle/typeql/releases/latest)
-        [![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://vaticle.com/discord)
-        [![Discussion Forum](https://img.shields.io/discourse/https/forum.vaticle.com/topics.svg)](https://forum.vaticle.com)
-        [![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
-        [![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
-        
-        # Meet TypeQL (and [TypeDB](https://github.com/vaticle/typedb))
-        
-        TypeDB is a strongly-typed database with a rich and logical type system. TypeDB empowers you to tackle complex problems, and TypeQL is its query language.
-        
-        ## A higher level of expressivity
-        
-        TypeQL allows you to model your domain based on logical and object-oriented principles. Composed of entity, relationship, and attribute types, as well as type hierarchies, roles, and rules, TypeQL allows you to think higher-level as opposed to join-tables, columns, documents, vertices, edges, and properties.
-        
-        ### Entity-Relationship Model
-        
-        TypeQL allows you to model your domain using the well-known Entity-Relationship model. It is composed of entity types, relation types, and attribute types, with the introduction of role types. TypeQL allows you to leverage the full expressivity of the ER model, and describe your schema through first normal form.
-        
-        ```typeql
-        define
-        
-        person sub entity,
-          owns name,
-          plays employment:employee;
-        company sub entity,
-          owns name,
-          plays employment:employer;
-        employment sub relation,
-          relates employee,
-          relates employer;
-        name sub attribute,
-          value string;
-        ```
-        
-        ### Type Hierarchies
-        
-        TypeQL allows you to easily model type inheritance into your domain model. Following logical and object-oriented principle, TypeQL allows data types to inherit the behaviours and properties of their supertypes. Complex data structures become reusable, and data interpretation becomes richer through polymorphism.
-        
-        ```typeql
-        define
-        
-        person sub entity,
-          owns first-name,
-          owns last-name;
-        
-        student sub person;
-        undergrad sub student;
-        postgrad sub student;
-        
-        teacher sub person;
-        supervisor sub teacher;
-        professor sub teacher;
-        ```
-        
-        
-        ### N-ary Relations
-        
-        In the real world, relations aren't just binary connections between two things. In rich systems, we often need to capture three or more things related with each other at once. Representing them as separate binary relationships would lose information. TypeQL can naturally represent arbitrary number of things as one relation.
-        
-        ```typeql
-        match
-         
-        $person isa person, has name "Leonardo";
-        $character isa character, has name "Jack";
-        $movie isa movie;
-        (actor: $person, character: $character, movie: $movie) isa cast;
-        get $movie;
-         
-        answers>>
-         
-        $movie isa movie, has name "Titanic";
-        ```
-        
-        
-        ### Nested Relations
-        
-        Relations are concepts we use to describe the association between two or more things. Sometimes, those things can be relations themselves. TypeQL can represent these structures naturally, as it enables relations to be nested in another relation, allowing you to express the model of your system in the most natural form.
-        
-        ```typeql
-        match
-         
-        $alice isa person, has name "Alice";
-        $bob isa person, has name "Bob";
-        $mar ($alice, $bob) isa marriage;
-        $city isa city;
-        ($mar, $city) isa located;
-         
-        answers>>
-         
-        $city isa city, has name "London";
-        ```
-        
-        
-        ## A higher degree of safety
-        
-        Types provide a way to describe the logical structures of your data, allowing TypeDB to validate that your code inserts and queries data correctly. Query validation goes beyond static type checking, and includes logical validations of meaningless queries. With strict type-checking errors, you have a dataset that you can trust.
-        
-        ### Logical Data Validation
-        
-        Inserted data gets validated beyond static type checking of attribute value types. Entities are validated to only have the correct attributes, and relations are validated to only relate things that are logically allowed. TypeDB performs richer validation of inserted entities and relations by evaluating the polymorphic types of the things involved.
-        
-        ```typeql
-        insert
-        
-        $charlie isa person, has name "Charlie";
-        $dataCo isa company, has name "DataCo";
-        (husband: $charlie, wife: $dataCo) isa marriage; # invalid relation
-        
-        commit>>
-        
-        ERROR: invalid data detected during type validation
-        ```
-        
-        
-        ### Logical Query Validation
-        
-        Read queries executed on TypeDB go through a type resolution process. This process not only optimises the query's execution, but also acts as a static type checker to reject meaningless and unsatisfiable queries, as they are likely a user error.
-        
-        ```typeql
-        match
-        
-        $alice isa person, has name "Alice";
-        $bob isa person, has name "Bob";
-        ($alice, $bob) isa marriage;
-        $dataCo isa company, has name "DataCo";
-        ($bob, $dataCo) isa marriage; # invalid relation
-        
-        answers>>
-        
-        ERROR: unsatisfiable query detected during type resolution
-        ```
-        
-        ## Evolved with logical inference
-        
-        TypeDB encodes your data for logical interpretation by a reasoning engine. It enables type-inference and rule-inference that creates logical abstractions of data. This allows the discovery of facts and patterns that would otherwise be too hard to find; and complex queries become much simpler.
-        
-        ### Rules
-        
-        TypeQL allows you to define rules in your schema. This extends the expressivity of your model as it enables the system to derive new conclusions when a certain logical form in your dataset is satisfied. Like functions in programming, rules can chain onto one another, creating abstractions of behaviour at the data level.
-        
-        ```typeql
-        define
-        
-        rule transitive-location:
-        when {
-          (located: $x, locating: $y);
-          (located: $y, locating: $z);
-        } then {
-          (located: $x, locating: $z);
-        };
-        ```
-        
-        ### Inference
-        
-        TypeDB's inference facility translates one query into all of its possible interpretations. This happens through two mechanisms: type-based and rule-based inference. Not only does this derive new conclusions and uncovers relationships that would otherwise be hidden, but it also enables the abstraction of complex patterns into simple queries.
-        
-        ```typeql
-        match
-        
-        $person isa person;
-        $uk isa country, has name "UK";
-        ($person, $uk) isa location;
-        get $person;
-        
-        answers>>
-        
-        $person isa teacher, has name "Alice";
-        $person isa postgrad, has name "Bob";
-        ```
-        
-        ## Using TypeQL
-        
-        ### TypeQL (native syntax)
-        
-        All TypeDB Clients, as well as TypeDB Console, accept TypeQL syntax natively. If you are using TypeDB, you do not need additional libraries/tools to use TypeQL syntax natively. 
-        
-        ### TypeQL for Java
-        
-        #### Language Library
-        
-        To use a TypeQL language library for Java, to be able to construct queries programmatically as opposed to manual string concatenations, please visit [vaticle/typeql-lang-java](https://github.com/vaticle/typeql-lang-java)
-        
-        #### Grammar
-        
-        If you would like to develop language TypeQL plugins or extension in Java, and require the TypeQL grammar library, you can import the following Maven package.
-        
-        ```xml
-        <repositories>
-            <repository>
-                <id>repo.vaticle.com</id>
-                <url>https://repo.vaticle.com/repository/maven/</url>
-            </repository>
-        </repositories>
-        
-        <dependencies>
-            <dependency>
-                <groupId>com.vaticle.typeql</groupId>
-                <artifactId>typeql-grammar</artifactId>
-                <version>{version}</version>
-            </dependency>
-        </dependencies>
-        ```
-        
-        Replace `{version}` with the version number, in which you can find the latest of TypeQL Grammar on our [Maven Repository](https://repo.vaticle.com/#browse/browse:maven:com%2Fvaticle%2Ftypeql%2Ftypeql-grammar).
-        
-        ## TypeQL for Python
-        
-        #### Language Library
-        
-        To use a TypeQL language library for Python, to be able to construct queries programmatically as opposed to manual string concatenations, please visit [typedb-osi/typeql-lang-python](https://github.com/typedb-osi/typeql-lang-python). The project is still under development by the community. You are welcome to contribute to the project development.
-        
-        #### Grammar
-        
-        If you would like to develop language TypeQL plugins or extension in Python, and require the TypeQL grammar library, you can import the following PyPI package.
-        
-        ```
-        pip install typeql-grammar=={version}
-        ```
-        
-        Replace `{version}` with the version number, in which you can find the latest on [TypeQL's PyPi Page](https://pypi.org/project/typeql-grammar/). 
-        
-        ## Contributions
-        
-        TypeDB & TypeQL has been built using various open-source Graph and Distributed Computing frameworks throughout its evolution. Today TypeDB & TypeQL is built using [RocksDB](https://rocksdb.org), [ANTLR](http://www.antlr.org), [SCIP](https://www.scipopt.org), [Bazel](https://bazel.build), [GRPC](https://grpc.io), and [ZeroMQ](https://zeromq.org), and [Caffeine](https://github.com/ben-manes/caffeine). In the past, TypeDB was enabled by various open-source technologies and communities that we are hugely thankful to: [Apache Cassandra](http://cassandra.apache.org), [Apache Hadoop](https://hadoop.apache.org), [Apache Spark](http://spark.apache.org), [Apache TinkerPop](http://tinkerpop.apache.org), and [JanusGraph](http://janusgraph.org). Thank you!
-        
-        ---
-        
-        ## Licensing
-        
-        The TypeQL language and related materials are distributed under the terms GNU Affero General Public License v3.0 ("AGPL 3.0") as published by the Free Software Foundation, but with the following special exception.
-        
-        Exception to AGPL 3.0: Any TypeQL language library that is based on material or materials in the Vaticle TypeQL repository, and that is used to communicate or interact (in each case) with a database created or managed or accessed (in each case) using a version of the TypeQL software that is made available by or on behalf of Vaticle Limited (UK Company Number 08766237) or any successor entity (but excluding any forked version of that software), may be distributed under one of the following licences:
-        
-        - The Apache License version 2: https://www.apache.org/licenses/LICENSE-2.0.txt
-        - The MIT License: https://opensource.org/licenses/MIT
-        - The BSD License (2-Clause): https://opensource.org/licenses/BSD-2-Clause
-        
-        As used above "successor entity" means any entity then owning copyrights in the TypeDB software that were previously owned by Vaticle Ltd.
-        
-        If you make any change to, or contribute to, (in each case) the TypeQL code or related materials, then this exception will apply to any TypeQL language library that uses or implements that change/contribution.
-        
 Keywords: grakn database graph knowledgebase knowledge-engineering
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -260,7 +18,251 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
+
+[![Grabl](https://grabl.io/api/status/vaticle/typeql/badge.svg)](https://grabl.io/vaticle/typeql)
+[![GitHub release](https://img.shields.io/github/release/vaticle/typeql.svg)](https://github.com/vaticle/typeql/releases/latest)
+[![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://vaticle.com/discord)
+[![Discussion Forum](https://img.shields.io/discourse/https/forum.vaticle.com/topics.svg)](https://forum.vaticle.com)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
+
+# Meet TypeQL (and [TypeDB](https://github.com/vaticle/typedb))
+
+TypeDB is a strongly-typed database with a rich and logical type system. TypeDB empowers you to tackle complex problems, and TypeQL is its query language.
+
+## A higher level of expressivity
+
+TypeQL allows you to model your domain based on logical and object-oriented principles. Composed of entity, relationship, and attribute types, as well as type hierarchies, roles, and rules, TypeQL allows you to think higher-level as opposed to join-tables, columns, documents, vertices, edges, and properties.
+
+### Entity-Relationship Model
+
+TypeQL allows you to model your domain using the well-known Entity-Relationship model. It is composed of entity types, relation types, and attribute types, with the introduction of role types. TypeQL allows you to leverage the full expressivity of the ER model, and describe your schema through first normal form.
+
+```typeql
+define
+
+person sub entity,
+  owns name,
+  plays employment:employee;
+company sub entity,
+  owns name,
+  plays employment:employer;
+employment sub relation,
+  relates employee,
+  relates employer;
+name sub attribute,
+  value string;
+```
+
+### Type Hierarchies
+
+TypeQL allows you to easily model type inheritance into your domain model. Following logical and object-oriented principle, TypeQL allows data types to inherit the behaviours and properties of their supertypes. Complex data structures become reusable, and data interpretation becomes richer through polymorphism.
+
+```typeql
+define
+
+person sub entity,
+  owns first-name,
+  owns last-name;
+
+student sub person;
+undergrad sub student;
+postgrad sub student;
+
+teacher sub person;
+supervisor sub teacher;
+professor sub teacher;
+```
+
+
+### N-ary Relations
+
+In the real world, relations aren't just binary connections between two things. In rich systems, we often need to capture three or more things related with each other at once. Representing them as separate binary relationships would lose information. TypeQL can naturally represent arbitrary number of things as one relation.
+
+```typeql
+match
+ 
+$person isa person, has name "Leonardo";
+$character isa character, has name "Jack";
+$movie isa movie;
+(actor: $person, character: $character, movie: $movie) isa cast;
+get $movie;
+ 
+answers>>
+ 
+$movie isa movie, has name "Titanic";
+```
+
+
+### Nested Relations
+
+Relations are concepts we use to describe the association between two or more things. Sometimes, those things can be relations themselves. TypeQL can represent these structures naturally, as it enables relations to be nested in another relation, allowing you to express the model of your system in the most natural form.
+
+```typeql
+match
+ 
+$alice isa person, has name "Alice";
+$bob isa person, has name "Bob";
+$mar ($alice, $bob) isa marriage;
+$city isa city;
+($mar, $city) isa located;
+ 
+answers>>
+ 
+$city isa city, has name "London";
+```
+
+
+## A higher degree of safety
+
+Types provide a way to describe the logical structures of your data, allowing TypeDB to validate that your code inserts and queries data correctly. Query validation goes beyond static type checking, and includes logical validations of meaningless queries. With strict type-checking errors, you have a dataset that you can trust.
+
+### Logical Data Validation
+
+Inserted data gets validated beyond static type checking of attribute value types. Entities are validated to only have the correct attributes, and relations are validated to only relate things that are logically allowed. TypeDB performs richer validation of inserted entities and relations by evaluating the polymorphic types of the things involved.
+
+```typeql
+insert
+
+$charlie isa person, has name "Charlie";
+$dataCo isa company, has name "DataCo";
+(husband: $charlie, wife: $dataCo) isa marriage; # invalid relation
+
+commit>>
+
+ERROR: invalid data detected during type validation
+```
+
+
+### Logical Query Validation
+
+Read queries executed on TypeDB go through a type resolution process. This process not only optimises the query's execution, but also acts as a static type checker to reject meaningless and unsatisfiable queries, as they are likely a user error.
+
+```typeql
+match
+
+$alice isa person, has name "Alice";
+$bob isa person, has name "Bob";
+($alice, $bob) isa marriage;
+$dataCo isa company, has name "DataCo";
+($bob, $dataCo) isa marriage; # invalid relation
+
+answers>>
+
+ERROR: unsatisfiable query detected during type resolution
+```
+
+## Evolved with logical inference
+
+TypeDB encodes your data for logical interpretation by a reasoning engine. It enables type-inference and rule-inference that creates logical abstractions of data. This allows the discovery of facts and patterns that would otherwise be too hard to find; and complex queries become much simpler.
+
+### Rules
+
+TypeQL allows you to define rules in your schema. This extends the expressivity of your model as it enables the system to derive new conclusions when a certain logical form in your dataset is satisfied. Like functions in programming, rules can chain onto one another, creating abstractions of behaviour at the data level.
+
+```typeql
+define
+
+rule transitive-location:
+when {
+  (located: $x, locating: $y);
+  (located: $y, locating: $z);
+} then {
+  (located: $x, locating: $z);
+};
+```
+
+### Inference
+
+TypeDB's inference facility translates one query into all of its possible interpretations. This happens through two mechanisms: type-based and rule-based inference. Not only does this derive new conclusions and uncovers relationships that would otherwise be hidden, but it also enables the abstraction of complex patterns into simple queries.
+
+```typeql
+match
+
+$person isa person;
+$uk isa country, has name "UK";
+($person, $uk) isa location;
+get $person;
+
+answers>>
+
+$person isa teacher, has name "Alice";
+$person isa postgrad, has name "Bob";
+```
+
+## Using TypeQL
+
+### TypeQL (native syntax)
+
+All TypeDB Clients, as well as TypeDB Console, accept TypeQL syntax natively. If you are using TypeDB, you do not need additional libraries/tools to use TypeQL syntax natively. 
+
+### TypeQL for Java
+
+#### Language Library
+
+To use a TypeQL language library for Java, to be able to construct queries programmatically as opposed to manual string concatenations, please visit [vaticle/typeql-lang-java](https://github.com/vaticle/typeql-lang-java)
+
+#### Grammar
+
+If you would like to develop language TypeQL plugins or extension in Java, and require the TypeQL grammar library, you can import the following Maven package.
+
+```xml
+<repositories>
+    <repository>
+        <id>repo.vaticle.com</id>
+        <url>https://repo.vaticle.com/repository/maven/</url>
+    </repository>
+</repositories>
+
+<dependencies>
+    <dependency>
+        <groupId>com.vaticle.typeql</groupId>
+        <artifactId>typeql-grammar</artifactId>
+        <version>{version}</version>
+    </dependency>
+</dependencies>
+```
+
+Replace `{version}` with the version number, in which you can find the latest of TypeQL Grammar on our [Maven Repository](https://repo.vaticle.com/#browse/browse:maven:com%2Fvaticle%2Ftypeql%2Ftypeql-grammar).
+
+## TypeQL for Python
+
+#### Language Library
+
+To use a TypeQL language library for Python, to be able to construct queries programmatically as opposed to manual string concatenations, please visit [typedb-osi/typeql-lang-python](https://github.com/typedb-osi/typeql-lang-python). The project is still under development by the community. You are welcome to contribute to the project development.
+
+#### Grammar
+
+If you would like to develop language TypeQL plugins or extension in Python, and require the TypeQL grammar library, you can import the following PyPI package.
+
+```
+pip install typeql-grammar=={version}
+```
+
+Replace `{version}` with the version number, in which you can find the latest on [TypeQL's PyPi Page](https://pypi.org/project/typeql-grammar/). 
+
+## Contributions
+
+TypeDB & TypeQL has been built using various open-source Graph and Distributed Computing frameworks throughout its evolution. Today TypeDB & TypeQL is built using [RocksDB](https://rocksdb.org), [ANTLR](http://www.antlr.org), [SCIP](https://www.scipopt.org), [Bazel](https://bazel.build), [GRPC](https://grpc.io), and [ZeroMQ](https://zeromq.org), and [Caffeine](https://github.com/ben-manes/caffeine). In the past, TypeDB was enabled by various open-source technologies and communities that we are hugely thankful to: [Apache Cassandra](http://cassandra.apache.org), [Apache Hadoop](https://hadoop.apache.org), [Apache Spark](http://spark.apache.org), [Apache TinkerPop](http://tinkerpop.apache.org), and [JanusGraph](http://janusgraph.org). Thank you!
+
+---
+
+## Licensing
+
+The TypeQL language and related materials are distributed under the terms GNU Affero General Public License v3.0 ("AGPL 3.0") as published by the Free Software Foundation, but with the following special exception.
+
+Exception to AGPL 3.0: Any TypeQL language library that is based on material or materials in the Vaticle TypeQL repository, and that is used to communicate or interact (in each case) with a database created or managed or accessed (in each case) using a version of the TypeQL software that is made available by or on behalf of Vaticle Limited (UK Company Number 08766237) or any successor entity (but excluding any forked version of that software), may be distributed under one of the following licences:
+
+- The Apache License version 2: https://www.apache.org/licenses/LICENSE-2.0.txt
+- The MIT License: https://opensource.org/licenses/MIT
+- The BSD License (2-Clause): https://opensource.org/licenses/BSD-2-Clause
+
+As used above "successor entity" means any entity then owning copyrights in the TypeDB software that were previously owned by Vaticle Ltd.
+
+If you make any change to, or contribute to, (in each case) the TypeQL code or related materials, then this exception will apply to any TypeQL language library that uses or implements that change/contribution.
+
+
```

### Comparing `typeql-grammar-2.8.0/README.md` & `typeql-grammar-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `typeql-grammar-2.8.0/setup.py` & `typeql-grammar-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from setuptools import setup
 from setuptools import find_packages
 
 packages = find_packages()
 
 setup(
     name = "typeql-grammar",
-    version = "2.8.0",
+    version = "2.9.0",
     description = "TypeQL Grammar for Python",
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     classifiers = ["Programming Language :: Python", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.5", "Programming Language :: Python :: 3.6", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Intended Audience :: Science/Research", "Environment :: Console", "Topic :: Database :: Front-Ends"],
     keywords = "grakn database graph knowledgebase knowledge-engineering",
     url = "https://github.com/vaticle/typeql",
     author = "Vaticle",
```

### Comparing `typeql-grammar-2.8.0/typeql_grammar.egg-info/PKG-INFO` & `typeql-grammar-2.9.0/typeql_grammar.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,257 +1,15 @@
 Metadata-Version: 2.1
 Name: typeql-grammar
-Version: 2.8.0
+Version: 2.9.0
 Summary: TypeQL Grammar for Python
 Home-page: https://github.com/vaticle/typeql
 Author: Vaticle
 Author-email: community@vaticle.com
 License: AGPLv3
-Description: [![Grabl](https://grabl.io/api/status/vaticle/typeql/badge.svg)](https://grabl.io/vaticle/typeql)
-        [![GitHub release](https://img.shields.io/github/release/vaticle/typeql.svg)](https://github.com/vaticle/typeql/releases/latest)
-        [![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://vaticle.com/discord)
-        [![Discussion Forum](https://img.shields.io/discourse/https/forum.vaticle.com/topics.svg)](https://forum.vaticle.com)
-        [![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
-        [![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
-        
-        # Meet TypeQL (and [TypeDB](https://github.com/vaticle/typedb))
-        
-        TypeDB is a strongly-typed database with a rich and logical type system. TypeDB empowers you to tackle complex problems, and TypeQL is its query language.
-        
-        ## A higher level of expressivity
-        
-        TypeQL allows you to model your domain based on logical and object-oriented principles. Composed of entity, relationship, and attribute types, as well as type hierarchies, roles, and rules, TypeQL allows you to think higher-level as opposed to join-tables, columns, documents, vertices, edges, and properties.
-        
-        ### Entity-Relationship Model
-        
-        TypeQL allows you to model your domain using the well-known Entity-Relationship model. It is composed of entity types, relation types, and attribute types, with the introduction of role types. TypeQL allows you to leverage the full expressivity of the ER model, and describe your schema through first normal form.
-        
-        ```typeql
-        define
-        
-        person sub entity,
-          owns name,
-          plays employment:employee;
-        company sub entity,
-          owns name,
-          plays employment:employer;
-        employment sub relation,
-          relates employee,
-          relates employer;
-        name sub attribute,
-          value string;
-        ```
-        
-        ### Type Hierarchies
-        
-        TypeQL allows you to easily model type inheritance into your domain model. Following logical and object-oriented principle, TypeQL allows data types to inherit the behaviours and properties of their supertypes. Complex data structures become reusable, and data interpretation becomes richer through polymorphism.
-        
-        ```typeql
-        define
-        
-        person sub entity,
-          owns first-name,
-          owns last-name;
-        
-        student sub person;
-        undergrad sub student;
-        postgrad sub student;
-        
-        teacher sub person;
-        supervisor sub teacher;
-        professor sub teacher;
-        ```
-        
-        
-        ### N-ary Relations
-        
-        In the real world, relations aren't just binary connections between two things. In rich systems, we often need to capture three or more things related with each other at once. Representing them as separate binary relationships would lose information. TypeQL can naturally represent arbitrary number of things as one relation.
-        
-        ```typeql
-        match
-         
-        $person isa person, has name "Leonardo";
-        $character isa character, has name "Jack";
-        $movie isa movie;
-        (actor: $person, character: $character, movie: $movie) isa cast;
-        get $movie;
-         
-        answers>>
-         
-        $movie isa movie, has name "Titanic";
-        ```
-        
-        
-        ### Nested Relations
-        
-        Relations are concepts we use to describe the association between two or more things. Sometimes, those things can be relations themselves. TypeQL can represent these structures naturally, as it enables relations to be nested in another relation, allowing you to express the model of your system in the most natural form.
-        
-        ```typeql
-        match
-         
-        $alice isa person, has name "Alice";
-        $bob isa person, has name "Bob";
-        $mar ($alice, $bob) isa marriage;
-        $city isa city;
-        ($mar, $city) isa located;
-         
-        answers>>
-         
-        $city isa city, has name "London";
-        ```
-        
-        
-        ## A higher degree of safety
-        
-        Types provide a way to describe the logical structures of your data, allowing TypeDB to validate that your code inserts and queries data correctly. Query validation goes beyond static type checking, and includes logical validations of meaningless queries. With strict type-checking errors, you have a dataset that you can trust.
-        
-        ### Logical Data Validation
-        
-        Inserted data gets validated beyond static type checking of attribute value types. Entities are validated to only have the correct attributes, and relations are validated to only relate things that are logically allowed. TypeDB performs richer validation of inserted entities and relations by evaluating the polymorphic types of the things involved.
-        
-        ```typeql
-        insert
-        
-        $charlie isa person, has name "Charlie";
-        $dataCo isa company, has name "DataCo";
-        (husband: $charlie, wife: $dataCo) isa marriage; # invalid relation
-        
-        commit>>
-        
-        ERROR: invalid data detected during type validation
-        ```
-        
-        
-        ### Logical Query Validation
-        
-        Read queries executed on TypeDB go through a type resolution process. This process not only optimises the query's execution, but also acts as a static type checker to reject meaningless and unsatisfiable queries, as they are likely a user error.
-        
-        ```typeql
-        match
-        
-        $alice isa person, has name "Alice";
-        $bob isa person, has name "Bob";
-        ($alice, $bob) isa marriage;
-        $dataCo isa company, has name "DataCo";
-        ($bob, $dataCo) isa marriage; # invalid relation
-        
-        answers>>
-        
-        ERROR: unsatisfiable query detected during type resolution
-        ```
-        
-        ## Evolved with logical inference
-        
-        TypeDB encodes your data for logical interpretation by a reasoning engine. It enables type-inference and rule-inference that creates logical abstractions of data. This allows the discovery of facts and patterns that would otherwise be too hard to find; and complex queries become much simpler.
-        
-        ### Rules
-        
-        TypeQL allows you to define rules in your schema. This extends the expressivity of your model as it enables the system to derive new conclusions when a certain logical form in your dataset is satisfied. Like functions in programming, rules can chain onto one another, creating abstractions of behaviour at the data level.
-        
-        ```typeql
-        define
-        
-        rule transitive-location:
-        when {
-          (located: $x, locating: $y);
-          (located: $y, locating: $z);
-        } then {
-          (located: $x, locating: $z);
-        };
-        ```
-        
-        ### Inference
-        
-        TypeDB's inference facility translates one query into all of its possible interpretations. This happens through two mechanisms: type-based and rule-based inference. Not only does this derive new conclusions and uncovers relationships that would otherwise be hidden, but it also enables the abstraction of complex patterns into simple queries.
-        
-        ```typeql
-        match
-        
-        $person isa person;
-        $uk isa country, has name "UK";
-        ($person, $uk) isa location;
-        get $person;
-        
-        answers>>
-        
-        $person isa teacher, has name "Alice";
-        $person isa postgrad, has name "Bob";
-        ```
-        
-        ## Using TypeQL
-        
-        ### TypeQL (native syntax)
-        
-        All TypeDB Clients, as well as TypeDB Console, accept TypeQL syntax natively. If you are using TypeDB, you do not need additional libraries/tools to use TypeQL syntax natively. 
-        
-        ### TypeQL for Java
-        
-        #### Language Library
-        
-        To use a TypeQL language library for Java, to be able to construct queries programmatically as opposed to manual string concatenations, please visit [vaticle/typeql-lang-java](https://github.com/vaticle/typeql-lang-java)
-        
-        #### Grammar
-        
-        If you would like to develop language TypeQL plugins or extension in Java, and require the TypeQL grammar library, you can import the following Maven package.
-        
-        ```xml
-        <repositories>
-            <repository>
-                <id>repo.vaticle.com</id>
-                <url>https://repo.vaticle.com/repository/maven/</url>
-            </repository>
-        </repositories>
-        
-        <dependencies>
-            <dependency>
-                <groupId>com.vaticle.typeql</groupId>
-                <artifactId>typeql-grammar</artifactId>
-                <version>{version}</version>
-            </dependency>
-        </dependencies>
-        ```
-        
-        Replace `{version}` with the version number, in which you can find the latest of TypeQL Grammar on our [Maven Repository](https://repo.vaticle.com/#browse/browse:maven:com%2Fvaticle%2Ftypeql%2Ftypeql-grammar).
-        
-        ## TypeQL for Python
-        
-        #### Language Library
-        
-        To use a TypeQL language library for Python, to be able to construct queries programmatically as opposed to manual string concatenations, please visit [typedb-osi/typeql-lang-python](https://github.com/typedb-osi/typeql-lang-python). The project is still under development by the community. You are welcome to contribute to the project development.
-        
-        #### Grammar
-        
-        If you would like to develop language TypeQL plugins or extension in Python, and require the TypeQL grammar library, you can import the following PyPI package.
-        
-        ```
-        pip install typeql-grammar=={version}
-        ```
-        
-        Replace `{version}` with the version number, in which you can find the latest on [TypeQL's PyPi Page](https://pypi.org/project/typeql-grammar/). 
-        
-        ## Contributions
-        
-        TypeDB & TypeQL has been built using various open-source Graph and Distributed Computing frameworks throughout its evolution. Today TypeDB & TypeQL is built using [RocksDB](https://rocksdb.org), [ANTLR](http://www.antlr.org), [SCIP](https://www.scipopt.org), [Bazel](https://bazel.build), [GRPC](https://grpc.io), and [ZeroMQ](https://zeromq.org), and [Caffeine](https://github.com/ben-manes/caffeine). In the past, TypeDB was enabled by various open-source technologies and communities that we are hugely thankful to: [Apache Cassandra](http://cassandra.apache.org), [Apache Hadoop](https://hadoop.apache.org), [Apache Spark](http://spark.apache.org), [Apache TinkerPop](http://tinkerpop.apache.org), and [JanusGraph](http://janusgraph.org). Thank you!
-        
-        ---
-        
-        ## Licensing
-        
-        The TypeQL language and related materials are distributed under the terms GNU Affero General Public License v3.0 ("AGPL 3.0") as published by the Free Software Foundation, but with the following special exception.
-        
-        Exception to AGPL 3.0: Any TypeQL language library that is based on material or materials in the Vaticle TypeQL repository, and that is used to communicate or interact (in each case) with a database created or managed or accessed (in each case) using a version of the TypeQL software that is made available by or on behalf of Vaticle Limited (UK Company Number 08766237) or any successor entity (but excluding any forked version of that software), may be distributed under one of the following licences:
-        
-        - The Apache License version 2: https://www.apache.org/licenses/LICENSE-2.0.txt
-        - The MIT License: https://opensource.org/licenses/MIT
-        - The BSD License (2-Clause): https://opensource.org/licenses/BSD-2-Clause
-        
-        As used above "successor entity" means any entity then owning copyrights in the TypeDB software that were previously owned by Vaticle Ltd.
-        
-        If you make any change to, or contribute to, (in each case) the TypeQL code or related materials, then this exception will apply to any TypeQL language library that uses or implements that change/contribution.
-        
 Keywords: grakn database graph knowledgebase knowledge-engineering
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -260,7 +18,251 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
+
+[![Grabl](https://grabl.io/api/status/vaticle/typeql/badge.svg)](https://grabl.io/vaticle/typeql)
+[![GitHub release](https://img.shields.io/github/release/vaticle/typeql.svg)](https://github.com/vaticle/typeql/releases/latest)
+[![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://vaticle.com/discord)
+[![Discussion Forum](https://img.shields.io/discourse/https/forum.vaticle.com/topics.svg)](https://forum.vaticle.com)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
+
+# Meet TypeQL (and [TypeDB](https://github.com/vaticle/typedb))
+
+TypeDB is a strongly-typed database with a rich and logical type system. TypeDB empowers you to tackle complex problems, and TypeQL is its query language.
+
+## A higher level of expressivity
+
+TypeQL allows you to model your domain based on logical and object-oriented principles. Composed of entity, relationship, and attribute types, as well as type hierarchies, roles, and rules, TypeQL allows you to think higher-level as opposed to join-tables, columns, documents, vertices, edges, and properties.
+
+### Entity-Relationship Model
+
+TypeQL allows you to model your domain using the well-known Entity-Relationship model. It is composed of entity types, relation types, and attribute types, with the introduction of role types. TypeQL allows you to leverage the full expressivity of the ER model, and describe your schema through first normal form.
+
+```typeql
+define
+
+person sub entity,
+  owns name,
+  plays employment:employee;
+company sub entity,
+  owns name,
+  plays employment:employer;
+employment sub relation,
+  relates employee,
+  relates employer;
+name sub attribute,
+  value string;
+```
+
+### Type Hierarchies
+
+TypeQL allows you to easily model type inheritance into your domain model. Following logical and object-oriented principle, TypeQL allows data types to inherit the behaviours and properties of their supertypes. Complex data structures become reusable, and data interpretation becomes richer through polymorphism.
+
+```typeql
+define
+
+person sub entity,
+  owns first-name,
+  owns last-name;
+
+student sub person;
+undergrad sub student;
+postgrad sub student;
+
+teacher sub person;
+supervisor sub teacher;
+professor sub teacher;
+```
+
+
+### N-ary Relations
+
+In the real world, relations aren't just binary connections between two things. In rich systems, we often need to capture three or more things related with each other at once. Representing them as separate binary relationships would lose information. TypeQL can naturally represent arbitrary number of things as one relation.
+
+```typeql
+match
+ 
+$person isa person, has name "Leonardo";
+$character isa character, has name "Jack";
+$movie isa movie;
+(actor: $person, character: $character, movie: $movie) isa cast;
+get $movie;
+ 
+answers>>
+ 
+$movie isa movie, has name "Titanic";
+```
+
+
+### Nested Relations
+
+Relations are concepts we use to describe the association between two or more things. Sometimes, those things can be relations themselves. TypeQL can represent these structures naturally, as it enables relations to be nested in another relation, allowing you to express the model of your system in the most natural form.
+
+```typeql
+match
+ 
+$alice isa person, has name "Alice";
+$bob isa person, has name "Bob";
+$mar ($alice, $bob) isa marriage;
+$city isa city;
+($mar, $city) isa located;
+ 
+answers>>
+ 
+$city isa city, has name "London";
+```
+
+
+## A higher degree of safety
+
+Types provide a way to describe the logical structures of your data, allowing TypeDB to validate that your code inserts and queries data correctly. Query validation goes beyond static type checking, and includes logical validations of meaningless queries. With strict type-checking errors, you have a dataset that you can trust.
+
+### Logical Data Validation
+
+Inserted data gets validated beyond static type checking of attribute value types. Entities are validated to only have the correct attributes, and relations are validated to only relate things that are logically allowed. TypeDB performs richer validation of inserted entities and relations by evaluating the polymorphic types of the things involved.
+
+```typeql
+insert
+
+$charlie isa person, has name "Charlie";
+$dataCo isa company, has name "DataCo";
+(husband: $charlie, wife: $dataCo) isa marriage; # invalid relation
+
+commit>>
+
+ERROR: invalid data detected during type validation
+```
+
+
+### Logical Query Validation
+
+Read queries executed on TypeDB go through a type resolution process. This process not only optimises the query's execution, but also acts as a static type checker to reject meaningless and unsatisfiable queries, as they are likely a user error.
+
+```typeql
+match
+
+$alice isa person, has name "Alice";
+$bob isa person, has name "Bob";
+($alice, $bob) isa marriage;
+$dataCo isa company, has name "DataCo";
+($bob, $dataCo) isa marriage; # invalid relation
+
+answers>>
+
+ERROR: unsatisfiable query detected during type resolution
+```
+
+## Evolved with logical inference
+
+TypeDB encodes your data for logical interpretation by a reasoning engine. It enables type-inference and rule-inference that creates logical abstractions of data. This allows the discovery of facts and patterns that would otherwise be too hard to find; and complex queries become much simpler.
+
+### Rules
+
+TypeQL allows you to define rules in your schema. This extends the expressivity of your model as it enables the system to derive new conclusions when a certain logical form in your dataset is satisfied. Like functions in programming, rules can chain onto one another, creating abstractions of behaviour at the data level.
+
+```typeql
+define
+
+rule transitive-location:
+when {
+  (located: $x, locating: $y);
+  (located: $y, locating: $z);
+} then {
+  (located: $x, locating: $z);
+};
+```
+
+### Inference
+
+TypeDB's inference facility translates one query into all of its possible interpretations. This happens through two mechanisms: type-based and rule-based inference. Not only does this derive new conclusions and uncovers relationships that would otherwise be hidden, but it also enables the abstraction of complex patterns into simple queries.
+
+```typeql
+match
+
+$person isa person;
+$uk isa country, has name "UK";
+($person, $uk) isa location;
+get $person;
+
+answers>>
+
+$person isa teacher, has name "Alice";
+$person isa postgrad, has name "Bob";
+```
+
+## Using TypeQL
+
+### TypeQL (native syntax)
+
+All TypeDB Clients, as well as TypeDB Console, accept TypeQL syntax natively. If you are using TypeDB, you do not need additional libraries/tools to use TypeQL syntax natively. 
+
+### TypeQL for Java
+
+#### Language Library
+
+To use a TypeQL language library for Java, to be able to construct queries programmatically as opposed to manual string concatenations, please visit [vaticle/typeql-lang-java](https://github.com/vaticle/typeql-lang-java)
+
+#### Grammar
+
+If you would like to develop language TypeQL plugins or extension in Java, and require the TypeQL grammar library, you can import the following Maven package.
+
+```xml
+<repositories>
+    <repository>
+        <id>repo.vaticle.com</id>
+        <url>https://repo.vaticle.com/repository/maven/</url>
+    </repository>
+</repositories>
+
+<dependencies>
+    <dependency>
+        <groupId>com.vaticle.typeql</groupId>
+        <artifactId>typeql-grammar</artifactId>
+        <version>{version}</version>
+    </dependency>
+</dependencies>
+```
+
+Replace `{version}` with the version number, in which you can find the latest of TypeQL Grammar on our [Maven Repository](https://repo.vaticle.com/#browse/browse:maven:com%2Fvaticle%2Ftypeql%2Ftypeql-grammar).
+
+## TypeQL for Python
+
+#### Language Library
+
+To use a TypeQL language library for Python, to be able to construct queries programmatically as opposed to manual string concatenations, please visit [typedb-osi/typeql-lang-python](https://github.com/typedb-osi/typeql-lang-python). The project is still under development by the community. You are welcome to contribute to the project development.
+
+#### Grammar
+
+If you would like to develop language TypeQL plugins or extension in Python, and require the TypeQL grammar library, you can import the following PyPI package.
+
+```
+pip install typeql-grammar=={version}
+```
+
+Replace `{version}` with the version number, in which you can find the latest on [TypeQL's PyPi Page](https://pypi.org/project/typeql-grammar/). 
+
+## Contributions
+
+TypeDB & TypeQL has been built using various open-source Graph and Distributed Computing frameworks throughout its evolution. Today TypeDB & TypeQL is built using [RocksDB](https://rocksdb.org), [ANTLR](http://www.antlr.org), [SCIP](https://www.scipopt.org), [Bazel](https://bazel.build), [GRPC](https://grpc.io), and [ZeroMQ](https://zeromq.org), and [Caffeine](https://github.com/ben-manes/caffeine). In the past, TypeDB was enabled by various open-source technologies and communities that we are hugely thankful to: [Apache Cassandra](http://cassandra.apache.org), [Apache Hadoop](https://hadoop.apache.org), [Apache Spark](http://spark.apache.org), [Apache TinkerPop](http://tinkerpop.apache.org), and [JanusGraph](http://janusgraph.org). Thank you!
+
+---
+
+## Licensing
+
+The TypeQL language and related materials are distributed under the terms GNU Affero General Public License v3.0 ("AGPL 3.0") as published by the Free Software Foundation, but with the following special exception.
+
+Exception to AGPL 3.0: Any TypeQL language library that is based on material or materials in the Vaticle TypeQL repository, and that is used to communicate or interact (in each case) with a database created or managed or accessed (in each case) using a version of the TypeQL software that is made available by or on behalf of Vaticle Limited (UK Company Number 08766237) or any successor entity (but excluding any forked version of that software), may be distributed under one of the following licences:
+
+- The Apache License version 2: https://www.apache.org/licenses/LICENSE-2.0.txt
+- The MIT License: https://opensource.org/licenses/MIT
+- The BSD License (2-Clause): https://opensource.org/licenses/BSD-2-Clause
+
+As used above "successor entity" means any entity then owning copyrights in the TypeDB software that were previously owned by Vaticle Ltd.
+
+If you make any change to, or contribute to, (in each case) the TypeQL code or related materials, then this exception will apply to any TypeQL language library that uses or implements that change/contribution.
+
+
```

