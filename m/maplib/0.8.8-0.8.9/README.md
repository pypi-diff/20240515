# Comparing `tmp/maplib-0.8.8.tar.gz` & `tmp/maplib-0.8.9.tar.gz`

## Comparing `maplib-0.8.8.tar` & `maplib-0.8.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0     1001      127      183 2024-04-23 08:08:23.000000 maplib-0.8.8/parquet_io/Cargo.toml
--rw-r--r--   0     1001      127     2881 2024-04-23 08:08:23.000000 maplib-0.8.8/parquet_io/src/lib.rs
--rw-r--r--   0     1001      127      876 2024-04-23 08:08:23.000000 maplib-0.8.8/Cargo.toml
--rw-r--r--   0     1001      127     1033 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/Cargo.toml
--rw-r--r--   0     1001      127    11726 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/ast.rs
--rw-r--r--   0     1001      127      925 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/constants.rs
--rw-r--r--   0     1001      127      635 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/document.rs
--rw-r--r--   0     1001      127      293 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/errors.rs
--rw-r--r--   0     1001      127      244 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/lib.rs
--rw-r--r--   0     1001      127     6449 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/mapping/constant_terms.rs
--rw-r--r--   0     1001      127     6094 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/mapping/default.rs
--rw-r--r--   0     1001      127     5734 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/mapping/errors.rs
--rw-r--r--   0     1001      127     5074 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/mapping/validation_inference.rs
--rw-r--r--   0     1001      127    25483 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/mapping.rs
--rw-r--r--   0     1001      127      800 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/parsing/errors.rs
--rw-r--r--   0     1001      127   191162 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/parsing/nom_parsing.rs
--rw-r--r--   0     1001      127    60674 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/parsing/parser_test.rs
--rw-r--r--   0     1001      127     2812 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/parsing/parsing_ast.rs
--rw-r--r--   0     1001      127      808 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/parsing.rs
--rw-r--r--   0     1001      127    13035 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/resolver.rs
--rw-r--r--   0     1001      127     1963 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/templates/errors.rs
--rw-r--r--   0     1001      127    11029 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/src/templates.rs
--rw-r--r--   0     1001      127        8 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/tests/stottr_testdata/.gitignore
--rw-r--r--   0     1001      127      462 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/tests/stottr_testdata/expected_easy_case.ttl
--rw-r--r--   0     1001      127    37941 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/tests/test_stottr.rs
--rw-r--r--   0     1001      127     1361 2024-04-23 08:08:23.000000 maplib-0.8.8/maplib/tests/utils.rs
--rw-r--r--   0     1001      127      212 2024-04-23 08:08:23.000000 maplib-0.8.8/shacl/Cargo.toml
--rw-r--r--   0     1001      127       70 2024-04-23 08:08:23.000000 maplib-0.8.8/shacl/src/errors.rs
--rw-r--r--   0     1001      127      455 2024-04-23 08:08:23.000000 maplib-0.8.8/shacl/src/lib.rs
--rw-r--r--   0     1001      127     1128 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/Cargo.toml
--rw-r--r--   0     1001      127      391 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/constants.rs
--rw-r--r--   0     1001      127     3823 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/conversion.rs
--rw-r--r--   0     1001      127     2691 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/errors.rs
--rw-r--r--   0     1001      127     9279 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/export_triples.rs
--rw-r--r--   0     1001      127      958 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/io_funcs.rs
--rw-r--r--   0     1001      127    20676 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/lib.rs
--rw-r--r--   0     1001      127     2353 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/native_parquet_write.rs
--rw-r--r--   0     1001      127    11265 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/ntriples_write.rs
--rw-r--r--   0     1001      127      496 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/rdfs_inferencing.rs
--rw-r--r--   0     1001      127      865 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/errors.rs
--rw-r--r--   0     1001      127     5904 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_aggregate.rs
--rw-r--r--   0     1001      127    17100 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_expressions.rs
--rw-r--r--   0     1001      127      939 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/distinct.rs
--rw-r--r--   0     1001      127     1407 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/extend.rs
--rw-r--r--   0     1001      127     1299 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/filter.rs
--rw-r--r--   0     1001      127     2400 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/group.rs
--rw-r--r--   0     1001      127     1172 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/join.rs
--rw-r--r--   0     1001      127     2113 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/left_join.rs
--rw-r--r--   0     1001      127     2270 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/load_tt.rs
--rw-r--r--   0     1001      127     1204 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/minus.rs
--rw-r--r--   0     1001      127     2091 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/order_by.rs
--rw-r--r--   0     1001      127    28820 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/path.rs
--rw-r--r--   0     1001      127     1055 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/project.rs
--rw-r--r--   0     1001      127     1742 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/pvalues.rs
--rw-r--r--   0     1001      127    17085 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/triple.rs
--rw-r--r--   0     1001      127     1245 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/union.rs
--rw-r--r--   0     1001      127     3927 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/values.rs
--rw-r--r--   0     1001      127     5571 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns.rs
--rw-r--r--   0     1001      127     1316 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql/lazy_order.rs
--rw-r--r--   0     1001      127    10582 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/sparql.rs
--rw-r--r--   0     1001      127     9779 2024-04-23 08:08:23.000000 maplib-0.8.8/triplestore/src/triples_read.rs
--rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 maplib-0.8.8/py_maplib/Cargo.toml
--rw-r--r--   0     1001      127      391 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/.gitignore
--rw-r--r--   0     1001      127    11459 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/LICENSE
--rw-r--r--   0     1001      127     6021 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/README.md
--rw-r--r--   0     1001      127       11 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/doc/.gitignore
--rw-r--r--   0     1001      127     1731 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/doc/API.md
--rw-r--r--   0     1001      127    13686 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/doc/rds_mapping.ipynb
--rw-r--r--   0     1001      127       22 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/python/maplib/.gitignore
--rw-r--r--   0     1001      127      127 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/python/maplib/__init__.py
--rw-r--r--   0     1001      127     8963 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/python/maplib/_maplib.pyi
--rw-r--r--   0     1001      127        0 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/python/maplib/py.typed
--rw-r--r--   0     1001      127     3499 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/src/error.rs
--rw-r--r--   0     1001      127    15049 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/src/lib.rs
--rw-r--r--   0     1001      127      138 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/.gitignore
--rw-r--r--   0     1001      127       72 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/out.ttl
--rw-r--r--   0     1001      127       20 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/requirements.txt
--rw-r--r--   0     1001      127     4994 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/test_basics.py
--rw-r--r--   0     1001      127     5901 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/test_blank_nodes_multi.py
--rw-r--r--   0     1001      127    18343 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/test_gtfs_benchmark.py
--rw-r--r--   0     1001      127    16847 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/test_integration.py
--rw-r--r--   0     1001      127     3367 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/test_pizza_example.py
--rw-r--r--   0     1001      127     1550 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/test_read.py
--rw-r--r--   0     1001      127       24 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/iterated_property_path_constant_object_query.csv
--rw-r--r--   0     1001      127     2935 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/iterated_property_path_constant_subject_query.csv
--rw-r--r--   0     1001      127    13780 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/iterated_property_path_query.csv
--rw-r--r--   0     1001      127     4813 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/iterated_property_path_query_with_bug.csv
--rw-r--r--   0     1001      127      122 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/larger_query.csv
--rw-r--r--   0     1001      127       88 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/multi_datatype_join_query.csv
--rw-r--r--   0     1001      127       48 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/multi_datatype_join_query_two_vars.csv
--rw-r--r--   0     1001      127       48 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/multi_datatype_leftjoin_query.csv
--rw-r--r--   0     1001      127      644 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/multi_datatype_query.csv
--rw-r--r--   0     1001      127      644 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/multi_datatype_query_sorting.csv
--rw-r--r--   0     1001      127      166 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/multi_datatype_union_query.csv
--rw-r--r--   0     1001      127     3247 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/property_path_query.csv
--rw-r--r--   0     1001      127      660 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/read_ntriples.csv
--rw-r--r--   0     1001      127      638 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/read_ntriples.nt
--rw-r--r--   0     1001      127      498 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/read_ntriples2.csv
--rw-r--r--   0     1001      127      757 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/simple_construct_query_nothing.csv
--rw-r--r--   0     1001      127    28024 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/simple_construct_query_something.csv
--rw-r--r--   0     1001      127      259 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/simple_insert_query_nothing.csv
--rw-r--r--   0     1001      127    11934 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/simple_insert_query_something.csv
--rw-r--r--   0     1001      127     3327 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/simple_property_path_query.csv
--rw-r--r--   0     1001      127    20308 2024-04-23 08:08:23.000000 maplib-0.8.8/py_maplib/tests/testdata/simple_query.csv
--rw-r--r--   0     1001      127    66654 2024-04-23 08:08:55.000000 maplib-0.8.8/py_maplib/Cargo.lock
--rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 maplib-0.8.8/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-23 08:08:23.000000 maplib-0.8.8/python/maplib/py.typed
--rw-r--r--   0     1001      127     8963 2024-04-23 08:08:23.000000 maplib-0.8.8/python/maplib/_maplib.pyi
--rw-r--r--   0     1001      127      127 2024-04-23 08:08:23.000000 maplib-0.8.8/python/maplib/__init__.py
--rw-r--r--   0     1001      127     6021 2024-04-23 08:08:23.000000 maplib-0.8.8/README.md
--rw-r--r--   0     1001      127    11459 2024-04-23 08:08:23.000000 maplib-0.8.8/LICENSE
--rw-r--r--   0        0        0     7224 1970-01-01 00:00:00.000000 maplib-0.8.8/PKG-INFO
+-rw-r--r--   0     1001      127     1033 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/Cargo.toml
+-rw-r--r--   0     1001      127    11726 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/ast.rs
+-rw-r--r--   0     1001      127      925 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/constants.rs
+-rw-r--r--   0     1001      127      635 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/document.rs
+-rw-r--r--   0     1001      127      293 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/errors.rs
+-rw-r--r--   0     1001      127      244 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/lib.rs
+-rw-r--r--   0     1001      127     6449 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/mapping/constant_terms.rs
+-rw-r--r--   0     1001      127     6094 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/mapping/default.rs
+-rw-r--r--   0     1001      127     5734 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/mapping/errors.rs
+-rw-r--r--   0     1001      127     5074 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/mapping/validation_inference.rs
+-rw-r--r--   0     1001      127    25483 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/mapping.rs
+-rw-r--r--   0     1001      127      800 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/parsing/errors.rs
+-rw-r--r--   0     1001      127   191162 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/parsing/nom_parsing.rs
+-rw-r--r--   0     1001      127    60674 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/parsing/parser_test.rs
+-rw-r--r--   0     1001      127     2812 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/parsing/parsing_ast.rs
+-rw-r--r--   0     1001      127      808 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/parsing.rs
+-rw-r--r--   0     1001      127    13035 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/resolver.rs
+-rw-r--r--   0     1001      127     1963 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/templates/errors.rs
+-rw-r--r--   0     1001      127    11029 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/src/templates.rs
+-rw-r--r--   0     1001      127        8 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/tests/stottr_testdata/.gitignore
+-rw-r--r--   0     1001      127      462 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/tests/stottr_testdata/expected_easy_case.ttl
+-rw-r--r--   0     1001      127    37941 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/tests/test_stottr.rs
+-rw-r--r--   0     1001      127     1361 2024-04-23 08:54:22.000000 maplib-0.8.9/maplib/tests/utils.rs
+-rw-r--r--   0     1001      127      876 2024-04-23 08:54:22.000000 maplib-0.8.9/Cargo.toml
+-rw-r--r--   0     1001      127      183 2024-04-23 08:54:22.000000 maplib-0.8.9/parquet_io/Cargo.toml
+-rw-r--r--   0     1001      127     2881 2024-04-23 08:54:22.000000 maplib-0.8.9/parquet_io/src/lib.rs
+-rw-r--r--   0     1001      127     1128 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/Cargo.toml
+-rw-r--r--   0     1001      127      391 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/constants.rs
+-rw-r--r--   0     1001      127     3823 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/conversion.rs
+-rw-r--r--   0     1001      127     2691 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/errors.rs
+-rw-r--r--   0     1001      127     9279 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/export_triples.rs
+-rw-r--r--   0     1001      127      958 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/io_funcs.rs
+-rw-r--r--   0     1001      127    20676 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/lib.rs
+-rw-r--r--   0     1001      127     2353 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/native_parquet_write.rs
+-rw-r--r--   0     1001      127    11265 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/ntriples_write.rs
+-rw-r--r--   0     1001      127      496 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/rdfs_inferencing.rs
+-rw-r--r--   0     1001      127      865 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/errors.rs
+-rw-r--r--   0     1001      127     5904 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_aggregate.rs
+-rw-r--r--   0     1001      127    17100 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_expressions.rs
+-rw-r--r--   0     1001      127      939 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/distinct.rs
+-rw-r--r--   0     1001      127     1407 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/extend.rs
+-rw-r--r--   0     1001      127     1299 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/filter.rs
+-rw-r--r--   0     1001      127     2400 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/group.rs
+-rw-r--r--   0     1001      127     1172 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/join.rs
+-rw-r--r--   0     1001      127     2113 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/left_join.rs
+-rw-r--r--   0     1001      127     2270 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/load_tt.rs
+-rw-r--r--   0     1001      127     1204 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/minus.rs
+-rw-r--r--   0     1001      127     2091 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/order_by.rs
+-rw-r--r--   0     1001      127    28820 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/path.rs
+-rw-r--r--   0     1001      127     1055 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/project.rs
+-rw-r--r--   0     1001      127     1742 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/pvalues.rs
+-rw-r--r--   0     1001      127    17085 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/triple.rs
+-rw-r--r--   0     1001      127     1245 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/union.rs
+-rw-r--r--   0     1001      127     3927 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/values.rs
+-rw-r--r--   0     1001      127     5571 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns.rs
+-rw-r--r--   0     1001      127     1316 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql/lazy_order.rs
+-rw-r--r--   0     1001      127    10582 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/sparql.rs
+-rw-r--r--   0     1001      127     9779 2024-04-23 08:54:22.000000 maplib-0.8.9/triplestore/src/triples_read.rs
+-rw-r--r--   0     1001      127      212 2024-04-23 08:54:22.000000 maplib-0.8.9/shacl/Cargo.toml
+-rw-r--r--   0     1001      127       70 2024-04-23 08:54:22.000000 maplib-0.8.9/shacl/src/errors.rs
+-rw-r--r--   0     1001      127      455 2024-04-23 08:54:22.000000 maplib-0.8.9/shacl/src/lib.rs
+-rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 maplib-0.8.9/py_maplib/Cargo.toml
+-rw-r--r--   0     1001      127      391 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/.gitignore
+-rw-r--r--   0     1001      127    11459 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/LICENSE
+-rw-r--r--   0     1001      127     6021 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/README.md
+-rw-r--r--   0     1001      127       11 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/doc/.gitignore
+-rw-r--r--   0     1001      127     1731 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/doc/API.md
+-rw-r--r--   0     1001      127    13686 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/doc/rds_mapping.ipynb
+-rw-r--r--   0     1001      127       22 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/python/maplib/.gitignore
+-rw-r--r--   0     1001      127      127 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/python/maplib/__init__.py
+-rw-r--r--   0     1001      127     8963 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/python/maplib/_maplib.pyi
+-rw-r--r--   0     1001      127        0 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/python/maplib/py.typed
+-rw-r--r--   0     1001      127     3499 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/src/error.rs
+-rw-r--r--   0     1001      127    15049 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/src/lib.rs
+-rw-r--r--   0     1001      127      138 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/.gitignore
+-rw-r--r--   0     1001      127       72 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/out.ttl
+-rw-r--r--   0     1001      127       20 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/requirements.txt
+-rw-r--r--   0     1001      127     4994 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/test_basics.py
+-rw-r--r--   0     1001      127     5901 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/test_blank_nodes_multi.py
+-rw-r--r--   0     1001      127    18343 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/test_gtfs_benchmark.py
+-rw-r--r--   0     1001      127    16847 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/test_integration.py
+-rw-r--r--   0     1001      127     3367 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/test_pizza_example.py
+-rw-r--r--   0     1001      127     1550 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/test_read.py
+-rw-r--r--   0     1001      127       24 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/iterated_property_path_constant_object_query.csv
+-rw-r--r--   0     1001      127     2935 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/iterated_property_path_constant_subject_query.csv
+-rw-r--r--   0     1001      127    13780 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/iterated_property_path_query.csv
+-rw-r--r--   0     1001      127     4813 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/iterated_property_path_query_with_bug.csv
+-rw-r--r--   0     1001      127      122 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/larger_query.csv
+-rw-r--r--   0     1001      127       88 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/multi_datatype_join_query.csv
+-rw-r--r--   0     1001      127       48 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/multi_datatype_join_query_two_vars.csv
+-rw-r--r--   0     1001      127       48 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/multi_datatype_leftjoin_query.csv
+-rw-r--r--   0     1001      127      644 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/multi_datatype_query.csv
+-rw-r--r--   0     1001      127      644 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/multi_datatype_query_sorting.csv
+-rw-r--r--   0     1001      127      166 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/multi_datatype_union_query.csv
+-rw-r--r--   0     1001      127     3247 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/property_path_query.csv
+-rw-r--r--   0     1001      127      660 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/read_ntriples.csv
+-rw-r--r--   0     1001      127      638 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/read_ntriples.nt
+-rw-r--r--   0     1001      127      498 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/read_ntriples2.csv
+-rw-r--r--   0     1001      127      757 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/simple_construct_query_nothing.csv
+-rw-r--r--   0     1001      127    28024 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/simple_construct_query_something.csv
+-rw-r--r--   0     1001      127      259 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/simple_insert_query_nothing.csv
+-rw-r--r--   0     1001      127    11934 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/simple_insert_query_something.csv
+-rw-r--r--   0     1001      127     3327 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/simple_property_path_query.csv
+-rw-r--r--   0     1001      127    20308 2024-04-23 08:54:22.000000 maplib-0.8.9/py_maplib/tests/testdata/simple_query.csv
+-rw-r--r--   0     1001      127    66654 2024-04-23 08:54:52.000000 maplib-0.8.9/py_maplib/Cargo.lock
+-rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 maplib-0.8.9/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-23 08:54:22.000000 maplib-0.8.9/python/maplib/py.typed
+-rw-r--r--   0     1001      127     8963 2024-04-23 08:54:22.000000 maplib-0.8.9/python/maplib/_maplib.pyi
+-rw-r--r--   0     1001      127      127 2024-04-23 08:54:22.000000 maplib-0.8.9/python/maplib/__init__.py
+-rw-r--r--   0     1001      127     6021 2024-04-23 08:54:22.000000 maplib-0.8.9/README.md
+-rw-r--r--   0     1001      127    11459 2024-04-23 08:54:22.000000 maplib-0.8.9/LICENSE
+-rw-r--r--   0        0        0     7224 1970-01-01 00:00:00.000000 maplib-0.8.9/PKG-INFO
```

### Comparing `maplib-0.8.8/parquet_io/src/lib.rs` & `maplib-0.8.9/parquet_io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/Cargo.toml` & `maplib-0.8.9/Cargo.toml`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/Cargo.toml` & `maplib-0.8.9/maplib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/ast.rs` & `maplib-0.8.9/maplib/src/ast.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/constants.rs` & `maplib-0.8.9/maplib/src/constants.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/document.rs` & `maplib-0.8.9/maplib/src/document.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/mapping/constant_terms.rs` & `maplib-0.8.9/maplib/src/mapping/constant_terms.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/mapping/default.rs` & `maplib-0.8.9/maplib/src/mapping/default.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/mapping/errors.rs` & `maplib-0.8.9/maplib/src/mapping/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/mapping/validation_inference.rs` & `maplib-0.8.9/maplib/src/mapping/validation_inference.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/mapping.rs` & `maplib-0.8.9/maplib/src/mapping.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/parsing/errors.rs` & `maplib-0.8.9/maplib/src/parsing/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/parsing/nom_parsing.rs` & `maplib-0.8.9/maplib/src/parsing/nom_parsing.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/parsing/parser_test.rs` & `maplib-0.8.9/maplib/src/parsing/parser_test.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/parsing/parsing_ast.rs` & `maplib-0.8.9/maplib/src/parsing/parsing_ast.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/parsing.rs` & `maplib-0.8.9/maplib/src/parsing.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/resolver.rs` & `maplib-0.8.9/maplib/src/resolver.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/templates/errors.rs` & `maplib-0.8.9/maplib/src/templates/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/src/templates.rs` & `maplib-0.8.9/maplib/src/templates.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/tests/test_stottr.rs` & `maplib-0.8.9/maplib/tests/test_stottr.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/maplib/tests/utils.rs` & `maplib-0.8.9/maplib/tests/utils.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/Cargo.toml` & `maplib-0.8.9/triplestore/Cargo.toml`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/conversion.rs` & `maplib-0.8.9/triplestore/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/errors.rs` & `maplib-0.8.9/triplestore/src/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/export_triples.rs` & `maplib-0.8.9/triplestore/src/export_triples.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/io_funcs.rs` & `maplib-0.8.9/triplestore/src/io_funcs.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/lib.rs` & `maplib-0.8.9/triplestore/src/lib.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/native_parquet_write.rs` & `maplib-0.8.9/triplestore/src/native_parquet_write.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/ntriples_write.rs` & `maplib-0.8.9/triplestore/src/ntriples_write.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/errors.rs` & `maplib-0.8.9/triplestore/src/sparql/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_aggregate.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_aggregate.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_expressions.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_expressions.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/distinct.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/distinct.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/extend.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/extend.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/filter.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/filter.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/group.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/group.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/join.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/join.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/left_join.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/left_join.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/load_tt.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/load_tt.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/minus.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/minus.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/order_by.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/order_by.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/path.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/path.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/project.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/project.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/pvalues.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/pvalues.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/triple.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/triple.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/union.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/union.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns/values.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns/values.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_graph_patterns.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_graph_patterns.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql/lazy_order.rs` & `maplib-0.8.9/triplestore/src/sparql/lazy_order.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/sparql.rs` & `maplib-0.8.9/triplestore/src/sparql.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/triplestore/src/triples_read.rs` & `maplib-0.8.9/triplestore/src/triples_read.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/Cargo.toml` & `maplib-0.8.9/py_maplib/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py_maplib"
-version = "0.8.8"
+version = "0.8.9"
 edition = "2021"
 
 [workspace]
 
 [dependencies]
 pyo3 = {version = "0.21.1", features = ["extension-module"] }
 maplib = {path="../maplib"}
```

### Comparing `maplib-0.8.8/py_maplib/LICENSE` & `maplib-0.8.9/py_maplib/LICENSE`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/README.md` & `maplib-0.8.9/py_maplib/README.md`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/doc/API.md` & `maplib-0.8.9/py_maplib/doc/API.md`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/doc/rds_mapping.ipynb` & `maplib-0.8.9/py_maplib/doc/rds_mapping.ipynb`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/python/maplib/_maplib.pyi` & `maplib-0.8.9/py_maplib/python/maplib/_maplib.pyi`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/src/error.rs` & `maplib-0.8.9/py_maplib/src/error.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/src/lib.rs` & `maplib-0.8.9/py_maplib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/test_basics.py` & `maplib-0.8.9/py_maplib/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/test_blank_nodes_multi.py` & `maplib-0.8.9/py_maplib/tests/test_blank_nodes_multi.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/test_gtfs_benchmark.py` & `maplib-0.8.9/py_maplib/tests/test_gtfs_benchmark.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/test_integration.py` & `maplib-0.8.9/py_maplib/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/test_pizza_example.py` & `maplib-0.8.9/py_maplib/tests/test_pizza_example.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/test_read.py` & `maplib-0.8.9/py_maplib/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/iterated_property_path_constant_subject_query.csv` & `maplib-0.8.9/py_maplib/tests/testdata/iterated_property_path_constant_subject_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/iterated_property_path_query.csv` & `maplib-0.8.9/py_maplib/tests/testdata/iterated_property_path_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/iterated_property_path_query_with_bug.csv` & `maplib-0.8.9/py_maplib/tests/testdata/iterated_property_path_query_with_bug.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/multi_datatype_query.csv` & `maplib-0.8.9/py_maplib/tests/testdata/multi_datatype_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/multi_datatype_query_sorting.csv` & `maplib-0.8.9/py_maplib/tests/testdata/multi_datatype_query_sorting.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/property_path_query.csv` & `maplib-0.8.9/py_maplib/tests/testdata/property_path_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/read_ntriples.csv` & `maplib-0.8.9/py_maplib/tests/testdata/read_ntriples.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/read_ntriples.nt` & `maplib-0.8.9/py_maplib/tests/testdata/read_ntriples.nt`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/simple_construct_query_nothing.csv` & `maplib-0.8.9/py_maplib/tests/testdata/simple_construct_query_nothing.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/simple_construct_query_something.csv` & `maplib-0.8.9/py_maplib/tests/testdata/simple_construct_query_something.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/simple_insert_query_something.csv` & `maplib-0.8.9/py_maplib/tests/testdata/simple_insert_query_something.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/simple_property_path_query.csv` & `maplib-0.8.9/py_maplib/tests/testdata/simple_property_path_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/tests/testdata/simple_query.csv` & `maplib-0.8.9/py_maplib/tests/testdata/simple_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/py_maplib/Cargo.lock` & `maplib-0.8.9/py_maplib/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1677,15 +1677,15 @@
 checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_maplib"
-version = "0.8.8"
+version = "0.8.9"
 dependencies = [
  "jemallocator",
  "log",
  "maplib",
  "mimalloc",
  "oxrdf",
  "polars",
```

### Comparing `maplib-0.8.8/pyproject.toml` & `maplib-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/python/maplib/_maplib.pyi` & `maplib-0.8.9/python/maplib/_maplib.pyi`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/README.md` & `maplib-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/LICENSE` & `maplib-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maplib-0.8.8/PKG-INFO` & `maplib-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: maplib
-Version: 0.8.8
+Version: 0.8.9
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

